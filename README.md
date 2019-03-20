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
| 400 |  Bad request   |
| 403 | Forbidden |
| 404 |  Not found   |
| 500 |  Server error   |
| 502 |  Database Error   |
| 503 | Unavailable |

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

Find multiple news with id 3, 6, 8 GET /article/find?id_in=3&id_in=6&id_in=8

or data

GET /article/find?id_or=3&id_or=6


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

## Like

*Example*

GET /users?email_like=%hoangnn% 

## Or

*Example*

GET /category/find?or_title=Category&or_status=0

## Search contains (include search array)

*Example*

GET /config/find?brands_contains=[13]

# Search Json

GET /product/find?image.imageThumb=link

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
| type | body | Kiểu người dùng enum(1,2,3,4,5) | No | enum |
| brand_id | body |  | No | number |
| rank_id | body |  | No | number |
| category_id | body |  | No | number |
| group_id | body |  | No | number |
| role_id | body |  | No | number |
| rules | body | Kiểu dữ liệu: 1,2,3,4 | No | string |

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

## /USER/CHANGEPASSWORD

**Method:** POST 

**Summary:** {{url}}/api/user/changePassword

**Description:** API change password

**HTTP Request**
`***POST*** /user/changePassword` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |
| password | body | Mật khẩu hiện tại | Yes | string |
| new_password | body | Mật khẩu mới | Yes | string |
| confirm | body | Mật khẩu giống mất khẩu mới | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |


## /USER/EXTEND

**Method:** POST 

**Summary:** {{url}}/api/user/extend

**Description:** API extend token

**HTTP Request**
`***POST*** /user/extend` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

# MEDIA
## /MEDIA/UPLOAD
**Method:** POST

**Summary:** {{url}}/api/media/upload

**Description:** API upload Image

Sử dụng data upload ảnh trả về để gửi lên, Không cần gửi source

```
{
    "urls": {
        "thumbLink": "/media/images/article/thumb_0605d5481e4701fd2d850ade29a1d8b1_13032019104101.png",
        "mediumLink": "/media/images/article/medium_0605d5481e4701fd2d850ade29a1d8b1_13032019104101.png",
        "originLink": "/media/images/article/origin_0605d5481e4701fd2d850ade29a1d8b1_13032019104101.png"
    },
    "type": ".png"
}
```

**HTTP Request**
`***POST*** /media/upload` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Content-Type | header |  | Yes | string |
| Authorization | header |  | Yes | string |
| File | formData |  | Yes | string |
| type | formData | Ex: news, profile, article, brand, other ... | No | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

# PRODUCT
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
| 200 | oke |

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
| 200 | oke |

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
| 200 | oke |

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
| 200 | oke |

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
| status | body | 0 - Đang xóa  1 - Đang active | No | number |
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
| 200 | oke |

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
| 200 | oke |

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
| 200 | oke |

# BRAND
## /BRAND/SCHEMA
**Method:** GET

**Summary:** {{url}}/api/brand/schema

**Description:** API count

**HTTP Request**
`***GET*** /brand/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /BRAND/COUNT
**Method:** GET

**Summary:** {{url}}/api/brand/count

**Description:** API count

**HTTP Request**
`***GET*** /brand/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /BRAND/FIND
**Method:** GET

**Summary:** {{url}}/api/brand/find

**Description:** API get list brand

**HTTP Request**
`***GET*** /brand/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /BRAND/FINDONE/2
**Method:** GET

**Summary:** {{url}}/api/brand/findOne/1

**Description:** API detail brand

**HTTP Request** 
`***GET*** /brand/findOne/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /BRAND/CREATE
**Method:** POST

**Summary:** {{url}}/api/brand/create

**Description:** API add brand

alias: Thường là dạng tieu-de

