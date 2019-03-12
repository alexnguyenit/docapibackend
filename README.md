# API LOYALTY BACKEND - CMC

This is API DOCUMENT LOYALTY BACKEND

**Version:** 1.0.2

**x-scope:** admin

## STATUS CODE
| Code | Description |
| ---- | ----------- |
| 200 | oke |
| 201 | oke |
| 204 | oke |
| 401 |  Unauthorized   |
| 400 |  Parameter Fail   |
| 404 |  Not found   |
| 500 |  Server error   |

## FILTER

=: Equals

_ne: Not equals

_lt: Lower than

_gt: Greater than

_lte: Lower than or equal to

_gte: Greater than or equal to

_in: Include in array

_contains: Contains

_containss: Contains case sensitive

_in: Matches any value in the array of values

_nin: Doesn't match any value in the array of values

*Examples*

Find users having John as first name.

GET /users?firstname=Tuan

Find products having a price equal or greater than 3.

GET /products?price_gte=3

Find multiple news with id 3, 6, 8 GET /news?id_in=3&id_in=6&id_in=8

## Sort

Sort according to a specific field.

*Example*

Sort user by email.

ASC: GET /user?_sort=email:ASC

DESC: GET /user?_sort=email:DESC

## Limit

Limit the size of the returned results.

*Example*

Limit the result length to 30.

GET /users?_limit=30

## Start

Skip a specific number of entries (especially useful for pagination).

*Example*

Get the second page of results.

GET /users?_start=10&_limit=10 

... 

# USER
## /USER/LOGIN

**Method:** POST

**Summary:** {{url}}/api/user/login

**Description:** API login

**HTTP Request**
`***POST*** /user/login` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| account | body |  | Yes |  |
| password | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /USER/SIGHUP

**Method:** POST

**Summary:** {{url}}/api/user/sighup

**Description:** API Sighup

**HTTP Request**
`***POST*** /user/sighup` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| firstname | body |  | Yes |  |
| password | body |  | Yes |  |
| phone | body |  | Yes |  |
| confirm | body |  | Yes |  |
| email | body |  | Yes |  |
| lastname | body |  | No |  |
| brand_id | body |  | No |  |
| rank_id | body |  | No |  |
| category_id | body |  | No |  |
| group_id | body |  | No |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /USER/LOGOUT

**Method:** POST

**Summary:** {{url}}/api/user/logout

**Description:** API logout

**HTTP Request**
`***POST*** /user/logout` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /USER/PROFILE

**Method:** GET

**Summary:** {{url}}/api/user/profile

**Description:** API profile

**HTTP Request**
`***GET*** /user/profile` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /USER/COUNT

**Method:** GET

**Summary:** {{url}}/api/user/count

**Description:** API profile

**HTTP Request**
`***GET*** /user/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /USER/MODIFY

**Method:** PUT

**Summary:** {{url}}/api/user/modify

**Description:** API modify

**HTTP Request**
`***PUT*** /user/modify` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |
| id | body |  | Yes |  |
| firstname | body |  | Yes | string |
| password | body |  | No | string |
| phone | body |  | Yes | string |
| confirm | body |  | No | string |
| new_password | body |  | No | string |
| email | body |  | Yes | string |
| lastname | body |  | No | string |
| gender | body | Giới tính người dùng với 0 là nữ và 1 là nam | No | number |
| birthday | body | Ngày sinh của người dùng: 16/4/1991 | No | string |
| avatar | body | Ảnh đại diện người dùng lấy từ API upload | No | object |
| info | body | Thông tin location, address... | No | object |
| type | body | Kiểu người dùng (1,2,3,4,5) | No | number |
| brand_id | body |  | No | number |
| rank_id | body |  | No | number |
| category_id | body |  | No | number |
| group_id | body |  | No | number |
| role_id | body |  | No | number |
| rules | body |  | No | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /USER/FORGOT

**Method:** POST

**Summary:** {{url}}/api/user/forgot

**Description:** API Forgot Password

**HTTP Request**
`***POST*** /user/forgot` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| email | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /USER/RESET

**Method:** POST 

**Summary:** {{url}}/api/user/reset

**Description:** API reset Password

**HTTP Request**
`***POST*** /user/reset` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| password | body |  | Yes |  |
| confirm | body |  | Yes |  |
| reset_password_token | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /USER/FIND

**Method:** GET

**Summary:** {{url}}/api/user/find

**Description:** API list all User

**HTTP Request**
`***GET*** /user/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /MEDIA/UPLOAD
**Method:** POST

**Summary:** {{url}}/api/media/upload

**Description:** API upload Image

**HTTP Request**
`***POST*** /media/upload` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Content-Type | header |  | Yes | string |
| Authorization | header |  | Yes | string |
| File | formData |  | Yes | string |
| type | formData |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

## /PRODUCT/SCHEMA

**Method:** GET

**Summary:** {{url}}/api/product/schema

**Description:** API count

**HTTP Request**
`***GET*** /product/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

## /PRODUCT/COUNT
**Method:** GET

**Summary:** {{url}}/api/product/count

**Description:** API count

**HTTP Request**
`***GET*** /product/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

## /PRODUCT/FIND
**Method:** GET

**Summary:** {{url}}/api/product/find

**Description:** API get list product

**HTTP Request**
`***GET*** /product/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

## /PRODUCT/FINDONE/1
**Method:** GET

**Summary:** {{url}}/api/product/findOne/1

**Description:** API detail product

**HTTP Request**
`***GET*** /product/findOne/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

## /PRODUCT/CREATE
**Method:** POST

**Summary:** {{url}}/api/product/create

**Description:** API add product

**HTTP Request**
`***POST*** /product/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |
| code | body |  | Yes | string |
| title | body |  | Yes | string |
| alias | body |  | No | string |
| description | body |  | No | text |
| parameters | body |  | No | object |
| type | body |  | No | number |
| category | body |  | No | string |
| brand_id | body |  | No | number |
| status | body |  | No | number |
| score | body |  | No | number |
| price | body |  | No | number |
| total | body |  | No | number |
| selled | body |  | No | number |
| start_date | body |  | No | date |
| end_date | body |  | No | date |
| image | body |  | No | object |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

## /PRODUCT/DESTROY/1
**Method:** DELETE

**Summary:** {{url}}/api/product/destroy/1

**Description:** API destroy

**HTTP Request**
`***DELETE*** /product/destroy/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

## /PRODUCT/UPDATE/1
**Method:** PUT

**Summary:** {{url}}/api/product/update/1

**Description:** API update product

**HTTP Request**
`***PUT*** /product/update/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |
