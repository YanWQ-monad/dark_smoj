# 2863 美食

## 题目描述

Bleaves 是一只贪吃的猪。

现在有 $$n$$ 个美食，一些美食之间可以互相搭配。美食之间的搭配关系可以抽象成一张 $$n$$ 个点，$$m$$ 条边的无向连通图。

现在 Bleaves 决定吃掉所有的美食。

她每次会随机选择一个还没吃完的美食，将其**一口吃完**，然后把可以与它搭配的美食**吃一口**，然后把还没吃过的可以与可以与它搭配的美食搭配的美食**吃一口**，不断重复。

求 Bleaves 期望吃几口。

换句话说，Bleaves 每次会随机选择一个还未删除的点 $$v$$，然后访问所有与 $$v$$ 连通的点，然后删除点 $$v$$，直到所有点都被删除。求期望访问次数。

你只需要回答模 $$998244353$$ 意义下的答案。

## 输入格式

第一行两个正整数 $$n,\,m$$，表示图的点数，边数。

接下来 $$m$$ 行，每行两个数 $$x,\,y$$，表示 $$x$$ 和 $$y$$ 之间存在一条边，保证 $$1 \leq x,\,y \leq n$$，不存在重边和自环。

## 输出格式

一行一个数表示答案。

## 输入样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.in" %}
```text
5 5
1 2
1 3
1 4
2 4
2 5
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.out" %}
```text
166374072
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输入样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.in" %}
```text
5 5
1 2
1 3
1 4
1 5
2 5
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.out" %}
```text
332748131
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

对于全部数据，$$1 \leq n \leq 10^5$$，$$m = n - 1$$ 或 $$m = n$$。

对于 $$10\%$$ 的数据，$$n < 20$$；

对于另外 $$20\%$$ 的数据，$$m = n - 1$$；

对于另外 $$10\%$$ 的数据，给定的图是一个环；

对于另外 $$20\%$$ 的数据，$$n \leq 10^3$$。

## 来源

[FJWC 2019 Day 5, Problem 3, 吃](http://218.5.5.242:9021/problem/192)

