# Shojin-App Landing Page

Shojin-Appの公式ランディングページのリポジトリです。
このプロジェクトは [Astro](https://astro.build) フレームワークを使用して構築されており、スタイリングには [BeerCSS](https://www.beercss.com/) を採用しています。

## 🚀 プロジェクトの概要

Shojin-Appの魅力を伝え、ユーザーにアプリのダウンロードを促すためのWebサイトです。
以下のセクションで構成されています：

- **Hero**: アプリの第一印象を決定づけるメインビジュアルとキャッチコピー
- **Features**: アプリの主要機能の紹介
- **Get Started**: アプリの利用開始方法やダウンロードリンク
- **Header/Footer**: ナビゲーションとリンク

## 🛠️ 技術スタック

- **Framework**: [Astro](https://astro.build)
- **Styling**: [BeerCSS](https://www.beercss.com/)
- **Runtime & Package Manager**: [Bun](https://bun.sh)

## 🧞 コマンド

プロジェクトのルートディレクトリで以下のコマンドを実行してください。

| コマンド | 説明 |
| :--- | :--- |
| `bun install` | 依存関係のインストール |
| `bun dev` | ローカル開発サーバーを `localhost:4321` で起動 |
| `bun build` | 本番用ビルドを `./dist/` に出力 |
| `bun preview` | ビルドされたサイトをローカルでプレビュー |

## 📂 プロジェクト構造

```text
/
├── public/       # 静的アセット（画像など）
├── src/
│   ├── components/   # 再利用可能なUIコンポーネント (Hero, Features, etc.)
│   ├── layouts/      # ページレイアウト
│   └── pages/        # ページルート (index.astro)
├── package.json
└── astro.config.mjs
```

## 開発について

### 新しいコンポーネントの追加
`src/components/` ディレクトリに新しい `.astro` ファイルを作成し、`src/pages/index.astro` などのページファイルでインポートして使用します。

### スタイリング
BeerCSSを使用しているため、HTML要素に適切なクラスを付与することでマテリアルデザインに準拠したスタイルを適用できます。
カスタムスタイルが必要な場合は、各コンポーネント内の `<style>` タグに記述するか、グローバルなCSSファイルを追加してください。
