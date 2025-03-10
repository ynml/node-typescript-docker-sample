# Node.js

このディレクトリは、TypeScript で実装された Node.js マイクロサービスを含んでいます。

## 技術スタック

- Node.js 18.x 以上
- TypeScript 5.x
- Docker

## プロジェクト構成

```
node/
├── Dockerfile        # Dockerビルド設定
├── tsconfig.json     # TypeScript設定
└── package.json      # 依存関係管理
```

## 開発環境のセットアップ

### ローカル開発

1. 依存関係のインストール:

```bash
pnpm install
```

2. 開発サーバーの起動:

```bash
pnpm start
```

3. ビルド:

```bash
pnpm compile
```

### Docker 環境

1. イメージのビルド:

```bash
docker build -t node-service .
```

2. コンテナの起動:

```bash
docker run -p 3000:3000 node-service
```

## 環境変数

| 変数名   | 説明                 | デフォルト値 |
| -------- | -------------------- | ------------ |
| PORT     | サービスのポート番号 | 3000         |
| NODE_ENV | 実行環境             | development  |
