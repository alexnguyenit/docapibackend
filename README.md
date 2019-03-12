--- 

title: API LOYALTY BACKEND 

language_tabs: 
   - shell 

toc_footers: 
   - <a href='#'>Sign Up for a Developer Key</a> 
   - <a href='https://github.com/alexnguyenit'>Documentation Powered by hoangnn</a> 

includes: 
   - errors 

search: true 

--- 

# Introduction 

This is API DOCUMENT LOYALTY BACKEND

**Version:** 1.0.2 

# Authentication 

|apiKey|*API Key*|
|---|---| 

# /USER/LOGIN
## ***POST*** 

**Summary:** {{url}}/api/user/login

**Description:** API login

### HTTP Request 
`***POST*** /user/login` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /USER/SIGHUP
## ***POST*** 

**Summary:** {{url}}/api/user/sighup

**Description:** API Sighup

### HTTP Request 
`***POST*** /user/sighup` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /USER/LOGOUT
## ***POST*** 

**Summary:** {{url}}/api/user/logout

**Description:** API logout

### HTTP Request 
`***POST*** /user/logout` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /USER/PROFILE
## ***GET*** 

**Summary:** {{url}}/api/user/profile

**Description:** API profile

### HTTP Request 
`***GET*** /user/profile` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /USER/COUNT
## ***GET*** 

**Summary:** {{url}}/api/user/count

**Description:** API profile

### HTTP Request 
`***GET*** /user/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /USER/MODIFY
## ***PUT*** 

**Summary:** {{url}}/api/user/modify

**Description:** API modify

### HTTP Request 
`***PUT*** /user/modify` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /USER/FORGOT
## ***POST*** 

**Summary:** {{url}}/api/user/forgot

**Description:** API Forgot Password

### HTTP Request 
`***POST*** /user/forgot` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /USER/RESET
## ***POST*** 

**Summary:** {{url}}/api/user/reset

**Description:** API reset Password

### HTTP Request 
`***POST*** /user/reset` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /USER/FIND
## ***GET*** 

**Summary:** {{url}}/api/user/find

**Description:** API list all User

### HTTP Request 
`***GET*** /user/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /DISTRICT/FIND
## ***GET*** 

**Summary:** {{url}}/api/district/find

**Description:** TODO: Add Description

### HTTP Request 
`***GET*** /district/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| province_id | query |  | Yes | integer |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WARD/FIND
## ***GET*** 

**Summary:** {{url}}/api/ward/find

**Description:** TODO: Add Description

### HTTP Request 
`***GET*** /ward/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| district_id | query |  | Yes | integer |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /PROVINCE/FIND
## ***GET*** 

**Summary:** {{url}}/api/province/find

**Description:** TODO: Add Description

### HTTP Request 
`***GET*** /province/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /ARTICLE/DESTROY/12
## ***DELETE*** 

**Summary:** {{url}}/api/article/destroy/11

**Description:** API destroy

### HTTP Request 
`***DELETE*** /article/destroy/12` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /ARTICLE/UPDATE/12
## ***PUT*** 

**Summary:** {{url}}/api/article/update/11

**Description:** API update article

### HTTP Request 
`***PUT*** /article/update/12` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /ARTICLE/CREATE
## ***POST*** 

**Summary:** {{url}}/api/article/create

**Description:** API add article

### HTTP Request 
`***POST*** /article/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /ARTICLE/FINDONE/1
## ***GET*** 

**Summary:** {{url}}/api/article/findOne/1

**Description:** API detail Article

### HTTP Request 
`***GET*** /article/findOne/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /ARTICLE/FIND
## ***GET*** 

**Summary:** {{url}}/api/article/find?_limit=2&_start=0&_attribute=id,title&title_contains=%cải tiến%

**Description:** API get list article

### HTTP Request 
`***GET*** /article/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| _limit | query |  | Yes | integer |
| _start | query |  | Yes | integer |
| _attribute | query |  | Yes | string |
| title_contains | query |  | Yes | string |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /ARTICLE/COUNT
## ***GET*** 

