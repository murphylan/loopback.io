---
lang: en
title: 'API docs: pooling.createpooledbindingfactory'
keywords: LoopBack 4.0, LoopBack 4, Node.js, TypeScript, OpenAPI
sidebar: lb4_sidebar
editurl: https://github.com/loopbackio/loopback-next/tree/master/extensions/pooling
permalink: /doc/en/lb4/apidocs.pooling.createpooledbindingfactory.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/pooling](./pooling.md) &gt; [createPooledBindingFactory](./pooling.createpooledbindingfactory.md)

## createPooledBindingFactory() function

Create a function to return a pooled binding factory

<b>Signature:</b>

```typescript
export declare function createPooledBindingFactory<T extends object>(bindingAddress: BindingAddress<T>): (context: Context) => PoolFactory<T>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  bindingAddress | [BindingAddress](./context.bindingaddress.md)<!-- -->&lt;T&gt; | Binding address |

<b>Returns:</b>

(context: [Context](./context.context.md)<!-- -->) =&gt; [PoolFactory](./pooling.poolfactory.md)<!-- -->&lt;T&gt;


