---
title: Marketplace プランでのライセンスの管理
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ISV コマーシャルマーケットプレースプランのライセンスを設定および管理する方法について説明します。
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284874"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="b42eb-103">Marketplace プランでのライセンスの管理</span><span class="sxs-lookup"><span data-stu-id="b42eb-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="b42eb-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="b42eb-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b42eb-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="b42eb-105">Global admin</span></span>
- <span data-ttu-id="b42eb-106">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="b42eb-106">Account admin</span></span>

<span data-ttu-id="b42eb-107">この記事では、パートナーセンターでオファーを設定し、Microsoft AppSource で使用できるようにし、そのプランのライセンスを管理するプロセスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="b42eb-108">この記事の機能は、現在パブリックプレビュー段階です。</span><span class="sxs-lookup"><span data-stu-id="b42eb-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="b42eb-109">始める前に</span><span class="sxs-lookup"><span data-stu-id="b42eb-109">Before you begin</span></span>

<span data-ttu-id="b42eb-110">このプロセスを開始する前に、以下の情報について理解しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="b42eb-110">Before beginning this process, you should familiarize yourself with the information below.</span></span>

### <a name="review-the-azure-marketplace-documentation"></a><span data-ttu-id="b42eb-111">Azure Marketplace のドキュメントを確認する</span><span class="sxs-lookup"><span data-stu-id="b42eb-111">Review the Azure Marketplace documentation</span></span>

<span data-ttu-id="b42eb-112">次の記事には、続行する前に理解しておく必要がある情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b42eb-112">The articles below contain information you should know before continuing.</span></span> 

