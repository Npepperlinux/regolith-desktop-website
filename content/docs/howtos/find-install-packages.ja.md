---
title: "パッケージの検索とインストール"
description: >
  パッケージを検索してシステムにインストールする。
---

{{< hint danger >}}
注意：このページは[Regolith 1.xのWebサイト](https://regolith-linux.org)からコピーされたもので、Regolith 2のものに更新されていません。古い情報が含まれている可能性があります。
{{< /hint >}}

RegolithはDebianベースのシステムです。Debianのパッケージングツールはパッケージの検索とインストールに利用することができます。

# コマンドラインでパッケージを検索する

`apt`コマンドはインストール済みのパッケージもしくはすべてのパッケージの検索に利用することができます。

```console
$ apt list --installed <package name> # finds installed packages
$ apt list <package name> # finds all packages
```

例として、インストール可能なRegolith公式の外観をリスト表示するには、次のコマンドを実行します。

```console
$ apt list regolith-look-*
...
```

システムにインストールされたステータスインジケーターを表示するには、次のコマンドを実行します。

```console
$ apt list --installed i3xrocks-*
```

# コマンドラインでパッケージをインストールする

コマンドラインでパッケージをインストールするには、再度`apt`コマンドを使用しますが、インストール時にはsudoを使用しなければなりません。

```console
$ sudo apt install <package name>
```

バッテリーステータスインジケーターをインストールするには、次のコマンドを実行します。

```console
$ sudo apt install i3xrocks-battery
```

# GUIアプリでパッケージの検索とインストールをする

`synaptic`といった、aptパッケージングシステムをより良いインターフェース上で利用できるアプリがいくつも存在します。パッケージの検索やインストールの方法について知るには、選択したツールのドキュメントを参照してください。
