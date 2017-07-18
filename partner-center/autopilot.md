---
title: "Windows Autopilot でデバイスのセットアップを効率化する | パートナー センター"
description: "Windows Autopilot でデバイスのセットアップを効率化するためにパートナー センターの Windows AutoPilot プロファイルを追加する"
author: KPacquer
keywords: "autopilot、windows autopilot、microsoft autopilot、ゼロタッチ展開、oobe、ログイン画面"
robots: NOINDEX,NOFOLLOW
ms.openlocfilehash: aa650ee5f2848694fe44d4751d52f8014e0d22a8
ms.sourcegitcommit: e8b504fa98b3ec4c7c8fd954f63ea81299791906
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/01/2017
---
# <a name="simplify-device-setup-with-windows-autopilot"></a><span data-ttu-id="0d8db-104">Windows Autopilot でデバイスのセットアップを効率化する</span><span class="sxs-lookup"><span data-stu-id="0d8db-104">Simplify device setup with Windows Autopilot</span></span> 

<span data-ttu-id="0d8db-105">Windows Autopilot によって、新しい Windows 10 Pro デバイスのセットアップを、最初のブートからほんの数ステップで効率的に実行し、セキュリティで保護することができます。</span><span class="sxs-lookup"><span data-stu-id="0d8db-105">Windows Autopilot streamlines and secures device setup for new Windows 10 Pro devices from first boot in only a few steps.</span></span> <span data-ttu-id="0d8db-106">詳しくは、[Windows AutoPilot の概要に関するページ](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)ご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0d8db-106">To learn more, see [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).</span></span>

## <a name="features"></a><span data-ttu-id="0d8db-107">機能</span><span class="sxs-lookup"><span data-stu-id="0d8db-107">Features</span></span>

*  <span data-ttu-id="0d8db-108">デバイスをセットアップするエンド ユーザーの**ローカル管理者のアクセス許可を無効にします**。</span><span class="sxs-lookup"><span data-stu-id="0d8db-108">**Disable local administrator permissions** for the end users setting up devices</span></span>
*  <span data-ttu-id="0d8db-109">**組織のログイン ページを表示します**。</span><span class="sxs-lookup"><span data-stu-id="0d8db-109">**Show an organization's login page**.</span></span> <span data-ttu-id="0d8db-110">組織では、デバイスを作業デバイスとして追加し、デバイスを Azure Active Directory に追加するログオン ページがあらかじめ定義できます。</span><span class="sxs-lookup"><span data-stu-id="0d8db-110">The organization can predefine a logon page that adds the device as a work device, and joins the device with Azure Active Directory.</span></span>
*  <span data-ttu-id="0d8db-111">**デバイスを Mobile Device Manager (MDM) に登録します**。たとえば、OOBE が完了した後の Microsoft Intune。</span><span class="sxs-lookup"><span data-stu-id="0d8db-111">**Enroll the device into a Mobile Device Manager (MDM)**, for example: Microsoft Intune, after OOBE is complete.</span></span>
*  <span data-ttu-id="0d8db-112">Windows AutoPilot 展開プロフィルを使用して、必要なステップと意思決定のみが実行されるように **out-of-box experience (OOBE) を効率化します**。</span><span class="sxs-lookup"><span data-stu-id="0d8db-112">**Streamline the out-of-box experience (OOBE)** to use just the steps and decisions required, using a Windows AutoPilot Deployment profile.</span></span> 

## <a name="requirements"></a><span data-ttu-id="0d8db-113">要件</span><span class="sxs-lookup"><span data-stu-id="0d8db-113">Requirements</span></span>

