# API LOYALTY BACKEND - CMC

# Introduction 

This is API DOCUMENT LOYALTY BACKEND

**Version:** 1.0.2 

**FILTER**

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

**Sort**

Sort according to a specific field.

*Example*

Sort users by email.

ASC: GET /user?_sort=email:ASC
DESC: GET /user?_sort=email:DESC

**Limit**
Limit the size of the returned results.

*Example*

Limit the result length to 30.

GET /users?_limit=30

**Start**

Skip a specific number of entries (especially useful for pagination).

*Example*

Get the second page of results.

GET /users?_start=10&_limit=10

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
