Apery の実行ファイル、評価関数ファイル、定跡ファイルです。

bin.zip を解凍して下さい。
(apery_nosse.exe を使う際は、bin.zip を解凍した後、bin フォルダに apery_nosse.exe を入れて下さい。)

apery_denousen_final.exe
電王戦FINALで使用したバイナリと同一のものです。新しいCPUかつメモリが沢山ないと動きません。
動作条件: 64bit 版 Windows
        Haswell 以降の CPU
        18GB程度の空きメモリ

apery_bmi2.exe
電王戦FINALバージョンからメモリ使用量と最低使用時間を変更したものです。
動作条件: 64bit 版 Windows
        Haswell 以降の CPU
        600MB程度の空きメモリ

apery_sse42.exe
電王戦FINALバージョンからメモリ使用量と最低使用時間と一部のCPU命令を変更したものです。
動作条件: 64bit 版 Windows
        SSE4.2 が使える CPU
        600MB程度の空きメモリ

apery_sse41.exe
電王戦FINALバージョンからメモリ使用量と最低使用時間と一部のCPU命令を変更したものです。
動作条件: 64bit 版 Windows
        SSE4.1 が使える CPU
        600MB程度の空きメモリ

apery_nosse.exe
電王戦FINALバージョンからメモリ使用量と最低使用時間と一部のCPU命令を変更したものです。
動作条件: 64bit 版 Windows
        ほとんどの CPU で問題なし
        600MB程度の空きメモリ


使用の際の注意点
・「将棋所」などのソフトにAperyを登録することで使用することが出来ます。
・binフォルダの名前を変えないで下さい。変えると評価関数や定跡のファイルを読み込むことが出来ません。
・USI_Hash の値がデフォルトでは小さいので、PCのメモリサイズに合わせて適宜大きくしてご利用下さい。
  分からなければそのままでも結構です。
・Threads オプションは物理コア数を上限にすると良いです。大抵の人にとっては、デフォルト値の半分の値に設定すると良いです。


電王戦FINALでのハードウェアとAperyの設定
CPU は Core i7 5960X
メモリは 64GB 搭載
apery_denousen_final.exe のデフォルト設定から、USI_Hash を 40000 にして下さい。(実際は32GBしか使わないので32GBを超える値なら何でも良いです。)
Threads は 8 にして下さい。
Minimum_Thinking_Time は 360000 にして下さい。(apery_denousen_final.exe ではデフォルトでそうなっています。)


ソースコードはこちらのリポジトリにありますので、興味がありましたらアクセスしてみて下さい。
https://github.com/HiraokaTakuya/apery.git

apery_denousen_final.exe は最初のコミット、それ以外はその次のコミットで今回のバイナリを生成しました。

平岡拓也
