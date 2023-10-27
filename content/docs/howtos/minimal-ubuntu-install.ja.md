---
title: "最小構成のUbuntuにインストール"
description: >
  RegolithをUbuntu Serverにインストールする
---

このページではRegolithデスクトップをUbuntu Serverにインストールする方法について解説します。これにより、デスクトップでインストールされるいくつかの主要なGNOMEデスクトップパッケージを回避して最小構成でセットアップする方法を提供します。

# 手順

## 1. Ubuntu Serverをインストール

Ubuntu Serverの20.04か22.04のどちらかの新鮮なコピーをインストールするには、オンラインの説明書を参照してください。

## 2. Regolithのパッケージキーとaptリポジトリを追加

Ubuntu Serverのインストール後、ターミナルセッションにログインします。次のURLから、インストール方法のテキストファイルをダウンロードします。

Ubuntu 22.04: https://regolith-desktop.com/install-release-ubuntu-22.04-amd64.txt

Ubuntu 20.04: https://regolith-desktop.com/install-release-ubuntu-20.04-amd64.txt

例：

```console
wget https://regolith-desktop.com/install-release-ubuntu-22.04-amd64.txt
cat install-release-ubuntu-22.04-amd64.txt
```

テキストファイルの内容の各手順を手動で実行するか、挑戦的な人であればファイルの供給先を確保します。完了すれば、Regolithデスクトップのパッケージリポジトリが新しいシステムにインストールされます。

## 3. RegolithをUbuntuのシステムにインストール

`regolith-system-ubuntu`はISOで使用され、最小構成でのインストールにも利用できる特別なパッケージです。このパッケージは、複数のデスクトップ環境で共有される典型的なデスクトップでは利用されない追加のブランディングが含まれています。次のコマンドを実行してRegolithデスクトップとすべての依存関係をインストールします。

```console
sudo apt install regolith-system-ubuntu
```

## 4. 再起動

システムを再起動すると、`lightdm`ログインマネージャーが新規Regolith環境にログインできるようになります。
