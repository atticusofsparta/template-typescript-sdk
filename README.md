# Template Usage/setup
For convenience, the following variables have been placed to setup files with your repository. You can find and replace them with your own values

- <ORGANIZATION_NAME>
- <SDK_NAME>
- <SDK_SHORT_DESCRIPTION>
- <REPOSITORY_URL>
- <NPM_PACKAGE_NAME>

The [build](./.github/workflows/build.yml) and [release](./.github/workflows/release.yml) actions expect your github secrets to be configured with:
- `secrets.SLACK_WEBHOOK`
- `secrets.CODECOV_TOKEN`
- `secrets.CI_GITHUB_TOKEN`
- `secrets.npm_token`

Be sure to setup your codecov badge at the top of this readme to show off your testing awesomeness! (or lack thereof)

# <NPM_PACKAGE_NAME>

[setup codecov](https://docs.codecov.com/docs/github-tutorial)

This is the home of [<SDK_NAME>] SDK. This SDK provides functionality for [<SDK_SHORT_DESCRIPTION>] available for both NodeJS and Web environments.

## Table of Contents

- [Installation](#installation)
- [Quick Start](#quick-start)
- [Usage](#usage)
  - [NodeJS Environments](#node)
  - [Web Environments](#web)
  - [Typescript](#typescript)
- [APIs](#apis)
- [Examples](./examples)
- [Developers](#developers)
  - [Requirements](#requirements)
  - [Setup & Build](#setup--build)
  - [Testing](#testing)
  - [Linting and Formatting](#linting--formatting)
  - [Architecture](#architecture)
- [Contributing](./CONTRIBUTING.md)

## Installation

```shell
npm install <NPM_PACKAGE_NAME>
```

or

```shell
yarn add <NPM_PACKAGE_NAME>
```

## Quick Start

```typescript
// INSERT A SHORT EXAMPLE OF HOW TO SETUP AND USE THE SDK
```

## Usage

The SDK is provided in both CommonJS and ESM formats, and it's compatible with bundlers such as Webpack, Rollup, and ESbuild. Utilize the appropriately named exports provided by this SDK's [package.json] based on your project's configuration. Refer to the [examples] directory to see how to use the SDK in various environments.

### Web

#### Bundlers (Webpack, Rollup, ESbuild, etc.)

```javascript
// INSERT EXAMPLE FOR USING IN ESM PROJECT
```

#### Browser

```javascript
// INSERT EXAMPLE FOR USING IN BROWSER PROJECT
```

### Node

```javascript
// INSERT EXAMPLE FOR USING IN CJS PROJECT
```

### Typescript

The SDK provides TypeScript types. When you import the SDK in a TypeScript project:

Types are exported from `./lib/types/[node/web]/index.d.ts` and should be automatically recognized, offering benefits such as type-checking and autocompletion.

## APIs

[INSERT A LIST OF ALL THE APIS PROVIDED BY THE SDK AND HOW TO USE THEM]

## Developers

### Requirements

- `nvm`
- `node` (>= 20)
- `yarn`

### Setup & Build

- `yarn install` - installs dependencies
- `yarn build` - builds web/node/bundled outputs

### Testing

- `yarn test` - runs integration tests
- `yarn example:web` - opens up the example web page
- `yarn example:cjs` - runs example CJS node script
- `yarn example:esm` - runs example ESM node script

### Linting & Formatting

- `yarn lint:check` - checks for linting errors
- `yarn lint:fix` - fixes linting errors
- `yarn format:check` - checks for formatting errors
- `yarn format:fix` - fixes formatting errors

### Architecture

- Code to interfaces.
- Prefer type safety over runtime safety.
- Prefer composition over inheritance.
- Prefer integration tests over unit tests.

For more information on how to contribute, please see [CONTRIBUTING.md].

### CI/CD

The [build](./.github/workflows/build.yml) and [release](./.github/workflows/release.yml) actions expect your:
- `secrets.SLACK_WEBHOOK`
- `secrets.CODECOV_TOKEN`
- `secrets.CI_GITHUB_TOKEN`
- `secrets.npm_token`

Be sure to setup your codecov badge at the top of this readme to show off your testing awesomeness! (or lack thereof)

<!-- ADD ALL LINK REFERENCES BELOW -->

[ar.io]: https://ar.io
[package.json]: ./package.json
[examples]: ./examples
[examples/webpack]: ./examples/webpack
[examples/vite]: ./examples/vite
[CONTRIBUTING.md]: ./CONTRIBUTING.md