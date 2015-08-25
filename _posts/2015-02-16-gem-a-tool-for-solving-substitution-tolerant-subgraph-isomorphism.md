---
layout:     publication
title:      "GEM++: A Tool for Solving Substitution-Tolerant Subgraph Isomorphism"
date:       2015-02-16 12:00:00
category:   publication
tags:
    - graph matching
    - binary linear programming
    - symbol spotting
authors:
    - jl@litis-univ-rouen
    - plb@isye-gatech
    - ph@litis-univ-rouen
    - sa@litis-univ-rouen
refs: "Proceedings of Graph-Based Representations in Pattern Recognition: 10th IAPR-TC-15 International Workshop, GbRPR 2015, Beijing, China, May 13-15, 2015. Lecture Notes in Computer Science Vol. 9069. Springer, 2015"
doi: 10.1007/978-3-319-18224-7_13
pdf: true
bibtex: true
---

The substitution-tolerant subgraph isomorphism is a particular error-tolerant subgraph matching that allows label substitutions for both vertices and edges. Such a matching is often required in pattern recognition applications since graphs extracted from images are generally labeled with features vectors computed from raw data which are naturally subject to noise. This paper describes an extended version of a Binary Linear Program (BLP) for solving this class of graph matching problem. The paper also presents GEM++, a software framework that implements the BLP and that we have made available for the research community. GEM++ allows the processing of different sub-problems (induced isomorphism or not, directed graphs or not) with complex labelling of vertices and edges. We also present some datasets available for evaluating future contributions in this field.
