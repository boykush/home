+++
title = "タスク管理をGitHub Projectsに統合した"
date = 2023-11-19
[taxonomies]
tags=["Operation"]
+++

ホームページ・OSSライブラリ等のリポジトリでIssueを運用しつつ、他の読書記録等のタスクも一箇所で扱いたくなったのでGitHub Projectsに統合した。

GitHub ProjectsはIssueの自動追加やステータス同期等の最小限のワークフローを備えていて便利。

読書記録はNotionで行っていたものをIssueへと移行した。リポジトリは以下

[boykush/bookshelf](https://github.com/boykush/bookshelf)

IssueのTODOに各章を列挙しチェックをつけていくことで読書の進捗もわかる。

読書記録程度だったらNotionのようなデータベースではなく、Issue templateで記録しやすくなっている程度で個人的に十分。

IssueだったらGitHub Actionsとの接続もできるし、便利なところは使っていきたいですね。
