---
title: 'basis for convex optimization'
date: 2021-08-15
permalink: /posts/2021/08/convex-optimization/
tags:
  - convex optimization
  - basis
---

## Notable Concepts
  - line / (closed) line segments: \theta * x1 + (1 - \theta) * x2, theta in R / in \[0, 1\]
  - affine set / convex set: \theta * x1 + (1 - \theta) * x2, theta in R / in \[0, 1\]
  - cone: theta * x, theta in R+ (nonnegative real values)
  - hyperplane / halfspace: a^T x = b or a^T (x - x0) = 0 / a^T x < b, a^T x > b  or a^T (x - x0) < 0, a^T (x - x0) > 0
  - balls / ellipsoids: (x - xc)^T P (x - xc) <= r^2 , P = I or other kinds of positive definite solution.
  - polyhedron: the solution set of a finite number of linear equalities and inequalities
  - simplex: conv hull of k+1 affinely independent points, and its affine dimensionality is k. such as line segment, triangle (with interior), tetrahedron (with interior). As well as, unit simplex (x >= 0, 1^T * x <= 1), or probability simplex (x >= 0, 1^T * x = 1)
  - partial order, minimum (最小, for each s in S, s <= s0, or, S included in s0+K), minimal (极小, if s in S s.t. s<= s0, then s = s0, or, Intersection(so-K, S) = {x} )
  - supporting hyperplane

## Optimization Problems

  - min f_0, s.t. f_i <= 0, h_j = 0.
