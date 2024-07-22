# heychat-api
---
title: 黑盒语音接口
language_tabs:
  - shell: Shell
  - http: HTTP
  - javascript: JavaScript
  - ruby: Ruby
  - python: Python
  - php: PHP
  - java: Java
  - go: Go
toc_footers: []
includes: []
search: true
code_clipboard: true
highlight_theme: darkula
headingLevel: 2
generator: "@tarslib/widdershins v4.0.23"

---

# 黑盒语音接口

Base URLs:

# Authentication

* API Key (apikey-header-token)
    - Parameter Name: **token**, in: header. 

# 频道消息接口

## POST 发送频道消息

POST /chatroom/v2/channel_msg/send

> Body 请求参数

```json
{
  "msg": "@{id:4611545164569485312} @{id:100030} #{id:3628471439769796608} 11111",
  "msg_type": 10,
  "heychat_ack_id": "0",
  "reply_id": "",
  "room_id": "3581310465924767744",
  "addition": "{\"img_files_info\":[]}",
  "at_user_id": "100030",
  "at_role_id": "4611545164569485312",
  "mention_channel_id": "3628471439769796608",
  "channel_id": "3595756374695264256",
  "channel_type": 1
}
```

### 请求参数

|名称|位置|类型|必选|说明|
|---|---|---|---|---|
|client_type|query|string| 否 |声明请求黑盒语音|
|x_client_type|query|string| 否 |声明客户端类型|
|os_type|query|string| 否 |声明客户端类型|
|x_os_type|query|string| 否 |声明客户端是bot|
|x_app|query|string| 否 |声明请求黑盒语音|
|chat_os_type|query|string| 否 |声明客户端是bot|
|chat_version|query|string| 否 |客户端版本号,不同版本返回的结果可能有区别|
|Content-Type|header|string| 是 |none|
|body|body|object| 否 |none|
|» msg|body|string| 是 |none|
|» msg_type|body|integer| 是 |none|
|» heychat_ack_id|body|string| 是 |none|
|» reply_id|body|string| 是 |none|
|» room_id|body|string| 是 |none|
|» addition|body|string| 是 |none|
|» at_user_id|body|string| 是 |none|
|» at_role_id|body|string| 是 |none|
|» mention_channel_id|body|string| 是 |none|
|» channel_id|body|string| 是 |none|
|» channel_type|body|integer| 是 |none|

> 返回示例

> 200 Response

```json
{}
```

### 返回结果

|状态码|状态码含义|说明|数据模型|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### 返回数据结构

# 权限接口

## POST 对单个用户授予权限

POST /chatroom/v2/room_role/grant

> Body 请求参数

```json
{
  "to_user_id": 66837313,
  "role_id": "3581310465983111170",
  "room_id": "3581310465924767744"
}
```

### 请求参数

|名称|位置|类型|必选|说明|
|---|---|---|---|---|
|client_type|query|string| 否 |声明请求黑盒语音|
|x_client_type|query|string| 否 |声明客户端类型|
|os_type|query|string| 否 |声明客户端类型|
|x_os_type|query|string| 否 |声明客户端是bot|
|x_app|query|string| 否 |声明请求黑盒语音|
|chat_os_type|query|string| 否 |声明客户端是bot|
|chat_version|query|string| 否 |客户端版本号,不同版本返回的结果可能有区别|
|Content-Type|header|string| 是 |none|
|body|body|object| 否 |none|
|» msg|body|string| 是 |none|
|» msg_type|body|integer| 是 |none|
|» heychat_ack_id|body|string| 是 |none|
|» reply_id|body|string| 是 |none|
|» room_id|body|string| 是 |none|
|» addition|body|string| 是 |none|
|» at_user_id|body|string| 是 |none|
|» at_role_id|body|string| 是 |none|
|» mention_channel_id|body|string| 是 |none|
|» channel_id|body|string| 是 |none|
|» channel_type|body|integer| 是 |none|

> 返回示例

> 200 Response

```json
{}
```

### 返回结果

|状态码|状态码含义|说明|数据模型|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### 返回数据结构

## POST 对单个用户授予剥夺权限

POST /chatroom/v2/room_role/revoke

> Body 请求参数

```json
{
  "to_user_id": 66837313,
  "role_id": "3581310465983111170",
  "room_id": "3581310465924767744"
}
```

