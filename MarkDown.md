# 見出し
# 見出しh1
## 見出しh2  
シャープの数だけ文字が小さくなる


# 段落
段落1

段落2  
空白行を挟むことで段落となります。


# br改行
hoge
fuga  
piyo  
fugaの後ろに空白スペース2つで改行


# Blockquotes 引用
> 引用  
> 引用
>> 多重引用  

先頭に>を記述します。ネストは>を多重に記述します。


# Code
```
print 'hoge'
```
`バッククオート` 3つ、あるいはダッシュ~３つで囲みます。


# インラインコード
これは `インラインコード`です。  
`バッククオート` で単語を囲むとインラインコードになります。


# Hr 水平線
hoge
***
hoge
___
hoge
---
アンダースコア_ 、アスタリスク*、ハイフン-などを3つ以上で水平線になります。


# ulリスト
- リスト1
    - リスト1_1
        - リスト1_1_1
        - リスト1_1_2
    - リスト1_2
- リスト2
- リスト3  
ハイフン-、プラス+、アスタリスク*のいずれかを先頭に記述します。  
ネストはスペースで表現します。


# Ol 番号付きリスト
1. 番号付きリスト1
    1. 番号付きリスト1-1
    1. 番号付きリスト1-2
1. 番号付きリスト2
1. 番号付きリスト3  
番号.を先頭に記述します。ネストはスペースで表現します。  
番号は自動的に採番されるため、すべての行を1.と記述するのがお勧めです。


# Link リンク
[Google](https://www.google.co.jp/)  
[表示文字](URL)でリンクに変換されます。


# 強調
## em
これは *イタリック* です  
これは _イタリック_ です  
アスタリスク*もしくはアンダースコア_1個で文字列を囲みます。

## strong
これは **ボールド** です  
これは __ボールド__ です  
アスタリスク*もしくはアンダースコア_2個で文字列を囲みます。

## em + strong
これは ***イタリック＆ボールド*** です  
これは ___イタリック＆ボールド___ です  
アスタリスク*もしくはアンダースコア_3個で文字列を囲みます。


# images 画像
![alt](cat-5605615_1920.jpg)
![代替文字列](cat-5605615_1920.jpg "タイトル")

<img src="cat-5605615_1920.jpg" alt="cat-5605615_1920" title="attach:cat" width="200" height="200">
先頭の!で画像と認識されます。画像の大きさなどの指定をする場合はimgタグを使用します。


# Table 表
| TH1 | TH2 |
----|---- 
| TD1 | TD3 |
| TD2 | TD4 |  
-と|を使ってtableを作成します。  
| 左揃え | 中央揃え | 右揃え |
|:---|:---:|---:|
| 1 | 2 | 3 |  
:で揃える位置を変更できます。


# 取り消し線
~~取り消し文字列~~  
~~で囲むと取り消し線になります


# チェックリスト
- [ ] not checked
- [x] checked