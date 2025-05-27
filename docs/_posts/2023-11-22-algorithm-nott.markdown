---
layout: post
title:  "Algorithm note"
date:   2023-11-22 21:29:16 +0800
categories: Algorithm
---
<h1>Graph algorithm</h1>

1. Single-Source Shortest Paths

<h1>Dynamic programming</h1>
寻找子问题， 考虑问题能否排序，从左到右或者倒序从右到左思考子问题

1. 区间dp

2. 数位dp

<h1>数论</h1>
1. 欧拉定理

<h1>数据结构</h1>

1. 单调栈


2. 差分数组

3. 单调队列
  通常用于解决NGE(Next Greater Element)问题，一般来说，在一个集合n中要获取比某一个元素下一个更大的元素，这个算法的时间复杂度是O(n)，那么如果要获取每一个元素的下一个更大元素，时间复杂度就是O(n^2)。而如果使用单调栈，则可以把该问题的时间复杂度降低到O(n)
  单调栈本质上是一个LIFO（后进先出）的队列结构
  
<h1>图算法</h1>

<h2>单源最短路径</h2>

1. BFS

2. Dijkstra

3. A*

4. Floyd