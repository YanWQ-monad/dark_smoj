# 2830 树与图

## 题目描述

最近有人发明了一款新游戏。给定具有 $$n$$ 个顶点的连通无向图和具有 $$n$$ 个节点的树，尝试以下列方式将该树放置在图上：

* 树的每个节点与图的顶点对应。即每个节点对应一个顶点，每个顶点对应一个节点。
* 如果树的两个节点之间存在边，则图中的相应顶点之间也必须存在边。

现在想知道有多少不同的放置方案，答案模 `1000000007`。

## 输入格式

多组测试数据。

第一行，一个整数 $$g$$，表示有 $$g$$ 组测试数据。

每组测试数据格式如下：

第一行，一个整数 $$n$$。

接下来是 $$n$$ 行 $$n$$ 列的二维数组 $$\text{graph}$$，如果 $$\text{graph}[i][j]$$ 为 `Y` 则表示无向图当中顶点 $$i$$ 和顶点 $$j$$ 之间有 1 条边，否则没边。

接下来是 $$n$$ 行 $$n$$ 列的二维数组 $$\text{tree}$$，如果 $$\text{tree}[i][j]$$ 为 `Y` 则表示树中节点 $$i$$ 和节点 $$j$$ 之间有 1 条边，否则没边。

## 输出格式

共 $$g$$ 行，每行一个整数。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
5

14
NYYYYYYYYYYYYY
YNYYYYYYYYYYYY
YYNYYYYYYYYYYY
YYYNYYYYYYYYYY
YYYYNYYYYYYYYY
YYYYYNYYYYYYYY
YYYYYYNYYYYYYY
YYYYYYYNYYYYYY
YYYYYYYYNYYYYY
YYYYYYYYYNYYYY
YYYYYYYYYYNYYY
YYYYYYYYYYYNYY
YYYYYYYYYYYYNY
YYYYYYYYYYYYYN
NYYYYYYYYYYYYY
YNNNNNNNNNNNNN
YNNNNNNNNNNNNN
YNNNNNNNNNNNNN
YNNNNNNNNNNNNN
YNNNNNNNNNNNNN
YNNNNNNNNNNNNN
YNNNNNNNNNNNNN
YNNNNNNNNNNNNN
YNNNNNNNNNNNNN
YNNNNNNNNNNNNN
YNNNNNNNNNNNNN
YNNNNNNNNNNNNN
YNNNNNNNNNNNNN

2
NY
YN
NY
YN

3
NYN
YNY
NYN
NYY
YNN
YNN

5
NYNNN
YNYYY
NYNYY
NYYNY
NYYYN
NYNNN
YNYNN
NYNYN
NNYNY
NNNYN

6
NYNNNY
YNYNNN
NYNYNN
NNYNYN
NNNYNY
YNNNYN
NYNNYN
YNNYNY
NNNNYN
NYNNNN
YNYNNN
NYNNNN
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
178290591
2
2
12
0
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

$$1 \leq g \leq 10$$，$$1 \leq n \leq 14$$。

## 来源

[Member Single Round Match 474 Round 1 - Division I, GameWithGraphAndTree](https://community.topcoder.com/stat?c=problem_statement&pm=10800)

