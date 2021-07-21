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

空集和全集都是既开又闭的，因为全集和空集是开集。也有可能存在非开非闭集合（e.g.只有全集和空集的拓扑中任意一个元素的集合既不是开集也不是闭集）。要意识到实数轴也是一种拓扑（最简单的排序拓扑），所以很多时候可以从实数轴出发，借助实数轴思考，并把结论推广到任意拓扑上去。

> Theorem 17.1 Let X be a topological space. Then the following conditions holds:

> (1) $`\empty`$ and X are closed.

> (2) Arbitrary intersections of closed sets are closed.

> (3) Finite unions of closed sets are cloesd.

还是那一套，但是是反向操作。交集无限并集有限。

> Theorem 17.2 Let Y be a subspace of X. Then a set A is closed in Y if and only if it equals the intersection of a closed set of X with Y

条件是iff，充分必要，注意前后的closed是针对不同的set。定理中蕴含的另一个意思就是，Y中的闭集不一定是X中的闭集。但是如同开集一样：

> Theorem 17.3 If A is closed in Y and Y is closed in X, then A is closed in X.

# Closure and Interior

> Given a subset A, the interior of A is defined as the union of all open sets contained in A. The closure of A is defined as the intersection of all closed sets containing A.

就是一个苹果带不带皮。。。结合open/closes set的定义，内部一定是开集，闭包一定是闭集。

> Theorem 17.4 Let Y be a subspace of X. Let A be a subset of Y, let $`\bar A`$ denote the closure of A in X. Then the closure of A in Y equals $`\bar A`$ $`\cap`$ Y

> Theorem 17.5 Let A be a subset of the topological space X. 

> (a) Then x $`in`$ $`\bar A`$ iff every open set U containing x intersects A

> (b) Supposing the topology of X is given by a basis, the $`\bar A`$ iff every basis element B containing x intersects A.

> U is an open set containing x <=> U is a neighborhood of x.

> Limit point/cluster point: every neighborhood of x intersects A in some point other than x itself.

闭包=内部+所有极点，like 苹果=果肉+苹果皮。闭集一定包含它的所有极点

# Hausdorff Spaces

拓扑学中最重要的概念之一。异常符合直觉，以至于我在看到这里之前都没有察觉到非Hausdorff空间的存在。这里书中应该是写落下了，所以我们补上在拓扑空间中数列收敛的定义：


![dummy image](../../static/img2.png)

如图所示，