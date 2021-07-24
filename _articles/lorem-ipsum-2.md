---
id: 2
title: "拓扑学习笔记（3）"
subtitle: "Topology notes"
date: "2021.7.17"
tags: "closed set, limit points, Hausdorff space"
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

$`X_n`$ converges to x if and only if for each open neighborhood U of x there is an m $`in`$ N such that $`X_n`$ $`in`$ U whenever n $`\geq`$ m

在这里，实数轴的经验开始不再适用。实数轴是稠密的，也就是说任何一个数字都有任意小的邻域。在离散的空间中则不是这样的，如下图：

![dummy image](../../static/img2.png)

如果有一个数列{b},那么根据定义，这个数列收敛至a,b,c。因为对于a和c来说，确确实实他们的每一个邻域都包含了b。但是在实际应用中，这种空间并不是很有研究价值（我没研究过，书上说的），所以我们想规避这种空间，以对大多数空间普适的结论。

> Hausdorff space: A topological space X is called a Hausdorff space if for each pair $`x_1`$, $`x_2`$ of distinct points pf X, there exists neighborhoods $`U_1`$, $`U_2`$ of $`x_1`$, $`x_2`$, respectively, that are disjoint.

Hausdorff空间不一定是稠密的；只要拓扑空间中包含了每一个元素单独构成的开集，那么这个空间就是一个Hausdorff空间。当然，这不是Hausdorff空间的必要条件（比如实数轴的标准拓扑；无法通过有限个开区间相交形成单个点的集合）。

> Thereom 17.8 Every finite point set in a Hausdorff space X is closed

Hausdorff空间每一个单个的点构成的集合都是它自己的闭包。所以，有限的点集合一定是闭集。实际上，有限集合为闭集这一条件称为$`T_1`$ axiom，这个条件比Hausdorff空间更宽松。

> Thereom 17.9 Let X be a space satisfying the $`T_1`$ axiom; let A be a subset of X. Then the point x is a limit point of A iff every neighborhood of x contains infinitely many points of A.

> Thereom 17.10 If X is a Hausdorff space, then a sequence of points of X conerges to at most one point of X.

Hausdorff空间中数列只有唯一的极限，这就解决了我们前面提到的问题。

> Thereom 17.11 Every simply ordered set is Hausdorff space in the order topology. The product of two Hausdorff spaces is a Hausdorff space. A subspace of a Hausdorff space is a Hausdorff space.

构造Hausdorff空间的常见方式。