#■初期設定

###・新規登録
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

###・リポジトリ作成
```
  $ git ilit	（初期作成：初期ブランチ名〔master〕）
　$ ls -a	(確認)
```
