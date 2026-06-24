## What changes

<!-- Briefly: the gist of the change and why it's needed. -->

## Type of change

- [ ] Bug fix
- [ ] New feature
- [ ] Refactoring / internal
- [ ] Documentation

## Checklist

- [ ] `pnpm build && pnpm typecheck && pnpm test` — green
- [ ] When touching the registry/templates: `pnpm typecheck:registry` / `pnpm typecheck:templates`
- [ ] `pnpm lint` green; `pnpm schemas` with no drift (`git diff --exit-code schemas`)
- [ ] A **changeset** added (`pnpm changeset`) if a published package changed
- [ ] Contracts changed **additively** only (or this is a deliberate major)
