---
title: Windows Autopilot プロファイルを使用したデバイスの既定のエクスペリエンスのカスタマイズ |パートナー センター
description: Autopilot プロファイルを使用したデバイスの既定のエクスペリエンスを事前に構成します。
ms.topic: article
ms.date: 02/06/19
author: maggiepuccievans
ms.author: evansma
keywords: autopilot、windows autopilot、microsoft の autopilot、ゼロ タッチ展開、oobe、ログイン画面、既製
ms.localizationpriority: medium
ms.openlocfilehash: 00c4bc3717b5f40984f60dd2c04ee7fec10b80da
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586915"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="599e7-104">Windows Autopilot プロファイルを使用したデバイスの既定のエクスペリエンスをカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="599e7-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

<span data-ttu-id="599e7-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="599e7-105">**Applies to**</span></span>

- <span data-ttu-id="599e7-106">CSP の請求書の直接パートナー、間接プロバイダー、および間接リセラー</span><span class="sxs-lookup"><span data-stu-id="599e7-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="599e7-107">お客様のデバイスを管理している場合は、顧客のユーザーの既定の experience (OOBE) をカスタマイズする必要があります。</span><span class="sxs-lookup"><span data-stu-id="599e7-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="599e7-108">デバイスを顧客に納入する前に Windows Autopilot プロファイルによって、新しいデバイスを事前に構成し、顧客が既に購入したデバイスに新しいプロファイルを適用できます。</span><span class="sxs-lookup"><span data-stu-id="599e7-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="599e7-109">この記事では、作成し、Autopilot プロファイルをパートナー センターでデバイスに適用する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="599e7-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="599e7-110">慣れていない既に Autopilot 場合のこれらの記事の情報を確認します。</span><span class="sxs-lookup"><span data-stu-id="599e7-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="599e7-111">Windows Autopilot の概要</span><span class="sxs-lookup"><span data-stu-id="599e7-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="599e7-112">Autopilot 展開リファレンス ガイド</span><span class="sxs-lookup"><span data-stu-id="599e7-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="599e7-113">概要</span><span class="sxs-lookup"><span data-stu-id="599e7-113">Overview</span></span>

<span data-ttu-id="599e7-114">パートナー センターで Windows Autopilot の機能、顧客のデバイスに適用するカスタム プロファイルを作成できます。</span><span class="sxs-lookup"><span data-stu-id="599e7-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="599e7-115">次のプロファイル設定は、この記事の公開時に使用可能なです。</span><span class="sxs-lookup"><span data-stu-id="599e7-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="599e7-116">プライバシーの設定をスキップします。</span><span class="sxs-lookup"><span data-stu-id="599e7-116">Skip privacy settings.</span></span> <span data-ttu-id="599e7-117">省略可能なこの Autopilot プロファイルの設定を使用することにより、OOBE プロセス中に、プライバシーの設定について確認されません。</span><span class="sxs-lookup"><span data-stu-id="599e7-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="599e7-118">デバイスのローカル管理者アカウントの作成を無効にします。</span><span class="sxs-lookup"><span data-stu-id="599e7-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="599e7-119">組織では、かどうか、プロセスが完了したら、デバイスを設定するユーザーが管理者アクセスする必要がありますを決定できます。</span><span class="sxs-lookup"><span data-stu-id="599e7-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="599e7-120">職場または学校のデバイスを自動的に設定します。</span><span class="sxs-lookup"><span data-stu-id="599e7-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="599e7-121">Autopilot に登録されたすべてのデバイスでは、作業が自動的に考慮するまたは学校のデバイスのため、この質問は、OOBE プロセス中には求められません。</span><span class="sxs-lookup"><span data-stu-id="599e7-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="599e7-122">Cortana、OneDrive、および OEM の登録セットアップ ページをスキップします。</span><span class="sxs-lookup"><span data-stu-id="599e7-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="599e7-123">Autopilot に登録されたすべてのデバイスは、既製の experience (OOBE) プロセス中に自動的にこれらのページをスキップします。</span><span class="sxs-lookup"><span data-stu-id="599e7-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="599e7-124">エンド ユーザー ライセンス契約 (EULA) をスキップします。</span><span class="sxs-lookup"><span data-stu-id="599e7-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="599e7-125">組織は Windows 10 バージョン 1709 以降、OOBE プロセス中に表示される使用許諾契約書 ページをスキップする決定できます。</span><span class="sxs-lookup"><span data-stu-id="599e7-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="599e7-126">参照してください[Windows Autopilot の使用許諾契約書ジョンソン](#windows-autopilot-eula-dismissal)以下の Windows の中に、EULA ページをスキップしています。 詳細については考慮すべき重要な情報をセットアップします。</span><span class="sxs-lookup"><span data-stu-id="599e7-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="599e7-127">次のプロファイルとデバイスの管理アクセス許可と制限事項が適用されます。</span><span class="sxs-lookup"><span data-stu-id="599e7-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="599e7-128">CSP パートナーは顧客には、パートナーの管理の委任特権が削除された場合でも、再販業者関係のある相手の既存のお客様の Autopilot プロファイルを管理する続行できます。</span><span class="sxs-lookup"><span data-stu-id="599e7-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="599e7-129">自分または別の CSP パートナーに追加されているお客様の既存のデバイスを管理できます。</span><span class="sxs-lookup"><span data-stu-id="599e7-129">You can manage existing devices for your customers that have been added either by you or by another CSP partner.</span></span>

