# 2957 连通

## 题目描述

战争刚结束时，帝国的道路几乎全部破坏，剩下的道路将帝国的个个城市连成了 $$n$$ 个联通块，在同一个联通块中的城市可以互相到达。帝国的道路建设计划共有 $$m$$ 天，每天会建好一条 $$u$$ 号联通块和 $$v$$ 号联通块的道路。但由于工期很紧，造出道路仅能单向通行，即只能从 $$u$$ 走到 $$v$$。

而谭雅的任务就是统计 $$q$$ 对重要城市对之间的关系，具体的说，对于一对重要城市对 $$x,\,y$$，假设，谭城市 $$x$$ 属于联通块 $$u$$，城市 $$y$$ 属于联通块 $$v$$，雅希望知道最早什么时候，$$u$$ 号联通块和 $$v$$ 号联通块可以互相到达。

## 输入格式

第一行读入 $$n,\,m,\,q$$，表示联通块数、建设天数和重要城市对个数。

第 2 到 $$m + 1$$ 行，第 $$i$$ 行读入 $$u_i,\,v_i$$，表示第 $$i - 1$$ 天建造的道路是 $$u_i$$ 到 $$v_i$$ 的单向道路。

接下来 $$q$$ 行，每行读入 $$u,\,v$$，表示有一对重要城市对的两座城市分别属于 $$u,\,v$$ 联通块。

## 输出格式

输出 $$q$$ 行，每行一个整数，表示两个联通块最早什么时候可以互相到达，如果在 $$m$$ 时刻仍不能互相到达，输出 `-1`。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
4 5 4
1 2
2 3
2 1
1 4
3 1
2 2
2 4
1 3
1 2
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
0
-1
5
3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

对于所有数据，满足 $$1 \leq n \leq 10^5$$，$$1 \leq m,\,q \leq 2 \times 10^5$$。

| SubTask 编号 | 分数 | 特殊性质 |
| :---: | :---: | :---: |
| 1 | 15 | $$1 \leq n \leq 100,\ 1 \leq m,\,q \leq 200$$ |
| 2 | 21 | $$1 \leq n \leq 2000,\ 1 \leq m \leq 3000,\ 1 \leq q \leq 10^4$$ |
| 3 | 17 | $$m$$ 为偶数，对于任意正整数 $$k$$ 满足 $$2k \leq m$$， 必定存在 $$u_{2k} = v_{2k - 1},\ v_{2k} = u_{2k - 1}$$ |
| 4 | 24 | $$1 \leq q \leq 10$$ |
| 5 | 23 | 无 |


