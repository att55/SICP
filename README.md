## Overview

計算機プログラムの構造と解釈 (Structure and Interpretation of Computer Programs) の Tips リポジトリ。

## Scheme

書内の説明に採用されている言語。
Lisp の方言のひとつで、静的スコープなどが特徴。

### Lisp

高水準プログラミング言語の中でもFORTRANに次いで2番目に古い言語。
これまでに多数の方言が存在してきたが、今日最も広く知られる LISP 方言は、Common Lisp と Scheme。

LISP は、アロンゾ・チャーチのラムダ計算表記法に影響を受け、コンピュータープログラムのための実用的かつ数学的な表記法として作られた。
そして、すぐに人工知能研究に好まれるプログラミング言語になった。
最初期のプログラミング言語として、LISP は計算機科学にて、木構造、ガベージコレクション、動的型付け、条件分岐、高階関数、再帰、セルフホスティング、コンパイラを含む多くのアイディアを切り開いた。

LISP の名前は、「list processor」に由来している。リストは LISP の主要なデータ構造であり、LISP ソースコードはそれ自体がリストからできている。その結果、LISP プログラムはソースコードをデータとして操作することができ、プログラマーは、マクロ・システムで新しい構文や LISP 埋め込みの新しい DSL を作成できる。

## Gauche

https://practical-scheme.net/gauche/index-j.html

Scheme 言語のスクリプトエンジン。 
Scheme プログラムを読み込み、直ちにコンパイルして仮想マシンで実行する。
Scheme 言語の標準である、"Revised^7 Report on the Algorithmic Language Scheme" (R7RS)に準拠している。

### 環境構築

```
$ brew install gauche
```

### 起動方法

```
$ gosh
>gosh (print "Hello World")
Hello World!!
>gosh (exit)

$ echo "(print \"Hello World\!\!\")" > hello.scm
$ gosh -l ./hello.scm
Hello World!!
>gosh (exit)
```
