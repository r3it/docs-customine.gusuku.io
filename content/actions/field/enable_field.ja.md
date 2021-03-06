---
title: "フィールドを有効化する"
date: 2018-01-22T16:07:50+09:00
weight: 1360
---

## 概要

無効化状態（入力不可になっている状態）になているフィールドを、元の入力できる状態に戻します。

## 使い方

「[フィールドを無効化する](../disable_field/)」で入力できない状態になったフィールドや、
ルックアップフィールドのコピー先になっているため入力不可になっているようなフィールドを、入力可能な状態に戻すことができます。

もともと入力可能な状態のフィールドに「フィールドを有効化する」を実行した場合、何も起こりません。エラーにはなりません。

### 設定するパラメーター

「フィールド」を設定します。

#### フィールド

enable（入力できる状態）にしたいフィールドを選択します。
複数選択することが可能で、選択したフィールド全てを同時に enable（入力できない状態）にします。

## 制限事項

以下のフィールドタイプは選択**できません**。

- スペース
- テーブル
- グループ
- 関連レコード一覧
- 作成者
- 作成日時
- 更新者
- 更新日時
- カテゴリー
- ステータス
- 作業者
