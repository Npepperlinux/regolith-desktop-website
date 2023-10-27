---
title: "既定でi3-barを非表示にする方法"
description: >
  i3-barを既定で非表示にする
---

{{< hint warning >}}
Regolithバージョン3.0ではXresourceキーが"i3-wm"から"wm"に置き換えられます。このページの内容はRegolith 3.0以降のものに更新されています。それ以前のバージョンを使用する場合は、キーの名前を"wm"から"i3-wm"として使用してください。例として、Regolith 1.xと2.xでは`wm.foo.bar`は`i3-wm.foo.bar`に変更されます。
{{< /hint >}}

`$HOME/.config/regolith3/Xresources`ファイルに
以下の行を追加します
```
wm.bar.mode: hide
```
次回ログイン時にはバーが既定で非表示になります。