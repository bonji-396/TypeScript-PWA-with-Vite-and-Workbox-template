# Vite で TypeScript + PWA のテンプレート

WebPackを利用して、TypeScriptでPWAのフロントエンドアプリを作るためのテンプレートです。

## 主な技術構成
- TypeScript
- PWA
- Sass
- RxJS


## 導入
```zsh
npm install
```

### 実際の導入

- ` npm create vite`コマンド  
   ```zsh
   npm create vite@latest TypeScript-PWA-with-Vite-template -- --template vanilla-ts
   cd TypeScript-PWA-with-Vite-template
   npm install rxjs
   npm install -D sass vite-plugin-pwa @types/serviceworker
   ```
- `vite.config.ts`を作成
- `src/main.ts`を修正
- `src/styles/main.scss`の作成
- `index.html`を修正
- `public/icons`に画像を追加


### 開発利用パッケージ

これらのパッケージは主に開発環境の構築とビルドプロセスの自動化に使用されています。
- @types/serviceworker:  
Service Worker APIのTypeScript型定義ファイル。PWA（Progressive Web App）開発において、Service Workerを型安全に実装するために使用
- sass:  
Webで人気の高いCSSプリプロセッサー。変数、ネスト、ミックスインなどの機能を提供し、効率的なスタイルシート開発を可能にする
- typescript:  
JavaScriptに静的型付けを追加したプログラミング言語。コード品質の向上とIDEのサポート強化に寄与する
- vite:  
モダンなフロントエンド開発ツール。超高速な開発サーバーとビルドツールを提供し、ESモジュールを活用した効率的な開発が可能
- vite-plugin-pwa:  
ViteのPWAプラグイン。Service Workerの生成、マニフェストファイルの管理など、PWAに必要な機能を自動化する

## 開発サーバー起動
```
npm run dev
```
## ビルド
```
npm run build
```
## ビルド結果のプレビュー
```
npm run preview
```