---
description: 用于进行关键表述
---

# 📋 标签

## 标签的作用

标签可以将事件、契约等内容进行高度概括。同时，也可作为内容本身的属性，与其他内容联动。

## 如何编写标签

### 规范

我们有如下规范的标签方案。

通常情况下,对于自身而言，<mark style="color:blue;">蓝色</mark>被定义为有利（加速），<mark style="color:orange;">橙色</mark>定义为不利（后退）

但是如果发生的改变是不针对自身的，需要使用相对应的 <mark style="color:purple;">紫色（对其他选手有利）</mark> / <mark style="color:green;">绿色（对其他选手不利）</mark> 标签。

若随机内容计算期望后没有改变可以设定为 黑色

这些颜色不需要进行额外编写，可以在编写时根据type自动生成。

| type        | 描述 | value |
| ----------- | -- | ----- |
| self\_good  |    | 0     |
| self\_bad   |    | 1     |
| other\_good |    | 2     |
| other\_bad  |    |       |
| normal      |    |       |

{% hint style="info" %}
任何附带随机元素的事件都必须包含 随机 标签。
{% endhint %}

#### 步数更改

若发生了步数更改，应该编写 <mark style="color:blue;">加速</mark>/<mark style="color:orange;">减速</mark> 标签

若是随机步数更改，应该编写 <mark style="color:blue;">随机加速</mark>/<mark style="color:orange;">随机减速</mark> 这里加速减速的设定可以按照数学期望设定。

传送&#x20;

#### 增益、减益效果

<mark style="color:blue;">增益效果</mark> <mark style="color:orange;">减益效果</mark> <mark style="color:blue;">无敌</mark> <mark style="color:orange;">眩晕</mark>

#### 场地影响

地形改变 障碍物 交换



<mark style="color:orange;"></mark>
