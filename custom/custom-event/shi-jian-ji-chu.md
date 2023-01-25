---
description: 愿...
---

# 事件基础

## 配置文件

我们可以用一个JSON文件表示一个事件。

<pre class="language-json"><code class="lang-json">{
    "name":"大钱包",
    "desc":"选手捡到了大钱包，获得随机(20000-46000)小马积分",
    "actions":[
<strong>        {
</strong>            "action":"getRandom",
            "data":{
                "min":20000,
                "max":46000
            },
            "var":"r_coin" //将action的返回值进行一个变量的赋值
        },
        {
            "action":"addCoin",
            "data":{
                "coin": "%r_coin%" //使用文本 %var% 来进行变量的使用
            }
        },
        {
            "action":"log",
            "data":{
                "content":"%horse_name%在奔跑的事后捡到了一个大钱包!获得了%r_coin%小马积分!"
            }
        }
    ]
}
</code></pre>

<table><thead><tr><th>属性</th><th>描述</th><th data-type="checkbox">必填</th></tr></thead><tbody><tr><td>name</td><td>事件名称</td><td>true</td></tr><tr><td>desc</td><td>事件显示在卡片的描述，不会使用变量。可以参考<mark style="color:blue;">事件描述表达</mark></td><td>true</td></tr><tr><td>actions</td><td>行为数组，不填写则不会发生任何事。</td><td>false</td></tr><tr><td>author</td><td>作者</td><td>false</td></tr></tbody></table>

## 编写事件逻辑

请参考 [luo-ji](../luo-ji/ "mention") 部分