*  <span data-ttu-id="0d8db-114">Windows 10 Pro Creators Update (バージョン 1703 以降) と共にプリインストールされているデバイス</span><span class="sxs-lookup"><span data-stu-id="0d8db-114">Devices pre-installed with Windows 10 Pro Creators Update (version 1703 or later)</span></span>
*  <span data-ttu-id="0d8db-115">ハードウェア ハッシュと呼ばれるデバイス識別子 (128 HWH または 4 k HWH)。通常、OEM によって提供されます。</span><span class="sxs-lookup"><span data-stu-id="0d8db-115">Device identifier known as a hardware hash (128 HWH or 4k HWH), which is typically provided by an OEM.</span></span> <span data-ttu-id="0d8db-116">識別子を使用して、パートナー センターで組織プロファイルを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="0d8db-116">You'll use identifiers to assign organization profiles in Partner Center.</span></span> <span data-ttu-id="0d8db-117">2017 年 8 月以降、ハードウェア ハッシュは必要なくなります。</span><span class="sxs-lookup"><span data-stu-id="0d8db-117">After August 2017 you will no longer need the hardware hash.</span></span> 
*  <span data-ttu-id="0d8db-118">デバイスは、インターネットにアクセスできる必要があります。</span><span class="sxs-lookup"><span data-stu-id="0d8db-118">The devices must have access to the internet.</span></span> <span data-ttu-id="0d8db-119">デバイスが接続できない場合、既定の Windows の out-of-box experience (OOBE) 画面が表示されます。</span><span class="sxs-lookup"><span data-stu-id="0d8db-119">When the device can’t connect, it shows the default Windows out-of-box experience (OOBE) screens.</span></span>
*  <span data-ttu-id="0d8db-120">デバイスを MDM に登録するには、Azure Active Directory Premium が必要です。</span><span class="sxs-lookup"><span data-stu-id="0d8db-120">Enrolling the device into an MDM requires Azure Active Directory Premium.</span></span>

## <a name="add-organization-login-pages-to-oobe"></a><span data-ttu-id="0d8db-121">組織のログイン ページを OOBE に追加する</span><span class="sxs-lookup"><span data-stu-id="0d8db-121">Add organization login pages to OOBE</span></span>

