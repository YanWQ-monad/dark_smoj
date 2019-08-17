# 2942 面积

## 题目描述

在数学上，克罗内克积（记作 $$\otimes$$），是一个矩阵间的运算，它的具体定义如下：

定义矩阵 $$A,\,B$$，大小分别为 $$k \times l$$ 和 $$n \times m$$。他们的克罗内克积是一个 $$kn \times lm$$ 的矩阵 $$C$$：

$$
\left(\begin{array}{cccc}{a_{11} B} & {a_{12} B} & {\cdots} & {a_{1 l} B} \\ {a_{21} B} & {a_{22} B} & {\cdots} & {a_{2 l} B} \\ {\vdots} & {\vdots} & {\ddots} & {\vdots} \\ {a_{k 1} B} & {a_{k 2} B} & {\cdots} & {a_{k l} B}\end{array}\right)
$$

每一个 $$a_{i j} B$$ 代表一个 $$m \times n$$ 的子矩阵：

$$
\left(\begin{array}{cccc}{a_{i j} b_{11}} & {a_{i j} b_{12}} & {\cdots} & {a_{i j} b_{1 n}} \\ {a_{i j} b_{21}} & {a_{i j} b_{22}} & {\cdots} & {a_{i j} b_{2 n}} \\ {\vdots} & {\vdots} & {\ddots} & {\vdots} \\ {a_{i j} b_{m 1}} & {a_{i j} b_{m 2}} & {\cdots} & {a_{i j} b_{m n}}\end{array}\right)
$$

考虑矩阵 $$A=\left(\begin{array}{cc}{+1} & {+1} \\ {+1} & {-1}\end{array}\right)$$，定义 $$A^{2}=A \otimes A,\, A^{3}=A^{2} \otimes A,\, \dots,\, A^{p}=A^{p-1} \otimes A$$。

最后，我们定义 $$A^{\infty}$$ 为一个无穷的二维数表。可以把这个数表的左上角的数的坐标看作为 $$(0,\,0)$$。

定义两个数表中的坐标是相互连通的，当且仅当这两个坐标间存在一条路径，使得路径中任意相邻的位置上的数相同且有一条公共边。

小 D 想知道，对于给定的坐标 $$(x,\,y)$$，它所在的连通块大小是多少，即有多少个坐标和它连通。

## 输入格式

一行两个整数 $$x,\,y$$，表示给定的坐标。

## 输出格式

输出一行一个整数 $$Ans$$，表示连通块的大小，如果连通块的大小是无穷的，输出 `infinity`。

## 输入样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.in" %}
```text
2 3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.out" %}
```text
5
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输入样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.in" %}
```text
1 4
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.out" %}
```text
infinity
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 样例解释

### 样例 1

矩阵前几行几列为：

```text
1  1  1  1  1  1 ...
1 -1  1 -1  1 -1 ...
1  1 -1(-1) 1  1 ...
1 -1 -1  1  1 -1 ...
1  1  1  1 -1 -1 ...
.  .  .  .  .  .
.  .  .  .  .  .
.  .  .  .  .  .
```

被 `()` 标出的即为询问的位置。

它所在的连通块的大小为 5。

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 20% | $$0 \leq x,\,y \leq 100$$ |
| 50% | $$0 \leq x,\,y \leq 10^4$$ |
| 100% | $$0 \leq x,\,y \leq 10^9$$ |

