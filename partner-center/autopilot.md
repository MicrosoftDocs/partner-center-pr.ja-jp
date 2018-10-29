---
title: Windows Autopilot でデバイスのセットアップを効率化する | パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: Windows Autopilot でデバイスのセットアップを効率化するためにパートナー センターの Windows AutoPilot プロファイルを追加する
author: KPacquer
ms.author: kenpacq
keywords: autopilot、windows autopilot、microsoft autopilot、ゼロタッチ展開、oobe、ログイン画面
ms.localizationpriority: medium
ms.openlocfilehash: 2c8e8953fbb79493a3704c9c8ea6982928c3fe92
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/29/2018
ms.locfileid: "5796655"
---
# <a name="simplify-device-setup-with-windows-autopilot"></a>Windows Autopilot でデバイスのセットアップを効率化する 

Windows Autopilot によって、新しい Windows 10 Pro デバイスのセットアップを、最初のブートからほんの数ステップで効率的に実行し、セキュリティで保護することができます。 詳しくは、[Windows AutoPilot の概要に関するページ](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)ご覧ください。

## <a name="features"></a>機能

*  デバイスをセットアップするエンド ユーザーの**ローカル管理者のアクセス許可を無効にします**。
*  **組織のログイン ページを表示します**。 組織では、デバイスを作業デバイスとして追加し、デバイスを Azure Active Directory に追加するログオン ページがあらかじめ定義できます。
*  **デバイスを Mobile Device Manager (MDM) に登録します**。たとえば、OOBE が完了した後の Microsoft Intune。
*  Windows AutoPilot 展開プロフィルを使用して、必要なステップと意思決定のみが実行されるように **out-of-box experience (OOBE) を効率化します**。 

## <a name="requirements"></a>要件

*  Windows 10 Pro Creators Update (バージョン 1703 以降) または Windows 10 Pro for Advanced PC がプリインストールされているデバイス
*  ハードウェア ハッシュと呼ばれるデバイス識別子 (128 HWH または 4 k HWH)。通常、OEM によって提供されます。 識別子を使用して、パートナー センターで組織プロファイルを割り当てます。 
*  デバイスは、インターネットにアクセスできる必要があります。 デバイスが接続できない場合、既定の Windows の out-of-box experience (OOBE) 画面が表示されます。
*  デバイスを MDM に登録するには、Azure Active Directory Premium が必要です。

## <a name="add-organization-login-pages-to-oobe"></a>組織のログイン ページを OOBE に追加する

