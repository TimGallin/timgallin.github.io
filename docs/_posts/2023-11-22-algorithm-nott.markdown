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

- 选或不选， 枚举选哪个 s[0:i]子数组/序列的答案
- 以index i结尾的子数组/序列 （可以记录子数组/序列的末尾值，不需要额外空间）  LIS



1. 区间dp

2. 数位dp

3. 划分型dp
 - 分割回文字符串

4. 线性dp
 - LCS  dfs(i,j) = max(dfs(i-1,j-1) + 1 if s[i]==t[j], dfs(i-1, j), dfs(i, j-1))
 - LIS  dfs(i) = max(dfs(j) for j in range(i)) +1

5. 背包问题
 - 0-1 背包 选或不选 dfs(i, c) = dfs(i-1,c)+dfs(i-1, c-v[i])
 - 完全背包  选或不选，不限制选择次数  dfs(i, c) = dfs(i-1,c)+dfs(i, c-v[i])
 - 分组背包  选或不选，限制选择次数    dfs(i, c) = dfs(i-1,k*v[i]) for k in range(max(limit, c//v[i])+1)

<h1>数论</h1>
1. 欧拉定理

<h1>数据结构</h1>

1. 单调栈


2. 差分数组

3. 单调队列
  通常用于解决NGE(Next Greater Element)问题，一般来说，在一个集合n中要获取比某一个元素下一个更大的元素，这个算法的时间复杂度是O(n)，那么如果要获取每一个元素的下一个更大元素，时间复杂度就是O(n^2)。而如果使用单调栈，则可以把该问题的时间复杂度降低到O(n)
  单调栈本质上是一个LIFO（后进先出）的队列结构
  
4. 堆
4.1 懒删除堆 
  用于解决动态从堆中更新对象
<h1>图算法</h1>

<h2>单源最短路径</h2>

1. BFS

2. Dijkstra

3. A*

4. Floyd

5. 一些小技巧
在数据范围小的前提下借鉴计数排序查找第k小/大的数
计数排序，用一个 cnt\textit{cnt}cnt 数组维护窗口内每个数的出现次数。然后遍历 cnt\textit{cnt}cnt 去求第 xxx 小的数。
什么是第 x 小的数？
设它是 num\textit{num}num，那么 <num<\textit{num}<num 的数有 <x<x<x 个，≤num\le\textit{num}≤num 的数有 ≥x\ge x≥x 个，就说明 num\textit{num}num 是第 xxx 小的数。

循环数组可以使用 （i+k-1）mod n 遍历

