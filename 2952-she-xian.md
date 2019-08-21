# 2952 射线

## 题目描述

有两条以 $$(0,\,0)$$ 为端点，分别经过 $$(a,\,b)$$，$$(c,\,d)$$ 的射线，你要求出夹在两条射线中间，且距离 $$(0,\,0)$$ 最近的点 $$(x,\,y)$$。

## 输入格式

第一行一个整数 $$t$$，表示数据组数。

接下来 $$t$$ 行，每行四个整数 $$a,\,b,\,c,\,d$$，意义如上。

## 输出格式

输出 $$t$$ 行每行两个整数 $$x,\,y$$，表示每组询问的答案。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
2
2 1 1 1
4 4 7 5
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
3 2
4 3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

对于所有数据，保证两条射线不重合，且 $$0 \leq a,\,b,\,c,\,d$$，$$(a,\,b)$$ 和 $$(c,\,d)$$ 都不为 $$(0,\,0)$$。

| 测试点 | 范围 | 特殊性质 |
| :---: | :---: | :---: |
| 1 | $$1 \leq t \leq 3,\ 0 \leq a,\,b,\,c,\,d \leq 10^3$$ | 无 |
| 2 | $$1 \leq t \leq 3,\ 0 \leq a,\,b,\,c,\,d \leq 10^6$$ | 无 |
| 3 | $$1 \leq t \leq 3,\ 0 \leq a,\,b,\,c,\,d \leq 10^7$$ | 无 |
| 4 | $$1 \leq t \leq 10^6,\ 0 \leq a,\,b,\,c,\,d \leq 10^9$$ | $$a = c,\ b \pm 1 = d$$ |
| 5-6 | $$1 \leq t \leq 10^4,\ 0 \leq a,\,b,\,c,\,d \leq 10^9$$ | 无 |
| 7-8 | $$1 \leq t \leq 10^5,\ 0 \leq a,\,b,\,c,\,d \leq 10^9$$ | 无 |
| 9-10 | $$1 \leq t \leq 10^6,\ 0 \leq a,\,b,\,c,\,d \leq 10^9$$ | 无 |

