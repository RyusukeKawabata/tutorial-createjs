## タッチデバイス対応

iOSやAndroid, Windows 10のようなタッチデバイスでタッチ操作を制御するには、`createjs.Touch`クラスを使ってタッチ操作を有効に設定します。`createjs.Touch`クラスによって自動的にタッチイベントがマウスイベントに変換されるため、特別な処理を実装する必要はありません。

```js
// ステージを作成
var stage = new createjs.Stage("myCanvas");

// タッチ操作をサポートしているブラウザーならば
if(createjs.Touch.isSupported() == true){
	// タッチ操作を有効にします。
	createjs.Touch.enable(stage)
}
```


![](../imgs/mouse_touch.html.png)

- [サンプルを再生する](https://ics-creative.github.io/tutorial-createjs/samples/mouse_touch.html)
- [サンプルのソースコードを確認する](../samples/mouse_touch.html)



[目次に戻る](../ReadMe.md)