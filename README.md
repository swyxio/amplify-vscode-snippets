![image](https://user-images.githubusercontent.com/6764957/88305633-4eae5080-cd3c-11ea-88a5-49c61030fe99.png)

This is an unofficial snippets extension for [AWS Amplify](https://docs.amplify.aws/cli) users. Speed up your development by scaffolding out commonly used code snippets for [Amplify CSS](https://blog.kylegalbraith.com/2020/03/31/customizing-the-aws-amplify-authentication-ui-with-your-own-react-components/), [UI Components](https://docs.amplify.aws/ui/), [API](https://docs.amplify.aws/guides/api-graphql/)/[DataStore](https://docs.amplify.aws/lib/datastore/) calls, and [GraphQL Transform](https://docs.amplify.aws/cli/graphql-transformer/overview)/) directives.

> :warning: this is unofficial and has no promise of maintenance! on the plus side, it's very simple. pls feel free to fork and customize your own!

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
