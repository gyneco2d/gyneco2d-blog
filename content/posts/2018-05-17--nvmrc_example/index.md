---
title: .nvmrcの書き方
subTitle: nodeのバージョンを書き込む
category: development
cover: ../article_icons/settings.jpg
---

Netlifyにこのサイトを設置するとき`.nvmrc`を用意する必要があったのでメモ．
nvmはNode.jsのバージョン管理ソフトウェアらしい．
プロジェクト直下のディレクトリに`.nvmrc`があるとそれを見に行ってそのバージョンを利用してくれる．

### 書式
nodeのバージョンを書き込むだけでいいらしい

```bash
$ node -v > .nvmrc
```

参考：[.nvmrc example? · Issue #995 · creationix/nvm](https://github.com/creationix/nvm/issues/995)

このバージョンがインストールされていない時はエラーが出るが，`nvm install && nvm use`できる．
