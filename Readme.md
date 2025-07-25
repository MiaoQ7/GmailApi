# TNT 邮件API文档

## 查询平台

> 创建人: zzzzzga

```text
查询可用平台
```

**接口URL**

> /api/buyEmailOrder/open/accountPlatformList

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

**响应示例**

* 成功(200)

```javascript
{
	"code": 1,
	"message": "success",
	"data": [
		{
			"_id": "68746b5c2c78de2b6a9c99b2", // ID
			"name": "apple", // 平台名称
			"canUseAccountNumber": 124, // 可用库存
			"sortNo": 999, // 排序号
			"icon": "platform/apple-1752460074029.png", // 图标
			"price": 1, // 单价
			"displayStatus": true // 显示
		},
		{
			"_id": "68747f19fbdb497d77a6e65f",
			"name": "ces",
			"canUseAccountNumber": 126,
			"sortNo": 0,
			"icon": "platform/1-1752465152482.png",
			"price": 1,
			"displayStatus": true
		}
	]
}
```

## 下单

> 创建人: zzzzzga

```text
下单购买邮箱
```

**接口URL**

> /api/buyEmailOrder/open/buy

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

**响应示例**

* 成功(200)

```javascript
{
	"code": 1,
	"message": "success",
	"data": "E07141416547128" // 订单号
}
```

## 查询验证码结果

> 创建人: zzzzzga

```text
查询获取的验证码
```

**接口URL**

> /api/buyEmailOrder/open/details/{orderNo}

**请求方式**

> POST

**Content-Type**

> json

**请求Header参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| Authorization | bd4d7f193ebc4ffc8558ebf18dbc2b84 | string | 是 | API秘钥 |

**路径变量**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| orderNo | E07111835093783 | string | 是 | 订单号 |

**响应示例**

* 成功(200)

```javascript
{
	"code": 1,
	"message": "success",
	"data": [
		{
			"_id": "6874a0d86019e853e292611e", // ID
			"orderDetailNo": "E07141416547128000000", // 订单号
			"email": "khfll7e8c@gmail.com", // 邮箱
			"platformName": "apple", // 平台名称
			"price": 1, // 价格
			"expireTime": "2025-07-14T06:36:56.037Z", // 过期时间
			"status": "Waiting", // 状态  CodeReceived 已接码 Released 已释放  Expired 已过期  Waiting 待接码
			"createTime": "2025-07-14T06:16:56.037Z", // 创建时间
			"text": "", // 验证码
			"updateTime": "2025-07-14T06:16:56.037Z", // 更新时间
			"orderId": "6874a0d66019e853e292611a" // 订单号
		}
	]
}
```

## 释放邮箱

> 创建人: zzzzzga

```text
释放邮箱，每小时限制最多60个
```

**接口URL**

> /api/buyEmailOrder/open/release

**请求方式**

> POST

**Content-Type**

> json

**请求Header参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| Authorization | bd4d7f193ebc4ffc8558ebf18dbc2b84 | string | 是 | API秘钥 |

**请求Body参数**

```javascript
{
    "id":"6874a0d86019e853e292611e" // 查询验证码结果中的 _id
}
```

**响应示例**

* 成功(200)

```javascript
{
	"code": 1,
	"message": "success"
}
```