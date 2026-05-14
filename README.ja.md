# kokoiku

特定の場所へ案内するためのシンプルなウェブアプリです。「kokoiku」（ココイク）は、ユーザーの現在地から事前に設定された目的地までのGoogleマップの経路案内リンクを生成し、メールやメッセージ、ウェブサイトを通じて場所の案内を簡単に共有できるようにします。

ユーザーが「kokoiku」のリンクを開くと、アプリはGPSで現在地を取得し、経路が計算済みのGoogleマップへの直接リンクを生成します。

## デモ

[https://codeforfukui.github.io/kokoiku/](https://codeforfukui.github.io/kokoiku/)

*デフォルトのデモリンクは、鯖江西山公園のレッサーパンダへの経路を案内します。*

## 特徴

*   **ワンクリックで経路案内:** ユーザーの現在地からの経路を計算したGoogleマップへの直接リンクを生成します。
*   **カスタマイズ可能な目的地:** URLのハッシュに座標を埋め込むことで、任意の目的地を簡単に設定できます。
*   **代替出発地:** GPSが利用できない、または許可が拒否された場合、固定の出発地（鯖江駅）をデフォルトとします。
*   **軽量:** 外部ライブラリに依存しない単一のHTMLファイルです。

## 自分のリンクを作成する方法

独自の目的地用の「kokoiku」リンクを作成するには、ベースURLに緯度と経度をハッシュ（`#`）で追加するだけです。

**形式:** `https://codeforfukui.github.io/kokoiku/#LATITUDE,LONGITUDE`

### 例1: リンクを共有する

メールやメッセージで、福井高専電子情報工学科棟入口への案内を送るには以下のURLを送信します:

```
https://codeforfukui.github.io/kokoiku/#35.937525,136.171508
```

### 例2: ウェブサイトに埋め込む

訪問者に場所を案内するため、ウェブサイトにリンクを追加します:

```html
<a href="https://codeforfukui.github.io/kokoiku/#35.950908,136.180781" target="_blank">
  鯖江のレッサーパンダを見に行こう！
</a>
```

## クレジット

作成: [Taisuke Fukuno](http://fukuno.jig.jp/784) (福野泰介)

## ライセンス

[CC BY 2.1 JP](https://creativecommons.org/licenses/by/2.1/jp/)
