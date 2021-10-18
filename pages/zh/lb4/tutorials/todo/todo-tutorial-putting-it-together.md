---
lang: zh
title: '把它们放在一起'
layout: translation
keywords: LoopBack 4.0, LoopBack 4, Node.js, TypeScript, OpenAPI, Tutorial
sidebar: zh_lb4_sidebar
permalink: /doc/zh/lb4/todo-tutorial-putting-it-together.html
---

### 把它们放在一起

我们已经完成了所有的组件，且它们都是自动绑定到我们的[应用程序](../../Application.md) 上，这样LoopBack的
[依赖注入](../../Dependency-injection.md) 系统就可以为我们把所有的组件联系在一起！

LoopBack的[启动模块](https://github.com/loopbackio/loopback-next/tree/master/packages/boot)将自动发现我们的控制器（Controllers）、
存储库（Repositories）、数据源（Datasources）和其他组件，并将它们注入我们的应用程序中使用。

> **注意**: 启动模块将扫描约定目录下的组件并自动注入它们。下面是默认组件分别对应目录的示例：
>
> - 控制器（Controllers）: `./src/controllers`
> - 数据源（Datasources）: `./src/datasources`
> - 模型（Models）: `./src/models`
> - 存储库（Repositories）: `./src/repositories`
>
> 要了解如何自定义这种行为，请看应用程序的[启动应用](../../Booting-an-Application.md#booters)部分。

让我们尝试一下我们的应用程序，首先，使用下面的命令启动应用程序。

```sh
$ npm start

Server is running at http://127.0.0.1:3000  
```

接下来，你可以使用API Explorer来浏览API，并提交Request请求!

{% include note.html content="
当使用API Explorer时, 请务必清空默认的<i><b>filter</b></i> 或者 <i><b>where</b></i> 区域的参数，这样才能返回期望的数据。" %}

这里是一些常见的测试请求：

- `POST /todos` 请求中附带请求体内容 `{ "title": "get the milk" }`
- `GET /todos/{id}`使用ID检索上一条 `POST` 请求创建的数据，查看是否有结果返回。
- `PATCH /todos/{id}`, 使用相同的ID, 同时请求中附带请求体内容
  `{ "desc": "need milk for cereal" }`

以上内容就是你刚刚创建了的第一个LoopBack 4应用程序!

_提醒: 使用 **CTRL+C** 快捷键停止运行中的程序_

### Where to go from here

There are still a ton of features you can use to build on top of the
`TodoListApplication`. Here are some tutorials that continues off from where we
left off here to guide you through adding in an additional feature:

- **Integrate with a REST based geo-coding service**: A typical REST API server
  needs to access data from a variety of sources, including SOAP or REST
  services. Continue to the bonus section to learn how LoopBack connectors make
  it super easy to fetch data from other services and
  [enhance your Todo application with location-based reminders](todo-tutorial-geocoding-service.md).
- **Add related Model with TodoListApplication**: If you would like to try out
  using some of the more advanced features of LoopBack 4 such as relations, try
  out the
  [TodoList tutorial](https://loopback.io/doc/en/lb4/todo-list-tutorial.html)
  which continues off from where we leave here.

### More examples and tutorials

Eager to continue learning about LoopBack 4? Check out our
[Examples](../../Examples.md) and [Tutorials](../../Tutorials.md) sections to
find examples for creating your own custom components, sequences and more!

In fact, this example can be simplified to only defining the model and
datasource, while still behaving the same. Using
[`CrudRestComponent`](https://loopback.io/doc/en/lb4/apidocs.rest-crud.crudrestcomponent.html),
the repository and controller classes can be omitted, as seen in the
[rest-crud example](https://github.com/loopbackio/loopback-next/tree/master/examples/rest-crud).

### Navigation

Previous step: [Add a controller](todo-tutorial-controller.md)
