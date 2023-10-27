---
title: "不要な依存関係の削除"
description: >
  Regolithで使用されていないデスクトップコンポーネントを削除する
---

RegolithをISOでインストールしたとき、既定では必要なデスクトップコンポーネントやパッケージのみがインストールされています。しかし、既に存在しているUbuntuシステムにRegolithをした場合、Regolithが必要としていないいくつかのデスクトップコンポーネントがシステムにインストールされたままになります。それらのパッケージをそのままにすることには何も問題はありませんが、既定のUbuntuセッションと同じ状態に戻すときに重要になる一方、多くのユーザーはそれらを削除することを好みます。

{{< hint danger >}}
注意：パッケージを削除することで予期しない動作や機能性が失われる原因になる可能性があります。
{{< /hint >}}

# LightDMをインストールする

`lightdm`ディスプレイマネージャーでは豊富な種類のテーマをインストールすることができますが、ここでは`regolith-lightdm-config`をインストールします。

```console
$ sudo apt install regolith-lightdm-config
```

パッケージの変更の認証をするため、`apt`の出力を確認してください。メニューが表示され、`gdm3`と`lightdm`のどちらかを選択するように求められるため、`lightdm`を選択します。

# 不要なパッケージを削除する

上記の手順により`lightdm`ディスプレイマネージャーを使用しているため、不要なパッケージを削除することができます。

```console
$ sudo apt remove gdm3 gnome-shell evolution-data-server*
```

パッケージの変更の認証をするため、`apt`の出力を確認してください。

これらのパッケージのすべての依存関係を削除することができます。

```console
$ sudo apt autoremove
```

# 再起動

この時点で、不要な依存関係をシステムから削除が完了しました。再起動して一連の処理が完了します。

# 取り消す

セットアップする前の状態に戻したい場合、次の内容を実行し、`gdm3`をディスプレイマネージャーとして選択します。

```console
$ sudo apt install gdm3 gnome-shell evolution-data-server ubuntu-session
$ sudo apt remove regolith-lightdm-session 
```
