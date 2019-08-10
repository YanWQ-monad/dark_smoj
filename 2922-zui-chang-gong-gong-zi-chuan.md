# 2922 最长公共子串

## 题目描述

现在给你 $$n$$ 个字符串，问这 $$n$$ 个字符串的最长公共子串长度是多少？

换句话说，即找到一个长度最小的字符串 $$T$$，使得 $$T$$ 在这 $$n$$ 个字符串中都分别出现。

## 输入格式

若干行，每行一个字符串。

## 输出格式

一个数，即最长公共子串长度，没有就输出 0。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
alsdfkjfjkdsal
fdjskalajfkdsla
aaaajfaaaa
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
2
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 样例解释

`jf`

## 数据范围

令字符串长度为 $$m$$（不是总长度）。

30% 的数据：$$n \leq 2$$，$$m \leq 10^5$$

另外 30% 的数据：$$n \leq 10$$，$$m \leq 10^3$$

100% 的数据：$$n \leq 10$$，$$m \leq 10^5$$

所有字符都是小写字母。

