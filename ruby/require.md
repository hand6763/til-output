# requireの使い方

外部ファイルの読み込みができる

## require関数とは
標準ライブラリや、gemでインストールしたライブラリ、自分で書いたコードからソースコードを読み込む関数。これにより、ライブラリに定義されたクラスやメソッドが利用できるようになる。

## require関数の使い方
標準ライブラリーやインストールしたライブラリーから使用する時  
```
require"ライブラリー名"
```

自分で書いたコードを読み込む場合
```
require"./path/to/file"
```
.rbの拡張子はいらない

## 実践
ruby/requireファイルを参照