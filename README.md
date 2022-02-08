# Slidev テンプレート

このテンプレートは[Slidev](https://github.com/slidevjs/slidev) + github actionsで自動的にPDFを生成してくれるやつです

### 始め方
```
yarn
yarn run dev
# visit http://localhost:3030
```

### ローカルでのPDF出力

```
yarn export
```

### githubでリリース
```
# vX.Xの形式でバージョンタグを切ることで自動リリースされます
git tag -a v1.0 -m "変更内容"
git push origin v1.0
```

Slidevの詳しい使い方は[documentations](https://sli.dev/)を参照してください
