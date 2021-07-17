---
id: 1
title: "拓扑学习笔记（2）"
subtitle: "Topology notes"
date: "2021.7.14"
tags: "order topology, product topology, subspace topology"
---

本篇对应原书第14~16章的内容

# The Order Topology

> Let X be a set with a simple order relation. Let B be the collection of 

> (1) all open intervals (a,b)

> (2) [$`a_0`$, b) where $`a_0`$ is the smallest element of X

> (3) (a, $`b_0`$] where $`b_0`$ is the largest element of X

> B is a basis for the order topology of X

排序，没啥好说的。Ray的定义也类似。

# The Product Topology

> The product topology on X $`\times`$Y is the topology having as basis the collection B of all sets of the form U $`\times`$V, where U is an open subset of X and V is an open subset of Y.

注意，B只是一个basis，而并非新拓扑的全部元素。形象地说，用正方形代表B中的元素的话，那一个正方形的右上和另一个正方形的左下相交也是这个拓扑的一个元素，也就是open set。然而，分别取两个集合的open set再做笛卡尔积是产生不了这样的元素的。但是，这里的U和V是任意open set。我们完全可以缩小这个基的涵盖面，如下：

> Theroem 15.1: Given B a basis of X and C a basis of Y, D the cartesian product of B and C, then D is a basis of X $`\times`$Y

基的笛卡尔积是积拓扑的基。这个结论相比于上面的定义取任意open set，更符合直觉一点。

投影的符号是$`\pi`$，定义和线性代数类似。

> Thereom 15.2 The collection S = { $`\pi_1^{-1}(U)|U`$open in X } $`\cup`$ { $`\pi_2^{-1}(V)|V`$open in Y } is a subbasis of the product topology on X $`\times`$Y

直觉上来讲，就是这些十字能够交叉出正方形（意思是这么个意思，我也知道我的解释很不靠谱=w=）

![dummy image](../../static/img0.png)

# The Subspace Topology

> Let X be a topological space with topology T. If Y is a subset of X, the collection $`T_y = \{ Y \cap U | U \in T\}`$ is a topology on Y, called the subspace topology

拓扑中每个开集与子集的交集的集族构成子拓扑。

>Lemma 16.1 $`B_y = \{ b \cap U | b \in B\}`$ is a basis for the subspace topology on Y

拓扑的基中的元素与子集的交集的集族构成子拓扑的基。

>Lemma 16.2 If U is open in Y and Y is open in X, then U is open in X

开集性质的传递性

>Lemma 16.3 If A is a subspace of X and B is a subspace of Y, then the product topology on A $`\times`$B is the same as the topology A $`\times`$B inherits as a subspace of X $`\times`$Y

> Convex(subset): Given an ordered set X, a subset Y is convex in X if for each pair of points a < b of Y, the entire interval (a, b) of points of X lies in Y. Intervals and rays are convex in X

好像没有不连续的情况...吧？

>Thereom 16.4 Let X be an ordered set in the order topology; let Y be a subset of X that is convex in X. Then the order topology on Y is the same as the topology Y inherits as a subspace of X. 