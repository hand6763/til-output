# 条件分岐
## scanf関数
```
scanf("%d",&a);
```
キーボードから文字列を入力する際に用いる関数  
整数型変数aに値を入れるには、先頭に&(アンパサント)をつけ、"で囲まれた部分には、%dと記入

### 複数のパラメータの入力も可能
```
#include <stdio.h>
 
void main(){
    int a, b;
    scanf("%d %d", &a, &b);     //  複数のパラメータの入力を受け付ける。
    printf("入力された値：%d %d¥n", a, b);
}
```
実行結果
```
1 2 ← 間をスペースで区切って入力。
入力された値：1 2
```

### スキャン集合指定子
文字・文字を入力する際には、入力するデータの値を限定することが可能
```
#include <stdio.h>
 
void main(){
    char s[32] = "";
    printf("abcのいずれかを入力:");
    scanf("%[abc]", s);
    printf("入力された値 = %s¥n", s);
    return 0;
}
```
abcのいずれかの値が入力された場合
```
abcのいずれかを入力:a
入力された値 = a ← 入力された値が出力される。
```
abc以外の値が入力された場合
```
abcのいずれかを入力:k
入力された値 =  ← 何も出力されない。
```


逆に、入力を受け付けない文字を指定することも可能
```
#include <stdio.h>
 
void main(){
    char s[32] = "";
    printf("abc以外のいずれかを入力:");
    scanf("%[^abc¥n]", s);
    printf("入力された値 = %s\n", s);
    return 0;
}
```

## if文
比較演算子
| 演算子 | 内容 |
----|---- 
| >= | 以上 |
| <= | 以下 |
| != | 等しくない |

論理演算子
| 演算子 | 内容 |
----|---- 
| && | AND |
| || | OR |
| ! | NOT |

### if~else文
```
if(条件式){
    処理①
}else{
    処理②
}
```

### else if文
```
if(条件式①){
    処理①
}else if(条件式②){
    処理②
}else{
    処理③
}
```

## switch文
else ifを用いた多数に分岐する条件分岐は、値が整数値であれば、switch(スイッチ)文を用いて以下のように書くことができる
```
#include <stdio.h>
 
void main(){
    int num;
    printf("1～3の値を入力してください：");
    //  キーボードから整数を入力
    scanf("%d",&num);
    //  入力した値が、正の数かどうかを調べる
    switch(num){
        case 1:
            printf("one¥n");    //  numが1だった場合の処理
            break;
        case 2:
            printf("two¥n");    //  numが2だった場合の処理 
            break;
        case 3:
            printf("three¥n");  //  numが3だった場合の処理 
            break;
        default:
            printf("不適切な値です。¥n"); //  それ以外の値が入力された場合の処理
            break;
    }
}
```


