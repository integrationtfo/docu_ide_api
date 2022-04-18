---
icon: note
tags:
  - requests
---

# Provider authentication

## Method

`POST`

## Endpoint

`/provider/authenticate`

## Description

This endpoint MUST be called when the partner requests an authentication for a specific user. Upon making sure the checksum is valid, and the request is validated by the partner through the pingback URL, the partner returns the user's identity information. For more details, see <https://docs.google.com/document/d/18wJkT5Pgdkl5RTYaXOlbP0QrxOE-wKNzYFW485LRqtI>

## Parameters

Name                         | Description
---------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------
`X-IDELLO-PROVIDER-KEY`      | [!badge text="string" variant="light"] [!badge text="required" variant="warning"] Unique key given to each provider. See IDLOAccountProviderToken
`X-IDELLO-PROVIDER-CHECKSUM` | [!badge text="string" variant="light"] [!badge text="required" variant="warning"] set using hash_hmac('sha1', $appKey . json_encode($request), $sharedSecret)

Example

```
{
  "uid": "string",
  "nonce": "string",
  "requested-url": "string"
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
    "token": "string"
  }
}
```
