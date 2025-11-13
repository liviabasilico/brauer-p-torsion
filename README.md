# Computing the isogeny type of the unipotent part of Brauer groups of abelian varieties

The code here is supplemental material for the preprint [arXiv:2511.08840](arxiv.org/abs/2511.08840), joint with Alexei Skorobogatov and Yuan Yang. The notebooks contain computations performed in SageMath v10.7 of the dimension and isogeny type of ${\bf U}_A$ and its torsion subgroups in various situations, following the principle explained in the appendix of the paper. Computations were made using the [implementation of Witt vectors](https://arxiv.org/abs/2504.01834) due to Rubén Muñoz-\-Bertrand. We thank Marco Lastres for technical help with the code.

The following is an outline of the files present here.

* Example 1: we explain how our script works, and compute the isogeny type of ${\bf U}_A$ for several supersingular abelian varieties $A$ of dimension $4$ and $a$-number $1$, in characteristic $3$.
* Example 2: a function that computes $\textnormal{dim}({\bf U}_A[p])$, given the isomorphism class of $A[p]$ in the form of a Kraft word.
* Example 3: here we compute the isogeny type of ${\bf U}_A$ for abelian varieties $A$ with $a$-number $1$ and varying Newton polygons. We draw from a list of all symmetric Newton polygons with $g\le20$ and no slopes $0$ or $1$ from file `newton_curves_2_to_20.json`.

We implement sparse matrix operations to make some computations more efficient. However, in our programs we still need to compute the dimension of a closed subvariety of a very large affine space. This is the main limitation to computing the dimension of ${\bf U}_A[p^n]$ for large values of $g,p$ and $n$. In particular cases it may be possible to greatly reduce the dimension of the ambient space a priori, thus overcoming this issue.

<sub> This work is licensed under a
[Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/). © Livia Grammatica 2025</sub>
