# 2669 排列问题

## 题目描述

给出 $$n$$ 和 $$m$$，定义 $$ans[i]$$ 是值为 $$i$$ 的排列 $$p$$ 的个数。

一个排列的值为 $$\sum_{i=1}^{n} |p_i-i|$$，答案对 $$m$$ 取模。

## 输入格式

第一行一个 $$t$$ 表示数据组数。

每组数据第一行两个整数 $$n$$，$$m$$。

## 输出格式

对于每组测试数据输出一行 $$n^2$$ 个数，第 $$i$$ 个数表示值为 $$i-1$$ 的排列个数。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
4
4 1000000223
3 1000000321
2 1000000123
1 1000000447
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
1 0 3 0 7 0 9 0 4 0 0 0 0 0 0 0
1 0 2 0 3 0 0 0 0
1 0 1 0
1
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 30% | $$1 \leq n \leq 10$$ |
| 60% | $$1 \leq n \leq 20$$ |
| 100% | $$1 \leq n \leq 50,\ 1 \leq t \leq 5$$ |

数据保证 $$m$$ 是质数。

## 来源

[NEUOJ 1372](http://oj.neauacm.cn/problem.php?id=1372)，[HDU 6429](http://acm.hdu.edu.cn/showproblem.php?pid=6429)

