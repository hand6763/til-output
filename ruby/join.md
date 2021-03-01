# joinメソッド
配列の要素を結合して１つの文字列としたい場合に使われる  
配列の各要素を文字列に変換し、引数を区切り文字として結合する

## 使い方
```
array = ["abc", "def", "ghi"]

puts array.join  #abcdefghi と出力される
```

```
array = ["abc", "def", "ghi"]

puts array.join(",")  #abc, def, ghi と出力される
```