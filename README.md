# @trapar-waves/captain

A template management tool for organizing and listing various project templates.

[![npm version](https://img.shields.io/npm/v/@trapar-waves/captain)](https://www.npmjs.com/package/@trapar-waves/captain)
[![license](https://img.shields.io/npm/l/@trapar-waves/captain)](https://github.com/Trapar-waves/Captain/blob/main/LICENSE)
[![downloads](https://img.shields.io/npm/dt/@trapar-waves/captain)](https://www.npmjs.com/package/@trapar-waves/captain)

## Features

- Centralized management of multiple project templates (CLI, React, Vue, LLM, etc.)
- Pre-integrated template metadata from official Trapar Waves template packages
- Provides a unified template list for quick access and selection
- Supports both ESM and CommonJS module formats

## Installation

To install the package, use npm:

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

## Usage

This package is primarily used as a dependency to provide a list of available templates. Here's how you can import and use it in your project:

```js
import { createList } from '@trapar-waves/captain';

console.log(createList);
// Outputs an array of template objects with name and description
```

## Supported Templates

- CLI templates
- React templates (Ant Design Pro, Mantine Tailwind, Tailwind, Tanstack, Maplibre integrations)
- Vue Tailwind template
- LLM project template

## Contributing

Contributions are welcome! Please follow the standard GitHub flow for submitting pull requests.

## License

MIT License © 2025 Trapar Waves

## Author

[Rikka](https://github.com/Muromi-Rikka)