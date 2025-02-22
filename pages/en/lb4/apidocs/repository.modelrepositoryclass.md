---
lang: en
title: 'API docs: repository.modelrepositoryclass'
keywords: LoopBack 4.0, LoopBack 4, Node.js, TypeScript, OpenAPI
sidebar: lb4_sidebar
editurl: https://github.com/loopbackio/loopback-next/tree/master/packages/repository
permalink: /doc/en/lb4/apidocs.repository.modelrepositoryclass.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/repository](./repository.md) &gt; [ModelRepositoryClass](./repository.modelrepositoryclass.md)

## ModelRepositoryClass interface

Signature for a Repository class bound to a given model. The constructor accepts only the dataSource to use for persistence.

`define*` functions return a class implementing this interface.

<b>Signature:</b>

```typescript
export interface ModelRepositoryClass<M extends Model, R extends Repository<M>> 
```

## Properties

|  Property | Type | Description |
|  --- | --- | --- |
|  [prototype](./repository.modelrepositoryclass.prototype.md) | R |  |

## Methods

|  Method | Description |
|  --- | --- |
|  [(new)(dataSource)](./repository.modelrepositoryclass._new_.md) | The constructor for the generated repository class |


