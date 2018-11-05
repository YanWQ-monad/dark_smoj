# 2697 增援前线

## 题目描述

小 X 的国家正在遭受袭击，必须抽调一些魂师上前线增援。

到前线用时最短的路上有一条宽度为 $$n$$ 米的河，而前来增援的魂师每飞行 $$l$$ 米就必须在一片荷叶上休息一下，才能够继续飞行。当然，魂师们也可以选择没飞够 $$l$$ 米就先休息一下，但不能一次飞超过 $$l$$ 米。

距离河的一侧距离为 $$i$$ 的荷叶共有 $$a_i$$ 片，每片荷叶在有魂师停于上方休息后，就会沉入水底，不能够再供其它魂师休息。

现在小 X 想要知道，至多有多少名魂师能够抵达前线。

## 输入格式

第一行输入两个整数 $$n,\,l$$，含义见题面描述。

接下来一行 $$n-1$$ 个整数 $$a_i$$，表示距离河的一侧距离为 $$i$$ 的荷叶的片数。

## 输出格式

输出一行一个整数，表示至多能够抵达前线的魂师数量。

## 输入样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.in" %}
```text
10 5
0 0 1 0 2 0 0 1 0
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.out" %}
```text
3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输入样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.in" %}
```text
10 3
1 1 1 1 2 1 1 1 1
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.out" %}
```text
3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 样例解释

对于样例 1，三名魂师可以分别走 $$0 \rightarrow 5 \rightarrow 10$$，$$0 \rightarrow 5 \rightarrow 10$$，$$0 \rightarrow 3 \rightarrow 8 \rightarrow 10$$。

对于样例 2，三名魂师可以分别走 $$0 \rightarrow 1 \rightarrow 4 \rightarrow 7 \rightarrow 10$$，$$0 \rightarrow 2 \rightarrow 5 \rightarrow 8 \rightarrow 10$$，$$0 \rightarrow 3 \rightarrow 6 \rightarrow 9 \rightarrow 10$$。

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 20% | $$l = n - 1$$ |
| 50% | $$1 \leq l < n \leq 5,\ 0 \leq a_i \leq 3$$ |
| 80% | $$1 \leq l < n \leq 100,\ 0 \leq a_i \leq 10$$ |
| 100% | $$1 \leq l < n \leq 10^5,\ 0 \leq a_i \leq 10^4$$ |

## 来源

[JZOJ 5948](https://jzoj.net/senior/#main/show/5948)

