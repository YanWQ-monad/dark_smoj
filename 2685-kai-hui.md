# 2685 开会

## 题目描述

现在有 $$n$$ 个人，每个人住在 $$(x_i, y_i)$$ 处，再给一个距离限制 $$d$$，现在你要找出一个开会地点 $$M(xx, yy)$$ 满足以下条件：

1. $$xx, yy$$ 是整数
2. 离 $$M$$ 最远的人距离不超过 $$d$$。
3. 所有人离 $$M$$ 的距离和最小。

所有的距离计算方式为：$$(x_a, y_a)$$ 与 $$(x_b, y_b)$$ 的距离为 $$|x_a-x_b| + |y_a-y_b|$$。

现在要求出满足要求的最小距离和。

## 输入格式

第一行一个正整数 $$n$$。

接下来 $$n$$ 行每行两个整数 $$x_i, y_i$$。

接下来一个整数 $$d$$。

## 输出格式

输出满足要求的最小距离和，无解输出 `impossible`。

## 输入样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.in" %}
```text
5
3 1
4 1
5 9
2 6
5 3
5
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.out" %}
```text
20
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输入样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.in" %}
```text
5
3 1
4 1
5 9
2 6
5 3
4
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.out" %}
```text
impossible
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 20% | $$1 \leq n \leq 10^3$$ |
| 另外 30% | $$0 \leq x_i, y_i \leq 10^3$$ |
| 100% | $$1 \leq n \leq 10^5,\ 0 \leq x_i, y_i, d \leq 10^9$$ |

