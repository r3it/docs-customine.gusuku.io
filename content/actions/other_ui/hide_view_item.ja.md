---
title: "一覧から指定の選択肢を消す"
date: 2018-01-22T16:07:50+09:00
weight: 1780
---

## 概要

一覧画面の一覧選択肢（プルダウン項目）から指定の選択肢を消します。

## 使い方

主に条件として「[一覧画面を表示した時](../../../conditions/condition_event/when_record_list_show/)」に、追加の条件を指定して、その条件時に特定の一覧選択肢が消えるように設定します。

例えば追加の条件として「[ログインユーザーがゲストならば](../../../conditions/condition_other_if/user_is_guest_condition/)」を組み合わせると、
ゲストユーザーには見せたくない一覧設定をプルダウンから消すことができます。


### 設定するパラメーター

「一覧の名前」を設定します。


#### 一覧の名前

消したい「一覧」の名前を指定します。
複数の「一覧」を一度に消すことも可能です。その場合、改行で区切って１行毎に消したい名前を入力してください。

言語毎に一覧の名前を変えている場合、各言語での名前を改行で区切って指定してください。

存在しない「一覧」の名前を指定してもエラーにはなりません。


## 制限事項

あくまでも画面上のプルダウン選択項目を消すだけで、消した設定の一覧を表示することを禁止することはできません。
プルダウン選択項目は消えても、ユーザーがその一覧へのリンク URL を知っていれば、そこから表示することはできます。

同様の理由で、一覧の一番上の選択項目を消しても、「アプリへのリンク」から画面遷移してきた場合は、
消す前に一番上にあった選択項目で一覧が表示されます。

スマートフォン版の画面には対応していません。
スマートフォン版で実行しても特にエラーにはなりません。