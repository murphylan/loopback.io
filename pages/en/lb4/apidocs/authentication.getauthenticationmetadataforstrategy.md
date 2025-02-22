---
lang: en
title: 'API docs: authentication.getauthenticationmetadataforstrategy'
keywords: LoopBack 4.0, LoopBack 4, Node.js, TypeScript, OpenAPI
sidebar: lb4_sidebar
editurl: https://github.com/loopbackio/loopback-next/tree/master/packages/authentication
permalink: /doc/en/lb4/apidocs.authentication.getauthenticationmetadataforstrategy.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/authentication](./authentication.md) &gt; [getAuthenticationMetadataForStrategy](./authentication.getauthenticationmetadataforstrategy.md)

## getAuthenticationMetadataForStrategy() function

Get the authentication metadata object for the specified strategy.

<b>Signature:</b>

```typescript
export declare function getAuthenticationMetadataForStrategy(metadata: AuthenticationMetadata[], strategyName: string): AuthenticationMetadata | undefined;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  metadata | [AuthenticationMetadata](./authentication.authenticationmetadata.md)<!-- -->\[\] | Array of authentication metadata objects |
|  strategyName | string | Name of the authentication strategy |

<b>Returns:</b>

[AuthenticationMetadata](./authentication.authenticationmetadata.md) \| undefined


