# 2914 分组

## 题目描述

Farmer John 想要将他的编号为 $$1 \sim n$$ 的 $$n$$ 头奶牛分为非空的 $$k$$ 组，使得任意两头来自不同组的奶牛都需要走一定的距离才能相遇。奶牛 $$x$$ 和奶牛 $$y$$（其中 $$1 \leq x < y \leq n$$）愿意为了见面走 $$(2019201913x + 2019201949y) \operatorname{mod} 2019201997$$ 英里。

给定一个将 $$n$$ 头奶牛分为 $$k$$ 个非空小组的分组方案，令 $$m$$ 为任意两头来自不同组的奶牛愿意为了见面行走的英里数的最小值。

为了测试奶牛们相互之间的忠诚度，Farmer John 想要将 $$n$$ 头奶牛以最佳的方式分为 $$k$$ 组，使得 $$m$$ 尽可能大。

## 输入格式

输入仅有一行，包含 $$n$$ 和 $$k$$，用空格分隔。

## 输出格式

输出最优的 $$m$$。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
3 2
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
2019201769
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 样例解释

在这个例子中，奶牛 1 和奶牛 2 愿意为了见面走 2019201817 英里。奶牛 2 和奶牛 3 愿意走 2019201685 英里。奶牛 1 和奶牛 3 愿意走 2019201769 英里。所以，将奶牛 1 单独分为一组，奶牛 2 和奶牛 3 分为一组，$$m = \min(2019201817, 2019201769) = 2019201769$$（这是我们在这个问题中能够达到的最佳结果）。

## 数据范围

$$2 \leq k \leq n \leq 7500$$。

## 来源

[USACO 2019 US Open Contest, Gold, Problem 2. I Would Walk 500 Miles](http://usaco.org/index.php?page=viewproblem2&cpid=946)

