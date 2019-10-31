# XAMPP設定

・右上の**Config**ボタン押下

![画像](img/XAMMP%E3%82%B3%E3%83%B3%E3%83%88%E3%83%AD%E3%83%BC%E3%83%AB%E3%83%91%E3%83%8D%E3%83%AB.PNG)

・**Service and Port Settings**ボタン押下

![画像](img/XAMMP2.PNG)

・MySQLタブで Main Portに3309を記述する

![画像](img/XAMMP3.PNG)

・**save**ボタン押下

・MySQLの**Config**ボタン押下---my.iniクリック

  
![画像](img/XAMMP4.PNG)
  
・port = 3309に変更(2か所)

![画像](img/XAMMP5.PNG)

・C:\xampp\phpMyAdmin\config.incより

　29行目の記述を追加する

![画像](img/XAMMP6.PNG)

・実際にPHPとMySQLを連携する際に必要な構文

![画像](img/XAMMP7.PNG)
