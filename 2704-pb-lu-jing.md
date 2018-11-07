# 2704 PB路径

## 题目描述

有 $$n$$ 个城市和 $$m$$ 条单向边，每条边有三个参数 $$x,\,y,\,z$$，表示这条边从 $$x$$ 出发到达 $$y$$，类别是 $$z$$。若 $$z=0$$，则这条路是人行道，称为 P；若 $$z=1$$，则这条路是自行车道，称为 B。

现在称字符串 $$S$$ 是按以下方式生成的无穷串：`P`，`PB`，`PBBP`，`PBBPBPPB`，`PBBPBPPBBPPBPBBP`，……

即 $$S$$=`PBBPBPPBBPPBPBBP...`

有个人想从城市 1 出发，一开始令字符串 $$T=\text{""}$$ 通过这些单向道路一直移动，每经过一条边 P 就令 $$T=T+’P’$$，每经过一条边 B 就令 $$T=T+’B’$$。

现在一定要求 $$T$$ 是 $$S$$ 的前缀，想问尽可能长的 $$S$$ 有多长，如果长度严格大于 $$10^{18}$$，输出 `-1`，否则输出对应的长度。

## 输入格式

第一行两个整数 $$n$$ 和 $$m$$。

接下来 $$m$$ 行，每行三个数 $$x,\,y,\,z$$。

## 输出格式

输出最长的 $$S$$ 的长度，如果长度严格大于 $$10^{18}$$，输出 `-1`，否则输出对应的长度。

## 输入样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.in" %}
```text
2 2
1 2 0
2 2 1
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
2 3
1 2 0
2 2 1
2 2 0
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.out" %}
```text
-1
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 30% | $$1 \leq n \leq 15$$ |
| 50% | $$1 \leq n \leq 100$$ |
| 100% | $$1 \leq n \leq 500,\ 0 \leq m \leq 2n^2$$ |

数据保证对于任意两条边 $$i,\,j$$，满足 $$x_i \not = x_j$$ 或 $$y_i \not = y_j$$ 或 $$z_i \not = z_j$$，可能有自环。

