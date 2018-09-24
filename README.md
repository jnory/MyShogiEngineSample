# このプロジェクトについて

MyShogiをMacのmonoで使う際の、エンジン設定のサンプルです。

# 使い方

MyShogi.exeのあるディレクトリにengineという名前でcloneして下さい。

# 仕組み

MyShogiはengine\_define.xmlというファイルを探して、そのファイルが含まれるフォルダを
検討エンジンのバイナリがあるフォルダと認識します。
新たにエンジンを追加する場合はフォルダを作ってengine\_define.xmlというファイルを作り、
そのフォルダに諸々のバイナリファイル(実行ファイル、モデルファイル、定跡ファイル)を置いて下さい。

# バイナリの命名規則

<EngineExeName>\_<CPU命令セット>.exe

です。

EngineExeNameはengine\_define.xmlの項目名です。
CPU命令セットはこのあたり https://github.com/yaneurao/MyShogi/blob/master/MyShogi/Model/Shogi/EngineDefine/CpuType.cs#L34 をみるとお察しできるかと思います。

