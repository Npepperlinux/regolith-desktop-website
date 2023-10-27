---
title: "Swayコンポジターのインストール"
description: >
  RegolithセッションをWaylandベースのセッションにアップグレードする
---


Waylandセッションのインストールは、次の手順で行うことができます。

1. `regolith-session-sway`パッケージと依存関係をインストール
2. 再起動
3. ログインパネルで"Regolith on Wayland"セッションを選択

## ハードウェアサポート

NVIDIAのグラフィックカードでプロプライエタリなNVIDIAドライバを使用するには、XResourcesで`regolith.sway.unsupported_gpu: true`を設定しなければなりません。この問題はオープンソースドライバのnouveauにはありません。詳しくは[こちら](https://github.com/swaywm/sway/issues/5392)。

## バーの変更

Waylandセッションでは`i3xrocks`の代わりに[`i3status-rs`](https://github.com/greshake/i3status-rust)が使用されます。  `i3status-rs`は、システムモニタリングで明確にリソース効率の高いアプローチを提供します。しかしながら、現時点でステータスインジケーターの`i3xrocks`パッケージは`i3status-rs`と統合されていません。`i3status-rs`でカスタム設定を使用するには、ユーザーが選択した設定ファイルを特定の場所に置き、XResourcesで`wm.bar.status_config`に設定ファイルの絶対パスを設定する必要があります。詳しくは[アップストリームプロジェクトのドキュメント](https://docs.rs/i3status-rs/latest/i3status_rs/blocks/index.html)を参照してください。
