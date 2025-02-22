---
lang: en
title: 'API docs: rest'
keywords: LoopBack 4.0, LoopBack 4, Node.js, TypeScript, OpenAPI
sidebar: lb4_sidebar
editurl: https://github.com/loopbackio/loopback-next/tree/master/packages/rest
permalink: /doc/en/lb4/apidocs.rest.html
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@loopback/rest](./rest.md)

## rest package

The REST API package for loopback-next.

## Remarks

A REST server for LoopBack 4 application instances, complete with:

- new custom routing engine (special thanks to @<!-- -->bajtos)! - tools for defining your application routes - OpenAPI 3.0 spec (openapi.json/openapi.yaml) generation using @<!-- -->loopback/openapi-v3 - a default sequence implementation to manage the request and response lifecycle

## Classes

|  Class | Description |
|  --- | --- |
|  [BaseRoute](./rest.baseroute.md) | Base implementation of RouteEntry |
|  [ControllerRoute](./rest.controllerroute.md) | A route backed by a controller |
|  [DefaultSequence](./rest.defaultsequence.md) | The default implementation of SequenceHandler. |
|  [FindRouteMiddlewareProvider](./rest.findroutemiddlewareprovider.md) |  |
|  [FindRouteProvider](./rest.findrouteprovider.md) |  |
|  [HttpHandler](./rest.httphandler.md) |  |
|  [InfoSpecEnhancer](./rest.infospecenhancer.md) | An OpenAPI spec enhancer to populate <code>info</code> with application metadata (package.json). |
|  [InvokeMethodMiddlewareProvider](./rest.invokemethodmiddlewareprovider.md) |  |
|  [InvokeMethodProvider](./rest.invokemethodprovider.md) |  |
|  [JsonBodyParser](./rest.jsonbodyparser.md) |  |
|  [LogErrorProvider](./rest.logerrorprovider.md) |  |
|  [MiddlewareSequence](./rest.middlewaresequence.md) | A sequence implementation using middleware chains |
|  [ParseParamsMiddlewareProvider](./rest.parseparamsmiddlewareprovider.md) |  |
|  [ParseParamsProvider](./rest.parseparamsprovider.md) | Provides the function for parsing args in requests at runtime. |
|  [RawBodyParser](./rest.rawbodyparser.md) | Parsing the request body into Buffer |
|  [RedirectRoute](./rest.redirectroute.md) |  |
|  [RegExpRouter](./rest.regexprouter.md) | Router implementation based on regexp matching |
|  [RejectProvider](./rest.rejectprovider.md) |  |
|  [RequestBodyParser](./rest.requestbodyparser.md) |  |
|  [RequestContext](./rest.requestcontext.md) | A per-request Context combining an IoC container with handler context (request, response, etc.). |
|  [RestApplication](./rest.restapplication.md) | An implementation of the Application class that automatically provides an instance of a REST server. This application class is intended to be a single-server implementation. Any attempt to bind additional servers will throw an error. |
|  [RestComponent](./rest.restcomponent.md) |  |
|  [RestServer](./rest.restserver.md) | A REST API server for use with Loopback. Add this server to your application by importing the RestComponent. |
|  [Route](./rest.route.md) |  |
|  [RouteSource](./rest.routesource.md) |  |
|  [RoutingTable](./rest.routingtable.md) | Routing table |
|  [SendProvider](./rest.sendprovider.md) | Provides the function that populates the response object with the results of the operation. |
|  [SendResponseMiddlewareProvider](./rest.sendresponsemiddlewareprovider.md) |  |
|  [StreamBodyParser](./rest.streambodyparser.md) | A special body parser to retain request stream as is. It will be used by explicitly setting <code>x-parser</code> to <code>'stream'</code> in the request body spec. |
|  [TextBodyParser](./rest.textbodyparser.md) |  |
|  [Trie](./rest.trie.md) | An implementation of trie for routes. The key hierarchy is built with parts of the route path delimited by <code>/</code> |
|  [TrieRouter](./rest.trierouter.md) | Router implementation based on trie |
|  [UrlEncodedBodyParser](./rest.urlencodedbodyparser.md) |  |

## Functions

