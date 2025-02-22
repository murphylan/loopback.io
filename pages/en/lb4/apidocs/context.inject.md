---
lang: en
title: 'API docs: context.inject'
keywords: LoopBack 4.0, LoopBack 4, Node.js, TypeScript, OpenAPI
sidebar: lb4_sidebar
editurl: https://github.com/loopbackio/loopback-next/tree/master/packages/context
permalink: /doc/en/lb4/apidocs.context.inject.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/context](./context.md) &gt; [inject](./context.inject.md)

## inject namespace

<b>Signature:</b>

```typescript
export declare namespace inject 
```

## Variables

|  Variable | Description |
|  --- | --- |
|  [binding](./context.inject.binding.md) | Inject the binding object for the given key. This is useful if a binding needs to be set up beyond just a constant value allowed by <code>@inject.setter</code>. The injected binding is found or created based on the <code>metadata.bindingCreation</code> option. See <code>BindingCreationPolicy</code> for more details. |
|  [context](./context.inject.context.md) | Inject the context object. |
|  [getter](./context.inject.getter.md) | Inject a function for getting the actual bound value.<!-- -->This is useful when implementing Actions, where the action is instantiated for Sequence constructor, but some of action's dependencies become bound only after other actions have been executed by the sequence.<!-- -->See also <code>Getter&lt;T&gt;</code>. |
|  [setter](./context.inject.setter.md) | Inject a function for setting (binding) the given key to a given value. (Only static/constant values are supported, it's not possible to bind a key to a class or a provider.)<!-- -->This is useful e.g. when implementing Actions that are contributing new Elements.<!-- -->See also <code>Setter&lt;T&gt;</code>. |
|  [tag](./context.inject.tag.md) | Inject an array of values by a tag pattern string or regexp |
|  [view](./context.inject.view.md) | Inject matching bound values by the filter function |


