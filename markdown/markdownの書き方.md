# 書き方メモ

## 見出し
```
# 見出し１
## 見出し２
### 見出し３
#### 見出し４
##### 見出し５
```
<details>
  <summary>例</summary>

  # 見出し１
  ## 見出し２
  ### 見出し３
  #### 見出し４
  ##### 見出し５
</details>

## 箇条書き
```
- abc
    - def
      - ghi
      - jkl
        - mno
    - pqr
- 123
    - 456
    - 789
```
※`-`は`*`でもOK
<details>
  <summary>例</summary>

  - abc
      - def
        - ghi
        - jkl
          - mno
      - pqr
  - 123
      - 456
      - 789
</details>

## 箇条書き(番号付き)
```
1. abc
    1. ghi
    1. jkl
        1. mno
1. 123
    1. 456
    1. 789
```
<details>
  <summary>例</summary>

  1. abc
      1. ghi
      1. jkl
          1. mno
  1. 123
      1. 456
      1. 789
</details>

## 書体
```
**太文字**
~~取り消し~~
*斜体*
```
<details>
  <summary>例</summary>
  
  **太文字**  
  ~~取り消し~~  
  *斜体*  
</details>

## 引用
```
> 引用
>> あああ
```
<details>
  <summary>例</summary>
  
  > 引用
  >> あああ
</details>

## コード
一行
```
`echo 'hogehoge';`
```
複数行  
※上の「```」の横に言語名を書くと、シンタックスハイライトされる
````
```php
$a = 'hogehoge';
print $a;
```
````
<details>
  <summary>例</summary>
  
一行  
`echo 'hogehoge';`  
  
複数行
```php
$a = 'hogehoge';
print $a;
```
</details>

## 水平線
```
---
***
```
<details>
  <summary>例</summary>
  
  ***
  ---
</details>

## テーブル
```
|みだしぎょう１|みだしぎょう２|みだしぎょう３|  <- ヘッダ行
|:------------|:----------:|-----------:|  <- 表の文字位置を指定する行
|ひだり       |まんなか     |みぎ         |  <- データ行
```
<details>
  <summary>例</summary>
  
|みだしぎょう１|みだしぎょう２|みだしぎょう３|
|:------------|:----------:|-----------:|
|ひだり       |まんなか     |みぎ         |
</details>

## リンク
```
[google](https://www.google.co.jp)
```
<details>
  <summary>例</summary>
  
  [google](https://www.google.co.jp)
</details>