**HTTP Request**
`***POST*** /brand/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |
| name | body |  | Yes | string |
| alias | body |  | No | string |
| logo | body |  | No | object |
| description | body |  | No | string |
| parameters | body |  | No | object |
| address | body |  | No | string |
| email | body |  | No | string |
| phone | body |  | No | string |
| status | body | 0 - Đang xóa  1 - Đang active | No | number |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /BRAND/DESTROY/12
**Method:** DELETE

**Summary:** {{url}}/api/brand/destroy/11

**Description:** API destroy

**HTTP Request**
`***DELETE*** /brand/destroy/12` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /BRAND/UPDATE/12
**Method:** PUT

**Summary:** {{url}}/api/brand/update/11

**Description:** API update brand

**HTTP Request**
`***PUT*** /brand/update/12` 

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
| 200 | oke |

# CATEGORY
## /CATEGORY/SCHEMA
**Method:** GET

**Summary:** {{url}}/api/category/schema

**Description:** API count

**HTTP Request**
`***GET*** /category/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CATEGORY/COUNT
**Method:** GET

**Summary:** {{url}}/api/category/count

**Description:** API count

**HTTP Request**
`***GET*** /category/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CATEGORY/FIND
**Method:** GET

**Summary:** {{url}}/api/category/find

**Description:** API get list category

**HTTP Request**
`***GET*** /category/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CATEGORY/FINDONE/1
**Method:** GET

**Summary:** {{url}}/api/category/findOne/1

**Description:** API detail category

**HTTP Request**
`***GET*** /category/findOne/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CATEGORY/CREATE
**Method:** POST

**Summary:** {{url}}/api/category/create

**Description:** API add category

alias: Thường là dạng tieu-de

**HTTP Request**
`***POST*** /category/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |
| title | body |  | Yes | string |
| type | body | Kiểu danh mục với: 0 - Là category của các article, 1 - Là category của các product, 2 - Là category của các voucher, 3 - Là category của các partner, 4 - Là category của các customer | No | string |
| alias | body | Ex: tieu-de | No | string |
| description | body |  | No | object |
| status | body | 0 - Đang xóa  1 - Đang active | No | text |
| parameters | body |  | No | number |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CATEGORY/DESTROY/1
**Method:** DELETE

**Summary:** {{url}}/api/category/destroy/1

**Description:** API destroy

**HTTP Request**
`***DELETE*** /category/destroy/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CATEGORY/UPDATE/1
**Method:** PUT

**Summary:** {{url}}/api/category/update/1

**Description:** API update category

**HTTP Request**
`***PUT*** /category/update/1` 

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
| 200 | oke |

# ARTICLE
## /ARTICLE/SCHEMA
**Method:** GET

**Summary:** {{url}}/api/article/schema

**Description:** API count

**HTTP Request**
`***GET*** /article/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /ARTICLE/COUNT
**Method:** GET

**Summary:** {{url}}/api/article/count

**Description:** API count

**HTTP Request**
`***GET*** /article/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /ARTICLE/FIND
**Method:** GET

**Summary:** {{url}}/api/article/find

**Description:** API get list article

**HTTP Request**
`***GET*** /article/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /ARTICLE/FINDONE/2
**Method:** GET

**Summary:** {{url}}/api/article/findOne/1

**Description:** API detail article

**HTTP Request**
`***GET*** /article/findOne/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /ARTICLE/CREATE
**Method:** POST

**Summary:** {{url}}/api/article/create

**Description:** API add article

slug: Thường là dạng tieu-de

**HTTP Request**
`***POST*** /article/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |
| subject | body |  | Yes | string |
| slug | body | Ex: doi-tuong or tieu-de | No | string |
| review | body |  | No | string |
| image | body |  | No | object |
| content | body |  | No | text |
| category_id | body |  | No | number |
| parameters | body |  | No | object |
| comments | body |  | No | object |
| status | body | Trạng thái bài viết với: 0 - Đang xóa 1 - Đang active 2 - Đang chờ phê duyệt 3 - Đã được cấp phép đăng 4 - Đã bị thu hồi | No | number |
| published_at | body |  | No | date |
| evicted_at | body |  | No | date |
| approved_at | body |  | No | date |
| approver_id | body |  | No | number |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /ARTICLE/DESTROY/1
**Method:** DELETE

