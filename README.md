# cli-debug
```
How to DEBUG

実行前のブレークポイント設定
ZB エントリ名:フラグ  (例>ZB ^TEST1:"L")

フラグ
"S"   コマンド単位　STEP/OVER
"S+"  コマンド単位　 STEP/INTO
"L"   行単位　STEP/OVER
"L+"  行単位　 STEP/INTO

実行方法
普通に起動する。すなわち 
Do エントリ名 (例>Do ^TEST1)

STEP方法
G　[RET]

コマンド単位実行
途中でコマンド単位のSTEP/INTOに変更する
B "S+"

途中でコマンド単位のSTEP/OVERに変更する
B "S"

Break設定を解除する
B "S-"

行単位実行
途中でSTEP/INTOに変更する
B "L+"

途中でSTEP/OVERに変更する
B "L"

Break設定を解除する
B "L-"

途中でSTEP/OUTする
B "C"

```