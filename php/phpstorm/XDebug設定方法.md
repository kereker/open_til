# XDebug設定方法

## 1.XDebugインストール

(※本記事ではJetBrains PhpStorm 2019.2.3バージョンによる記載です)  

* php_xdebug-2.8.0-7.3-vc15-x86_64.dll(アプリケーション拡張)」ダウンロード
  * [XDebugダウウンロード](https://xdebug.org/download)

* C:\xampp\php\extに貼り付け  
 ![画像1](img/gazo1.PNG)

## 2.Phpstormの設定  

 ![画像2](img/gazo2.PNG)

* 構成の編集をクリック  
 ![画像3](img/gazo3.PNG)
* ＋をクリック
* PHP Remote Debugを選択
* 名前:任意（ここではXAMPP）
  
* IDEキーでデバッグ接続をフィルターするにチェック入れる  
* サーバ：「...」を選択する
  * 名前:任意（ここではXAMPP）
  * ホスト：127.0.0.1
  * デバッカー：Xdebug
  * 「OK」ボタン押下
* ideキー（セッション id）:
  * PHPSTORMを記述
  * 「OK」ボタン押下
  
## 3.XAMPPの設定

* PHP（php.ini）を選択  
 ![画像4](img/gazo4.PNG)  
* 下記の記述を追加↓  
  
```bash
[XDebug]  
zend_extension = "c:\xampp\php\ext\php_xdebug-2.8.0-7.3-vc15-x86_64.dll"  
xdebug.remote_autostart = 1  
xdebug.profiler_append = 0  
xdebug.profiler_enable = 0  
xdebug.profiler_enable_trigger = 0  
xdebug.profiler_output_dir = "c:\xampp\tmp"  
xdebug.remote_enable = 1  
xdebug.remote_handler = "dbgp"  
xdebug.remote_host = "127.0.0.1"  
xdebug.remote_log="c:\xampp\tmp\xdebug.txt"  
xdebug.remote_autostart = 1  
xdebug.remote_port = 9000  
xdebug.trace_output_dir = "c:\xampp\tmp"  
xdebug.remote_cookie_expire_time = 36000  
xdebug.idekey = "PHPSTORM"  
```

（注意） xdebug.idekey = "PHPSTORM" と Phpstormの設定のideキーの記述名を一致させる

## 4.XDebugの起動確認

※phpinfo()の実行結果を見るだけのPHPファイルを用意する

* localhostサーバを立ち上げ、XDebugがあることを確認（検索かけると良い）  
 ![画像5](img/gazo5.PNG)

### -備考-

本記事とバージョンが違う方は下記のリンク先も合わせて参照してください  

[違うバージョンの方へ！](https://qiita.com/hitotch/items/7b2895f9822ded3fa7db)  
