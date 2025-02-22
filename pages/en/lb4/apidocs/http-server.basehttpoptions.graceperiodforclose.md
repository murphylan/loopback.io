---
lang: en
title: 'API docs: http-server.basehttpoptions.graceperiodforclose'
keywords: LoopBack 4.0, LoopBack 4, Node.js, TypeScript, OpenAPI
sidebar: lb4_sidebar
editurl: https://github.com/loopbackio/loopback-next/tree/master/packages/http-server
permalink: /doc/en/lb4/apidocs.http-server.basehttpoptions.graceperiodforclose.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/http-server](./http-server.md) &gt; [BaseHttpOptions](./http-server.basehttpoptions.md) &gt; [gracePeriodForClose](./http-server.basehttpoptions.graceperiodforclose.md)

## BaseHttpOptions.gracePeriodForClose property

The `gracePeriodForClose` property controls how to stop the server gracefully. Its value is the number of milliseconds to wait before in-flight requests finish when the server is being stopped. With this setting, we also reject new requests from existing keep-alive connections in addition to stopping accepting new connections.

Defaults to Infinity (don't force-close). If you want to immediately destroy all sockets set its value to `0`<!-- -->.

See [stoppable](https://www.npmjs.com/package/stoppable)

<b>Signature:</b>

```typescript
gracePeriodForClose?: number;
```

