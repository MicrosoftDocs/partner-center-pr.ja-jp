---
title: Windows Autopilot でデバイスのセットアップを効率化する | パートナー センター
description: Windows Autopilot でデバイスのセットアップを効率化するためにパートナー センターの Windows AutoPilot プロファイルを追加する
author: KPacquer
keywords: autopilot、windows autopilot、microsoft autopilot、ゼロタッチ展開、oobe、ログイン画面
ms.localizationpriority: medium
ms.openlocfilehash: 09dc187347c7d433a5edfd1feb616d0b0275acce
ms.sourcegitcommit: 123a7f53d633c27eb5f982926d856de47afb1042
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/09/2018
ms.locfileid: "4489398"
---
# <a name="simplify-device-setup-with-windows-autopilot"></a><span data-ttu-id="47613-104">Windows Autopilot でデバイスのセットアップを効率化する</span><span class="sxs-lookup"><span data-stu-id="47613-104">Simplify device setup with Windows Autopilot</span></span> 

<span data-ttu-id="47613-105">Windows Autopilot によって、新しい Windows 10 Pro デバイスのセットアップを、最初のブートからほんの数ステップで効率的に実行し、セキュリティで保護することができます。</span><span class="sxs-lookup"><span data-stu-id="47613-105">Windows Autopilot streamlines and secures device setup for new Windows 10 Pro devices from first boot in only a few steps.</span></span> <span data-ttu-id="47613-106">詳しくは、[Windows AutoPilot の概要に関するページ](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)ご覧ください。</span><span class="sxs-lookup"><span data-stu-id="47613-106">To learn more, see [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).</span></span>

## <a name="features"></a><span data-ttu-id="47613-107">機能</span><span class="sxs-lookup"><span data-stu-id="47613-107">Features</span></span>

*  <span data-ttu-id="47613-108">デバイスをセットアップするエンド ユーザーの**ローカル管理者のアクセス許可を無効にします**。</span><span class="sxs-lookup"><span data-stu-id="47613-108">**Disable local administrator permissions** for the end users setting up devices</span></span>
*  <span data-ttu-id="47613-109">**組織のログイン ページを表示します**。</span><span class="sxs-lookup"><span data-stu-id="47613-109">**Show an organization's login page**.</span></span> <span data-ttu-id="47613-110">組織では、デバイスを作業デバイスとして追加し、デバイスを Azure Active Directory に追加するログオン ページがあらかじめ定義できます。</span><span class="sxs-lookup"><span data-stu-id="47613-110">The organization can predefine a logon page that adds the device as a work device, and joins the device with Azure Active Directory.</span></span>
*  <span data-ttu-id="47613-111">**デバイスを Mobile Device Manager (MDM) に登録します**。たとえば、OOBE が完了した後の Microsoft Intune。</span><span class="sxs-lookup"><span data-stu-id="47613-111">**Enroll the device into a Mobile Device Manager (MDM)**, for example: Microsoft Intune, after OOBE is complete.</span></span>
*  <span data-ttu-id="47613-112">Windows AutoPilot 展開プロフィルを使用して、必要なステップと意思決定のみが実行されるように **out-of-box experience (OOBE) を効率化します**。</span><span class="sxs-lookup"><span data-stu-id="47613-112">**Streamline the out-of-box experience (OOBE)** to use just the steps and decisions required, using a Windows AutoPilot Deployment profile.</span></span> 

## <a name="requirements"></a><span data-ttu-id="47613-113">要件</span><span class="sxs-lookup"><span data-stu-id="47613-113">Requirements</span></span>

