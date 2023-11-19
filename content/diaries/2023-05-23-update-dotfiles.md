+++
title = "dotfilesをupdateした"
date = 2023-05-23
[taxonomies]
tags=["Tech"]
+++

# はじめに

最近dotfilesを整理して開発環境をアップデートしていた。備忘録的にリンク等を残す。

# CUI・TUIツールの整理
これまで色々なツールを入れてきたが結局使わずにいたツールも多かった。ので頻繁に使っているコマンドだけになるよう整理した。

愛用しているのは以下のツール群

- [bat](https://github.com/sharkdp/bat)
- [exa](https://github.com/ogham/exa)
- [fzf](https://github.com/junegunn/fzf)
- [gitui](https://github.com/extrawurst/gitui)
- [git-delta](https://github.com/dandavison/delta)
- [ripgrep](https://github.com/BurntSushi/ripgrep)
- [starship](https://github.com/starship/starship)
- [zoxide](https://github.com/ajeetdsouza/zoxide)

有名どころが多いので説明は省略する。fzfの代替とな[skim](https://github.com/lotabout/skim)はどうなんだろう。また調べてみたい。

# ターミナルマルチプレクサをZellijへ移行
ターミナルはAlacrittyを使っているが、tmuxから[Zellij](https://github.com/zellij-org/zellij)へターミナルマルチプレクサの環境を大きく変えた。

気分転換がてらといった感じで大きな意思はないけれど、前評判通りユーザーフレンドリーなUIのおかげで不自由なく使っている。

tmuxに比べてショートカットのタイプ数は増えたが、シンプルよりイージーを優先したインターフェースという印象で個人的には好き。

# Neovimのlua化
長らくさぼって後回しにしていたがついにlua化を行なった。オプション設定は引き継ぎつつプラグインはlua製へと置き換えた。


最近はIntellijに頼りきっているのもあって、補完系プラグインはまだ入れていないけれど。

採用したプラグイン一覧は以下

- [packer.nvim](https://github.com/wbthomason/packer.nvim)
- [nvim-tree](https://github.com/nvim-tree/nvim-tree.lua)
- [telescope.nvim](https://github.com/nvim-telescope/telescope.nvim)
- [lualine.nvim](https://github.com/nvim-lualine/lualine.nvim)
- [bufferline.nvim](https://github.com/akinsho/bufferline.nvim)
- [gitsigns.nvim](https://github.com/lewis6991/gitsigns.nvim)
- [nvim-autopairs](https://github.com/windwp/nvim-autopairs)

luaファイルを役割別に分割しやすくなっていて良い、分け方はこんな感じ。

```
❯ tree
.
├── init.lua
└── lua
    ├── core-colorscheme.lua
    ├── core-keymappings.lua
    ├── core-options.lua
    ├── core-plugin-manager.lua
    ├── plugin-bufferline.lua
    ├── plugin-gitsigns.lua
    ├── plugin-lualine.lua
    ├── plugin-nvim-autopairs.lua
    ├── plugin-nvim-tree.lua
    └── plugin-telescope.lua
```

# カラースキームを一律Nordに変更
これまでMaterial DesingのColorを使っていたが、ターミナルからIDEまで一律で[Nord](https://www.nordtheme.com/)にスキームを変更した。

[Arctic Ice Studio](https://github.com/arcticicestudio)が出している他のリポジトリも気になる。

フォントは変わらず[Hack](https://github.com/source-foundry/Hack)を使っている。

# おわりに
他にもdotfilesではないけれども、本ホームページのZola Themesを[simple-dev-blog](https://github.com/bennetthardwick/simple-dev-blog-zola-starter)から[apollo](https://github.com/not-matthias/apollo)に変えたりと、身の回りの整理をしていた。

普段はエンジニアという職種で課題解決を軸に難しいことを考えながらサービスを提供する側だけれど、たまには何も考えずにツールの利用側になるのも大事だなと感じた。

備忘録として残しておく。
