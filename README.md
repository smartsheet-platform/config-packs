## Config-Pack for the Smartsheet MCP Server

**config-packs** is the development and distribution repo for Smartsheet `config-rocket` ecosystem config packs.

## Available config packs:

+ [`Smartsheet MCP`](./src/assembly/roo-rocket/smartsheet/)
  + A Roo Code config-pack for a Smartsheet Model Context Protocol (MCP) server for interacting with the Smartsheet API.

## Deployment
### Bundle the config-pack

```bash
pnpm run bundle
```

### Generate Binary Hash
```bash
openssl dgst -sha256 -binary binary/smartsheet-mcp.zip | openssl base64 | tr '+/' '-_' | tr -d '='
```