**Summary:** {{url}}/api/article/destroy/1

**Description:** API destroy

**HTTP Request**
`***DELETE*** /article/destroy/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /ARTICLE/UPDATE/1
**Method:** PUT

**Summary:** {{url}}/api/article/update/1

**Description:** API update article

**HTTP Request**
`***PUT*** /article/update/1` 

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
| 200 | oke |

# REWARD - ( VOUCHER - COUPON - EVENT )
## /REWARD/SCHEMA
**Method:** GET

**Summary:** {{url}}/api/reward/schema

**Description:** API count

**HTTP Request**
`***GET*** /reward/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /REWARD/COUNT
**Method:** GET

**Summary:** {{url}}/api/reward/count

**Description:** API count

**HTTP Request**
`***GET*** /reward/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /REWARD/FIND
**Method:** GET

**Summary:** {{url}}/api/reward/find?_limit=2&_start=0&_attribute=id,title&title_contains=%cải tiến%

**Description:** API get list reward

**HTTP Request**
`***GET*** /reward/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| _limit | query |  | No | integer |
| _start | query |  | No | integer |
| _attribute | query |  | No | string |
| title_contains | query |  | No | string |
| x-scope | header |  | yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /REWARD/FINDONE/1
**Method:** GET

**Summary:** {{url}}/api/reward/findOne/1

**Description:** API detail reward

**HTTP Request**
`***GET*** /reward/findOne/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /REWARD/CREATE
**Method:** POST

**Summary:** {{url}}/api/reward/create

**Description:** API add reward

alias: Thường là dạng tieu-de

**HTTP Request**
`***POST*** /reward/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |
| title | body | Kiểu bài viết với: 0 - Là info, 1 - Là event, 2 - Là voucher, 3 - Là coupon, 4 - Là other | Yes | string |
| alias | body | Ex: tieu-de | No | number |
| category_id | body |  | No | number |
| type | body |  | No | number |
| image | body |  | No | object |
| preview | body |  | No | string |
| content | body |  | No | text |
| score | body |  | No | number |
| amount | body | Giá trị của nội dung nếu là voucher, coupon | No | number |
| code | body |  | No | string |
| approved_at | body |  | No | date |
| approver_id | body |  | No | number |


**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /REWARD/DESTROY/12
**Method:** DELETE

**Summary:** {{url}}/api/reward/destroy/11

**Description:** API destroy

**HTTP Request**
`***DELETE*** /reward/destroy/12` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /REWARD/UPDATE/12
**Method:** PUT

**Summary:** {{url}}/api/reward/update/11

**Description:** API update reward

**HTTP Request**
`***PUT*** /reward/update/12` 

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
| 200 | oke |

# ENTITY
## /ENTITY/SCHEMA
**Method:** GET

**Summary:** {{url}}/api/entity/schema

**Description:** API count

**HTTP Request**
`***GET*** /entity/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /ENTITY/COUNT
**Method:** GET

**Summary:** {{url}}/api/entity/count

**Description:** API count

**HTTP Request**
`***GET*** /entity/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /ENTITY/FIND
**Method:** GET

**Summary:** {{url}}/api/entity/find

**Description:** API get list entity

**HTTP Request**
`***GET*** /entity/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /ENTITY/FINDONE/1
**Method:** GET

**Summary:** {{url}}/api/entity/findOne/1

**Description:** API detail entity

**HTTP Request**
`***GET*** /entity/findOne/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /ENTITY/CREATE
**Method:** POST

**Summary:** {{url}}/api/entity/create

**Description:** API add entity

slug: Thường là dạng tieu-de

