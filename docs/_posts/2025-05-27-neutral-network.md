---
layout: post/ai
title:  "神经网络"
date:   2025-05-23 21:53:14 +0800
categories: ai
---

## 感知机 ##
感知机接收多个输入信号，输出一个信号（即0或1）。

、、、
y = 0 (w1x1 + w2x3 <=0)
    1 (w1x1 + w2x3 >0)
、、、

## 神经网络 ##
神经网络与感知机有很多相同之处，感知机虽然有着通过多层神经元处理输入从而表达复杂函数的可能性，然后其中的权重与偏置仍然需要人工设定，而神经网络与其最大的区别就在于可以从数据中自行学习权重与偏置。

**不同之处**
- 激活函数（activation function）： 讲输入值转换为一个新的输出值，这个输出值可能是线性的也可能是非线性的，激活函数是链接感知机与神经网络的桥梁

激活函数总多种类， 激活函数必须是非线性函数，（线性函数会使得加深网络层数失去意义因为即使加深层数函数的输出还是线性恒定的，具体地说，线性函数加深层数总是可以通过直接在单层节点上乘以固定的权重倍数来达到同样的效果）
- 阶跃函数（Step Function）： 指通过判断某一个阈值而输出固定值的函数 例如  0 if x<1 else 1
- sigmoid 函数: 连续的平滑曲线，可以输出连续的值
- Relu（Rectified Linear Unit）

## 单层神经网络 ##

## 多层神经网络 ##