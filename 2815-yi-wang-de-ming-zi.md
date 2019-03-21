# 2815 遗忘的名字

## 题目背景

> 我是 达拉崩巴斑得⻉迪⼘多⽐鲁翁  
> 是不是 达拉崩巴斑得⻉迪⼘多⽐鲁翁  
> 我是 昆图库塔卡提考特苏⽡西拉松  
> 是不是 昆特牌提琴烤蛋挞苏打⻢拉松

由此可⻅，⻓名字不便于记忆。

## 题目描述

牧牧有⼀个多年不⻅的朋友，他的名字就很⻓很⻓。这天他们在餐馆⾥碰⾯了，这让牧牧⼗分的尴尬——因为牧牧⼀时想不起来他的名字，更⽆法称呼。

所幸牧牧的备忘录⾥写了⼀些有关他的特征信息，你可以根据这些信息来找到最有可能的名字，牧牧希望你能帮助他避免尴尬。

朋友的名字 $$T$$ 是⼀个**仅包含⼩写字⺟的字符串**。特征信息⼀共由 $$n$$ 个**仅包含⼩写字⺟的字符串** $$\{ S_i \}$$ 组成。牧牧认为⼀个字符串是**特征字符串**，当且仅当它**⾄少**是⼀个特征信息的⼦串。⽽朋友的名字的任意⼀个⻓度**不超过** $$k$$ 的⼦串都必须是**特征字符串**。

因为朋友的名字真的很⻓，你找到的 $$T$$ 越⻓正确率就越⾼，因此你需要告诉牧牧满⾜要求的最⻓的 $$T$$ ，如果这样的 $$T$$ 有多个，任意输出⼀个即可。如果 $$T$$ 可以⽆限⻓，输出 `INF`。

## 输入格式

第⼀⾏两个整数 $$n,\,k$$，含义同题⽬描述。

接下来 $$n$$ ⾏，每⾏⼀个字符串，表⽰ $$S_i$$。

## 输出格式

输出⼀⾏⼀个字符串表⽰ $$T$$，或 `INF`。

## 输入样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.in" %}
```text
1 3
abaaba
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.out" %}
```text
INF
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输入样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.in" %}
```text
3 4
abskbak
kbakioindui
jinduiwenle
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.out" %}
```text
abskbakioinduiwenle
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

* 对于 10% 的数据， $$\sum | S_i |$$；
* 对于 25% 的数据， $$k \leq 4$$；
* 对于 50% 的数据， $$\sum | S_i | \leq 10^3$$；
* 对于 100% 的数据， $$\sum | S_i | \leq 10^6$$。

