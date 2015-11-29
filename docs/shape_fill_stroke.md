# シェイプの塗りと線

シェイプには塗りと枠線を設定できます。塗りだけを設定したり、線だけを描いて塗らないということも可能です。

## 塗り

塗りというのは図形に囲まれた領域となります。`beginFill()`メソッドで塗りの色を指定します。

書式
```js
Graphicsオブジェクト.beginFill(塗りの色);
Graphicsオブジェクト.endFill();
```

サンプル

```js
// シェイプを作成
var shape = new createjs.Shape();
// 塗りの色を指定
shape.graphics.beginFill("red");
// 円を描く
shape.graphics.drawCircle(0, 0, 80);
```

![](../imgs/shape_begin_fill.html.png)

[サンプルを開く](../samples/shape_begin_fill.html)


### コラム

図形を描いたら`endFill()`メソッドで描き終わったことを指定します。必ずしも使わなくても大丈夫ですが、複数のシェイプを描くときには指定しておくほうが無難でしょう。


## 線

線とは図形の境界線のことです。`setStrokeStyle()`メソッドで線の太さを、`beginStroke()`メソッドで線の色を設定することができます。


書式

```js
Graphicsオブジェクト.beginFill(塗りの色);
Graphicsオブジェクト.setStrokeStyle(線の太さ);
```

サンプル

```js
// シェイプを作成
var shape = new createjs.Shape();
// 線の色を指定
shape.graphics.beginStroke("red");
// 線の幅を指定
shape.graphics.setStrokeStyle(5);
// 円を描く
shape.graphics.drawCircle(0, 0, 80);
```




![](../imgs/shape_begin_stroke.html.png)

[サンプルを開く](../samples/shape_begin_stroke.html)

### コラム

図形を描いたら`endStroke()`メソッドで描き終わったことを指定します。必ずしも使わなくても大丈夫ですが、複数のシェイプを描くときには指定しておくほうが無難でしょう。


[目次に戻る](../ReadMe.md)