# Vitrine Kit

**An agentic starter kit for online stores and catalogs.** A feature registry in the
shadcn/ui style (copy-in), but for **whole store features**, behind five stable contracts
(**Tokens · Data · Slots · Config · Blueprint**). One client = one repository; the unique
design is applied by an AI step.

## Two delivery channels

- **npm packages** [`@vitrine-kit/*`](https://www.npmjs.com/org/vitrine-kit) (semver, public npm) —
  `contracts`, `core`, `payload-blueprint` and the `vitrine` CLI. This is where the critical logic
  lives: a bug = an incident for every client at once (contracts, payment, order).
- **copy-in feature registry** — catalog, product page, cart, checkout
  (Stripe / Paddle / YooKassa), SEO. Features are copied into the client's repository (like shadcn/ui) —
  the client owns the code and styles it with tokens, without changing the logic.

## Quick start

```bash
npm i -g @vitrine-kit/vitrine
vitrine init my-shop
```

Then — via an AI agent: the created repository has a `CLAUDE.md` and Claude Code slash commands
(`/setup`, `/design`, `/add-feature`, `/update`, `/doctor`).

## Repositories

- [**vitrine**](https://github.com/vitrine-kit/vitrine) — the monorepo: contracts, core,
  payload-blueprint, the CLI, the copy-in feature registry and the client repository templates.

## License

[MIT](https://github.com/vitrine-kit/vitrine/blob/main/LICENSE).
