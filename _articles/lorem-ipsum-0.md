---
id: 0
title: "拓扑学习笔记（1）"
subtitle: "Sed sit amet arcu a diam tincidunt porta"
date: "2021.7.12"
tags: "tag1, tag2"
---

参考书：Topology, James R. Munkres

其实写下这篇笔记时，拓扑的书已经看了近1/4了。由于生活繁忙（其实并没有），每次再拿起书的时候发现之前看的又忘了大半。于是我决定自己弄在网上记录下学习中的重要结论（一些简单的定义和结论我会略过，请读者自己翻书）以及自己的一些思考，主要诉求是网站要支持LaTeX，所以想来想去还是自己搭一个最方便。学习拓扑主要还是出自个人兴趣。毕竟纯数这种东西，对我以及一般人的生活毫无用处，简直就是无用之用的代名词。本科时候学过一些数学，虽然学习过程还算比较享受，但有些时候还是会很功利的背下一些自己不理解的结论。而现在，我想在学校之外，单纯是为了理解这个世界、不“卷”的学习最纯粹的数学。

Topological Space

> A topology on a set X is a collection T of subsets of X having the following properties:

>(1) $`\empty`$ and X are in T

>(2) The union of the elements of any subcollection of T is in T

>(3) The intersection of the elements of any finite subcollection of T is in T

拓扑的定义。拓扑的定义有多种，但是殊途同归。有些是从open set出发的，但是我更喜欢这一种，简单直观。交集要求有限，可以联想到在实数轴上的open set也有同样的要求。