MyConfig
========
### 初期設定 

./setup.sh

- diff-highlightの設定
```
chmod +x diff-highlight
sudo mv diff-highlight /usr/local/bin/diff-highlight
```

### 一つずつ設定する
#### ゆろよろさんのブログにしたがって実行（参考1)

```
git clone https://github.com/yuroyoro/dotfiles.git
cd dotfiles
./setup.sh
```
※　setup.shでは、各設定ファイルへのシンボリックリンクを生成するのですが、すでにファイルが存在する場合はlnコマンドが失敗するので、その場合は適宜対処してください。

対処法：（非推奨）

```
ls -la | grep dotfiles | xargs rm 
```


以下　参考URL１通りやる。

#### oh-my-zshを導入

(参考4)(参考5)通りにやればよい。themeは“dallas”

.zshrcをホームディレクトリにコピー


#### neobundle を導入

neobundleのGithubからマニュアル通りにneobundleをいれる

#### tmuxを導入
tmuxの footerのカラースキームを変更（参考6）

tmux の設定でmemを扱うときに（参考6)が必要

tmux のマウスの設定（参考8）  

.tmux.confを自分のホームディレクトリに入れる

#### vimの設定
vim設定ファイルをとってこればok          

.vimrc を自分のホームディレクトリに入れる

powerlineのキャッシュがのこっている場合は（参考9）

#### gitの設定
(参考10)の通りにやればよい


### 参考URL
1. yuruyoro http://d.hatena.ne.jp/tetsuyai/20111202/1325038360
2. neobundle https://github.com/Shougo/neobundle.vim
3.  oh-my-zsh http://mollifier.hatenablog.com/entry/20101009/p1
4. oh-my-zsh一覧　     
5. oh-my-zsh sample https://github.com/robbyrussell/oh-my-zsh これでthemeでdallasを選択
6. tmux http://materia.jp/blog/20120301.html
7. tmux:memory http://yonchu.hatenablog.com/entry/2013/02/01/231646　
8. mouse の設定 http://qiita.com/u1tnk/items/9a680d16065217015e16
9. vim power line cache https://github.com/Lokaltog/vim-powerline
10. gitの設定　http://qiita.com/tailak/items/eadd0fb6169efe96ff7e
