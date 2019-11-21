---
title: Windows Autopilot プロファイルでデバイスの out-of-box experience をカスタマイズする | パートナー センター
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn how to customize or pre-configure a new device's out-of-box experience with Autopilot profiles before you deliver the device to the customer.
author: maggiepuccievans
ms.author: evansma
keywords: Autopilot, Windows Autopilot, Microsoft Autopilot, ゼロタッチ展開, OOBE, ログイン画面, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: a07c18fda7de0aa5854fb46a91bea692c033d51c
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253333"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Windows Autopilot プロファイルでデバイスの out-of-box experience をカスタマイズする

**適用対象**

- CSP 直接請求パートナー、間接プロバイダー、間接リセラー

顧客のデバイスを管理する場合、顧客のユーザーの out-of-box experience (OOBE) をカスタマイズすることが必要な場合があります。 顧客にデバイスを提供する前に Windows Autopilot プロファイルを使用して新しいデバイスを事前に構成し、顧客が既に購入したデバイスに新しいプロファイルを適用することができます。 

Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)** .  This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.

この記事では、パートナー センターで Autopilot プロファイルを作成してデバイスに適用する方法について説明します。

まだ Autopilot に慣れていない場合は、次の記事の情報を確認してください。

- [Windows Autopilot の概要](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Autopilot 展開リファレンス ガイド](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>概要

パートナー センターで Windows Autopilot の機能を使うと、カスタム プロファイルを作成し、顧客のデバイスに適用することができます。 この記事を公開した時点では、次のプロファイル設定を使用できました。

- プライバシーの設定をスキップします。 この Autopilot プロファイルのオプションの設定を使うと、OOBE プロセスの間は、プライバシーの設定について組織による確認は行われません。

- デバイスでローカル管理者アカウントの作成を無効にします。 デバイスをセットアップするユーザーがプロセス完了後に管理者アクセス権を持つ必要があるかどうかについて、組織による決定が可能です。

- 職場または学校用のデバイスを自動的にセットアップします。 Autopilot で登録されるすべてのデバイスは、自動的に職場または学校のデバイスと見なされるため、OOBE プロセスではの質問はありません。

- Cortana、OneDrive、OEM 登録のセットアップのページをスキップします。 Autopilot で登録されるすべてのデバイスでは、out-of-box experience (OOBE) プロセスの間にこれらのページが自動的にスキップされます。

- 使用許諾契約 (EULA) をスキップします。 Windows 10 バージョン 1709 以降では、OOBE プロセスの間に表示される EULA ページをスキップすることについて、組織による決定が可能です。 Windows セットアップ中の EULA ページのスキップに関して考慮する必要のある重要な情報については、後出の「[Windows AutoPilot での使用許諾契約の非表示](#windows-autopilot-eula-dismissal)」を参照してください。

以下のプロファイルおよびデバイス管理のアクセス許可と制限事項が適用されます。

- CSP パートナーは、リセラー関係のある既存の顧客がパートナーの代理管理特権を削除した場合でも、顧客の Autopilot プロファイルを、引き続き管理できます。

- パートナーは、自分で追加した顧客の既存のデバイスを管理できます。

- You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>パートナー センターで Autopilot プロファイルを作成および管理する

パートナー センターで、Windows Autopilot 展開プロファイルを作成し、デバイスにそれらを適用できます。

>[!NOTE]
>プロファイルを作成して適用できるのは、管理エージェントだけです。

### <a name="create-a-new-autopilot-profile"></a>新しい Autopilot プロファイルを作成する

1. パートナー センター メニューで **[顧客]** を選択し、Autopilot プロファイルを作成する顧客を選択します。

2. 顧客の詳細ページで、 **[デバイス]** を選択します。

3. **[Windows Autopilot プロファイル]** で **[新しいプロファイルの追加]** を選択します。

4. プロファイルの名前と説明を入力し、OOBE の設定を構成します。 以下から選択します。  

   - セットアップでプライバシーの設定をスキップする

   - セットアップでローカル管理者アカウントを無効にする
  
   - セットアップで自動的にページをスキップする<br>
        ("*職場または学校のために自動的に設定を選択する*" と "*Cortana、OneDrive、OEM 登録のセットアップのページをスキップする*" が含まれます)
  
   - 使用許諾契約 (EULA) をスキップする<br> 
       >[!IMPORTANT] 
       >Windows セットアップ中の EULA ページのスキップに関して考慮する必要のある重要な情報については、後出の「[Windows AutoPilot での使用許諾契約の非表示](#windows-autopilot-eula-dismissal)」を参照してください。

5. 完了したら、 **[送信]** を選びます。

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Autopilot プロファイルを顧客のデバイスに適用する

>[!NOTE]
>以下の説明では、顧客のデバイスをパートナー センターに既に追加してあり、顧客のデバイス一覧にアクセスできるものとします。 顧客のデバイスをまだ追加していない場合は、「[顧客のアカウントにデバイスを追加する](#add-devices-to-a-customers-account)」の説明に従った後、以下の手順のようにします。

顧客の Autopilot プロファイルを作成した後は、顧客のデバイスにそれを適用できます。

1. パートナー センターのメニューで **[顧客]** を選択し、Autopilot プロファイル作成の対象となる顧客を選択します。

2. 顧客の詳細ページで、 **[デバイス]** を選択します。

3. **[デバイスへのプロファイルの適用]** でプロファイルを追加するデバイスまたはデバイス グループを選択してから、 **[プロファイルの適用]** を選択します。 適用したプロファイルが、 **[プロファイル]** 列に表示されます。

4. 次の手順に従って、プロファイルがデバイスに正常に適用されたことを確認します。

    」を参照します。  デバイスをネットワークに接続し、電源をオンにします。

    b.  適切な OOBE 画面 (存在する場合) が表示されることを確認します。

    c.  OOBE プロセスが停止したら、デバイスを工場出荷時の既定の設定にリセットして、新しいユーザー用に準備します。

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>顧客のデバイスから Autopilot プロファイルを削除する

1. パートナー センターのメニューで **[顧客]** を選択し、Autopilot プロファイル作成の対象となる顧客を選択します。

2. 顧客の詳細ページで、 **[デバイス]** を選択します。

3. **[デバイスへのプロファイルの適用]** でプロファイルを削除するデバイスを選択してから、 **[プロファイルの削除]** を選択します。

   >[!NOTE]
   >デバイスからプロファイルを削除しても、一覧からプロファイルが削除されることはありません。 プロファイルを削除する場合は、「[Autopilot プロファイルを更新または削除する](#update-or-delete-an-autopilot-profile)」での説明のようにします。

### <a name="update-or-delete-an-autopilot-profile"></a>Autopilot プロファイルを更新または削除する

顧客にデバイスを出荷した後で、顧客が out-of-box experience の変更を希望した場合は、パートナー センターでプロファイルを変更できます。

顧客がデバイスをインターネットに接続すると、OOBE プロセスの間にプロファイルの最新バージョンがダウンロードされます。 また、顧客がデバイスを工場出荷時の既定の設定に戻したときも、やはり OOBE プロセスの間にプロファイルの最新バージョンがデバイスにダウンロードされます。

1. パートナー センターのメニューで **[顧客]** を選択し、Autopilot プロファイルの変更を希望している顧客を選択します。

2. 顧客の詳細ページで、 **[デバイス]** を選択します。

3. **[Windows Autopilot プロファイル]** で、更新する必要があるプロファイルを選択します。 必要な変更を行った後、 **[送信]** を選択します。

このプロファイルを削除するには、ページの右上隅にある **[プロファイルの削除]** を選択します。

### <a name="add-devices-to-a-customers-account"></a>顧客のアカウントにデバイスを追加する

>[!NOTE]
>販売エージェントと管理エージェントは、顧客のアカウントにデバイスを追加できます。

顧客のデバイスにカスタム Autopilot プロファイルを適用するためには、顧客のデバイス一覧にアクセスできる必要があります。

OEM 名、シリアル番号、モデルの組み合わせを使う場合は、次の制限事項に注意してください。

- この組み合わせは、新しいデバイス (4 k ハッシュなど) でのみ動作し、128b ハッシュ (RS2 以前のデバイス) に対してはサポートされていません。

- 組み合わせの登録では大文字と小文字が区別されるため、ファイル内のデータが、OEM プロバイダー (ハードウェア プロバイダー) によって提供されるモデルおよび製造元の名前と "***正確に***" 一致する必要があります。

パートナー センターで顧客のアカウントにデバイスを追加するには、以下の手順に従います。

1. パートナー センターのメニューで **[顧客]** を選択し、デバイスが管理対象となる顧客を選択します。

2. 顧客の詳細ページで、 **[デバイス]** を選択します。

3. **[デバイスへのプロファイルの適用]** で **[デバイスの追加]** を選択します。

4. デバイス一覧の名前を入力し、 **[参照]** を選択して、顧客の一覧 (.csv ファイル形式) をパートナー センターにアップロードします。

    >[!NOTE]
    >この .csv ファイルは、デバイスを購入したときに受け取っているはずです。 .csv ファイルを受け取っていない場合は、「[Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)」 (Windows Autopilot にデバイスを追加する) の手順に従って自分で作成できます。  

5. .csv ファイルをアップロードし、 **[保存]** を選択します。

.csv ファイルをアップロードしようとするとエラー メッセージが表示される場合は、ファイルの形式を確認します。 ハードウェア ハッシュのみ、OEM 名とシリアル番号とモデル (その列の順序で)、または Windows 製品 ID を使用することができます。 **[デバイスの追加]** の横にあるリンクで提供されているサンプルの .csv ファイルを使用して、デバイス一覧を作成することもできます。

Your .csv file should look something like this:

> **Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**

> **{serialNumber},,,Microsoft Corporation,Surface Laptop**

Note that "Manufacturer name" and "Device model" are case-sensitive.

If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows AutoPilot での使用許諾契約の非表示

### <a name="important-information"></a>重要な情報

Windows Autopilot を使用すると、顧客向けに管理しているデバイスで Windows のカスタマイズしたインストールを構成することができます。 顧客が承認した場合は、Windows のセットアップ時に通常はユーザーに対して表示される特定のセットアップ画面を非表示にすることができます。これには、EULA (使用許諾契約) の同意画面が含まれます。

この機能を使用することで、ユーザーに条項を通知して承諾を求める画面を非表示にした場合は、パートナーが条項の非表示について顧客から十分な同意と承認を得たものと見なされ、かつ顧客が組織か個人ユーザーかを問わず、パートナーが顧客の代理として、顧客に適用されるすべての条項の通知に同意し、これを承諾したものと見なされます。 これには、このツールによって画面を非表示にしない場合にユーザーに対して表示される、ライセンス契約条件や通知への同意を含みます。 お客様は、マイクロソフトまたはその認定代理店からソフトウェアのライセンスを正当に取得していない場合、デバイス上でその Windows ソフトウェアを使用することはできません。
