# 2690 去字母

## 题目描述

给你两个字符串 $$S$$ 和 $$T$$，设 $$n$$ 为 $$S$$ 长度，$$m$$ 为 $$T$$ 长度，现在保证 $$T$$ 是 $$S$$ 的子序列，还给你一个排列 $$p$$，表示有个人操作 $$n$$ 次，第 $$i$$ 次操作是删除 $$S_i$$。

现在问最多删除多少次，使得删除完之后的新字符串 $$S’$$ 满足 $$T$$ 仍然是 $$S’$$ 的子序列。

## 输入格式

第一行一个字符串 $$S$$。

第二行一个字符串 $$T$$。

接下来一行有 $$n$$ 个数，表示序列 $$p$$。

## 输出格式

输出满足要求的最多删除次数。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
ababcba
abb
5 3 4 1 7 6 2
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

删了 3 次之后得到字符串 `abba`，依然满足。

删 4 次之后会得到 `bba`，不满足。

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 40% | $$1 \leq n, m \leq 10^3$$ |
| 100% | $$1 \leq n, m \leq 10^5$$ |

数据保证字符串只由小写字母组成，且 $$p$$ 是一个序列。

## 来源

[Codeforces Round \#402 \(Div. 1\) A](https://codeforces.com/contest/778/problem/A)

