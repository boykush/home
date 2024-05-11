+++
title = "ScrapsというWiki用のSSGを作っている話"
date = 2023-07-10
[taxonomies]
tags=["Tech", "Output"]
+++

# はじめに

Obsidianを使ってWikiをまとめていたがせっかくならページ公開したいな〜と考えていた。どうやらObsidianでページ公開するには有料プランである必要があるらしい。

有料プランにするほどのモチベはなかったが、Rust入門中だったのでせっかくならStatic Site Generatorを作っちゃえ。となった。

GitHub Repositoryは以下

- [GitHub](https://github.com/boykush/scraps)

# 実装
基本機能はSSGとしてMarkdownをHtmlへと変換する機能。Wiki用ということで加えてページ内リンクを簡単に記述できるようになっている。

実装で用いたメインのライブラリ群は以下

- anyhow(thiserror)
- clap
- pulldown-cmark
- serde
- tera

特にTeraのドキュメントは読み込んだ。同じくTeraを用いているZolaと似たような使い心地になるよう意識した。

# CI/CD
ScrapsのリリースはGitHub Releasesとcrates-ioを用いて管理している。よって cargo install scraps でインストールをできるようにした

- [crates.io](https://crates.io/crates/scraps)

# SSGのデプロイサポート
GitHub Pagesでのデプロイをサポートすべく、GitHub Actionsのカスタムアクションを用意した。

- [scraps-deploy-action](https://github.com/boykush/scraps-deploy-action)

またカスタムアクションから呼び出すDocker ImageはGitHubリポジトリのPackagesで管理した

- [scraps-image](https://github.com/boykush/scraps-image)

# ドキュメント
ScrapsのドキュメントはScraps自身を用いて作成している。同リポジトリに置いているので機能開発中のデバッグ用もかねている

- [Getting Started - Scraps Doc](https://boykush.github.io/scraps/Getting%20Started.html)

# 終わりに

v0.6.1時点で一通りの機能が揃ったので、実際にScrapsを用いてWikiを作り始めている

- [Kush's Wiki](https://boykush.github.io/wiki/)

我ながら良い使い心地なのでWikiも充実させていきつつ、Scrapsの開発も続けていきたい
