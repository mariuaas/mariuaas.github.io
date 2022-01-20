---
title: "Topics from MSc Thesis: Resolvent Operators"
# last_modified_at: 2016-03-09T16:20:02-05:00
categories:
  - Blog
tags:
  - operators
  - resolvent formalism
published: false
---

Previously, we introduced inverse problems in the context of integral equations, and we showed how we can solve linear inverse problems with homogeneous operators via SVE/SVD to construct a pseudoinverse. In this post we will be discussing how we solve inverse problems from integral equations of the second kind -- i.e. inhomogenous integral operators on the form

$$
\begin{align}
    y(t) &= x(t) -  \lambda^{-1}\int_\mathcal{S} w(s,t) x(s) \,\,ds \\
    &= \big([I - \lambda^{-1} W]x\big)(t).
\end{align}
$$

While the above equation might seem intimidating, recall that for the finite dimensional case -- i.e. for any numerical solution -- the operator $W$ can simply be considered a matrix.

We could attempt to invert the matrix using SVD, similar to the homogeneous case, however we will instead opt to use *resolvent formalism*.