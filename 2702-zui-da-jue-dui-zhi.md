# 2702 最大绝对值

## 题目描述

给你一个数组 $$a$$，定于 $$f(l,r)=\sum_{i=l}^{r-1}|a_i-a_{i+1}|\cdot g(i-l)$$，若 $$x$$ 为偶数 $$g(x)$$ 为 1，若 $$x$$ 为奇数 $$g(x)$$ 为 -1。

现在问最大的 $$f(l,r)$$ 是多少。

## 输入格式

第一行一个整数 $$n$$。

第二行描述 $$a$$。

## 输出格式

输出最大的 $$f$$ 值。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
5
1 4 2 3 1
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 样例解释

选择 $$f(1, 2)$$ 或 $$f(2, 5)$$ 都可以。

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 40% | $$1 \leq n \leq 10^3$$ |
| 100% | $$1 \leq n \leq 10^5,\ -10^8 \leq a_i \leq 10^8$$ |



