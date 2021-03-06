# Examples

<a href="https://iris-go.com"> <img align="right" width="115px" src="https://iris-go.com/images/icon.svg?v=a" title="logo created by @merry.dii" /> </a>

<a href="https://travis-ci.org/kataras/iris"><img src="https://img.shields.io/travis/kataras/iris.svg?style=flat-square" alt="Build Status"></a>
<a href="https://github.com/iris-contrib/examples/blob/v12/LICENSE"><img src="https://img.shields.io/badge/%20license-MIT%20%20License%20-E91E63.svg?style=flat-square" alt="License"></a>
<a href="https://github.com/kataras/iris/blob/master/HISTORY.md"><img src="https://img.shields.io/badge/version-v12.2.x%20-blue.svg?style=flat-square" alt="CHANGELOG/HISTORY"></a>

This repository provides easy to understand code snippets on how to get started with web development with the Go programming language using the [Iris](https://github.com/kataras/iris) web framework. This branch contains the latest [iris master examples](github.com/kataras/iris/tree/master). For the stable's version examples navigate through the [v12 branch](https://github.com/iris-contrib/examples/tree/v12).

To read the Iris documentation please navigate to [the wiki pages](https://github.com/kataras/iris/wiki) instead.

> Examples are tested using Windows 10, Ubuntu 20.04 with [Microsoft's Visual Studio Code](https://code.visualstudio.com/) and built using the [Go 1.15.0](https://golang.org/dl).

# Table of Contents

* [Serverless](https://github.com/iris-contrib/gateway#netlify)
* [REST API for Apache Kafka](kafka-api)
* [URL Shortener](url-shortener)
* [Dropzone.js](dropzonejs)
* [Caddy](caddy)
* Database
    * [MySQL, Groupcache & Docker](database/mysql)
    * [MongoDB](database/mongodb)
    * [Sqlx](database/orm/sqlx/main.go)
    * [Xorm](database/orm/xorm/main.go)
    * [Gorm](database/orm/gorm/main.go)
    * [Reform](database/orm/reform/main.go)
* HTTP Server
    * [HOST:PORT](http-server/listen-addr/main.go)
    * [Public Test Domain](http-server/listen-addr-public/main.go)
    * [UNIX socket file](http-server/listen-unix/main.go)
    * [TLS](http-server/listen-tls/main.go)
    * [Letsencrypt (Automatic Certifications)](http-server/listen-letsencrypt/main.go)
    * [Socket Sharding (SO_REUSEPORT)](http-server/socket-sharding/main.go)
    * [Graceful Shutdown](http-server/graceful-shutdown/default-notifier/main.go)
    * [Notify on shutdown](http-server/notify-on-shutdown/main.go)
    * Custom TCP Listener
        * [Common net.Listener](http-server/custom-listener/main.go)
    * Custom HTTP Server
        * [Pass a custom Server](http-server/custom-httpserver/easy-way/main.go)
        * [Use Iris as a single http.Handler](http-server/custom-httpserver/std-way/main.go)
        * [Multi Instances](http-server/custom-httpserver/multi/main.go)
        * [HTTP/3 Quic](http-server/http3-quic)
* Configuration
    * [Functional](configuration/functional/main.go)
    * [Configuration Struct](configuration/from-configuration-structure/main.go)
    * [Import from YAML](configuration/from-yaml-file/main.go)
        * [Share Configuration across instances](configuration/from-yaml-file/shared-configuration/main.go)
    * [Import from TOML](configuration/from-toml-file/main.go)
* Routing
    * [Overview](routing/overview/main.go)
    * [Basic](routing/basic/main.go)
    * [Custom HTTP Errors](routing/http-errors/main.go)
    * [Not Found - Intelligence](routing/intelligence/main.go)
        * [Not Found - Suggest Closest Paths](routing/intelligence/manual/main.go)
    * [Dynamic Path](routing/dynamic-path/main.go)
        * [Root Wildcard](routing/dynamic-path/root-wildcard/main.go)
        * [Implement a Parameter Type](routing/macros/main.go)
        * [Same Path Pattern but Func](routing/dynamic-path/same-pattern-different-func/main.go)
    * Middleware
        * [Per Route](routing/writing-a-middleware/per-route/main.go)
        * [Globally](routing/writing-a-middleware/globally/main.go)
        * [Handlers Execution Rule](routing/route-handlers-execution-rules/main.go)
        * [Route Register Rule](routing/route-register-rule/main.go)
        * Convert net/http Handlers
            * [From func(w http.ResponseWriter, r *http.Request, next http.HandlerFunc)](convert-handlers/negroni-like/main.go)
            * [From http.Handler or http.HandlerFunc](convert-handlers/nethttp/main.go)
            * [From func(http.HandlerFunc) http.HandlerFunc](convert-handlers/real-usecase-raven/writing-middleware/main.go)
    * [Rewrite Middleware](routing/rewrite/main.go)
    * [Route State](routing/route-state/main.go)
    * [Reverse Routing](routing/reverse/main.go)
    * [Router Wrapper](routing/custom-wrapper/main.go)
    * [Custom Router](routing/custom-router/main.go)
    * Subdomains
        * [Single](routing/subdomains/single/main.go)
        * [Multi](routing/subdomains/multi/main.go)
        * [Wildcard](routing/subdomains/wildcard/main.go)
        * [WWW](routing/subdomains/www/main.go)
            * [WWW Method](routing/subdomains/www/www-method/main.go)
        * [Redirection](routing/subdomains/redirect/main.go)
            * [Multi Instances](routing/subdomains/redirect/multi-instances/main.go)
        * [HTTP Errors View](routing/subdomains/http-errors-view/main.go)
    * [HTTP Method Override](https://github.com/kataras/iris/blob/master/middleware/methodoverride/methodoverride_test.go)
    * [API Versioning](routing/versioning/main.go)
    * [Sitemap](routing/sitemap/main.go)
* Logging
    * [Request Logger](logging/request-logger/main.go)
        * [AccessLog: simple example](logging/request-logger/accesslog-simple/main.go)
        * [AccessLog: log request & response and more](logging/request-logger/accesslog)
        * [AccessLog: custom fields and template](logging/request-logger/accesslog-template/main.go)
        * [AccessLog: CSV Format](logging/request-logger/accesslog-csv/main.go)
        * [AccessLog: listen to logs and render them](logging/request-logger/accesslog-broker/main.go)
        * [Log Requests to a JSON File](logging/request-logger/request-logger-file-json/main.go) 
    * [Application File Logger](logging/file-logger/main.go)
    * [Application JSON Logger](logging/json-logger/main.go)
    * [Rollbar](logging/rollbar/main.go)
* API Documentation
    * [Yaag](apidoc/yaag/main.go)
    * [Swagger](https://github.com/iris-contrib/swagger/tree/master/example)
* [Testing](testing/httptest/main_test.go)
* [Recovery](recover/main.go)
* [Profiling](pprof/main.go)
* File Server
    * [File Server](file-server/file-server/main.go)
    * [HTTP/2 Push Targets](file-server/http2push/main.go)
    * [HTTP/2 Push Targets (Embedded)](file-server/http2push-embedded/main.go)
    * [HTTP/2 Push Targets (Gzipped Embedded)](file-server/http2push-embedded-gzipped/main.go)
    * [Favicon](file-server/favicon/main.go)
    * [Basic](file-server/basic/main.go)
    * [Embedding Files Into App Executable File](file-server/embedding-files-into-app/main.go)
    * [Embedding Gzipped Files Into App Executable File](file-server/embedding-gzipped-files-into-app/main.go)
    * [Send Files (rate limiter included)](file-server/send-files/main.go)
    * Single Page Applications
        * [Basic SPA](file-server/single-page-application/basic/main.go)
        * [Embedded Single Page Application](file-server/single-page-application/embedded-single-page-application/main.go)
        * [Embedded Single Page Application with other routes](file-server/single-page-application/embedded-single-page-application-with-other-routes/main.go)
    * [Upload File](file-server/upload-file/main.go)
    * [Upload Multiple Files](file-server/upload-files/main.go)
* View
    * [Overview](view/overview/main.go)
    * [Basic](view/template_html_0/main.go)
    * [A simple Layout](view/template_html_1/main.go)
    * [Layouts: `yield` and `render` tmpl funcs](view/template_html_2/main.go)
    * [The `urlpath` tmpl func](view/template_html_3/main.go)
    * [The `url` tmpl func](view/template_html_4/main.go)
    * [Inject Data Between Handlers](view/context-view-data/main.go)
    * [Inject Engine Between Handlers](view/context-view-engine/main.go)
    * [Embedding Templates Into App Executable File](view/embedding-templates-into-app/main.go)
    * [Write to a custom `io.Writer`](view/write-to)
    * Parse a Template from Text
        * [HTML, Pug and Ace](view/parse-parse/main.go)
        * [Django](view/parse-parse/django/main.go)
        * [Amber](view/parse-parse/amber/main.go)
        * [Jet](view/parse-parse/jet/main.go)
        * [Handlebars](view/parse-parse/handlebars/main.go)
    * [Blocks](view/template_blocks_0)
    * [Blocks Embedded](view/template_blocks_1_embedded)
    * [Pug: `Actions`](view/template_pug_0)
    * [Pug: `Includes`](view/template_pug_1)
    * [Pug Embedded`](view/template_pug_2_embedded)
    * [Ace](view/template_ace_0)
    * [Django](view/template_django_0)
    * [Amber](view/template_amber_0)
    * [Amber Embedded](view/template_amber_1_embedded)
    * [Jet](view/template_jet_0)
    * [Jet Embedded](view/template_jet_1_embedded)
    * [Jet 'urlpath' tmpl func](view/template_jet_2)
    * [Jet Template Funcs from Struct](view/template_jet_3)
    * [Handlebars](view/template_handlebars_0)
    * Third-Parties
        * [Render `valyala/quicktemplate` templates](view/quicktemplate)
        * [Render `shiyanhui/hero` templates](view/herotemplate)
* [Request ID](https://github.com/kataras/iris/blob/master/middleware/requestid/requestid_test.go)
* [Request Rate Limit](request-ratelimit/main.go)
* [Request Referrer](request-referrer/main.go)
* [Webassembly](webassembly/main.go)
* Request Body
    * [Bind JSON](request-body/read-json/main.go)
    *   * [Struct Validation](request-body/read-json-struct-validation/main.go)
    * [Bind XML](request-body/read-xml/main.go)
    * [Bind MsgPack](request-body/read-msgpack/main.go)
    * [Bind YAML](request-body/read-yaml/main.go)
    * [Bind Form](request-body/read-form/main.go)
        * [Checkboxes](request-body/read-form/checkboxes/main.go)
    * [Bind Query](request-body/read-query/main.go)
    * [Bind Headers](request-body/read-headers/main.go)
    * [Bind Params](request-body/read-params/main.go)
    * [Bind Body](request-body/read-body/main.go)
    * [Bind Custom per type](request-body/read-custom-per-type/main.go)
    * [Bind Custom via Unmarshaler](request-body/read-custom-via-unmarshaler/main.go)
    * [Bind Many times](request-body/read-many/main.go)
* Response Writer
    * [Content Negotiation](response-writer/content-negotiation)
    * [Text, Markdown, YAML, HTML, JSON, JSONP, Msgpack, XML and Binary](response-writer/write-rest/main.go)
    * [Protocol Buffers](response-writer/protobuf/main.go)
    * [HTTP/2 Server Push](response-writer/http2push/main.go)
    * [Stream Writer](response-writer/stream-writer/main.go)
    * [Transactions](response-writer/transactions/main.go)
    * [SSE](response-writer/sse/main.go)
    * [SSE (third-party package usage for server sent events)](response-writer/sse-third-party/main.go)
    * Cache
        * [Simple](response-writer/cache/simple/main.go)
        * [Client-Side (304)](response-writer/cache/client-side/main.go)
* Compression
    * [Server-Side](compression/main.go)
    * [Client-Side](compression/client/main.go)
    * [Client-Side (using Iris)](compress/client-using-iris/main.go)
* Localization and Internationalization
    * [i18n](i18n)
    * [i18n templates and functions](i18n/i18n-template)
* Authentication, Authorization & Bot Detection 
    * [Basic Authentication](auth/basicauth/main.go)
    * [CORS](auth/cors)
    * [JWT](auth/jwt/main.go)
    * [JWT (community edition)](https://github.com/iris-contrib/middleware/tree/v12/jwt/_example/main.go)
    * [OAUth2](auth/goth/main.go)
    * [Manage Permissions](auth/permissions/main.go)
    * [Google reCAPTCHA](auth/recaptcha/main.go)
    * [hCaptcha](auth/hcaptcha/main.go)
* Cookies
    * [Basic](cookies/basic/main.go)
    * [Options](cookies/options/main.go)
    * [Encode/Decode (with `securecookie`)](cookies/securecookie/main.go)
* Sessions
    * [Overview: Config](sessions/overview/main.go)
        * [Overview: Routes](sessions/overview/example/example.go)
    * [Basic](sessions/basic/main.go)
    * [Secure Cookie](sessions/securecookie/main.go)
    * [Flash Messages](sessions/flash-messages/main.go)
    * [Databases](sessions/database)
        * [Badger](sessions/database/badger/main.go)
        * [BoltDB](sessions/database/boltdb/main.go)
        * [Redis](sessions/database/redis/main.go)
* Websocket
    * [Gorilla FileWatch (3rd-party)](websocket/gorilla-filewatch/main.go)
    * [Basic](websocket/basic)
        * [Server](websocket/basic/server.go)
        * [Go Client](websocket/basic/go-client/client.go)
        * [Browser Client](websocket/basic/browser/index.html)
        * [Browser NPM Client (browserify)](websocket/basic/browserify/app.js)
    * [Native Messages](websocket/native-messages/main.go)
    * [TLS](websocket/secure/README.md)
    * [Online Visitors](websocket/online-visitors/main.go)
* Dependency Injection
    * [Overview (Movies Service)](ependency-injection/overview/main.go)
    * [Basic](dependency-injection/basic/main.go)
        * [Middleware](dependency-injection/basic/middleware/main.go)
    * [Sessions](dependency-injection/sessions/main.go)
    * [Smart Contract](dependency-injection/smart-contract/main.go)
    * [JWT](dependency-injection/jwt/main.go)
        * [JWT (iris-contrib)](dependency-injection/jwt/contrib/main.go)
    * [Register Dependency from Context](dependency-injection/context-register-dependency/main.go)
* MVC
    * [Overview](mvc/overview)
    * [Repository and Service layers](mvc/repository)
    * [Hello world](mvc/hello-world/main.go)
    * [Basic](mvc/basic/main.go)
        * [Wildcard](mvc/basic/wildcard/main.go)
    * [Singleton](mvc/singleton)
    * [Regexp](mvc/regexp/main.go)
    * [Session Controller](mvc/session-controller/main.go)
    * [Authenticated Controller](mvc/authenticated-controller/main.go)
    * [Versioned Controller](mvc/versioned-controller/main.go)
    * [Websocket Controller](mvc/websocket)
    * [Register Middleware](mvc/middleware)
    * [gRPC](mvc/grpc-compatible)
    * [Login (Repository and Service layers)](mvc/login)
    * [Login (Single Responsibility)](mvc/login-mvc-single-responsibility)
    * [Vue.js Todo App](mvc/vuejs-todo-mvc)
    * [HTTP Error Handler](mvc/error-handler-http)
    * [Error Handler](mvc/error-handler)
    * [Handle errors using mvc.Result](mvc/error-handler-custom-result)
    * [Handle errors using PreflightResult](mvc/error-handler-preflight)
    * [Handle errors by hijacking the result](mvc/error-handler-hijack)
* [Bootstrapper](bootstrapper)
* Desktop Applications
    * [The blink package](desktop/blink)
    * [The lorca package](desktop/lorca)
    * [The webview package](desktop/webview)
* Middlewares [(Community)](https://github.com/iris-contrib/middleware)

## Run

1. Install the Go Programming Language, version 1.15+ from [here](https://golang.org/dl).
2. Install Iris: `go get -u github.com/kataras/iris/v12@v12.2.0-alpha`
3. [Download the examples](https://github.com/iris-contrib/examples/archive/master.zip) and copy-paste them to your `$GOPATH/src/github.com/iris-contrib/examples`

And run

```sh
$ cd $GOPATH/src/github.com/iris-contrib/examples/compression
$ go run main.go
```

Do not forget to [star or watch the Iris project](https://github.com/kataras/iris/stargazers).

## Any troubles with examples?

    https://github.com/iris-contrib/examples/issues

## Su, 04 June 2017

This repository is just a mirror of the https://github.com/kataras/iris/master/_examples folder.
