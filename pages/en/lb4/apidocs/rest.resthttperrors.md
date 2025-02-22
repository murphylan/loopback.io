---
lang: en
title: 'API docs: rest.resthttperrors'
keywords: LoopBack 4.0, LoopBack 4, Node.js, TypeScript, OpenAPI
sidebar: lb4_sidebar
editurl: https://github.com/loopbackio/loopback-next/tree/master/packages/rest
permalink: /doc/en/lb4/apidocs.rest.resthttperrors.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/rest](./rest.md) &gt; [RestHttpErrors](./rest.resthttperrors.md)

## RestHttpErrors namespace

<b>Signature:</b>

```typescript
export declare namespace RestHttpErrors 
```

## Functions

|  Function | Description |
|  --- | --- |
|  [invalidData(data, name, extraProperties)](./rest.resthttperrors.invaliddata.md) |  |
|  [invalidParamLocation(location)](./rest.resthttperrors.invalidparamlocation.md) |  |
|  [invalidRequestBody(details)](./rest.resthttperrors.invalidrequestbody.md) |  |
|  [missingRequired(name)](./rest.resthttperrors.missingrequired.md) |  |
|  [unsupportedMediaType(contentType, allowedTypes)](./rest.resthttperrors.unsupportedmediatype.md) |  |

## Interfaces

|  Interface | Description |
|  --- | --- |
|  [ValidationErrorDetails](./rest.resthttperrors.validationerrordetails.md) | An invalid request body error contains a <code>details</code> property as the machine-readable error. Each entry in <code>error.details</code> contains 4 attributes: <code>path</code>, <code>code</code>, <code>info</code> and <code>message</code>. <code>ValidationErrorDetails</code> defines the type of each entry, which is an object. The type of <code>error.details</code> is <code>ValidationErrorDetails[]</code>. |

## Variables

|  Variable | Description |
|  --- | --- |
|  [INVALID\_REQUEST\_BODY\_MESSAGE](./rest.resthttperrors.invalid_request_body_message.md) |  |


