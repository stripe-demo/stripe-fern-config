# Stripe Demo Fern Configuration

This repository contains the Stripe Demo Fern configuration: 
  - [OpenAPI](./openapi.yaml)
  - [Generators configuration](./generators.yml)

## Validating your API Definition

To validate the API, run: 
```bash
npm install -g fern-api # only required once
fern check
```

## Updating your Docs

View your generated documentation website at [stripe.docs.buildwithfern.com](https://stripe.docs.buildwithfern.com).

### Local Development server

To run a local development server with hot-reloading you can run the following command

```bash
fern docs dev
```

### Hosted URL

Documentation is automatically updated when you push to main via the `fern generate` command

```bash
npm install -g fern-api # only required once
fern generate --docs
```

## Generate the TypeScript SDK

To update the TypeScript SDK, simply run the `Release Node.js SDK` GitHub Action with the desired version for the release. Under the hood, this leverages the Fern CLI: 

```sh
fern generate --group node-sdk
```
