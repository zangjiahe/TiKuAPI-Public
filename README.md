

# 网课题库API

> v1.0.0

Base URLs:

* <a href="https://api.bcaqfy.xin:8443">请求地址:https://api.bcaqfy.xin:8443</a>

##购买加Q:11504209

## GET 远程查题

GET /tiku/search

### 请求参数

|名称|位置|类型|必选|说明|
|---|---|---|---|---|
|keyword|query|string| 是 |需要查询的题目|
|token|query|string| 是 |购买所得token秘钥|

> 返回示例

> 成功

```json
{
  "data": {
    "question": "护士查房时观察到某急性胰腺炎病人偶有阵发性的肌肉抽搐。最可能的原因是",
    "answer": "低钙反应",
    "times": 952
  },
  "code": 200,
  "msg": "查询成功！"
}
```

### 返回结果

|状态码|状态码含义|说明|数据模型|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### 返回数据结构

状态码 **200**

|名称|类型|必选|约束|中文名|说明|
|---|---|---|---|---|---|
|» data|object|true|none||响应数据|
|»» question|string|true|none||所查询问题|
|»» answer|string|true|none||查询所得答案|
|»» times|integer|true|none||当前token剩余次数|
|» code|integer|true|none||响应状态|
|» msg|string|true|none||响应消息|

# 数据模型


