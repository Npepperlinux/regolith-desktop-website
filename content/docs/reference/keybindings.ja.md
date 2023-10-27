---
title: "キーバインド"
linkTitle: "Keybindings"
weight: 1
description: >
  Regolithで既定で提供されるキーマップ
---

| 動作                                                                             | キーバインド                    |
| ---------------------------------------------------------------------------------- | ------------------------------ |
| [ 起動 - アプリケーション ](#LaunchApplication)                                       | `⊞ Win` Space                  |
| [ 起動 - ブラウザ ](#LaunchBrowser)                                               | `⊞ Win` `Shift` Enter          |
| [ 起動 - コマンド ](#LaunchCommand)                                               | `⊞ Win` `Shift` Space          |
| [ 起動 - ファイルブラウザ ](#LaunchFileBrowser)                                      | `⊞ Win` `Shift` n              |
| [ 起動 - ファイル検索 ](#LaunchFileSearch)                                        | `⊞ Win` `Alt` Space            |
| [ 起動 - 通知ビューワー ](#LaunchNotificationViewer)                        | `⊞ Win` n                      |
| [ 起動 - ターミナル ](#LaunchTerminal)                                             | `⊞ Win` Enter                  |
| [ 起動 - このダイアログ ](#LaunchThisDialog)                                        | `⊞ Win` `Shift` ?              |
| [ 修正 - Bluetooth設定 ](#ModifyBluetoothSettings)                          | `⊞ Win` b                      |
| [ 修正 - ウィンドウとワークスペース1~10に移動 ](#ModifyCarryWindowtoWorkspace1-10)    | `⊞ Win` `Alt` 0..9             |
| [ 修正 - ウィンドウとワークスペース11~19に移動 ](#ModifyCarryWindowtoWorkspace11-19) | `⊞ Win` `Alt` `Ctrl` 1..9      |
| [ 修正 - ウィンドウをワークスペースごと移動 ](#ModifyContainingWorkspace)                      | `⊞ Win` `Ctrl` `Shift` ↑ ↓ ← → |
| [ 修正 - ディスプレイ設定 ](#ModifyDisplaySettings)                              | `⊞ Win` d                      |
| [ 修正 - ウィンドウレイアウトの読み込み ](#ModifyLoadWindowLayout)                           | `⊞ Win` .                      |
| [ 修正 - ウィンドウをワークスペース1~10に移動 ](#ModifyMoveWindowtoWorkspace1-10)     | `⊞ Win` `Shift` 0..9           |
| [ 修正 - ウィンドウをワークスペース11~19に移動](#ModifyMoveWindowtoWorkspace11-19)    | `⊞ Win` `Ctrl` `Shift` 1..9    |
| [ 修正 - スクラッチパッドに移動 ](#ModifyMovetoScratchpad)                           | `⊞ Win` `Ctrl` m               |
| [ 修正 - 次のウィンドウの向き ](#ModifyNextWindowOrientation)                 | `⊞ Win` Backspace              |
| [ 修正 - ウィンドウレイアウトの保存 ](#ModifySaveWindowLayout)                           | `⊞ Win` ,                      |
| [ 修正 - 設定 ](#ModifySettings)                                             | `⊞ Win` c                      |
| [ 修正 - フォーカスをタイルとフローティング間で切り替え ](#ModifyTile/FloatFocusToggle)                 | `⊞ Win` `Shift` t              |
| [ 修正 - バーの切り替え ](#ModifyToggleBar)                                          | `⊞ Win` i                      |
| [ 修正 - Wi-Fi設定 ](#ModifyWifiSettings)                                    | `⊞ Win` w                      |
| [ 修正 - フローティングウィンドウの切り替え ](#ModifyWindowFloatingToggle)                   | `⊞ Win` `Shift` f              |
| [ 修正 - 全画面表示の切り替え ](#ModifyWindowFullscreenToggle)               | `⊞ Win` f                      |
| [ 修正 - ウィンドウレイアウトのモード ](#ModifyWindowLayoutMode)                           | `⊞ Win` t                      |
| [ 修正 - ウィンドウ位置 ](#ModifyWindowPosition)                                | `⊞ Win` `Shift` k j h l        |
| [ 修正 - ウィンドウ位置 ](#ModifyWindowPosition)                                | `⊞ Win` `Shift` ↑ ↓ ← →        |
| [ 操作 - 次のワークスペース ](#NavigateNextWorkspace)                              | `⊞ Win` Tab                    |
| [ 操作 - 次のワークスペース ](#NavigateNextWorkspace)                              | `⊞ Win` `Alt` →                |
| [ 操作 - 前のワークスペース ](#NavigatePreviousWorkspace)                      | `⊞ Win` `Alt` ←                |
| [ 操作 - 前のワークスペース ](#NavigatePreviousWorkspace)                      | `⊞ Win` `Shift` Tab            |
| [ 操作 - ウィンドウサイズの比較 ](#NavigateRelativeWindow)                            | `⊞ Win` k j h l                |
| [ 操作 - ウィンドウサイズの比較 ](#NavigateRelativeWindow)                            | `⊞ Win` ↑ ↓ ← →                |
| [ 操作 - スクラッチパッド ](#NavigateScratchpad)                                     | `⊞ Win` `Ctrl` a               |
| [ 操作 - ウィンドウのリスト ](#NavigateWindowbyName)                               | `⊞ Win` `Ctrl` Space           |
| [ 操作 - ワークスペース11~19 ](#NavigateWorkspace11-19)                          | `⊞ Win` `Ctrl` 1..9            |
| [ 操作 - ワークスペース1~10 ](#NavigateWorkspaces1-10)                            | `⊞ Win` 0..9                   |
| [ リサイズ - リサイズモードを開始 ](#ResizeEnterResizeMode)                             | `⊞ Win` r                      |
| [ セッション - アプリを終了 ](#SessionExitApp)                                            | `⊞ Win` `Shift` q              |
| [ セッション - 画面のロック ](#SessionLockScreen)                                      | `⊞ Win` Escape                 |
| [ セッション - ログアウト ](#SessionLogout)                                               | `⊞ Win` `Shift` e              |
| [ セッション - 電源オフ ](#SessionPowerDown)                                        | `⊞ Win` `Shift` p              |
| [ セッション - 再起動 ](#SessionReboot)                                               | `⊞ Win` `Shift` b              |
| [ セッション - セッションのリフレッシュ ](#SessionRefreshSession)                              | `⊞ Win` `Shift` r              |
| [ セッション - i3設定の再読み込み ](#SessionReloadi3Config)                             | `⊞ Win` `Shift` c              |
| [ セッション - i3の再起動 ](#SessionRestarti3)                                        | `⊞ Win` `Ctrl` r               |
| [ セッション - スリープ ](#SessionSleep)                                                 | `⊞ Win` `Shift` s              |
| [ セッション - アプリの中断 ](#SessionTerminateApp)                                  | `⊞ Win` `Alt` q                |
