---
lang: en
title: 'API docs: context.bindingkey'
keywords: LoopBack 4.0, LoopBack 4, Node.js, TypeScript, OpenAPI
sidebar: lb4_sidebar
editurl: https://github.com/loopbackio/loopback-next/tree/master/packages/context
permalink: /doc/en/lb4/apidocs.context.bindingkey.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/context](./context.md) &gt; [BindingKey](./context.bindingkey.md)

## BindingKey class

<b>Signature:</b>

```typescript
export declare class BindingKey<ValueType> 
```

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [CONFIG\_NAMESPACE](./context.bindingkey.config_namespace.md) | <code>static</code> | string | Name space for configuration binding keys |
|  [key](./context.bindingkey.key.md) |  | string |  |
|  [PROPERTY\_SEPARATOR](./context.bindingkey.property_separator.md) | <code>static</code> | (not declared) |  |
|  [propertyPath?](./context.bindingkey.propertypath.md) |  | string \| undefined | <i>(Optional)</i> |

## Methods

|  Method | Modifiers | Description |
|  --- | --- | --- |
|  [buildKeyForConfig(key)](./context.bindingkey.buildkeyforconfig.md) | <code>static</code> | Build a binding key for the configuration of the given binding. The format is <code>&lt;key&gt;:$config</code> |
|  [create(key, propertyPath)](./context.bindingkey.create.md) | <code>static</code> | Create a new key for a binding bound to a value of type <code>ValueType</code>. |
|  [deepProperty(propertyPath)](./context.bindingkey.deepproperty.md) |  | Get a binding address for retrieving a deep property of the object bound to the current binding key. |
|  [generate(namespace)](./context.bindingkey.generate.md) | <code>static</code> | Generate a universally unique binding key.<!-- -->Please note the format of they generated key is not specified, you must not rely on any specific formatting (e.g. UUID style). |
|  [parseKeyWithPath(keyWithPath)](./context.bindingkey.parsekeywithpath.md) | <code>static</code> | Parse a string containing both the binding key and the path to the deeply nested property to retrieve. |
|  [toString()](./context.bindingkey.tostring.md) |  |  |
|  [validate(key)](./context.bindingkey.validate.md) | <code>static</code> | Validate the binding key format. Please note that <code>#</code> is reserved. Returns a string representation of the binding key. |


