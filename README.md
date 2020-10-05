# tutorial

## インストール

Git for Windowsのページでインストーラーをダウンロード、実行。
http://msysgit.github.io/

## 初期設定==

以下のコマンドを打ち込む

  $ git config --global user.name "<gitで使用するユーザ名>"
  $ git config --global user.email "<gitで使用するメールアドレス>"

==リポジトリの作成==
*リポジトリを作成したいディレクトリに移動し、コマンドを実行（例：gittestというリポジトリを作成）
===コンソール===
<syntaxhighlight lang="bash">
$ mkdir gittest
$ cd gittest
$ git init
Initialized empty Git repository in /Users/yourname/Desktop/gittest/.git/
</syntaxhighlight>

==ファイルをリポジトリに追加==
*ファイルのリポジトリのインデックスに追加する。注意：この作業は一度だけ（更新とは違うことを理解）
<syntaxhighlight lang="bash">
$ git add <追加したいファイルの名前>
</syntaxhighlight>

==変更をコミットする==
変更した部分を反映するには「コミット」という操作を行う（"commit"=「捧げる」という意味の英単語）。
<syntaxhighlight lang="bash">
$ git commit -m "<コメント>"
</syntaxhighlight>
<p>既に登録はしてあるので、再度ファイルを指定する必要がないことに注目。</p>
<p>コメント部分にはコミットした内容を書く。後から見た時に何が変更されたか分かるようなコメントを残す。</p>

===コミットし忘れを確認===
statusコマンドでコミットのし忘れがないか確認できる。
<syntaxhighlight lang="bash">
$ git status
# On branch master
nothing to commit (working directory clean)
</syntaxhighlight>

===変更履歴の参照===
リポジトリの変更履歴（＝何をコミットしたか）を確認するには、logコマンドを使用する
<syntaxhighlight lang="bash">
$ git log
commit bd5cf3a110ad28bc690aac579c3f55069f0df965
Author: tester <test@esd.info.hiroshima-cu.ac.jp>
Date:   Tue May 27 11:07:38 2014 +0100

    てすとなう

</syntaxhighlight>

==プッシュ==
ローカルリポジトリの内容をリモートリポジトリに反映する操作をプッシュと呼ぶ（ファイルでいうアップロードと同じと思えばよい）。

==参考==
*[http://www.backlog.jp/git-guide/ サルでもわかるGit入門]
*[http://futurismo.biz/archives/824 Cygwinでgitkが使えないときの対策メモ]
*[http://nwpct1.hatenablog.com/entry/2014/01/13/115232 git勉強内容まとめ9(GitHubを利用した開発手順メモ)]
*[http://qiita.com/mountcedar/items/682743c95fd3b8fc274b いまさら聞けないgitの使い方]

==外部リンク==
*[http://git-scm.com/ Git] - 公式。
*[https://github.com/ GitHub]
*[http://msysgit.github.io/ Git for Windows]。
*[https://code.google.com/p/tortoisegit/ TortoiseGit]。
