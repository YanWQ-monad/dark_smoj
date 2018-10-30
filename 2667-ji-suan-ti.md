# 2667 计算题

## 题目描述

给出 $$n$$，$$\mathrm{lcm}(S)$$ 表示非空集合 $$S$$ 里面所有数的最小公倍数，例如，$$\mathrm{lcm}(6, 24) = 24$$，$$\mathrm{lcm}(12, 8) = 24$$，$$\mathrm{lcm}(1, 2, 3, 4, 8) = 24$$。

定义 $$\mathrm{mslcm}(n)$$ 为所有满足 $$\mathrm{lcm}(S)$$ 等于 $$n$$ 的 $$S$$ 中，使得 $$S$$ 集合所有元素的值的和最大，那么这个和就为 $$\mathrm{mslcm}(n)$$。

求 $$\sum_{i=2}^{n} \mathrm{mslcm}(i)$$。

## 输入格式

每行一个 $$n$$，表示一组测试数据。

输入以 $$n=0$$ 结束。

## 输出格式

对于每组测试数据，输出相应的答案。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
10
1000
0
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出格式

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
86
823080
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 40% | $$2 \leq n \leq 10^3$$ |
| 100% | $$2 \leq n \leq 2 \times 10^7,\ 1 \leq t \leq 200$$ |

## 来源

[UVA 1730](https://uva.onlinejudge.org/external/17/1730.pdf)，[UVALive 7340](https://icpcarchive.ecs.baylor.edu/external/73/7340.pdf)

