---
title: "所属グループ（ロール）を取得する"
date: 2018-01-22T16:07:50+09:00
weight: 1610
---

## 概要

現在ログインしているユーザーが所属するグループ（ロール）を取得します。

## 使い方

このアクションを実行すると、所属するグループの情報がアクションの結果として保存されます。

この情報を式を使用して $1 などから参照することも可能ですが、「[指定のグループ・組織に所属するならば](../../../conditions/condition_other_if/if_user_belongs_to)」と組み合わせるのがより典型的な使用方法です。

### 設定するパラメーター

「セット先フィールド（省略可）」を指定します。

#### セット先フィールド（省略可）

取得したグループを他のフィールドにセットする場合に指定します。直接フィールドにはセットせず、結果を別のアクションで使用したい場合は、省略できます。

セット先をグループ選択フィールドにした場合、現在選択されている他のグループはクリアされたうえで、ログインユーザーの所属グループが選択された状態になります。複数のグループに所属している場合はすべてセットされます。

セット先を文字列(1行)等にした場合、グループ名がセットされます。複数のグループに所属している場合はグループ名をカンマ区切りで並べたものがセットされます。

## 制限事項

ユーザーがゲストユーザーの場合は取得できません。