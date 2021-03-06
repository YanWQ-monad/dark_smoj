# 2935 先知系统

## 题目描述

西比拉先知系统是一个强大的心灵指数监测网絡，能以声像扫描主动监控市民的心智与精神状态。为了判定出更复杂的人类心理参数，西比拉系统纳入了不同于既存人类规范的超群人格——不会随意和他人产生共鸣，也不会感情用事，能以非人类的眼光来俯瞰并裁定人类。

被纳入的超群人格会相互影响，共同处理数据。他们之间具体的影响方式形如一张无向图，如果你对一个节点进行操作，和这个节点相邻的节点也会受到相同的影响。

操作有一种：使一个节点的权值加上 $$x$$。

同时你还希望询问一个节点的权值（每一个节点的初始权值为 0）。

## 输入格式

第一行读入 $$n,\,m,\,q$$，表示节点个数和边数，以及操作和询问的总数。

接下来 $$m$$ 行，每行两个数 $$u_i,\,v_i$$，表示 $$u_i,\,v_i$$ 之间有连边。

接下来 $$q$$ 行，每行先读入一个 `type`。

* `type=0` 表示一个询问，读入一个 $$x$$，表示询问 $$x$$ 节点的权值。
* `type=1` 表示一个操作，读入 $$x,\,y$$，表示将 $$x$$ 节点的权值加上 $$y$$（与 $$x$$ 相邻的节点权值也要加上 $$y$$）。

## 输出格式

对于每一行询问输出一行，表示该节点的权值。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
4 4 4
1 2
1 3
1 4
2 3
1 1 1
0 2
1 3 3
0 2
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
1
4
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

对于所有的测试点，$$1 \leq n,\,m,\,q \leq 3 \times 10^5$$，$$y \leq 10^3$$。

| SubTask 编号 | 分数 | 特殊性质 |
| :---: | :---: | :---: |
| 1 | 31 | $$n,\,m,\,q \leq 3 \times 10^3$$ |
| 2 | 17 | 任意两个点之间一定满足不连通或存在恰好一条路径，且这条路径的长度不超过 2 |
| 3 | 25 | 除了 1 号节点以外，所有节点的度数小于 10 |
| 4 | 27 | 无 |

