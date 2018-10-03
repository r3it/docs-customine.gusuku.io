---
title: "ステータスを変更する（指定のレコード）"
date: 2018-01-22T16:07:50+09:00
weight: 1720
---

## 概要

指定したレコードに指定されたステータス変更アクションを実行します。

## 使い方

### 設定するパラメーター

「更新先アプリ」「レコード」「ステータス変更アクション」「作業者フィールド」を設定します。

#### 更新先アプリ

ステータスを更新するアプリを選択します。

#### レコード

ステータスを更新するレコードを取得したアクションを選択します。

#### ステータス変更アクション

アプリに設定したステータス変更アクション名を入力してください。  
（変更後のステータスではなく、アクション名を入力する必要があります）

#### 作業者（更新先アプリから）
#### 作業者（このアプリから）

変更後のステータスに作業者の設定が必要な場合は、  
作業者が設定されたフィールドを選択してください。  
（作業者を直接指定することはできません）

このパラメーターはオプションです。
プロセス管理の設定に従って自動で次の作業者を決める場合は選択しなくて構いません。

このフィールドを、更新先アプリのフィールドから選びたい場合は「作業者（更新先アプリから）」から、
現在カスタマイズしている対象のアプリから選びたい場合は「作業者（このアプリから）」で選択してください。

「作業者（更新先アプリから）」と「作業者（このアプリから）」の両方が選択されている場合、
「作業者（更新先アプリから）」が優先され、「作業者（このアプリから）」は無視されます。

選択可能なフィールドは「ユーザー選択」「（レコードの）作成者」「（レコードの）更新者」のいずれかとなります。

## 制限事項

作業者を直接指定することはできません。  
アプリにユーザー選択フィールドを用意して、そこに作業者として設定したいユーザーを登録してください。  
作業者フィールドに複数のユーザーが設定されている場合は一人目のユーザーが作業者に登録されます。

または、レコードの作成者、更新者を作業者に指定することも可能です。