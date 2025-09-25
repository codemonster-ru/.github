# Naming Guide

This document describes the naming conventions for Codemonster packages to ensure consistency and clarity within the ecosystem.

## 1. General Rules
- Vendor is always `codemonster-ru` (in both Composer and NPM).
- Package names should be short and descriptive (`config`, `router`, `support`, `view`).
- If a package is implemented in multiple languages, the same name is used within each ecosystem.

## 2. PHP packages
- **Composer**: `codemonster-ru/<name>`
- **GitHub**: `codemonster-ru/<name>-php`
- **Namespace**: `Codemonster\<PackageName>`

📌 Example:
- `composer require codemonster-ru/config`
- GitHub: `github.com/codemonster-ru/config-php`
- Namespace: `Codemonster\Config`

## 3. JS/TS packages
- **NPM**: `@codemonster-ru/<name>`
- **GitHub**: `codemonster-ru/<name>-js`
- **package.json → name**: `@codemonster-ru/<name>`

📌 Example:
- `npm install @codemonster-ru/config`
- GitHub: `github.com/codemonster-ru/config-js`

## 4. Multilingual Packages
If a package exists for both PHP and JS:
- Composer and NPM packages have the same name (`config`).
- GitHub repositories are distinguished by a postfix (`-php` / `-js`).
- A link to the other implementation is required in the README.

📌 Example:
```
PHP → composer require codemonster-ru/env
JS → npm install @codemonster-ru/env
GitHub: codemonster-ru/env-php
GitHub: codemonster-ru/env-js
```

## 5. Annabel framework
- **Core**: `codemonster-ru/annabel` (PHP)
- **Skeleton**: `codemonster-ru/annabel-skeleton`
- **SSR Bridge**: `codemonster-ru/ssr-bridge` (PHP)
- **SSR Service**: `@codemonster-ru/ssr-service` (Node.js)

## 6. Final table

| Destination | Composer | NPM | GitHub repo |
|--------------|--------------------------|----------------------------|----------------------------|
| Framework | codemonster-ru/annabel | — | annabel |
| Skeleton | codemonster-ru/annabel-skeleton | — | annabel-skeleton |
| SSR Bridge | codemonster-ru/ssr-bridge | — | ssr-bridge |
| SSR Service | — | @codemonster-ru/ssr-service | ssr-service |
| Env (PHP) | codemonster-ru/env | — | env-php |
| Env (JS) | — | @codemonster-ru/env | env-js |
| Config | codemonster-ru/config | — | config-php |
| Support | codemonster-ru/support | — | support-php |
| Router | codemonster-ru/router | — | router-php |
| View | codemonster-ru/view | — | view-php |