**Summary:** {{url}}/api/article/count

**Description:** API count

### HTTP Request 
`***GET*** /article/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CATEGORY/DESTROY/5
## ***DELETE*** 

**Summary:** {{url}}/api/category/destroy/1

**Description:** API destroy

### HTTP Request 
`***DELETE*** /category/destroy/5` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CATEGORY/UPDATE/5
## ***PUT*** 

**Summary:** {{url}}/api/category/update/1

**Description:** API update article

### HTTP Request 
`***PUT*** /category/update/5` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CATEGORY/CREATE
## ***POST*** 

**Summary:** {{url}}/api/category/create

**Description:** API add article

### HTTP Request 
`***POST*** /category/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CATEGORY/FIND
## ***GET*** 

**Summary:** {{url}}/api/category/find

**Description:** API get list article

### HTTP Request 
`***GET*** /category/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| _limit | query |  | Yes | integer |
| _start | query |  | Yes | integer |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CATEGORY/COUNT
## ***GET*** 

**Summary:** {{url}}/api/category/count

**Description:** API count

### HTTP Request 
`***GET*** /category/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CATEGORY/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/category/schema

**Description:** API count

### HTTP Request 
`***GET*** /category/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /BRAND/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/brand/schema

**Description:** API count

### HTTP Request 
`***GET*** /brand/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /BRAND/COUNT
## ***GET*** 

**Summary:** {{url}}/api/brand/count

**Description:** API count

### HTTP Request 
`***GET*** /brand/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /BRAND/FIND
## ***GET*** 

**Summary:** {{url}}/api/brand/find

**Description:** API get list article

### HTTP Request 
`***GET*** /brand/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /BRAND/FINDONE/2
## ***GET*** 

**Summary:** {{url}}/api/brand/findOne/1

**Description:** API detail Article

### HTTP Request 
`***GET*** /brand/findOne/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /BRAND/CREATE
## ***POST*** 

**Summary:** {{url}}/api/brand/create

**Description:** API add article

### HTTP Request 
`***POST*** /brand/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /BRAND/DESTROY/12
## ***DELETE*** 

**Summary:** {{url}}/api/brand/destroy/11

**Description:** API destroy

### HTTP Request 
`***DELETE*** /brand/destroy/12` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /BRAND/UPDATE/12
## ***PUT*** 

**Summary:** {{url}}/api/brand/update/11

**Description:** API update article

### HTTP Request 
`***PUT*** /brand/update/12` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /NEWS/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/news/schema

**Description:** API count

### HTTP Request 
`***GET*** /news/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /NEWS/COUNT
## ***GET*** 

**Summary:** {{url}}/api/news/count

**Description:** API count

### HTTP Request 
`***GET*** /news/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /NEWS/FIND
## ***GET*** 

**Summary:** {{url}}/api/news/find

**Description:** API get list article

### HTTP Request 
`***GET*** /news/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /NEWS/FINDONE/2
## ***GET*** 

**Summary:** {{url}}/api/news/findOne/1

**Description:** API detail Article

### HTTP Request 
`***GET*** /news/findOne/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /NEWS/CREATE
## ***POST*** 

**Summary:** {{url}}/api/news/create

**Description:** API add article

### HTTP Request 
`***POST*** /news/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /NEWS/DESTROY/1
## ***DELETE*** 

**Summary:** {{url}}/api/news/destroy/1

**Description:** API destroy

### HTTP Request 
`***DELETE*** /news/destroy/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /NEWS/UPDATE/1
## ***PUT*** 

**Summary:** {{url}}/api/news/update/1

**Description:** API update article

### HTTP Request 
`***PUT*** /news/update/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /ARTICLE/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/article/schema

**Description:** API count

### HTTP Request 
`***GET*** /article/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CONFIG/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/config/schema

**Description:** API count

### HTTP Request 
`***GET*** /config/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CONFIG/COUNT
## ***GET*** 

**Summary:** {{url}}/api/config/count

**Description:** API count

### HTTP Request 
`***GET*** /config/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CONFIG/FIND
## ***GET*** 

