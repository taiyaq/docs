---
title: "対訳の作成"
weight: 3
chapter: false
---

以下のサイトを翻訳してみます。  
https://facebook.github.io/react-native/docs/using-a-scrollview.html

ブラウザから上記リンクを開いて下さい。

<!-- 
先ずは該当ドキュメントのライセンスを参照して翻訳して問題ないことを確認します。
react-nativeのドキュメントのライセンスは
https://github.com/facebook/react-native/blob/master/LICENSE-docs
から確認できます。 -->

# 対訳の作成
以下のように、1,2,3の順でクリックして新規の対訳情報を作成します。

![create](../images/create01.png?width=50pc)

以下のように翻訳の準備ができればokです。

![create02](../images/create02.png?width=25pc)

# 編集対象を絞り込む

沢山の対訳情報が揃いましたが、どれから翻訳すればいいか迷うはずです。

そこでサイドバーを開いた状態で翻訳したい部分をクリックしてみて下さい。

![filter01](../images/filter01.png?width=50pc)

自動でフィルタ条件が設定され該当の対訳情報が絞り込まれます。

これはうまく機能しない場合もあります。
その場合はフィルタ条件にヒットしそうな文字列を入力してみます。

![filter02](../images/filter02.png?width=50pc)

上手く絞りこめるはずです。
絞り込まれない場合はもう少し単語の数を減らしてみて下さい。

# 対訳編集

該当の対訳を見つけたら実際に翻訳してみます。

ところで、翻訳を手動で行うのは大変なので便利なエクステンションを使いましょう。  
[google翻訳です](https://chrome.google.com/webstore/detail/google-translate/aapbdbdomjkkjkaonfhkkikfgjllcleb?hl=ja)


これを使うと文章単位で翻訳できます。
![translate01](../images/translate01.png?width=50pc)

ご覧の通り。結構使えます。
これをコピーしましょう。

![translate02](../images/translate02.png?width=50pc)

ただコピーするだけだと保存できない場合があります。今回はエラーが出ていますね。
対訳情報は特殊構文になっておりその通りにしないと保存できません。


今回ペースとなる英文は以下のように設定されています。

```html
The<1>ScrollView</1>is a generic scrolling container that can host multiple components and views. The scrollable items need not be homogeneous, and you can scroll both vertically and horizontally (by setting the<2>horizontal</2>property).
```

``ScrollView``と``horizontal``が特殊なタグ ``<数値>`` ``</数値>`` で囲まれています。
HTMLにおいて強調表示だったりリンクだった部分です。
翻訳時もその情報を対訳に付与する必要があるため、該当する単語に同じタグを割り当てて下さい。

![translate03](../images/translate03.png?width=50pc)

今回は以下のような対訳を設定しました。保存できるようになっているので忘れずに``Save``を押して下さい。

```HTML
<1>ScrollView</1>は、複数のコンポーネントとビューをホストできる一般的なスクロールコンテナです。スクロール可能なアイテムは同種である必要はなく、（<2>horizo​​ntal</2>プロパティを設定することによって）垂直方向と水平方向の両方でスクロールすることができます。
```

![translate04](../images/translate04.png?width=50pc)

翻訳を押すと翻訳されます。

簡単ですね。ちなみに ``<br>``だけは特別使うことができます。

見た目として改行が必要だと思ったら入れてみて下さい。(但し、使えない場所もあります。)
![br](../images/br.png?width=50pc)

上記はもちろんだめな例です。見た目が良くなるように上手く使ってみて下さい。

# 次の対訳に移動する

![next](../images/next.png?width=50pc)

図のように上記はボタンになっており次の翻訳への移動に使うことができます。  
上手く使って作業の効率化を図って下さい。

# 対訳のアップロード

対訳の作成が一通り終わったらアップロードしてみましょう。


## 追加情報の登録


![editDetail](../images/editDetail.png?width=50pc)

上記のように自作翻訳をクリックして詳細編集を選んで下さい。

![editDetail02](../images/editDetail02.png?width=50pc)

タイトルとTagを設定して下さい。

今回は以下のように設定しました。


|種別|内容|
|:---|:---|
|タイトル | ``React-native ScrollViewの説明の翻訳`` |
|Tags | ``React.js, JavaScript`` |
 
としてます。

``公開状態`` にチェックを入れると公開されます。
ドキュメントのライセンス状態を確認してからチェックを入れるか作者に許可をもらうことを推奨します。

Description には、どうして翻訳したかを記入しておくと良いでしょう。

![upload](../images/upload.png?width=50pc)

アップロードをクリックして下さい。


![upload02](../images/upload02.png?width=50pc)

再度、アップロードをクリックして下さい。


![complete](../images/complete.png?width=50pc)

アップロードが完了しました。ありがとうございます。
