---
layout:     post
title:      "Managing multiple SSH identities"
date:       2014-12-17 17:17:00
category:   linux
tags:		ssh security
---

What's my username on that server ?
Now that you've remembered your username (say `remoteuser`), you need to figure out the associated password. Ooh-oh.

<!--break-->

{% highlight bash %}
me@localhost ~ $ ssh -i path/to/private/key remoteuser@remotehost
me@localhost ~ $ Password: ********
{% endhighlight %}
