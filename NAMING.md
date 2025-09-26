# Naming Guide

This document describes the naming conventions for Codemonster packages to ensure consistency and clarity within the ecosystem.

## 1. General Rules

-   Vendor is always `codemonster-ru` (in both Composer and NPM).
-   Package names should be short and descriptive (`config`, `router`, `support`, `view`).
-   If a package is implemented in multiple languages, the **first implementation gets the clean name** (`codemonster-ru/<name>`).
    -   Subsequent implementations in other languages must use a postfix (`-php`, `-js`, `-ts`, etc.) in the GitHub repository name.

## 2. PHP packages

-   **Composer**: `codemonster-ru/<name>`
-   **GitHub**:
    -   If PHP is the **first implementation** → `codemonster-ru/<name>`
    -   If the name is already taken by another language → `codemonster-ru/<name>-php`
-   **Namespace**: `Codemonster\<PackageName>`

📌 Example 1 (PHP first):

-   `composer require codemonster-ru/config`
-   GitHub: `github.com/codemonster-ru/config`
-   Namespace: `Codemonster\Config`

📌 Example 2 (JS first, then PHP):

-   JS → GitHub: `github.com/codemonster-ru/env`
-   PHP → GitHub: `github.com/codemonster-ru/env-php`
-   Composer: `codemonster-ru/env`
-   Namespace: `Codemonster\Env`

## 3. JS/TS packages

-   **NPM**: `@codemonster-ru/<name>`
-   **GitHub**:
    -   If JS/TS is the **first implementation** → `codemonster-ru/<name>`
    -   If the name is already taken by another language → `codemonster-ru/<name>-js`
-   **package.json → name**: `@codemonster-ru/<name>`

📌 Example 1 (JS first):

-   `npm install @codemonster-ru/env`
-   GitHub: `github.com/codemonster-ru/env`

📌 Example 2 (PHP first, then JS):

-   PHP → GitHub: `github.com/codemonster-ru/config`
-   JS → GitHub: `github.com/codemonster-ru/config-js`
-   NPM: `@codemonster-ru/config`

## 4. Annabel framework

-   **Core**: `codemonster-ru/annabel`
-   **Skeleton**: `codemonster-ru/annabel-skeleton`
-   **SSR Bridge**: `codemonster-ru/ssr-bridge`
-   **SSR Service**: `@codemonster-ru/ssr-service`

## 5. Final table

| Destination | Composer                        | NPM                         | GitHub repo      |
| ----------- | ------------------------------- | --------------------------- | ---------------- |
| Framework   | codemonster-ru/annabel          | —                           | annabel          |
| Skeleton    | codemonster-ru/annabel-skeleton | —                           | annabel-skeleton |
| SSR Bridge  | codemonster-ru/ssr-bridge       | —                           | ssr-bridge       |
| SSR Service | —                               | @codemonster-ru/ssr-service | ssr-service      |
| Env         | codemonster-ru/env              | —                           | env              |
| Env         | —                               | @codemonster-ru/env         | env-js           |
| Config      | codemonster-ru/config           | —                           | config           |
| Router      | codemonster-ru/router           | —                           | router           |
| View        | codemonster-ru/view             | —                           | view             |
