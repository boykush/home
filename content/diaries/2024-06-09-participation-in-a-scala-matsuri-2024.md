+++
title = "「ScalaMatsuri 2024」に参加・登壇してきた"
date = 2024-06-09
[taxonomies]
tags=["Tech", "Output"]
+++

[ScalaMatsuri 2024](https://scalamatsuri.org/ja)に参加・登壇してきた

Xのハッシュタグは `#ScalaMatsuri`

終始タイムラインも賑わっていてとても楽しかった。

コロナ前ぶりの完全オフライン開催、ということでアフターパーティ等で人との繋がりも強く感じられとても濃い2日間となった（トレーニングデイ含めると3日間

## 「Introduction to safe programming with numeric library」 登壇振り返り
発表資料は以下

<iframe class="speakerdeck-iframe" frameborder="0" src="https://speakerdeck.com/player/a5a88a998b7643eba1bd728a75d1042a" title="Introduction to safe programming with numeric library / 数値ライブラリで始める安全なプログラミング" allowfullscreen="true" style="border: 0px; background: padding-box padding-box rgba(0, 0, 0, 0.1); margin: 0px; padding: 0px; border-radius: 6px; box-shadow: rgba(0, 0, 0, 0.2) 0px 5px 40px; width: 100%; height: auto; aspect-ratio: 560 / 419;" data-ratio="1.3365155131264916"></iframe>

概要として、[typelevel/spire](https://github.com/typelevel/spire)という数値ライブラリの中から主に有理数（Rational）型を使って、数値誤差のない安全な料金計算を行う。という内容

普遍的な数値誤差の話題についてだったので、普段関わらない界隈の人からもリアクションをもらえて嬉しかった。
たまたま業務で触っていた内容の紹介で正直題材に恵まれたが、しっかり勉強して20分発表しきれたのでやりきった。

発表内容は事前に社のチームの人に共有し、内容・英語に関してFBをもらうことができた。とてもありがたい。

また初のカンファレンス登壇だったが、ScalaMatsuriの運営はとてもかっちりとしていて万全のサポートをしていただいた。
そのおかげで安心して登壇に臨むことができスタッフの方々にとても感謝。

## 個人的にキャッチアップしたいセッション
[プログラム一覧](https://scalamatsuri.org/ja/programs)

全体として興味深いセッションが並んでいて、かつまとまり・バランスがよいプログラムであったように感じた

個人的に興味を持った技術的な話題を抽出すると以下
- [com.lihaoyi](https://github.com/com-lihaoyi)エコシステム
- [scala-cli](https://scala-cli.virtuslab.org/)ツール
- [Ox](https://github.com/softwaremill/ox)

どれも取りかかりやすいイメージを持ち、Scala3 + 上記のライブラリ・ツール群であればちょっとした開発をするときにハードル低くScalaを使えるなと思った。

その他、個人的に内容が親和性が高く
