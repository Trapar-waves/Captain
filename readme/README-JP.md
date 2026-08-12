# @trapar-waves/captain

![npm version](https://img.shields.io/npm/v/@trapar-waves/captain)
![npm dm](https://img.shields.io/npm/dm/@trapar-waves/captain)
![License](https://img.shields.io/github/license/Trapar-waves/Captain)
![GitHub last commit](https://img.shields.io/github/last-commit/Trapar-waves/Captain)
![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/Trapar-waves/Captain/release.yml)
![Renovate](https://img.shields.io/badge/renovate-enabled-blue)

---

[English](../README.md) | [中文](./README-CN.md) | [Русский язык](./README-RU.md)

> さまざまなプロジェクトテンプレートを整理・一覧表示するテンプレート管理ツール。CLI、React、Vue、LLM などのテンプレートを迅速に発見・選択できるよう、Trapar Waves テンプレートパッケージの統一レジストリとメタデータを提供します。

## ✨ 特徴

- **集中型テンプレートレジストリ：** 複数のプロジェクトテンプレート（CLI、React、Vue、LLM など）を単一の情報源から管理。
- **事前統合されたメタデータ：** 公式 Trapar Waves テンプレートパッケージのメタデータが組み込まれており、すぐに使用可能。
- **統一テンプレートリスト：** プログラムによるテンプレートへのアクセスと選択のための一貫した API（`createList`）を提供。
- **デュアルモジュールサポート：** ESM と CommonJS の両方のモジュール形式に対応し、最大限の互換性を実現。
- **型安全性：** TypeScript で記述され、完全な型定義がエクスポートされ、信頼性の高い開発体験を提供。
- **軽量：** 最小限の依存関係（`destr`、`pkg-types`、`ufo`）で小さなフットプリント。

## 💻 技術スタック

- **言語：** TypeScript
- **ビルドツール：** Rslib（`@rslib/core`）
- **ランタイム：** Node.js
- **依存関係：** `destr`（安全な JSON パース）、`pkg-types`（package.json ユーティリティ）、`ufo`（URL ユーティリティ）
- **リント：** ESLint と `@antfu/eslint-config`

依存関係の完全なリストは [package.json](../package.json) を参照してください。

## 🚀 はじめに

### 前提条件

- Node.js（>= 18.x 推奨）
- パッケージマネージャー（npm、yarn、または pnpm）

### インストール

プロジェクトの依存関係としてパッケージをインストール：

```bash
npm install @trapar-waves/captain
```

yarn の場合：

```bash
yarn add @trapar-waves/captain
```

pnpm の場合：

```bash
pnpm add @trapar-waves/captain
```

### 使用方法

プロジェクトでテンプレートリストをインポートして使用：

```ts
import { createList } from '@trapar-waves/captain';

console.log(createList);
// 名前と説明を含むテンプレートオブジェクトの配列を出力
```

## 📁 プロジェクト構造

```
├── src/
│   ├── index.ts          # エントリーポイント、パブリック API の再エクスポート
│   ├── create-list.ts    # テンプレートリスト作成ロジック
│   └── package.ts        # テンプレートパッケージメタデータ定義
├── dist/                 # コンパイル済み出力（ESM + CJS）
├── rslib.config.ts       # Rslib ビルド設定
├── eslint.config.js      # ESLint 設定
├── tsconfig.json         # TypeScript 設定
└── package.json          # プロジェクトの依存関係とスクリプト
```

## 📋 サポートされているテンプレート

| テンプレート | 説明 |
|-------------|------|
| `@trapar-waves/cli-template` | CLI 開発テンプレート |
| `@trapar-waves/llm-template` | LLM プロジェクトテンプレート |
| `@trapar-waves/react-antd-pro` | React + Ant Design Pro エンタープライズアプリ |
| `@trapar-waves/react-mantine-tailwind` | React + Mantine + Tailwind UI |
| `@trapar-waves/react-tailwind` | React + Tailwind スターター |
| `@trapar-waves/react-tanstack` | React + TanStack Query/Router |
| `@trapar-waves/react-three-maplibre` | 3D マップ可視化（Three.js + MapLibre） |
| `@trapar-waves/react-visgl-maplibre` | 地理空間 3D レンダリング（Deck.gl + MapLibre） |
| `@trapar-waves/vue-tailwind` | Vue 3 + Tailwind スターター |

## 🤝 コントリビュート

コントリビュートを歓迎します！以下の手順に従ってコントリビュートしてください：

1. リポジトリをフォーク
2. 機能ブランチを作成（`git checkout -b feature/amazing-feature`）
3. 変更をコミット（`git commit -m 'Add some amazing feature'`）
4. ブランチにプッシュ（`git push origin feature/amazing-feature`）
5. Pull Request を作成

## 📄 ライセンス

MIT License © 2025 Trapar Waves

## 👤 作者

- **Rikka：** [admin@rikka.cc](mailto:admin@rikka.cc)
- **GitHub プロフィール：** [Muromi-Rikka](https://github.com/Muromi-Rikka)

## 🔗 リンク

- **リポジトリ：** [https://github.com/Trapar-waves/Captain](https://github.com/Trapar-waves/Captain)
- **Issues：** [https://github.com/Trapar-waves/Captain/issues](https://github.com/Trapar-waves/Captain/issues)
