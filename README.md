# openapi

This is a work-in-progress OpenAPI 3 spec to be built with Redoc and hosted on GitHub Pages. Currently only showcases implemented endpoints and expected responses.

This could be used as an alternative to the `mkdocs` repo https://github.com/predecessor-api/docs

### Install Redocly

```
npm install @redocly/cli -g
```

### Build

```
redocly build-docs openapi/openapi.yaml -o index.html
```

```
npm run build
```

### Generate types/clients

Can generate types and clients for various programming languages, this might be a bit excessive...

https://openapi-generator.tech/docs/installation/

Prerequisites to install:

- npm
- java

```
openapi-generator-cli generate -i dist.yaml -g go -o golang
```

```
openapi-generator-cli generate -i dist.yaml -g typescript -o typescript
```
