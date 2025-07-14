# 全局公共参数

**全局Header参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| 暂无参数 |

**全局Query参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| 暂无参数 |

**全局Body参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| 暂无参数 |

**全局认证方式**

> 无需认证

# 状态码说明

| 状态码 | 中文描述 |
| --- | ---- |
| 暂无参数 |

# 下单

> 创建人: zzzzzga

> 更新人: zzzzzga

> 创建时间: 2025-07-14 13:48:24

> 更新时间: 2025-07-14 13:51:34

```text
暂无描述
```

**接口状态**

> 开发中

**接口URL**

> /api/buyEmailOrder/open/buy

| 环境  | URL |
| --- | --- |


**Mock URL**

> /api/buyEmailOrder/open/buy?apipost_id=3606348233f4b6

**请求方式**

> POST

**Content-Type**

> json

**请求Header参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| Authorization | bd4d7f193ebc4ffc8558ebf18dbc2b84 | string | 是 | API密钥 |

**请求Body参数**

```javascript
{
    "platformId":"68708da21ef8267d7f1114fb",
    "buyNum": 1
}
```

**认证方式**

> 继承父级

**响应示例**

* 成功(200)

```javascript
暂无数据
```

**请求Header参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| Authorization | bd4d7f193ebc4ffc8558ebf18dbc2b84 | string | 是 | API密钥 |

**Query**

# 平台

> 创建人: zzzzzga

> 更新人: zzzzzga

> 创建时间: 2025-07-14 13:48:43

> 更新时间: 2025-07-14 13:51:32

```text
暂无描述
```

**接口状态**

> 开发中

**接口URL**

> /api/buyEmailOrder/open/accountPlatformList

| 环境  | URL |
| --- | --- |


**Mock URL**

> /api/buyEmailOrder/open/accountPlatformList?apipost_id=3606468ab3f4b8

**请求方式**

> POST

**Content-Type**

> json

**请求Header参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| Authorization | bd4d7f193ebc4ffc8558ebf18dbc2b84 | string | 否 | API秘钥 |

**请求Body参数**

```javascript
{
}
```

**认证方式**

> 继承父级

**响应示例**

* 成功(200)

```javascript
暂无数据
```

**请求Header参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| Authorization | bd4d7f193ebc4ffc8558ebf18dbc2b84 | string | 否 | API秘钥 |

**Query**

# 查询结果

> 创建人: zzzzzga

> 更新人: zzzzzga

> 创建时间: 2025-07-14 13:48:58

> 更新时间: 2025-07-14 13:51:30

```text
暂无描述
```

**接口状态**

> 开发中

**接口URL**

> /api/buyEmailOrder/open/details/{orderNo}

| 环境  | URL |
| --- | --- |


**Mock URL**

> /api/buyEmailOrder/open/details/{orderNo}?apipost_id=3606559db3f4bb

**请求方式**

> POST

**Content-Type**

> none

**请求Header参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| Authorization | bd4d7f193ebc4ffc8558ebf18dbc2b84 | string | 是 | API秘钥 |

**路径变量**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| orderNo | E07111835093783 | string | 是 | 订单号 |

**认证方式**

> 继承父级

**响应示例**

* 成功(200)

```javascript
暂无数据
```

**请求Header参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| Authorization | bd4d7f193ebc4ffc8558ebf18dbc2b84 | string | 是 | API秘钥 |

**Query**
