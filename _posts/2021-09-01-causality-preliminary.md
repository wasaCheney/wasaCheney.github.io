---
title: 'Causality preliminary'
date: 2021-09-01
permalink: /posts/2021/09/casality-preliminary/
tags:
  - causality
  - preliminary
---

This is an reading notes from an [causality introduction website](https://mp.weixin.qq.com/s?__biz=MzIzMjQyNzQ5MA==&mid=2247577325&idx=1&sn=ae0ba345ac71ba662385501d1cce1084&chksm=e896f460dfe17d76c1c96d4d49cd582db07e58528ebf659105b1f132b6c523c535bea0b76f0a&mpshare=1&scene=1&srcid=0901iYhwPHVdpGR6W9hB6C7I&sharer_sharetime=1630454820118&sharer_shareid=90613f16f63791e4bdb8558a8e0e032d&exportkey=A82BzUbnjahw8Xsx9hUKk50%3D&pass_ticket=JWW3B%2Fmet59y%2BaMQ4Z0vuvt5vLpzv6uROzOvOBPqGtmFZCJCx200jlLNKenVC0HA&wx_header=0#rd)

Yule-Simpson’s Paradox
=====================
- Two subjects, with each passing rate for male is less than that for female, but overall, passing rate for Male is greater than that for female
- Mathematically, a/b < c/d, and a'/b' < c'/d', but (a + a')/(b+b') > (c + c')/(d + d'), it is trivial
- But statistically, it does make sense: a third (underlying, unobservale) variable could twist/change relations of two varialbes. It means that
  observation data might result in wrong conclusions.
  
Rubin Causal Model, More Precise
==================
- i-th individual, Zi = 1/0 means treating/intervening or not, Yi(1/0) means potentional outcome for intervening or not
- individual causal effect, Yi(1) - Yi(0), but only Yi = Zi * Yi(1) - (1 - Zi) * Yi(0) could be observed in practice
- make Z random, which means Z and {Y(1), Y(0)} are independent, then Average Causal Effect (ACE):
  ACE(Z->Y) = E[Yi(1) - Yi(0)] = E[Yi(1)] - E[Yi(0)] = E[Yi(1)|Zi=1] - E[Yi(0)|Zi=0] = E[Yi|Zi=1] - E[Yi|Zi=0]
- When sample is finite, {Yi(1), Yi(0)} might be unkown but constant, so Yi is random only because Z is made random

Fisher Randomization Test
====================
- sharp null, H0: Yi(1) = Yi(0), for all i=1,...,n
-  Z = (Z1, ..., Zn), Y = (Y1, ..., Yn), m = sum_i Zi means number of individuals intervened
- randomization assignment, p(Z|Y) = 1 / C(m from n)

Neyman Repeated Sampling Procedure
=====================
- under finite sample, how to estimate ACE tao = 1/n sum_i (Yi(1) - Yi(0))
- one unbiased estimator, 1/m sum_i (ZiYi) - 1/(n-m) sum_i (1 - Zi)Yi

Ignorability
==============
- Z means intervening or not, Y means potential outcome, X means covariant
- a strong ignorability, Z and {Yi(1), Yi(0)} are independent
- a general ignorability, Z and {Yi(1), Yi(0)} are independent conditioned on X???
- the effect of some causation (could be verified), the causation of some effect (could be assumed or explored)
- 
