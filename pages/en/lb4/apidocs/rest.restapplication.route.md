---
lang: en
title: 'API docs: rest.restapplication.route'
keywords: LoopBack 4.0, LoopBack 4
sidebar: lb4_sidebar
permalink: /doc/en/lb4/apidocs.rest.restapplication.route.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/rest](./rest.md) &gt; [RestApplication](./rest.restapplication.md) &gt; [route](./rest.restapplication.route.md)

## RestApplication.route() method

Register a new Controller-based route.

<b>Signature:</b>

```typescript
route<T>(verb: string, path: string, spec: OperationObject, controllerCtor: ControllerClass<T>, controllerFactory: ControllerFactory<T>, methodName: string): Binding;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  verb | <code>string</code> | HTTP verb of the endpoint |
|  path | <code>string</code> | URL path of the endpoint |
|  spec | <code>OperationObject</code> | The OpenAPI spec describing the endpoint (operation) |
|  controllerCtor | <code>ControllerClass&lt;T&gt;</code> | Controller constructor |
|  controllerFactory | <code>ControllerFactory&lt;T&gt;</code> | A factory function to create controller instance |
|  methodName | <code>string</code> | The name of the controller method |

<b>Returns:</b>

`Binding`

## Example


```ts
class MyController {
  greet(name: string) {
    return `hello ${name}`;
  }
}
app.route('get', '/greet', operationSpec, MyController, 'greet');

```