**Summary:** {{url}}/api/config/find

**Description:** API get list config

### HTTP Request 
`***GET*** /config/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CONFIG/FINDONE/1
## ***GET*** 

**Summary:** {{url}}/api/config/findOne/1

**Description:** API detail config

### HTTP Request 
`***GET*** /config/findOne/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CONFIG/CREATE
## ***POST*** 

**Summary:** {{url}}/api/config/create

**Description:** API add config

### HTTP Request 
`***POST*** /config/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CONFIG/DESTROY/1
## ***DELETE*** 

**Summary:** {{url}}/api/config/destroy/2

**Description:** API destroy

### HTTP Request 
`***DELETE*** /config/destroy/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CONFIG/UPDATE/1
## ***PUT*** 

**Summary:** {{url}}/api/config/update/2

**Description:** API update config

### HTTP Request 
`***PUT*** /config/update/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CONTACT/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/contact/schema

**Description:** API count

### HTTP Request 
`***GET*** /contact/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CONTACT/COUNT
## ***GET*** 

**Summary:** {{url}}/api/contact/count

**Description:** API count

### HTTP Request 
`***GET*** /contact/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CONTACT/FIND
## ***GET*** 

**Summary:** {{url}}/api/contact/find

**Description:** API get list contact

### HTTP Request 
`***GET*** /contact/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CONTACT/FINDONE/2
## ***GET*** 

**Summary:** {{url}}/api/contact/findOne/1

**Description:** API detail contact

### HTTP Request 
`***GET*** /contact/findOne/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CONTACT/CREATE
## ***POST*** 

**Summary:** {{url}}/api/contact/create

**Description:** API add contact

### HTTP Request 
`***POST*** /contact/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CONTACT/DESTROY/2
## ***DELETE*** 

**Summary:** {{url}}/api/contact/destroy/2

**Description:** API destroy

### HTTP Request 
`***DELETE*** /contact/destroy/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /CONTACT/UPDATE/2
## ***PUT*** 

**Summary:** {{url}}/api/contact/update/2

**Description:** API update contact

### HTTP Request 
`***PUT*** /contact/update/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /DISTRICT/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/district/schema

**Description:** API count

### HTTP Request 
`***GET*** /district/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /DISTRICT/COUNT
## ***GET*** 

**Summary:** {{url}}/api/district/count

**Description:** API count

### HTTP Request 
`***GET*** /district/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /DISTRICT/FINDONE/2
## ***GET*** 

**Summary:** {{url}}/api/district/findOne/1

**Description:** API detail district

### HTTP Request 
`***GET*** /district/findOne/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /DISTRICT/CREATE
## ***POST*** 

**Summary:** {{url}}/api/district/create

**Description:** API add district

### HTTP Request 
`***POST*** /district/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /DISTRICT/DESTROY/2
## ***DELETE*** 

**Summary:** {{url}}/api/district/destroy/2

**Description:** API destroy

### HTTP Request 
`***DELETE*** /district/destroy/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /DISTRICT/UPDATE/2
## ***PUT*** 

**Summary:** {{url}}/api/district/update/2

**Description:** API update district

### HTTP Request 
`***PUT*** /district/update/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /EXCHANGE/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/exchange/schema

**Description:** API count

### HTTP Request 
`***GET*** /exchange/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /EXCHANGE/COUNT
## ***GET*** 

**Summary:** {{url}}/api/exchange/count

**Description:** API count

### HTTP Request 
`***GET*** /exchange/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /EXCHANGE/FIND
## ***GET*** 

**Summary:** {{url}}/api/exchange/find

**Description:** API get list exchange

### HTTP Request 
`***GET*** /exchange/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /EXCHANGE/FINDONE/1
## ***GET*** 

**Summary:** {{url}}/api/exchange/findOne/1

**Description:** API detail exchange

### HTTP Request 
`***GET*** /exchange/findOne/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /EXCHANGE/CREATE
## ***POST*** 

**Summary:** {{url}}/api/exchange/create

**Description:** API add exchange

