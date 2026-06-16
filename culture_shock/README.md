# 日本に来てびっくりしたこと

留学生のみなさんが日本で感じたカルチャーショックを紹介するWebページを作ってください。

## アウトプット

1ページのWebサイトをチームで制作します。

テーマ：

> 日本に来てびっくりしたこと / Culture Shock in Japan

## ファイルのつくり

```txt
culture-shock-page/
├── index.html
├── css/
│   ├── common.css
│   ├── st-a.css　# Aさん
│   ├── st-b.css  # Bさん
│   ├── st-c.css  # Cさん
│   └── st-d.css  # Dさん
└── README.md
```

## 担当表

```txt
st-a：Aさん
st-b：Bさん
st-c：Cさん
st-d：Dさん
```

## 作業ルール

1. 自分の担当セクションだけ編集する
2. 自分のCSSファイルだけ編集する
3. `common.css` は編集しない
4. `main` ブランチに直接 push しない
5. 自分のブランチを作って作業する
6. 作業が終わったら Pull Request を作る
7. 他の人の Pull Request を1回レビューする

## ブランチ名の例

```txt
feature/st-a
feature/st-b
feature/st-c
feature/st-d
```

## commitメッセージ例

```txt
add st-a culture shock section
update st-b design
fix st-c text
add st-d country info
```

## Pull Requestテンプレート

```md
## やったこと
- 自分の担当セクションを編集しました
- 自分のCSSファイルを編集しました

## 担当
st-〇

## テーマ
例：電車が時間通りに来ること

## 確認してほしいこと
- 文章が分かりやすいか
- レイアウトが崩れていないか
- 自分の担当以外を変更していないか
```

## 人数を増やす場合

`st-e.css` や `st-f.css` を追加し、`index.html` の `<head>` にCSS読み込みを追加します。

```html
<link rel="stylesheet" href="css/st-e.css">
<link rel="stylesheet" href="css/st-f.css">
```

`index.html` の `<main>` 内にも、同じ形式でセクションを追加します。

```html
<section id="st-e" class="shock-card">
  <h2>ここに驚いたことを書く</h2>
  <p class="country">出身国：〇〇</p>
</section>
```
