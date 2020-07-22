# amplify-vscode-snippets 

this is an unofficial snippets extension for AWS amplify.

## Install

You can add this by searching `Amplify Snippets` in your VS Code Extensions.

Direct link here: https://marketplace.visualstudio.com/items?itemName=sw-yx.amplify-vscode-snippets

## Snippets Included


### TypeScript/JavaScript

|     Prefix | Method                                                  |
| ---------: | ------------------------------------------------------- |
| `import amplify→` | `import Amplify from 'aws-amplify';import awsconfig from './aws-exports';Amplify.configure(awsconfig);`        |
| `Authenticator→` | `import { withAuthenticator,AmplifySignOut } from \"@aws-amplify/ui-react\"` |
| `DataStore import→` | `import { DataStore } from '@aws-amplify/datastore'` etc |
| `DataStore Read/Create/Update/Delete→` | relevant sample code |




### CSS

|     Prefix | Method                                                  |
| ---------: | ------------------------------------------------------- |
| `Amplify :root→` | `--amplify-primary-color/tint/shade`        |



### GraphQL

|     Prefix | Method                                                  |
| ---------: | ------------------------------------------------------- |
| `@auth public read→` | `@auth(rules: [{ allow: owner, queries: null }])`        |
| `@auth everything private→` | `@auth(rules: [{ allow: owner }])`        |
| `basic @model with no auth→` | `type Todo @model { /* etc */ }`        |


<!--
## Requirements

If you have any requirements or dependencies, add a section describing those and how to install and configure them.

## Extension Settings

Include if your extension adds any VS Code settings through the `contributes.configuration` extension point.

For example:

This extension contributes the following settings:

* `myExtension.enable`: enable/disable this extension
* `myExtension.thing`: set to `blah` to do something
-->


## Known Issues

this is not an official extension! it is just a helper for swyx

## Publishing

- `vsce publish minor`
- https://code.visualstudio.com/api/working-with-extensions/publishing-extension