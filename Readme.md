# 全局公共参数

**全局Header参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| X-API-KEY | bbbb | string | 是 | APIKEY |
| X-SIGN | aaaa | string | 是 | 签名 |

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
| 1 | success |
| 0 | error |
| 400 | Bad Request |
| 401 | 认证失败 |
| 402 | 登录失败 |
| 404 | 接口不存在 |
| 410 | 文件名错误,不能包含 .. 等字符 |
| 500 | 系统繁忙 |
| 405 | 方法不被允许 |
| 101 | 数据已经存在 |
| 102 | 数据不存在 |
| 1001 | 参数无效 |
| 1002 | 参数为空 |
| 1003 | 未找到对应商品 |
| 1004 | 未达到最小数量 |
| 1005 | 用户余额不足 |
| 1006 | 钱包未设置 |
| 1007 | 无权限 |
| 2001 | 订单已存在 |
| 2002 | 没有可用的钱包 |
| 2003 | wallet not exists |
| 2004 | freeze amount invalid |
| 2005 | wallet balance insufficient |
| 2006 | restore amount invalid |
| 2007 | wallet frozen balance insufficient |
| 2008 | amount invalid |
| 2009 | user balance insufficient |
| 2010 | restore user balance failed |
| 2011 | deduct user balance failed |
| 2012 | order status error |

# gmail 下单

> 创建人: zzzzzga

> 更新人: zzzzzga

> 创建时间: 2025-07-11 17:44:45

> 更新时间: 2025-07-11 17:44:45

```text
暂无描述
```

**目录Header参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| 暂无参数 |

**目录Query参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| 暂无参数 |

**目录Body参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| 暂无参数 |

**目录认证信息**

> 继承父级

**Query**

## 下单

> 创建人: zzzzzga

> 更新人: zzzzzga

> 创建时间: 2025-07-11 17:47:40

> 更新时间: 2025-07-14 13:40:54

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

> /api/buyEmailOrder/open/buy?apipost_id=325fe149b3f006

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

* 失败(404)

```javascript
暂无数据
```

**请求Header参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| Authorization | bd4d7f193ebc4ffc8558ebf18dbc2b84 | string | 是 | API密钥 |

**Query**

## 平台

> 创建人: zzzzzga

> 更新人: zzzzzga

> 创建时间: 2025-07-11 17:49:13

> 更新时间: 2025-07-14 13:42:10

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

> /api/buyEmailOrder/open/accountPlatformList?apipost_id=32604d6373f0f9

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

* 失败(404)

```javascript
暂无数据
```

**请求Header参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| Authorization | bd4d7f193ebc4ffc8558ebf18dbc2b84 | string | 否 | API秘钥 |

**Query**

## 查询结果

> 创建人: zzzzzga

> 更新人: zzzzzga

> 创建时间: 2025-07-11 18:36:26

> 更新时间: 2025-07-14 13:43:45

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

> /api/buyEmailOrder/open/details/{orderNo}?apipost_id=326b1e92f3f19e

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

* 失败(404)

```javascript
暂无数据
```

**请求Header参数**

| 参数名 | 示例值 | 参数类型 | 是否必填 | 参数描述 |
| --- | --- | ---- | ---- | ---- |
| Authorization | bd4d7f193ebc4ffc8558ebf18dbc2b84 | string | 是 | API秘钥 |

**Query**
