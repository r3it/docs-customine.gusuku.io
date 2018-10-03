---
title: "JavaScript を実行する"
date: 2018-01-22T16:07:50+09:00
weight: 2000
---

## 概要

任意の JavaScript を実行します。

## 使い方

### 設定するパラメーター

「JavaScript」を設定します。

#### JavaScript

実行する JavaScript を直接記述します。

通常の kintone カスタマイズと同様に、kintone オブジェクトを使うことができます。

##### 値を返して他のアクションから参照させる方法

この JavaScrippt から return で返した結果は、他のアクションから $1 などの式で参照することが可能です。
return では Promise を返すことも可能です。

```
return "Hello, World!";
```

##### 他のアクションの結果を参照する方法

この JavaScript から他のアクションの結果を参照したい場合、customine オブジェクト経由で参照することができます。
例えば１番アクションの結果は customine[1] で取得できます。

```
alert("1番アクションの結果は[" + customine[1] + "]です！");
```

ただし、アクションの結果は、そのアクションが完了していないと正しく取ることができません。