組織固有のページを追加するには、組織の [Azure AD ディレクトリ](https://go.microsoft.com/fwlink/?linkid=848958)にデバイスを追加し、ログイン ページを作成します。


## <a name="remove-windows-pages-from-oobe-with-a-windows-autopilot-deployment-profile"></a>Windows AutoPilot 展開プロファイルを使用して OOBE から Windows のページを削除する

**Windows AutoPilot 展開プロファイルの設定の例**
*  セットアップでプライバシー設定をスキップする
*  セットアップでローカル管理者アカウントを無効にする
*  セットアップで自動的にページをスキップする
   *  職場または学校用のセットアップを自動的に選択する
   *  Cortana、OneDrive、OEM 登録のセットアップのページをスキップする

### <a name="add-devices-and-apply-a-profile"></a>デバイスを追加し、プロファイルを適用する

パートナー センターでは、Windows AutoPilot 展開プロファイルを作成して、デバイスの一覧に適用します。

デバイスを構成するには、デバイスの一覧をアップロードし、デバイスに適用するプロファイルを作成して適用します。

1.  デバイスの一覧を追加します。

    (販売エージェントと管理エージェントが、パートナー センターにデバイスの一覧を追加するアクセス権を持っています)。
    
    間接リセラーは、間接プロバイダーと協力してこれを追加することができます。

    a.  [Windows AutoPilot の概要に関するページ](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)にあるトピックから、PowerShell スクリプトを使って .csv ファイルを作成します。 この .csv ファイルには、シリアル番号、OEM 名、モデル名、製品 ID、デバイス識別子などのデバイス情報が含まれています。 

    b.   パートナー センターから**お客様**に移動します。 >、デバイスを受け取る顧客を選択 >**デバイス > デバイスの追加**します。

    c.  デバイスのバッチに名前を付けます (例: "Contoso Sales Department PCs – April 2017 order")。 

    d.   **[参照]** をクリックし、デバイス情報ファイルを選択して **[検証]** をクリックします。

    **注:** .csv ファイルをアップロードしようとした後にエラー メッセージが表示される場合は、ファイルの形式を確認します。 8 月以降は、ハードウェア ハッシュのみを使う、OEM 名、シリアル番号、モデルを列の順序で使う、または Windows 製品 ID を使うことができます。 **[デバイスの追加]** の横のリンクから入手できる .csv ファイルを使うこともできます。

2.  デバイスに適用できるプロファイルを作成します。 (管理エージェントのみは、作成し、パートナー センターで、プロファイルを適用するアクセス権を持ちます)。

    a.   **[デバイス]** で、**[新しいプロファイルの追加]** をクリックします。

    b.   プロファイルに名前を付けます (例: "Contoso Desktop Profile – Skip All OOBE")。

    c.   OOBE の設定を構成します。 たとえば、**[セットアップで簡単設定をスキップする]** をオンにします。

    d.   **[送信]** をクリックします。

3.  プロファイルを適用します。

    a.   **[デバイス]** の **[デバイスの割り当てと削除]** ウィンドウで、構成するデバイスを選択します。 バッチ全体を選択するには、バッチ名 (例: "Contoso Sales Department PCs – March 2017 order") の横にあるチェック ボックスをオンにします。

    b.   **[プロファイルの適用]** をクリックし、プロファイル (例: "Contoso Desktop Profile – Skip All OOBE") を選択します。 デバイスの [プロファイル] 列にプロファイルが表示されます。

4.  省略可能: テストしてプロファイルが動作することを確認します。

    a.   デバイスをネットワークに接続し、電源をオンにします。

    b.   適切な OOBE 画面 (存在する場合) が表示されることを確認します。

    c.   新しいユーザー用のデバイスを準備するには、OOBE エクスペリエンスを完了し、デバイスを工場出荷時の既定の設定にリセットします。


## <a name="to-update-or-delete-a-profile"></a>プロファイルを更新または削除するには 

デバイスにプロファイルを割り当てた後、既にデバイスを顧客に付与した場合でも、プロファイルを更新できます。 デバイスがインターネットに接続されたときに、OOBE プロセスでプロファイルの最新バージョンがダウンロードされます。 顧客がデバイスで工場出荷時の既定の設定を復元した場合も、デバイスはプロファイルの最新の更新プログラムをダウンロードします。 

### <a name="you-can-remove-a-profile-from-a-device"></a>デバイスからプロファイルを削除することができます。
1. プロファイルを削除するデバイス (またはデバイスのバッチ) を選択します。 

2. **[デバイスの割り当てと削除]** ウィンドウで、**[プロファイルの削除]** を選択します。

3. 削除するプロファイルに移動し、プロファイルを削除します。 プロファイルは、すべてのデバイスから削除されます。

**[デバイス]** で、プロファイルを選択します。 ここから、既存の設定を変更することができます。

## <a name="windows-autopilot-eula-dismissal--important-information"></a>Windows AutoPilot での使用許諾契約の非表示 – 重要な情報

このツールを使用すると、お客様向けに管理しているデバイスで Windows の個別のインストールを構成することができます。 お客様の承認があれば、Windows のセットアップ時に通常はユーザーに対して表示される特定のセットアップ画面を非表示にすることができます。こうした画面には、使用許諾契約へ同意する画面も含まれます。 

この機能を使用することで、ユーザーに条項を通知して承諾を求める画面を非表示にした場合は、パートナー様が条項の非表示についてお客様から十分な同意と承認を得たものと見なされ、かつお客様が組織か個人ユーザーかを問わず、パートナー様がお客様の代理として、お客様に適用されるすべての条項の通知に同意し、これを承諾したものと見なされます。 これには、このツールによって画面を非表示にしない場合にユーザーに対して表示される、ライセンス契約条件や通知への同意を含みます。 お客様は、マイクロソフトまたはその認定代理店からソフトウェアのライセンスを正当に取得していない場合、デバイス上でその Windows ソフトウェアを使用することはできません。


