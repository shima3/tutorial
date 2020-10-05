# Git tutorial

## インストール

Git for Windowsのページでインストーラーをダウンロードし、実行する。
http://msysgit.github.io/

## 初期設定

以下のコマンドを実行する。

    $ git config --global user.name "<GitHubでのユーザ名>"
    $ git config --global user.email "<GitHubでのメールアドレス>"

## リポジトリの作成

    $ mkdir intro
    $ cd intro
    $ git init

## バージョン管理する対象ファイルの登録

テキストエディタでREADME.mdファイルに紹介文を保存してから次のコマンドを実行する。

    $ git add README.md

## 変更のローカルリポジトリへの記録

    $ git commit -m "<コメント>"

<コメント>にはコミットした内容を書く。
後から見た時に何が変更されたか分かるようなコメントが良い。

## コミットし忘れの確認

    $ git status
    # On branch master
    nothing to commit (working directory clean)

## 変更履歴の確認

    $ git log
    commit bd5cf3a110ad28bc690aac579c3f55069f0df965
    Author: tester <test@esd.info.hiroshima-cu.ac.jp>
    Date:   Tue May 27 11:07:38 2014 +0100

    ほげほげ

## リモートリポジトリへのアップロード

ローカルリポジトリの内容をリモートリポジトリに反映する操作をプッシュと呼ぶ（ファイルでいうアップロードと同じと思えばよい）。

## 参考

サルでもわかるGit入門
http://www.backlog.jp/git-guide/

git勉強内容まとめ9(GitHubを利用した開発手順メモ)
http://nwpct1.hatenablog.com/entry/2014/01/13/115232

いまさら聞けないgitの使い方
http://qiita.com/mountcedar/items/682743c95fd3b8fc274b

Git - 公式
http://git-scm.com/

Git for Windows
http://msysgit.github.io/