<span data-ttu-id="0d8db-122">組織固有のページを追加するには、組織の [Azure AD ディレクトリ](https://go.microsoft.com/fwlink/?linkid=848958)にデバイスを追加し、ログイン ページを作成します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-122">To add organization-specific pages, add the devices into your organization’s [Azure AD directory](https://go.microsoft.com/fwlink/?linkid=848958) and create login pages.</span></span>


## <a name="remove-windows-pages-from-oobe-with-a-windows-autopilot-deployment-profile"></a><span data-ttu-id="0d8db-123">Windows AutoPilot 展開プロファイルを使用して OOBE から Windows のページを削除する</span><span class="sxs-lookup"><span data-stu-id="0d8db-123">Remove Windows pages from OOBE with a Windows AutoPilot deployment profile</span></span>

### <a name="examples-of-settings-in-a-windows-autopilot-deployment-profile"></a><span data-ttu-id="0d8db-124">Windows AutoPilot 展開プロファイルの設定の例</span><span class="sxs-lookup"><span data-stu-id="0d8db-124">Examples of settings in a Windows AutoPilot deployment profile</span></span>
*  <span data-ttu-id="0d8db-125">セットアップでプライバシー設定をスキップする</span><span class="sxs-lookup"><span data-stu-id="0d8db-125">Skip Privacy Settings in setup</span></span>
*  <span data-ttu-id="0d8db-126">セットアップでローカル管理者アカウントを無効にする</span><span class="sxs-lookup"><span data-stu-id="0d8db-126">Disable local admin account in setup</span></span>
*  <span data-ttu-id="0d8db-127">セットアップで自動的にページをスキップする</span><span class="sxs-lookup"><span data-stu-id="0d8db-127">Automatically skip pages in setup</span></span>
   *  <span data-ttu-id="0d8db-128">職場または学校用のセットアップを自動的に選択する</span><span class="sxs-lookup"><span data-stu-id="0d8db-128">Automatically select setup for work or school</span></span>
   *  <span data-ttu-id="0d8db-129">Cortana、OneDrive、OEM 登録のセットアップのページをスキップする</span><span class="sxs-lookup"><span data-stu-id="0d8db-129">Skip Cortana, OneDrive, and OEM registration setup pages</span></span>

### <a name="add-devices-and-apply-a-profile"></a><span data-ttu-id="0d8db-130">デバイスを追加し、プロファイルを適用する</span><span class="sxs-lookup"><span data-stu-id="0d8db-130">Add devices and apply a profile</span></span>

<span data-ttu-id="0d8db-131">パートナー センターで、Windows AutoPilot 展開プロファイルを作成し、デバイスの一覧にプロファイルを適用できます。</span><span class="sxs-lookup"><span data-stu-id="0d8db-131">In Partner Center, you can create a Windows AutoPilot deployment profile and apply it to a list of the devices.</span></span>

<span data-ttu-id="0d8db-132">デバイスを構成するには、パートナー センターにデバイスの一覧をアップロードし、デバイスに適用するプロファイルを作成して適用します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-132">To configure devices, upload a list of the devices into Partner Center, create a profile that applies to the devices, and apply it.</span></span>

1.  <span data-ttu-id="0d8db-133">パートナー センターにデバイスの一覧を追加します </span><span class="sxs-lookup"><span data-stu-id="0d8db-133">Add the list of devices into Partner Center.</span></span> <span data-ttu-id="0d8db-134">(販売エージェントと管理エージェントが、パートナー センターにデバイスの一覧を追加するアクセス権を持っています)。</span><span class="sxs-lookup"><span data-stu-id="0d8db-134">(Sales agents and admin agents have access to add the list of devices into Partner Center.)</span></span>

    <span data-ttu-id="0d8db-135">a.</span><span class="sxs-lookup"><span data-stu-id="0d8db-135">a.</span></span>  <span data-ttu-id="0d8db-136">[Windows AutoPilot の概要に関するページ](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)にあるトピックから、PowerShell スクリプトを使って .csv ファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-136">Create a .csv file using the PowerShell script from the topic: [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).</span></span> <span data-ttu-id="0d8db-137">この .csv ファイルには、シリアル番号、OEM 名、モデル名、製品 ID、デバイス識別子などのデバイス情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0d8db-137">This .csv file contains device info including the serial number, OEM name, model name, product ID and device identifier.</span></span> 

    <span data-ttu-id="0d8db-138">b.</span><span class="sxs-lookup"><span data-stu-id="0d8db-138">b.</span></span>  <span data-ttu-id="0d8db-139">パートナー センターのダッシュボードから、**[顧客]** に移動してデバイスを受け取る顧客を選択し、**[デバイス]、[デバイスの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-139">From the Partner Center dashboard, go to **Customers** > select the customer that’s receiving the devices > **Devices > Add devices**.</span></span>

    <span data-ttu-id="0d8db-140">c. </span><span class="sxs-lookup"><span data-stu-id="0d8db-140">c.</span></span>  <span data-ttu-id="0d8db-141">デバイスのバッチに名前を付けます (例: "Contoso Sales Department PCs – April 2017 order")。</span><span class="sxs-lookup"><span data-stu-id="0d8db-141">Name the batch of devices, for example, “Contoso Sales Department PCs – April 2017 order.”</span></span> 

    <span data-ttu-id="0d8db-142">d. </span><span class="sxs-lookup"><span data-stu-id="0d8db-142">d.</span></span>  <span data-ttu-id="0d8db-143">**[参照]** をクリックし、デバイス情報ファイルを選択して **[検証]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0d8db-143">Click **Browse** > select the device info file > **Validate**.</span></span>

    <span data-ttu-id="0d8db-144">**注:** .csv ファイルをアップロードしようとした後にエラー メッセージが表示される場合は、ファイルの形式を確認します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-144">**Note:** If you get an error message after trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="0d8db-145">8 月以降は、ハードウェア ハッシュのみを使う、OEM 名、シリアル番号、モデルを列の順序で使う、または Windows 製品 ID を使うことができます。</span><span class="sxs-lookup"><span data-stu-id="0d8db-145">After August, you can use the Hardware Hash only, or the OEM name, serial number, and model in that column order, or the Windows Product ID.</span></span> <span data-ttu-id="0d8db-146">**[デバイスの追加]** の横のリンクから入手できる .csv ファイルを使うこともできます。</span><span class="sxs-lookup"><span data-stu-id="0d8db-146">You can also use the sample .csv file provided from the link next to **Add devices**.</span></span>

2.  <span data-ttu-id="0d8db-147">デバイスに適用できるプロファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-147">Create a profile that you can apply to the devices.</span></span> <span data-ttu-id="0d8db-148">(パートナー センターで、プロファイルを作成して適用するアクセス権を持つのは管理エージェントのみです)。</span><span class="sxs-lookup"><span data-stu-id="0d8db-148">(Only admin agents have access to create and apply profiles in Partner Center.)</span></span>

    <span data-ttu-id="0d8db-149">a. </span><span class="sxs-lookup"><span data-stu-id="0d8db-149">a.</span></span>  <span data-ttu-id="0d8db-150">**[デバイス]** で、**[新しいプロファイルの追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0d8db-150">From **Devices**, click **Add new profile**.</span></span>

    <span data-ttu-id="0d8db-151">b. </span><span class="sxs-lookup"><span data-stu-id="0d8db-151">b.</span></span>  <span data-ttu-id="0d8db-152">プロファイルに名前を付けます (例: "Contoso Desktop Profile – Skip All OOBE")。</span><span class="sxs-lookup"><span data-stu-id="0d8db-152">Name the profile, for example, “Contoso Desktop Profile – Skip All OOBE”.</span></span>

    <span data-ttu-id="0d8db-153">c. </span><span class="sxs-lookup"><span data-stu-id="0d8db-153">c.</span></span>  <span data-ttu-id="0d8db-154">OOBE の設定を構成します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-154">Configure the OOBE settings.</span></span> <span data-ttu-id="0d8db-155">たとえば、**[セットアップで簡単設定をスキップする]** をオンにします。</span><span class="sxs-lookup"><span data-stu-id="0d8db-155">For example, check **Skip Express Settings in setup**.</span></span>

    <span data-ttu-id="0d8db-156">d. </span><span class="sxs-lookup"><span data-stu-id="0d8db-156">d.</span></span>  <span data-ttu-id="0d8db-157">**[送信]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0d8db-157">Click **Submit**.</span></span>

3.  <span data-ttu-id="0d8db-158">プロファイルを適用します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-158">Apply the profile.</span></span>

    <span data-ttu-id="0d8db-159">a. </span><span class="sxs-lookup"><span data-stu-id="0d8db-159">a.</span></span>  <span data-ttu-id="0d8db-160">**[デバイス]** の **[デバイスの割り当てと削除]** ウィンドウで、構成するデバイスを選択します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-160">From **Devices**, in the **Assign and delete devices** pane, select the devices that you want to configure.</span></span> <span data-ttu-id="0d8db-161">バッチ全体を選択するには、バッチ名 (例: "Contoso Sales Department PCs – March 2017 order") の横にあるチェック ボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="0d8db-161">To select an entire batch, click the checkbox next to the batch name (for example, “Contoso Sales Department PCs – March 2017 order”).</span></span>

    <span data-ttu-id="0d8db-162">b. </span><span class="sxs-lookup"><span data-stu-id="0d8db-162">b.</span></span>  <span data-ttu-id="0d8db-163">**[プロファイルの適用]** をクリックし、プロファイル (例: "Contoso Desktop Profile – Skip All OOBE") を選択します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-163">Click **Apply profile**, and select the profile (for example, “Contoso Desktop Profile – Skip All OOBE”).</span></span> <span data-ttu-id="0d8db-164">デバイスの [プロファイル] 列にプロファイルが表示されます。</span><span class="sxs-lookup"><span data-stu-id="0d8db-164">The devices will show the profile in the Profile column.</span></span>

4.  <span data-ttu-id="0d8db-165">省略可能: テストしてプロファイルが動作することを確認します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-165">Optional: Test to see that your profile works.</span></span>

    <span data-ttu-id="0d8db-166">a. </span><span class="sxs-lookup"><span data-stu-id="0d8db-166">a.</span></span>  <span data-ttu-id="0d8db-167">デバイスをネットワークに接続し、電源をオンにします。</span><span class="sxs-lookup"><span data-stu-id="0d8db-167">Connect a device to the network, and turn it on.</span></span>

    <span data-ttu-id="0d8db-168">b. </span><span class="sxs-lookup"><span data-stu-id="0d8db-168">b.</span></span>  <span data-ttu-id="0d8db-169">適切な OOBE 画面 (存在する場合) が表示されることを確認します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-169">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="0d8db-170">c. </span><span class="sxs-lookup"><span data-stu-id="0d8db-170">c.</span></span>  <span data-ttu-id="0d8db-171">新しいユーザー用のデバイスを準備するには、OOBE エクスペリエンスを完了し、デバイスを工場出荷時の既定の設定にリセットします。</span><span class="sxs-lookup"><span data-stu-id="0d8db-171">To prepare the device for a new user, complete the OOBE experience, then reset the device to its factory default settings.</span></span>


## <a name="to-update-or-delete-a-profile"></a><span data-ttu-id="0d8db-172">プロファイルを更新または削除するには</span><span class="sxs-lookup"><span data-stu-id="0d8db-172">To update or delete a profile</span></span> 

<span data-ttu-id="0d8db-173">デバイスにプロファイルを割り当てた後、既にデバイスを顧客に付与した場合でも、プロファイルを更新できます。</span><span class="sxs-lookup"><span data-stu-id="0d8db-173">Once you’ve assigned a profile to a device, you can update it, even if you’ve already given the device to your customer.</span></span> <span data-ttu-id="0d8db-174">デバイスがインターネットに接続されたときに、OOBE プロセスでプロファイルの最新バージョンがダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="0d8db-174">When the device connects to the internet, it downloads the latest version of your profile during the OOBE process.</span></span> <span data-ttu-id="0d8db-175">顧客がデバイスで工場出荷時の既定の設定を復元した場合も、デバイスはプロファイルの最新の更新プログラムをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="0d8db-175">If your customer restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 

###<a name="you-can-remove-a-profile-from-a-device"></a><span data-ttu-id="0d8db-176">デバイスからプロファイルを削除することができます。</span><span class="sxs-lookup"><span data-stu-id="0d8db-176">You can remove a profile from a device</span></span>
1. <span data-ttu-id="0d8db-177">プロファイルを削除するデバイス (またはデバイスのバッチ) を選択します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-177">Select the device (or batch of devices) you want to remove the profile from.</span></span> 

2. <span data-ttu-id="0d8db-178">**[デバイスの割り当てと削除]** ウィンドウで、**[プロファイルの削除]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-178">In **Assign and delete devices** pane, select **Remove profile**.</span></span>

3. <span data-ttu-id="0d8db-179">削除するプロファイルに移動し、プロファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-179">Go to the profile you want to remove and delete it.</span></span> <span data-ttu-id="0d8db-180">プロファイルは、すべてのデバイスから削除されます。</span><span class="sxs-lookup"><span data-stu-id="0d8db-180">The profile will be deleted from all devices.</span></span>

<span data-ttu-id="0d8db-181">**[デバイス]** で、プロファイルを選択します。</span><span class="sxs-lookup"><span data-stu-id="0d8db-181">From **Devices**, select the profile.</span></span> <span data-ttu-id="0d8db-182">ここから、既存の設定を変更することができます。</span><span class="sxs-lookup"><span data-stu-id="0d8db-182">From here, you can modify the existing settings.</span></span>
