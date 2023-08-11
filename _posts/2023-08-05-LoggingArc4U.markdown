---
layout: post
title:  "Arc4U in Jekyll!"
date:   2023-08-05 11:04:48 +0200
categories: jekyll update
---
# What can you do with Arc4u?

## Elia Architectural Framework

Arc4u is a framework providing support for many common tasks and problems that need to be solved in Elia applications written [in.NET](http://in.NET) (Core).

The specific areas of the support that is provided are:

* Logging / Diagnostics
* Dependency Injection
* Serialization
* Caching
* OData support
* Authentication
* gRPC
* Data Layer helpers
* Entity Framework Core helpers
* Unclassified

In addition, Arc4u provides helpers, abstractions, extensions and utilities for specific .NET products and technologies used in Elia projects:

* [Prism](https://prismlibrary.com/)
* [MongoDB](https://www.mongodb.com/)
* [NServiceBus](https://particular.net/nservicebus)
* [KubeMQ](https://kubemq.io/)

## Logging / Diagnostics

### Logging category support

Although .NET Core already provides logging, Arc4u provides methods specifying different common logging categories in Elia applications:

* Technical: logging concerning technical (IT) stuff
* Business: logging that concerns business rules
* Monitoring: logging concerning performance monitoring like CPU and memory

They correspond to what is defined in [Arc4u/MessageCategory.cs at master · GFlisch/Arc4u (github.com)](https://github.com/GFlisch/Arc4u/blob/master/src/Arc4u.Standard.Diagnostics/MessageCategory.cs) . The categories are used in reporting and other scenarios where it is necessary to reduce "unwanted noise" in what is being logged.

These categories are built on the standard .NET Core ILogger and are supported in a fluent way. See [Arc4u/ILoggerExtension.cs at master · GFlisch/Arc4u (github.com)](https://github.com/GFlisch/Arc4u/blob/master/src/Arc4u.Standard.Diagnostics/Fluent/ILoggerExtension.cs). This allows us to write:

```
logger.Technical().Information(<span class="hljs-string">"Start the Api process."</span>).Log();
logger.Business().Warning(<span class="hljs-string">"User Not Found"</span>).Log();
```

... resulting in cleaner code.

```
npm install --production
NODE_ENV=production node app
```

### Paris

Paris is the capital of France.

### Tokyo

Tokyo is the capital of Japan.
