# 2968 数列期望

## 题目描述

给出一个长度为 $$n$$ 的数列 $$a$$。

进行若干轮操作，每次操作在 $$[1,\,n]$$ 中等概率选择一个使得 $$a_i > 0$$ 的 $$i$$，并将 $$a_i$$ 减少 1。

问，期望多少次操作后 $$a_1$$ 被减成了 0。

## 输入格式

第一行一个整数 $$n$$。

第二行 $$n$$ 个整数，第 $$i$$ 个为 $$a_i$$。

## 输出格式

一行一个整数，表示答案。为避免精度误差，答案对 $$323232323$$ 取模。

即设答案化为最简分式后的形式为 $$\frac{a}{b}$$，其中 $$a$$ 和 $$b$$ 互质。输出整数 $$x$$ 使得 $$bx \equiv a\, (\operatorname{mod} 323232323)$$ 且 $$0 \leq x \leq 323232323$$。可以证明这样的整数 $$x$$ 是唯一的。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
3
2 3 3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
202020207
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

每个测试点 10 分，共 10 个测试点：

| 测试点 | 数据 |
| :---: | :---: |
| 1 | $$1 \leq n,\,a_i \leq 5$$ |
| 2 | $$1 \leq n \leq 10^5,\ 1 \leq a_i \leq 1$$ |
| 3-4 | $$1 \leq n \leq 2,\ 1 \leq a_i \leq 10^3$$ |
| 5-6 | $$1 \leq n,\,a_i \leq 10^3$$ |
| 7-8 | $$1 \leq n \leq 2,\ 1 \leq a_i \leq 5 \times 10^5$$ |
| 9-10 | $$1 \leq n,\,a_i \leq 5 \times 10^5$$ |

