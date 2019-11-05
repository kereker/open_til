# GitHub〜まとめ〜

## ■はじめに
```
    このページはGitの使い方を初心者なりにまとめたページです。
    主にターミナル作業の内容
```
## ■ターミナル(Gitの操作を行うツールの)コマンド
```
・cd ディレクトリを移動する。   ※ディレクトリ≒フォルダ
   (例:cd ~/Documents/my_udemy_code/git_tutorial )

・ls ディレクトリの内容を表示する。
   (例: ls)

・mkdir 新規ディレクトリの作成する。(今いるディレクトリの中に)
   (例:mkdir git_tutorial)

・rm ファイル削除する。
   (例:git rm --cached index.html)
        --cachedオプションで、インデックスのみ削除し、作業ツリーにファイルを残す事ができる。

・cp ファイルコピーする。

・touch ファイル作成
　　(例:$ touch <ファイル名>)

・mv ファイルの移動or名前変更する。
   (例:git mv index.html index2.html)名前変更
理由は、git mv が　　『	$ mv oldname newname
　　　　　　　　　　　　  $ git add newname
	                $ git rm oldname	』  	が省略形となるため

・cat ファイルの中身を表示する。
   (例:cat ファイル名)
```

## ■初期設定

### 新規登録
```
  $ git config --global user.name "<GitHubでのユーザー名>"
  $ git config --global user.email "<GitHubでのメアド>"
  $ git config --global core.editor "<エディタを設定する>"

　　・登録の確
    $ git config user.name    (登録されたユーザー名)
    $ git config user.email   (登録されたメアド)
    $ git config core.editor  (登録されたエディタ)
    $ git config -list        (登録されているデータ)


    $ cat ~/.gitconfig
```


## ■リポジトリ
```
    ファイルやディレクトリの状態を記録する場所です
```
### リポジトリ作成
```
  $ git ilit	（初期作成：初期ブランチ名〔master〕）
　$ ls -a	(確認)
```
### リモートリポジトリ
```
    専用のサーバに配置して複数人で共有するためのリポジトリ
```
```
    ・リモートリポジトリ作成(追加)
     $ git remote add <新規リモートリポジット名> <設定したいリポジトリのURL>
    
    ・保存されているリポジトリ名表示
     $ git remote

    ・保存されているリポジトリ名表示 + URL(fetch + push)
     $ git remote -v
```
## ■ブランチ
```
・一覧表示(存在する自分の全てのブランチ)
　$ git branch

・作成　
　$ git branch <新規ブランチ名>

・移動
  $git checkout <ブランチ名>

・作成+移動
　$git checkout -b <新規ブランチ名>

　～オプション～　
 　-d 削除（非強制）
　 -D 削除（強制）
```

## ■プルリクエスト
```
    ①masterブランチを最新情報に更新
     $ git pull <リモートリポジット名> master

    ②ブランチ作成(+移動)
     $git checkout -b <新規ブランチ名>

    ③ファイル編集
     ターミナルを開き編集したいファイルを開き編集する。
    
    ④コミット
     $git add <ファイル名>
     $git commit <ファイル名>>
    
    ⑤GitHubへプッシュ
    　$ git push <リモートリポジット名> master

    ▼⑥~⑧はGitHubでの作業
    ⑥プルリクエストを送る
    ⑦コードレビュー
    ⑧プルリクエストをマージ

    ⑨ブランチ削除
     $git branch -D <ブランチ名>
```



# ★参考サイト

[サルでもわかるGit入門〜バージョン管理を使いこなそう〜](https://backlog.com/ja/git-tutorial/)

[Qiita～エンジニアリングに関する知識を記録・共有するためのサービスサイト～](https://qiita.com/search?utf8=%E2%9C%93&sort=&q=Git+)

