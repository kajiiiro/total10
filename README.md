# make 10 / 10 puzzle

高速道路を走っていて、暇な時にするあれです。
前を走る車のナンバーを10にするあれです。

## ルール

数々のローカルルールがあるかとは思いますが、
ここでは以下のルールを用いるものとします。

* 4桁のナンバーに対応
* ナンバーの数値でない部分は0として考える
* 先頭が0の場合はそのまま利用しなければならない
* 利用できる演算子は以下
  * +
  * -
  * /
  * *
  * ()
* 符号の反転はあり
  * ()と符号の反転がありになることから計算順序はある程度自由となります
* 数字の順番は入れ替えできない
  * wikipediaでは入れ替えられないルールの方がメジャーなようです
  * ですが、偶然の数字の並びをそのまま楽しみたいですよね

## 利用方法

コマンドで以下を実行する。

~~~sh
$ node index.js
[計算対象の4桁の数値] [合計値:基本的に10] result:[カンマ区切りの計算文字列]
~~~

## 結果確認

~~~sh
$ echo "[計算文字列]" | bc
10
~~~


