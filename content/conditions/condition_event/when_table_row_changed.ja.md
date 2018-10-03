---
title: "テーブルに行を追加または削除した時"
date: 2018-01-22T16:07:50+09:00
weight: 1077
---

## 概要

テーブルに行を追加または削除した時にアクションを実行します。

## 使い方

ユーザーがレコードの追加画面や編集画面で、行の⊕⊖ボタンを押して行を追加したり削除したりしたときにアクションを実行する条件です。

「[テーブルに行を追加する](../../../actions/table/add_table_row/)」で行を追加した場合や
「[テーブルから行を削除する](../../../actions/table/remove_table_row/)」で行を削除した場合にも発動します。

「[レコードをテーブルに書き出す](../../../actions/table/write_record_to_table/)」でテーブルに行を書き出したりクリアした場合は発動しません。

PCの画面、スマートフォン用の画面のどちらの場合でも発動します。

### 設定するパラメーター

「テーブル」を設定します。

#### テーブル

テーブルを選択します。
複数選択することができ、その場合、選択したテーブルのどれか１つで行が追加・削除されたときにアクションが実行されます。

## 制限事項

「[テーブルをスプレッド化する](../../../actions/table/set_handsontable/)」でスプレッド化している場合、
この条件は発動しません。
