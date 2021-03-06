---
title: "レコードから重複を除去する"
date: 2018-03-06T12:01:14+09:00
weight: 1800
---

## 概要

レコードの中から、指定のキーの値が重複しているものを除いて、重複がない状態にします。

## 使い方

対象となるレコードは事前に「[全レコードを取得する](../get_all_records)」や「[キーを指定してレコードを取得する](../get_records_by_key)」などのアクションで取得するように設定しておきます。

レコードは重複するレコードがあった場合、並び順で下になるものが削除されます。

### 設定するパラメーター

「レコード選択アクション」「キーとなるフィールド」を設定します。

#### レコード選択アクション

対象となるレコードを取得したアクションを選択します。

自分自身は選べません。

#### キーとなるフィールド

レコードが重複しているかどうかを判断するときに、比較するフィールドを選択します。

例えば「都道府県」フィールドを指定した場合、同じ都道府県のレコードが２つ以上あった場合、２つ目以降は削除され、１つ目だけが残ります。

フィールドは複数選択することができます。その場合、選択したすべてのフィールドが一致するレコードが「重複している」と判定されます。

選択できるフィールドのタイプは以下になります。

- 文字列(1行)
- 数値
- 計算
- 日時
- 日付
- 時刻
- ルックアップ
- ラジオボタン
- ドロップダウン
- リンク