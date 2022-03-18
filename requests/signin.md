---
icon: note
tags: [requests]
---
# Sign in

## Method
`POST`

## Endpoint
`/account/signin`

## Parameters
| Name| Description |
| --- | --- |
|`username`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"]
|`password`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] md5 hash of the user password

Example
```
{
  "username": "joe",
  "password": "5f4dcc3b5aa765d61d8327deb882cf99",
}
```

## Responses

Example
```
# Code 200
{
  "success": 1,
  "msg": "OK",
  "code": "OK",
  "data": {
    "session_name": "X-tfo-idello-session",
    "session_id": "xyz1234"
  }
}
```

| Name| Description |
| --- | --- |
|`session_name`| Session name, used for setting POST headers
|`session_id`| Session ID for subsequent calls