---
title: "スペースに文字を表示する"
date: 2018-01-22T16:07:50+09:00
weight: 1540
---

## 概要

指定の場所（スペース）に文字（テキスト）を表示します。

[「スペース・メニュー位置に表示した文字を変更する」](../set_label_text_v2)と組み合わせることで、
状況に応じて画面に表示するテキストを変更することができます。

## 準備

アプリにテキストを表示するスペースフィールドを配置しておいてください。

## 使い方

### 設定するパラメーター

「場所」「表示するテキスト」を設定します。

#### 場所

テキストを表示するスペースフィールドを指定します。１つのスペースフィールドに複数種類のテキストを表示することもできます。

#### 表示するテキスト

画面に表示するテキストを指定します。

文字を装飾したり、テキストの中に式を埋め込むことができます。

## 上級者向け情報

設置したテキストには以下の css クラス名がつきます。

- customine-label
- customine-at-spacer

また、ID として

- customine-label-アクション番号（customine-button-1 など）

がつきます。

これを利用して、アプリに css ファイルを登録すればスタイルをカスタマイズすることができます。


## 制限事項

一覧画面では使えません。

スマートフォン版アプリには対応していません。
