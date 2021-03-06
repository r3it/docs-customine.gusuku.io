---
title: "文字数をチェックする"
date: 2018-01-22T16:07:50+09:00
weight: 1310
---

## 概要

フィールドの文字数をチェックします。

kintone の「文字列(1行)」自身にある文字数チェックとほぼ同様です。

kintone 標準のチェックと違い、条件と組み合わせることで、より複雑なチェックが可能になります。

## 使い方

### 設定するパラメーター

「フィールド」「最小値」「最大値」「エラーメッセージ」を設定します。

#### フィールド

どのフィールドをチェックするかを選択します。

- 複数のフィールドを選択すると、それらすべてのフィールドを個々にチェックします。
- テーブル内のフィールドを指定した場合、特別な場合(*1)を除き、テーブル内のすべての行がチェックされます。

(*1) 条件側で、「フィールドの値を編集して値が変わった時」のように、テーブル行を限定するように条件が入っている場合は、対象の行だけチェックされます。

#### 最小値

フィールドの長さ最小値を入力します。

#### 最大値

フィールドの長さ最大値を入力します。

#### エラーメッセージ

エラーがあった場合に表示するエラーメッセージを入力します。

## 制限事項

選択できるフィールドは次の種類のいずれかに限られます。

- 文字列（1行）
- 文字列（複数行）
- リッチエディター
- リンク