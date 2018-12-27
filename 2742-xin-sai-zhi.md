# 2742 新赛制

## 题目描述

有 $$n$$ 个选手参加最近一次 NOIp 比赛，但这次比赛的赛制有了根本的改变！当比赛结束后，所有选手的源代码都公开，随便查看代码，进入“挑战”阶段。每位学生都有一次机会可以“挑战”某一个选手的代码，“挑战”的结果有两种可能：

1. 挑战成功；
2. 挑战失败。

如果是挑战成功，那么被挑战的选手就会“被淘汰”。

挑战阶段全部结束后，给出如下的信息：

1. 给出 1 个数组 $$a$$，如果 $$a_i$$ 等于 `Y`，表示第 $$i$$ 个选手在挑战阶段“挑战”了某个选手（挑战的结果可能是成功也可能是失败），如果 $$a_i$$ 等于 `N` 表示第 $$i$$ 个选手在挑战阶段没有“挑战”任何选手。一个选手最多只会挑战一人（选手不能挑战自己）。
2. 再给出 1 个数组 $$b$$，如果 $$b$$ 等于 `Y`，表示第 $$i$$ 个选手最终"被挑战成功"了（即被淘汰了）。如果 $$b_i$$ 等于 `N` 表示第 $$i$$ 个选手没有"被挑战成功"（即不会被淘汰）。一个选手不会"被挑战成功"多次。
3. 当选手"被挑战成功"后，该选手知道自己被淘汰了，变得很失落，该选手不会发起任何挑战了。
4. 选手可以“被挑战失败”多次。比如：很多选手都挑战你，但可能都“挑战失败”了。
5. 当选手（不妨设为 $$x$$）“被挑战成功”后，其他选手还可以继续挑战选手 $$x$$，但结果一定是“挑战失败”，也就是说 $$x$$ 最多只会被“挑战成功” 1 次。

选手之间的“挑战”不会有时间上的重叠，也就是说，所有的“挑战”都有严格的时间上的先后次序。问有多少种不同的挑战方案满足上面的所有要求？答案模 `1000000007`。如果没有任何方案能满足上述的要求，输出 0。

## 输入格式

多组测试数据。

第一行，一个整数 $$g$$。

每组测试数据格式如下：

第一行，一个整数 $$n$$。

第二行，$$n$$ 个字符，第 $$i$$ 个字符是 $$a_i$$。

第三行，$$n$$ 个字符，第 $$i$$ 个字符是 $$b_i$$。

## 输出格式

共 $$g$$ 行，每行一个整数。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
3
2
YY
NY
4
YYNN
NNYY
4
YNNN
NYYY
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
1
4
0
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

$$1 \leq g \leq 5$$，$$1 \leq n \leq 2500$$。