- [<span data-ttu-id="b42eb-113">Dynamics 365 for Customer Engagement & PowerApps オファーの作成</span><span class="sxs-lookup"><span data-stu-id="b42eb-113">Create a Dynamics 365 for Customer Engagement & PowerApps offer</span></span>](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [<span data-ttu-id="b42eb-114">パートナー センターでコマーシャル マーケットプレース アカウントを作成する</span><span class="sxs-lookup"><span data-stu-id="b42eb-114">Create a commercial marketplace account in Partner Center</span></span>](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a><span data-ttu-id="b42eb-115">プラン ID を作成する</span><span class="sxs-lookup"><span data-stu-id="b42eb-115">Create your Offer ID</span></span>

<span data-ttu-id="b42eb-116">以下の手順では、プラン ID を入力するように求められます。</span><span class="sxs-lookup"><span data-stu-id="b42eb-116">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="b42eb-117">次の点に注意して、適切なプラン ID を取得してください。</span><span class="sxs-lookup"><span data-stu-id="b42eb-117">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="b42eb-118">この ID は、マーケットプレース オファーの Web アドレスと Azure Resource Manager テンプレート (該当する場合) で顧客に表示されます。</span><span class="sxs-lookup"><span data-stu-id="b42eb-118">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="b42eb-119">オファー ID の長さはパブリッシャー ID の組み合わせで 40 文字以下にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b42eb-119">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="b42eb-120">使用できるのは小文字と数字だけです。</span><span class="sxs-lookup"><span data-stu-id="b42eb-120">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="b42eb-121">プラン ID には、ハイフンとアンダースコアを含めることができますが、スペースは使用できません。</span><span class="sxs-lookup"><span data-stu-id="b42eb-121">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="b42eb-122">たとえば、発行元 ID が testpublisherid で、「test-1」と入力した場合、オファー web アドレスはになり https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 ます。</span><span class="sxs-lookup"><span data-stu-id="b42eb-122">For example, if your Publisher ID is testpublisherid and you enter test-offer-1, the offer web address will be https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1.</span></span>
- <span data-ttu-id="b42eb-123">**[作成]** を選択した後にこの ID を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="b42eb-123">This ID can't be changed after you select **Create**.</span></span>

### <a name="create-your-offer-alias"></a><span data-ttu-id="b42eb-124">プランのエイリアスを作成する</span><span class="sxs-lookup"><span data-stu-id="b42eb-124">Create your Offer alias</span></span>

<span data-ttu-id="b42eb-125">プランのエイリアスは、パートナーセンターでオファーに使用される名前です。</span><span class="sxs-lookup"><span data-stu-id="b42eb-125">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="b42eb-126">次のガイドラインに従う適切なプランのエイリアスも必要になります。</span><span class="sxs-lookup"><span data-stu-id="b42eb-126">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="b42eb-127">この名前はマーケットプレースでは使用されず、顧客に表示されるオファー名やその他の値とは異なります。</span><span class="sxs-lookup"><span data-stu-id="b42eb-127">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="b42eb-128">[作成] を選択した後にこの名前を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="b42eb-128">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="b42eb-129">プランを作成する</span><span class="sxs-lookup"><span data-stu-id="b42eb-129">Create your offer</span></span>

<span data-ttu-id="b42eb-130">ライセンスプロセスの最初の手順は、市販の marketplace プランを作成することです。</span><span class="sxs-lookup"><span data-stu-id="b42eb-130">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="b42eb-131">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="b42eb-131">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="b42eb-132">左側のナビゲーションメニューで、[ **商用 Marketplace/概要**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-132">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="b42eb-133">[概要] ページの上部にある [ **新しいプラン**] を選択し、[ **顧客エンゲージメント用の Dynamics 365 & PowerApps**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-133">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="b42eb-134">前の手順で作成した **プラン ID** と **プランのエイリアス** を入力します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-134">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="b42eb-135">**[作成]** を選択してオファーを生成し、続行します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-135">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="b42eb-136">ライセンスオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-136">Choose your licensing options.</span></span>

    - <span data-ttu-id="b42eb-137">プランのライセンス管理を有効にするには、[ **Microsoft によるアプリライセンス管理を有効** にする] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-137">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="b42eb-138">これは1回限りの設定であり、プランを発行した後に変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="b42eb-138">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="b42eb-139">また、顧客がライセンスを使用せずにアプリの基本機能を実行し、ライセンスを購入した後に premium 機能を実行できるようにすることもできます。</span><span class="sxs-lookup"><span data-stu-id="b42eb-139">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="b42eb-140">これを行うには、[ **ライセンスが割り当てられていない場合でも、顧客がアプリをインストールできるように** する] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-140">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="b42eb-141">プランのライセンス管理を有効にしない場合は、[ **今すぐ入手する (無料)**]、[ **無料試用版**]、または [ **連絡してください**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-141">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="b42eb-142">プランを作成する</span><span class="sxs-lookup"><span data-stu-id="b42eb-142">Create your plan</span></span>

<span data-ttu-id="b42eb-143">この手順では、プランに対して有効にするプランを定義します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-143">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="b42eb-144">左側のナビゲーションメニューで、[ **プランの概要**] を選択し、[ **新しいプランの作成**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-144">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="b42eb-145">**プラン ID** と **プラン名** を入力し、[**作成**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-145">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="b42eb-146">[ **プランの一覧** ] ページで、 **プランの説明** を入力します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-146">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="b42eb-147">説明を保存して後で終了するには、[ **下書きの保存**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-147">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="b42eb-148">操作が完了したら、[ **レビューと発行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-148">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="b42eb-149">プランの情報が、[プランの一覧 (プラン] セクション) の appsource.microsoft.com に表示されるようになります。</span><span class="sxs-lookup"><span data-stu-id="b42eb-149">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="b42eb-150">このプランのプランをすべて作成したら、各プランのサービス ID をコピーする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b42eb-150">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="b42eb-151">プランの一覧ページの上部にある [ **プランの概要** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-151">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="b42eb-152">各プランのサービス ID を安全な場所にコピーします。</span><span class="sxs-lookup"><span data-stu-id="b42eb-152">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="b42eb-153">ソリューションへのサービス Id の追加</span><span class="sxs-lookup"><span data-stu-id="b42eb-153">Add Service IDs to your solution</span></span>

<span data-ttu-id="b42eb-154">次の手順では、先ほどコピーした各プランのサービス Id を追加して、ソリューションを更新します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-154">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="b42eb-155">この詳細については、「 [ソリューションの AppSource パッケージを作成する](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b42eb-155">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="b42eb-156">パッケージをアップロードしてプランを発行する</span><span class="sxs-lookup"><span data-stu-id="b42eb-156">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="b42eb-157">左側のナビゲーションウィンドウで、[ **商用 Marketplace**] を選択し、[ **技術構成**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-157">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="b42eb-158">[ **基本ライセンスモデル**] で、[ **ユーザー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-158">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="b42eb-159">[ **CRM パッケージ**] に、パッケージの場所の URL を入力します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-159">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="b42eb-160">左側のナビゲーションウィンドウの他のタブを使用して、その他の必要な情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-160">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="b42eb-161">完了したら、[ **レビューと発行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-161">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="b42eb-162">プランを発行した後、お客様の情報を確認して確認します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-162">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="b42eb-163">このプロセスに問題がある場合は、お客様に通知します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-163">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="b42eb-164">すべての問題が解決されると、プランが AppSource で利用可能であることを知らせる通知を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="b42eb-164">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="b42eb-165">その時点で、有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b42eb-165">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="b42eb-166">パートナーセンターでプランをライブにする</span><span class="sxs-lookup"><span data-stu-id="b42eb-166">Make your offer live in Partner Center</span></span>

<span data-ttu-id="b42eb-167">次の手順では、AppSource でプランをライブにするプロセスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-167">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="b42eb-168">このプロセスの詳細については、「 [リストオプションの概要](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b42eb-168">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="b42eb-169">プランを発行すると、4-6 時間がかかります。</span><span class="sxs-lookup"><span data-stu-id="b42eb-169">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="b42eb-170">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="b42eb-170">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="b42eb-171">左側のナビゲーションメニューで、[ **商用 Marketplace/概要**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-171">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="b42eb-172">[ **概要** ] ページで、探しているプランを見つけます。</span><span class="sxs-lookup"><span data-stu-id="b42eb-172">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="b42eb-173">発行準備が完了したプランの状態は " **プレビュー**" になります。</span><span class="sxs-lookup"><span data-stu-id="b42eb-173">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="b42eb-174">プランを選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-174">Select the offer.</span></span>
4. <span data-ttu-id="b42eb-175">[ **プランの概要** ] ページで、[ **ライブ** にする] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-175">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="b42eb-176">このプランは、4-6 時間以内に有効になります。</span><span class="sxs-lookup"><span data-stu-id="b42eb-176">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="b42eb-177">AppSource でプランの一覧を表示するには、**プランの概要** ページの下部にある [ **appsource** ] リンクを選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-177">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="b42eb-178">**ライセンスが有効なプランの** 場合: プランでライセンスチェックが必要な場合、ユーザーは [ **Contact Me**] をクリックして潜在顧客を入力するだけで、連絡を取ることができます。</span><span class="sxs-lookup"><span data-stu-id="b42eb-178">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="b42eb-179">**無料インストールオプションを使用したライセンスが有効なプランの** 場合: プランでライセンスチェックが必要ない場合、管理者のユーザーには [**今すぐ入手**] ボタンが表示され **ます。**</span><span class="sxs-lookup"><span data-stu-id="b42eb-179">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="b42eb-180">無料のインストールオプションを試す場合は、[ **今すぐ入手** する] をクリックします。これにより、Power Platform 管理センターにプランがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="b42eb-180">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="b42eb-181">質問がある場合、または有料プランにアップグレードする場合は、ユーザーは引き続き **Contact Me** を使用できます。</span><span class="sxs-lookup"><span data-stu-id="b42eb-181">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-dealreg"></a><span data-ttu-id="b42eb-182">DealReg に ISV Connect 取引を登録する</span><span class="sxs-lookup"><span data-stu-id="b42eb-182">Register ISV Connect deal in DealReg</span></span>

<span data-ttu-id="b42eb-183">次の手順では、取引を登録します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-183">The next step is to register your deal.</span></span> <span data-ttu-id="b42eb-184">これを行うには、「 [取引を登録](https://docs.microsoft.com/partner-center/register-deals)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b42eb-184">To do this, see [Register your deals](https://docs.microsoft.com/partner-center/register-deals).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="b42eb-185">顧客を招待する</span><span class="sxs-lookup"><span data-stu-id="b42eb-185">Invite the customer</span></span>

<span data-ttu-id="b42eb-186">次の手順を使用して、この取引に参加するよう顧客を招待します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-186">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="b42eb-187">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="b42eb-187">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="b42eb-188">左側のナビゲーションメニューで、[ **商用 Marketplace/概要**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-188">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="b42eb-189">**送信** された取引をフィルター処理し、[**進行中**] タブを選択して、目的の取引を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-189">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
4. <span data-ttu-id="b42eb-190">この案件の [概要] ページで、[ **ライセンスの管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-190">On the overview page for this deal, select **Manage licenses**.</span></span>
5. <span data-ttu-id="b42eb-191">[ **ライセンスの管理** ] ウィンドウで、[顧客の **詳細** ] ドロップダウンリストから顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-191">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="b42eb-192">顧客の関係がまだ存在しない場合は、[ **+ 新しい顧客を招待**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-192">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
6. <span data-ttu-id="b42eb-193">表示されているリンクをコピーします。</span><span class="sxs-lookup"><span data-stu-id="b42eb-193">Copy the link that is displayed.</span></span>
7. <span data-ttu-id="b42eb-194">お客様の課金管理者またはグローバル管理者にこのリンクを電子メールで送信し、このリンクを使用して admin.microsoft.com にアクセスし、確立しているリレーションシップを受け入れて承認します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-194">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="b42eb-195">顧客がこの手順を実行するまで、リレーションシップは確立されません。</span><span class="sxs-lookup"><span data-stu-id="b42eb-195">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="b42eb-196">ライセンスのアクティブ化、管理、および削除</span><span class="sxs-lookup"><span data-stu-id="b42eb-196">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="b42eb-197">顧客がいったん確立されたら、プランの追加を開始し、各プランにライセンスを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="b42eb-197">Once your customer has been established, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="b42eb-198">この処理の [ライセンスの管理] ウィンドウで、[ **+ プランの追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-198">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="b42eb-199">[ **このソリューションのプラン** ] フィールドと [ **ライセンス数** ] フィールドを入力し、[ **ライセンスの更新**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-199">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="b42eb-200">ライセンスは、顧客が管理して従業員に割り当てを行うために admin.microsoft.com で利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="b42eb-200">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="b42eb-201">既存のプランのライセンス数を変更するには、[ **ライセンス数** ] フィールドに新しい番号を入力し、[ **ライセンスの更新**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-201">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="b42eb-202">案件のライセンスを非アクティブ化または削除するには、[ **アクション** ] フィールドのごみ箱アイコンを選択し、[ **更新ライセンス**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b42eb-202">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>