# Prism

Prism is a set of packages for API mocking and contract testing with OpenAPI v2 (formerly known as Swagger) and OpenAPI v3.x.

- **Mock Servers**: Life-like mock servers from any API Specification Document.
- **Validation Proxy**: Contract Testing for API Consumers and Developers.
- **Comprehensive API Specification Support**: OpenAPI v3.1, OpenAPI v3.0, OpenAPI v2.0 (formerly Swagger) and Postman Collections.

> Note: This branch refers to Prism 3.x, which is the current version most likely you will use. If you're looking for the 2.x version, look at the 2.x branch

## Overview
- Installation and Usage
- Documentation and Community
- Roadmap
- FAQs
- Contributing

### 🧰 Installation and Usage
#### Installation
Prism requires NodeJS >= 12 to properly work.

```json
npm install -g @stoplight/prism-cli

# OR

yarn global add @stoplight/prism-cli

```
For more installation options, see our installation documentation.

#### Mocking
Prism can help you create a fake "mock" based off an OpenAPI document, which helps people see how your API will work before you even have it built. Run it locally with the prism mock command to run your API on a HTTP server you can interact with.

```json
prism mock https://raw.githack.com/OAI/OpenAPI-Specification/master/examples/v3.0/petstore-expanded.yaml
```

Learn more about how the mock server works.

#### Validation Proxy
Prism can help you check for discrepencies between your API implementation and the OpenAPI document that describes, letting you funnel HTTP traffic through it with the prism proxy command.

```json
prism proxy examples/petstore.oas2.yaml https://petstore.swagger.io/v2
```