*  <span data-ttu-id="47613-114">Windows 10 Pro Creators Update (バージョン 1703 以降) または Windows 10 Pro for Advanced PC がプリインストールされているデバイス</span><span class="sxs-lookup"><span data-stu-id="47613-114">Devices pre-installed with Windows 10 Pro Creators Update (version 1703 or later) or Windows 10 Pro for Advanced PCs.</span></span>
*  <span data-ttu-id="47613-115">ハードウェア ハッシュと呼ばれるデバイス識別子 (128 HWH または 4 k HWH)。通常、OEM によって提供されます。</span><span class="sxs-lookup"><span data-stu-id="47613-115">Device identifier known as a hardware hash (128 HWH or 4k HWH), which is typically provided by an OEM.</span></span> <span data-ttu-id="47613-116">識別子を使用して、パートナー センターで組織プロファイルを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="47613-116">You'll use identifiers to assign organization profiles in the Partner Center.</span></span> 
*  <span data-ttu-id="47613-117">デバイスは、インターネットにアクセスできる必要があります。</span><span class="sxs-lookup"><span data-stu-id="47613-117">The devices must have access to the internet.</span></span> <span data-ttu-id="47613-118">デバイスが接続できない場合、既定の Windows の out-of-box experience (OOBE) 画面が表示されます。</span><span class="sxs-lookup"><span data-stu-id="47613-118">When the device can’t connect, it shows the default Windows out-of-box experience (OOBE) screens.</span></span>
*  <span data-ttu-id="47613-119">デバイスを MDM に登録するには、Azure Active Directory Premium が必要です。</span><span class="sxs-lookup"><span data-stu-id="47613-119">Enrolling the device into an MDM requires Azure Active Directory Premium.</span></span>

## <a name="add-organization-login-pages-to-oobe"></a><span data-ttu-id="47613-120">組織のログイン ページを OOBE に追加する</span><span class="sxs-lookup"><span data-stu-id="47613-120">Add organization login pages to OOBE</span></span>

