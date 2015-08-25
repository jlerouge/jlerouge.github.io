---
layout:     publication
title:      "IODA: An input/output deep architecture for image labeling"
date:       2015-03-18 12:00:00
category:   publication
tags:
    - neural networks
    - deep learning
    - medical imaging
authors:
    - jl@litis-insa
    - rh@litis-insa
    - cc@litis-insa
    - fj@hematology-becquerel
    - rm@nuclear-becquerel,litis-insa
refs: Pattern Recognition, vol. 48, iss. 9, pp. 2847-2858, 2015
doi: 10.1016/j.patcog.2015.03.017
pdf: true
bibtex: true
---

In this paper, we propose a deep neural network (DNN) architecture called Input Output Deep Architecture (IODA) for solving the problem of image labeling. IODA directly links a whole image to a whole label map, assigning a label to each pixel using a single neural network forward step.

Instead of designing a handcrafted a priori model on labels (such as an atlas in the medical domain), we propose to automatically learn the dependencies between labels. The originality of IODA is to transpose DNN input pre-training trick to the output space, in order to learn a high level representation of labels. It allows a fast image labeling inside a fully neural network framework, without the need of any preprocessing such as feature designing or output coding.

In this paper, IODA is applied on both a toy texture problem and a real-world medical image dataset, showing promising results. We provide an open source implementation of IODA.