**HTTP Request**
`***POST*** /entity/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |
| name | body |  | Yes | string |
| alias | body | Ex: tieu-de | No | string |
| description | body |  | No | text |
| parameters | body |  | No | object |
| code | body |  | No | string |
| brand_id | body |  | No | number |
| type | body |  | No | string |
| category | body |  | No | string |
| scope | body |  | No | string |
| level | body |  | No | number |
| parent_id | body |  | No | number |
| image | body |  | No | object |
| url | body |  | No | text |
| extension_id | body |  | No | number |
| object_id | body |  | No | number |
| group_id | body |  | No | number |
| status | body | Trạng thái bài viết với: 0 - Đang xóa 1 - Đang active | No | number |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /ENTITY/DESTROY/1
**Method:** DELETE

**Summary:** {{url}}/api/entity/destroy/1

**Description:** API destroy

**HTTP Request**
`***DELETE*** /entity/destroy/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /ENTITY/UPDATE/1
**Method:** PUT

**Summary:** {{url}}/api/entity/update/1

**Description:** API update entity

**HTTP Request**
`***PUT*** /entity/update/1` 

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
| 200 | oke |

# MENU - NAVIGATION
## /NAVIGATION/FIND
**Method:** GET

**Summary:** {{url}}/api/navigation/list

**Description:** API get list navigation

**HTTP Request**
`***GET*** /navigation/list` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

# CONFIG
## /CONFIG/SCHEMA
**Method:** GET

**Summary:** {{url}}/api/config/schema

**Description:** API count

**HTTP Request**
`***GET*** /config/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CONFIG/COUNT
**Method:** GET

**Summary:** {{url}}/api/config/count

**Description:** API count

**HTTP Request**
`***GET*** /config/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CONFIG/FIND
**Method:** GET

**Summary:** {{url}}/api/config/find

**Description:** API get list config

**HTTP Request**
`***GET*** /config/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CONFIG/FINDONE/1
**Method:** GET

**Summary:** {{url}}/api/config/findOne/1

**Description:** API detail config

**HTTP Request**
`***GET*** /config/findOne/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CONFIG/CREATE
**Method:** POST

**Summary:** {{url}}/api/config/create

**Description:** API add config

slug: Thường là dạng tieu-de

**HTTP Request**
`***POST*** /config/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |
| key | body |  | Yes | string |
| value | body |  | Yes | text |
| name | body |  | Yes | string |
| description | body |  | No | text |
| type | body |  | No | number |
| category_id | body | Reference category | No | number |
| group | body |  | No | string |
| brands | body | [1,2,3,4] | No | object array |
| parameters | body |  | No | object |
| status | body | Trạng thái bài viết với: 0 - Đang xóa 1 - Đang active | No | number |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CONFIG/DESTROY/1
**Method:** DELETE

**Summary:** {{url}}/api/config/destroy/1

**Description:** API destroy

**HTTP Request**
`***DELETE*** /config/destroy/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CONFIG/UPDATE/1
**Method:** PUT

**Summary:** {{url}}/api/config/update/1

**Description:** API update config

**HTTP Request**
`***PUT*** /config/update/1` 

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
| 200 | oke |

# CAMPAIGN
## /CAMPAIGN/SCHEMA
**Method:** GET

**Summary:** {{url}}/api/campaign/schema

**Description:** API count

**HTTP Request**
`***GET*** /campaign/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CAMPAIGN/COUNT
**Method:** GET

**Summary:** {{url}}/api/campaign/count

**Description:** API count

**HTTP Request**
`***GET*** /campaign/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CAMPAIGN/FIND
**Method:** GET

**Summary:** {{url}}/api/campaign/find

**Description:** API get list campaign

**HTTP Request**
`***GET*** /campaign/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CAMPAIGN/FINDONE/1
**Method:** GET

**Summary:** {{url}}/api/campaign/findOne/1

**Description:** API detail campaign

**HTTP Request**
`***GET*** /campaign/findOne/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CAMPAIGN/CREATE
**Method:** POST

**Summary:** {{url}}/api/campaign/create

**Description:** API add campaign

slug: Thường là dạng tieu-de

