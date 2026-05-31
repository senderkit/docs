# SenderKit Docs

This repository contains Mintlify documentation for SenderKit.
The product source code lives in a sibling repo, mounted via `--add-dir ../`.

## Source-of-truth locations
- SDK source: `../senderkit-sdk/packages/sdk/src/`
- CLI commands: `../senderkit-sdk/packages/cli/src/core/commands/`
- MCP server (bundled in the CLI): `../senderkit-sdk/packages/cli/src/mcp/`
- MCP server (hosted by the app, served at `/mcp`): `../senderkit-app/lib/mcp/`
- Main Next.js app: `../senderkit-app/` (routes in `app/`, server logic in `lib/`)
- OpenAPI spec: `../senderkit-app/public/openapi.yaml` (served at `https://senderkit.com/openapi.yaml`; there is no `openapi.yaml` at the app root)
- Product positioning: `../senderkit-app/README.md`

Note: there is no `@senderkit/react-email` doc coverage and no `packages/mcp`
package — MCP is bundled in the CLI and hosted by the app.

## Conventions
- Use Mintlify components (`<CodeGroup>`, `<ParamField>`, `<ResponseField>`, `<Steps>`, `<Card>`, `<Tabs>`) over plain Markdown where structure helps.
- Never paraphrase function signatures or CLI flags from memory — always read them from source.
- `docs.json` is the navigation config (not the old `mint.json`).
