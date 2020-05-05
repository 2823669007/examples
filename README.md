# Examples

<a href="https://iris-go.com"> <img align="right" width="115px" src="https://iris-go.com/images/icon.svg?v=a" title="logo created by @merry.dii" /> </a>

<a href="https://travis-ci.org/kataras/iris"><img src="https://img.shields.io/travis/kataras/iris.svg?style=flat-square" alt="Build Status"></a>
<a href="https://github.com/iris-contrib/examples/blob/v12/LICENSE"><img src="https://img.shields.io/badge/%20license-MIT%20%20License%20-E91E63.svg?style=flat-square" alt="License"></a>
<a href="https://github.com/kataras/iris/blob/v12/HISTORY.md"><img src="https://img.shields.io/badge/version-v12.1%20-blue.svg?style=flat-square" alt="CHANGELOG/HISTORY"></a>

This repository provides easy to understand code snippets on how to get started with web development with the Go programming language using the [Iris](https://github.com/kataras/iris) web framework.

To read the Iris documentation please navigate to [the wiki pages](https://github.com/kataras/iris/wiki) instead.

## Table of Contents

* Tutorials
    * [Dockerize](tutorial/docker)
    * [Caddy](tutorial/caddy)
    * [MongoDB](tutorial/mongodb)
    * [Dropzone.js](tutorial/dropzonejs)
    * [URL Shortener](tutorial/url-shortener/main.go)
    * [Online Visitors](tutorial/online-visitors/main.go)
    * [REST API for Apache Kafka](tutorial/api-for-apache-kafka)
    * [Vue.js Todo (MVC)](tutorial/vuejs-todo-mvc)
    * [gRPC (MVC)](mvc/grpc-compatible)
* HTTP Listening
    * [HOST:PORT](http-listening/listen-addr/main.go)
    * [Public Test Domain](http-listening/listen-addr-public/main.go)
    * [UNIX socket file](http-listening/listen-unix/main.go)
    * [TLS](http-listening/listen-tls/main.go)
    * [Letsencrypt (Automatic Certifications)](http-listening/listen-letsencrypt/main.go)
    * [Graceful Shutdown](http-listening/graceful-shutdown/default-notifier/main.go)
    * [Notify on shutdown](http-listening/notify-on-shutdown/main.go)
    * Custom TCP Listener
        * [Common net.Listener](http-listening/custom-listener/main.go)
        * [SO_REUSEPORT for unix systems](http-listening/custom-listener/unix-reuseport/main.go)
    * Custom HTTP Server
        * [Pass a custom Server](http-listening/custom-httpserver/easy-way/main.go)
        * [Use Iris as a single http.Handler](http-listening/custom-httpserver/std-way/main.go)
        * [Multi Instances](http-listening/custom-httpserver/multi/main.go)
        * [HTTP/3 Quic](http-listening/http3-quic)
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
    * [Not Found - Suggest Closest Paths](routing/not-found-suggests/main.go)
    * [Dynamic Path](routing/dynamic-path/main.go)
        * [Root Wildcard](routing/dynamic-path/root-wildcard/main.go)
        * [Implement a Parameter Type](routing/macros/main.go)
    * Middleware
        * [Per Route](routing/writing-a-middleware/per-route/main.go)
        * [Globally](routing/writing-a-middleware/globally/main.go)
        * [Route Register Rule](routing/route-register-rule/main.go)
        * Convert net/http Handlers
            * [From func(w http.ResponseWriter, r *http.Request, next http.HandlerFunc)](convert-handlers/negroni-like/main.go)
            * [From http.Handler or http.HandlerFunc](convert-handlers/nethttp/main.go)
            * [From func(http.HandlerFunc) http.HandlerFunc](convert-handlers/real-usecase-raven/writing-middleware/main.go)
    * [Route State](routing/route-state/main.go)
    * [Reverse Routing](routing/reverse/main.go)
    * [Router Wrapper](routing/custom-wrapper/main.go)
    * [Custom Router](routing/custom-high-level-router/main.go)
    * Custom Context
        * [Method Overriding](routing/custom-context/method-overriding/main.go)
        * [New Implementation](routing/custom-context/new-implementation/main.go)
* Subdomains
    * [Single](subdomains/single/main.go)
    * [Multi](subdomains/multi/main.go)
    * [Wildcard](subdomains/wildcard/main.go)
    * [WWW](subdomains/www/main.go)
    * [Redirection](subdomains/redirect/main.go)
* API Versioning
    * [How it works](https://github.com/kataras/iris/wiki/API-versioning)
    * [Example](versioning/main.go)
* API Documentation
    * [yaag](apidoc/yaag/main.go)
* Testing
    * [Example](testing/httptest/main_test.go)
* File Server
    * [Favicon](file-server/favicon/main.go)
    * [Basic](file-server/basic/main.go)
    * [Embedding Files Into App Executable File](file-server/embedding-files-into-app/main.go)
    * [Embedding Gziped Files Into App Executable File](file-server/embedding-gziped-files-into-app/main.go)
    * [Send Files (rate limiter included)](file-server/send-files/main.go)
    * Single Page Applications
        * [Basic SPA](file-server/single-page-application/basic/main.go)
        * [Embedded Single Page Application](file-server/single-page-application/embedded-single-page-application/main.go)
        * [Embedded Single Page Application with other routes](file-server/single-page-application/embedded-single-page-application-with-other-routes/main.go)
* View
    * [Overview](view/overview/main.go)
    * [Basic](view/template_html_0/main.go)
    * [A simple Layout](view/template_html_1/main.go)
    * [Layouts: `yield` and `render` tmpl funcs](view/template_html_2/main.go)
    * [The `urlpath` tmpl func](view/template_html_3/main.go)
    * [The `url` tmpl func](view/template_html_4/main.go)
    * [Inject Data Between Handlers](view/context-view-data/main.go)
    * [Embedding Templates Into App Executable File](view/embedding-templates-into-app/main.go)
    * [Write to a custom `io.Writer`](view/write-to)
    * [Pug: Greeting](view/template_pug_0)
    * [Pug: `Actions`](view/template_pug_1)
    * [Pug: `Includes`](view/template_pug_2)
    * [Pug: `Extends`](view/template_pug_3)
    * [Jet Template](/view/template_jet_0)
    * [Jet Embedded](view/template_jet_1_embedded)
    * [Jet 'urlpath' tmpl func](/view/template_jet_2)
    * [Jet Template Funcs from Struct](/view/template_jet_3)
    * Third-Parties
        * [Render `valyala/quicktemplate` templates](http_responsewriter/quicktemplate)
        * [Render `shiyanhui/hero` templates](http_responsewriter/herotemplate)
* Request Body
    * [Bind JSON](http_request/read-json/main.go)
    *   * [Struct Validation](http_request/read-json-struct-validation/main.go)
    * [Bind XML](http_request/read-xml/main.go)
    * [Bind MsgPack](http_request/read-msgpack/main.go)
    * [Bind YAML](http_request/read-yaml/main.go)
    * [Bind Form](http_request/read-form/main.go)
    * [Bind Query](http_request/read-query/main.go)
    * [Bind Body](http_request/read-body/main.go)
    * [Bind Custom per type](http_request/read-custom-per-type/main.go)
    * [Bind Custom via Unmarshaler](http_request/read-custom-via-unmarshaler/main.go)
    * [Bind Many times](http_request/read-many/main.go)
    * [Upload/Read File](http_request/upload-file/main.go)
    * [Upload multiple Files](http_request/upload-files/main.go)
    * [Extract Referrer](http_request/extract-referer/main.go)
* Response Writer
    * [Content Negotiation](http_responsewriter/content-negotiation)
    * [Text, Markdown, YAML, HTML, JSON, JSONP, Msgpack, XML and Binary](http_responsewriter/write-rest/main.go)
    * [Write Gzip](http_responsewriter/write-gzip/main.go)
    * [Stream Writer](http_responsewriter/stream-writer/main.go)
    * [Transactions](http_responsewriter/transactions/main.go)
    * [SSE](http_responsewriter/sse/main.go)
    * [SSE (third-party package usage for server sent events)](http_responsewriter/sse-third-party/main.go)
    * [Webassembly](webassembly/basic/main.go)
* Cache
    * [Simple](cache/simple/main.go)
    * [Client-Side (304)](cache/client-side/main.go)
* Localization and Internationalization
    * [i18n](i18n/main.go)
* Sitemaps
    * [Sitemap](sitemap/main.go)
* Authentication
    * [Basic Authentication](authentication/basicauth/main.go)
    * [OAUth2](authentication/oauth2/main.go)
    * [Request Auth(JWT)](experimental-handlers/jwt/main.go)
    * [Manage Permissions](permissions/main.go)
* Cookies
    * [Basic](cookies/basic/main.go)
    * [Encode/Decode (with `securecookie`)](cookies/securecookie/main.go)
* Sessions
    * [Overview](sessions/overview/main.go)
    * [Middleware](sessions/middleware/main.go)
    * [Secure Cookie](sessions/securecookie/main.go)
    * [Flash Messages](sessions/flash-messages/main.go)
    * [Databases](sessions/database)
        * [Badger](sessions/database/badger/main.go)
        * [BoltDB](sessions/database/boltdb/main.go)
        * [Redis](sessions/database/redis/main.go)
* Websocket
    * [Basic](websocket/basic)
        * [Server](websocket/basic/server.go)
        * [Go Client](websocket/basic/go-client/client.go)
        * [Browser Client](websocket/basic/browser/index.html)
        * [Browser NPM Client (browserify)](websocket/basic/browserify/app.js)
    * [Native Messages](websocket/native-messages/main.go)
    * [TLS](websocket/secure/README.md)
* Dependency Injection
    * [Overview (Movies Service)](ependency-injection/overview/main.go)
    * [Basic](dependency-injection/basic/main.go)
        * [Middleware](dependency-injection/basic/middleware/main.go)
    * [Sessions](dependency-injection/sessions/main.go)
    * [Smart Contract](dependency-injection/smart-contract/main.go)
* MVC
    * [Overview - Repository and Service layers](mvc/overview)
    * [Login - Repository and Service layers](mvc/login)
    * [Hello world](mvc/hello-world/main.go)
    * [Basic](mvc/basic/main.go)
        * [Wildcard](mvc/basic/wildcard/main.go)
    * [Singleton](mvc/singleton)
    * [Regexp](mvc/regexp/main.go)
    * [Session Controller](mvc/session-controller/main.go)
    * [Websocket Controller](mvc/websocket)
    * [Register Middleware](mvc/middleware)
* Object-Relational Mapping
    * [Using `go-xorm/xorm` (Mysql, MyMysql, Postgres, Tidb, SQLite, MsSql, MsSql, Oracle)](orm/xorm/main.go)
    * [Using `jinzhu/gorm`](orm/gorm/main.go)
* Project Structure
    * [Bootstrapper](structuring/bootstrap)
    * [MVC with Repository and Service layer Overview](structuring/mvc-plus-repository-and-service-layers)
    * [Login (MVC with Single Responsibility package)](structuring/login-mvc-single-responsibility-package)
    * [Login (MVC with Datamodels, Datasource, Repository and Service layer)](structuring/login-mvc)
* Desktop Applications
    * [The blink package](desktop-app/blink)
    * [The lorca package](desktop-app/lorca)
    * [The webview package](desktop-app/webview)
* Middlewares (Builtin)
    * [Rate Limit](miscellaneous/ratelimit/main.go)
    * [HTTP Method Override](https://github.com/kataras/iris/blob/master/middleware/methodoverride/methodoverride_test.go)
    * [Request Logger](http_request/request-logger/main.go)
        * [Log Requests to a File](http_request/request-logger/request-logger-file/main.go)
    * [Recovery](miscellaneous/recover/main.go)
    * [Profiling (pprof)](miscellaneous/pprof/main.go)
    * [Internal Application File Logger](miscellaneous/file-logger/main.go)
    * [Google reCAPTCHA](miscellaneous/recaptcha/main.go)
    * [hCaptcha](miscellaneous/hcaptcha/main.go)
* Middlewares [(Community)](https://github.com/iris-contrib/middleware)

> Examples are tested using Windows 10, Ubuntu 16.10 with [Microsoft's Visual Studio Code](https://code.visualstudio.com/) and built using the [Go 1.14.2](https://golang.org/dl).

## Run

1. Install the Go Programming Language, version 1.14 from [here](https://golang.org/dl).
2. Install Iris: `go get github.com/kataras/iris/v12@latest`
3. [Download the examples](https://github.com/iris-contrib/examples/archive/v12.zip) and copy-paste them to your `$GOPATH/src/github.com/iris-contrib/examples`

And run

```sh
$ cd $GOPATH/src/github.com/iris-contrib/examples/overview
$ go run main.go
```

Do not forget to [star or watch the Iris project](https://github.com/kataras/iris/stargazers).

## Any troubles with examples?

    https://github.com/iris-contrib/examples/issues

## Su, 04 June 2017

This repository is just a mirror of the https://github.com/kataras/iris/master/_examples folder.
