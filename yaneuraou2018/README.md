# これは何？

このフォルダには9bce145d4645060a6ce1bc940a9c473af2975d28からビルドしたやねうら王(KPP\_KKPT版)のバイナリを含んでいます。

# モデルファイル
モデルファイルは大きいのでこのリポジトリに含めることができません。

簡単に使おうと思う場合は、以下の2つの作業を行って下さい。

1. https://github.com/yaneurao/YaneuraOu/blob/master/README.md を参照し、「リゼロ評価関数 KPP\_KKPT型 epoch4」をダウンロードした上、evalフォルダの下にファイルを展開して下さい。
2. https://github.com/yaneurao/YaneuraOu/releases/tag/v4.73\_book を参照し、お好きな定跡ファイルをダウンロードしてbookフォルダの下にファイルを展開して下さい。

# 自分でビルドする方へ
とりあえずSSE4.2向けのビルドのみ同梱しています。それ以外のバイナリが欲しい方はご自分でビルドして下さい。
ビルドする場合は、engine\_define.xml内のCpuTypeを書き換える必要があります。

# engine\_define.xmlについて
また、engine\_define.xmlは、MyShogiのバイナリから生成させたサンプルXMLを元に改変しています。
生成コードはここにあります。
https://github.com/yaneurao/MyShogi/blob/master/MyShogi/Model/Shogi/EngineDefine/Sample/EngineDefineSample.cs

# ライセンス
ビルドに当たって多少ソースコードを書き換えました。
コードは https://github.com/jnory/YaneuraOu/tree/myshogi_engine_sample から取得できます。
ライセンスは本家がGPLv3のため、こちらもGPLv3になります。

