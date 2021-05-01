---
title: Marketplace プランでのライセンスの管理
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ISV コマーシャルマーケットプレースプランのライセンスを設定および管理する方法について説明します。
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f049ffda4c3d9476c09257fc814e5acac393cb54
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328017"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="175c9-103">Marketplace プランでのライセンスの管理</span><span class="sxs-lookup"><span data-stu-id="175c9-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="175c9-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="175c9-104">**Appropriate roles**</span></span>

- <span data-ttu-id="175c9-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="175c9-105">Global admin</span></span>
- <span data-ttu-id="175c9-106">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="175c9-106">Account admin</span></span>

<span data-ttu-id="175c9-107">この記事では、パートナーセンターでオファーを設定し、Microsoft AppSource で使用できるようにし、そのプランのライセンスを管理するプロセスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="175c9-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="175c9-108">この記事の機能は、現在パブリックプレビュー段階です。</span><span class="sxs-lookup"><span data-stu-id="175c9-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="175c9-109">開始する前に</span><span class="sxs-lookup"><span data-stu-id="175c9-109">Before you begin</span></span>

### <a name="commercial-marketplace-basics"></a><span data-ttu-id="175c9-110">商用マーケットプレースの基本</span><span class="sxs-lookup"><span data-stu-id="175c9-110">Commercial marketplace basics</span></span>

<span data-ttu-id="175c9-111">このプロセスを開始する前に、コマーシャルマーケットプレースの基本を理解しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="175c9-111">Before you begin this process, you should familiarize yourself with the basics of the commercial marketplace.</span></span> <span data-ttu-id="175c9-112">次の表の記事は、作業を開始するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="175c9-112">The articles in the table below will help get you started.</span></span> 

