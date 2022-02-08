---
# テーマはslidev公式のデフォルト
# コンフィグの詳細は下記から
# https://github.com/slidevjs/slidev/blob/main/packages/types/src/config.ts
theme: default
colorSchema: 'light'
class: 'text-left'
highlighter: shiki
lineNumbers: false
drawings:
  persist: false
---

# いい感じのタイトル

githubで管理するテキストベースの資料

<div class="pt-12">
    所属とか名前とか
</div>

---

# リスト表示

いい感じの説明テキスト
- 📝 **アイコン** -マークダウンのリスト
  - 字下げ
    - さらに字下げ
- リストリスト

説明テキスト

| テーブル | テーブル |
| --- | --- |
| カラム | カラム |
| カラム | カラム |
<br>
リンク：[Slidev](https://sli.dev/guide/)

<!-- CSSでテンプレートを上書きできる(タイトル部分)  -->
<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
layout: two-cols
---
<!-- 2カラム -->
# 左側
## タイトル1

左側のテキスト

::right::
# 右側
## タイトル2
右側のテキスト

---
layout: image-right
image: https://source.unsplash.com/collection/94734566/1920x1080
---

# 自己紹介とかイントロ

右側に画像を配置するスライド、注釈のサンプル[^1]

[^1]: [Learn More](https://sli.dev/guide/syntax.html#line-highlighting)

<style>
.footnotes-sep {
  @apply mt-20 opacity-10;
}
.footnotes {
  @apply text-sm opacity-75;
}
.footnote-backref {
  display: none;
}
</style>

---

# Vueコンポーネント

<div grid="~ cols-2 gap-4">
<div>

Vueコンポーネントをスライドに埋め込むことができる

`<Tweet />`や`<Youtube />`などのビルトインのコンポーネントを使うこともできるし
自分でコンポーネントを作成してそれを使用することもできる

```html
<Counter :count="10" />
```

<!-- ./components/Counter.vue -->
<Counter :count="10" m="t-4" />

詳しくは [ガイド](https://sli.dev/builtin/components.html) を参照

</div>
<div>

```html
<Tweet id="1390115482657726468" />
```

<Tweet id="1390115482657726468" scale="0.65" />

</div>
</div>


---

# グリッド表示

説明を上部に表示しつつ、divタグを使って２カラム表示を作ることができるサンプル

<div grid="~ cols-2 gap-2" m="-t-2">

```yaml
---
theme: default
---
```

```yaml
---
theme: seriph
---
```

<img border="rounded" src="https://github.com/slidevjs/themes/blob/main/screenshots/theme-default/01.png?raw=true">

<img border="rounded" src="https://github.com/slidevjs/themes/blob/main/screenshots/theme-seriph/01.png?raw=true">

ほげほげほげほげ

ふがふがふがふが
</div>
