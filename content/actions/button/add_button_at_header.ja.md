---
title: "ボタンをメニュー位置に配置する"
date: 2018-01-22T16:07:50+09:00
weight: 1210
---

## 概要

指定の場所（メニュー位置）にボタンを配置します。

「[ボタンを押した時](../../../conditions/condition_other/button_clicked)」の条件と組み合わせることで、
ボタンを押した時に何かのアクションを実行するようなカスタマイズを行うことができます。


## 使い方

ボタンは配置しただけではボタンが画面に表示されるだけで、押しても何も起こりません。
ボタンを押したときに何か行うようなカスタマイズを行うには、さらに別のアクションを配置して、そのアクションに「[ボタンを押した時](../../../conditions/condition_other/button_clicked)」条件をセットします。

１つの場所に複数のボタンを置くこともできます。
この場合、アクションを実行した順番に、左から右へボタンが追加されていきます。

### 設定するパラメーター

「場所」「ラベル」を設定します。

#### 場所

ボタンを置く場所を選択します。

- レコード詳細メニューの上側 ... レコード詳細画面や編集画面の、下図の位置に表示します。

![レコード詳細画面の上側](/images/ja/actions/button/add_button_at_header/1.png)

- 一覧画面メニューの右側 ... レコード一覧画面の、下図の位置に表示します。

![一覧画面メニューの右側](/images/ja/actions/button/add_button_at_header/2.png)

- 一覧画面メニューの下側 ... レコード一覧画面の、下図の位置に表示します。

![一覧画面メニューの下側](/images/ja/actions/button/add_button_at_header/3.png)

#### ラベル

ボタンを画面に表示する際に、ボタンに表示するラベルを指定します。

## 上級者向け情報

設置したボタンには以下の css クラス名がつきます。

- customine-button
- レコード詳細画面の上側の場合 customine-at-record-header-menu-space
- 一覧画面メニューの右側の場合 customine-at-header-menu-space
- 一覧画面メニューの下側の場合 customine-at-header-space

また、ID として

- customine-button-アクション番号（customine-button-1 など）

がつきます。

これを利用して、アプリに css ファイルを登録すればボタンのスタイルをカスタマイズすることができます。

## 制限事項

「レコード詳細画面の上側」は一覧画面では使えません。

「一覧画面メニューの右側」「一覧画面メニューの下側」は一覧画面以外では使えません。

スマートフォン版アプリでは「一覧画面メニューの右側の場合」には対応していません。