<span data-ttu-id="47613-121">組織固有のページを追加するには、組織の [Azure AD ディレクトリ](https://go.microsoft.com/fwlink/?linkid=848958)にデバイスを追加し、ログイン ページを作成します。</span><span class="sxs-lookup"><span data-stu-id="47613-121">To add organization-specific pages, add the devices into your organization’s [Azure AD directory](https://go.microsoft.com/fwlink/?linkid=848958) and create login pages.</span></span>


## <a name="remove-windows-pages-from-oobe-with-a-windows-autopilot-deployment-profile"></a><span data-ttu-id="47613-122">Windows AutoPilot 展開プロファイルを使用して OOBE から Windows のページを削除する</span><span class="sxs-lookup"><span data-stu-id="47613-122">Remove Windows pages from OOBE with a Windows AutoPilot deployment profile</span></span>

**<span data-ttu-id="47613-123">Windows AutoPilot 展開プロファイルの設定の例</span><span class="sxs-lookup"><span data-stu-id="47613-123">Examples of settings in a Windows AutoPilot deployment profile</span></span>**
*  <span data-ttu-id="47613-124">セットアップでプライバシー設定をスキップする</span><span class="sxs-lookup"><span data-stu-id="47613-124">Skip Privacy Settings in setup</span></span>
*  <span data-ttu-id="47613-125">セットアップでローカル管理者アカウントを無効にする</span><span class="sxs-lookup"><span data-stu-id="47613-125">Disable local admin account in setup</span></span>
*  <span data-ttu-id="47613-126">セットアップで自動的にページをスキップする</span><span class="sxs-lookup"><span data-stu-id="47613-126">Automatically skip pages in setup</span></span>
   *  <span data-ttu-id="47613-127">職場または学校用のセットアップを自動的に選択する</span><span class="sxs-lookup"><span data-stu-id="47613-127">Automatically select setup for work or school</span></span>
   *  <span data-ttu-id="47613-128">Cortana、OneDrive、OEM 登録のセットアップのページをスキップする</span><span class="sxs-lookup"><span data-stu-id="47613-128">Skip Cortana, OneDrive, and OEM registration setup pages</span></span>

### <a name="add-devices-and-apply-a-profile"></a><span data-ttu-id="47613-129">デバイスを追加し、プロファイルを適用する</span><span class="sxs-lookup"><span data-stu-id="47613-129">Add devices and apply a profile</span></span>

<span data-ttu-id="47613-130">パートナー センターは、Windows AutoPilot 展開プロファイルを作成し、デバイスの一覧に適用します。</span><span class="sxs-lookup"><span data-stu-id="47613-130">From Partner Center, you can create a Windows AutoPilot deployment profile and apply it to a list of the devices.</span></span>

<span data-ttu-id="47613-131">デバイスを構成するには、デバイスの一覧をアップロードし、デバイスに適用するプロファイルを作成して適用します。</span><span class="sxs-lookup"><span data-stu-id="47613-131">To configure devices, upload a list of the devices, create a profile that applies to the devices, and apply it.</span></span>

1.  <span data-ttu-id="47613-132">デバイスの一覧を追加します。</span><span class="sxs-lookup"><span data-stu-id="47613-132">Add the list of devices.</span></span>

    <span data-ttu-id="47613-133">(販売エージェントと管理エージェントが、パートナー センターにデバイスの一覧を追加するアクセス権を持っています)。</span><span class="sxs-lookup"><span data-stu-id="47613-133">Sales agents and admin agents have access to add the list of devices into Partner Center.</span></span>
    
    <span data-ttu-id="47613-134">間接リセラーは、間接プロバイダーと協力してこれを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="47613-134">Indirect resellers can work with their indirect provider to add this.</span></span>

    <span data-ttu-id="47613-135">a.</span><span class="sxs-lookup"><span data-stu-id="47613-135">a.</span></span>  <span data-ttu-id="47613-136">[Windows AutoPilot の概要に関するページ](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)にあるトピックから、PowerShell スクリプトを使って .csv ファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="47613-136">Create a .csv file using the PowerShell script from the topic: [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).</span></span> <span data-ttu-id="47613-137">この .csv ファイルには、シリアル番号、OEM 名、モデル名、製品 ID、デバイス識別子などのデバイス情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="47613-137">This .csv file contains device info including the serial number, OEM name, model name, product ID and device identifier.</span></span> 

    <span data-ttu-id="47613-138">b. </span><span class="sxs-lookup"><span data-stu-id="47613-138">b.</span></span>  <span data-ttu-id="47613-139">パートナー センターから**お客様**に移動します。 >、デバイスを受け取る顧客を選択 >**デバイス > デバイスの追加**します。</span><span class="sxs-lookup"><span data-stu-id="47613-139">From Partner Center, go to **Customers** > select the customer that’s receiving the devices > **Devices > Add devices**.</span></span>

    <span data-ttu-id="47613-140">c.</span><span class="sxs-lookup"><span data-stu-id="47613-140">c.</span></span>  <span data-ttu-id="47613-141">デバイスのバッチに名前を付けます (例: "Contoso Sales Department PCs – April 2017 order")。</span><span class="sxs-lookup"><span data-stu-id="47613-141">Name the batch of devices, for example, “Contoso Sales Department PCs – April 2017 order.”</span></span> 

    <span data-ttu-id="47613-142">d. </span><span class="sxs-lookup"><span data-stu-id="47613-142">d.</span></span>  <span data-ttu-id="47613-143">**[参照]** をクリックし、デバイス情報ファイルを選択して **[検証]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="47613-143">Click **Browse** > select the device info file > **Validate**.</span></span>

    <span data-ttu-id="47613-144">**注:** .csv ファイルをアップロードしようとした後にエラー メッセージが表示される場合は、ファイルの形式を確認します。</span><span class="sxs-lookup"><span data-stu-id="47613-144">**Note:** If you get an error message after trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="47613-145">8 月以降は、ハードウェア ハッシュのみを使う、OEM 名、シリアル番号、モデルを列の順序で使う、または Windows 製品 ID を使うことができます。</span><span class="sxs-lookup"><span data-stu-id="47613-145">After August, you can use the Hardware Hash only, or the OEM name, serial number, and model in that column order, or the Windows Product ID.</span></span> <span data-ttu-id="47613-146">**[デバイスの追加]** の横のリンクから入手できる .csv ファイルを使うこともできます。</span><span class="sxs-lookup"><span data-stu-id="47613-146">You can also use the sample .csv file provided from the link next to **Add devices**.</span></span>

2.  <span data-ttu-id="47613-147">デバイスに適用できるプロファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="47613-147">Create a profile that you can apply to the devices.</span></span> <span data-ttu-id="47613-148">(管理エージェントのみは、作成し、パートナー センターで、プロファイルを適用するアクセス権を持ちます)。</span><span class="sxs-lookup"><span data-stu-id="47613-148">(Only admin agents have access to create and apply profiles in the Partner Center.)</span></span>

    <span data-ttu-id="47613-149">a. </span><span class="sxs-lookup"><span data-stu-id="47613-149">a.</span></span>  <span data-ttu-id="47613-150">**[デバイス]** で、**[新しいプロファイルの追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="47613-150">From **Devices**, click **Add new profile**.</span></span>

    <span data-ttu-id="47613-151">b. </span><span class="sxs-lookup"><span data-stu-id="47613-151">b.</span></span>  <span data-ttu-id="47613-152">プロファイルに名前を付けます (例: "Contoso Desktop Profile – Skip All OOBE")。</span><span class="sxs-lookup"><span data-stu-id="47613-152">Name the profile, for example, “Contoso Desktop Profile – Skip All OOBE”.</span></span>

    <span data-ttu-id="47613-153">c. </span><span class="sxs-lookup"><span data-stu-id="47613-153">c.</span></span>  <span data-ttu-id="47613-154">OOBE の設定を構成します。</span><span class="sxs-lookup"><span data-stu-id="47613-154">Configure the OOBE settings.</span></span> <span data-ttu-id="47613-155">たとえば、**[セットアップで簡単設定をスキップする]** をオンにします。</span><span class="sxs-lookup"><span data-stu-id="47613-155">For example, check **Skip Express Settings in setup**.</span></span>

    <span data-ttu-id="47613-156">d. </span><span class="sxs-lookup"><span data-stu-id="47613-156">d.</span></span>  <span data-ttu-id="47613-157">**[送信]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="47613-157">Click **Submit**.</span></span>

3.  <span data-ttu-id="47613-158">プロファイルを適用します。</span><span class="sxs-lookup"><span data-stu-id="47613-158">Apply the profile.</span></span>

    <span data-ttu-id="47613-159">a. </span><span class="sxs-lookup"><span data-stu-id="47613-159">a.</span></span>  <span data-ttu-id="47613-160">**[デバイス]** の **[デバイスの割り当てと削除]** ウィンドウで、構成するデバイスを選択します。</span><span class="sxs-lookup"><span data-stu-id="47613-160">From **Devices**, in the **Assign and delete devices** pane, select the devices that you want to configure.</span></span> <span data-ttu-id="47613-161">バッチ全体を選択するには、バッチ名 (例: "Contoso Sales Department PCs – March 2017 order") の横にあるチェック ボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="47613-161">To select an entire batch, click the checkbox next to the batch name (for example, “Contoso Sales Department PCs – March 2017 order”).</span></span>

    <span data-ttu-id="47613-162">b. </span><span class="sxs-lookup"><span data-stu-id="47613-162">b.</span></span>  <span data-ttu-id="47613-163">**[プロファイルの適用]** をクリックし、プロファイル (例: "Contoso Desktop Profile – Skip All OOBE") を選択します。</span><span class="sxs-lookup"><span data-stu-id="47613-163">Click **Apply profile**, and select the profile (for example, “Contoso Desktop Profile – Skip All OOBE”).</span></span> <span data-ttu-id="47613-164">デバイスの [プロファイル] 列にプロファイルが表示されます。</span><span class="sxs-lookup"><span data-stu-id="47613-164">The devices will show the profile in the Profile column.</span></span>

4.  <span data-ttu-id="47613-165">省略可能: テストしてプロファイルが動作することを確認します。</span><span class="sxs-lookup"><span data-stu-id="47613-165">Optional: Test to see that your profile works.</span></span>

    <span data-ttu-id="47613-166">a. </span><span class="sxs-lookup"><span data-stu-id="47613-166">a.</span></span>  <span data-ttu-id="47613-167">デバイスをネットワークに接続し、電源をオンにします。</span><span class="sxs-lookup"><span data-stu-id="47613-167">Connect a device to the network, and turn it on.</span></span>

    <span data-ttu-id="47613-168">b. </span><span class="sxs-lookup"><span data-stu-id="47613-168">b.</span></span>  <span data-ttu-id="47613-169">適切な OOBE 画面 (存在する場合) が表示されることを確認します。</span><span class="sxs-lookup"><span data-stu-id="47613-169">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="47613-170">c. </span><span class="sxs-lookup"><span data-stu-id="47613-170">c.</span></span>  <span data-ttu-id="47613-171">新しいユーザー用のデバイスを準備するには、OOBE エクスペリエンスを完了し、デバイスを工場出荷時の既定の設定にリセットします。</span><span class="sxs-lookup"><span data-stu-id="47613-171">To prepare the device for a new user, complete the OOBE experience, then reset the device to its factory default settings.</span></span>


## <a name="to-update-or-delete-a-profile"></a><span data-ttu-id="47613-172">プロファイルを更新または削除するには</span><span class="sxs-lookup"><span data-stu-id="47613-172">To update or delete a profile</span></span> 

<span data-ttu-id="47613-173">デバイスにプロファイルを割り当てた後、既にデバイスを顧客に付与した場合でも、プロファイルを更新できます。</span><span class="sxs-lookup"><span data-stu-id="47613-173">Once you’ve assigned a profile to a device, you can update it, even if you’ve already given the device to your customer.</span></span> <span data-ttu-id="47613-174">デバイスがインターネットに接続されたときに、OOBE プロセスでプロファイルの最新バージョンがダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="47613-174">When the device connects to the internet, it downloads the latest version of your profile during the OOBE process.</span></span> <span data-ttu-id="47613-175">顧客がデバイスで工場出荷時の既定の設定を復元した場合も、デバイスはプロファイルの最新の更新プログラムをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="47613-175">If your customer restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 

### <a name="you-can-remove-a-profile-from-a-device"></a><span data-ttu-id="47613-176">デバイスからプロファイルを削除することができます。</span><span class="sxs-lookup"><span data-stu-id="47613-176">You can remove a profile from a device</span></span>
1. <span data-ttu-id="47613-177">プロファイルを削除するデバイス (またはデバイスのバッチ) を選択します。</span><span class="sxs-lookup"><span data-stu-id="47613-177">Select the device (or batch of devices) you want to remove the profile from.</span></span> 

2. <span data-ttu-id="47613-178">**[デバイスの割り当てと削除]** ウィンドウで、**[プロファイルの削除]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="47613-178">In **Assign and delete devices** pane, select **Remove profile**.</span></span>

3. <span data-ttu-id="47613-179">削除するプロファイルに移動し、プロファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="47613-179">Go to the profile you want to remove and delete it.</span></span> <span data-ttu-id="47613-180">プロファイルは、すべてのデバイスから削除されます。</span><span class="sxs-lookup"><span data-stu-id="47613-180">The profile will be deleted from all devices.</span></span>

<span data-ttu-id="47613-181">**[デバイス]** で、プロファイルを選択します。</span><span class="sxs-lookup"><span data-stu-id="47613-181">From **Devices**, select the profile.</span></span> <span data-ttu-id="47613-182">ここから、既存の設定を変更することができます。</span><span class="sxs-lookup"><span data-stu-id="47613-182">From here, you can modify the existing settings.</span></span>

## <a name="windows-autopilot-eula-dismissal--important-information"></a><span data-ttu-id="47613-183">Windows AutoPilot での使用許諾契約の非表示 – 重要な情報</span><span class="sxs-lookup"><span data-stu-id="47613-183">Windows Autopilot EULA dismissal – important information</span></span>

<span data-ttu-id="47613-184">このツールを使用すると、お客様向けに管理しているデバイスで Windows の個別のインストールを構成することができます。</span><span class="sxs-lookup"><span data-stu-id="47613-184">Using this tool allows you to configure individual installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="47613-185">お客様の承認があれば、Windows のセットアップ時に通常はユーザーに対して表示される特定のセットアップ画面を非表示にすることができます。こうした画面には、使用許諾契約へ同意する画面も含まれます。</span><span class="sxs-lookup"><span data-stu-id="47613-185">If authorized to do so by the customer, you may choose to suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA acceptance screen.</span></span> 

<span data-ttu-id="47613-186">この機能を使用することで、ユーザーに条項を通知して承諾を求める画面を非表示にした場合は、パートナー様が条項の非表示についてお客様から十分な同意と承認を得たものと見なされ、かつお客様が組織か個人ユーザーかを問わず、パートナー様がお客様の代理として、お客様に適用されるすべての条項の通知に同意し、これを承諾したものと見なされます。</span><span class="sxs-lookup"><span data-stu-id="47613-186">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="47613-187">これには、このツールによって画面を非表示にしない場合にユーザーに対して表示される、ライセンス契約条件や通知への同意を含みます。</span><span class="sxs-lookup"><span data-stu-id="47613-187">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="47613-188">お客様は、マイクロソフトまたはその認定代理店からソフトウェアのライセンスを正当に取得していない場合、デバイス上でその Windows ソフトウェアを使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="47613-188">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>


