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

# 「数値ライブラリで始める安全なプログラミング」 登壇振り返り
発表資料は以下

<iframe class="speakerdeck-iframe" frameborder="0" src="https://speakerdeck.com/player/a5a88a998b7643eba1bd728a75d1042a" title="Introduction to safe programming with numeric library / 数値ライブラリで始める安全なプログラミング" allowfullscreen="true" style="border: 0px; background: padding-box padding-box rgba(0, 0, 0, 0.1); margin: 0px; padding: 0px; border-radius: 6px; box-shadow: rgba(0, 0, 0, 0.2) 0px 5px 40px; width: 100%; height: auto; aspect-ratio: 560 / 419;" data-ratio="1.3365155131264916"></iframe>

概要として、[typelevel/spire](https://github.com/typelevel/spire)という数値ライブラリの中から主に有理数（Rational）型を使って、数値誤差のない安全な料金計算を行う。という内容

普遍的な数値誤差の話題についてだったので、普段関わらない界隈の人からもリアクションをもらえて嬉しかった。
たまたま業務で触っていた内容の紹介で正直題材に恵まれたが、しっかり勉強して20分発表しきれたのでやりきった。

発表内容は事前に社のチームの人に共有し、内容・英語に関してFBをもらうことができた。とてもありがたい。

また初のカンファレンス登壇だったが、ScalaMatsuriの運営はとてもかっちりとしていて万全のサポートをしていただいた。
そのおかげで安心して登壇に臨むことができスタッフの方々にとても感謝。

# 個人的に理解が進んだセッション
[プログラム一覧](https://scalamatsuri.org/ja/programs)

全体として興味深いセッションが並んでいて、かつまとまり・バランスがよいプログラムであったように感じた

興味を持った技術的な話題を抽出すると以下
- [com.lihaoyi](https://github.com/com-lihaoyi)エコシステム
- [scala-cli](https://scala-cli.virtuslab.org/)ツール
- [Ox](https://github.com/softwaremill/ox)

どれも取りかかりやすいイメージを持ち、Scala3 + 上記のライブラリ・ツール群であればちょっとした開発をするときにハードル低くScalaを使えるなと思った。

その他、個人的に親和性が高く理解が進んだセッションについて

## [Scala ビルド時間の最適化](https://scalamatsuri.org/ja/programs/SESSION_DAY_2_01)
sbtのようなビルドツールの中で、sbt,Zinc,scalacのレイヤがどのような役割を持ちビルドがされているか、そしてどう拘束かに取り組んでいるか、わかりやすく紹介がされていた。

こうゆうふうにサブプロジェクトやファイルを分けるとビルド早くなるよ〜といったように、ビルド高速化の勘所が分かりよかった。

直近のビルド高速化リリースタイムラインも紹介され、ミッションをやりきってリリースまで持っていく執念のようなものを感じた。とてもすごいと思ったし自分もそうありたい。

## [作って学ぶ Extensible Effects](https://scalamatsuri.org/ja/programs/SESSION_DAY_2_04)
発表資料は以下

[Google Doc](https://docs.google.com/presentation/d/1raybiE8Otk2nreKDyRHoF1HK50K9K-fjL8-37QK8kW4/edit?usp=sharing)

こちらは個人的に業務でatnos-effライブラリを使っていることもあり、ライブラリを内部を理解できるよう意気込んでいたセッション

そういった背景で発表全体をやんわりとは理解できたが、サンプルコードの一行一行までは理解がおよんでいないので後でゆっくり見返したい。

atnos-effライブラリで似たような内部実装を見かけた気がする（特にトランスパイルのあたり）ので、ライブラリとも比較しながら読み込むのが良さそう。

Effは個人的にとても大好きなので、今後ともしっかり付き合っていきたい。

# まとめ
個人的な話になるが、新卒で社会人になったのと同時にコロナに突入した代なのでオフラインカンファレンスはなにもかもがわくわくして参加できた。

発表者の顔を直接見ながら発表を聞くのは、オンラインイベントでは感じられない熱・執念のようなものを強く感じ、一気にコロナ前の社会に戻った感覚があった。

ScalaMatsuriは国際カンファレンスなので、登壇者含め多くの外国の方が参加していた。スピーカーディナーや懇親会での英語での会話はとても刺激になった。（僕はまともに話せてないけど

まずはこのブログに書いたキャッチアップ、そして1年後までにまともな英会話力！

改めて、運営スタッフの方々、登壇者の方々、一緒に場を共有できた参加者の方々、ありがとうございました。
