ターミナル(Gitの操作を行うツールの)コマンド
```
・cd ディレクトリを移動する。
   (例:cd ~/Documents/my_udemy_code/git_tutorial )

・ls ディレクトリの内容を表示する。
   (例: ls)

・mkdir 新規ディレクトリの作成する。
   (例: )

・rm ファイル削除する。
   (例:git rm --cached index.html)--cachedオプショ
ンで、インデックスのみ削除し、作業ツリーにファイル
を残す事ができる。

・cp ファイルコピーする。

・ファイル作成
　　(例:$ touch <ファイル名>)

・mv ファイルの移動or名前変更する。
   (例:git mv index.html index2.html)名前変更
理由は、git mv が

　　『	$ mv oldname newname
	$ git add newname
	$ git rm oldname	』
					が省略形

・cat ファイルの中身を表示する。
   (例:cat ファイル名)
```


ファイル
```
・作成
  $ touch <ファイル名>
```


ブランチ
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
