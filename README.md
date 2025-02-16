# Nuxt3 i18n プロジェクト

## 機能

- 多言語対応（i18n）
- TypeScriptサポート
- Nuxt DevTools

## セットアップ

依存関係のインストール:

```bash
# npm
npm install

# pnpm
pnpm install

# yarn
yarn install
```

## 開発サーバー

`http://localhost:3000`で開発サーバーを起動:

```bash
# npm
npm run dev

# pnpm
pnpm dev

# yarn
yarn dev
```

## 多言語対応（i18n）について

このプロジェクトでは[@nuxtjs/i18n](https://i18n.nuxtjs.org/)を使用して多言語対応を実装しています。

### サポート言語

- 英語 (en)
- フランス語 (fr)

### 使用例

```vue
<script setup>
const { setLocale } = useI18n();
</script>

<template>
  <!-- 言語切り替えボタン -->
  <button @click="setLocale('en')">English</button>
  <button @click="setLocale('fr')">Français</button>
  
  <!-- 翻訳テキストの表示 -->
  <p>{{ $t('welcome') }}</p>
</template>
```

## 本番環境用ビルド

本番環境用にアプリケーションをビルド:

```bash
# npm
npm run build

# pnpm
pnpm build

# yarn
yarn build
```

本番環境ビルドのプレビュー:

```bash
# npm
npm run preview

# pnpm
pnpm preview

# yarn
yarn preview
```

詳細は[Nuxtデプロイメントドキュメント](https://nuxt.com/docs/getting-started/deployment)をご確認ください。
