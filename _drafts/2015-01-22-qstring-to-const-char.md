---
layout:     post
title:      "Converting QString to const char *"
date:       2015-01-22 17:00:00
category:   code
tags:       qt c++
---

QString filename("/some/path/to/my/filename");
const char *f = filename.toStdString().c_str();

http://stackoverflow.com/questions/5837442/why-is-this-qstring-to-const-char-conversion-producing-a-debian-identifier-on-w

<!--break-->

This code:

const char* username = inUsername.toLocal8Bit().data();
is equivalent to this:

const char * username;
{
    const QByteArray l8b = inUsername.toLocal8Bit();
    username = l8b.data();
}
Do you see what's going on? By the time the statement has executed, the temporary QByteArray has been deleted by the compiler again. Since data() only returns a pointer to the internal QByteArray buffer, username now points to deleted/freed memory.

To solve the problem, make username and password QByteArrays instead of const char*s, and use username.data(), password.data() instead where you used username, password before.
