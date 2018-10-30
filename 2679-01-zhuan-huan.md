# 2679 01转换

## 题目描述

给定两个长度相同的 01 串 $$S$$ 和 $$T$$，问从串 $$S$$ 转化到串 $$T$$ 最少需要对 $$S$$ 操作多少次。

一共有两种操作：

1. 将串的第一个元素翻转；
2. 找到串的第一个 1 出现的位置 $$x$$，将位置 $$x+1$$ 的元素翻转。

## 输入格式

第一行一个正整数 $$n$$。

接下来一行一个长度为 $$n$$ 的 01 串，表示 $$S$$。

接下来一行一个长度为 $$n$$ 的 01 串，表示 $$T$$。

## 输出格式

对于每组数据，输出相应的答案模 `1000000007`。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
3
111
000
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

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 30% | $$1 \leq n \leq 15$$ |
| 60% | $$1 \leq n \leq 30$$ |
| 100% | $$1 \leq n \leq 50$$ |
