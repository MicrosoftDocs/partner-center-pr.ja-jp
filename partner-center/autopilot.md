---
title: デバイスの既定のエクスペリエンスをカスタマイズする
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: お客様の新しいデバイスを提供する前に、Windows 自動操縦プロファイルを使用して、デバイスの既定のエクスペリエンス (OOBE) をカスタマイズまたは事前構成できます。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 5294495403be729adecb5a7814ade4f9d454a0f6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149827"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="0157b-103">新しいデバイスで Windows Autopilot プロファイルを使用して、顧客の既定のエクスペリエンスをカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="0157b-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="0157b-104">**適切なロール**: 管理エージェント |全体管理者 |Sales agent |ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="0157b-104">**Appropriate roles**: Admin agent | Global admin | Sales agent | User management admin</span></span>

<span data-ttu-id="0157b-105">顧客のデバイスを管理する場合、顧客のユーザーの out-of-box experience (OOBE) をカスタマイズすることが必要な場合があります。</span><span class="sxs-lookup"><span data-stu-id="0157b-105">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="0157b-106">顧客にデバイスを提供する前に Windows Autopilot プロファイルを使用して新しいデバイスを事前に構成し、顧客が既に購入したデバイスに新しいプロファイルを適用することができます。</span><span class="sxs-lookup"><span data-stu-id="0157b-106">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="0157b-107">Oem は、デバイスの **プロダクトキー id (pkid)** を表示する [自動操縦デバイス] ボックスの外側に出荷ラベルを含めることを開始したことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="0157b-107">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="0157b-108">この1次元の読み取り可能なバーコードを使用すると、ダウンストリームパートナーは、デバイスをボックスにボックスを解除してデバイス ID を別の方法で収集することなく、デバイスを自動操縦用に登録することができます。</span><span class="sxs-lookup"><span data-stu-id="0157b-108">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="0157b-109">この記事では、パートナー センターで Autopilot プロファイルを作成してデバイスに適用する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="0157b-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="0157b-110">まだ Autopilot に慣れていない場合は、次の記事の情報を確認してください。</span><span class="sxs-lookup"><span data-stu-id="0157b-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="0157b-111">Windows Autopilot の概要</span><span class="sxs-lookup"><span data-stu-id="0157b-111">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="0157b-112">Autopilot 展開リファレンス ガイド</span><span class="sxs-lookup"><span data-stu-id="0157b-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="0157b-113">概要</span><span class="sxs-lookup"><span data-stu-id="0157b-113">Overview</span></span>

