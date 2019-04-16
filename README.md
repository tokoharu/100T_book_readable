# 100T_book_readable


## ツリーの読み方
次のような行が並んでいます
```
+- NONE,69,0,lnsgkgsnl/1r5b1/ppppppppp/9/9/9/PPPPPPPPP/1B5R1/LNSGKGSNL b - 1
    +- ２六歩[２七],-69,0,lnsgkgsnl/1r5b1/ppppppppp/9/9/7P1/PPPPPPP1P/1B5R1/LNSGKGSNL w - 2
```
左から、指し手（前いた場所）, 評価値, 評価値のズレの合計,局面(SFEN形式),を表します。

「評価値のズレの合計」とは、かいつまんで説明すれば、最適な応手からの離れ具合を表現するものです。
具体的には、最善でないとされる指し手を選んだ際に、最善とされる指し手との評価値の差を順次加算していくものです。
したがって、0であれば最善手（もしくはその一つ）です。

### normal_tree
ここにあるツリーは、30,100と名前を付けています。それぞれ、上記に説明のある「評価値のズレの合計」が30以内、または100以内の局面のみを載せ、残りを記載していないツリーです。

30を見るとかなりサイズは小さいのですが、多くの局面が最適とされる手順に関するものになっていることがわかります。
評価値の差が1のものを探したい場合には",1,"のような形で検索するのがよいかと思います。
