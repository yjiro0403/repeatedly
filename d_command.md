D言語を最近始めた自分が使うかもしれないコマンドをメモ
##入力
文字列を受け取り、0番目の数字を数値に変換して受け取る(複数受け取りたい場合はスペースで区切る).  

以下をインポート：
```d
import std.stdio; //readln  
import std.array; //split
import std.conv //to
```

```d
string[] input = readln().split;  
int num = input[0].to!int;
```

//文字列を受け取る→受け取った複数の数字を数値に変換して配列に格納    
int a[] = readln().split.map!(to!int).array;