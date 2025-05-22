---
title: "Regolithデスクトップ環境"
layout: "hextra-home"
---

{{< hextra/hero-container
  image="/images/v-tour/regolith-empty.png"
  imageTitle="Regolithデスクトップ環境"
  imageWidth="853"
>}}
{{< hextra/hero-badge link="/docs/reference/releases/regolith-3.2-release-notes" >}}
  <div class="hx-w-2 hx-h-2 hx-rounded-full hx-bg-primary-400"></div>
  <span>最新バージョン: v3.2</span>
  {{< icon name="arrow-circle-right" attributes="height=14" >}}
{{< /hextra/hero-badge >}}

<div class="hx-mt-6 hx-mb-6">
{{< hextra/hero-headline >}}
  Regolithデスクトップ環境
{{< /hextra/hero-headline >}}
</div>

<div class="hx-mt-6 hx-mb-6">
{{< hextra/hero-subtitle >}}
  生産性を重視したUbuntuディストリとデスクトップ環境
{{< /hextra/hero-subtitle >}}
</div>

<div class="hx-mt-6 hx-mb-6">
{{< hextra/hero-button text="始める" link="docs/" >}}
{{< hextra/hero-badge style="padding: 13px 12px !important; font-size: .875rem !important;" link="https://opencollective.com/regolith/donate" >}}
  <span>Regolithを支援する <img class="not-prose" style="display: inline; height: 22px;" src='https://badgen.net/opencollective/backers/regolith'/></span>
  {{< icon name="arrow-circle-right" attributes="height=14" >}}
{{< /hextra/hero-badge >}}
</div>
{{< /hextra/hero-container >}}

<div class="hx-mt-6"></div>
<div class="hx-mt-6"></div>
<div class="hx-mt-6"></div>

{{< hextra/feature-grid cols="2" >}}
  {{< hextra/feature-card
    title="生産性第一"
    subtitle="Regolithは、人気があり、高速で、構成しやすく、キーボードを中心とした生産的なワークフローに最適な、i3とSwayで実行されます。Regolithは、i3とSwayを、 `i3bar`、`rofication`、`i3status-rs`、`ilia`といった他のデスクトップコンポーネントと統合し、完全なデスクトップエクスペリエンスを提供します。"
  >}}

  {{< hextra/feature-card
    title="GNOMEのシステム管理"
    subtitle="軽量なウィンドウマネージャーを`gnome-session`と統合することで、Regolithは典型的な`gnome-shell`ベースの環境の複雑な点の多くを回避し、シンプルで一貫したシステム環境を提供します。"
  >}}
{{< /hextra/feature-grid >}}

<div class="hx-mt-6"></div>

{{< hextra/feature-grid cols="1" >}}
  {{< hextra/feature-card
    title="Regolithのインストール"
    link="/docs/using-regolith/install/"
    subtitle="Regolithデスクトップのインストール方法については<span class=\"regolith-links\">こちら</span>。"
  >}}
{{< /hextra/feature-grid >}}

<div class="hx-mt-6 hx-mb-6"></div>
<div class="hx-mt-6 hx-mb-6"></div>
{{< hextra/hero-section >}}
  ビジュアルツアー
{{< /hextra/hero-section >}}

{{< columns cols="2" >}}
  {{< column
      title="初回ログイン"
      border="true"
      image="/images/v-tour/regolith-ilia-keybindings.png"
  >}}
    初回ログイン時に、i3-wmで使用する最も重要なキーバインドをオーバーレイで表示します（{{< keys "super,?" >}}でいつでも切り替えられます）。
  {{< /column >}}

  {{< column
      title="ターミナル"
      border="true"
      image="/images/v-tour/regolith-floating-terminal.png"
  >}}
    ターミナル上で作業する人は、{{< keys "super,enter" >}}を押すことで作業に取り掛かることができます。
  {{< /column >}}

  {{< column
      title="アプリランチャー"
      border="true"
      image="/images/v-tour/regolith-ilia-apps.png"
  >}}
    プログラムを実行する単一のグローバルアプリランチャーが、{{< keys "super,space" >}}を押すことで、どこからでも、即座に利用することができます。
  {{< /column >}}

  {{< column
      title="レイアウト管理"
      border="true"
      image="/images/v-tour/regolith-desktop-terminals.png"
  >}}
    もっとターミナルが必要ですか？{{< keys "super,backspace" >}}と{{< keys "super,enter" >}}で水平・垂直モードを切り替えて、その場でレイアウトを作成できます。{{< keys "super,h,j,k,l" >}}でウィンドウの位置を移動できます。
  {{< /column >}}

  {{< column
    title="フローティングウィンドウ"
    border="true"
    image="/images/v-tour/regolith-floating-windows.png"
  >}}
    {{< keys "super,f" >}}でフローティングモードに切り替えることができます。{{< keys "super,r" >}}でウィンドウをリサイズし、{{< keys "super" >}}を押しながらマウスで移動させます。
  {{< /column >}}

  {{< column
      title="Gnomeのシステム管理"
      border="true"
      image="/images/v-tour/regolith-gnome-flashback.png"
  >}}
    Gnome Flashbackは一貫したシンプルなシステム環境を提供します。 UIの調整、USBドライブの自動マウント、ワイヤレスネットワークへの接続を行います。{{< keys "super,c" >}}からコントロールパネルを起動することができます。
  {{< /column >}}

  {{< column
      title="Regolith Look"
      border="true"
      image="/images/v-tour/regolith-screenshot-look-selector.png"
  >}}
    <code>regolith-look</code>コマンドで、<a href="https://ethanschoonover.com/solarized" class="regolith-links">Solarized</a> や他の外観に簡単に切り替えられます。<b>looks</b>ではパッケージマネージャを利用するため、使用するテーマリソースのみを保存します。 
  {{< /column >}}

  {{< column
      title="探して操作"
      border="true"
      image="/images/v-tour/regolith-ilia-windows.png"
  >}}
    もっとやりたいことがありますか？{{< keys "super,ctrl,space" >}}や{{< keys "super,[0 - 19]" >}}を押すことで、瞬時に必要なウィンドウを見つけることができます。
  {{< /column >}}

  {{< column
      title="間隔の管理"
      border="true"
      image="/images/v-tour/regolith-many-windows.png"
  >}}
    無駄なUIを省き、ウィンドウレイアウトを細かく管理することなく、ピクセル単位で活用することができます。
  {{< /column >}}

  {{< column
      title="通知"
      border="true"
      image="/images/v-tour/regolith-ilia-notifications.png"
  >}}
    デスクトップ通知は注意を引こうと競合することなく、{{< keys "super,n" >}}を押して画面上のダイアログで管理することが可能です。
  {{< /column >}}
{{< /columns >}}
