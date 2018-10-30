# 2658 光

## 题目描述

给出一棵点数为 $$n$$ 的树。

现在有 $$m$$ 个询问，每次给出 $$u,\,v,\,w$$，表示在 $$u$$ 和 $$v$$ 这两个点放置光源，使得与 $$u$$ 或者 $$v$$ 距离不超过 $$w$$ 的所有点（$$u$$ 和 $$v$$ 考虑在内）被照亮，问有多少点被照亮。每个询问独立。

数据加密，读入的数是 $$uu$$、$$vv$$、$$ww$$，满足 $$u=((uu+lastans)\mod n)+1$$, $$v=((vv+lastans)\mod n)+1$$, $$w=(ww+lastans)\mod n$$，其中 $$lastans$$ 是上一次询问的答案，$$lastans$$ 初始化为 0。

## 输入格式

第一行一个 $$t$$ 表示数据组数。

每组数据第一行两个整数 $$n,\,m$$。 

接下来有 $$n-1$$ 行，每行两个正整数 $$x,\,y$$，树上有边 $$x  \leftrightarrow y$$。

接下来有 $$m$$ 行，每行三个整数 $$uu,\,vv,\,ww$$，表示加密的数据。

## 输出格式

对于每组测试数据的每个询问，输出答案。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
1
5 5
1 2
2 3
2 4
3 5
5 1 0
3 4 4
1 2 3
5 1 3
5 1 4
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
2
4
5
5
5
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 30% | $$1 \leq n, m \leq 10^3$$ |
| 另外 20% | 树是一条链 |
| 100% | $$1 \leq n, m \leq 10^5,\ 1 \leq t \leq 2$$ |

数据保证给出一棵树，且 $$1 \leq uu, vv, ww < n$$。

