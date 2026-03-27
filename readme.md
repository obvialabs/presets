<b align="center">

[![Version](https://img.shields.io/npm/v/@obvia/presets?style=for-the-badge&logo=npm&labelColor=ff2949&color=e93146&logoColor=white&label=Version)](https://www.npmjs.com/package/@obvia/presets)
[![Typescript](https://img.shields.io/static/v1?message=5.9.3&style=for-the-badge&logo=typescript&labelColor=1886c9&color=0A66C2&logoColor=white&label=TypeScript)](https://www.typescriptlang.org/)
[![Linting](https://img.shields.io/static/v1?message=Eslint&style=for-the-badge&logo=eslint&labelColor=eb6a3b&color=cc5c33&logoColor=white&label=Linting)](https://npmjs.com/package/@obvia/presets)
[![License](https://img.shields.io/static/v1?message=MIT&style=for-the-badge&logo=opensourceinitiative&labelColor=25D366&color=20bd5b&logoColor=white&label=License)](https://npmjs.com/package/@obvia/presets)
[![CI](https://img.shields.io/github/actions/workflow/status/obvialabs/presets/publish.yml?style=for-the-badge&logo=githubactions&labelColor=161717&color=0f0f0f&logoColor=white&label=CI)](https://github.com/obvialabs/presets/actions)
</b>

> Designed to provide consistent rules and configurations across projects with minimal setup.

Welcome to the **Obvia presets** — a shared foundation for linting and typing rules across the ecosystem.
This package continuously tracks the latest modern releases of ESLint and TypeScript, ensuring every
project stays aligned. It’s not meant to be a static config, but a living set of presets that evolve with
the ecosystem. If following the latest versions fits your workflow, this package offers a reliable way to
keep all your projects consistent and up‑to‑date.

- **Unified rules** → Consistent ESLint and TypeScript configs across all Obvia projects
- **Always modern** → Tracks the latest ESLint and TypeScript releases
- **Minimal setup** → Drop‑in presets, no need to reinvent configs
- **Ecosystem alignment** → Ensures every package and project follows the same standards
- **Onboarding‑friendly** → Simplifies developer experience for new contributors

## Installation

All presets are bundled in a single package — no need to install separate configs for each framework

```bash
pnpm add --save-dev @obvia/presets
```

## Quickstart

### Linting

Choose the preset that matches your project and add it to `eslint.config.js`

```js
// Base → General rules for most projects
import { base } from "@obvia/presets/base-eslint"

// React → Rules for react and react Hooks
import { react } from "@obvia/presets/react-eslint"

// Next.js → Optimized rules for next.js applications
import { next } from "@obvia/presets/next-eslint"

export default [
  base,
  // react,
  // next,
]
```

### Configuration

Extend the corresponding config in your `tsconfig.json`

```json
// Base → General Typescript rules
{
  "extends": "@obvia/presets/base-config"
}
// React → Typescript config for react projects
{
  "extends": "@obvia/presets/react-config"
}
// Next.js → Typescript config for next.js projects
{
  "extends": "@obvia/presets/next-config"
}
```

## Roadmap

The roadmap shows both the **currently available presets** and the **planned additions**.

| Preset    | Description                                         | Path                     | Status      |
|-----------|-----------------------------------------------------|--------------------------|-------------|
| **Base**  | General typescript + eslint rules for most projects | `@obvia/presets/base-*`  | ✅ Available |
| **React** | Additional rules for react and react hooks          | `@obvia/presets/react-*` | ✅ Available |
| **Next**  | Optimized rules for next.js applications            | `@obvia/presets/next-*`  | ✅ Available |
| **Vue**   | Rules optimized for vue.js applications             | _(coming soon)_          | 🔜 Planned  |
| **Nuxt**  | Configurations for nuxt.js projects                 | _(coming soon)_          | 🔜 Planned  |

## Security

If you think there is a security vulnerability in the **Presets**, you can help resolve the
issue immediately by sending an e-mail to **Selçuk Çukur** at **<hello@selcukcukur.me>**. Please
do not publicly post security vulnerabilities.

## License

**Presets** project is published as open source. The **[MIT License](License.md)** is used, which
is one of the well-known open source coding licenses. You can get detailed information about the license terms
by visiting the link below.

- **[MIT License](license.md)**