- <span data-ttu-id="599e7-130">お客様が Microsoft Store for Business または Microsoft Intune ポータルにアップロードするデバイスを管理することはできません。</span><span class="sxs-lookup"><span data-stu-id="599e7-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="599e7-131">作成し、パートナー センターでの Autopilot プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="599e7-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="599e7-132">パートナー センターでは、Windows Autopilot deployment プロファイルを作成し、デバイスにも適用されます。</span><span class="sxs-lookup"><span data-stu-id="599e7-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="599e7-133">管理エージェントのみを作成し、プロファイルを適用できます。</span><span class="sxs-lookup"><span data-stu-id="599e7-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="599e7-134">新しい Autopilot プロファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="599e7-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="599e7-135">選択**顧客**を選択し、パートナー センターのメニューから、顧客作成するの Autopilot プロファイル。</span><span class="sxs-lookup"><span data-stu-id="599e7-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="599e7-136">顧客の詳細 ページで、次のように選択します。**デバイス**します。</span><span class="sxs-lookup"><span data-stu-id="599e7-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="599e7-137">**Windows Autopilot プロファイル**選択**新しいプロファイルを追加する**します。</span><span class="sxs-lookup"><span data-stu-id="599e7-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="599e7-138">プロファイルの名前と説明を入力し、OOBE 設定を構成します。</span><span class="sxs-lookup"><span data-stu-id="599e7-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="599e7-139">以下から選択します。</span><span class="sxs-lookup"><span data-stu-id="599e7-139">Choose from:</span></span>  

   - <span data-ttu-id="599e7-140">セットアップでのプライバシー設定をスキップします。</span><span class="sxs-lookup"><span data-stu-id="599e7-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="599e7-141">セットアップでローカル管理者アカウントを無効にする</span><span class="sxs-lookup"><span data-stu-id="599e7-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="599e7-142">セットアップで自動的にページをスキップする</span><span class="sxs-lookup"><span data-stu-id="599e7-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="599e7-143">(が含まれています*職場または学校のセットアップが自動的に選択*と*Skip Cortana、OneDrive、および OEM の登録セットアップ ページ*)</span><span class="sxs-lookup"><span data-stu-id="599e7-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="599e7-144">エンド ユーザー ライセンス契約 (EULA) をスキップします。</span><span class="sxs-lookup"><span data-stu-id="599e7-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="599e7-145">参照してください[Windows Autopilot の使用許諾契約書ジョンソン](#windows-autopilot-eula-dismissal)以下の Windows の中に、EULA ページをスキップしています。 詳細については考慮すべき重要な情報をセットアップします。</span><span class="sxs-lookup"><span data-stu-id="599e7-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="599e7-146">完了したら、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="599e7-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="599e7-147">お客様のデバイスに、Autopilot プロファイルを適用します。</span><span class="sxs-lookup"><span data-stu-id="599e7-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="599e7-148">以下の手順では、パートナー センターに、お客様のデバイスを既に追加したことと、デバイスの一覧にアクセスできることを仮定します。</span><span class="sxs-lookup"><span data-stu-id="599e7-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="599e7-149">お客様のデバイスに追加済みしていない場合の指示に従って[、お客様のアカウントにデバイスを追加](#add-devices-to-a-customers-account)し、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="599e7-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="599e7-150">Autopilot プロファイルを顧客を作成した後は、お客様のデバイスに適用できます。</span><span class="sxs-lookup"><span data-stu-id="599e7-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="599e7-151">選択**顧客**を選択し、パートナー センターのメニューから、顧客プロファイルを作成した、Autopilot にします。</span><span class="sxs-lookup"><span data-stu-id="599e7-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="599e7-152">顧客の詳細 ページで、次のように選択します。**デバイス**します。</span><span class="sxs-lookup"><span data-stu-id="599e7-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="599e7-153">**プロファイルをデバイスに適用**デバイスまたはデバイス グループのプロファイルを追加し、選択する選択**プロファイルを適用**します。</span><span class="sxs-lookup"><span data-stu-id="599e7-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="599e7-154">適用したプロファイルが表示されます、**プロファイル**列。</span><span class="sxs-lookup"><span data-stu-id="599e7-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="599e7-155">プロファイルをデバイスに正常に適用されることを確認するのには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="599e7-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="599e7-156">a. </span><span class="sxs-lookup"><span data-stu-id="599e7-156">a.</span></span>  <span data-ttu-id="599e7-157">デバイスをネットワークに接続して、オンにします。</span><span class="sxs-lookup"><span data-stu-id="599e7-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="599e7-158">b. </span><span class="sxs-lookup"><span data-stu-id="599e7-158">b.</span></span>  <span data-ttu-id="599e7-159">適切な OOBE 画面 (存在する場合) が表示されることを確認します。</span><span class="sxs-lookup"><span data-stu-id="599e7-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="599e7-160">c.</span><span class="sxs-lookup"><span data-stu-id="599e7-160">c.</span></span>  <span data-ttu-id="599e7-161">OOBE プロセスが停止したら、新しいユーザーのための準備を出荷時の既定設定にデバイスをリセットします。</span><span class="sxs-lookup"><span data-stu-id="599e7-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="599e7-162">顧客のデバイスから Autopilot プロファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="599e7-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="599e7-163">選択**顧客**を選択し、パートナー センターのメニューから、顧客プロファイルを作成した、Autopilot にします。</span><span class="sxs-lookup"><span data-stu-id="599e7-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="599e7-164">顧客の詳細 ページで、次のように選択します。**デバイス**します。</span><span class="sxs-lookup"><span data-stu-id="599e7-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="599e7-165">**プロファイルをデバイスに適用**からプロファイルを削除しを選択するデバイスを選択します。**プロファイルを削除する**します。</span><span class="sxs-lookup"><span data-stu-id="599e7-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="599e7-166">デバイスからプロファイルを削除しても、一覧から、プロファイルは削除されません。</span><span class="sxs-lookup"><span data-stu-id="599e7-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="599e7-167">プロファイルを削除する場合は、次の手順に[Update または delete Autopilot プロファイルを](#update-or-delete-an-autopilot-profile)します。</span><span class="sxs-lookup"><span data-stu-id="599e7-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="599e7-168">更新または削除、Autopilot プロファイル</span><span class="sxs-lookup"><span data-stu-id="599e7-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="599e7-169">顧客にデバイスを出荷した後は、既製のエクスペリエンスを変更する場合は、パートナー センターでプロファイルを変更できます。</span><span class="sxs-lookup"><span data-stu-id="599e7-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="599e7-170">顧客のデバイスは、インターネットに接続するとき、OOBE プロセス中に、最新のプロファイル バージョンがダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="599e7-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="599e7-171">また、顧客は、デバイスを工場出荷時の既定の設定に戻し、いつでも、デバイスはもう一度最新バージョンをダウンロード プロファイル OOBE プロセス中に。</span><span class="sxs-lookup"><span data-stu-id="599e7-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="599e7-172">選択**顧客**から、パートナー センターのメニューとし、Autopilot プロファイルを変更する必要がある顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="599e7-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="599e7-173">顧客の詳細 ページで、次のように選択します。**デバイス**します。</span><span class="sxs-lookup"><span data-stu-id="599e7-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="599e7-174">**Windows Autopilot プロファイル**を更新する必要があるプロファイルを選択します。</span><span class="sxs-lookup"><span data-stu-id="599e7-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="599e7-175">内容を変更し、**送信**します。</span><span class="sxs-lookup"><span data-stu-id="599e7-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="599e7-176">このプロファイルを削除するには、次のように選択します。**プロファイルを削除する**ページの右上隅にあるからです。</span><span class="sxs-lookup"><span data-stu-id="599e7-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="599e7-177">お客様のアカウントにデバイスを追加します。</span><span class="sxs-lookup"><span data-stu-id="599e7-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="599e7-178">販売エージェントと管理エージェントは、お客様のアカウントにデバイスを追加できます。</span><span class="sxs-lookup"><span data-stu-id="599e7-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="599e7-179">カスタムの Autopilot プロファイルをお客様のデバイスに適用する前に、お客様のデバイスの一覧にアクセスできる必要があります。</span><span class="sxs-lookup"><span data-stu-id="599e7-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="599e7-180">OEM 名、シリアル番号、およびモデルの組み合わせを使用する場合は、これらの制限の注意。</span><span class="sxs-lookup"><span data-stu-id="599e7-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="599e7-181">この組は、以降のデバイス (4 k ハッシュなど) に対してのみ 128b ハッシュ (RS2 と以前のデバイス) はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="599e7-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="599e7-182">ファイル内のデータは、モデルと製造元の名前と一致する必要がありますので、タプルの登録は大文字小文字が区別***まったく***OEM プロバイダー (ハードウェア プロバイダー) によって提供されます。</span><span class="sxs-lookup"><span data-stu-id="599e7-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="599e7-183">パートナー センターでお客様のアカウントにデバイスを追加するには、以下の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="599e7-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="599e7-184">選択**顧客**パートナー センターのメニュー デバイスを管理する顧客を選択からします。</span><span class="sxs-lookup"><span data-stu-id="599e7-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="599e7-185">顧客の詳細 ページで、次のように選択します。**デバイス**します。</span><span class="sxs-lookup"><span data-stu-id="599e7-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="599e7-186">**プロファイルをデバイスに適用**選択**デバイスの追加**します。</span><span class="sxs-lookup"><span data-stu-id="599e7-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="599e7-187">デバイスの一覧の名前を入力し、**参照**(.csv ファイル形式) で、顧客の一覧をパートナー センターにアップロードします。</span><span class="sxs-lookup"><span data-stu-id="599e7-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="599e7-188">デバイス購入時にこの .csv ファイルを受信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="599e7-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="599e7-189">.Csv ファイルを受信していない場合は、次の手順で作成する自分でできます[に Windows Autopilot デバイスを追加](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)します。</span><span class="sxs-lookup"><span data-stu-id="599e7-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="599e7-190">.Csv ファイルをアップロードし、**保存**します。</span><span class="sxs-lookup"><span data-stu-id="599e7-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="599e7-191">.Csv ファイルをアップロードするときにエラー メッセージを取得する場合は、ファイルの形式を確認します。</span><span class="sxs-lookup"><span data-stu-id="599e7-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="599e7-192">ハードウェア ハッシュのみ、または OEM 名、シリアル番号、および (その列の順序で)、モデルまたは Windows プロダクト ID を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="599e7-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="599e7-193">次に、リンクから提供されたサンプルの .csv ファイルを使用することもできます。**デバイスの追加**デバイス一覧を作成します。</span><span class="sxs-lookup"><span data-stu-id="599e7-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="599e7-194">Windows Autopilot の使用許諾契約書ジョンソン</span><span class="sxs-lookup"><span data-stu-id="599e7-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="599e7-195">重要な情報</span><span class="sxs-lookup"><span data-stu-id="599e7-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="599e7-196">Windows Autopilot の顧客を管理するデバイスで Windows のインストールをカスタマイズを構成することができます。</span><span class="sxs-lookup"><span data-stu-id="599e7-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="599e7-197">そのためには、顧客が承認されると場合、抑制または (エンド ユーザー ライセンス契約) 使用許諾契約書への同意の画面を含む、Windows をセットアップするときに、ユーザーに提示される通常設定の特定の画面を非表示にできます。</span><span class="sxs-lookup"><span data-stu-id="599e7-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="599e7-198">非表示にするか、ユーザーから、お客様の代わりに、用語、およびそのするを非表示にするための十分な同意と承認を取得した用語の意味の承認または通知を提供するように設計された任意の画面を非表示をこの関数を使用すると、同意します。(かどうか、組織または個々 のユーザーとして場合もあります)、お客様は、通知に同意して、いずれかをそのまま使用条項をお客様に適用されます。</span><span class="sxs-lookup"><span data-stu-id="599e7-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="599e7-199">これには、このツールによって画面を非表示にしない場合にユーザーに対して表示される、ライセンス契約条件や通知への同意を含みます。</span><span class="sxs-lookup"><span data-stu-id="599e7-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="599e7-200">お客様は、マイクロソフトまたはその認定代理店からソフトウェアのライセンスを正当に取得していない場合、デバイス上でその Windows ソフトウェアを使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="599e7-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>