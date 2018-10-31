# 2678 或和

## 题目描述

给定两个整数 $$a,\,b$$，求 $$a \operatorname{or} (a+1) \operatorname{or} (a+2) \operatorname{or} \cdots \operatorname{or} b$$ 和 $$a \operatorname{and} (a+1) \operatorname{and} (a+2) \operatorname{and} \cdots \operatorname{and} b$$。

## 输入格式

第一行一个 $$t$$，表示数据组数。

接下来 $$t$$ 行，每行两个正整数 $$a$$ 和 $$b$$。

## 输出格式

对于每组测试数据，按照格式输出相应的答案。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
2
1 1
1 2
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
Case 1: 1 1
Case 2: 3 0
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

| 数据点 | 范围 |
| :---: | :---: |
| 40% | $$1 \leq a \leq b \leq 100$$ |
| 100% | $$1 \leq t \leq 10^4,\ 1 \leq a \leq b \leq 10^9$$ |



