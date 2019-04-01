# 2829 黑白球

## 题目描述

一个箱子里面有 $$n$$ 个黑球 $$m$$ 个白球。你每小时都随机从箱子里面抽出两个小球，然后把这两个球都染成黑球，然后再放回去。问需要多少小时才能把所有小球变成黑色小球？输出期望值。

## 输入格式

多组测试数据。

第一行，一个整数 $$g$$，表示有 $$g$$ 组测试数据。

每组测试数据格式如下:

一行，两个整数，$$n$$ 和 $$m$$。

## 输出格式

共 $$g$$ 行，每行一个实数。误差不能超过 $$10^{-5}$$。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
5
1 1
2 1
1 2
4 7
1 3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
1.0
1.5
2.0
13.831068977298521
3.4
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

$$1 \leq g \leq 10$$，$$1 \leq n,\,m \leq 47$$。

## 来源

[Single Round Match 488 Round 1 - Division I, TheBoredomDivOne](https://community.topcoder.com/stat?c=problem_statement&pm=11193)

