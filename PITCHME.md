## Laravelを  """さいはや""" で理解するためのいくつかのお約束

---

### What is this?

この資料はGitPitchを使ってみたいがために作った資料です。

---

### What is this? - part2

最近こんな書き込みをインターネットウェッブで見かける

---

"初心者必見！『Laravel』入門"

---

:thinking:

---

### Laravelは「初心者」必見になり得るか？
A：なり得ない。多分勘違いをしている人が多そうな雰囲気がある

---

## Laravelを正確に表現しよう

---

### Laravelについての説明

---

### Bad Context
✗ 「Ruby on Rails と同じ、 MVC で CRUD を採用」


✗ 「Bootstrap や Vue、 React も標準対応」

---

### Good Context

○ 「Easy(最短で使用する)でCRUDを採用している」

◎ 「Ruby on Railsの思想 [Active Record]パターンが影響されているORM [Eloquent]が便利(だと思う)」

　 「EasyだけでなくSimpleな設計が行えるので多岐に渡る設計(Architecture)を組みやすい」
  
○ 「コマンド一つ(Artisan)で簡単にVueフレームワークを導入できるパッケージが人気」

◎ 「RESTfulなAPI設計がSimpleに行えるのでフロントフレームワークに依存する必要が無い」

---

### 要するに何？

#### A：よくあるPHPフレームワークの「制約」が緩くて自在に拡張も縮小も可能なフレームワーク

---

## はたして簡単だろうか？

---

## 本題

---

## """さいはや""" で理解する #とは

---

### Easyパターン
リーダブルを参照しよう(日本語非公式版)
https://readouble.com/laravel/6.x/ja/installation.html

---
### Simpleパターン

例えば、EloquentではCollectionというデータモデル（Class）でDBとのやり取りを取得している

---

例えば、Eloquentで取得したCollectionをソートしたいときは？

調べたらすぐ出てくる

https://readouble.com/laravel/6.x/ja/collections.html#method-sortby

わりと簡単

---

UploadedFileで取得した一時的ファイルのパス情報が欲しい、

なんて奇特な実装が必要になってしまった時

https://qiita.com/mashirou_yuguchi/items/14d3614173c114c30f02

```php
$request->file('file')->getPathname();
```

---

見つけるのに時間が掛かったりする

---

### 調べる時のやり方

---

###　Tl； DL

+++

## 実際に実装の流れを追うのが一番確実

---
