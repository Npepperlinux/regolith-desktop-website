---
title: "ロック画面の壁紙のプログラムの変更"
description: >
  Regolithを`gnome-flashback`以外のロック画面を使用するように設定する
---

### 1. `gnome-flashback`をビルトインされたロック画面として無効にするよう設定する

Regolithの既定では`gnome-flashback`がロック画面として扱われています。これは`gsettings`コマンドラインプログラムによって設定を置き換えることができます。

```console
$ gsettings set org.gnome.gnome-flashback screensaver false
```

### 2. 使用したいロック画面プログラムがi3のキーバインドから実行するようにする

下記のように`~/.config/regolith3/Xresources`ファイルにオーバーライドを指定します（使用したいロック画面プログラムが記述された`your-script.sh`が置かれている場合）。

{{< hint warning >}}
Regolithバージョン3.0ではXresourceキーが"i3-wm"から"wm"に置き換えられます。このページの内容はRegolith 3.0以降のものに更新されています。それ以前のバージョンを使用する場合は、キーの名前を"wm"から"i3-wm"として使用してください。例として、Regolith 1.xと2.xでは`wm.foo.bar`は`i3-wm.foo.bar`に変更されます。
{{< /hint >}}

```toml
wm.program.lock: your-script.sh
```

例えば、`i3lock`がインストールされていると想定した場合：

```console
$ echo "wm.program.lock: /usr/bin/i3lock" >> ~/.config/regolith3/Xresources
```
