---
title: "レコードをテーブルに書き出す"
date: 2018-03-06T12:01:14+09:00
weight: 1010
---

## 概要

レコードのデータをこのアプリのテーブルに書き出します。

## 使い方

「[条件を指定してレコードを取得する](../../record/get_records_by_query)」などで取得したレコードを、テーブルの行として書き出すことができます。

元となるレコードは、他のアプリのものでも構いませんし、自アプリの「[テーブル行をレコードとして取得する](../get_record_from_table)」で取得したものでも構いません。

「テーブル行をレコードとして取得する」とこの「レコードをテーブルに書き出す」をつなげることで、
アプリ内でのテーブルデータのコピーが実現できます。

### 設定するパラメーター

「書き出し先テーブル」「レコード」「マッピング」「既存の行」を設定します。

#### 書き出し先テーブル

どのテーブルへ書き出すか、テーブルを選択します。

#### レコード

書き出し元となるレコードデータを取得したアクションを選択します。

#### マッピング

書き出すテーブルのフィールド（列）値を設定します。

このパラメーターの詳しい記述方法は[フィールドマッピングの記述方法](../../field_mapping/)を参照してください。

フィールドの値を空にした場合、空の値を書き出すのではなく、そのフィールドは書き出しません。
更新の場合は元のレコードの値を維持し、挿入の場合はアプリ設定上の初期値がセットされることになります。

#### 既存の行

書き出し先のテーブルにもともとある行をクリアするか、クリアせずに追記するかを選択します。

## 制限事項

テーブルの外側のフィールドへは書き出しできません。

