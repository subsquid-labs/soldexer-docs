# Soldexer documentation

Source content for the Soldexer documentation site, published at [docs.soldexer.dev](https://docs.soldexer.dev).

## What this is

This repository holds the Markdown (`.mdx`) pages, navigation config, and assets for the Soldexer docs. It is a [Mintlify](https://mintlify.com/docs) site: the site structure and navigation are defined in `docs.json`, and each page is an `.mdx` file.

Soldexer is a data service for accessing Solana historical and real-time data, powered by [SQD Network](https://sqd.dev/network). The documentation here covers the ways to consume Soldexer data:

- **HTTP API**: POST queries to a `/stream` endpoint and receive newline-separated JSON blocks. See `api-reference/`.
- **Pipes SDK**: a streaming indexer toolkit built from composable source, transformer, and target components. See `pipes/`.
- **Squid SDK**: an indexing framework. See `squid-sdk/`.

The Soldexer service itself lives in a separate repository: [subsquid-labs/soldexer](https://github.com/subsquid-labs/soldexer).

## Repository layout

| Path | Contents |
| --- | --- |
| `docs.json` | Mintlify site config: theme, navigation tabs, navbar, footer |
| `get-started/` | Introduction, approach comparison, FAQ |
| `pipes/` | Pipes SDK quickstart, guides, and component reference |
| `squid-sdk/` | Squid SDK intro, example, and guide |
| `api-reference/` | Solana HTTP API reference and OpenAPI spec |
| `api-reference-evm/` | EVM HTTP API reference and OpenAPI spec |
| `external-tools/` | Notes on related tools |
| `resources/` | Brand kit |
| `changelog/` | Release notes |
| `logo/`, `snippets/` | Logos and reusable content snippets |

## Editing

Pages are `.mdx` files using Mintlify components (such as `<Card>`, `<CardGroup>`, `<Tip>`, and `<Expandable>`). When adding or moving a page, update the matching entry under `navigation` in `docs.json` so it appears in the site.

## Local preview

This is a Mintlify project (no `package.json`). To preview the site locally, install the Mintlify CLI and run it from the repository root. See the [Mintlify development guide](https://mintlify.com/docs) for the current commands and Node.js version requirements.

## Links

- Site: [docs.soldexer.dev](https://docs.soldexer.dev)
- Soldexer website: [soldexer.dev](https://soldexer.dev)
- SQD documentation: [docs.sqd.dev](https://docs.sqd.dev)
