---
title: "地図にマーカーを追加する"
date: 2018-01-22T16:07:50+09:00
weight: 1520
---

## 概要

設置済みの地図にマーカーを追加します。

## 使い方

「[地図をスペースに表示する](../show_google_map/)」や「[地図をメニュー位置に表示する](../show_google_map_at_menu)」で地図を設置しておきます。

より高速に表示するためには、緯度経度の情報をアプリに持たせておくとよいでしょう。
住所を指定して表示する場合よりも、緯度経度を指定したほうが高速に表示されます。

一覧画面で使用すると、一覧のレコードの数だけ繰り返し実行されます。

### 設定するパラメーター

「地図」「住所または緯度経度」「マーカー名」を設定します。

#### 地図

どの地図にマーカーを表示するのかを地図を設置したアクションを選択して指定します。


#### 住所または緯度経度

地図に表示する位置を指定します。

住所で指定する場合、番地までの細かい住所で指定することもできますし、市町村名までのような大まかな住所で指定することもできます。
また、「東京スカイツリー」のように著名な建物の場合、建物名だけでも表示可能です。これらは Google Maps の機能になります。

緯度経度で指定する場合、緯度の数値、経度の数値をカンマで区切って設定します。

```
34.687315, 135.526201
```

フィールドに住所の情報が入っている場合、式を使ってフィールドの値を渡すことができます。
フィールドが「都道府県」「住所1」「住所2」に分かれている場合は次のように指定します。

```
${都道府県} ${住所1} ${住所2}
```

#### マーカー名

マーカーの名前を設定します。
省略した場合、「住所または緯度経度」が住所で指定されていれば、住所がマーカー名になります。


## 制限事項

一覧画面で使用すると、一覧のレコードの数だけ繰り返し実行されます。

この時、「住所または緯度経度」で緯度経度ではなく住所を指定すると、１つマーカーを設置するたびに約２秒の待ち時間が入ります。
そのためすべてのマーカーを表示するために時間がかかります。

これは、Google Maps の制限で、住所から位置を検索する処理を短い時間で繰り返し呼ぶことができない、という制約によるものです。

この制限を回避するには、住所ではなく緯度経度で指定してください。