**HTTP Request**
`***POST*** /campaign/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |
| name | body |  | Yes | string |
| alias | body | Ex: tieu-de | No | string |
| code | body |  | No | string |
| brand_id | body | Reference Brand | No | number |
| description | body |  | No | text |
| note | body |  | No | text |
| programs | body |  | No | object |
| localtions | body |  | No | object |
| rewards | body |  | No | object |
| articles | body |  | No | object |
| connections | body |  | No | object |
| conditions | body |  | No | object |
| parameters | body |  | No | object |
| image | body |  | No | object |
| target | body |  | No | string |
| expect | body |  | No | string |
| result | body |  | No | string |
| statistic | body |  | No | string |
| schedule | body |  | No | string |
| cost | body |  | No | number |
| paid | body |  | No | number |
| point | body |  | No | number |
| percentage | body |  | No | number |
| piority | body |  | No | number |
| level | body |  | No | number |
| parameters | body |  | No | object |
| comments | body |  | No | object |
| start_date | body | Ex: 16/4/2019 | No | string |
| end_date | body | Ex: 16/4/2019 | No | string |
| status | body | Trạng thái bài viết với: 0 - Đang xóa 1 - Đang active | No | number |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CAMPAIGN/DESTROY/1
**Method:** DELETE

**Summary:** {{url}}/api/campaign/destroy/1

**Description:** API destroy

**HTTP Request**
`***DELETE*** /campaign/destroy/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /CAMPAIGN/UPDATE/1
**Method:** PUT

**Summary:** {{url}}/api/campaign/update/1

**Description:** API update campaign

**HTTP Request**
`***PUT*** /campaign/update/1` 

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
| 200 | oke |

# EXTENSION
## /EXTENSION/SCHEMA
**Method:** GET

**Summary:** {{url}}/api/extension/schema

**Description:** API count

**HTTP Request**
`***GET*** /extension/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /EXTENSION/COUNT
**Method:** GET

**Summary:** {{url}}/api/extension/count

**Description:** API count

**HTTP Request**
`***GET*** /extension/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /EXTENSION/FIND
**Method:** GET

**Summary:** {{url}}/api/extension/find

**Description:** API get list extension

**HTTP Request**
`***GET*** /extension/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /EXTENSION/FINDONE/1
**Method:** GET

**Summary:** {{url}}/api/extension/findOne/1

**Description:** API detail extension

**HTTP Request**
`***GET*** /extension/findOne/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /EXTENSION/CREATE
**Method:** POST

**Summary:** {{url}}/api/extension/create

**Description:** API add extension

slug: Thường là dạng tieu-de

**HTTP Request**
`***POST*** /extension/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |
| name | body |  | Yes | string |
| alias | body | Ex: tieu-de | No | string |
| code | body |  | No | string |
| brand | body |  | No | string |
| description | body |  | No | text |
| note | body |  | No | text |
| scope | body |  | No | string |
| type | body |  | No | string |
| parameters | body |  | No | object |
| structure | body |  | No | object |
| config | body |  | No | object |
| installed_at | body |  | No | datetime |
| installed_by | body |  | No | number |
| removed_at | body |  | No | datetime |
| removed_by | body |  | No | number |
| actived_at | body |  | No | datetime |
| actived_by | body |  | No | number |
| stoped_at | body |  | No | datetime |
| stoped_by | body |  | No | number |
| called_time | body |  | No | number |
| worked_time | body |  | No | number |
| version | body |  | No | string |
| start_date | body | Ex: 2019-03-08 | No | string |
| end_date | body | Ex: 2020-03-08 | No | string |
| status | body | Trạng thái bài viết với: 0 - Đang xóa 1 - Đang active | No | number |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /EXTENSION/DESTROY/1
**Method:** DELETE

**Summary:** {{url}}/api/extension/destroy/1

**Description:** API destroy

**HTTP Request**
`***DELETE*** /extension/destroy/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Authorization | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 | oke |

## /EXTENSION/UPDATE/1
**Method:** PUT

**Summary:** {{url}}/api/extension/update/1

**Description:** API update extension

**HTTP Request**
`***PUT*** /extension/update/1` 

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
| 200 | oke |
