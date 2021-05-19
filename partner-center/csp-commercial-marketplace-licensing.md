---
title: マーケットプレース プランでのライセンスの管理
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ISV コマーシャルマーケットプレースプランのライセンスを設定および管理する方法について説明します。
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c128b99b034564bcaa100ca975253f8b1bad7a42
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147957"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="3216a-103">マーケットプレース プランでのライセンスの管理</span><span class="sxs-lookup"><span data-stu-id="3216a-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="3216a-104">**適切なロール**: 全体管理者 |アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="3216a-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="3216a-105">この記事では、パートナーセンターでオファーを設定し、Microsoft AppSource で使用できるようにし、そのプランのライセンスを管理するプロセスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="3216a-105">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="3216a-106">この記事の機能は、現在パブリックプレビュー段階です。</span><span class="sxs-lookup"><span data-stu-id="3216a-106">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="3216a-107">開始する前に</span><span class="sxs-lookup"><span data-stu-id="3216a-107">Before you begin</span></span>

### <a name="commercial-marketplace-basics"></a><span data-ttu-id="3216a-108">商用マーケットプレースの基本</span><span class="sxs-lookup"><span data-stu-id="3216a-108">Commercial marketplace basics</span></span>

<span data-ttu-id="3216a-109">このプロセスを開始する前に、コマーシャルマーケットプレースの基本を理解しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="3216a-109">Before you begin this process, you should familiarize yourself with the basics of the commercial marketplace.</span></span> <span data-ttu-id="3216a-110">次の表の記事は、作業を開始するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="3216a-110">The articles in the table below will help get you started.</span></span> 

