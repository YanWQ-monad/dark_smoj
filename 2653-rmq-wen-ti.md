# 2653 RMQ问题

## 题目描述

给出序列 $$a$$，现在你在数组 $$b$$ 中每个位置独立随机赋值为一个 0 到 1 的实数，如果 $$b$$ 数组和 $$a$$ 数组相似，那么 $$b$$ 数组的权定为 $$\sum_{i=1}^{n} b_i$$，否则定为 0。

两个数组相似当且仅当对于任意 $$1 \leq l \leq r \leq n$$，都有 $$RMQ(a, l, r) = RMQ(b, l, r)$$。

$$RMQ(a, l, r)$$ 的值为最小的 $$i$$ 使得 $$a_i$$ 为 $$a_l, a_{l+1}, \cdots, a_r$$ 中的最大值。

现在问你数组 $$b$$ 的权的期望值。

## 输入格式

第一行一个正整数 $$t$$ 表示数据组数。

每组数据第一行一个整数 $$n$$。

接下来有一行 $$n$$ 个整数，表示序列 $$a$$。

## 输出格式

对于每组测试数据，如果答案为 $$\frac{p}{q}$$ 且 $$p, q$$ 互质，那么请输出一个 $$c$$ 满足 $$0 \leq c < 1000000007$$ 且 $$p-cq$$ 是 `1000000007` 的倍数。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
3
3
1 2 3
3
1 2 1
5
1 2 3 2 1
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
250000002
500000004
125000001
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 20% | $$1 \leq n \leq 200$$ |
| 40% | $$1 \leq n \leq 2 \times 10^3$$ |
| 100% | $$1 \leq n \leq 10^5,\ 1 \leq t \leq 5$$ |

并且 $$1 \leq a_i \leq n$$。

## 来源

[HDU 6305](http://acm.hdu.edu.cn/showproblem.php?pid=6305)

