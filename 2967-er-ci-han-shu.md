# 2967 二次函数

## 题目描述

给出 $$n$$ 个形如 $$f_i(x) = a_ix^2 + b_ix$$ 的二次函数。

有 $$q$$ 次询问，每次给出一个 $$x$$，询问 $$\max\{f_i(x)\}$$。

## 输入格式

第一行两个正整数 $$n,\,q$$。

接下来的 $$n$$ 行，每行两个整数 $$a_i,\,b_i$$。

接下来的 $$q$$ 行，每行一个整数 $$x$$。

## 输出格式

对于每个询问，输出一行一个整数表示答案。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
2 4
3 0
4 -2
-1
0
1
2
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
6
0
3
12
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

每个测试点 10 分，共 10 个测试点：

| 测试点 | 范围 | 特殊性质 |
| :---: | :---: | :---: |
| 1-2 | $$1 \leq n,\,q \leq 10^4$$ | 无 |
| 3-4 | $$1 \leq n \leq 10^4,\ 1 \leq q \leq 5 \times 10^5$$ | 无 |
| 5-6 | $$1 \leq n \leq 5 \times 10^5,\ 1 \leq q \leq 10^4$$ | 无 |
| 7-8 | $$1 \leq n,\,q \leq 5 \times 10^5$$ | $$| a_i | \leq 1$$ |
| 9-10 | $$1 \leq n,\,q \leq 5 \times 10^5$$ | 无 |

对于所有的数据，有：$$1 \leq  |a_i|,\,|b_i|,\,|x| \leq 32323$$。

