
# ugcs_jp

ugcs_jpは「UgCS 4.xの日本語リソースを作ろう」というプロジェクトです。

ドローン用の地上管制ソフトウェア(GCS)としては高機能だけれど、日本語化されていないのでユーザーが少ないのがUgCS。

Mission Planner(Ardupilot)やQGroundControl(PX4)の日本語化も進んでいるけれど、
UgCSも頑張って日本語にするぞ～！
 
# デモ

![demo1](https://user-images.githubusercontent.com/55542434/97267392-70ecc880-186d-11eb-98fe-d8ff0804e023.png)

左上の初期メニューだけ日本語化した様子です。

# UgCSとは

UgCSは、DJI，Parrot，Ardupilot，PX4は当然として、
その他様々なメーカーのドローンに対応しているの地上管制ソフトウェア(GCS)です。

オープンソースソフトウェアじゃないので、お値段が少々お高いですが、それを補う程に優秀なソフトウェアです。
https://www.ugcs.com/pricing

しかし、機能がたくさんありすぎて使い方がわからない。
Mission Plannerの英語版も分からなかったけど、更に分からない(T_T

そういうわけで、日本語化してみます。

# 解説
 
UgCSの日本語化は非常に簡単です。

2つのファイル

* ja_JP.po  (日本語
* ja_JP.png (

を所定のディレクトリに置くだけです。

# Installation
 
Requirementで列挙したライブラリなどのインストール方法を説明する
 
```bash
pip install huga_package
```
 
# Usage
 
DEMOの実行方法など、"hoge"の基本的な使い方を説明する
 
```bash
git clone https://github.com/hoge/~
cd examples
python demo.py
```
 
# Note
 
注意点などがあれば書く
 
# Author
 
作成情報を列挙する
 
* 作成者
* 所属
* E-mail
 
# License
ライセンスを明示する
 
"hoge" is under [MIT license](https://en.wikipedia.org/wiki/MIT_License).
 
社内向けなら社外秘であることを明示してる
 
"hoge" is Confidential.