### HTTP Request 
`***POST*** /exchange/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /EXCHANGE/DESTROY/1
## ***DELETE*** 

**Summary:** {{url}}/api/exchange/destroy/1

**Description:** API destroy

### HTTP Request 
`***DELETE*** /exchange/destroy/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /EXCHANGE/UPDATE/1
## ***PUT*** 

**Summary:** {{url}}/api/exchange/update/1

**Description:** API update exchange

### HTTP Request 
`***PUT*** /exchange/update/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /FORMULA/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/formula/schema

**Description:** API count

### HTTP Request 
`***GET*** /formula/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /FORMULA/COUNT
## ***GET*** 

**Summary:** {{url}}/api/formula/count

**Description:** API count

### HTTP Request 
`***GET*** /formula/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /FORMULA/FIND
## ***GET*** 

**Summary:** {{url}}/api/formula/find

**Description:** API get list formula

### HTTP Request 
`***GET*** /formula/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /FORMULA/FINDONE/1
## ***GET*** 

**Summary:** {{url}}/api/formula/findOne/1

**Description:** API detail formula

### HTTP Request 
`***GET*** /formula/findOne/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /FORMULA/CREATE
## ***POST*** 

**Summary:** {{url}}/api/formula/create

**Description:** API add formula

### HTTP Request 
`***POST*** /formula/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /FORMULA/DESTROY/1
## ***DELETE*** 

**Summary:** {{url}}/api/formula/destroy/1

**Description:** API destroy

### HTTP Request 
`***DELETE*** /formula/destroy/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /FORMULA/UPDATE/1
## ***PUT*** 

**Summary:** {{url}}/api/formula/update/1

**Description:** API update formula

### HTTP Request 
`***PUT*** /formula/update/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /GROUP/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/group/schema

**Description:** API count

### HTTP Request 
`***GET*** /group/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /GROUP/COUNT
## ***GET*** 

**Summary:** {{url}}/api/group/count

**Description:** API count

### HTTP Request 
`***GET*** /group/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /GROUP/FIND
## ***GET*** 

**Summary:** {{url}}/api/group/find

**Description:** API get list group

### HTTP Request 
`***GET*** /group/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /GROUP/FINDONE/2
## ***GET*** 

**Summary:** {{url}}/api/group/findOne/1

**Description:** API detail group

### HTTP Request 
`***GET*** /group/findOne/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /GROUP/CREATE
## ***POST*** 

**Summary:** {{url}}/api/group/create

**Description:** API add group

### HTTP Request 
`***POST*** /group/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /GROUP/DESTROY/1
## ***DELETE*** 

**Summary:** {{url}}/api/group/destroy/1

**Description:** API destroy

### HTTP Request 
`***DELETE*** /group/destroy/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /GROUP/UPDATE/1
## ***PUT*** 

**Summary:** {{url}}/api/group/update/1

**Description:** API update group

### HTTP Request 
`***PUT*** /group/update/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /PRODUCT/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/product/schema

**Description:** API count

### HTTP Request 
`***GET*** /product/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /PRODUCT/COUNT
## ***GET*** 

**Summary:** {{url}}/api/product/count

**Description:** API count

### HTTP Request 
`***GET*** /product/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /PRODUCT/FIND
## ***GET*** 

**Summary:** {{url}}/api/product/find

**Description:** API get list product

### HTTP Request 
`***GET*** /product/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /PRODUCT/FINDONE/1
## ***GET*** 

**Summary:** {{url}}/api/product/findOne/1

**Description:** API detail product

### HTTP Request 
`***GET*** /product/findOne/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /PRODUCT/CREATE
## ***POST*** 

**Summary:** {{url}}/api/product/create

**Description:** API add product

### HTTP Request 
`***POST*** /product/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /PRODUCT/DESTROY/1
## ***DELETE*** 

**Summary:** {{url}}/api/product/destroy/1

**Description:** API destroy

