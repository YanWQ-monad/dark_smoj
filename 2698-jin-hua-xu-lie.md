# 2698 进化序列

## 题目描述

Abathur 采集了一系列 Primal Zerg 的基因样本，这些基因构成了一个完整的进化链。为了方便，我们用 $$a_0,\,a_1,\,\cdots,\,a_{n-1}$$ 这 $$n$$ 个正整数来描述它们。

一个基因 $$a_x$$ 可以进化为序列中它之后的基因 $$a_y$$。这个进化的复杂度，等于 $$a_x \operatorname{or} a_{x+1} \operatorname{or} \cdots \operatorname{or} a_y$$ 的值，其中 $$\operatorname{or}$$ 是二进制的或运算。

Abathur 认为复杂度小于 $$m$$ 的进化被认为是温和的。它希望计算出温和的进化的对数。

## 输入格式

第一行包含两个整数 $$n,\,m$$。

接下来一行包含 $$a_0,\,a_1,\,\cdots,\,a_{n-1}$$ 这 $$n$$ 个正整数，描述这 $$n$$ 个基因。

## 输出格式

第一行包含一个整数，表示温和的进化的对数。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
4 6
1 3 5 1
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
2
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 30% | $$1 \leq n \leq 10^3$$ |
| 100% | $$1 \leq n \leq 10^5,\ 0 \leq m, a_i \leq 2^{30}$$ |

## 来源

[JZOJ 3518](https://jzoj.net/senior/#contest/show/1150/1)

