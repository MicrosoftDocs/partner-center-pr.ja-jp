---
title: Windows Autopilot プロファイルを使用して、デバイスのボックスのエクスペリエンスをカスタマイズ |パートナー センター
description: Autopilot プロファイルを使用して、デバイスのボックスのエクスペリエンスを事前に構成します。
ms.topic: article
ms.date: 2/6/19
author: maggiepuccievans
ms.author: evansma
keywords: autopilot、windows autopilot、microsoft autopilot、ゼロタッチ展開、oobe、ログイン画面、インボックス
ms.localizationpriority: medium
ms.openlocfilehash: 62e83c63bb10c041549f5a09bc32bdae979d462d
ms.sourcegitcommit: 5251779c33378f9ef4735fcb7c91877339462b1e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/07/2019
ms.locfileid: "9062280"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="8ba0b-104">Windows Autopilot プロファイルを使用して、デバイスのボックスのエクスペリエンスをカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

**<span data-ttu-id="8ba0b-105">適用対象</span><span class="sxs-lookup"><span data-stu-id="8ba0b-105">Applies to</span></span>**

- <span data-ttu-id="8ba0b-106">CSP 直接請求パートナー、間接プロバイダー、および間接リセラー</span><span class="sxs-lookup"><span data-stu-id="8ba0b-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="8ba0b-107">ユーザーのデバイスを管理する場合は、顧客のユーザーのインボックス エクスペリエンス (OOBE) をカスタマイズする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="8ba0b-108">デバイスを顧客に提供する前に、Windows Autopilot プロファイルで新しいデバイスを事前構成し、顧客が購入済みのデバイスに新しいプロファイルを適用できます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="8ba0b-109">この記事では、作成し、パートナー センターでのデバイスに Autopilot プロファイルを適用する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="8ba0b-110">慣れていない既に autopilot、これらの記事の情報に確認してください。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="8ba0b-111">Windows Autopilot の概要</span><span class="sxs-lookup"><span data-stu-id="8ba0b-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="8ba0b-112">Autopilot 展開リファレンス ガイド</span><span class="sxs-lookup"><span data-stu-id="8ba0b-112">Autopilot deployment reference guide</span></span>](http://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="8ba0b-113">概要</span><span class="sxs-lookup"><span data-stu-id="8ba0b-113">Overview</span></span>

<span data-ttu-id="8ba0b-114">Windows Autopilot 機能を使用してパートナー センターでは、ユーザーのデバイスに適用するカスタム プロファイルを作成できます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="8ba0b-115">この記事の公開時点では、次のプロファイル設定が提供されていた。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="8ba0b-116">プライバシーの設定をスキップします。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-116">Skip privacy settings.</span></span> <span data-ttu-id="8ba0b-117">このオプションの Autopilot プロファイルの設定を使用することにより、OOBE プロセス中にプライバシーの設定に関する求めません。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="8ba0b-118">デバイスでローカル管理者アカウントの作成を無効にします。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="8ba0b-119">かどうか、デバイスのセットアップ、ユーザーが必要管理者のアクセス権プロセスが完了したら組織を決定できます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="8ba0b-120">職場または学校のデバイスを自動的に設定します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="8ba0b-121">Autopilot による登録されているすべてのデバイスでは、作業が自動的に考慮するまたは学校のデバイスでは、この質問は、OOBE プロセス中には求められませんようにします。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="8ba0b-122">Cortana、OneDrive、OEM 登録のセットアップのページをスキップします。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="8ba0b-123">Autopilot による登録されているすべてのデバイスは、インボックスの experience (OOBE) プロセス中に自動的にこれらのページをスキップします。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="8ba0b-124">エンド ユーザー ライセンス条項 (EULA) をスキップします。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="8ba0b-125">Windows 10 バージョン 1709 以降、組織は、OOBE プロセス中に提示された使用許諾契約のページをスキップを決定できます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="8ba0b-126">[Windows Autopilot の使用許諾契約](#windows-autopilot-eula-dismissal)の下の重要な情報について、Windows セットアップ中に、使用許諾契約のページをスキップすることを検討するを参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="8ba0b-127">次のプロファイルとデバイスの管理アクセス許可と制限事項が適用されます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="8ba0b-128">CSP パートナーは、相手、再販業者関係がある既存の顧客の Autopilot プロファイルの管理、顧客がパートナーの代理管理特権を削除した場合でも引き続きことができます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="8ba0b-129">自分または別の CSP パートナーに追加されている顧客の既存のデバイスを管理できます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-129">You can manage existing devices for your customers that have been added either by you or by another CSP partner.</span></span>

- <span data-ttu-id="8ba0b-130">お客様がビジネス向け Microsoft ストアまたは Microsoft Intune ポータルにアップロードしたデバイスを管理することはできません。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="8ba0b-131">作成し、パートナー センターでの Autopilot プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="8ba0b-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="8ba0b-132">パートナー センターでは、Windows Autopilot 展開プロファイルを作成し、それをデバイスに適用します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="8ba0b-133">管理エージェントのみが作成し、プロファイルを適用できます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="8ba0b-134">新しい Autopilot プロファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="8ba0b-135">パートナー センター メニューから**顧客**を選択しの Autopilot プロファイルを作成している顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="8ba0b-136">顧客の詳細ページでは、**デバイス**を選択します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="8ba0b-137">**Windows Autopilot プロファイル**] の下には、**新しいプロファイルの追加**を選択します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="8ba0b-138">プロファイルの名前と説明を入力し、OOBE の設定を構成します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="8ba0b-139">を選択します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-139">Choose from:</span></span>  

   - <span data-ttu-id="8ba0b-140">セットアップでプライバシー設定をスキップします。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="8ba0b-141">セットアップでローカル管理者アカウントを無効にする</span><span class="sxs-lookup"><span data-stu-id="8ba0b-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="8ba0b-142">セットアップで自動的にページをスキップする</span><span class="sxs-lookup"><span data-stu-id="8ba0b-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="8ba0b-143">(*職場または学校のセットアップを自動的に選択して*、*スキップ Cortana、OneDrive、OEM 登録セットアップ ページ*が含まれています)</span><span class="sxs-lookup"><span data-stu-id="8ba0b-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="8ba0b-144">エンド ユーザー ライセンス条項 (EULA) をスキップします。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="8ba0b-145">[Windows Autopilot の使用許諾契約](#windows-autopilot-eula-dismissal)の下の重要な情報について、Windows セットアップ中に、使用許諾契約のページをスキップすることを検討するを参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="8ba0b-146">完了したら、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="8ba0b-147">ユーザーのデバイスに Autopilot プロファイルを適用します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="8ba0b-148">以下の手順では、パートナー センターにお客様のデバイスを既に追加して、そのデバイスの一覧にアクセスできることを前提としています。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="8ba0b-149">お客様のデバイスを追加していない場合は、[顧客のアカウントに追加のデバイス](#add-devices-to-a-customers-account)の指示に従ってとし、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="8ba0b-150">顧客の Autopilot プロファイルを作成した後は、お客様のデバイスに適用できます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="8ba0b-151">パートナー センター メニューから**顧客**を選択し、[顧客の Autopilot プロファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="8ba0b-152">顧客の詳細ページでは、**デバイス**を選択します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="8ba0b-153">**デバイスにプロファイルを適用**] の下には、デバイスまたはデバイス グループにプロファイルを追加し、**適用プロファイル**を選択するを選択します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="8ba0b-154">**プロファイル**] 列に適用するプロファイルが表示されます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="8ba0b-155">プロファイルをデバイスに正常に適用されることを確認するのには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="8ba0b-156">a. </span><span class="sxs-lookup"><span data-stu-id="8ba0b-156">a.</span></span>  <span data-ttu-id="8ba0b-157">デバイスをネットワークに接続しがオンにします。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="8ba0b-158">b. </span><span class="sxs-lookup"><span data-stu-id="8ba0b-158">b.</span></span>  <span data-ttu-id="8ba0b-159">適切な OOBE 画面 (存在する場合) が表示されることを確認します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="8ba0b-160">c.</span><span class="sxs-lookup"><span data-stu-id="8ba0b-160">c.</span></span>  <span data-ttu-id="8ba0b-161">OOBE プロセスを停止する場合は、新しいユーザーのための準備を工場出荷時のデフォルト設定をデバイスをリセットします。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="8ba0b-162">ユーザーのデバイスから、Autopilot プロファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="8ba0b-163">パートナー センター メニューから**顧客**を選択し、[顧客の Autopilot プロファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="8ba0b-164">顧客の詳細ページでは、**デバイス**を選択します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="8ba0b-165">**デバイスにプロファイルを適用**] の下には、プロファイルを削除し、**プロファイルの削除**を選択するデバイスを選択します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="8ba0b-166">デバイスからプロファイルを削除しても、プロファイルは、一覧から削除されません。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="8ba0b-167">プロファイルを削除する場合は、[更新または削除 Autopilot プロファイル](#update-or-delete-an-autopilot-profile)に指示します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="8ba0b-168">更新または Autopilot プロファイルの削除</span><span class="sxs-lookup"><span data-stu-id="8ba0b-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="8ba0b-169">顧客にデバイスを出荷した後、ボックスのエクスペリエンスを変更する場合、パートナー センターで、プロファイルを変更できます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="8ba0b-170">ユーザーのデバイスは、インターネットに接続するとき、OOBE プロセス中にプロファイルの最新バージョンがダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="8ba0b-171">また、いつでも、顧客が、デバイスを工場出荷時の既定の設定を復元、デバイスはもう一度ダウンロード プロファイルの最新バージョン、OOBE プロセス中にします。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="8ba0b-172">パートナー センター メニューから**顧客**を選択し、Autopilot プロファイルを変更することを希望する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="8ba0b-173">顧客の詳細ページでは、**デバイス**を選択します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="8ba0b-174">[ **Windows Autopilot プロファイル**を更新する必要があるプロファイルを選択します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="8ba0b-175">必要な変更を行い、**提出**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="8ba0b-176">このプロファイルを削除するには、ページの右上隅から**プロファイルを削除**を選択します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="8ba0b-177">デバイスが顧客アカウントに追加します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="8ba0b-178">販売エージェントと管理エージェントは、顧客のアカウントに、デバイスを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="8ba0b-179">カスタムの Autopilot プロファイルを適用すると、ユーザーのデバイスを前に、お客様のデバイスの一覧にアクセスできる必要があります。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="8ba0b-180">OEM 名、シリアル番号、およびモデルの組み合わせを使用する場合は、これらの制限を認識します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="8ba0b-181">この組は、新しいデバイス (4 k ハッシュ、たとえば) に対してのみ 128b ハッシュ (RS2 と以前のデバイス) はサポートされません。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="8ba0b-182">組登録は大文字と小文字ため、OEM プロバイダー (ハードウェア プロバイダー) によって提供されるため、ファイル内のデータが、モデルと製造元の名前***正確に***一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="8ba0b-183">パートナー センターで顧客のアカウントにデバイスを追加するには、以下の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="8ba0b-184">パートナー センター メニューから**顧客**を選択し、[顧客がデバイスを管理します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="8ba0b-185">顧客の詳細ページでは、**デバイス**を選択します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="8ba0b-186">**デバイスにプロファイルを適用**] の下には、**追加のデバイス**を選択します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="8ba0b-187">デバイスの一覧の名前を入力し、[パートナー センターに .csv ファイル形式で、顧客の一覧をアップロードする**参照**をします。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="8ba0b-188">デバイス購入のこの .csv ファイルを受信したする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="8ba0b-189">.Csv ファイルを受信していない場合は、 [Windows Autopilot に追加のデバイス](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)での手順に従って自分で 1 つを作成できます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="8ba0b-190">.Csv ファイルをアップロードし、[**保存**します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="8ba0b-191">.Csv ファイルをアップロードしているときにエラー メッセージを取得する場合は、ファイルの形式を確認します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="8ba0b-192">ハードウェア ハッシュのみ、または OEM 名、シリアル番号、およびモデル (その列の順番に)、または Windows 製品 ID を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="8ba0b-193">デバイスの一覧を作成するのに**追加のデバイス**の横にあるリンクから提供された .csv ファイルを使用することもことができます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="8ba0b-194">Windows Autopilot の使用許諾契約</span><span class="sxs-lookup"><span data-stu-id="8ba0b-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="8ba0b-195">重要な情報</span><span class="sxs-lookup"><span data-stu-id="8ba0b-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="8ba0b-196">Windows Autopilot では、顧客を管理するデバイスで Windows のカスタマイズされたインストールを構成することができます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="8ba0b-197">顧客が、これを行うに承認されている場合は、抑制または (使用許諾契約書) 使用許諾契約書の承認画面を含む、Windows セットアップ時に通常、ユーザーに表示される特定のセットアップ画面を非表示にできます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="8ba0b-198">この関数を使用して、同意したものを抑制する通知またはから顧客の代理で用語、およびそのことを非表示にするための十分な同意と承認を取得した条項ことを意味の受け入れをユーザーに提供するように設計されている画面を非表示(かどうか、組織や、ケースと個々 のユーザーがあります)、顧客は、通知に同意し、いずれかに同意語句は、お客様に該当します。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="8ba0b-199">これには、このツールによって画面を非表示にしない場合にユーザーに対して表示される、ライセンス契約条件や通知への同意を含みます。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="8ba0b-200">お客様は、マイクロソフトまたはその認定代理店からソフトウェアのライセンスを正当に取得していない場合、デバイス上でその Windows ソフトウェアを使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="8ba0b-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>