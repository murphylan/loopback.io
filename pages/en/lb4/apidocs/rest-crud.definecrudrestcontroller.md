---
lang: en
title: 'API docs: rest-crud.definecrudrestcontroller'
keywords: LoopBack 4.0, LoopBack 4, Node.js, TypeScript, OpenAPI
sidebar: lb4_sidebar
editurl: https://github.com/loopbackio/loopback-next/tree/master/packages/rest-crud
permalink: /doc/en/lb4/apidocs.rest-crud.definecrudrestcontroller.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/rest-crud](./rest-crud.md) &gt; [defineCrudRestController](./rest-crud.definecrudrestcontroller.md)

## defineCrudRestController() function

Create (define) a CRUD Controller class for the given model.

<b>Signature:</b>

```typescript
export declare function defineCrudRestController<T extends Entity, IdType, IdName extends keyof T, Relations extends object = {}>(modelCtor: typeof Entity & {
    prototype: T & {
        [key in IdName]: IdType;
    };
}, options: CrudRestControllerOptions): CrudRestControllerCtor<T, IdType, IdName, Relations>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  modelCtor | typeof [Entity](./repository.entity.md) &amp; { prototype: T &amp; { \[key in IdName\]: IdType; }; } | A model class, e.g. <code>Product</code>. |
|  options | [CrudRestControllerOptions](./rest-crud.crudrestcontrolleroptions.md) | Configuration options, e.g. <code>{basePath: '/products'}</code>. |

<b>Returns:</b>

[CrudRestControllerCtor](./rest-crud.crudrestcontrollerctor.md)<!-- -->&lt;T, IdType, IdName, Relations&gt;

## Example


```ts
const ProductController = defineCrudRestController<
Product,
typeof Product.prototype.id,
'id'
>(Product, {basePath: '/products'});

inject('repositories.ProductRepository')(
 ProductController,
  undefined,
  0,
);

app.controller(ProductController);
```


