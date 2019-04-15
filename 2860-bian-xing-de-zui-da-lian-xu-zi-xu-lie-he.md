# 2860 变形的最大连续子序列和

## 题目描述

有 $$n$$ 个非负整数从左往右排成一行，第 $$i$$ 个非负整数是 $$a_i$$。

对于每一个 $$a_i$$，都有 1 次操作：这次操作使得 $$a_i$$ 有 $$p_i\%$$ 的概率会变成 $$- a_i$$，有 $$1 - p_i\%$$ 的概率不变。

当所有的 $$a_i$$ 都操作结束后，输出最大连续子序列和的期望值。由于子序列允许为空，所以答案总是非负。

## 输入格式

多组测试数据。

第一行，一个整数 $$g$$，表示有 $$g$$ 组测试数据。

每组测试数据格式如下：

第一行，一个整数 $$n$$。

第二行，$$n$$ 个整数，第 $$i$$ 个整数是 $$a_i$$。

第三行，$$n$$ 个整数，第 $$i$$ 个整数是 $$p_i$$。

## 输出格式

共 $$g$$ 行，每行一个实数。与标准答案的误差不超过 $$10^{-7}$$。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
3
3
10 20 30
0 0 0
3
10 40 20
0 100 0
3
1 1 1
50 50 50
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
60.0
20.0
1.375
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

$$g \leq 3$$，$$1 \leq n \leq 50$$，$$0 \leq a_i \leq 50$$，$$0 \leq p_i \leq 100$$。

## 来源

[TCO19 Single Round Match 743 Round 1 - Division I, ExpectedSum](https://community.topcoder.com/stat?c=problem_statement&pm=15233)

