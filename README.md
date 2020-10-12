# Serverless Offline Step Functions

Serverless Offline Plugin to Support Step Functions for Local Development.

**Features**:

- Fully Written in TypeScript
- Promise based (no process spawn)

## Sponsor

If the plugin is being useful to your company and want to keep the development active, consider buying me a coffee 🙂... coffee is the thing that makes me the most happy person in the world and I'd appreciate the sponsorship.

[![ko-fi](https://www.ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/Y8Y42C4E9)

## Requirements

- [serverless-step-functions plugin](https://github.com/serverless-operations/)

## Installation

```shell
$ npm i -D @fernthedev/serverless-offline-step-functions

# or

$ yarn add -D @fernthedev/serverless-offline-step-functions
```

## Using it with Webpack

If your project uses `serverless-webpack` to compile/transpile your serverless application. **Make sure is defined in your plugins before this plugin and `serverless-offline`**

### Example

```yml
plugins:
  - serverless-webpack # Defined Before
  - serverless-step-functions
  - '@fernthedev/serverless-offline-step-functions'
  - serverless-offline
```

## State Types Supported

| States | Notes |
| ------ | ------ |
| ***Task*** | `Retry/Catch`, `Timeout` and `Heartbeat` are not supported yet. |
| ***Choice*** | ✅ |
| ***Wait***  | ✅ |
| ***Parallel*** | Not Supported at all yet. |
| ***Pass*** | ✅ |
| ***Fail***| ✅ |
| ***Succeed***|✅|

## Credits and inspiration

The plugin began as a fork of [flocasts/serverless-offline-step-functions](https://github.com/flocasts/serverless-offline-step-functions) for a fix. Then I decided to do a full rewrite of it 😀

## License

[MIT](./LICENSE)

## How to Contribute

Thank you for your interest on contributing. There's a tons of ways that you can contribute!

- If you see that something is not right, open an issue!
- If you know exactly what is happening, open a PR!
- Want to improve the docs? Open a PR!
- Want to improve the code? Open a PR!

Please follow both PR and Issues template for contribution. **Any Open Issue/PR that does not follow the templates will be closed**
