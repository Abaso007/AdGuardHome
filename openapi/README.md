# AdGuard Home OpenAPI

We are using [OpenAPI specification](https://swagger.io/docs/specification/about/) to generate AdGuard Home API specification.

## How to edit the API spec

The easiest way would be to use [Swagger Editor](http://editor.swagger.io/) and just copy/paste the YAML file there.

## Changelog

See [`CHANGELOG.md`](CHANGELOG.md) where we keep track of all non-compatible changes that are being made.

## Authentication

If AdGuard Home’s web user is password-protected, a web client must use authentication mechanism when sending requests to server. Basic access authentication is the most simple method: a client must pass `Authorization` HTTP header along with all requests:

```http
Authorization: Basic BASE64_DATA
```

Where `BASE64_DATA` is base64-encoded data for `username:password` string.
