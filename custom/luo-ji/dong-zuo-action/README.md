---
description: 使用json表示简单的逻辑...
---

# 动作(Action)

## 动作对象

```json
{
    "action": "log",
    "data": {},
    "var": "",
    "conditions": []
}
```

<table><thead><tr><th>属性</th><th>类型</th><th>描述</th><th data-type="checkbox">必选</th></tr></thead><tbody><tr><td>data</td><td>object</td><td>针对action的参数与数据</td><td>true</td></tr><tr><td>action</td><td>string</td><td>动作的名字，中英都可使用</td><td>true</td></tr><tr><td>var</td><td>string</td><td>将action的返回值进行赋值于一个变量，会自动创建变量空间</td><td>false</td></tr><tr><td>conditions</td><td>array&#x3C;condition></td><td>用于判断是否执行动作的条件</td><td>false</td></tr></tbody></table>

## 可用动作列表

### 赛场动作

| 动作      | 描述                   |
| ------- | -------------------- |
| log     | 输出赛场日志               |
| addCoin | 添加小马积分，若为负值，则会减少小马积分 |
|         |                      |

### 逻辑动作

| 动作        | 描述            |
| --------- | ------------- |
| getRandom | 获取一个随机数值      |
| eval      | 执行js代码，并获得返回值 |
|           |               |
|           |               |
