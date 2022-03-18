---
icon: note
tags: [requests]
title: Resend Activation
---
# Resend Activation
Resend signup activation email

## Method
`POST`

## Endpoint
`/account/resend-activation`

## Parameters
| Name| Description |
| --- | --- |
|`email`| [!badge text="string" variant="light"] [!badge text="required" variant="warning"] 

Example
```
{
  "email": "string",
}
```

## Responses

Example
```
# Code 200
{
  "success": 1,
  "msg": "OK",
  "code": "OK"
}
```

