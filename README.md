# Weather
<img src="https://user-images.githubusercontent.com/33755507/112159674-c23a9180-8c2c-11eb-9111-de9340436be6.PNG" width="320px">

## 概要
雨が降るかどうかを極めてよい精度で知ることが出来るアプリケーションです。

～～

週末の天気予報がよく外れます。

<br>

これは、気象現象が「カオス」であり、わずかなパラメータのズレが大きな誤差につながるためであって、仕方ないのですが、ちょっと出掛けた隙に大雨が降ってくることがよくあり、業を煮やした私は、精確な天気予報アプリを作ることにしました。

実は、時間と位置・種類を適切に絞り込めば、天気予報の的中率は100％に近付きます。<br>
例えば、１分後の気象の予報は、私たちが当てずっぽうに言ってもほぼ100%当たるであろうことは、容易に想像できますね。<br>
現代の気象予報の技術を以てすれば、3時間以内で雨が降るか、降らないか、という情報だけに限定した場合、的中率は95％を超えると言われています。<br>
さらに、１時間以内の降水情報なら、５分間隔で計算が行われていますが、この情報がテキストの形で、一般に提供されることはありません。これは非常にもったいないと思います。<br>

<br>

話がわき道に逸れましたが、短時間であればあるほど、また情報を限定すればするほど、正確な気象予報が得られることは直感的にご理解頂けると思います。<br>
洗濯物を干すときに、明後日の天気なんかどうでも良いのではないのでしょうか。それよりも、雨が少しでも降るかどうか精度よく知りたい、と願うのは作者だけではないはず。<br>

当初は自分だけで使う予定でしたが、公開すれば広く公の利益になると思い、無償で保守・提供をしていくことにしました。<br>
こうしたアプリですから、精確さを何より重視しています。また、的中率が高い情報のみを載せ、一致させることが難しい情報は扱いません。

<br>

### 他のアプリとの違い

<br>

☆ **雨が降ってくる時間を分単位で知ることが出来ます**。<br>
2021年3月に調査したところ、同じ機能を実装しているアプリ・プログラムは１つもありませんでした。

☆ **極めて正確です**。<br>
例えば、３０分以内に限定した場合、雨が降る時間の的中率は98％です。（作者が３０回以上サンプルを取って調査した結果）

☆ **動作は非常に高速で、視認性に優れています**。<br>
テキストベースのためです。広告や画像・ログインシステム等、余計なリソースも一切ありません。

☆ **プログラムが広く公開されています**。<br>
このアプリおよびソースコード（2021年6月頃公開予定）はMITライセンスで提供されており、改変・再配布は作者に責任を求めない限り自由です。
また、脆弱性や不具合もこのため、見つかりやすくなっています。

☆ **作者が日常的に使っているアプリです**。<br>
これは、不具合修正が極めて速いことを意味します。また、利用者にとって有益なアップデートを重視している証拠でもあります。

<br>

### 仕様

<br>

A.1時間以内の降水量を**5分間隔**で取得出来ます。的中率92%以上。

B.24時間以内の天気を**3時間間隔**で把握可能です。的中率85％以上。

C.３日以内の天気を**毎日**取得できます。一致率は７割くらい。


<br>

※ソースは[ココ](https://www.data.jma.go.jp/fcd/yoho/data/kensho/score_f.html)。

<br><br>

## 使い方
### 1.アプリをダウンロードして適当なファイルに展開します。
<img src="https://user-images.githubusercontent.com/33755507/113813406-ccbb6600-97aa-11eb-997c-78f248e25354.PNG" width="320px">

右側の**Release → バージョン名 → ページ下方のAssetsというところ**からWindows用のファイルをダウンロード。

適当なところに展開するのが良いと思います。**ソースを直接ダウンロードして使えないです**。気を付けてください。

### 2.Windows>Weather.exe を実行します。

### 3.アプリ内の指示に従って自宅のタイル座標と地域を指定します。

<img src="https://user-images.githubusercontent.com/33755507/112163277-388cc300-8c30-11eb-8fbe-898b185882ca.png" width="160px">　<img src="https://user-images.githubusercontent.com/33755507/112163450-640fad80-8c30-11eb-9b94-20ef12ac3393.PNG" width="320px">

入力したら「保存」をクリック。ほとんど難しい操作が無いため、使っているうちにすぐ慣れます。

<br>

## アップデート
時々、新機能やUIの改善を目的としたアップデートを行います。そのうち、アップデート確認の機能を付ける予定です。

また、このソフトが使っている[Weather API](https://weather.tsukumijima.net/)の仕様変更に伴って生じた不具合の修正も随時行います。

このアプリは製作者も使っているため、不具合発見・修正は割と早いと思います。内容によりますが、２～７日で修正パッチをアップする予定です。

BitBucketやgitが使える方はリポジトリを複製して、masterブランチをpullするとアップデートが簡単です。

２０２１年４月以降、さらに機能の拡充を予定しています。

リリースしたばかりで、何かと不便があるかと思いますが、お付き合い頂ければ幸いです。

<br><br>

## Q&A
### バグを見つけました。
新規[Issue](https://github.com/rarafy/Weather/issues)でご報告ください。

### 追加してほしい機能があります。
同じく[Issue](https://github.com/rarafy/Weather/issues)から、お知らせください。

### データが消えました。
再度入力してください。


<br>

## 不具合・脆弱性
- 現在のところ不具合の報告はありません。


<br><br><br>
### 画像置き場
<img src="https://user-images.githubusercontent.com/33755507/112722243-a811f380-8f4b-11eb-84cf-a9aedee04ecf.png" width="20px"> <img src="https://user-images.githubusercontent.com/33755507/112722247-a9dbb700-8f4b-11eb-80a2-d8d68646276a.png" width="20px"> <img src="https://user-images.githubusercontent.com/33755507/112722294-02ab4f80-8f4c-11eb-90bc-f186cc5a5744.png" width="20px">