### HTTP Request 
`***DELETE*** /product/destroy/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /PRODUCT/UPDATE/1
## ***PUT*** 

**Summary:** {{url}}/api/product/update/1

**Description:** API update product

### HTTP Request 
`***PUT*** /product/update/1` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /PROVINCE/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/province/schema

**Description:** API count

### HTTP Request 
`***GET*** /province/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /PROVINCE/COUNT
## ***GET*** 

**Summary:** {{url}}/api/province/count

**Description:** API count

### HTTP Request 
`***GET*** /province/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /PROVINCE/FINDONE/2
## ***GET*** 

**Summary:** {{url}}/api/province/findOne/1

**Description:** API detail province

### HTTP Request 
`***GET*** /province/findOne/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /PROVINCE/CREATE
## ***POST*** 

**Summary:** {{url}}/api/province/create

**Description:** API add province

### HTTP Request 
`***POST*** /province/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /PROVINCE/DESTROY/2
## ***DELETE*** 

**Summary:** {{url}}/api/province/destroy/2

**Description:** API destroy

### HTTP Request 
`***DELETE*** /province/destroy/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /PROVINCE/UPDATE/2
## ***PUT*** 

**Summary:** {{url}}/api/province/update/2

**Description:** API update province

### HTTP Request 
`***PUT*** /province/update/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /RANKING/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/ranking/schema

**Description:** API count

### HTTP Request 
`***GET*** /ranking/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /RANKING/COUNT
## ***GET*** 

**Summary:** {{url}}/api/ranking/count

**Description:** API count

### HTTP Request 
`***GET*** /ranking/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /RANKING/FIND
## ***GET*** 

**Summary:** {{url}}/api/ranking/find

**Description:** API get list ranking

### HTTP Request 
`***GET*** /ranking/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /RANKING/FINDONE/2
## ***GET*** 

**Summary:** {{url}}/api/ranking/findOne/1

**Description:** API detail ranking

### HTTP Request 
`***GET*** /ranking/findOne/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /RANKING/CREATE
## ***POST*** 

**Summary:** {{url}}/api/ranking/create

**Description:** API add ranking

### HTTP Request 
`***POST*** /ranking/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /RANKING/DESTROY/2
## ***DELETE*** 

**Summary:** {{url}}/api/ranking/destroy/2

**Description:** API destroy

### HTTP Request 
`***DELETE*** /ranking/destroy/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /RANKING/UPDATE/2
## ***PUT*** 

**Summary:** {{url}}/api/ranking/update/2

**Description:** API update ranking

### HTTP Request 
`***PUT*** /ranking/update/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /ROLE/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/role/schema

**Description:** API count

### HTTP Request 
`***GET*** /role/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /ROLE/COUNT
## ***GET*** 

**Summary:** {{url}}/api/role/count

**Description:** API count

### HTTP Request 
`***GET*** /role/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /ROLE/FIND
## ***GET*** 

**Summary:** {{url}}/api/role/find

**Description:** API get list role

### HTTP Request 
`***GET*** /role/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /ROLE/FINDONE/2
## ***GET*** 

**Summary:** {{url}}/api/role/findOne/1

**Description:** API detail role

### HTTP Request 
`***GET*** /role/findOne/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /ROLE/CREATE
## ***POST*** 

**Summary:** {{url}}/api/role/create

**Description:** API add role

### HTTP Request 
`***POST*** /role/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /ROLE/DESTROY/2
## ***DELETE*** 

**Summary:** {{url}}/api/role/destroy/2

**Description:** API destroy

### HTTP Request 
`***DELETE*** /role/destroy/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /ROLE/UPDATE/2
## ***PUT*** 

**Summary:** {{url}}/api/role/update/2

**Description:** API update role

### HTTP Request 
`***PUT*** /role/update/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WALLET/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/wallet/schema

**Description:** API count

### HTTP Request 
`***GET*** /wallet/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WALLET/COUNT
## ***GET*** 

**Summary:** {{url}}/api/wallet/count

**Description:** API count

### HTTP Request 
`***GET*** /wallet/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WALLET/FIND
## ***GET*** 

**Summary:** {{url}}/api/wallet/find

**Description:** API get list wallet

### HTTP Request 
`***GET*** /wallet/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WALLET/FINDONE/2
## ***GET*** 

