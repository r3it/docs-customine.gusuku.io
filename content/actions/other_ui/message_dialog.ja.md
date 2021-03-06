---
title: "情報ダイアログを表示する"
date: 2018-01-22T16:07:50+09:00
weight: 1500
---

## 概要

図のようなダイアログを表示します。
主にユーザーに何か情報を表示する目的で使用します。

![情報ダイアログ](/images/ja/actions/other_ui/message_dialog/1.png)

## 使い方

### 設定するパラメーター

「メッセージ入力」「OKボタンの名前」を設定します。

#### メッセージ入力

ダイアログのメッセージ部分に表示するテキストを入力します。

#### OKボタンの名前

OKボタンに表示するラベルを変更したい場合、このパラメーターを変更します。

## その他の注意点

ユーザーがダイアログの「OK」を押して、ダイアログを閉じた時にアクション完了になります。
ダイアログを表示した段階ではアクション完了になりません。

「[他のアクションの実行が完了した時](../../../conditions/condition_other/when_action_complete/)」でこのアクションの完了を待つ場合、上記に注意してください。
