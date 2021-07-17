---
id: 3
title: "拓扑学习笔记（3）"
subtitle: "Topology notes"
date: "2021.7.17"
tags: "closed set, limit points"
---

本篇对应原书第17章的内容

# Closed Sets
> A subset A of a topological space X is said to be closed if the set X - A is open.

空集和全集都是既开又闭的，因为全集和空集是开集。其余的集合要么是开集要么是闭集，没有两者均不是的。要意识到实数轴也是一种拓扑（最简单的排序拓扑），所以很多时候可以从实数轴出发，借助实数轴思考，并把结论推广到任意拓扑上去。

> Theorem 17.1 Let X be a topological space. Then the following conditions holds:

> (1) $`\empty`$ and X are closed.

> (2) Arbitrary intersections of closed sets are closed.

> (3) Finite unions of closed sets are cloesd.

还是那一套，但是是反向操作。交集无限并集有限。

> Theorem 17.2 Let Y be a subspace of X. Then a set A is closed in Y if and only if it equals the intersection of a closed set of X with Y

条件是iff，充分必要，注意前后的closed是针对不同的set。定理中蕴含的另一个意思就是，Y中的闭集不一定是X中的闭集。但是如同开集一样：

> Theorem 17.3 If A is closed in Y and Y is closed in X, then A is closed in X.

to be continued...
