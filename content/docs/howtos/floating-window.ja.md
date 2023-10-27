---
title: "アプリをフローティングウィンドウで起動する方法"
description: >
  いくつかのGUIアプリはフローティングウィンドウモードで起動することができます。
---

{{< hint danger >}}
注意：このページは[Regolith 1.xのWebサイト](https://regolith-linux.org)からコピーされたもので、Regolith 2のものに更新されていません。古い情報が含まれている可能性があります。
{{< /hint >}}

いくつかのX11アプリケーションでは実行中のアプリケーション下で`class`を指定する`--class`フラグをサポートしています。Regolithでは、`floating_window`クラスのアプリがi3のフローティングウィンドウモードで起動することができるように設計されています。

## 例

### `gnome-terminal`

端末をフローティングウィンドウで起動する方法：

```console
$ gnome-terminal --class=floating_window
```

### Firefox

Firefoxフローティングウィンドウで起動する方法：

```console
$ firefox --class=floating_window
```
