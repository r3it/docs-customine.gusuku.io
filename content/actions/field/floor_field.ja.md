---
title: "フィールドの値を切り捨てる"
date: 2018-01-22T16:07:50+09:00
weight: 1430
---

## 概要

指定のフィールド値を「切り捨て」で丸めます。

## 使い方

### 設定するパラメーター

「フィールド」「桁数」を設定します。

#### フィールド

切り捨てするフィールドを選択します。
数値フィールドのみ選択できます。

#### 桁数

切り捨てする桁数を入力します。
マイナスの数値を入力すると小数点以下になります。

```
# 「-2」を指定。
111.119 -> 111.11

#「2」を指定
190 -> 100
```