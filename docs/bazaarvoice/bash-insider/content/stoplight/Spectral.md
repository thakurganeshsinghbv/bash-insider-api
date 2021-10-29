# Spectral

- **Custom Rulesets**: Create custom rules to lint JSON or YAML objects
- **Ready-to-use Rulesets**: Validate and lint OpenAPI v2 & v3 and AsyncAPI Documents
- **JSON Path Support**: Use JSON path to apply rules to specific parts of your objects
- **Ready-to-use Functions**: Built-in set of functions to help create custom rules. Functions include pattern checks, parameter checks, alphabetical ordering, a specified number of characters, provided keys are present in an object, etc.
- **Custom Functions**: Create custom functions for advanced use cases
- **JSON Validation**: Validate JSON with Ajv

## Overview
- Installation and Usage
- Documentation
- Support
- FAQs

### 🧰 Installation and Usage
#### Install

```json
npm install -g @stoplight/spectral-cli

# OR

yarn global add @stoplight/spectral-cli

```
#### Create a Ruleset

Spectral, being a generic YAML/JSON linter, needs a ruleset in order to be able to lint files. You can learn more about the rulesets here.

If you intend to lint an OpenAPI or AsyncAPI document, we have a few predefined rulesets you can extend to get Spectral up and running. To reference them, you can run the following command:

```json
echo '{\n\t"extends": ["spectral:oas", "spectral:asyncapi"]\n}' > .spectral.json

```

#### Lint

```json
spectral lint petstore.yaml

```