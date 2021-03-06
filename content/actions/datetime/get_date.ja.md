---
title: "特定の日付を取得する"
date: 2018-01-22T16:07:50+09:00
weight: 1400
---

## 概要

特定の日付を取得して他のアクションから参照できるようにします。

## 使い方

取得した日付をフィールドに入れたい場合、「セット先フィールド（省略可）」パラメーターにそのフィールドを選択します。

取得した日付をすぐフィールドに入れるのではなく、他のアクションで使いたい場合は数式を利用します。

「特定の日付を取得する」をセットしたアクションを実行すると、アクションの結果としてその日付が内部に保存されます。

保存された日付は、数式を使用して、「=$1」などで取得できます。

保存された日付は、kintone の日付フィールドにそのままセットできる形式になっています。

例）取得した日付を、他のアクション（「[レコードを追加する](../../record/insert_record/)」）で使用する例

1. 「特定の日付を取得する」を設置します。アクション番号が１番だったとします。
2. 「[レコードを追加する](../../record/insert_record/)」の「マッピング」で、セットしたい日付フィールドに対して「=$1」と入れます。
    （「特定の日付を取得する」のアクション番号が２番だったら、「=$2」とします）


### 設定するパラメーター

「日付の種類」を設定します。

#### 日付の種類

「今日」や「今月月初」など、取得したい日付を選択します。

## 他の方法

アクションを使用せずに、数式で関数を使って取得する方法もあります。

「[フィールドに値をセットする](../../field/set_field_value/)」の「値」パラメーターなどで

```
=getDate("今月月初")
```

のように、関数を指定することができます。

上記例の「今月月初」の部分には以下のいずれかを指定できます。

- 今日
- 昨日
- 明日
- 今月月初
- 今月末日
- 先月月初
- 先月末日
- 来月月初
- 来月末日
- 本年年初
- 本年年末
- 昨年年初
- 昨年年末
- 来年年初
- 来年年末
- 本年度初日
- 本年度末日
- 昨年度初日
- 昨年度末日
- 来年度初日
- 来年度末日

#### セット先フィールド（省略可）

取得した日付を他のフィールドにセットする場合に指定します。直接フィールドにはセットせず、結果を別のアクションで使用したい場合は、省略できます。

## 制限事項

- 基準となる今日の日付は、kintone にログインしたユーザーのプロフィール設定で、「タイムゾーン」に設定されたタイムゾーン（時差）に基きます。
特定のタイムゾーン（例えば日本時間）に固定することはできません。

- この「やること」においては「年度」の範囲は４月～３月で固定です。異なる年度範囲で年度開始日等を取得することはできません。
