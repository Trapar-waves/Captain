# @trapar-waves/captain

![npm version](https://img.shields.io/npm/v/@trapar-waves/captain)
![npm dm](https://img.shields.io/npm/dm/@trapar-waves/captain)
![License](https://img.shields.io/github/license/Trapar-waves/Captain)
![GitHub last commit](https://img.shields.io/github/last-commit/Trapar-waves/Captain)
![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/Trapar-waves/Captain/release.yml)
![Renovate](https://img.shields.io/badge/renovate-enabled-blue)

---

[English](../README.md) | [日本語](./README-JP.md) | [Русский язык](./README-RU.md)

> 一个模板管理工具，用于组织和列出各种项目模板。它提供了 Trapar Waves 模板包的统一注册表及元数据，方便快速发现和选择 CLI、React、Vue、LLM 等模板。

## ✨ 特性

- **集中式模板注册表：** 从单一来源管理多个项目模板（CLI、React、Vue、LLM 等）。
- **预集成元数据：** 内置来自官方 Trapar Waves 模板包的模板元数据，开箱即用。
- **统一模板列表：** 提供一致的 API（`createList`），支持以编程方式访问和选择模板。
- **双模块格式支持：** 同时支持 ESM 和 CommonJS 模块格式，具有最大兼容性。
- **类型安全：** 使用 TypeScript 编写，导出完整的类型定义，提供可靠的开发体验。
- **轻量级：** 最少的依赖（`destr`、`pkg-types`、`ufo`），体积小巧。

## 💻 技术栈

- **语言：** TypeScript
- **构建工具：** Rslib（`@rslib/core`）
- **运行时：** Node.js
- **依赖：** `destr`（安全 JSON 解析）、`pkg-types`（package.json 工具）、`ufo`（URL 工具）
- **代码检查：** ESLint 和 `@antfu/eslint-config`

查看 [package.json](../package.json) 获取完整的依赖列表。

## 🚀 快速开始

### 前置条件

- Node.js（推荐 >= 18.x）
- 包管理器（npm、yarn 或 pnpm）

### 安装

将包安装为项目依赖：

```bash
npm install @trapar-waves/captain
```

或使用 yarn：

```bash
yarn add @trapar-waves/captain
```

或使用 pnpm：

```bash
pnpm add @trapar-waves/captain
```

### 使用方法

在项目中导入并使用模板列表：

```ts
import { createList } from '@trapar-waves/captain';

console.log(createList);
// 输出包含名称和描述的模板对象数组
```

## 📁 项目结构

```
├── src/
│   ├── index.ts          # 入口点，重新导出公共 API
│   ├── create-list.ts    # 模板列表创建逻辑
│   └── package.ts        # 模板包元数据定义
├── dist/                 # 编译输出（ESM + CJS）
├── rslib.config.ts       # Rslib 构建配置
├── eslint.config.js      # ESLint 配置
├── tsconfig.json         # TypeScript 配置
└── package.json          # 项目依赖和脚本
```

## 📋 支持的模板

| 模板 | 描述 |
|------|------|
| `@trapar-waves/cli-template` | CLI 开发模板 |
| `@trapar-waves/llm-template` | LLM 项目模板 |
| `@trapar-waves/react-antd-pro` | React + Ant Design Pro 企业应用 |
| `@trapar-waves/react-mantine-tailwind` | React + Mantine + Tailwind UI |
| `@trapar-waves/react-tailwind` | React + Tailwind 入门模板 |
| `@trapar-waves/react-tanstack` | React + TanStack Query/Router |
| `@trapar-waves/react-three-maplibre` | 3D 地图可视化（Three.js + MapLibre） |
| `@trapar-waves/react-visgl-maplibre` | 地理空间 3D 渲染（Deck.gl + MapLibre） |
| `@trapar-waves/vue-tailwind` | Vue 3 + Tailwind 入门模板 |

## 🤝 贡献

欢迎贡献，非常感谢！请按照以下步骤贡献：

1. Fork 仓库
2. 创建特性分支（`git checkout -b feature/amazing-feature`）
3. 提交更改（`git commit -m 'Add some amazing feature'`）
4. 推送到分支（`git push origin feature/amazing-feature`）
5. 创建 Pull Request

## 📄 许可证

MIT License © 2025 Trapar Waves

## 👤 作者

- **Rikka：** [admin@rikka.cc](mailto:admin@rikka.cc)
- **GitHub 主页：** [Muromi-Rikka](https://github.com/Muromi-Rikka)

## 🔗 链接

- **仓库：** [https://github.com/Trapar-waves/Captain](https://github.com/Trapar-waves/Captain)
- **Issues：** [https://github.com/Trapar-waves/Captain/issues](https://github.com/Trapar-waves/Captain/issues)
