# 2805 染色

## 题目描述

有个 $$r$$ 行 $$c$$ 列的二维表格，行的编号从上往下是 0 至 $$r-1$$，列编号从左往右是 0 至 $$c-1$$，二维表格共被分成 $$r \times c$$ 个单元格子。每个单元格子一开始都是白色。

现在要执行 $$k$$ 条指令，每条指令的步骤是：

1. 随机从二维表格里选取一个单元格子（不妨称为 A 格子）
2. 随机从二维表格里选取一个单元格子（不妨称为 B 格子）
3. 格子 A 和 B 确定了一个矩形，矩形里面所有的单元格子都会被染色。

每个单元格随机选择，均匀分布，每个选择独立于其他选择。A 和 B 可能对应于同一个单元格。

你的任务是：执行 $$k$$ 条指令后，有多少个单元格子会被染上颜色？输出该期望值。

## 输入格式

多组测试数据。

第一行，一个整数 $$g$$，表示有 $$g$$ 组测试数据。

每组测试数据格式：

一行，3 个整数：$$k,\,r,\,c$$。

## 输出格式

一个实数。你的输出与标准答案的误差不能超过 $$10^{-6}$$。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
4
1 2 1
2 2 1
1 2 2
3 5 7
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
1.5
1.875
2.25
19.11917924647044
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

$$1 \leq g \leq 6$$，$$0 \leq k \leq 100$$，$$1 \leq r,\,c \leq 10^3$$。

## 来源

[Single Round Match 409 Round 1 - Division I, GridColoring](https://community.topcoder.com/stat?c=problem_statement&pm=8012)