**Summary:** {{url}}/api/wallet/findOne/1

**Description:** API detail wallet

### HTTP Request 
`***GET*** /wallet/findOne/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WALLET/CREATE
## ***POST*** 

**Summary:** {{url}}/api/wallet/create

**Description:** API add wallet

### HTTP Request 
`***POST*** /wallet/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WALLET/DESTROY/2
## ***DELETE*** 

**Summary:** {{url}}/api/wallet/destroy/2

**Description:** API destroy

### HTTP Request 
`***DELETE*** /wallet/destroy/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WALLET/UPDATE/2
## ***PUT*** 

**Summary:** {{url}}/api/wallet/update/2

**Description:** API update wallet

### HTTP Request 
`***PUT*** /wallet/update/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WARD/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/ward/schema

**Description:** API count

### HTTP Request 
`***GET*** /ward/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WARD/COUNT
## ***GET*** 

**Summary:** {{url}}/api/ward/count

**Description:** API count

### HTTP Request 
`***GET*** /ward/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WARD/FINDONE/2
## ***GET*** 

**Summary:** {{url}}/api/ward/findOne/1

**Description:** API detail ward

### HTTP Request 
`***GET*** /ward/findOne/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WARD/CREATE
## ***POST*** 

**Summary:** {{url}}/api/ward/create

**Description:** API add ward

### HTTP Request 
`***POST*** /ward/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WARD/DESTROY/2
## ***DELETE*** 

**Summary:** {{url}}/api/ward/destroy/2

**Description:** API destroy

### HTTP Request 
`***DELETE*** /ward/destroy/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WARD/UPDATE/2
## ***PUT*** 

**Summary:** {{url}}/api/ward/update/2

**Description:** API update ward

### HTTP Request 
`***PUT*** /ward/update/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WISHLIST/SCHEMA
## ***GET*** 

**Summary:** {{url}}/api/wishlist/schema

**Description:** API count

### HTTP Request 
`***GET*** /wishlist/schema` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WISHLIST/COUNT
## ***GET*** 

**Summary:** {{url}}/api/wishlist/count

**Description:** API count

### HTTP Request 
`***GET*** /wishlist/count` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WISHLIST/FIND
## ***GET*** 

**Summary:** {{url}}/api/wishlist/find

**Description:** API get list wishlist

### HTTP Request 
`***GET*** /wishlist/find` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WISHLIST/FINDONE/2
## ***GET*** 

**Summary:** {{url}}/api/wishlist/findOne/1

**Description:** API detail wishlist

### HTTP Request 
`***GET*** /wishlist/findOne/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WISHLIST/CREATE
## ***POST*** 

**Summary:** {{url}}/api/wishlist/create

**Description:** API add wishlist

### HTTP Request 
`***POST*** /wishlist/create` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WISHLIST/DESTROY/2
## ***DELETE*** 

**Summary:** {{url}}/api/wishlist/destroy/2

**Description:** API destroy

### HTTP Request 
`***DELETE*** /wishlist/destroy/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /WISHLIST/UPDATE/2
## ***PUT*** 

**Summary:** {{url}}/api/wishlist/update/2

**Description:** API update wishlist

### HTTP Request 
`***PUT*** /wishlist/update/2` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| Content-Type | header |  | Yes | string |
| x-scope | header |  | Yes | string |
| Body | body |  | Yes |  |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

# /MEDIA/UPLOAD
## ***POST*** 

**Summary:** {{url}}/api/media/upload

**Description:** API upload Image

### HTTP Request 
`***POST*** /media/upload` 

**Parameters**

| Name | Located in | Description | Required | Type |
| ---- | ---------- | ----------- | -------- | ---- |
| x-scope | header |  | Yes | string |
| Content-Type | header |  | Yes | string |
| File | formData |  | Yes | string |
| type | formData |  | Yes | string |

**Responses**

| Code | Description |
| ---- | ----------- |
| 200 |  |

<!-- Converted with the swagger-to-slate https://github.com/lavkumarv/swagger-to-slate -->