| <span data-ttu-id="175c9-113">トピック</span><span class="sxs-lookup"><span data-stu-id="175c9-113">Topic</span></span>  | <span data-ttu-id="175c9-114">[アーティクル]</span><span class="sxs-lookup"><span data-stu-id="175c9-114">Article</span></span>  |
|-------|--------|
|<span data-ttu-id="175c9-115">商用 marketplace プラン</span><span class="sxs-lookup"><span data-stu-id="175c9-115">Commercial marketplace plans</span></span> | [<span data-ttu-id="175c9-116">コマーシャル マーケットプレース オファーのプランと価格</span><span class="sxs-lookup"><span data-stu-id="175c9-116">Plans and pricing for commercial marketplace offers</span></span>](/azure/marketplace/plans-pricing)    |
|<span data-ttu-id="175c9-117">商用 marketplace プラン</span><span class="sxs-lookup"><span data-stu-id="175c9-117">Commercial marketplace offers</span></span>  | [<span data-ttu-id="175c9-118">リストの種類</span><span class="sxs-lookup"><span data-stu-id="175c9-118">Listing types</span></span>](/azure/marketplace/determine-your-listing-type)    |
|<span data-ttu-id="175c9-119">商用 marketplace アカウント</span><span class="sxs-lookup"><span data-stu-id="175c9-119">Commercial marketplace accounts</span></span> |  [<span data-ttu-id="175c9-120">パートナー センターでコマーシャル マーケットプレース アカウントを作成する</span><span class="sxs-lookup"><span data-stu-id="175c9-120">Create a commercial marketplace account in Partner Center</span></span>](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a><span data-ttu-id="175c9-121">プラン ID を確認する</span><span class="sxs-lookup"><span data-stu-id="175c9-121">Determine your Offer ID</span></span>

<span data-ttu-id="175c9-122">以下の手順では、プラン ID を入力するように求められます。</span><span class="sxs-lookup"><span data-stu-id="175c9-122">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="175c9-123">次の点に注意して、適切なプラン ID を取得してください。</span><span class="sxs-lookup"><span data-stu-id="175c9-123">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="175c9-124">この ID は、マーケットプレース オファーの Web アドレスと Azure Resource Manager テンプレート (該当する場合) で顧客に表示されます。</span><span class="sxs-lookup"><span data-stu-id="175c9-124">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="175c9-125">オファー ID の長さはパブリッシャー ID の組み合わせで 40 文字以下にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="175c9-125">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="175c9-126">使用できるのは小文字と数字だけです。</span><span class="sxs-lookup"><span data-stu-id="175c9-126">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="175c9-127">プラン ID には、ハイフンとアンダースコアを含めることができますが、スペースは使用できません。</span><span class="sxs-lookup"><span data-stu-id="175c9-127">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="175c9-128">たとえば、発行元 ID がで、「」と入力した場合、 `testpublisherid` `test-offer-1` オファー web アドレスはになり `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` ます。</span><span class="sxs-lookup"><span data-stu-id="175c9-128">For example, if your Publisher ID is `testpublisherid` and you enter `test-offer-1`, the offer web address will be `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1`.</span></span>
- <span data-ttu-id="175c9-129">**[作成]** を選択した後にこの ID を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="175c9-129">This ID can't be changed after you select **Create**.</span></span>

### <a name="determine-your-offer-alias"></a><span data-ttu-id="175c9-130">プランのエイリアスを確認する</span><span class="sxs-lookup"><span data-stu-id="175c9-130">Determine your Offer alias</span></span>

<span data-ttu-id="175c9-131">プランのエイリアスは、パートナーセンターでオファーに使用される名前です。</span><span class="sxs-lookup"><span data-stu-id="175c9-131">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="175c9-132">次のガイドラインに従う適切なプランのエイリアスも必要になります。</span><span class="sxs-lookup"><span data-stu-id="175c9-132">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="175c9-133">この名前はマーケットプレースでは使用されず、顧客に表示されるオファー名やその他の値とは異なります。</span><span class="sxs-lookup"><span data-stu-id="175c9-133">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="175c9-134">[作成] を選択した後にこの名前を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="175c9-134">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="175c9-135">プランを作成する</span><span class="sxs-lookup"><span data-stu-id="175c9-135">Create your offer</span></span>

<span data-ttu-id="175c9-136">ライセンスプロセスの最初の手順は、市販の marketplace プランを作成することです。</span><span class="sxs-lookup"><span data-stu-id="175c9-136">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="175c9-137">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="175c9-137">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="175c9-138">左側のナビゲーションメニューで、[ **商用 Marketplace/概要**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-138">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="175c9-139">[概要] ページの上部にある [ **新しいプラン**] を選択し、[ **顧客エンゲージメント用の Dynamics 365 & PowerApps**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-139">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="175c9-140">前の手順で作成した **プラン ID** と **プランのエイリアス** を入力します。</span><span class="sxs-lookup"><span data-stu-id="175c9-140">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="175c9-141">**[作成]** を選択してオファーを生成し、続行します。</span><span class="sxs-lookup"><span data-stu-id="175c9-141">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="175c9-142">ライセンスオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-142">Choose your licensing options.</span></span>

    - <span data-ttu-id="175c9-143">プランのライセンス管理を有効にするには、[ **Microsoft によるアプリライセンス管理を有効** にする] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-143">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="175c9-144">これは1回限りの設定であり、プランを発行した後に変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="175c9-144">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="175c9-145">また、顧客がライセンスを使用せずにアプリの基本機能を実行し、ライセンスを購入した後に premium 機能を実行できるようにすることもできます。</span><span class="sxs-lookup"><span data-stu-id="175c9-145">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="175c9-146">これを行うには、[ **ライセンスが割り当てられていない場合でも、顧客がアプリをインストールできるように** する] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-146">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="175c9-147">プランのライセンス管理を有効にしない場合は、[ **今すぐ入手する (無料)**]、[ **無料試用版**]、または [ **連絡してください**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-147">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="175c9-148">プランを作成する</span><span class="sxs-lookup"><span data-stu-id="175c9-148">Create your plan</span></span>

<span data-ttu-id="175c9-149">この手順では、プランに対して有効にするプランを定義します。</span><span class="sxs-lookup"><span data-stu-id="175c9-149">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="175c9-150">左側のナビゲーションメニューで、[ **プランの概要**] を選択し、[ **新しいプランの作成**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-150">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="175c9-151">**プラン ID** と **プラン名** を入力し、[**作成**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-151">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="175c9-152">[ **プランの一覧** ] ページで、 **プランの説明** を入力します。</span><span class="sxs-lookup"><span data-stu-id="175c9-152">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="175c9-153">説明を保存して後で終了するには、[ **下書きの保存**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-153">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="175c9-154">操作が完了したら、[ **レビューと発行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-154">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="175c9-155">プランの情報が、[プランの一覧 (プラン] セクション) の appsource.microsoft.com に表示されるようになります。</span><span class="sxs-lookup"><span data-stu-id="175c9-155">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="175c9-156">このプランのプランをすべて作成したら、各プランのサービス ID をコピーする必要があります。</span><span class="sxs-lookup"><span data-stu-id="175c9-156">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="175c9-157">プランの一覧ページの上部にある [ **プランの概要** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-157">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="175c9-158">各プランのサービス ID を安全な場所にコピーします。</span><span class="sxs-lookup"><span data-stu-id="175c9-158">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="175c9-159">ソリューションへのサービス Id の追加</span><span class="sxs-lookup"><span data-stu-id="175c9-159">Add Service IDs to your solution</span></span>

<span data-ttu-id="175c9-160">次の手順では、先ほどコピーした各プランのサービス Id を追加して、ソリューションを更新します。</span><span class="sxs-lookup"><span data-stu-id="175c9-160">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="175c9-161">この詳細については、「 [ソリューションの AppSource パッケージを作成する](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="175c9-161">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="175c9-162">パッケージをアップロードしてプランを発行する</span><span class="sxs-lookup"><span data-stu-id="175c9-162">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="175c9-163">左側のナビゲーションウィンドウで、[ **商用 Marketplace**] を選択し、[ **技術構成**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-163">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="175c9-164">[ **基本ライセンスモデル**] で、[ **ユーザー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-164">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="175c9-165">[ **CRM パッケージ**] に、パッケージの場所の URL を入力します。</span><span class="sxs-lookup"><span data-stu-id="175c9-165">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="175c9-166">左側のナビゲーションウィンドウの他のタブを使用して、その他の必要な情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="175c9-166">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="175c9-167">完了したら、[ **レビューと発行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-167">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="175c9-168">プランを発行した後、お客様の情報を確認して確認します。</span><span class="sxs-lookup"><span data-stu-id="175c9-168">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="175c9-169">このプロセスに問題がある場合は、お客様に通知します。</span><span class="sxs-lookup"><span data-stu-id="175c9-169">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="175c9-170">すべての問題が解決されると、プランが AppSource で利用可能であることを知らせる通知を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="175c9-170">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="175c9-171">その時点で、有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="175c9-171">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="175c9-172">パートナーセンターでプランをライブにする</span><span class="sxs-lookup"><span data-stu-id="175c9-172">Make your offer live in Partner Center</span></span>

<span data-ttu-id="175c9-173">次の手順では、AppSource でプランをライブにするプロセスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="175c9-173">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="175c9-174">このプロセスの詳細については、「 [リストオプションの概要](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="175c9-174">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="175c9-175">プランを発行すると、4-6 時間がかかります。</span><span class="sxs-lookup"><span data-stu-id="175c9-175">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="175c9-176">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="175c9-176">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="175c9-177">左側のナビゲーションメニューで、[ **商用 Marketplace/概要**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-177">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="175c9-178">[ **概要** ] ページで、探しているプランを見つけます。</span><span class="sxs-lookup"><span data-stu-id="175c9-178">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="175c9-179">発行準備が完了したプランの状態は " **プレビュー**" になります。</span><span class="sxs-lookup"><span data-stu-id="175c9-179">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="175c9-180">プランを選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-180">Select the offer.</span></span>
4. <span data-ttu-id="175c9-181">[ **プランの概要** ] ページで、[ **ライブ** にする] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-181">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="175c9-182">このプランは、4-6 時間以内に有効になります。</span><span class="sxs-lookup"><span data-stu-id="175c9-182">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="175c9-183">AppSource でプランの一覧を表示するには、**プランの概要** ページの下部にある [ **appsource** ] リンクを選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-183">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="175c9-184">**ライセンスが有効なプランの** 場合: プランでライセンスチェックが必要な場合、ユーザーは [ **Contact Me**] をクリックして潜在顧客を入力するだけで、連絡を取ることができます。</span><span class="sxs-lookup"><span data-stu-id="175c9-184">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="175c9-185">**無料インストールオプションを使用したライセンスが有効なプランの** 場合: プランでライセンスチェックが必要ない場合、管理者のユーザーには [**今すぐ入手**] ボタンが表示され **ます。**</span><span class="sxs-lookup"><span data-stu-id="175c9-185">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="175c9-186">無料のインストールオプションを試す場合は、[ **今すぐ入手** する] をクリックします。これにより、Power Platform 管理センターにプランがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="175c9-186">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="175c9-187">質問がある場合、または有料プランにアップグレードする場合は、ユーザーは引き続き **Contact Me** を使用できます。</span><span class="sxs-lookup"><span data-stu-id="175c9-187">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-deal-registration"></a><span data-ttu-id="175c9-188">ISV Connect の登録に関する案件の登録</span><span class="sxs-lookup"><span data-stu-id="175c9-188">Register ISV Connect deal in Deal Registration</span></span>

<span data-ttu-id="175c9-189">顧客にライセンスを割り当てる前に、各販売がパートナーセンターに登録されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="175c9-189">Before you can assign licenses to a customer, each sale needs to be registered in Partner Center.</span></span> <span data-ttu-id="175c9-190">これを行うには、「 [取引を登録](register-deals.md)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="175c9-190">To do this, see [Register your deals](register-deals.md).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="175c9-191">顧客を招待する</span><span class="sxs-lookup"><span data-stu-id="175c9-191">Invite the customer</span></span>

<span data-ttu-id="175c9-192">次の手順を使用して、この取引に参加するよう顧客を招待します。</span><span class="sxs-lookup"><span data-stu-id="175c9-192">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="175c9-193">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="175c9-193">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="175c9-194">左側のナビゲーションメニューで、[ **商用 Marketplace/概要**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-194">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="175c9-195">左側のナビゲーションメニューで、[ **紹介**] を選択し、[ **取引登録**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-195">On the left navigation menu, select **Referrals**, and then select **Deal Registration**.</span></span>
4. <span data-ttu-id="175c9-196">**送信** された取引をフィルター処理し、[**進行中**] タブを選択して、目的の取引を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-196">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
5. <span data-ttu-id="175c9-197">この案件の [概要] ページで、[ **ライセンスの管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-197">On the overview page for this deal, select **Manage licenses**.</span></span>
6. <span data-ttu-id="175c9-198">[ **ライセンスの管理** ] ウィンドウで、[顧客の **詳細** ] ドロップダウンリストから顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-198">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="175c9-199">顧客の関係がまだ存在しない場合は、[ **+ 新しい顧客を招待**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-199">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
7. <span data-ttu-id="175c9-200">表示されているリンクをコピーします。</span><span class="sxs-lookup"><span data-stu-id="175c9-200">Copy the link that is displayed.</span></span>
8. <span data-ttu-id="175c9-201">お客様の課金管理者またはグローバル管理者にこのリンクを電子メールで送信し、このリンクを使用して admin.microsoft.com にアクセスし、確立しているリレーションシップを受け入れて承認します。</span><span class="sxs-lookup"><span data-stu-id="175c9-201">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="175c9-202">顧客がこの手順を実行するまで、リレーションシップは確立されません。</span><span class="sxs-lookup"><span data-stu-id="175c9-202">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="175c9-203">ライセンスのアクティブ化、管理、および削除</span><span class="sxs-lookup"><span data-stu-id="175c9-203">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="175c9-204">お客様があなたとの関係を承認したら、プランの追加を開始し、各プランにライセンスを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="175c9-204">Once your customer has authorized the relationship with you, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="175c9-205">この処理の [ライセンスの管理] ウィンドウで、[ **+ プランの追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-205">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="175c9-206">[ **このソリューションのプラン** ] フィールドと [ **ライセンス数** ] フィールドを入力し、[ **ライセンスの更新**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-206">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="175c9-207">ライセンスは、顧客が管理して従業員に割り当てを行うために admin.microsoft.com で利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="175c9-207">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="175c9-208">既存のプランのライセンス数を変更するには、[ **ライセンス数** ] フィールドに新しい番号を入力し、[ **ライセンスの更新**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-208">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="175c9-209">案件のライセンスを非アクティブ化または削除するには、[ **アクション** ] フィールドのごみ箱アイコンを選択し、[ **更新ライセンス**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="175c9-209">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="175c9-210">次の手順</span><span class="sxs-lookup"><span data-stu-id="175c9-210">Next steps</span></span>

[<span data-ttu-id="175c9-211">ライセンスに関するリソース</span><span class="sxs-lookup"><span data-stu-id="175c9-211">Licensing resources</span></span>](support-resources-licensing.md)
