---
icon: note
tags:
  - requests
---

# Profile

## Method

`POST`

## Endpoint

`/profile/me`

## Description

Get the current logged in account's information

## Parameters

Name                         | Description
---------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------
`X-tfo-idello-session `      | [!badge text="string" variant="light"] [!badge text="required" variant="warning"] (header) Session ID




## Responses

Example

```
# Code 200
{
  "success": 1,
  "msg": "OK",
  "code": "OK",
  "data": {
    "id": 1,
    "firstname": "John",
    "lastname": "Smith",
    "roles": [
      "admin",
      "user"
    ],
    "personas": [
      "parent",
      "student",
      "child"
    ],
    "slug": "string",
    "preferences": [
      {
        "id": 1,
        "slug": "string",
        "type": "filter",
        "status": "P",
        "name": "video",
        "title": "Vidéo"
      }
    ],
    "avatar": "string"
  }
}
```
