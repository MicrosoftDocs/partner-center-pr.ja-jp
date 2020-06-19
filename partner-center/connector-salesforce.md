---
title: Salesforce CRM パートナーセンターの共同販売コネクタ
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターでの紹介を Salesforce CRM と同期する
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: e51ddc8ec3ea568a20404801802548f79cae43d0
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991620"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="b68d2-103">Salesforce CRM のための共同販売コネクタ - 概要</span><span class="sxs-lookup"><span data-stu-id="b68d2-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="b68d2-104">適切なロール</span><span class="sxs-lookup"><span data-stu-id="b68d2-104">Appropriate roles</span></span>

- <span data-ttu-id="b68d2-105">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="b68d2-105">Referrals admin</span></span>
- <span data-ttu-id="b68d2-106">CRM のシステム管理者またはシステムカスタマイザー</span><span class="sxs-lookup"><span data-stu-id="b68d2-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="b68d2-107">パートナーセンターの共同販売コネクタを使用すると、販売元は CRM システム内から Microsoft と共同で販売することができます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="b68d2-108">パートナーセンターを使用して共同販売取引を管理するためのトレーニングを行う必要はありません。</span><span class="sxs-lookup"><span data-stu-id="b68d2-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="b68d2-109">共同販売コネクタを使用して、Microsoft の販売者に連絡したり、Microsoft 販売者からの推薦を受け取ったり、紹介を受け入れたり拒否したりすることができます。また、商談の価値や決算日などの商談データを変更することもできます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="b68d2-110">また、これらの共同販売取引に関するマイクロソフト販売者からの更新を受け取ることもできます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="b68d2-111">パートナーセンターではなく、選択した CRM 内での作業中に、すべての紹介作業を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="b68d2-112">このソリューションは、Microsoft のパワー自動化ソリューションに基づいており、パートナーセンター Api を使用しています。</span><span class="sxs-lookup"><span data-stu-id="b68d2-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="b68d2-113">をインストールする前に-前提条件</span><span class="sxs-lookup"><span data-stu-id="b68d2-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="b68d2-114">**トピック**</span><span class="sxs-lookup"><span data-stu-id="b68d2-114">**Topics**</span></span>   |<span data-ttu-id="b68d2-115">**詳細**</span><span class="sxs-lookup"><span data-stu-id="b68d2-115">**Details**</span></span>   |<span data-ttu-id="b68d2-116">**リンク**</span><span class="sxs-lookup"><span data-stu-id="b68d2-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="b68d2-117">Microsoft Partner Network ID</span><span class="sxs-lookup"><span data-stu-id="b68d2-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="b68d2-118">有効な MPN ID が必要です</span><span class="sxs-lookup"><span data-stu-id="b68d2-118">You need a valid MPN ID</span></span>|<span data-ttu-id="b68d2-119">[MPN](https://partner.microsoft.com/)に参加するには</span><span class="sxs-lookup"><span data-stu-id="b68d2-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="b68d2-120">共同販売の準備完了</span><span class="sxs-lookup"><span data-stu-id="b68d2-120">Co-sell ready</span></span>|<span data-ttu-id="b68d2-121">お客様の IP/サービスソリューションは、共同販売の準備ができている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b68d2-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="b68d2-122">Microsoft との販売</span><span class="sxs-lookup"><span data-stu-id="b68d2-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="b68d2-123">パートナー センター アカウント</span><span class="sxs-lookup"><span data-stu-id="b68d2-123">Partner Center account</span></span>|<span data-ttu-id="b68d2-124">パートナーセンターのテナントに関連付けられている MPN ID は、共同販売ソリューションに関連付けられている MPN ID と同じである必要があります。</span><span class="sxs-lookup"><span data-stu-id="b68d2-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="b68d2-125">コネクタをデプロイする前に、パートナーセンターポータルで共同販売の紹介を確認できることを確認します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="b68d2-126">アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="b68d2-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="b68d2-127">パートナー センターのユーザー ロール</span><span class="sxs-lookup"><span data-stu-id="b68d2-127">Partner Center user roles</span></span>|<span data-ttu-id="b68d2-128">コネクタをインストールして使用する従業員は、参照管理者である必要があります</span><span class="sxs-lookup"><span data-stu-id="b68d2-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="b68d2-129">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="b68d2-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="b68d2-130">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="b68d2-130">Salesforce CRM</span></span>|<span data-ttu-id="b68d2-131">CRM ユーザーロールは、システム管理者またはシステムカスタマイザーです。</span><span class="sxs-lookup"><span data-stu-id="b68d2-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="b68d2-132">Salesforce CRM でロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="b68d2-132">Assign roles in Salesforce CRM</span></span>](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="b68d2-133">パワー自動化フローアカウント</span><span class="sxs-lookup"><span data-stu-id="b68d2-133">Power Automate Flow Account</span></span>|<span data-ttu-id="b68d2-134">CRM システム管理者またはシステムカスタマイザー用のアクティブな[電源自動化](https://flow.microsoft.com)アカウント。</span><span class="sxs-lookup"><span data-stu-id="b68d2-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="b68d2-135">そのユーザーは、インストールの前に少なくとも1回、[電源の自動](https://flow.microsoft.com)登録を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="b68d2-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="b68d2-136">Salesforce CRM のパートナーセンターの紹介同期をインストールする</span><span class="sxs-lookup"><span data-stu-id="b68d2-136">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="b68d2-137">[[パワー自動化](https://flow.microsoft.com)] にアクセスし、右上隅にある [**環境**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="b68d2-138">これにより、使用可能な CRM インスタンスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-138">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="b68d2-139">右上隅にあるドロップダウンから適切な CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="b68d2-140">左側のナビゲーションバーで [**ソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="b68d2-141">上部のメニューの [ **AppSource を開く**] リンクをクリックします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-141">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource を開く":::

5. <span data-ttu-id="b68d2-143">ポップアップ画面で、 **Salesforce のパートナーセンターの紹介コネクタ**を検索します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-143">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="b68d2-145">[**今すぐ入手**する] ボタンをクリックし、[**続行**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="b68d2-146">これにより、Salesforce CRM 環境を選択してアプリケーションをインストールできるページが開きます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-146">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="b68d2-147">使用条件に同意します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-147">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="使用可能な CRMS":::

8. <span data-ttu-id="b68d2-149">その後、[**ソリューションの管理**] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-149">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="b68d2-150">ページの下部にある矢印ボタンを使用して、[パートナーセンターの紹介] に移動します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-150">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="b68d2-151">[パートナーセンターの紹介] ソリューションの横に、[**インストールのスケジュール**] が表示されます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-151">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="b68d2-152">インストールには10-15 分かかります。</span><span class="sxs-lookup"><span data-stu-id="b68d2-152">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="b68d2-153">インストールが完了したら、[Power の[自動化](https://flow.microsoft.com)] に戻り、左側のナビゲーション領域から [**ソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-153">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="b68d2-154">**Salesforce のパートナーセンターの紹介同期**は、[ソリューション] の一覧で確認できます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-154">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="b68d2-155">**Salesforce のパートナーセンター紹介同期**を選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-155">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="b68d2-156">次の電源の自動化フローとエンティティを利用できます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-156">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/salesforce/salesforce-flows.png" alt-text="Salesforce フロー":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="b68d2-158">ベストプラクティス: 運用前にテストする</span><span class="sxs-lookup"><span data-stu-id="b68d2-158">Best Practice: Test before you go live</span></span>

<span data-ttu-id="b68d2-159">運用環境でパワー自動化ソリューションをインストール、構成、およびカスタマイズする前に、必ずステージング CRM インスタンスでソリューションをテストしてください。</span><span class="sxs-lookup"><span data-stu-id="b68d2-159">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="b68d2-160">ステージング環境/CRM インスタンスに Microsoft Power 自動ソリューションをインストールします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-160">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="b68d2-161">ソリューションのコピーを作成し、構成を実行して、ステージング環境でフローのカスタマイズを自動化します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-161">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="b68d2-162">ステージング/CRM インスタンスでソリューションをテストします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-162">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="b68d2-163">成功した場合は、運用インスタンスにマネージドソリューションとしてインポートします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-163">On success, import as managed solution to the production instance.</span></span>

## <a name="configure-the-solution"></a><span data-ttu-id="b68d2-164">ソリューションを構成する</span><span class="sxs-lookup"><span data-stu-id="b68d2-164">Configure the solution</span></span>

1. <span data-ttu-id="b68d2-165">CRM インスタンスにソリューションをインストールしたら、[ [Power の自動化](https://flow.microsoft.com/)] に戻ります。</span><span class="sxs-lookup"><span data-stu-id="b68d2-165">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="b68d2-166">右上隅にある [**環境**] ドロップダウンで、パワー自動化ソリューションをインストールした CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-166">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="b68d2-167">次の3つのユーザーアカウントを関連付ける接続を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b68d2-167">You will need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="b68d2-168">参照管理者の資格情報を持つパートナーセンターのユーザー</span><span class="sxs-lookup"><span data-stu-id="b68d2-168">Partner Center user with referrals admin credentials</span></span>
   - <span data-ttu-id="b68d2-169">パートナー センターのイベント</span><span class="sxs-lookup"><span data-stu-id="b68d2-169">Partner Center Events</span></span>
   - <span data-ttu-id="b68d2-170">Power を使用した CRM 管理ソリューションのフローが自動化されます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-170">CRM admin with the Power Automate flows in the solution.</span></span>

   1. <span data-ttu-id="b68d2-171">左側のナビゲーションバーから [**接続**] を選択し、一覧から "パートナーセンターの紹介" ソリューションを選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-171">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

   2. <span data-ttu-id="b68d2-172">[**接続の作成**] をクリックして接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-172">Create a connection by clicking **Create a connection**.</span></span>

       :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="接続を作成する":::

   3. <span data-ttu-id="b68d2-174">右上隅の検索バーで、**パートナーセンターの参照 (プレビュー)** を検索します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>

   4. <span data-ttu-id="b68d2-175">参照管理者の資格情報ロールを使用して、パートナーセンターユーザーの接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-175">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   5. <span data-ttu-id="b68d2-176">次に、パートナーセンターのユーザーに、参照管理者の資格情報を使用してパートナーセンターのイベント接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-176">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

   6. <span data-ttu-id="b68d2-177">CRM 管理者ユーザーの Common Data Service (現在の環境) の接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-177">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="b68d2-178">電源自動化フローを接続に関連付けるには、各パワー自動化フローを編集して、Common Data Service とパートナーセンターの紹介に接続します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-178">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="b68d2-179">変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-179">Save the changes.</span></span>

5. <span data-ttu-id="b68d2-180">パワー自動化フローを**有効に**します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-180">**Turn on** the the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="b68d2-181">Webhook Api を使用してリソース変更イベントに登録する</span><span class="sxs-lookup"><span data-stu-id="b68d2-181">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="b68d2-182">パートナーセンターの Webhook Api を使用すると、リソース変更イベントに登録できます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-182">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="b68d2-183">これらの変更イベントは、HTTP 投稿として url に送信されます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-183">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="b68d2-184">Url を登録するには、**パートナーセンターの Webhook 登録 (Insider Preview)** パワー自動化フローを選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-184">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="b68d2-185">接続の追加 (a.)参照管理者の資格情報を持つパートナーセンターのユーザー (b)次の強調表示されているパートナーセンターのイベント</span><span class="sxs-lookup"><span data-stu-id="b68d2-185">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="トリガー":::

3. <span data-ttu-id="b68d2-187">これらの更新を行うと、次のように表示されます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-187">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="b68d2-189">変更内容を保存し、[**有効にする**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-189">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="b68d2-190">パートナーセンターの webhook でイベントの変更をリッスンできるようにするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-190">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="b68d2-191">[**パートナーセンター] を**選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-191">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="b68d2-192">[**編集**] アイコンを選択し、[ **HTTP 要求の受信時**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-192">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="b68d2-193">**コピー**アイコンを選択して、指定された HTTP POST URL をコピーします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-193">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL のコピー":::

8. <span data-ttu-id="b68d2-195">次に、"パートナーセンターの Webhook の登録 (Insider Preview)" パワー自動化フローを選択し、[**実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-195">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="b68d2-196">右側のウィンドウで [実行フロー] ウィンドウが開いていることを確認し、[**続行**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-196">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="b68d2-197">次の詳細を入力します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-197">Enter the following details:</span></span>

    1. <span data-ttu-id="b68d2-198">**Http トリガーエンドポイント**: 前の手順からコピーされた URL</span><span class="sxs-lookup"><span data-stu-id="b68d2-198">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="b68d2-199">**登録するイベント**: "紹介-作成" と "参照-更新"</span><span class="sxs-lookup"><span data-stu-id="b68d2-199">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="b68d2-200">**既存のトリガーエンドポイントがある場合は上書き**します (存在する場合は既存のエンドポイントを上書きします)。</span><span class="sxs-lookup"><span data-stu-id="b68d2-200">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="b68d2-201">[**実行**] を選択し、[完了] を選択し**ます。**</span><span class="sxs-lookup"><span data-stu-id="b68d2-201">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="b68d2-202">Webhook は、イベントの作成と更新をリッスンできるようになりました。</span><span class="sxs-lookup"><span data-stu-id="b68d2-202">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="b68d2-203">同期手順のカスタマイズ</span><span class="sxs-lookup"><span data-stu-id="b68d2-203">Customize synchronization steps</span></span>

<span data-ttu-id="b68d2-204">パートナーセンターと CRM システムの間で共同販売参照が同期されると、パートナーセンター PC で同期されるフィールドがここに表示されます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-204">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="b68d2-205">多くの場合、CRM システムは高度にカスタマイズされています。</span><span class="sxs-lookup"><span data-stu-id="b68d2-205">Often CRM systems are highly customized.</span></span> <span data-ttu-id="b68d2-206">パワー自動化フローをカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-206">You can customize the Power Automate flows.</span></span> <span data-ttu-id="b68d2-207">フィールドマッピングガイドに従って、必要に応じて、パワー自動化フローの手順に適切な変更を加えます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-207">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="b68d2-208">Microsoft パートナーセンターから CRM へのマッピングが提供されますが、CRM 環境に基づいて、フィールドをさらにカスタマイズすることもできます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-208">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="b68d2-209">各パワー自動化フローの複数の手順は、ニーズに応じてカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-209">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="b68d2-210">使用可能なカスタマイズの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-210">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="b68d2-211">パートナーセンターで作成または更新イベントのフィールドを CRM の参照同期にカスタマイズするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-211">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="b68d2-212">[パートナーセンター] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-212">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="b68d2-213">[**編集**] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-213">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="b68d2-214">選択 **(スコープ) 潜在顧客または営業案件を同期**します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-214">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="b68d2-215">作成イベントの CRM フィールドマッピングをカスタマイズするには、[**新しい共有の営業案件]、[**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-215">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="b68d2-216">[**はい] の場合**はサブステップを選択し、 **CRM で [新しい営業案件の作成**] を展開します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-216">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="b68d2-217">このセクションでマッピングを編集するには、[フィールドマッピングガイド] を使用します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-217">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="b68d2-218">更新イベントの CRM フィールドマッピングをカスタマイズするには、[(スコープ) 潜在顧客または営業案件を同期する] ステップをクリックします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-218">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="b68d2-219">**営業案件の更新である場合は、** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-219">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="b68d2-220">[サブステップ**if yes]** を選択し、次に**パートナーセンターと CRM の営業案件オブジェクト間の差異がある場合**は、を展開します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-220">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="b68d2-221">**既存の営業案件を更新**する場合は、[**はい]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-221">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="b68d2-222">更新イベントの CRM から PC への参照同期のフィールドをカスタマイズするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-222">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="b68d2-223">[**編集**] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-223">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="b68d2-224">[ **(スコープ)] を選択して、営業案件を同期**します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-224">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="b68d2-225">更新イベントの CRM フィールドマッピング (フィールドマッピングガイドに基づく) をカスタマイズする場合は、**パートナーセンターと CRM の潜在顧客オブジェクトが異なるかどうか**を選択してから、を選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-225">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="b68d2-226">[**はい] の場合**はサブステップを選択し、[**営業案件データを使用して紹介を更新する**] ステップを展開します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-226">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="b68d2-227">このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-227">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="b68d2-228">Create events の CRM to PC 参照同期のフィールドをカスタマイズするには</span><span class="sxs-lookup"><span data-stu-id="b68d2-228">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="b68d2-229">[**編集**] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-229">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="b68d2-230">**参照の同期を選択 (スコープ) します。**</span><span class="sxs-lookup"><span data-stu-id="b68d2-230">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="b68d2-231">[イベントの作成] で (フィールドマッピングガイドに基づいて) CRM フィールドマッピングをカスタマイズする場合は、[ **Microsoft の紹介を作成する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-231">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="b68d2-232">このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-232">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a><span data-ttu-id="b68d2-233">Salesforce CRM 営業案件レイアウトで別のセクションを作成する</span><span class="sxs-lookup"><span data-stu-id="b68d2-233">Create Separate Section in Salesforce CRM Opportunity Layout</span></span>

<span data-ttu-id="b68d2-234">パートナーセンターと Salesforce CRM 間で推薦を同期するには、Power 区別のソリューションで、Microsoft 固有の紹介フィールドを明確にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b68d2-234">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="b68d2-235">これにより、販売者チームは、共同販売のために Microsoft と共有する参照を決定することができます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-235">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="b68d2-236">Salesforce CRM**営業案件**エンティティのパートナーセンターの紹介同期の一部として、一連のカスタムフィールドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-236">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM **Opportunity** entity.</span></span> <span data-ttu-id="b68d2-237">CRM 管理者ユーザーは、**営業案件**のカスタムフィールドを使用して、別の crm セクションを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b68d2-237">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>
<span data-ttu-id="b68d2-238">Salesforce CRM 管理者ユーザーは、別の CRM セクションを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b68d2-238">Salesforce CRM administrator user will need to create a separate CRM section.</span></span>

<span data-ttu-id="b68d2-239">次のカスタムフィールドは、CRM セクションの一部にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b68d2-239">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="b68d2-240">**パートナーセンターとの同期**: 営業案件を Microsoft パートナーセンターと同期するかどうか</span><span class="sxs-lookup"><span data-stu-id="b68d2-240">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="b68d2-241">**参照識別子**: Microsoft パートナーセンターの紹介の読み取り専用識別子フィールド</span><span class="sxs-lookup"><span data-stu-id="b68d2-241">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="b68d2-242">**紹介リンク**: Microsoft パートナーセンターでの紹介への読み取り専用リンク</span><span class="sxs-lookup"><span data-stu-id="b68d2-242">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="b68d2-243">**Microsoft ではどのように役立つでしょうか。**</span><span class="sxs-lookup"><span data-stu-id="b68d2-243">**How can Microsoft help?**</span></span> <span data-ttu-id="b68d2-244">紹介のために Microsoft が必要とするヘルプ</span><span class="sxs-lookup"><span data-stu-id="b68d2-244">Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="b68d2-245">**製品**: この営業案件に関連付けられている製品の一覧</span><span class="sxs-lookup"><span data-stu-id="b68d2-245">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="b68d2-246">**監査**: Microsoft パートナーセンターの紹介と同期するための読み取り専用の監査証跡</span><span class="sxs-lookup"><span data-stu-id="b68d2-246">**Audit**: A read only audit trail for syncing with Microsoft Partner Center referral</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="b68d2-247">フィールドとリレーションシップの設定</span><span class="sxs-lookup"><span data-stu-id="b68d2-247">Set up fields and relationships</span></span>

1. <span data-ttu-id="b68d2-248">Salesforce アカウントにサインインし、[**営業案件**] にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-248">Sign into your Salesforce account and go to **Opportunity**.</span></span>

2. <span data-ttu-id="b68d2-249">[**セットアップ**] および [**オブジェクトの編集**] オプションをクリックして、必要なフィールドを追加します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-249">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>

3. <span data-ttu-id="b68d2-250">左側のナビゲーションから [**フィールド & リレーションシップ**を選択する]</span><span class="sxs-lookup"><span data-stu-id="b68d2-250">Select **Fields & Relationships** from the left navigation</span></span>

   :::image type="content" source="images/salesforce/fields1.png" alt-text="Fields":::

4. <span data-ttu-id="b68d2-252">**フィールド & リレーションシップ**テーブルに次のフィールドを追加します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-252">Add the following fields in the **Fields & Relationship** table:</span></span>

   |<span data-ttu-id="b68d2-253">**フィールドラベル**</span><span class="sxs-lookup"><span data-stu-id="b68d2-253">**Field label**</span></span>   |<span data-ttu-id="b68d2-254">**フィールド名**</span><span class="sxs-lookup"><span data-stu-id="b68d2-254">**Field name**</span></span>|<span data-ttu-id="b68d2-255">**データの種類**</span><span class="sxs-lookup"><span data-stu-id="b68d2-255">**Data type**</span></span>|<span data-ttu-id="b68d2-256">**付ける**</span><span class="sxs-lookup"><span data-stu-id="b68d2-256">**Indexed**</span></span>|
   |---------------------|:-------------------|:--------------|:----------------|
   |<span data-ttu-id="b68d2-257">Audit</span><span class="sxs-lookup"><span data-stu-id="b68d2-257">Audit</span></span>| <span data-ttu-id="b68d2-258">Audit__c</span><span class="sxs-lookup"><span data-stu-id="b68d2-258">Audit__c</span></span>|<span data-ttu-id="b68d2-259">長いテキスト領域 (100000) (表示されている4行目)</span><span class="sxs-lookup"><span data-stu-id="b68d2-259">Long Text Area(100000)(visible line 4)</span></span>||
   |<span data-ttu-id="b68d2-260">Microsoft ではどのように役立つでしょうか。</span><span class="sxs-lookup"><span data-stu-id="b68d2-260">How can Microsoft help?</span></span>|<span data-ttu-id="b68d2-261">How_can_Microsoft_help_c</span><span class="sxs-lookup"><span data-stu-id="b68d2-261">How_can_Microsoft_help_c</span></span>|<span data-ttu-id="b68d2-262">ピック</span><span class="sxs-lookup"><span data-stu-id="b68d2-262">Picklist\*</span></span>|
   |<span data-ttu-id="b68d2-263">製品</span><span class="sxs-lookup"><span data-stu-id="b68d2-263">Products</span></span>|<span data-ttu-id="b68d2-264">Products_c</span><span class="sxs-lookup"><span data-stu-id="b68d2-264">Products_c</span></span>|<span data-ttu-id="b68d2-265">テキスト (255)</span><span class="sxs-lookup"><span data-stu-id="b68d2-265">text (255)</span></span>||
   |<span data-ttu-id="b68d2-266">Referral</span><span class="sxs-lookup"><span data-stu-id="b68d2-266">Referral</span></span> | <span data-ttu-id="b68d2-267">Referral_Identfier_c</span><span class="sxs-lookup"><span data-stu-id="b68d2-267">Referral_Identfier_c</span></span>|<span data-ttu-id="b68d2-268">テキスト (100) (外部 ID)</span><span class="sxs-lookup"><span data-stu-id="b68d2-268">Text(100)(External ID)</span></span>|<span data-ttu-id="b68d2-269">はい</span><span class="sxs-lookup"><span data-stu-id="b68d2-269">yes</span></span>|
   |<span data-ttu-id="b68d2-270">紹介リンク</span><span class="sxs-lookup"><span data-stu-id="b68d2-270">Referral Link</span></span>| <span data-ttu-id="b68d2-271">Referral_Link_c_</span><span class="sxs-lookup"><span data-stu-id="b68d2-271">Referral_Link_c_</span></span>|<span data-ttu-id="b68d2-272">URL (255)</span><span class="sxs-lookup"><span data-stu-id="b68d2-272">URL(255)</span></span>||
   |<span data-ttu-id="b68d2-273">パートナーセンターとの同期</span><span class="sxs-lookup"><span data-stu-id="b68d2-273">Sync with Partner Center</span></span>|<span data-ttu-id="b68d2-274">sync_with_partner_center_c</span><span class="sxs-lookup"><span data-stu-id="b68d2-274">sync_with_partner_center_c</span></span>|<span data-ttu-id="b68d2-275">Checkbox (既定値はオフ)</span><span class="sxs-lookup"><span data-stu-id="b68d2-275">Checkbox (default unchecked)</span></span>||

   <span data-ttu-id="b68d2-276">\* 候補リストの値:</span><span class="sxs-lookup"><span data-stu-id="b68d2-276">\*Picklist values:</span></span>

   - <span data-ttu-id="b68d2-277">ワークロード固有の価値提案</span><span class="sxs-lookup"><span data-stu-id="b68d2-277">Workload specific value proposition</span></span>
   - <span data-ttu-id="b68d2-278">お客様のテクニカルアーキテクチャ</span><span class="sxs-lookup"><span data-stu-id="b68d2-278">Customer technical architecture</span></span>
   - <span data-ttu-id="b68d2-279">概念実証またはデモ</span><span class="sxs-lookup"><span data-stu-id="b68d2-279">Proof of concept or demo</span></span>
   - <span data-ttu-id="b68d2-280">引用符またはライセンス</span><span class="sxs-lookup"><span data-stu-id="b68d2-280">Quotes or licensing</span></span>
   - <span data-ttu-id="b68d2-281">販売後の顧客の成功</span><span class="sxs-lookup"><span data-stu-id="b68d2-281">Post sales customer success</span></span>
   - <span data-ttu-id="b68d2-282">全般またはその他</span><span class="sxs-lookup"><span data-stu-id="b68d2-282">General or other</span></span>

5. <span data-ttu-id="b68d2-283">フィールドは、[**フィールド & リレーションシップ**] の下に作成されます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-283">The fields would get created under **Fields & Relationships**</span></span>

   :::image type="content" source="images/salesforce/fields2.png" alt-text="作成されたフィールド":::

6. <span data-ttu-id="b68d2-285">営業案件のレイアウトでは、上記のフィールドと同じセクションを作成します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-285">In the Opportunity layout, create a separate section with the fields as listed above.</span></span>

   - <span data-ttu-id="b68d2-286">このセクションは、営業案件のレイアウトで販売元に提供されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b68d2-286">This section should be available for the sellers in the Opportunity layout</span></span>

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="パートナーセンターのフィールドレイアウト":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="b68d2-288">エンドツーエンドの双方向の共同販売参照の同期</span><span class="sxs-lookup"><span data-stu-id="b68d2-288">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="b68d2-289">パワー自動化ソリューションをインストールし、構成し、カスタマイズしたら、Salesforce CRM とパートナーセンター間の共同販売参照の同期をテストできます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-289">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="b68d2-290">前提条件</span><span class="sxs-lookup"><span data-stu-id="b68d2-290">Pre-requisites</span></span>

<span data-ttu-id="b68d2-291">パートナーセンターと Salesforce CRM 間で推薦を同期するには、Power 区別のソリューションで、Microsoft 固有の紹介フィールドを明確にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b68d2-291">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="b68d2-292">この id により、販売者チームは、共同販売のために Microsoft と共有する参照を決定することができます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-292">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="b68d2-293">Salesforce CRM ソリューションの**営業案件**エンティティのパートナーセンターの紹介同期の一部として、一連のカスタムフィールドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-293">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="b68d2-294">CRM 管理者ユーザーは、**営業案件**のカスタムフィールドを使用して、別の crm セクションを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b68d2-294">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="b68d2-295">次のカスタムフィールドは、CRM セクションの一部にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b68d2-295">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="b68d2-296">**パートナーセンターとの同期**: 営業案件を Microsoft パートナーセンターと同期するかどうか</span><span class="sxs-lookup"><span data-stu-id="b68d2-296">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="b68d2-297">**参照識別子**: Microsoft パートナーセンターの紹介の読み取り専用識別子フィールド</span><span class="sxs-lookup"><span data-stu-id="b68d2-297">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="b68d2-298">**紹介リンク**: Microsoft パートナーセンターでの紹介への読み取り専用リンク</span><span class="sxs-lookup"><span data-stu-id="b68d2-298">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="b68d2-299">Microsoft**ヘルプ**を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b68d2-299">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="b68d2-300">**製品**: この営業案件に関連付けられている製品の一覧</span><span class="sxs-lookup"><span data-stu-id="b68d2-300">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="b68d2-301">**監査**: パートナーセンターの紹介と同期するための読み取り専用の監査証跡</span><span class="sxs-lookup"><span data-stu-id="b68d2-301">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="b68d2-302">モデル</span><span class="sxs-lookup"><span data-stu-id="b68d2-302">SCENARIOS:</span></span>

1. <span data-ttu-id="b68d2-303">CRM で参照が作成または更新され、パートナーセンターで同期される場合の参照の同期:</span><span class="sxs-lookup"><span data-stu-id="b68d2-303">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="b68d2-304">CRM の**営業案件**セクションで可視性を持つユーザーを使用して、Salesforce crm 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-304">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="b68d2-305">Salesforce CRM 環境で "新しい営業案件" を作成するときに、次のセクションが存在することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-305">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 環境":::

   3. <span data-ttu-id="b68d2-307">この機会を Microsoft パートナーセンターと同期するには、カードビューで次のフィールドを設定していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-307">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="b68d2-308">"パートナーセンターとの同期": はい</span><span class="sxs-lookup"><span data-stu-id="b68d2-308">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="b68d2-309">「Microsoft がどのように役立つか」: 次のオプションから選択してください。</span><span class="sxs-lookup"><span data-stu-id="b68d2-309">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="b68d2-310">製品: 製品のソリューション Id</span><span class="sxs-lookup"><span data-stu-id="b68d2-310">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="b68d2-311">[営業案件**とパートナーセンターの同期**] オプションを **[はい]** に設定したら、10分待ってから、パートナーセンターアカウントにサインインします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-311">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="b68d2-312">参照は、Salesforce CRM と同期されます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-312">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="b68d2-313">[パートナーセンターとの同期] オプションが [はい] に設定されている場合、Salesforce CRM で営業案件を更新すると、変更がパートナーセンターアカウントと同期されます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-313">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="b68d2-314">パートナーセンターで正常に同期された営業案件は、Salesforce CRM の✔アイコンで識別されます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-314">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="b68d2-315">Microsoft パートナーセンターで参照が作成または更新され、Salesforce CRM 環境で同期される場合の紹介の同期:</span><span class="sxs-lookup"><span data-stu-id="b68d2-315">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="b68d2-316">パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-316">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="b68d2-317">左側のメニューから [**紹介**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-317">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="b68d2-318">[新しい取引] オプションをクリックして、パートナーセンターから新しい共同販売紹介を作成します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-318">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="b68d2-319">Salesforce CRM 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="b68d2-319">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="b68d2-320">**[Open opportunity**] に移動します。</span><span class="sxs-lookup"><span data-stu-id="b68d2-320">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="b68d2-321">Microsoft パートナーセンターで作成された紹介が、Salesforce CRM で同期されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="b68d2-321">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce の営業案件画面":::

    6. <span data-ttu-id="b68d2-323">同期された参照を選択すると、カードビューの詳細が設定されます。</span><span class="sxs-lookup"><span data-stu-id="b68d2-323">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b68d2-324">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b68d2-324">Next steps</span></span>

- [<span data-ttu-id="b68d2-325">Microsoft Power の自動化プラットフォームの詳細</span><span class="sxs-lookup"><span data-stu-id="b68d2-325">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/-automate/)

- [<span data-ttu-id="b68d2-326">見込み客を管理する</span><span class="sxs-lookup"><span data-stu-id="b68d2-326">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="b68d2-327">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="b68d2-327">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="b68d2-328">パートナー センター Webhook</span><span class="sxs-lookup"><span data-stu-id="b68d2-328">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)