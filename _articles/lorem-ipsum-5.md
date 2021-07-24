---
id: 5
title: "拓扑学习笔记（4）"
subtitle: "Topology notes"
date: "2021.7.24"
tags: "continuous functions"
---

本篇对应原书第18章的内容

# Continuous functions

> Continuous: Let X and Y be topological spaces. A function f: X->Y is said to be continuous if for each open subset V of Y, the set $`f^{-1}(V)`$ is an open subset of X.

连续的定义：任意开集的原相是开集。这个定义直接隐藏了任意拓扑的结构，从而给出了最一般的有关连续性的定义（而不是像实分析那样$`\epsilon`$来$`\epsilon`$去，小家子气XD）。另外，如果能够证明Y的基的所有元素的原相都是开集，那么f就是连续的（因为任意开集的并集是开集，且Y中任意开集可以由基生成出来）。

> Theorem 18.1 Let X and Y be topological spaces; let f: X->Y. Then the following are equivalent.

> 1. f is continuous

> 2. For every subset A of X, one has $`f(\overline{A}) \subset \overline{f(A)}`$

> 3. For every closed set B of Y, the set $`f^{-1}(B)`$ is closed in X

> 4. For each x $`\in`$ X and each neighborhood V of $`f(x)`$, there is a neighborhood U of x such that $`f(U) \subset V`$

4有点像是传统的$`\epsilon`$-language了.如果4成立，那么我们说f在x处连续。

to be continued...