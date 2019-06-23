---
lang: en
title: 'API docs: rest.requestcontext'
keywords: LoopBack 4.0, LoopBack 4
sidebar: lb4_sidebar
permalink: /doc/en/lb4/apidocs.rest.requestcontext.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/rest](./rest.md) &gt; [RequestContext](./rest.requestcontext.md)

## RequestContext class

A per-request Context combining an IoC container with handler context (request, response, etc.).

<b>Signature:</b>

```typescript
export declare class RequestContext extends Context implements HandlerContext 
```

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(request, response, parent, serverConfig, name)](./rest.requestcontext._constructor_.md) |  | Constructs a new instance of the <code>RequestContext</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [basePath](./rest.requestcontext.basepath.md) |  | <code>string</code> | Get the effective base path of the incoming request. This base path combines <code>baseUrl</code> provided by Express when LB4 handler is mounted on a non-root path, with the <code>basePath</code> value configured at LB4 side. |
|  [request](./rest.requestcontext.request.md) |  | <code>Request</code> |  |
|  [requestedBaseUrl](./rest.requestcontext.requestedbaseurl.md) |  | <code>string</code> | Get the base URL used by the client to make the request. This URL contains the protocol, hostname, port and base path. The path of the invoked route and query string is not included.<!-- -->Please note these values may be different from what we are observing at HTTP/TCP level, because reverse proxies like nginx are rewriting them. |
|  [requestedProtocol](./rest.requestcontext.requestedprotocol.md) |  | <code>string</code> | Get the protocol used by the client to make the request. Please note this protocol may be different from what we are observing at HTTP/TCP level, because reverse proxies like nginx or sidecars like Envoy are switching between protocols. |
|  [response](./rest.requestcontext.response.md) |  | <code>Response</code> |  |
|  [serverConfig](./rest.requestcontext.serverconfig.md) |  | <code>RestServerResolvedConfig</code> |  |

