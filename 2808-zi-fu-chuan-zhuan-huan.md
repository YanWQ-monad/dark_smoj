# 2808 字符串转换

## 题目描述

给出两个字符串 $$s$$ 和 $$t$$，他们长度相等，都是由小写字母 `a`、`b`、`c` 组成。每次操作，你可以对字符串 $$s$$ 进行如下操作之一：

1. 选择 $$s$$ 的一个字符 `a`，把该字符变成字符 `b`，费用是 `cost[0]`。
2. 选择 $$s$$ 的一个字符 `b`，把该字符变成字符 `c`，费用是 `cost[1]`。
3. 选择 $$s$$ 的一个字符 `c`，把该字符变成字符 `a`，费用是 `cost[2]`。

你的目标是把字符串 $$s$$ 变成 $$t$$，但是总费用不能超过给定的 `maxCost`，有多少种不同的操作方式？下面定义“不同的操作方式”：假设有两种操作方式 A 和 B ，只要满足如下两种情况之一，就认为是“不同的操作方式”：

1. A 和 B 的操作次数不同。
2. 存在一个整数 $$k$$，在第 $$k$$ 轮操作时，操作方式 A 是选择 $$s$$ 的第 $$i$$ 个字符进行操作，而操作方式 B 是选择 $$s$$ 的第 $$j$$ 个字符进行操作，且 $$i \not = j$$。

## 输入格式

第一行，字符串 $$s$$。长度不超过 11。

第二行，字符串 $$t$$。长度不超过 11。

第三行，三个整数，`cost[0]`、`cost[1]`、`cost[2]`。

第四行，一个整数，`maxCost`。

## 输出格式

一个整数。答案模 $$10^9+7$$。

## 输入样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.in" %}
```text
a
b
100 2 3
205
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.out" %}
```text
2
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输入样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.in" %}
```text
abcba
abcba
67 23 43
0
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.out" %}
```text
1
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输入样例 3

{% code-tabs %}
{% code-tabs-item title="sample3.in" %}
```text
bbaccbbb
bbacbbac
70437 133 133
991840667
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 3

{% code-tabs %}
{% code-tabs-item title="sample3.out" %}
```text
89619301
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 样例解释

### 样例 1

操作方式 1：$$a \rightarrow b$$，费用是 100。 

操作方式 2：$$a \rightarrow b \rightarrow c \rightarrow a \rightarrow b$$，费用是 205。

### 样例 2

如果 $$s$$ 和 $$t$$ 相同，那么空操作也是一种操作方式。

## 数据范围

$$1 \leq maxCost \leq 10^9$$。

| 测试点 | 范围 |
| :---: | :---: |
| 40% | $$\operatorname{len}(s)=2,\,1 \leq cost \leq 10^2$$ |
| 100% | $$1 \leq cost \leq 10^9$$ |

