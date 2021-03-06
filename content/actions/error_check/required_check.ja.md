---
title: "必須チェックを行う"
date: 2018-01-22T16:07:50+09:00
weight: 1260
---

## 概要

フィールドの必須チェックを行います。
フィールドに値が入力・選択されていない場合にエラーメッセージをセットします。

## 使い方

### 設定するパラメーター

「フィールド」「エラーメッセージ」を設定します。

#### フィールド

どのフィールドをチェックするかを選択します。

- 複数のフィールドを選択すると、それらすべてのフィールドを個々にチェックします。
- テーブル内のフィールドを指定した場合、特別な場合(*1)を除き、テーブル内のすべての行がチェックされます。

(*1) 条件側で、「フィールドの値を編集して値が変わった時」のように、テーブル行を限定するように条件が入っている場合は、対象の行だけチェックされます。

#### エラーメッセージ

エラーがあった場合に表示するエラーメッセージを入力します。

## 制限事項

以下の種類のフィールドは選択__できません__。

- テーブル
- スペース
- グループ
- 関連レコード一覧
- レコード番号
- 作成者
- 作成日時
- 更新者
- 更新日時
- カテゴリー
- ステータス
- 作業者

## 既知の問題

「添付ファイル」形式のフィールドを選択した場合、
添付ファイルが１つも添付されていなくてもエラーにならない問題が確認されています。

