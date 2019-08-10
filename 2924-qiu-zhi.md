# 2924 求值

## 题目描述

给定一个长度为 $$n$$ 的字符串 $$S$$，令 $$T_i$$ 表示它从第 $$i$$ 个字符开始的后缀。求

$$
\sum_{1 \leqslant i < j \leqslant n} \text{len}(T_i) + \text{len}(T_j) - 2 \times \text{lcp}(T_i,\,T_j)
$$

其中，$$\text{len}(a)$$ 表示字符串 $$a$$ 的长度，$$\text{lcp}(a,b)$$ 表示字符串 $$a$$ 和字符串 $$b$$ 的最长公共前缀。

## 输入格式

一行一个字符串 $$S$$。

## 输出格式

一行一个整数，即所求的答案。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
cacao
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
54
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 样例解释

$$(1 + 2 + 3 + 4 + 5) \times (5 - 1) = 60$$

$$\text{lcp}("cacao",\,"cao") = 2$$

$$\text{lcp}("acao",\,"ao") = 2$$

$$60 - 2 \times 2 - 1 \times 2 = 54$$

## 数据范围

40% 的数据：$$2 \leq n \leq 10^3$$

100% 的数据：$$2 \leq n \leq 10^5$$

字符串由小写字符组成。

