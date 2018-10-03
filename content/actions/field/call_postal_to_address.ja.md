---
title: "郵便番号から住所を検索する(旧)"
date: 2018-01-22T16:07:50+09:00
weight: 1542
---

## 概要

郵便番号を入力して住所を検索して、フォームに住所を自動的に入力する機能を提供します。

## 非推奨

こちらは古いバージョンになるので、[新しいバージョン](../call_postal_to_address_v2/)をご使用ください。

## 使い方

例えば「住所検索」のようなボタンを押したときに検索を実行したい場合、事前にボタンを配置しておきます。

### 設定するパラメーター

「郵便番号」「都道府県フィールド」「住所(1)フィールド」～「住所(4)フィールド」を設定します。

#### 郵便番号

郵便番号の値を入力します。

フィールドではなく値ですので、郵便番号フィールドから値をとりたい場合は、以下の例のように式を使ってください。

    =文字列_1行_2

#### 都道府県フィールド

検索結果で得た都道府県名をセットする先のフィールドを指定します。

セット先がドロップダウンなどの選択式のフィールドの場合、選択肢は「富山県」のように「県」などを末尾につけてください。
選択肢が「富山」のように「県」を省略した形だと、エラーになります。

#### 住所(1)フィールド
#### 住所(2)フィールド
#### 住所(3)フィールド
#### 住所(4)フィールド

市区町村名以降の住所をセットするフィールドを選択します。

通常、住所(1)が市区町村名、住所(2)は町域名になり、住所(3)(4)は予備になります。

住所(1)～住所(4) を同じフィールドにすることもできます。
その場合、市区町村名、町域名などをつなげて１つのフィールドにセットします。

### 制限事項

「都道府県フィールド」で選択できるフィールドタイプは以下の通りです。

- 文字列（1行）
- 文字列（複数行）
- リッチエディター
- ドロップダウン

「住所(1)フィールド」～「住所(4)フィールド」で選択できるフィールドタイプは以下の通りです。

- 文字列（1行）
- 文字列（複数行）
- リッチエディター