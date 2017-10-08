# Java9 Sandbox

このリポジトリではJava9 を使ったモジュールのビルドをいくつかの演習をこなしていきます。

このリポジトリではDockerを使ってビルドしました。
その中で、dockerのイメージがおかしくなっているのか
gradleのwrapperのダウンロードではSSL関係のエラーが発生します。
https://github.com/docker-library/openjdk/issues/145

gradleやmavenを利用するサンプルをdockerで利用する場合は
~/.gradleや~/.m2をボリュームマウントして利用すると良いでしょう。

ソースの説明は現状あまりありません。追加するつもりはあります。

## Table of Contents 

* [practice1](practice1/README.md) javacでモジュールをビルドしてみよう
* [practice2](practice2/README.md) 複数モジュールをjavacでビルドしてみよう
* [practice3](practice3/README.md) 複数モジュールをjavacでビルドしてjarにパッケージして実行してみよう
* [practice4](practice4/README.md) Automatic Moduleを利用して、moduleとしてビルドされていないjarファイルを利用してみよう
* [practice5](practice5/README.md) リフレクションを利用したサンプルを利用して、モジュールのexport, openについて探ってみよう
* [practice6](practice6/README.md) モジュールのリフレクションを利用して実行時にexportを追加して本来動かないコードを動かしてみよう
* [practice7](practice7/README.md) Callbackを使うような、3パッケージの構成を書いてみよう
* [practice7](practice7) gradleを使ってjava9をビルドしてみようと思ったら普通にビルドできた
* [practice7](practice8) mavenを使ってjava9をビルドしてみようと思ったら普通にビルドできた

## おまけ

もう少し複雑なサンプルは[この辺のリポジトリ](https://github.com/torstenwerner/java-9-no-jar-hell)を見ると良いでしょう。