---
title: "一覧で画面に表示されているレコードを取得する"
date: 2018-01-22T16:07:50+09:00
weight: 1730
---

## 概要

一覧の画面で現在のページに表示されているレコードを取得します。

## 使い方

取得したレコードは、例えば「[レコード中のフィールド平均値を計算する](../../aggregate/calc_records_average)」のような集計関数で集計したり、
計算式を使用して計算に利用することができます。


### 設定するパラメーター

パラメーターはありません。

## 制限事項

スマートフォン用の画面では使用できません。

一覧が複数ページにまたがっている場合、現在表示されているページのレコードのみが取得されます。
見えていないページのレコードは取得されません。

見えていない分まで含め、すべてのレコードを取得したい場合は、
「[一覧の条件でレコードを全件取得する](../get_record_using_list)」を使用します。