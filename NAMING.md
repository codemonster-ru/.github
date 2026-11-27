# CodeMonster repository and package names

Use short, descriptive names in lowercase. Join multiple words with hyphens, as in `http-client`
and `ssr-service`. Preserve established public names such as `floater.js` and GitHub's reserved
`.github` repository.

## Packages

- Composer packages use `codemonster-ru/<name>`. PHP code uses the `Codemonster\` namespace.
- npm packages use `@codemonster-ru/<name>`. Use that name in `package.json`.
- If two repositories share a base name, keep the established repository name and use a language
  suffix for the other implementation. The suffix distinguishes GitHub repositories. The npm and
  Composer packages can share their unqualified names because the registries are separate.
- Use the current canonical GitHub URL in GitHub Actions, package metadata, and documentation.

## Published examples

| Project | GitHub source or package repository | Registry name |
| --- | --- | --- |
| Annabel source monorepo | [`annabel`](https://github.com/codemonster-ru/annabel) | |
| Annabel framework package mirror | [`annabel-framework`](https://github.com/codemonster-ru/annabel-framework) | `codemonster-ru/annabel` on Composer |
| Annabel Skeleton | [`annabel-skeleton`](https://github.com/codemonster-ru/annabel-skeleton) | `codemonster-ru/annabel-skeleton` on Composer |
| Annabel CMS | [`annabel-cms`](https://github.com/codemonster-ru/annabel-cms) | `codemonster-ru/annabel-cms` on Composer |
| PHP Env | [`env`](https://github.com/codemonster-ru/env) | `codemonster-ru/env` on Composer |
| Node.js Env | [`env-js`](https://github.com/codemonster-ru/env-js) | `@codemonster-ru/env` on npm |
| PHP Config | [`config`](https://github.com/codemonster-ru/config) | `codemonster-ru/config` on Composer |
| SSR Bridge | [`ssr-bridge`](https://github.com/codemonster-ru/ssr-bridge) | `codemonster-ru/ssr-bridge` on Composer |
| SSR Service | [`ssr-service`](https://github.com/codemonster-ru/ssr-service) | `@codemonster-ru/ssr-service` on npm |
| CodeMonster UI | [`ui`](https://github.com/codemonster-ru/ui) | `@codemonster-ru/ui-*` design-system packages on npm |
| CodeMonster UI for Annabel Razor | [`ui-razor`](https://github.com/codemonster-ru/ui-razor) | `codemonster-ru/ui-razor` on Composer |
| Floater.js | [`floater.js`](https://github.com/codemonster-ru/floater.js) | `@codemonster-ru/floater.js` on npm |
