---
label: Introduction
icon: home
---
# Introduction

This document describes the API opened to external services from Idello. Namely this API was developed to allow sign-ups to Idéllo on third-party sites. 

## Overview

Idello API uses the following computed url `https://www.idello.org/fr/api/v1`. This is followed by a language variable or either `fr` or `en`. 


!!!
Idello supports a Cross Origin Access to its API. The only restriction of the service is for the external service provider to be known be known by Idello. 

Also, each external service provider shall provide its identifier for each of its requests and a checksum of the data sent to validate the authenticity of the request. 

Note that you should have an uniquely-identifying ID and a secret given by the TFO  to allow to request the API. 

!!!


| Request Header Name| Request Header Value |
| --- | --- |
|`Xdistantidentifier`| The uniquely-identifying ID given by TFO
|`Xdistantchecksum`| The JSON data HMAC using the secret with the SHA1 algorithm
|`ContentType`| `application/json`