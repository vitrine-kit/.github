# Contributing to Vitrine Kit

Thanks for your interest! These rules apply to the [@vitrine-kit](https://github.com/vitrine-kit) repositories.

## Environment

- **Node 20 LTS** + **pnpm** (`corepack enable`).
- `pnpm install` at the monorepo root. The `@vitrine-kit/*` packages are public — no token needed.

## Before a PR — a green gate

```bash
pnpm build && pnpm typecheck && pnpm test
# if you touched the registry/templates:
pnpm typecheck:registry && pnpm typecheck:templates
pnpm lint
pnpm schemas   # and make sure there's no drift: git diff --exit-code schemas
```

## Conventions

- **The contracts (`@vitrine-kit/contracts`) are extended additively only** (semver). Changing the shape
  of existing fields is a breaking change (major) and a deliberate decision.
- **Where to put code:** in the packages — what makes a bug an incident for everyone (contract, payment, order);
  in the registry — what varies per client (look, sections).
- A new registry feature depends **only on the contracts** (checked by the import-boundary test).
- **The language of the code and documentation is English** (comments, messages, docs); match the existing style
  and comment density.
- **The biome formatter is off** — keep the existing style by hand, keep lint green.

## Versions and publishing

Any change to a published package comes with a changeset:

```bash
pnpm changeset
```

Version bumps and publishing to npm are automated by CI on merge to `main`. Do not run `version` /
`publish` by hand.

## Pull requests

- Branch from `main`; a PR with the template filled in (including the "changeset added" item).
- The PR must pass CI (build / typecheck / test / lint / schemas).