|  Function | Description |
|  --- | --- |
|  [assignRouterSpec(target, additions)](./rest.assignrouterspec.md) |  |
|  [compareRoute(route1, route2)](./rest.compareroute.md) | Compare two routes by verb/path for sorting |
|  [createBodyParserBinding(parserClass, key)](./rest.createbodyparserbinding.md) | Create a binding for the given body parser class |
|  [createControllerFactoryForBinding(key)](./rest.createcontrollerfactoryforbinding.md) | Create a controller factory function for a given binding key |
|  [createControllerFactoryForClass(controllerCtor)](./rest.createcontrollerfactoryforclass.md) | Create a controller factory function for a given class |
|  [createControllerFactoryForInstance(controllerInst)](./rest.createcontrollerfactoryforinstance.md) | Create a controller factory function for a given instance |
|  [createResolvedRoute(route, pathParams)](./rest.createresolvedroute.md) |  |
|  [createRoutesForController(spec, controllerCtor, controllerFactory)](./rest.createroutesforcontroller.md) | Create routes for a controller with the given spec |
|  [getContentType(req)](./rest.getcontenttype.md) | Get the content-type header value from the request |
|  [getParserOptions(type, options)](./rest.getparseroptions.md) | Extract parser options based on the parser type |
|  [getParserOptions(type, options)](./rest.getparseroptions_1.md) |  |
|  [getParserOptions(type, options)](./rest.getparseroptions_2.md) |  |
|  [getParserOptions(type, options)](./rest.getparseroptions_3.md) |  |
|  [getPathVariables(path)](./rest.getpathvariables.md) | Get all path variables. For example, <code>/root/{foo}/bar</code> =<!-- -->&gt; <code>['foo']</code> |
|  [invokeBodyParserMiddleware(handle, request)](./rest.invokebodyparsermiddleware.md) | Parse the request body asynchronously |
|  [joinPath(basePath, path)](./rest.joinpath.md) |  |
|  [normalizeParsingError(err)](./rest.normalizeparsingerror.md) | Normalize parsing errors as <code>4xx</code> |
|  [parseJson(text, reviver, prohibitedKeys)](./rest.parsejson.md) | Parse a json string that rejects prohibited keys |
|  [parseOperationArgs(request, route, requestBodyParser, options)](./rest.parseoperationargs.md) | Parses the request to derive arguments to be passed in for the Application controller method |
|  [rebaseOpenApiSpec(spec, basePath)](./rest.rebaseopenapispec.md) |  |
|  [sanitizeJsonParse(reviver, prohibitedKeys)](./rest.sanitizejsonparse.md) | Factory to create a reviver function for <code>JSON.parse</code> to sanitize keys |
|  [toExpressPath(path)](./rest.toexpresspath.md) | Convert an OpenAPI path to Express (path-to-regexp) style |
|  [validateApiPath(path)](./rest.validateapipath.md) | Validate the path to be compatible with OpenAPI path template. No parameter modifier, custom pattern, or unnamed parameter is allowed. |
|  [validateRequestBody(body, requestBodySpec, globalSchemas, options)](./rest.validaterequestbody.md) | Check whether the request body is valid according to the provided OpenAPI schema. The JSON schema is generated from the OpenAPI schema which is typically defined by <code>@requestBody()</code>. The validation leverages AJV schema validator. |
|  [validateValueAgainstSchema(value, schema, globalSchemas, options)](./rest.validatevalueagainstschema.md) | Validate the value against JSON schema. |
|  [writeResultToResponse(response, result)](./rest.writeresulttoresponse.md) | Writes the result from Application controller method into the HTTP response |

## Interfaces

|  Interface | Description |
|  --- | --- |
|  [ApiExplorerOptions](./rest.apiexploreroptions.md) |  |
|  [BodyParser](./rest.bodyparser.md) | Interface to be implemented by body parser extensions |
|  [HttpServerLike](./rest.httpserverlike.md) |  |
|  [Node](./rest.node.md) | A Node in the trie |
|  [OpenApiSpecForm](./rest.openapispecform.md) | The form of OpenAPI specs to be served |
|  [OpenApiSpecOptions](./rest.openapispecoptions.md) | Options to customize how OpenAPI specs are served |
|  [RequestBodyParserOptions](./rest.requestbodyparseroptions.md) | Options for request body parsing See https://github.com/expressjs/body-parser/\#options<!-- -->Built-in parsers retrieve their own options from the request body parser options. The parser specific properties override common ones. |
|  [RequestWithSession](./rest.requestwithsession.md) | extending express request type with a session field |
|  [ResolvedNode](./rest.resolvednode.md) |  |
|  [ResolvedRoute](./rest.resolvedroute.md) | A route with path parameters resolved |
|  [RestRouter](./rest.restrouter.md) |  |
|  [RestServerResolvedOptions](./rest.restserverresolvedoptions.md) |  |
|  [RouteEntry](./rest.routeentry.md) | An entry in the routing table |
|  [SequenceHandler](./rest.sequencehandler.md) | A sequence handler is a class implementing sequence of actions required to handle an incoming request. |
|  [Session](./rest.session.md) | interface to set variables in user session |
|  [SessionUserProfile](./rest.sessionuserprofile.md) | user profile to add in session |
|  [ValidationOptions](./rest.validationoptions.md) | Options for request body validation using AJV |
|  [ValueValidationOptions](./rest.valuevalidationoptions.md) | Options for any value validation using AJV |

