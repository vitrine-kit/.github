# Vitrine Kit

**Агентский стартер-кит для интернет-магазинов и каталогов.** Реестр фич в стиле
shadcn/ui (copy-in), но для **целых фич магазина**, за пятью стабильными контрактами
(**Tokens · Data · Slots · Config · Blueprint**). Один клиент = один репозиторий; уникальный
дизайн применяется ИИ-шагом.

## Два канала доставки

- **npm-пакеты** [`@vitrine-kit/*`](https://www.npmjs.com/org/vitrine-kit) (semver, публичный npm) —
  `contracts`, `core`, `payload-blueprint` и CLI `vitrine`. Сюда кладут критлогику: баг = инцидент
  у всех клиентов сразу (контракты, платёж, заказ).
- **copy-in реестр фич** — каталог, страница товара, корзина, checkout
  (Stripe / Paddle / YooKassa), SEO. Фичи копируются в репозиторий клиента (как shadcn/ui) —
  клиент владеет кодом и стилизует его токенами, не меняя логику.

## Быстрый старт

```bash
npm i -g @vitrine-kit/vitrine
vitrine init my-shop
```

Дальше — через ИИ-агента: в созданном репозитории есть `CLAUDE.md` и слэш-команды Claude Code
(`/setup`, `/design`, `/add-feature`, `/update`, `/doctor`).

## Репозитории

- [**vitrine**](https://github.com/vitrine-kit/vitrine) — монорепо: контракты, core,
  payload-blueprint, CLI, copy-in реестр фич и шаблоны клиентского репозитория.

## Лицензия

[MIT](https://github.com/vitrine-kit/vitrine/blob/main/LICENSE).
