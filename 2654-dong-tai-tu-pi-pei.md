# 2654 动态图匹配

## 题目描述

给出 $$n$$（$$n$$ 偶数）个点的无向图，一开始无边，有两种操作：

1. `+ u v`， 表示往图中加入 $$u \leftrightarrow v$$ 这条无向边，允许多重边。
2. `- u v`，表示从图中删除一条 $$u \leftrightarrow v$$ 的无向边，保证合法。

每操作一次输出一行 $$\frac{n}{2}$$ 个数的信息，第 $$i$$ 个数表示现在图中匹配数为 $$i$$ 的方案数是多少，答案模 `1000000007`。

## 输入格式

第一行一个正整数 $$t$$ 表示数据组数。

每组测试数据第一行两个整数 $$n$$ 和 $$m$$。

接下来有 $$m$$ 行，每行表示一种操作。

## 输出格式

对于每组数据，每次操作后输出相应的答案模 `1000000007`。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
1
4 8
+ 1 2
+ 3 4
+ 1 3
+ 2 4
- 1 2
- 3 4
+ 1 2
+ 3 4
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
1 0
2 1
3 1
4 2
3 1
2 1
3 1
4 2
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 40% | $$2 \leq n \leq 10,\ 1 \leq m \leq 100$$ |
| 100% | $$2 \leq n \leq 10,\ 1 \leq m \leq 3 \times 10^4$$ |

数据保证 $$n$$ 为偶数，且操作合法。$$1 \leq t \leq 5$$。

## 来源

[HDU 6321](http://acm.hdu.edu.cn/showproblem.php?pid=6321)

