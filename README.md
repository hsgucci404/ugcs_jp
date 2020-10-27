
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
その他様々なメーカーのドローンに対応している地上管制ソフトウェア(GCS)です。

オープンソースソフトウェアじゃないので、お値段が少々お高いですが、それを補う程に優秀なソフトウェアです。
https://www.ugcs.com/pricing

しかし、機能がたくさんありすぎて使い方がわからない。

Mission Plannerの英語版も分からなかったけど、更に分からない(T_T

そういうわけで、日本語化してみます。

# 解説
 
UgCSの日本語化は非常に簡単です。

2つのファイル

* ja_JP.po　　(Unityの日本語リソースファイル)
* ja_JP.png　(日本の国旗)

を所定のディレクトリに置くだけです。

# インストール方法

Windows版しか試しておりませんので、Windowsのインストール方法を書きます。
他のＯＳでも手法は同様だと思われます。

(1)下記の２ファイルをダウンロードします。

リンクを右クリックして[リンク先を保存]に類するメニューをクリックすると良いでしょう。

* [ja-JP.po](https://github.com/hsgucci404/ugcs_jp/raw/main/ja-JP.po)
* [ja-JP.png](https://github.com/hsgucci404/ugcs_jp/raw/main/ja-JP.png)

(2)ダウンロードしたファイルを、UgCSのインストール先のフォルダにコピーします。

デフォルトのままでインストールした場合、

C:\Program Files(x86)\UgCS\client\Assets\Resources\Localization\

になります。
ここには、英語や中国語など、他の言語のデータがあります。
ここへ日本語のファイル（具体的にはja-JP.po）を置くことで、UgCSは認識してくれます。
国旗のファイルは一応用意しましたが、効果がよくわかりません（汗

![install](https://user-images.githubusercontent.com/55542434/97270424-7b5d9100-1872-11eb-86a6-174ee4380b78.png)

コピーすると、下図の様な警告が出ますが、管理者として[続行]してください。

![admin](https://user-images.githubusercontent.com/55542434/97270750-ff177d80-1872-11eb-9b75-84ab36cecfbb.png)

これで準備は完了です


# Usage

UgCS clientを起動し、
左上のボタンからメニューを[Main menu]-[Configuration]-[Language]と入っていくと
[日本語]が追加されているはずです。

![menu](https://user-images.githubusercontent.com/55542434/97272492-5fa7ba00-1875-11eb-841f-3b2494eadbaa.png)

あとは[日本語]をクリックして反映させましょう。


# 注意点

※注意１

今後、日本語化する際は、このja-JP.poを編集すれば良いのですが、
Program Files(x86)以下のフォルダ/ファイルの編集権限は管理者にしかありません。

したがってテキストエディタ等で直接

C:\Program Files(x86)\UgCS\client\Assets\Resources\Localization\ja-JP.po

を開いて編集しても、うまく反映されません。（これで1時間悩みました）

したがって、ポイントとしては、デスクトップなどの作業エリアにja-JP.poファイルを置いて編集・保存し、
保存する都度、上記Localizationフォルダへ上書きコピーしてください。

上記の警告ダイアログが出ますが、管理者として続行すれば問題ありません。

※注意２

編集したja-JP.poファイルを上書きコピーしても、
UgCS clientアプリケーションを一旦終了して再起動しないと反映されません。

書き換える度にアプリを再起動しましょう。

# Author
 
* hsgucci
* E-mail: hsgucci@yahoo.co.jp
