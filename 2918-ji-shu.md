# 2918 计数

## 题目描述

给出 $$n$$ 和 $$p$$，表示 $$n$$ 维空间和质数 $$p$$。再给出 $$n$$ 维空间下的两个点 $$s$$ 和 $$t$$，问以 $$s$$ 为起点 $$t$$ 为终点组成的超立方体内有多少个整点满足要求，答案模 1000000009。

对于一个整点，如果有某一维是负数，它的值为 0，原点的值为 1。其它点的值是 $$(x_1 - 1,\,x_2,\,\cdots,\,x_n),\,(x_1,\,x_2 - 1,\,\cdots,\,x_n),\,\cdots,\,(x_1,\,x_2,\,\cdots,\,x_n - 1)$$ 的和。

一个点是合法当且仅当它的值不是 $$p$$ 的倍数。

## 输入格式

第一行一个整数 $$t$$，表示测试数据组数。

每组测试数据格式：

第一行两个整数 $$n$$ 和 $$p$$。

第二行 $$n$$ 个数，表示高维空间里的初始点坐标。

第三行 $$n$$ 个数，表示高维空间里的结束点坐标。

## 输出格式

对于每一组数据，按照格式要求输出对应的结果模 1000000009。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
3
3 2
4 0 4
7 9 8
4 3
0 3 0 2
6 8 1 5
5 7
1 2 3 4 5
11 12 13 14 15 
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
Case 1: 9
Case 2: 17
Case 3: 2515
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

对于 40% 的数据：$$n = 2$$。

对于 100% 的数据：$$0 < n < 8,\,t \leq 10$$，$$p$$ 是质数且 $$p < 20$$，坐标的值非负且小于 $$10^9$$。

