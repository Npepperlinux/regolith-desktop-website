---
title: "アップストリームと動作を比較検証する"
description: >
  このページでは、オリジナルのバグの原因を掘り当てる方法について解説します。
---

{{< hint danger >}}
注意：このページは[Regolith 1.xのWebサイト](https://regolith-linux.org)からコピーされたもので、Regolith 2のものに更新されていません。古い情報が含まれている可能性があります。
{{< /hint >}}

Regolithはいくつかの既存のオープンソースプロジェクトといくつかの追加のカスタムパッケージによって成り立っています。Regolithで見つかったバグのいくつかは、実際にはアップストリームのプロジェクトのバグでもあります。 源流のバグであることを確定するのが、それらを修正するための最初の一歩です。

## `gnome-flashback`を確認する

多くのRegolithのGNOMEのサポートは`gnome-flashback`プロジェクトから由来しています。`gnome-flashback`セッションを実行するには、セッションをインストールしてログイン画面に戻り、セッションを選択してからアカウントにログインし直します。

1. `gnome-session-flashback`セッションをインストールする

```console
sudo apt install gnome-session-flashback
```

2. 再起動した後、`GNOME Flashback (Metacity)`セッションを選択する

{{< img "images/gnome-flashback-session-login.png" "">}}

3. 動作をRegolithと比較して検証します。`gnome-flashback`にも問題が存在している場合、そのバグは同じように動作します。`gnome-flashback`にバグが存在しなかった場合は、バグはRegolithに存在するようです。