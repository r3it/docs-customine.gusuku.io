---
title: "ログインユーザーが指定のユーザーならば"
date: 2018-03-26T14:53:50+09:00
weight: 1010
---

## 概要

アプリにアクセスしているユーザーが指定のユーザーの場合に条件を満たします。

## 使い方

この条件は他の「いつ実行するか」系の条件と組み合わせて使用します。

例えば一覧画面を表示した時に、「一覧画面を表示時に、かつ、現在のユーザーが指定ユーザーならば」という条件を指定したい場合、
「一覧画面を表示した時」とこの条件を組み合わせます。

### 設定するパラメーター

「ログイン名」を指定します。

#### ログイン名

ユーザーのログイン名を指定します。表示名ではありません。

カンマ区切りで複数のユーザーを指定することができます。その場合、指定したいずれかのユーザーと一致すれば条件が満たされます。
例えば「A,B,C」と指定した場合、ログインユーザーがAさん、またはBさん、またはCさんならばOKで、DさんならばNGとなります。
