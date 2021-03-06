---
title: "テーブルから行を削除した時"
date: 2018-01-22T16:07:50+09:00
weight: 1076
---

## 概要

テーブルから行を削除した時にアクションを実行します。

## 使い方

ユーザーがレコードの追加画面や編集画面で、行の⊖ボタンを押して行を削除したときにアクションを実行する条件です。

「[テーブルから行を削除する](../../../actions/table/remove_table_row/)」で行を削除した場合にも発動します。

「[レコードをテーブルに書き出す](../../../actions/table/write_record_to_table/)」の「既存のテーブル行はクリアする」でテーブル行をクリアした場合は発動しません。

PCの画面、スマートフォン用の画面のどちらの場合でも発動します。

行の追加では発動しません。

### 設定するパラメーター

「テーブル」を設定します。

#### テーブル

テーブルを選択します。
複数選択することができ、その場合、選択したテーブルのどれか１つで行が削除されたときにアクションが実行されます。

## 制限事項

「[テーブルをスプレッド化する](../../../actions/table/set_handsontable/)」でスプレッド化している場合、
この条件は発動しません。

