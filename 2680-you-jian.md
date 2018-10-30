# 2680 邮件

## 题目描述

给出若干个字符串，问这些字符串中一共出现了多少个不同的有效的 email。一个有效的 email 组成为“用户名`@`域名”，用户名和域名都不能以 `.` 为开头和结尾，也不能出现连续两个 `.`。

## 输入格式

若干行，每行一个字符串。

## 输出格式

输出一行一个数，表示所有字符串中不同的有效 email 的个数。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
a.b@c.d
b@c.de.
@qq
q@.q
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
5
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 样例解释

合法的 email 有：`a.b@c`, `a.b@c.d`, `b@c`, `b@c.d`, `b@c.de`。

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 30% | $$1 \leq l \leq 200$$ |
| 60% | $$1 \leq l \leq 10^3$$ |
| 100% | $$1 \leq l \leq 5 \times 10^5$$ |

其中 $$l$$ 为字符串总长度，且所有字符均为 `@`, `.`, 小写字母以及换行。

