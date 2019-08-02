# 2916 区间求解

## 题目描述

给你一个长度为 $$n$$ 的数组和一个正整数 $$m$$，还有 $$q$$ 个询问，每次询问是求区间 $$[l,\,r]$$ 和满足以下要求的子序列数。

子序列需要满足：$$l \leq p_1 < p_2 < \cdots < p_k \leq r$$，并且 $$\sum_{i=1}^{k} a_{p_i} = 0 \,(\operatorname{mod} m)$$。空子序列也是一种方案，每次询问输出结果模 1000000007。

## 输入格式

第一行两个正整数 $$n$$ 和 $$m$$。

接下来一行有 $$n$$ 个整数，第 $$i$$ 个数表示 $$a$$ 数组中的第 $$i$$ 个数。

接下来一行有一个正整数 $$q$$。

接下来有 $$q$$ 行，每行两个正整数 $$l$$ 和 $$r$$，表示询问区间 $$[l,\,r]$$。

## 输出格式

对于每一个询问，输出对应的结果模 1000000007。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
4 3
5 1 3 2
4
1 2
1 3
1 4
2 4
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
2
4
6
4
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

对于 20% 的数据：$$1 \leq n,\,q \leq 20$$

对于 40% 的数据：$$1 \leq n,\,q \leq 10^3$$

还有另外 20% 的数据：$$q = 1$$

对于 100% 的数据：$$1 \leq n,\,q \leq 2 \times 10^5$$，$$1 \leq m \leq 20$$，$$0 \leq a_i \leq 10^9$$，$$ 1 \leq l_i \leq r_i \leq n$$。

