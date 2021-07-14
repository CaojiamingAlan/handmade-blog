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

> to do