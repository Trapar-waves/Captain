# @trapar-waves/captain

![npm version](https://img.shields.io/npm/v/@trapar-waves/captain)
![npm dm](https://img.shields.io/npm/dm/@trapar-waves/captain)
![License](https://img.shields.io/github/license/Trapar-waves/Captain)
![GitHub last commit](https://img.shields.io/github/last-commit/Trapar-waves/Captain)
![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/Trapar-waves/Captain/release.yml)
![Renovate](https://img.shields.io/badge/renovate-enabled-blue)

---

[中文](./readme/README-CN.md) | [日本語](./readme/README-JP.md) | [Русский язык](./readme/README-RU.md)

> A template management tool for organizing and listing various project templates. It provides a unified registry of Trapar Waves template packages with metadata, enabling quick discovery and selection of templates for CLI, React, Vue, LLM, and more.

## ✨ Features

- **Centralized Template Registry:** Manages multiple project templates (CLI, React, Vue, LLM, etc.) from a single source of truth.
- **Pre-integrated Metadata:** Ships with built-in template metadata from official Trapar Waves template packages, ready to use out of the box.
- **Unified Template List:** Provides a consistent API (`createList`) for accessing and selecting templates programmatically.
- **Dual Module Support:** Supports both ESM and CommonJS module formats for maximum compatibility.
- **Type Safety:** Written in TypeScript with full type definitions exported for a reliable developer experience.
- **Lightweight:** Minimal dependencies (`destr`, `pkg-types`, `ufo`) with a small footprint.

## 💻 Tech Stack

- **Language:** TypeScript
- **Build Tool:** Rslib (`@rslib/core`)
- **Runtime:** Node.js
- **Dependencies:** `destr` (safe JSON parsing), `pkg-types` (package.json utilities), `ufo` (URL utilities)
- **Linting:** ESLint with `@antfu/eslint-config`

See the [package.json](./package.json) for a full list of dependencies.

## 🚀 Getting Started

### Prerequisites

- Node.js (>= 18.x recommended)
- Package manager (npm, yarn, or pnpm)

### Installation

Install the package as a dependency in your project:

```bash
npm install @trapar-waves/captain
```

Or with yarn:

```bash
yarn add @trapar-waves/captain
```

Or with pnpm:

```bash
pnpm add @trapar-waves/captain
```

### Usage

Import and use the template list in your project:

```ts
import { createList } from '@trapar-waves/captain';

console.log(createList);
// Outputs an array of template objects with name and description
```

## 📁 Project Structure

```
├── src/
│   ├── index.ts          # Entry point, re-exports public API
│   ├── create-list.ts    # Template list creation logic
│   └── package.ts        # Template package metadata definitions
├── dist/                 # Compiled output (ESM + CJS)
├── rslib.config.ts       # Rslib build configuration
├── eslint.config.js      # ESLint configuration
├── tsconfig.json         # TypeScript configuration
└── package.json          # Project dependencies and scripts
```

## 📋 Supported Templates

| Template | Description |
|----------|-------------|
| `@trapar-waves/cli-template` | CLI development template |
| `@trapar-waves/llm-template` | LLM project template |
| `@trapar-waves/react-antd-pro` | React + Ant Design Pro enterprise app |
| `@trapar-waves/react-mantine-tailwind` | React + Mantine + Tailwind UI |
| `@trapar-waves/react-tailwind` | React + Tailwind starter |
| `@trapar-waves/react-tanstack` | React + TanStack Query/Router |
| `@trapar-waves/react-three-maplibre` | 3D map visualization (Three.js + MapLibre) |
| `@trapar-waves/react-visgl-maplibre` | Geospatial 3D rendering (Deck.gl + MapLibre) |
| `@trapar-waves/vue-tailwind` | Vue 3 + Tailwind starter |

## 🤝 Contributing

Contributions are welcome and greatly appreciated! Please follow these steps to contribute:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

MIT License © 2025 Trapar Waves

## 👤 Author

- **Rikka:** [admin@rikka.cc](mailto:admin@rikka.cc)
- **GitHub Profile:** [Muromi-Rikka](https://github.com/Muromi-Rikka)

## 🔗 Links

- **Repository:** [https://github.com/Trapar-waves/Captain](https://github.com/Trapar-waves/Captain)
- **Issues:** [https://github.com/Trapar-waves/Captain/issues](https://github.com/Trapar-waves/Captain/issues)
