---
title: "Taiyaqとは"
weight: 1
chapter: false
---

# Taiyaq

Taiyaq(タイヤク)は**プログラマ向けの翻訳サービス**です。

その名前に由来する通り、対訳を皆で共有して翻訳されたドキュメントを読む事ができます。このサービスを使うことで直接最新ライブラリのドキュメントや README を読むことができます。例えば、hyperpp の[README](https://taiyaq.com/contents/PGg8jzP12zX8JtE7LALAdzvOAJ)を直接日本語訳でよめます。

![hyper_app_readme](images/hyperapp_readme.png)

みなさんが翻訳されたドキュメントを読む時に気にしていることは**最新のパージョンのもの**を読んでいるのかどうかです。

大抵ライブラリはバージョンが上がっていきドキュメントの内容も更新されていきます。

**翻訳はその後に行われ**るため、古い情報を参考にライブラリの使いかたを覚えることになりかねません。

余計な二度手間を踏むことになかねません。例えばこんな感じです

* **質問** `React.js` の使いかたについて教えてください。以下のようなコードを書いたんですが、、、

```js
import React from 'react';

var Parent = React.createClass({
    getInitialState:function() {
    return {
            display: "none"
    }
  },
// 省略
```

* **解答** そもそも `createClass`を使うのば ES2015 においては推奨されていません

というようなやり取りです。

そもそも React.js の本家のサイトを参照すればこんな質問が飛ぶことはありませんでした。

つまりインターネットにおいては新旧が混在しているため正しい情報を得ることが難しいのです。翻訳ドキュメントは古いかもしれない情報を更に翻訳したものですから余計に不利となります。

これを解決したいと考えこのサービスが生まれました。