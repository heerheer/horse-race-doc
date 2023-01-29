---
description: 使用json表示简单的逻辑...
---

# 行为(Action)

## 行为对象

```json
{
    "action": "log",
    "data": {},
    "var": "",
    "conditions": []
}
```

<table><thead><tr><th>属性</th><th>类型</th><th>描述</th><th data-type="checkbox">必选</th></tr></thead><tbody><tr><td>data</td><td>object</td><td>针对action的参数与数据</td><td>true</td></tr><tr><td>action</td><td>string</td><td>动作的名字，中英都可使用</td><td>true</td></tr><tr><td>var</td><td>string</td><td>将action的返回值进行赋值于一个变量，会自动创建变量空间</td><td>false</td></tr><tr><td>conditions</td><td>array&#x3C;condition></td><td>用于判断是否执行动作的条件</td><td>false</td></tr></tbody></table>

在载入行为时，行为名会被进行一定的解析，以便于使得编写时更加易用。

### 中文模式

不推荐使用中文编写，但可以根据行为列表中的中文，在解析后自动会转化为英文识别。

`行为名`

### 英文模式

## 行为名

`actionName`

`action-name`

`ActionName`
