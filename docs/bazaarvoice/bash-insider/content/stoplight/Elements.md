# Elements

Elements is an API Documentation toolkit, leveraging OpenAPI and Markdown (CommonMark) to provide beautiful, interactive API reference documentation, that you can integrate with any existing content-management system or single-page application.

Elements is made by Stoplight, which offers hosted documentation, visual API design tools, and all sorts of other handy API tooling, but you do not need a Stoplight account to use Elements.

How you chose to work with Elements depends on what you are trying to do.

- **Web Component** - Integrate with any Content Management System or create a simple HTML rendering of your API documentation.
- **Command Line Interface** - Coming soon! Quickly get up and running, see how your API documentation could look with little effort.

## Integrations
Learn how to integrate Elements with any of these popular frameworks.

- AngularJS
- ReactJS
- NextJS
- GatsbyJS

## Elements vs Elements Dev Portal
The concept of Elements is to be a collection of components that can be useful for building out API documentation, and those components are split across two different packages:

- [@stoplight/elements] - We generally just call this "Elements", and is home to the "API Component".
- [@stoplight/elements-dev-portal] - This collection of components is referred to as Elements Dev Portal, and contains the "Stoplight Project" component and the "Search" component.
All of these components are available as Web Components or React components, so you can use them pretty much anywhere.

If you have one single API with a single OpenAPI document that needs turning into API Reference Documentation, you want the "API Component", and it can be used with any OpenAPI definition via a URL or JavaScript object.

Elements Dev Portal is like an extension, a superset of Elements functionality, that contain multiple APIs and Markdown Articles presented together. This allows for adding generic tutorials and guides along with the API reference documentation, and requires a Stoplight Project to power it all, along with mocking and some other advanced functionality not available in the standalone Elements package.

## Free Hosted Docs
If you don’t want to host your own documentation, and don’t need to embed the docs into an existing site, consider using Stoplight Documentation, which is basically hosted Elements.

The free plan will get you a long way, and there's no need to figure out deployments. If your API description documents are in a Git repo, connect that to Stoplight and it will render your documentation for you whenever commits are pushed or merged.