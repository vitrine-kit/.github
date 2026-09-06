# Vitrine Kit

**Agency tooling for client catalogs and stores.** Scaffold one repository per client, install whole-store features from a copy-in registry, ship shared runtime as versioned packages, and apply each client’s look with an AI design step — held together by five stable contracts.

**[Website](https://vitrine-kit.github.io/vitrine/)** ·
**[Developer wiki](https://vitrine-kit.github.io/vitrine/developers/)** ·
**[npm](https://www.npmjs.com/org/vitrine-kit)** ·
**[vitrine](https://github.com/vitrine-kit/vitrine)**

[![npm](https://img.shields.io/npm/v/@vitrine-kit/vitrine?label=%40vitrine-kit%2Fvitrine)](https://www.npmjs.com/package/@vitrine-kit/vitrine)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/vitrine-kit/vitrine/blob/main/LICENSE)

**Status:** published on public npm · MIT · Node 20 + pnpm

## What you get

- **Copy-in features** — install catalog, product page, cart, checkout, and more into the client repo (shadcn/ui-style), not opaque npm UI blobs
- **Five stable contracts** — Tokens · Data · Slots · Config · Blueprint keep features portable across backends
- **Safe updates** — three-way merge with pristine originals; `vitrine doctor` checks lock, files, and env
- **Design without forking behavior** — AI design steps rewrite token values only; structure and data stay intact
- **Public npm, offline-ready CLI** — no PAT for clients; kit cache under `~/.vitrine` works offline
- **Agent-ready repos** — generated `CLAUDE.md`, slash commands, and a CLI surface AI agents can drive

## Quick start

```bash
npm i -g @vitrine-kit/vitrine
vitrine init my-shop
cd my-shop
pnpm install && pnpm dev
```

More detail on the **[website](https://vitrine-kit.github.io/vitrine/)** and in the **[developer wiki](https://vitrine-kit.github.io/vitrine/developers/)**.

## Pick a tier

- **Catalog** — browse, search, and product pages without a cart
- **Simple store** — cart, checkout, accounts, and payments (Stripe / Paddle / YooKassa) on Payload
- **Full store** — Vendure-backed commerce for richer operational needs

## Repository

- [**vitrine**](https://github.com/vitrine-kit/vitrine) — monorepo: contracts, core, CLI, copy-in feature registry, and client templates

## Contributing & security

Where to ask, file bugs, or report vulnerabilities:
[SUPPORT.md](https://github.com/vitrine-kit/.github/blob/main/SUPPORT.md).
Setup and PR conventions:
[CONTRIBUTING.md](https://github.com/vitrine-kit/.github/blob/main/CONTRIBUTING.md).
Security reports are private only —
[SECURITY.md](https://github.com/vitrine-kit/.github/blob/main/SECURITY.md).

## License

[MIT](https://github.com/vitrine-kit/vitrine/blob/main/LICENSE).
