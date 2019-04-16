# 2859 干草

## 题目描述

有 $$n$$ 头奶牛，$$p$$ 袋干草。每一袋干草都随机的选择分给 $$n$$ 头奶牛中的某一头奶牛。

所有选择都是相互独立的。

当 $$p$$ 袋干草分配结束后，得到干草最多的奶牛是“冠军奶牛”。

但有可能有多头奶牛都是“冠军奶牛”（因为它们得到同样多的干草，而且都是最多的），求出现多头奶牛是“冠军奶牛”的概率。

## 输入格式

多组测试数据。

第一行，一个整数 $$g$$，表示有 $$g$$ 组测试数据。

每组测试数据格式：

第一行，两个整数：$$p$$ 和 $$n$$。

## 输出格式

共 $$p$$ 行，每行一个实数，与标准答案误差不能超过 $$10^{-7}$$。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
5
7 1
2 2
3 3
6 4
50 50
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
0.0
0.5
0.2222222222222222
0.380859375
0.49549217175140714
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

$$1 \leq g \leq 5$$，$$1 \leq n,\,p \leq 51$$。

## 来源

[TCO19 SRM 747 Round 1 - Division I, TieForMax](https://community.topcoder.com/stat?c=problem_statement&pm=15237)

