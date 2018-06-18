Name
====

Alpine Linuxの自然言語処理パッケージ作成 設定ファイル

## Description

Alpine Linuxで日本語の自然言語処理関連ツールのapkファイルを作成するためのビルドファイルです。
毎回Dockerfileにビルドのスクリプトを書くのが大変なので作りました。

ビルドせずにすぐ使いたい人は以下コマンドで全パッケージが入ったDockerを実行できます。
```
$ docker pull kangaechu/docker-alpine-nlp-jp
```

### 対応しているパッケージ

- [MeCab (+ IPADIC)](http://taku910.github.io/mecab/)
- [Juman](http://nlp.ist.i.kyoto-u.ac.jp/EN/index.php?JUMAN)
- [KNP](http://nlp.ist.i.kyoto-u.ac.jp/?KNP)
- [Juman++](https://github.com/ku-nlp/jumanpp)

## Requirement

Alpine Linux

## Usage

https://wiki.alpinelinux.org/wiki/Creating_an_Alpine_package
https://qiita.com/SKAhack/items/0d2146305f569f09b96a

を参考にセットアップしてください。

セットアップが終わったらAPKBUILDがあるディレクトリに移動して

```bash
# abuild -r
```

を実行すれば`~/packages`ディレクトリにパッケージが作成されます。

## Licence

MIT

## Author

[kangaechu](https://github.com/kangaechu)
