naobin
======

grepdf
======
PDFの中身をgrepするスクリプトです．

pdftotextでテキスト変換してからgrepするので，pdftotextできないようになっているPDFには対応していません．
また，数式などは正しく認識できない場合もあります．
現時点ではスクリプトを実行したディレクトリだけしか検索しないので，
ディレクトリ間を再帰的に検索はできません．

検索したい文字列を引数に入れてください．

現時点では引数は1つだけにしか対応していません．

Example)
./grepdf.sh hoge.pdf


light
======
ノートPCの画面の明るさを調整するためのスクリプトです
標準に搭載されているものやxbacklightを利用しても調整できないときに
使用してください

使用方法はxbacklightコマンドに合わせています
一度getオプションを実行して、現在の明るさを取得してから
少しずつ明るさを落として調整してください

 -get       : 現在の明るさを取得する

 -set [num] : 明るさを指定する

Example)
./light -get
sudo ./light -set 300
