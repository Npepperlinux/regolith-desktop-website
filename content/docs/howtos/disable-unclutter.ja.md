---
title: "マウスの非表示の無効化（unclutter）"
description: >
  unclutter-xfixesを無効化する
---

{{< hint danger >}}
注意：このページは[Regolith 1.xのWebサイト](https://regolith-linux.org)からコピーされたもので、Regolith 2のものに更新されていません。古い情報が含まれている可能性があります。
{{< /hint >}}

既定ではマウスの数秒放置するとマウスカーソルが非表示になります。マウスカーソルが常に画面上に表示されている状態を好む場合は、次の手順を行います。

1. Xresourcesをオーバーライドしてunclutterランチャープログラムに空の値を指定します。
  ```console
  $ echo "wm.program.unclutter: :" >> ~/.config/regolith3/Xresources
  ```
2. 変更を適用するため、ログアウトしてから戻ります。

