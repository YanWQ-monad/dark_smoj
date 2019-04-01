# 2819 移动“哨兵棋子”

## 题目描述

一条数轴有 $$n$$ 个棋子，每个棋子可以占据一个整数位置。$$n$$ 个棋子目前位于不同的整数位置，现在你想要移动它们以便它们占据 $$n$$ 个连续位置（例如，位置 5, 6, 7, 8）。当前所有棋子中位置最小或者位置最大的棋子，称为“哨兵棋子”。每一次，你只能移动“哨兵棋子”。你可以把“哨兵棋子”移动到当前任何未占用的整数位置，前提是在这个新位置该棋子不再是一个“哨兵棋子”。请确定使得 $$n$$ 个棋子最终占据连续的 $$n$$ 个位置的最小移动次数和最大移动次数。

## 输入格式

第一行，一个整数 $$n$$。

接下来有 $$n$$ 行，第 $$i$$ 行是一个整数 $$a_i$$，表示第 $$i$$ 个棋子的位置。

## 输出格式

第一行，一个整数，最小移动次数。

第二行，一个整数，最大移动次数。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
3
7
4
9
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
1
2
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

$$1 \leq n \leq 10^5$$，$$1 \leq a_i \leq 10^9$$。

## 来源

[USACO 2019 February Contest, Silver, Problem 1, Sleepy Cow Herding](http://usaco.org/index.php?page=viewproblem2&cpid=918)

