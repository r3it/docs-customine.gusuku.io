---
title: "地図をメニュー位置に表示する"
date: 2018-01-22T16:07:50+09:00
weight: 1510
---

## 概要

指定の場所（メニュー位置）に地図を配置します。

## 使い方

事前に Google Maps のサイトで、API キーを入手しておきます。
API キーの入手方法については

https://developers.google.com/maps/documentation/javascript/get-api-key

を参照してください。

### 設定するパラメーター

「場所」「APIキー」「住所または緯度経度」「ズームレベル」「マーカー名」を設定します。

#### 場所

地図を表示する場所を指定します。

- レコード詳細メニューの上側 ... レコード詳細画面や編集画面の、下図の位置に表示します。

![レコード詳細画面の上側](/images/ja/actions/external/show_google_map_at_menu/1.png)

- 一覧画面メニューの右側 ... レコード一覧画面の、下図の位置に表示します。

![一覧画面メニューの右側](/images/ja/actions/external/show_google_map_at_menu/2.png)

- 一覧画面メニューの下側 ... レコード一覧画面の、下図の位置に表示します。

![一覧画面メニューの下側](/images/ja/actions/external/show_google_map_at_menu/3.png)


#### APIキー

Google Maps の API キーを入力します。

API キーは Google Maps のサイトから取得してください。

https://cloud.google.com/maps-platform/?hl=ja
https://developers.google.com/maps/documentation/javascript/get-api-key?hl=ja

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

#### ズームレベル

ズームレベルを入力します。

Google Maps のドキュメントにより、以下を目安にしてください。

- 1: 世界
- 5: 大陸
- 10:市
- 15:通り
- 20:建物

https://developers.google.com/maps/documentation/javascript/tutorial?hl=ja#MapOptions


#### マーカー名

マーカーの名前を設定します。
省略した場合、「住所または緯度経度」が住所で指定されていれば、住所がマーカー名になります。


## 制限事項

「レコード詳細画面の上側」は一覧画面では使えません。

「一覧画面メニューの右側」「一覧画面メニューの下側」は一覧画面以外では使えません。

スマートフォン版アプリでは「一覧画面メニューの下側」のみ対応しています。

### 2つの以上の地図の表示

同じアクション番号で「地図をメニュー位置に表示する」を２回繰り返し実行した場合、同じ地図とみなされ、地図は1つしか表示されません。
２回目のアクションでは現在表示している地図位置を変更しません。

異なるアクション番号で「地図をメニュー位置に表示する」をそれぞれ実行した場合、それぞれの地図が別々に表示されます。

マーカーを増やしたい場合、「地図をメニュー位置に表示する」を繰り返し実行するのではなく、
「[地図にマーカーを追加する](../add_google_map_marker)」を使用してください。
