# 2689 排列问题

## 题目描述

给出一个长度为 $$n$$ 的静态排列 $$b[]$$ 和 $$q$$ 个操作。

每个操作如下：

1. `add x y`，表示将 $$a_x, a_{x+1},\cdots,a_y$$ 的值都加一。
2. `query x y`，表示询问 $$\sum_{i=x}^{y}\lfloor \frac{a_i}{b_i} \rfloor$$ 。

数组 $$a$$ 初始化为 0。

## 输入格式

若干行组测试数据：

每组数据第一行两个整数 $$n$$ 和 $$q$$。

接下来一行有 $$n$$ 个整数，表示排列 $$b$$ 。

接下来有 $$q$$ 行，每行表示一个操作。

## 输出格式

对于每组数据，对于每个 `query`，输出相应的求值结果。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
5 12
1 5 2 4 3
add 1 4
query 1 4
add 2 5
query 2 5
add 3 5
query 1 5
add 2 4
query 1 4
add 2 5
query 2 5
add 2 2
query 1 5
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
1
1
2
4
4
6
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 40% | $$1 \leq n, q \leq 10^3$$  |
| 100% | $$1 \leq n, q \leq 10^5,\ t \leq 5$$  |

 保证操作合法并且 ****$$b$$ 是一个排列。

## 来源

[HDU 6315](http://acm.hdu.edu.cn/showproblem.php?pid=6315)

