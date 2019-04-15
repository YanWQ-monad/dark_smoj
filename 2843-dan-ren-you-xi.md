# 2843 单人游戏

## 题目描述

本游戏是单人游戏，玩家通过移动棋子得到分数。

棋盘由 $$n$$ 个格子排成一行，从左到右编号为 1 到 $$n$$，每个格子都有一个相关的价值。最初，棋子位于第 1 个格子上，当前方向是向右的。

在每个回合中，棋子在当前方向上行走零步或多步，每一步就是走一个格子。然后在下一回合中，棋子的方向反转。

一开始，玩家总得分是 0 分。

每次棋子从格子 A 移动到格子 B，那么从 A 至 B 这一段连续的格子的得分都会累加到玩家的总得分去。

如果某次移动会使得玩家总得分小于 0，那么玩家肯定不会进行这样的移动。

如果允许玩家最多进行 $$k$$ 次移动，输出玩家获得的最高总得分。

## 输入格式

多组测试数据。

第一行，一个整数 $$g$$，表示有 $$g$$ 组测试数据。

每组测试数据格式如下：

第一行，两个整数，$$n$$ 和 $$k$$。

第二行，$$n$$ 个整数，第 $$i$$ 个整数 $$a_i$$ 是第 $$i$$ 个格子的价值。

## 输出格式

共 $$g$$ 行，每行一个整数。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
5
5 3
2 -2 4 3 -10
2 10
-6 5
2 10
5 -6
3 3
10 -100 80
3 4
10 -100 80
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
21
0
50
30
90
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

$$1 \leq g \leq 5$$，$$1 \leq n \leq 50$$，$$1 \leq k \leq 4 \times 10^8$$，$$-4 \times 10^8 \leq a_i \leq 4 \times 10^8$$。

## 来源

[Single Round Match 450 Round 1 - Division I, RowGame](https://community.topcoder.com/stat?c=problem_statement&pm=10664)

