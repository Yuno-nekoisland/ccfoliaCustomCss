# ccfoliaCustomCss

## 注意点

- 本リポジトリは、**個人的に利用するため**のものです。
- ここに辿り着いて利用したいと思った方は、自分で書くか下記クレジットに記載しているリポジトリを使って

## クレジット・参考元

本リポジトリは以下のプロジェクトや記事を参考にしており、**部分的に引用**しています。
先行事例に感謝し、敬意を表して記載します。

- [OBSでココフォリアを表示させる時のカスタムCSSについて | U7D05 BAR](https://ydk.vc/obs-ccfolia-css/)（著: yudukiak）
- [ccfoliaCSS by yudukiak](https://github.com/yudukiak/ccfoliaCSS)
- https://github.com/GhGANTZ/customCss/tree/main

## 下記は自分用メモ

## 構成概要

各シナリオごとにディレクトリを分けており、以下のような構造になっています。

```
css
├─asset
│  ├─common
│  │  └─・・・・・・
│  └─シナリオ名
│     ├─import-css/ # Import用カスタムCSS
│     └─obs-src/ # OBS向けのカスタムCSS
└─docs
```

### 📁 `import-css/`

- ココフォリアの外観（背景、メモ、UI要素など）をカスタマイズするCSSファイルを格納。
- 例: メモ欄の装飾、背景の変更、全体のテーマカラー調整など。

### 📁 `obs-src/`

- OBS（Open Broadcaster Software）の配信レイアウトに適用するためのCSSを格納。
- 例: 透明背景のスタイル、フレーム表示、視覚的な強調装飾など。

## 利用方法

1. 任意のシナリオディレクトリを選択。
2. `import-css`フォルダ内のCSSファイルをimportする形で、外観装飾のCSSを読み込む。
3. `obs-src`フォルダ内のCSSをOBSの「ブラウザソース」で読み込む想定。シナリオ毎に変数指定する。
