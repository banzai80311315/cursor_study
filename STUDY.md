# HTML と CSS の学習記録

## 2024 年の学習内容

### 基本的な HTML と CSS の構造

#### HTML ファイル（index.html）の作成

基本的な HTML5 の構造を作成しました。主な要素：

- `<!DOCTYPE html>`宣言
- 日本語対応（`lang="ja"`）
- メタ情報の設定
- 基本的なページ構造（header, main, footer）

```html
<!DOCTYPE html>
<html lang="ja">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>はじめてのHTML</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <header>
      <h1>ようこそ！</h1>
    </header>
    <main>
      <section>
        <h2>HTMLの基本</h2>
        <p>これは段落（パラグラフ）です。</p>
        <ul>
          <li>リスト項目1</li>
          <li>リスト項目2</li>
          <li>リスト項目3</li>
        </ul>
      </section>
    </main>
    <footer>
      <p>&copy; 2024 はじめてのHTML</p>
    </footer>
  </body>
</html>
```

#### CSS ファイル（styles.css）の作成

モダンでレスポンシブなデザインを実装：

- 全体のレイアウト設定
- ヘッダーとフッターのスタイリング
- メインコンテンツの配置
- リストのスタイリング
- 見出しのデザイン

```css
/* 全体のスタイル */
body {
  font-family: "Helvetica Neue", Arial, sans-serif;
  line-height: 1.6;
  margin: 0;
  padding: 0;
  background-color: #f5f5f5;
}

/* ヘッダーのスタイル */
header {
  background-color: #4caf50;
  color: white;
  text-align: center;
  padding: 2rem;
}

/* メインコンテンツのスタイル */
main {
  max-width: 800px;
  margin: 2rem auto;
  padding: 0 1rem;
}

section {
  background-color: white;
  padding: 2rem;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

/* 見出しのスタイル */
h1 {
  margin: 0;
  font-size: 2.5rem;
}

h2 {
  color: #333;
  border-bottom: 2px solid #4caf50;
  padding-bottom: 0.5rem;
}

/* リストのスタイル */
ul {
  list-style-type: none;
  padding: 0;
}

li {
  padding: 0.5rem 0;
  border-bottom: 1px solid #eee;
}

/* フッターのスタイル */
footer {
  text-align: center;
  padding: 1rem;
  background-color: #333;
  color: white;
  position: fixed;
  bottom: 0;
  width: 100%;
}
```

### 学んだこと

1. HTML の基本構造と主要なタグの使い方
2. CSS でのスタイリングの基本
3. モダンなウェブデザインの実装方法
4. レスポンシブデザインの考え方

### 次のステップ

- より多くの HTML 要素の学習
- CSS アニメーションの追加
- JavaScript の導入
- レスポンシブデザインの強化

## 1. 基本的な HTML 構造

- `<!DOCTYPE html>`宣言
- `<html lang="ja">`で日本語ページの指定
- `<head>`と`<body>`の役割
- メタ情報とタイトルの設定

## 2. 自己紹介ページの作成

### HTML 要素の使用

- ヘッダー（`<header>`）
- ナビゲーション（`<nav>`）
- メインコンテンツ（`<main>`）
- セクション（`<section>`）
- 画像（`<img>`）
- リスト（`<ul>`, `<li>`）
- フッター（`<footer>`）

### CSS スタイリング

- フレックスボックスレイアウト
  ```css
  .profile {
    display: flex;
    gap: 2rem;
    align-items: start;
  }
  ```
- グリッドレイアウト
  ```css
  .link-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 1rem;
  }
  ```
- アニメーション効果
  ```css
  .dog-icon:hover {
    transform: scale(1.05);
  }
  ```

## 3. リンク集ページの作成

### 実装した機能

- ナビゲーションメニュー
- リンクカードのデザイン
- レスポンシブデザイン
- ホバーエフェクト

### 学んだ CSS テクニック

- トランジション効果
  ```css
  transition: transform 0.3s, box-shadow 0.3s;
  ```
- ボックスシャドウ
  ```css
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  ```
- アクティブ状態のスタイリング
  ```css
  .nav-link.active {
    background-color: rgba(255, 255, 255, 0.3);
  }
  ```

## 4. 画像の扱い方

- ローカル画像の使用方法
- 画像パスの指定方法
- 画像のサイズ調整
- 代替テキスト（alt 属性）の重要性

## 5. レスポンシブデザイン

- ビューポートの設定
  ```html
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  ```
- フレックスボックスとグリッドの活用
- メディアクエリの使用

## 今後の学習予定

1. JavaScript の基礎
2. フォームの作成
3. アニメーションの追加
4. アクセシビリティの改善
