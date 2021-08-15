---
title: 'basis for convex optimization'
date: 2021-08-15
permalink: /posts/2021/08/convex-optimization/
tags:
  - convex optimization
  - basis
---

## Notable Sets
  - line / (closed) line segments: \theta * x1 + (1 - \theta) * x2, theta in R / in \[0, 1\]
  - affine set / convex set: \theta * x1 + (1 - \theta) * x2, theta in R / in \[0, 1\]
  - cone: theta * x, theta in R+ (nonnegative real values)
  - hyperplane / halfspace: a^T x = b or a^T (x - x0) = 0 / a^T x < b, a^T x > b  or a^T (x - x0) < 0, a^T (x - x0) > 0
  - balls / ellipsoids: (x - xc)^T P (x - xc) <= r^2 , P = I or other kinds of positive definite solution.
  - polyhedron: the solution set of a finite number of linear equalities and inequalities
  - simplex: conv hull of k+1 affinely independent points, and its affine dimensionality is k. such as line segment, triangle (with interior), tetrahedron (with interior)
