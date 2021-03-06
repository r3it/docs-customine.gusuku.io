---
title: "所属組織を取得する"
date: 2018-01-22T16:07:50+09:00
weight: 1620
---

## 概要

現在ログインしているユーザーが所属する組織を取得します。

## 使い方

このアクションを実行すると、所属する組織の情報がアクションの結果として保存されます。
複数の組織に所属していればそれらすべてが取得されます。

この情報を式を使用して $1 などから参照することも可能ですが、「[指定のグループ・組織に所属するならば](../../../conditions/condition_other_if/if_user_belongs_to)」と組み合わせるのがより典型的な使用方法です。

### 設定するパラメーター

「セット先フィールド（省略可）」を指定します。

#### セット先フィールド（省略可）

取得した組織を他のフィールドにセットする場合に指定します。直接フィールドにはセットせず、結果を別のアクションで使用したい場合は、省略できます。

セット先を組織選択フィールドにした場合、現在選択されている他の組織はクリアされたうえで、ログインユーザーの所属組織が選択された状態になります。複数の組織に所属している場合はすべてセットされます。

セット先を文字列(1行)等にした場合、組織名がセットされます。複数の組織に所属している場合は組織名をカンマ区切りで並べたものがセットされます。

## 制限事項

組織に親子関係がある場合、子組織に所属していても、親組織に所属していなければ、取得されるのは子組織のみになります。

ユーザーがゲストユーザーの場合は取得できません。
