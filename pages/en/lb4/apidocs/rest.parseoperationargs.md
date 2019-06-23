---
lang: en
title: 'API docs: rest.parseoperationargs'
keywords: LoopBack 4.0, LoopBack 4
sidebar: lb4_sidebar
permalink: /doc/en/lb4/apidocs.rest.parseoperationargs.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/rest](./rest.md) &gt; [parseOperationArgs](./rest.parseoperationargs.md)

## parseOperationArgs() function

Parses the request to derive arguments to be passed in for the Application controller method

<b>Signature:</b>

```typescript
export declare function parseOperationArgs(request: Request, route: ResolvedRoute, requestBodyParser?: RequestBodyParser, options?: RequestBodyValidationOptions): Promise<OperationArgs>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  request | <code>Request</code> | Incoming HTTP request |
|  route | <code>ResolvedRoute</code> | Resolved Route |
|  requestBodyParser | <code>RequestBodyParser</code> |  |
|  options | <code>RequestBodyValidationOptions</code> |  |

<b>Returns:</b>

`Promise<OperationArgs>`