| <span data-ttu-id="3216a-111">トピック</span><span class="sxs-lookup"><span data-stu-id="3216a-111">Topic</span></span>  | <span data-ttu-id="3216a-112">[アーティクル]</span><span class="sxs-lookup"><span data-stu-id="3216a-112">Article</span></span>  |
|-------|--------|
|<span data-ttu-id="3216a-113">商用 marketplace プラン</span><span class="sxs-lookup"><span data-stu-id="3216a-113">Commercial marketplace plans</span></span> | [<span data-ttu-id="3216a-114">コマーシャル マーケットプレース オファーのプランと価格</span><span class="sxs-lookup"><span data-stu-id="3216a-114">Plans and pricing for commercial marketplace offers</span></span>](/azure/marketplace/plans-pricing)    |
|<span data-ttu-id="3216a-115">商用 marketplace プラン</span><span class="sxs-lookup"><span data-stu-id="3216a-115">Commercial marketplace offers</span></span>  | [<span data-ttu-id="3216a-116">リストの種類</span><span class="sxs-lookup"><span data-stu-id="3216a-116">Listing types</span></span>](/azure/marketplace/determine-your-listing-type)    |
|<span data-ttu-id="3216a-117">商用 marketplace アカウント</span><span class="sxs-lookup"><span data-stu-id="3216a-117">Commercial marketplace accounts</span></span> |  [<span data-ttu-id="3216a-118">パートナー センターでコマーシャル マーケットプレース アカウントを作成する</span><span class="sxs-lookup"><span data-stu-id="3216a-118">Create a commercial marketplace account in Partner Center</span></span>](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a><span data-ttu-id="3216a-119">プラン ID を確認する</span><span class="sxs-lookup"><span data-stu-id="3216a-119">Determine your Offer ID</span></span>

<span data-ttu-id="3216a-120">以下の手順では、プラン ID を入力するように求められます。</span><span class="sxs-lookup"><span data-stu-id="3216a-120">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="3216a-121">次の点に注意して、適切なプラン ID を取得してください。</span><span class="sxs-lookup"><span data-stu-id="3216a-121">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="3216a-122">この ID は、マーケットプレース オファーの Web アドレスと Azure Resource Manager テンプレート (該当する場合) で顧客に表示されます。</span><span class="sxs-lookup"><span data-stu-id="3216a-122">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="3216a-123">オファー ID の長さはパブリッシャー ID の組み合わせで 40 文字以下にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="3216a-123">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="3216a-124">使用できるのは小文字と数字だけです。</span><span class="sxs-lookup"><span data-stu-id="3216a-124">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="3216a-125">プラン ID には、ハイフンとアンダースコアを含めることができますが、スペースは使用できません。</span><span class="sxs-lookup"><span data-stu-id="3216a-125">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="3216a-126">たとえば、発行元 ID がで、「」と入力した場合、 `testpublisherid` `test-offer-1` オファー web アドレスはになり `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` ます。</span><span class="sxs-lookup"><span data-stu-id="3216a-126">For example, if your Publisher ID is `testpublisherid` and you enter `test-offer-1`, the offer web address will be `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1`.</span></span>
- <span data-ttu-id="3216a-127">**[作成]** を選択した後にこの ID を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="3216a-127">This ID can't be changed after you select **Create**.</span></span>

### <a name="determine-your-offer-alias"></a><span data-ttu-id="3216a-128">プランのエイリアスを確認する</span><span class="sxs-lookup"><span data-stu-id="3216a-128">Determine your Offer alias</span></span>

<span data-ttu-id="3216a-129">プランのエイリアスは、パートナーセンターでオファーに使用される名前です。</span><span class="sxs-lookup"><span data-stu-id="3216a-129">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="3216a-130">次のガイドラインに従う適切なプランのエイリアスも必要になります。</span><span class="sxs-lookup"><span data-stu-id="3216a-130">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="3216a-131">この名前はマーケットプレースでは使用されず、顧客に表示されるオファー名やその他の値とは異なります。</span><span class="sxs-lookup"><span data-stu-id="3216a-131">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="3216a-132">[作成] を選択した後にこの名前を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="3216a-132">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="3216a-133">プランを作成する</span><span class="sxs-lookup"><span data-stu-id="3216a-133">Create your offer</span></span>

<span data-ttu-id="3216a-134">ライセンスプロセスの最初の手順は、市販の marketplace プランを作成することです。</span><span class="sxs-lookup"><span data-stu-id="3216a-134">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="3216a-135">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="3216a-135">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="3216a-136">左側のナビゲーション メニューで、[コマーシャル マーケットプレース **/概要] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="3216a-136">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="3216a-137">[概要] ページの上部にある[新しいオファー] を選択し **、[Dynamics 365 for Customer Engagement & PowerApps] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="3216a-137">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="3216a-138">前に **作成したオファー ID** **とオファーエイリアス** を入力します。</span><span class="sxs-lookup"><span data-stu-id="3216a-138">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="3216a-139">**[作成]** を選択してオファーを生成し、続行します。</span><span class="sxs-lookup"><span data-stu-id="3216a-139">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="3216a-140">ライセンス オプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="3216a-140">Choose your licensing options.</span></span>

    - <span data-ttu-id="3216a-141">オファーのライセンス管理を有効にするには、[Microsoft によるアプリ **ライセンス管理を有効にする] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="3216a-141">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="3216a-142">これは 1 回だけ設定され、オファーが発行された後は変更できます。</span><span class="sxs-lookup"><span data-stu-id="3216a-142">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="3216a-143">また、顧客がライセンスなしでアプリの基本機能を実行したり、ライセンスを購入した後に Premium 機能を実行したりすることもできます。</span><span class="sxs-lookup"><span data-stu-id="3216a-143">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="3216a-144">これを行うには、[ライセンスが割り当てられていない場合でも、顧客に **アプリのインストールを許可する] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="3216a-144">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="3216a-145">オファーでライセンス管理を有効にしない場合は、[ 今すぐ取得 **する (** 無料) ] 、 [無料試用版] 、 または [連絡する]**を選択します**。</span><span class="sxs-lookup"><span data-stu-id="3216a-145">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="3216a-146">プランを作成する</span><span class="sxs-lookup"><span data-stu-id="3216a-146">Create your plan</span></span>

<span data-ttu-id="3216a-147">これらの手順では、オファーに対して有効にするプランを定義します。</span><span class="sxs-lookup"><span data-stu-id="3216a-147">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="3216a-148">左側のナビゲーション メニューで、[プランの概要] **を選択し**、[新しいプランの **作成] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="3216a-148">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="3216a-149">[プラン **ID] と [** プラン名] **を入力し**、[作成] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="3216a-149">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="3216a-150">[プランの **一覧] ページ** で、プランの説明 **を入力します**。</span><span class="sxs-lookup"><span data-stu-id="3216a-150">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="3216a-151">説明を保存し、後で完了するには、[下書きの保存] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="3216a-151">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="3216a-152">完了したら、 [確認して発行 **] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="3216a-152">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="3216a-153">プラン情報は、オファーの一覧 (appsource.microsoft.com セクション) の下に表示されます。</span><span class="sxs-lookup"><span data-stu-id="3216a-153">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="3216a-154">このオファーのすべてのプランを作成したら、各プランのサービス ID をコピーする必要があります。</span><span class="sxs-lookup"><span data-stu-id="3216a-154">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="3216a-155">[ **プランの一覧]** ページの上部にある [プランの概要] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3216a-155">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="3216a-156">各プランのサービス ID を安全な場所にコピーします。</span><span class="sxs-lookup"><span data-stu-id="3216a-156">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="3216a-157">サービスの ID をソリューションに追加する</span><span class="sxs-lookup"><span data-stu-id="3216a-157">Add Service IDs to your solution</span></span>

<span data-ttu-id="3216a-158">次の手順では、先ほどコピーした各プランのサービス Id を追加して、ソリューションを更新します。</span><span class="sxs-lookup"><span data-stu-id="3216a-158">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="3216a-159">この詳細については、「 [ソリューションの AppSource パッケージを作成する](/powerapps/developer/data-platform/create-package-app-appsource)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3216a-159">For guidance on this, see [Create an AppSource Package for your solution](/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="3216a-160">パッケージをアップロードしてプランを発行する</span><span class="sxs-lookup"><span data-stu-id="3216a-160">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="3216a-161">左側のナビゲーションウィンドウで、[ **商用 Marketplace**] を選択し、[ **技術構成**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3216a-161">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="3216a-162">[ **基本ライセンスモデル**] で、[ **ユーザー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3216a-162">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="3216a-163">[ **CRM パッケージ**] に、パッケージの場所の URL を入力します。</span><span class="sxs-lookup"><span data-stu-id="3216a-163">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="3216a-164">左側のナビゲーションウィンドウの他のタブを使用して、その他の必要な情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="3216a-164">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="3216a-165">完了したら、[ **レビューと発行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3216a-165">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="3216a-166">プランを発行した後、お客様の情報を確認して確認します。</span><span class="sxs-lookup"><span data-stu-id="3216a-166">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="3216a-167">このプロセスに問題がある場合は、お客様に通知します。</span><span class="sxs-lookup"><span data-stu-id="3216a-167">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="3216a-168">すべての問題が解決されると、プランが AppSource で利用可能であることを知らせる通知を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="3216a-168">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="3216a-169">その時点で、有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3216a-169">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="3216a-170">パートナーセンターでプランをライブにする</span><span class="sxs-lookup"><span data-stu-id="3216a-170">Make your offer live in Partner Center</span></span>

<span data-ttu-id="3216a-171">次の手順では、AppSource でプランをライブにするプロセスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="3216a-171">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="3216a-172">このプロセスの詳細については、「 [リストオプションの概要](/azure/marketplace/determine-your-listing-type)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3216a-172">To learn more about this process, see [Introduction to listing options](/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="3216a-173">プランを発行すると、4-6 時間がかかります。</span><span class="sxs-lookup"><span data-stu-id="3216a-173">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="3216a-174">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="3216a-174">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="3216a-175">左側のナビゲーションメニューで、[ **商用 Marketplace/概要**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3216a-175">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="3216a-176">[ **概要** ] ページで、探しているプランを見つけます。</span><span class="sxs-lookup"><span data-stu-id="3216a-176">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="3216a-177">発行準備が完了したプランの状態は " **プレビュー**" になります。</span><span class="sxs-lookup"><span data-stu-id="3216a-177">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="3216a-178">オファーを選択します。</span><span class="sxs-lookup"><span data-stu-id="3216a-178">Select the offer.</span></span>
4. <span data-ttu-id="3216a-179">[ **プランの概要** ] ページで、[ **ライブ** にする] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3216a-179">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="3216a-180">オファーは 4 ~ 6 時間以内に提供されます。</span><span class="sxs-lookup"><span data-stu-id="3216a-180">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="3216a-181">AppSource でオファーの一覧を表示するには、[オファーの概要] ページの下部にある **[AppSource]** **リンクを選択** します。</span><span class="sxs-lookup"><span data-stu-id="3216a-181">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="3216a-182">**ライセンスが有効** なオファーの場合: オファーでライセンス チェックが必要な場合、ユーザーは [連絡してください]をクリックしてリードを入力するだけなので、ユーザーと通信できます。</span><span class="sxs-lookup"><span data-stu-id="3216a-182">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="3216a-183">**無料インストール オプション** を使用したライセンスが有効なオファーの場合: オファーでライセンス チェックが必要ない場合、管理者ユーザーには、[連絡] に加えて [今すぐ取得] ボタン **が表示されます**。</span><span class="sxs-lookup"><span data-stu-id="3216a-183">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="3216a-184">無料のインストール オプションを試したいユーザーは、[今すぐ取得] をクリックする必要があります。このオプションをクリックすると、管理センターにオファー Power Platformされます。</span><span class="sxs-lookup"><span data-stu-id="3216a-184">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="3216a-185">ユーザーは、質問 **がある場合や** 有料プランにアップグレードする場合は、引き続き [連絡する] を使用できます。</span><span class="sxs-lookup"><span data-stu-id="3216a-185">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-deal-registration"></a><span data-ttu-id="3216a-186">取引登録で ISV Connect 取引を登録する</span><span class="sxs-lookup"><span data-stu-id="3216a-186">Register ISV Connect deal in Deal Registration</span></span>

<span data-ttu-id="3216a-187">顧客にライセンスを割り当てる前に、各販売を顧客に登録パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="3216a-187">Before you can assign licenses to a customer, each sale needs to be registered in Partner Center.</span></span> <span data-ttu-id="3216a-188">これを行うには、「取引を [登録する」を参照してください](register-deals.md)。</span><span class="sxs-lookup"><span data-stu-id="3216a-188">To do this, see [Register your deals](register-deals.md).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="3216a-189">顧客を招待する</span><span class="sxs-lookup"><span data-stu-id="3216a-189">Invite the customer</span></span>

<span data-ttu-id="3216a-190">この取引に参加する顧客を招待するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="3216a-190">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="3216a-191">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="3216a-191">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="3216a-192">左側のナビゲーション メニューで、[コマーシャル マーケットプレース **/概要] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="3216a-192">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="3216a-193">左側のナビゲーション メニューで[紹介] **を選択** し、[Deal **Registration]を選択します**。</span><span class="sxs-lookup"><span data-stu-id="3216a-193">On the left navigation menu, select **Referrals**, and then select **Deal Registration**.</span></span>
4. <span data-ttu-id="3216a-194">[送信された **取引]** をフィルター処理し、[進行中] **タブを** 選択して、目的の取引を選択します。</span><span class="sxs-lookup"><span data-stu-id="3216a-194">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
5. <span data-ttu-id="3216a-195">この取引の概要ページで、[ライセンスの管理] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="3216a-195">On the overview page for this deal, select **Manage licenses**.</span></span>
6. <span data-ttu-id="3216a-196">[ライセンスの **管理] ウィンドウ** で、[顧客の詳細] ドロップダウン **リストから顧客を** 選択します。</span><span class="sxs-lookup"><span data-stu-id="3216a-196">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="3216a-197">顧客関係がまだ存在しない場合は、 [+ 新しい顧客を **同意する招待] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="3216a-197">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
7. <span data-ttu-id="3216a-198">表示されるリンクをコピーします。</span><span class="sxs-lookup"><span data-stu-id="3216a-198">Copy the link that is displayed.</span></span>
8. <span data-ttu-id="3216a-199">顧客の課金管理者またはグローバル管理者にこのリンクを電子メールで送信し、このリンクを使用して admin.microsoft.com にアクセスし、確立している関係を承認します。</span><span class="sxs-lookup"><span data-stu-id="3216a-199">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="3216a-200">顧客がこの手順を実行するまで、リレーションシップは確立されません。</span><span class="sxs-lookup"><span data-stu-id="3216a-200">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="3216a-201">ライセンスのアクティブ化、管理、および削除</span><span class="sxs-lookup"><span data-stu-id="3216a-201">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="3216a-202">お客様があなたとの関係を承認したら、プランの追加を開始し、各プランにライセンスを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="3216a-202">Once your customer has authorized the relationship with you, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="3216a-203">この処理の [ライセンスの管理] ウィンドウで、[ **+ プランの追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3216a-203">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="3216a-204">[ **このソリューションのプラン** ] フィールドと [ **ライセンス数** ] フィールドを入力し、[ **ライセンスの更新**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3216a-204">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="3216a-205">ライセンスは、顧客が管理して従業員に割り当てを行うために admin.microsoft.com で利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="3216a-205">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="3216a-206">既存のプランのライセンス数を変更するには、[ **ライセンス数** ] フィールドに新しい番号を入力し、[ **ライセンスの更新**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3216a-206">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="3216a-207">案件のライセンスを非アクティブ化または削除するには、[ **アクション** ] フィールドのごみ箱アイコンを選択し、[ **更新ライセンス**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3216a-207">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3216a-208">次のステップ</span><span class="sxs-lookup"><span data-stu-id="3216a-208">Next steps</span></span>

[<span data-ttu-id="3216a-209">ライセンスに関するリソース</span><span class="sxs-lookup"><span data-stu-id="3216a-209">Licensing resources</span></span>](support-resources-licensing.md)