<span data-ttu-id="0157b-114">パートナー センターで Windows Autopilot の機能を使うと、カスタム プロファイルを作成し、顧客のデバイスに適用することができます。</span><span class="sxs-lookup"><span data-stu-id="0157b-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="0157b-115">この記事を公開した時点では、次のプロファイル設定を使用できました。</span><span class="sxs-lookup"><span data-stu-id="0157b-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="0157b-116">プライバシーの設定をスキップします。</span><span class="sxs-lookup"><span data-stu-id="0157b-116">Skip privacy settings.</span></span> <span data-ttu-id="0157b-117">この Autopilot プロファイルのオプションの設定を使うと、OOBE プロセスの間は、プライバシーの設定について組織による確認は行われません。</span><span class="sxs-lookup"><span data-stu-id="0157b-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="0157b-118">デバイスでローカル管理者アカウントの作成を無効にします。</span><span class="sxs-lookup"><span data-stu-id="0157b-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="0157b-119">デバイスをセットアップするユーザーがプロセス完了後に管理者アクセス権を持つ必要があるかどうかについて、組織による決定が可能です。</span><span class="sxs-lookup"><span data-stu-id="0157b-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="0157b-120">職場または学校用のデバイスを自動的にセットアップします。</span><span class="sxs-lookup"><span data-stu-id="0157b-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="0157b-121">Autopilot で登録されるすべてのデバイスは、自動的に職場または学校のデバイスと見なされるため、OOBE プロセスではの質問はありません。</span><span class="sxs-lookup"><span data-stu-id="0157b-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="0157b-122">Cortana、OneDrive、OEM 登録のセットアップのページをスキップします。</span><span class="sxs-lookup"><span data-stu-id="0157b-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="0157b-123">Autopilot で登録されるすべてのデバイスでは、out-of-box experience (OOBE) プロセスの間にこれらのページが自動的にスキップされます。</span><span class="sxs-lookup"><span data-stu-id="0157b-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="0157b-124">使用許諾契約 (EULA) をスキップします。</span><span class="sxs-lookup"><span data-stu-id="0157b-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="0157b-125">Windows 10 バージョン 1709 以降では、OOBE プロセスの間に表示される EULA ページをスキップすることについて、組織による決定が可能です。</span><span class="sxs-lookup"><span data-stu-id="0157b-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="0157b-126">Windows セットアップ中の EULA ページのスキップに関して考慮する必要のある重要な情報については、後出の「[Windows AutoPilot での使用許諾契約の非表示](#windows-autopilot-eula-dismissal)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0157b-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="0157b-127">以下のプロファイルおよびデバイス管理のアクセス許可と制限事項が適用されます。</span><span class="sxs-lookup"><span data-stu-id="0157b-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="0157b-128">CSP パートナーは、リセラー関係のある既存の顧客がパートナーの代理管理特権を削除した場合でも、顧客の Autopilot プロファイルを、引き続き管理できます。</span><span class="sxs-lookup"><span data-stu-id="0157b-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="0157b-129">パートナーは、自分で追加した顧客の既存のデバイスを管理できます。</span><span class="sxs-lookup"><span data-stu-id="0157b-129">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="0157b-130">顧客がビジネス向け Microsoft Store または Microsoft Intune ポータルにアップロードしたデバイスを管理することはできません。</span><span class="sxs-lookup"><span data-stu-id="0157b-130">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="0157b-131">パートナー センターで Autopilot プロファイルを作成および管理する</span><span class="sxs-lookup"><span data-stu-id="0157b-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="0157b-132">パートナー センターで、Windows Autopilot 展開プロファイルを作成し、デバイスにそれらを適用できます。</span><span class="sxs-lookup"><span data-stu-id="0157b-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="0157b-133">プロファイルを作成して適用できるのは、管理エージェントだけです。</span><span class="sxs-lookup"><span data-stu-id="0157b-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="0157b-134">新しい Autopilot プロファイルを作成する</span><span class="sxs-lookup"><span data-stu-id="0157b-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="0157b-135">パートナー センター メニューで **[顧客]** を選択し、Autopilot プロファイルを作成する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="0157b-136">顧客の詳細ページで、**[デバイス]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="0157b-137">**[Windows Autopilot プロファイル]** で **[新しいプロファイルの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="0157b-138">プロファイルの名前と説明を入力し、OOBE の設定を構成します。</span><span class="sxs-lookup"><span data-stu-id="0157b-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="0157b-139">次の中から選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-139">Choose from:</span></span>  

   - <span data-ttu-id="0157b-140">セットアップでプライバシーの設定をスキップする</span><span class="sxs-lookup"><span data-stu-id="0157b-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="0157b-141">セットアップでローカル管理者アカウントを無効にする</span><span class="sxs-lookup"><span data-stu-id="0157b-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="0157b-142">セットアップで自動的にページをスキップする</span><span class="sxs-lookup"><span data-stu-id="0157b-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="0157b-143">("*職場または学校のために自動的に設定を選択する*" と "*Cortana、OneDrive、OEM 登録のセットアップのページをスキップする*" が含まれます)</span><span class="sxs-lookup"><span data-stu-id="0157b-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="0157b-144">使用許諾契約 (EULA) をスキップする</span><span class="sxs-lookup"><span data-stu-id="0157b-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="0157b-145">Windows セットアップ中の EULA ページのスキップに関して考慮する必要のある重要な情報については、後出の「[Windows AutoPilot での使用許諾契約の非表示](#windows-autopilot-eula-dismissal)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0157b-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="0157b-146">完了したら、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="0157b-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="0157b-147">Autopilot プロファイルを顧客のデバイスに適用する</span><span class="sxs-lookup"><span data-stu-id="0157b-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="0157b-148">以下の説明では、顧客のデバイスをパートナー センターに既に追加してあり、顧客のデバイス一覧にアクセスできるものとします。</span><span class="sxs-lookup"><span data-stu-id="0157b-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="0157b-149">顧客のデバイスをまだ追加していない場合は、「[顧客のアカウントにデバイスを追加する](#add-devices-to-a-customers-account)」の説明に従った後、以下の手順のようにします。</span><span class="sxs-lookup"><span data-stu-id="0157b-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="0157b-150">顧客の Autopilot プロファイルを作成した後は、顧客のデバイスにそれを適用できます。</span><span class="sxs-lookup"><span data-stu-id="0157b-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="0157b-151">パートナー センターのメニューで **[顧客]** を選択し、Autopilot プロファイル作成の対象となる顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="0157b-152">顧客の詳細ページで、**[デバイス]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="0157b-153">**[デバイスへのプロファイルの適用]** でプロファイルを追加するデバイスまたはデバイス グループを選択してから、**[プロファイルの適用]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="0157b-154">適用したプロファイルが、**[プロファイル]** 列に表示されます。</span><span class="sxs-lookup"><span data-stu-id="0157b-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="0157b-155">次の手順に従って、プロファイルがデバイスに正常に適用されたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="0157b-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="0157b-156">a.</span><span class="sxs-lookup"><span data-stu-id="0157b-156">a.</span></span>  <span data-ttu-id="0157b-157">デバイスをネットワークに接続し、電源をオンにします。</span><span class="sxs-lookup"><span data-stu-id="0157b-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="0157b-158">b.</span><span class="sxs-lookup"><span data-stu-id="0157b-158">b.</span></span>  <span data-ttu-id="0157b-159">適切な OOBE 画面 (存在する場合) が表示されることを確認します。</span><span class="sxs-lookup"><span data-stu-id="0157b-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="0157b-160">c.</span><span class="sxs-lookup"><span data-stu-id="0157b-160">c.</span></span>  <span data-ttu-id="0157b-161">OOBE プロセスが停止したら、デバイスを工場出荷時の既定の設定にリセットして、新しいユーザー用に準備します。</span><span class="sxs-lookup"><span data-stu-id="0157b-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="0157b-162">顧客のデバイスから Autopilot プロファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="0157b-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="0157b-163">パートナー センターのメニューで **[顧客]** を選択し、Autopilot プロファイル作成の対象となる顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="0157b-164">顧客の詳細ページで、**[デバイス]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="0157b-165">**[デバイスへのプロファイルの適用]** でプロファイルを削除するデバイスを選択してから、**[プロファイルの削除]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="0157b-166">デバイスからプロファイルを削除しても、一覧からプロファイルが削除されることはありません。</span><span class="sxs-lookup"><span data-stu-id="0157b-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="0157b-167">プロファイルを削除する場合は、「[Autopilot プロファイルを更新または削除する](#update-or-delete-an-autopilot-profile)」での説明のようにします。</span><span class="sxs-lookup"><span data-stu-id="0157b-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="0157b-168">Autopilot プロファイルを更新または削除する</span><span class="sxs-lookup"><span data-stu-id="0157b-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="0157b-169">顧客にデバイスを出荷した後で、顧客が out-of-box experience の変更を希望した場合は、パートナー センターでプロファイルを変更できます。</span><span class="sxs-lookup"><span data-stu-id="0157b-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="0157b-170">顧客がデバイスをインターネットに接続すると、OOBE プロセスの間にプロファイルの最新バージョンがダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="0157b-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="0157b-171">また、顧客がデバイスを工場出荷時の既定の設定に戻したときも、やはり OOBE プロセスの間にプロファイルの最新バージョンがデバイスにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="0157b-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="0157b-172">パートナー センターのメニューで **[顧客]** を選択し、Autopilot プロファイルの変更を希望している顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="0157b-173">顧客の詳細ページで、**[デバイス]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="0157b-174">**[Windows Autopilot プロファイル]** で、更新する必要があるプロファイルを選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="0157b-175">必要な変更を行った後、**[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="0157b-176">このプロファイルを削除するには、ページの右上隅にある **[プロファイルの削除]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="0157b-177">顧客のアカウントにデバイスを追加する</span><span class="sxs-lookup"><span data-stu-id="0157b-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="0157b-178">販売エージェントと管理エージェントは、顧客のアカウントにデバイスを追加できます。</span><span class="sxs-lookup"><span data-stu-id="0157b-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="0157b-179">顧客のデバイスにカスタム Autopilot プロファイルを適用するためには、顧客のデバイス一覧にアクセスできる必要があります。</span><span class="sxs-lookup"><span data-stu-id="0157b-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="0157b-180">OEM 名、シリアル番号、モデルの組み合わせを使う場合は、次の制限事項に注意してください。</span><span class="sxs-lookup"><span data-stu-id="0157b-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="0157b-181">この組み合わせは、新しいデバイス (4 k ハッシュなど) でのみ動作し、128b ハッシュ (RS2 以前のデバイス) に対してはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0157b-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="0157b-182">組み合わせの登録では大文字と小文字が区別されるため、ファイル内のデータが、OEM プロバイダー (ハードウェア プロバイダー) によって提供されるモデルおよび製造元の名前と "***正確に***" 一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0157b-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="0157b-183">パートナー センターで顧客のアカウントにデバイスを追加するには、以下の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="0157b-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="0157b-184">パートナー センターのメニューで **[顧客]** を選択し、デバイスが管理対象となる顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="0157b-185">顧客の詳細ページで、**[デバイス]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="0157b-186">**[デバイスへのプロファイルの適用]** で **[デバイスの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="0157b-187">デバイス一覧の名前を入力し、**[参照]** を選択して、顧客の一覧 (.csv ファイル形式) をパートナー センターにアップロードします。</span><span class="sxs-lookup"><span data-stu-id="0157b-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="0157b-188">この .csv ファイルは、デバイスを購入したときに受け取っているはずです。</span><span class="sxs-lookup"><span data-stu-id="0157b-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="0157b-189">.csv ファイルを受け取っていない場合は、「[Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)」 (Windows Autopilot にデバイスを追加する) の手順に従って自分で作成できます。</span><span class="sxs-lookup"><span data-stu-id="0157b-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="0157b-190">.csv ファイルをアップロードし、**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0157b-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="0157b-191">.csv ファイルをアップロードしようとするとエラー メッセージが表示される場合は、ファイルの形式を確認します。</span><span class="sxs-lookup"><span data-stu-id="0157b-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="0157b-192">ハードウェア ハッシュのみ、OEM 名とシリアル番号とモデル (その列の順序で)、または Windows 製品 ID を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="0157b-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="0157b-193">**[デバイスの追加]** の横にあるリンクで提供されているサンプルの .csv ファイルを使用して、デバイス一覧を作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="0157b-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="0157b-194">.Csv ファイルは次のようになります。</span><span class="sxs-lookup"><span data-stu-id="0157b-194">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="0157b-195">**デバイスのシリアル番号、Windows 製品 ID、ハードウェアハッシュ、製造元名、デバイスモデル**</span><span class="sxs-lookup"><span data-stu-id="0157b-195">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="0157b-196">**{,,,} Microsoft Corporation、Surface ノート Pc**</span><span class="sxs-lookup"><span data-stu-id="0157b-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="0157b-197">"製造元名" と "デバイスモデル" は大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="0157b-197">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="0157b-198">製造元名とデバイスモデルに対してどのような値を設定するかわからない場合は、デバイスでこれを実行して、正しい値を収集できます。</span><span class="sxs-lookup"><span data-stu-id="0157b-198">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="0157b-199">Windows AutoPilot での使用許諾契約の非表示</span><span class="sxs-lookup"><span data-stu-id="0157b-199">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="0157b-200">重要な情報</span><span class="sxs-lookup"><span data-stu-id="0157b-200">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="0157b-201">Windows Autopilot を使用すると、顧客向けに管理しているデバイスで Windows のカスタマイズしたインストールを構成することができます。</span><span class="sxs-lookup"><span data-stu-id="0157b-201">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="0157b-202">顧客が承認した場合は、Windows のセットアップ時に通常はユーザーに対して表示される特定のセットアップ画面を非表示にすることができます。これには、EULA (使用許諾契約) の同意画面が含まれます。</span><span class="sxs-lookup"><span data-stu-id="0157b-202">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="0157b-203">この機能を使用することで、ユーザーに条項を通知して承諾を求める画面を非表示にした場合は、パートナーが条項の非表示について顧客から十分な同意と承認を得たものと見なされ、かつ顧客が組織か個人ユーザーかを問わず、パートナーが顧客の代理として、顧客に適用されるすべての条項の通知に同意し、これを承諾したものと見なされます。</span><span class="sxs-lookup"><span data-stu-id="0157b-203">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="0157b-204">これには、このツールによって画面を非表示にしない場合にユーザーに対して表示される、ライセンス契約条件や通知への同意を含みます。</span><span class="sxs-lookup"><span data-stu-id="0157b-204">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="0157b-205">お客様は、マイクロソフトまたはその認定代理店からソフトウェアのライセンスを正当に取得していない場合、デバイス上でその Windows ソフトウェアを使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="0157b-205">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>