## Namespaces

|  Namespace | Description |
|  --- | --- |
|  [builtinParsers](./rest.builtinparsers.md) |  |
|  [RestBindings](./rest.restbindings.md) | RestServer-specific bindings |
|  [RestHttpErrors](./rest.resthttperrors.md) |  |
|  [RestMiddlewareGroups](./rest.restmiddlewaregroups.md) | Built-in middleware groups for the REST sequence |
|  [RestTags](./rest.resttags.md) | Binding tags for RestServer |

## Variables

|  Variable | Description |
|  --- | --- |
|  [DEFAULT\_LIMIT](./rest.default_limit.md) |  |
|  [ERR\_NO\_MULTI\_SERVER](./rest.err_no_multi_server.md) |  |
|  [REQUEST\_BODY\_PARSER\_TAG](./rest.request_body_parser_tag.md) | Binding tag for request body parser extensions |
|  [SequenceActions](./rest.sequenceactions.md) |  |

## Type Aliases

|  Type Alias | Description |
|  --- | --- |
|  [AjvErrorOptions](./rest.ajverroroptions.md) | Options for AJV errors |
|  [AjvFactory](./rest.ajvfactory.md) | Factory function for Ajv instances |
|  [AjvFormat](./rest.ajvformat.md) | Ajv format definition with a name |
|  [AjvKeyword](./rest.ajvkeyword.md) | Ajv keyword definition with a name |
|  [BodyParserFunction](./rest.bodyparserfunction.md) | Plain function for body parsing |
|  [BodyParserMiddleware](./rest.bodyparsermiddleware.md) | Express body parser function type |
|  [ControllerClass](./rest.controllerclass.md) | Controller class |
|  [ControllerFactory](./rest.controllerfactory.md) | A factory function to create controller instances synchronously or asynchronously |
|  [ControllerInstance](./rest.controllerinstance.md) |  |
|  [FindRoute](./rest.findroute.md) | Find a route matching the incoming request. Throw an error when no route was found. |
|  [HttpRequestListener](./rest.httprequestlistener.md) |  |
|  [InvokeMethod](./rest.invokemethod.md) | Invokes a method defined in the Application Controller |
|  [LogError](./rest.logerror.md) | Log information about a failed request. |
|  [NodeWithValue](./rest.nodewithvalue.md) |  |
|  [OperationArgs](./rest.operationargs.md) |  |
|  [OperationRetval](./rest.operationretval.md) | Return value of a controller method (a function implementing an operation). This is a type alias for "any", used to distinguish operation results from other "any" typed values. |
|  [ParseParams](./rest.parseparams.md) | A function to parse OpenAPI operation parameters for a given route |
|  [PathParameterValues](./rest.pathparametervalues.md) |  |
|  [Reject](./rest.reject.md) | Reject the request with an error. |
|  [RequestBody](./rest.requestbody.md) | Request body with metadata |
|  [RequestBodyValidationOptions](./rest.requestbodyvalidationoptions.md) |  |
|  [RestComponentConfig](./rest.restcomponentconfig.md) |  |
|  [RestRouterOptions](./rest.restrouteroptions.md) |  |
|  [RestServerConfig](./rest.restserverconfig.md) | Valid configuration for the RestServer constructor. |
|  [RestServerOptions](./rest.restserveroptions.md) | RestServer options |
|  [RestServerResolvedConfig](./rest.restserverresolvedconfig.md) |  |
|  [RouterSpec](./rest.routerspec.md) |  |
|  [SchemaValidatorCache](./rest.schemavalidatorcache.md) | Cache for AJV schema validators |
|  [Send](./rest.send.md) | Send the operation response back to the client. |
|  [SequenceFunction](./rest.sequencefunction.md) | A sequence function is a function implementing a custom sequence of actions to handle an incoming request. |