### 请求参数

|名称|位置|类型|必选|说明|
|---|---|---|---|---|
|client_type|query|string| 否 |声明请求黑盒语音|
|x_client_type|query|string| 否 |声明客户端类型|
|os_type|query|string| 否 |声明客户端类型|
|x_os_type|query|string| 否 |声明客户端是bot|
|x_app|query|string| 否 |声明请求黑盒语音|
|chat_os_type|query|string| 否 |声明客户端是bot|
|chat_version|query|string| 否 |客户端版本号,不同版本返回的结果可能有区别|
|Content-Type|header|string| 是 |none|
|body|body|object| 否 |none|
|» msg|body|string| 是 |none|
|» msg_type|body|integer| 是 |none|
|» heychat_ack_id|body|string| 是 |none|
|» reply_id|body|string| 是 |none|
|» room_id|body|string| 是 |none|
|» addition|body|string| 是 |none|
|» at_user_id|body|string| 是 |none|
|» at_role_id|body|string| 是 |none|
|» mention_channel_id|body|string| 是 |none|
|» channel_id|body|string| 是 |none|
|» channel_type|body|integer| 是 |none|

> 返回示例

> 200 Response

```json
{}
```

### 返回结果

|状态码|状态码含义|说明|数据模型|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|成功|Inline|

### 返回数据结构

# 数据模型

<h2 id="tocS_频道消息发送参数">频道消息发送参数</h2>

<a id="schema频道消息发送参数"></a>
<a id="schema_频道消息发送参数"></a>
<a id="tocS频道消息发送参数"></a>
<a id="tocs频道消息发送参数"></a>

```json
{
  "msg": "string",
  "msg_type": 0,
  "heychat_ack_id": "string",
  "reply_id": "string",
  "room_id": "string",
  "addition": "string",
  "at_user_id": "string",
  "at_role_id": "string",
  "mention_channel_id": "string",
  "channel_id": "string"
}

```

### 属性

|名称|类型|必选|约束|中文名|说明|
|---|---|---|---|---|---|
|msg|string|true|none||none|
|msg_type|integer|true|none||none|
|heychat_ack_id|string|true|none||none|
|reply_id|string|true|none||none|
|room_id|string|true|none||none|
|addition|string|true|none||none|
|at_user_id|string|true|none||none|
|at_role_id|string|true|none||none|
|mention_channel_id|string|true|none||none|
|channel_id|string|true|none||none|

<h2 id="tocS_Tag">Tag</h2>

<a id="schematag"></a>
<a id="schema_Tag"></a>
<a id="tocStag"></a>
<a id="tocstag"></a>

```json
{
  "id": 1,
  "name": "string"
}

```

### 属性

|名称|类型|必选|约束|中文名|说明|
|---|---|---|---|---|---|
|id|integer(int64)|false|none||标签ID编号|
|name|string|false|none||标签名称|

<h2 id="tocS_Category">Category</h2>

<a id="schemacategory"></a>
<a id="schema_Category"></a>
<a id="tocScategory"></a>
<a id="tocscategory"></a>

```json
{
  "id": 1,
  "name": "string"
}

```

### 属性

|名称|类型|必选|约束|中文名|说明|
|---|---|---|---|---|---|
|id|integer(int64)|false|none||分组ID编号|
|name|string|false|none||分组名称|

<h2 id="tocS_Pet">Pet</h2>

<a id="schemapet"></a>
<a id="schema_Pet"></a>
<a id="tocSpet"></a>
<a id="tocspet"></a>

```json
{
  "id": 1,
  "category": {
    "id": 1,
    "name": "string"
  },
  "name": "doggie",
  "photoUrls": [
    "string"
  ],
  "tags": [
    {
      "id": 1,
      "name": "string"
    }
  ],
  "status": "available"
}

```

### 属性

|名称|类型|必选|约束|中文名|说明|
|---|---|---|---|---|---|
|id|integer(int64)|true|none||宠物ID编号|
|category|[Category](#schemacategory)|true|none||分组|
|name|string|true|none||名称|
|photoUrls|[string]|true|none||照片URL|
|tags|[[Tag](#schematag)]|true|none||标签|
|status|string|true|none||宠物销售状态|

#### 枚举值

|属性|值|
|---|---|
|status|available|
|status|pending|
|status|sold|

