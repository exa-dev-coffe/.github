---
title: Default module
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
generator: "@tarslib/widdershins v4.0.30"

---

# Default module

Base URLs:

* <a href="">KONG PROD: </a>

# Authentication

- HTTP Authentication, scheme: bearer

# ACCOUNT/UPLOAD

## POST Upload Profile

POST /upload/upload-profile

> Body Parameters

```yaml
file: file://C:\Users\Exa\Downloads\logo.png

```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|
|» file|body|string(binary)| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## DELETE Delete

DELETE /upload/delete-profile

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|url|query|string| no |none|

> Response Examples

> 404 Response

```json
{
  "success": true,
  "message": "string",
  "timestamp": "string",
  "data": null
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|none|Inline|

### Responses Data Schema

HTTP Status Code **404**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» success|boolean|true|none||none|
|» message|string|true|none||none|
|» timestamp|string|true|none||none|
|» data|null|true|none||none|

# ACCOUNT/AUTH

## POST Register

POST /auth/register

> Body Parameters

```json
{
  "fullName": "test",
  "password": "ekasyafrinonazhifan",
  "email": "bloodsuker18@gmail.com"
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## POST Login

POST /auth/login

> Body Parameters

```json
{
  "email": "admin@gmail.com",
  "password": "password123"
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## POST Refresh

POST /auth/refresh

> Body Parameters

```json
{
  "refreshToken": ""
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## POST Logout

POST /auth/logout

> Body Parameters

```json
{
  "refreshToken": ""
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## GET Me

GET /me

> Response Examples

> 500 Response

```json
{
  "success": true,
  "message": "string",
  "timestamp": "string",
  "data": null
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **500**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» success|boolean|true|none||none|
|» message|string|true|none||none|
|» timestamp|string|true|none||none|
|» data|null|true|none||none|

## POST Forgot password

POST /auth/forgot-password

> Body Parameters

```json
{
  "email": "admin@gmail.com"
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## POST Change-password

POST /auth/change-password

> Body Parameters

```json
{
  "token": "eyJhbGciOiJIUzUxMiJ9.eyJyb2xlIjoidXNlciIsImZ1bGxOYW1lIjoidGVzdCIsInR5cGUiOiJSRVNFVF9QQVNTV09SRCIsInVzZXJJZCI6NDYsImVtYWlsIjoiYmxvb2RzdWtlcjE4QGdtYWlsLmNvbSIsInN1YiI6ImJsb29kc3VrZXIxOEBnbWFpbC5jb20iLCJpYXQiOjE3NTgzMzI5NTAsImV4cCI6MTc1ODMzMzI1MH0.ojCivxFHAsc0t2NJUjGxe7WGe_8LnMm57Nlc31MoM0oz5f5Xg-IbACR5lvZ0NEajN1gzFVoamLDO_wimUrp6lg",
  "password": "ekasyafrinonazhifan31"
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 404 Response

```json
{
  "success": true,
  "message": "string",
  "timestamp": "string",
  "data": null
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|none|Inline|

### Responses Data Schema

HTTP Status Code **404**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» success|boolean|true|none||none|
|» message|string|true|none||none|
|» timestamp|string|true|none||none|
|» data|null|true|none||none|

## GET Login Google

GET /auth/google

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

# ACCOUNT/BARISTA

## POST Register Barista

POST /barista/register-barista

> Body Parameters

```json
{
  "fullName": "test",
  "password": "ekasyafrinonazhifan",
  "email": "bloodsuker18@gmail.com"
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## GET Get Barista

GET /barista/list-barista

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|page|query|integer| no |none|
|size|query|integer| no |none|
|sort|query|string| no |Field|
|searchKey|query|string| no |none|
|searchValue|query|string| no |none|

> Response Examples

> 200 Response

```json
{
  "success": true,
  "message": "string",
  "timestamp": "string",
  "data": [
    {
      "userId": 0,
      "email": "string",
      "fullName": "string",
      "photo": "string"
    }
  ]
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **200**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» success|boolean|true|none||none|
|» message|string|true|none||none|
|» timestamp|string|true|none||none|
|» data|[object]|true|none||none|
|»» userId|integer|true|none||none|
|»» email|string|true|none||none|
|»» fullName|string|true|none||none|
|»» photo|string¦null|true|none||none|

## DELETE Delete Barista

DELETE /barista

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|userId|query|string| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

# ACCOUNT/PROFILE

## PATCH Update Profile

PATCH /update-profile

> Body Parameters

```json
{
  "fullName": "test uodate 1",
  "photo": "https://storage.eka-dev.cloud/project/coffe/images/profiles/1759926231032bb8e9df4-0ab0-4229-b343-11451350bf79.png",
  "refreshToken": ""
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 200 Response

```json
{
  "success": true,
  "message": "string",
  "timestamp": "string",
  "data": {
    "accessToken": "string",
    "refreshToken": "string"
  }
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **200**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» success|boolean|true|none||none|
|» message|string|true|none||none|
|» timestamp|string|true|none||none|
|» data|object|true|none||none|
|»» accessToken|string|true|none||none|
|»» refreshToken|string|true|none||none|

# MASTER DATA/CATEGORY

## GET Get List Categories

GET /categories

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|page|query|string| no |none|
|size|query|string| no |none|
|sort|query|string| no |none|
|searchKey|query|string| no |none|
|searchValue|query|string| no |none|
|noPaginate|query|boolean| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## POST Insert Category

POST /categories

> Body Parameters

```json
{
  "name": "test"
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 201 Response

```json
{
  "message": "string",
  "data": null,
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|none|Inline|

### Responses Data Schema

HTTP Status Code **201**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» message|string|true|none||none|
|» data|null|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

## DELETE Delete category

DELETE /categories

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|query|integer| no |none|

> Response Examples

> 400 Response

```json
{
  "message": "string",
  "data": null,
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|400|[Bad Request](https://tools.ietf.org/html/rfc7231#section-6.5.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **400**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» message|string|true|none||none|
|» data|null|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

# MASTER DATA/MENU

## GET Get Menu

GET /menus

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|page|query|integer| no |none|
|size|query|integer| no |none|
|sort|query|string| no |Field|
|searchKey|query|string| no |none|
|searchValue|query|string| no |none|
|noPaginate|query|boolean| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## POST Create Menu

POST /menus

> Body Parameters

```json
{
  "name": "test",
  "description": "test",
  "price": 1000,
  "categoryId": null,
  "photo": "https://storage.eka-dev.cloud/project/coffe/images/menus/20250926210047-0f7546f3-0fd0-4ddb-a50d-e8a73e0c3230.png"
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## PUT Update Menu

PUT /menus

> Body Parameters

```json
{
  "name": "test Update",
  "description": "test",
  "price": 1000,
  "categoryId": null,
  "id": 7,
  "isAvailable": true,
  "photo": "https://storage.eka-dev.cloud/project/coffe/images/menus/20250926210047-0f7546f3-0fd0-4ddb-a50d-e8a73e0c3230.png"
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 200 Response

```json
{
  "message": "string",
  "data": null,
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **200**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» message|string|true|none||none|
|» data|null|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

## DELETE Delete Menu

DELETE /menus

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|query|string| no |none|

> Response Examples

> 404 Response

```json
{
  "message": "string",
  "data": null,
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|none|Inline|

### Responses Data Schema

HTTP Status Code **404**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» message|string|true|none||none|
|» data|null|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

## GET Get Uncategorized

GET /menus/uncategorized

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|page|query|integer| no |none|
|size|query|integer| no |none|
|sort|query|string| no |Field|
|searchKey|query|string| no |none|
|searchValue|query|string| no |none|
|noPaginate|query|boolean| no |none|

> Response Examples

> 200 Response

```json
{
  "message": "string",
  "data": [
    {
      "id": 0,
      "name": "string",
      "description": "string",
      "photo": "string",
      "isAvailable": true,
      "price": 0,
      "categoryId": 0,
      "categoryName": "string"
    }
  ],
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **200**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» message|string|true|none||none|
|» data|[object]|true|none||none|
|»» id|integer|true|none||none|
|»» name|string|true|none||none|
|»» description|string|true|none||none|
|»» photo|string|true|none||none|
|»» isAvailable|boolean|true|none||none|
|»» price|integer|true|none||none|
|»» categoryId|integer|true|none||none|
|»» categoryName|string|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

## GET Get By Category

GET /menus/by-category

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|query|string| no |none|

> Response Examples

> 200 Response

```json
{
  "message": "string",
  "data": [
    null
  ],
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **200**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» message|string|true|none||none|
|» data|[any]|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

## PATCH Set Category

PATCH /menus/set-category

> Body Parameters

```json
{
  "id": 7,
  "categoryId": 10
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 400 Response

```json
{
  "message": "string",
  "data": null,
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|400|[Bad Request](https://tools.ietf.org/html/rfc7231#section-6.5.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **400**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» message|string|true|none||none|
|» data|null|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

## GET Get One Menu

GET /menus/detail

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|query|number| no |none|

> Response Examples

> 200 Response

```json
{
  "message": "string",
  "data": {
    "id": 0,
    "name": "string",
    "description": "string",
    "photo": "string",
    "isAvailable": true,
    "price": 0,
    "categoryId": 0,
    "categoryName": "string"
  },
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **200**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» message|string|true|none||none|
|» data|object|true|none||none|
|»» id|integer|true|none||none|
|»» name|string|true|none||none|
|»» description|string|true|none||none|
|»» photo|string|true|none||none|
|»» isAvailable|boolean|true|none||none|
|»» price|integer|true|none||none|
|»» categoryId|integer|true|none||none|
|»» categoryName|string|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

# MASTER DATA/UPLOAD

## POST Upload Menu

POST /upload/upload-menu

> Body Parameters

```yaml
file: file://C:\Users\Exa\Downloads\logo.png

```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|
|» file|body|string(binary)| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## DELETE Delete

DELETE /upload/delete-menu

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|url|query|string| no |none|

> Response Examples

> 200 Response

```json
{
  "message": "string",
  "data": null,
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **200**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» message|string|true|none||none|
|» data|null|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

# MASTER DATA/TABLE

## GET Get Tables

GET /tables

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|page|query|integer| no |none|
|size|query|integer| no |none|
|sort|query|string| no |Field|
|searchKey|query|string| no |none|
|searchValue|query|string| no |none|
|noPaginate|query|boolean| no |none|

> Response Examples

> 200 Response

```json
{
  "message": "string",
  "data": {
    "data": null,
    "totalData": 0,
    "totalPages": 0,
    "currentPage": 0,
    "pageSize": 0,
    "lastPage": true
  },
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **200**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» message|string|true|none||none|
|» data|object|true|none||none|
|»» data|null|true|none||none|
|»» totalData|integer|true|none||none|
|»» totalPages|integer|true|none||none|
|»» currentPage|integer|true|none||none|
|»» pageSize|integer|true|none||none|
|»» lastPage|boolean|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

## POST Create Table

POST /tables

> Body Parameters

```json
{
  "name": "test 2"
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 201 Response

```json
{
  "message": "string",
  "data": null,
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|none|Inline|

### Responses Data Schema

HTTP Status Code **201**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» message|string|true|none||none|
|» data|null|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

## PUT Update Table

PUT /tables

> Body Parameters

```json
{
  "name": "test 2 upatede",
  "id": 1
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 500 Response

```json
{
  "data": null,
  "message": "string",
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **500**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» data|null|true|none||none|
|» message|string|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

## DELETE Delete Table

DELETE /tables

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|query|integer| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

# WALLET/BALANCE

## GET Get Balance

GET /balance

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## POST Activate Balance

POST /balance/activate

> Body Parameters

```json
{
  "pin": "123456"
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

# WALLET/BALANCE HISTORY

## GET Get Balance History

GET /balance-history

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|page|query|integer| no |none|
|size|query|integer| no |none|
|sort|query|string| no |Field|
|searchKey|query|string| no |none|
|searchValue|query|string| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## POST Top Up

POST /balance/top-up

> Body Parameters

```json
{
  "pin": "12356",
  "amount": 100000
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 500 Response

```json
{
  "success": true,
  "message": "string",
  "timestamp": "string",
  "data": null
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|500|[Internal Server Error](https://tools.ietf.org/html/rfc7231#section-6.6.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **500**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» success|boolean|true|none||none|
|» message|string|true|none||none|
|» timestamp|string|true|none||none|
|» data|null|true|none||none|

# TRANSACTION/TRANSACTION

## POST Create Transaction

POST /checkout

> Body Parameters

```json
{
  "tableId": 1,
  "orderFor": "eka",
  "pin": "123456",
  "datas": [
    {
      "menuId": 5,
      "qty": 1,
      "notes": "test"
    },
    {
      "menuId": 6,
      "qty": 4,
      "notes": "test"
    }
  ]
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## PATCH Set Rating Menu

PATCH /history-checkouts/set-rating-menu

> Body Parameters

```json
{
  "id": 20,
  "rating": 4
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 400 Response

```json
{
  "message": "string",
  "data": null,
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|400|[Bad Request](https://tools.ietf.org/html/rfc7231#section-6.5.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **400**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» message|string|true|none||none|
|» data|null|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

# TRANSACTION/TRANSACTION/User

## GET Get Transactions Copy

GET /history-checkouts

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|page|query|integer| no |none|
|size|query|integer| no |none|
|sort|query|string| no |Field|
|searchKey|query|string| no |none|
|searchValue|query|string| no |none|
|noPaginate|query|boolean| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## GET Get Transaction Detail Copy

GET /history-checkouts/detail

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|query|integer| no |none|

> Response Examples

> 404 Response

```json
{
  "message": "string",
  "data": null,
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|none|Inline|

### Responses Data Schema

HTTP Status Code **404**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» message|string|true|none||none|
|» data|null|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

# TRANSACTION/TRANSACTION/Admin/Barista

## GET Get Transactions

GET /transactions

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|page|query|integer| no |none|
|size|query|integer| no |none|
|sort|query|string| no |Field|
|searchKey|query|string| no |none|
|searchValue|query|string| no |none|
|noPaginate|query|boolean| no |none|
|startDate|query|string| no |none|
|endDate|query|string| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

## GET Get Transaction Detail

GET /transactions/detail

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|id|query|integer| no |none|

> Response Examples

> 404 Response

```json
{
  "message": "string",
  "data": null,
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|none|Inline|

### Responses Data Schema

HTTP Status Code **404**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» message|string|true|none||none|
|» data|null|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

## PATCH Update Status Order

PATCH /transactions/update-order-status

> Body Parameters

```json
{
  "id": 14
}
```

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|body|body|object| no |none|

> Response Examples

> 400 Response

```json
{
  "message": "string",
  "data": null,
  "success": true,
  "timestamp": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|400|[Bad Request](https://tools.ietf.org/html/rfc7231#section-6.5.1)|none|Inline|

### Responses Data Schema

HTTP Status Code **400**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» message|string|true|none||none|
|» data|null|true|none||none|
|» success|boolean|true|none||none|
|» timestamp|string|true|none||none|

## GET Summary Transaction

GET /transactions/summary-report

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|startDate|query|string| no |none|
|endDate|query|string| no |none|

> Response Examples

> 200 Response

```json
{}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|none|Inline|

### Responses Data Schema

# Data Schema

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

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|id|integer(int64)|true|none||Pet ID|
|category|[Category](#schemacategory)|true|none||group|
|name|string|true|none||name|
|photoUrls|[string]|true|none||image URL|
|tags|[[Tag](#schematag)]|true|none||tag|
|status|string|true|none||Pet Sales Status|

#### Enum

|Name|Value|
|---|---|
|status|available|
|status|pending|
|status|sold|

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

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|id|integer(int64)|false|none||Category ID|
|name|string|false|none||Category Name|

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

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|id|integer(int64)|false|none||Tag ID|
|name|string|false|none||Tag Name|

