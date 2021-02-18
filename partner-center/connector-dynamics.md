---
title: Dynamics 365 CRM パートナーセンターの共同販売コネクタ
ms.topic: how-to
ms.date: 02/16/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターの紹介を Dynamics 365 CRM の共同販売コネクタと同期します。 販売元は、CRM システム内から Microsoft と共同で販売することができます。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: e465130b96886cf2bb77bcd94f56c1a12545a5d5
ms.sourcegitcommit: 64243caed029ffe40e2bbc369f4ee96f4f0ca26f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/18/2021
ms.locfileid: "100645770"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="d5618-104">Dynamics 365 CRM の共同販売コネクタ–概要</span><span class="sxs-lookup"><span data-stu-id="d5618-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="d5618-105">適切なロール</span><span class="sxs-lookup"><span data-stu-id="d5618-105">Appropriate roles</span></span>

- <span data-ttu-id="d5618-106">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="d5618-106">Referrals admin</span></span>
- <span data-ttu-id="d5618-107">CRM のシステム管理者またはシステムカスタマイザー</span><span class="sxs-lookup"><span data-stu-id="d5618-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="d5618-108">パートナーセンターの共同販売コネクタを使用すると、販売元は CRM システム内から Microsoft と共同で販売することができます。</span><span class="sxs-lookup"><span data-stu-id="d5618-108">Partner Center Co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="d5618-109">パートナーセンターを使用して共同販売取引を管理するためのトレーニングを行う必要はありません。</span><span class="sxs-lookup"><span data-stu-id="d5618-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="d5618-110">共同販売コネクタを使用して、Microsoft 販売者に連絡するための新しい共同販売参照を作成したり、Microsoft 販売者からの推薦を受け取ったり、紹介を受け入れたり拒否したり、商談の価値や終了日などの取引データを変更したりします。</span><span class="sxs-lookup"><span data-stu-id="d5618-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="d5618-111">また、これらの共同販売取引に関するマイクロソフト販売者からの更新を受け取ることもできます。</span><span class="sxs-lookup"><span data-stu-id="d5618-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="d5618-112">パートナーセンターではなく、選択した CRM ですべての紹介作業を管理できます。</span><span class="sxs-lookup"><span data-stu-id="d5618-112">You can manage all of your referrals work in the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="d5618-113">このソリューションは、Microsoft のパワー自動化ソリューションに基づいており、パートナーセンター Api を使用しています。</span><span class="sxs-lookup"><span data-stu-id="d5618-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="d5618-114">をインストールする前に-前提条件</span><span class="sxs-lookup"><span data-stu-id="d5618-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="d5618-115">**トピック**</span><span class="sxs-lookup"><span data-stu-id="d5618-115">**Topics**</span></span>   |<span data-ttu-id="d5618-116">**詳細**</span><span class="sxs-lookup"><span data-stu-id="d5618-116">**Details**</span></span>   |<span data-ttu-id="d5618-117">**リンク**</span><span class="sxs-lookup"><span data-stu-id="d5618-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="d5618-118">Microsoft Partner Network ID</span><span class="sxs-lookup"><span data-stu-id="d5618-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="d5618-119">有効な MPN ID が必要です</span><span class="sxs-lookup"><span data-stu-id="d5618-119">You need a valid MPN ID</span></span>|<span data-ttu-id="d5618-120">[MPN](https://partner.microsoft.com/)に参加するには</span><span class="sxs-lookup"><span data-stu-id="d5618-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="d5618-121">共同販売の準備完了</span><span class="sxs-lookup"><span data-stu-id="d5618-121">Cosell ready</span></span>|<span data-ttu-id="d5618-122">お客様の IP/サービスソリューションは、共同販売の準備ができている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5618-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="d5618-123">Microsoft との販売</span><span class="sxs-lookup"><span data-stu-id="d5618-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="d5618-124">パートナー センター アカウント</span><span class="sxs-lookup"><span data-stu-id="d5618-124">Partner Center account</span></span>|<span data-ttu-id="d5618-125">パートナーセンターのテナントに関連付けられている MPN ID は、共同販売ソリューションに関連付けられている MPN ID と同じである必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5618-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="d5618-126">コネクタをデプロイする前に、パートナーセンターポータルで共同販売の紹介を確認できることを確認します。</span><span class="sxs-lookup"><span data-stu-id="d5618-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="d5618-127">アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="d5618-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="d5618-128">パートナー センターのユーザー ロール</span><span class="sxs-lookup"><span data-stu-id="d5618-128">Partner Center user roles</span></span>|<span data-ttu-id="d5618-129">コネクタをインストールして使用する従業員は、参照管理者である必要があります</span><span class="sxs-lookup"><span data-stu-id="d5618-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="d5618-130">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="d5618-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| 
|<span data-ttu-id="d5618-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="d5618-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="d5618-132">CRM ユーザーロールは、システム管理者またはシステムカスタマイザーです。</span><span class="sxs-lookup"><span data-stu-id="d5618-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="d5618-133">Dynamics 365 でロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="d5618-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="d5618-134">パワー自動化フローアカウント</span><span class="sxs-lookup"><span data-stu-id="d5618-134">Power Automate Flow Account</span></span>|<span data-ttu-id="d5618-135">テスト/ステージングおよび運用のためにデータベースを使用して、新しい運用環境を作成します。</span><span class="sxs-lookup"><span data-stu-id="d5618-135">Create new production environment with database for test/staging and production.</span></span> <span data-ttu-id="d5618-136">データベースが存在する既存の運用環境がある場合は、再利用できます。</span><span class="sxs-lookup"><span data-stu-id="d5618-136">If you have an existing production environment with database it can be re-used.</span></span> <span data-ttu-id="d5618-137">コネクタソリューションをインストールするユーザーは、電源を自動で使用し、この環境にアクセスする必要があります。進行状況を監視し、[ソリューション] の [履歴の表示] をクリックすると、インストールが [Power の自動化](https://flow.microsoft.com/) に失敗することを確認できます。</span><span class="sxs-lookup"><span data-stu-id="d5618-137">User who is going to install connector solution needs to have Power Automate license and access to this environment.You can monitor the progress and get more details should the installation fail in [Power Automate](https://flow.microsoft.com/) by clicking See history under Solutions.</span></span>|[<span data-ttu-id="d5618-138">環境の作成または管理</span><span class="sxs-lookup"><span data-stu-id="d5618-138">Create or manage environment</span></span>](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="d5618-139">Dynamics 365 のパートナーセンターの紹介同期をインストールする (電源自動化ソリューション)</span><span class="sxs-lookup"><span data-stu-id="d5618-139">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="d5618-140">[ [パワー自動化](https://flow.microsoft.com) ] にアクセスし、右上隅にある [ **環境** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-140">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="d5618-141">この手順では、使用可能な CRM インスタンスを表示します。</span><span class="sxs-lookup"><span data-stu-id="d5618-141">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="d5618-142">右上隅にあるドロップダウンから適切な CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-142">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="d5618-143">左側のナビゲーションバーで [ **ソリューション** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-143">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="d5618-144">上部のメニューの [ **AppSource を開く** ] リンクをクリックします。</span><span class="sxs-lookup"><span data-stu-id="d5618-144">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource を開く":::

5. <span data-ttu-id="d5618-146">ポップアップ画面で、 **Dynamics365 のパートナーセンターの紹介コネクタ** を検索します。</span><span class="sxs-lookup"><span data-stu-id="d5618-146">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="d5618-147">[ **今すぐ入手** する] ボタンをクリックし、[ **続行**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d5618-147">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="d5618-148">これにより、CRM (Dynamics 365) 環境を選択してアプリケーションをインストールできるページが開きます。</span><span class="sxs-lookup"><span data-stu-id="d5618-148">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="d5618-149">使用条件に同意します。</span><span class="sxs-lookup"><span data-stu-id="d5618-149">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="d5618-150">進行状況を監視し、[**ソリューション**] の [**履歴の表示**] をクリックすると、インストールが Power の自動化に失敗することを確認できます。</span><span class="sxs-lookup"><span data-stu-id="d5618-150">You can monitor the progress and get more details should the installation fail in Power Automate by clicking **See history** under **Solutions**.</span></span>
 

9. <span data-ttu-id="d5618-151">インストールが完了したら、[Power の [自動化](https://flow.microsoft.com) ] に戻り、左側のナビゲーション領域から [ **ソリューション** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-151">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="d5618-152">**Dynamics 365 のパートナーセンターの紹介同期** は、[ソリューション] の一覧で確認できます。</span><span class="sxs-lookup"><span data-stu-id="d5618-152">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="d5618-153">**Dynamics 365 のパートナーセンターの紹介同期** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-153">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="d5618-154">次の電源の自動化フローとエンティティを利用できます。</span><span class="sxs-lookup"><span data-stu-id="d5618-154">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="使用可能な CRMS":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="d5618-156">ベストプラクティス: 運用前にテストする</span><span class="sxs-lookup"><span data-stu-id="d5618-156">Best practice: test before you go live</span></span>

<span data-ttu-id="d5618-157">運用環境でパワー自動化ソリューションをインストール、構成、およびカスタマイズする前に、必ずステージング CRM インスタンスでソリューションをテストしてください。</span><span class="sxs-lookup"><span data-stu-id="d5618-157">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="d5618-158">ステージング環境/CRM インスタンスに Microsoft Power 自動ソリューションをインストールします。</span><span class="sxs-lookup"><span data-stu-id="d5618-158">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="d5618-159">ステージング環境で Microsoft パワー自動化ソリューションを構成し、カスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="d5618-159">Configure and customize the Microsoft Power Automate solution in staging environment.</span></span>
- <span data-ttu-id="d5618-160">ステージング/CRM インスタンスでソリューションをテストします。</span><span class="sxs-lookup"><span data-stu-id="d5618-160">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="d5618-161">成功した場合は、運用インスタンスにマネージドソリューションとしてインポートします。</span><span class="sxs-lookup"><span data-stu-id="d5618-161">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="d5618-162">ソリューションの構成</span><span class="sxs-lookup"><span data-stu-id="d5618-162">Configure the solution</span></span>

1. <span data-ttu-id="d5618-163">CRM インスタンスにソリューションをインストールしたら、[ [Power の自動化](https://flow.microsoft.com/)] に戻ります。</span><span class="sxs-lookup"><span data-stu-id="d5618-163">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="d5618-164">右上隅にある [ **環境** ] ドロップダウンで、パワー自動化ソリューションをインストールした CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-164">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="d5618-165">次の3つのユーザーアカウントを関連付ける接続を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5618-165">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="d5618-166">参照管理者の資格情報を持つパートナーセンターのユーザー</span><span class="sxs-lookup"><span data-stu-id="d5618-166">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="d5618-167">パートナー センターのイベント</span><span class="sxs-lookup"><span data-stu-id="d5618-167">Partner Center Events</span></span>

   - <span data-ttu-id="d5618-168">Power を使用した CRM 管理ソリューションのフローが自動化されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-168">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="d5618-169">左側のナビゲーションバーから [ **接続** ] を選択し、一覧から "パートナーセンターの紹介" ソリューションを選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="d5618-170">[ **接続の作成**] をクリックして接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="d5618-170">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="接続を作成する":::

      3. <span data-ttu-id="d5618-172">右上隅の検索バーで、 **パートナーセンターの参照 (プレビュー)** を検索します。</span><span class="sxs-lookup"><span data-stu-id="d5618-172">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="d5618-173">参照管理者の資格情報ロールを使用して、パートナーセンターユーザーの接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="d5618-173">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="d5618-174">次に、パートナーセンターのユーザーに、参照管理者の資格情報を使用してパートナーセンターのイベント接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="d5618-174">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="d5618-175">CRM 管理者ユーザーの Common Data Service (現在の環境) の接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="d5618-175">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
     
      7. <span data-ttu-id="d5618-176">すべての接続を追加すると、環境内に次の接続が表示されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-176">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="接続":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="d5618-178">接続を編集する</span><span class="sxs-lookup"><span data-stu-id="d5618-178">Edit the connections</span></span>

1. <span data-ttu-id="d5618-179">[ **ソリューション** ] ページに戻り、[ **既定のソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-179">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="d5618-180">[**すべて**] をクリックして、[**接続の参照 (プレビュー)** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-180">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics-3.png" alt-text="接続する":::

2. <span data-ttu-id="d5618-182">3つのドットアイコンを選択して、各接続を1つずつ編集します。</span><span class="sxs-lookup"><span data-stu-id="d5618-182">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="d5618-183">関連する接続を追加します。</span><span class="sxs-lookup"><span data-stu-id="d5618-183">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="一覧表示された接続"::: 

3.  <span data-ttu-id="d5618-185">[ソリューション] ページに戻り、Dynamics 365 のパートナーセンター紹介同期を選択し、次のシーケンスの各フローの横にある3つのドットアイコンをクリックしてフローをオンにします。</span><span class="sxs-lookup"><span data-stu-id="d5618-185">Return to the Solutions page, select Partner Center Referrals Synchronization for Dynamics 365 and turn on the flow by clicking on three dots icon next to each flow in the following sequence.</span></span> <span data-ttu-id="d5618-186">フローをオンにしている間に問題が発生した場合は、 [カスタマイズの手順](connector-dynamics.md#customize-synchronization-steps) と [トラブルシューティングの手順](connectors-troubleshoot.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5618-186">If you encounter any issues while turning on the flow refer to [customization steps](connector-dynamics.md#customize-synchronization-steps) and [troubleshooting steps](connectors-troubleshoot.md).</span></span> 

<span data-ttu-id="d5618-187">次の順序でフローを有効にします。</span><span class="sxs-lookup"><span data-stu-id="d5618-187">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="d5618-188">パートナーセンターの Webhook の登録 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d5618-188">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="d5618-189">パートナーセンターへの共同販売紹介– Dynamics 365 の作成 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d5618-189">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="d5618-190">カスタマイズDynamics 365 フローから詳細を作成または取得します。</span><span class="sxs-lookup"><span data-stu-id="d5618-190">[Customize] Create or Get Details from Dynamics 365 flow</span></span> 
- <span data-ttu-id="d5618-191">パートナーセンターから Dynamics 365-ヘルパー (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d5618-191">Partner Center to Dynamics 365 - Helper (Insider Preview)</span></span>
- <span data-ttu-id="d5618-192">パートナーセンターの Microsoft 共同販売参照の更新 Dynamics 365 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d5618-192">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="d5618-193">パートナーセンターから Dynamics 365 へ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d5618-193">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="d5618-194">Dynamics 365 からパートナーセンターへ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d5618-194">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="d5618-195">Dynamics 365 営業案件パートナーセンター (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d5618-195">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="d5618-196">Dynamics 365 Microsoft ソリューション (パートナーセンター) (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d5618-196">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="d5618-197">Webhook Api を使用してリソース変更イベントに登録する</span><span class="sxs-lookup"><span data-stu-id="d5618-197">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="d5618-198">パートナーセンターの Webhook Api を使用すると、リソース変更イベントに登録できます。</span><span class="sxs-lookup"><span data-stu-id="d5618-198">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="d5618-199">これらの変更イベントは、HTTP 投稿として url に送信されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-199">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="d5618-200">[ **パートナーセンター] を Dynamics 365 (Insider Preview) に** 選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-200">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

2. <span data-ttu-id="d5618-201">[ **編集** ] アイコンを選択し、[ **HTTP 要求の受信時**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-201">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

3. <span data-ttu-id="d5618-202">**コピー** アイコンを選択して、指定された HTTP POST URL をコピーします。</span><span class="sxs-lookup"><span data-stu-id="d5618-202">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="URL のコピー":::

4. <span data-ttu-id="d5618-204">次に、"パートナーセンターの Webhook の登録 (Insider Preview)" パワー自動化フローを選択し、[ **実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-204">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

5. <span data-ttu-id="d5618-205">右側のウィンドウで [実行フロー] ウィンドウが開いていることを確認し、[ **続行**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d5618-205">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

6. <span data-ttu-id="d5618-206">次の詳細を入力します。</span><span class="sxs-lookup"><span data-stu-id="d5618-206">Enter the following details:</span></span>

   - <span data-ttu-id="d5618-207">**Http トリガーエンドポイント**: 前の手順からコピーされた URL</span><span class="sxs-lookup"><span data-stu-id="d5618-207">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

   - <span data-ttu-id="d5618-208">**登録するイベント**: 使用可能なすべてのイベントを選択します ("紹介-作成済み"、"紹介-更新済み"、"関連付けられている紹介-作成"、"関連付けられた参照-更新")。</span><span class="sxs-lookup"><span data-stu-id="d5618-208">**Events to Register**: Select all available events (“referral-created”, “referral-updated”, “related-referral-created”, “related-referral-updated”)</span></span>

   <span data-ttu-id="d5618-209">-**既存のトリガーエンドポイントが存在する場合は上書き** する: はい、特定の webhook イベントに登録できるのは1つの URL のみであることに注意することが重要です。</span><span class="sxs-lookup"><span data-stu-id="d5618-209">-**Overwrite existing trigger endpoints if present**: Yes It is important to note that only one URL can be registered for a given webhook event.</span></span> <span data-ttu-id="d5618-210">特定の webhook イベントに登録できる URL は1つだけであることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="d5618-210">It is important to note that only one URL can be registered for a given webhook event.</span></span> 

7. <span data-ttu-id="d5618-211">[ **実行** ] を選択し、[完了] を選択し **ます。**</span><span class="sxs-lookup"><span data-stu-id="d5618-211">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="d5618-212">Webhook は、イベントの作成と更新をリッスンできるようになりました。</span><span class="sxs-lookup"><span data-stu-id="d5618-212">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="d5618-213">同期手順のカスタマイズ</span><span class="sxs-lookup"><span data-stu-id="d5618-213">Customize synchronization steps</span></span>

<span data-ttu-id="d5618-214">CRM システムは高度にカスタマイズされており、CRM のセットアップに基づいて、パワー自動化ソリューションをカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="d5618-214">CRM systems are highly customized, and you can customize the Power Automate solution based on your CRM setup.</span></span>  <span data-ttu-id="d5618-215">パートナーセンターと CRM システムの間で共同販売参照が同期されると、パートナーセンター PC で同期されるフィールドが、 [カスタムフィールドマッピングガイド](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)に一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-215">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed in the [Custom field mapping guide](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).</span></span>

<span data-ttu-id="d5618-216">フィールドマッピングガイドに従って、必要に応じて、Dynamics 365 フローまたは環境変数 **の [カスタマイズ]**  で、適切な変更を行います。</span><span class="sxs-lookup"><span data-stu-id="d5618-216">Follow the field mapping guide, and if necessary, make appropriate changes in **[Customize] Create or Get Details from Dynamics 365 flow**  or environment variables.</span></span> <span data-ttu-id="d5618-217">今後のソリューションのアップグレードに影響する可能性があるため、Power オートメーションソリューションの他のフローを更新しないことをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="d5618-217">It is recommended not to update any other flows in Power Automate solution as it can impact future solution upgrades.</span></span> 

<span data-ttu-id="d5618-218">使用できるカスタマイズは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="d5618-218">The following are the available customizations:</span></span>

- <span data-ttu-id="d5618-219">[営業案件名のチェックマーク]: 既定では、パートナーセンターと Dynamics 365 CRM の間の同期が正常に行われていることを示すために、[営業案件名] の横にチェックマークが表示されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-219">Check mark in Opportunity name: By default, a check mark will be displayed next to Opportunity name to indicate that synchronization between Partner Center and Dynamics 365 CRM is happening successfully.</span></span> <span data-ttu-id="d5618-220">同様に、同期に失敗した場合は、クロスマークが表示されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-220">Similarly, a cross mark will be displayed if synchronization fails.</span></span> <span data-ttu-id="d5618-221">営業案件名に check マークまたは十字マークが追加されないようにするには、営業案件名環境変数の [表示] チェックマークの現在の値を [いいえ] に設定します。</span><span class="sxs-lookup"><span data-stu-id="d5618-221">To avoid adding check or cross mark in Opportunity name, set the current value of Display check mark in opportunity name environment variable to No.</span></span>

- <span data-ttu-id="d5618-222">取引値: 既定では、パートナーセンターからの取引値は CRM の **estimatedvalue** との間で同期されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-222">Deal value: By default, deal value from Partner Center will be synced to and from **estimatedvalue** in CRM.</span></span> <span data-ttu-id="d5618-223">CRM で、同期の対象となるフィールドが異なる場合は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="d5618-223">If you have a different field in CRM for deal value to sync from:</span></span>

    <span data-ttu-id="d5618-224">a.</span><span class="sxs-lookup"><span data-stu-id="d5618-224">a.</span></span>    <span data-ttu-id="d5618-225">CRM のフィールド名を使用して、Dynamics 365 環境変数の商談値フィールド名を更新します。</span><span class="sxs-lookup"><span data-stu-id="d5618-225">Update Deal value field name in Dynamics 365 environment variable with the CRM’s field name.</span></span> <span data-ttu-id="d5618-226">表示名ではなく、フィールドの名前を指定する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="d5618-226">Note that you should provide the field’s name not its display name.</span></span>

    <span data-ttu-id="d5618-227">b.</span><span class="sxs-lookup"><span data-stu-id="d5618-227">b.</span></span>    <span data-ttu-id="d5618-228">編集 **[カスタマイズ] Dynamics 365 flow から詳細を作成または取得**  し、crm での営業案件の **作成または更新** に関する情報を参照して、 **新しい営業案件** を作成し、 **既存の営業** 案件のアクションを更新して crm の正しいフィールドに **DealValue** 値を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="d5618-228">Edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to **Create or update** opportunity in CRM and update **Create a new opportunity** and **Update existing opportunity** actions to assign **DealValue** value to correct field in CRM.</span></span> <span data-ttu-id="d5618-229">また、[**推定収益**] フィールドから **DealValue assignment** を削除します。</span><span class="sxs-lookup"><span data-stu-id="d5618-229">Also, remove **DealValue assignment** from **Estimated Revenue** field.</span></span>

- <span data-ttu-id="d5618-230">顧客アカウントの国コード: 新しい紹介を作成するときに、2文字の国コード (ISO 3166) を指定することが必須です。</span><span class="sxs-lookup"><span data-stu-id="d5618-230">Customer Account Country Code: It is mandatory to provide a two-letter country code (ISO 3166) when creating a new referral.</span></span> <span data-ttu-id="d5618-231">既定では、国コードは CRM のアカウントの address1_country フィールドと同期されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-231">By default, country code will be synced to and from Account’s address1_country field in CRM.</span></span> <span data-ttu-id="d5618-232">国コードの同期元として CRM に別のフィールドがある場合は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="d5618-232">If you have a different field in CRM for country code to sync from:</span></span>

   <span data-ttu-id="d5618-233">a.</span><span class="sxs-lookup"><span data-stu-id="d5618-233">a.</span></span>    <span data-ttu-id="d5618-234">2文字のコードを含む Account の非ルックアップ国コードフィールドの場合:</span><span class="sxs-lookup"><span data-stu-id="d5618-234">For a non-lookup country code field in Account which contains two-letter code:</span></span>

   - <span data-ttu-id="d5618-235">Dynamics 365 環境変数の顧客アカウントの国コードフィールド名を CRM のフィールド名に更新します。</span><span class="sxs-lookup"><span data-stu-id="d5618-235">Update Customer account country code field name in Dynamics 365 environment variable with the CRM’s field name.</span></span> <span data-ttu-id="d5618-236">表示名ではなく、フィールドの名前を指定する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="d5618-236">Note that you should provide the field’s name not its display name.</span></span>

   - <span data-ttu-id="d5618-237">Edit **[カスタマイズ] Dynamics 365 flow から詳細を作成または取得**  し、crm の [顧客アカウントの作成または取得] 操作に移動して、crm の適切なフィールドに Country 値を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="d5618-237">Edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to Create or get customer account in CRM action to assign Country value to correct field in CRM.</span></span> <span data-ttu-id="d5618-238">また、[住所 1: 国/地域] フィールドから Country 値の割り当てを削除します。</span><span class="sxs-lookup"><span data-stu-id="d5618-238">Also, remove Country value assignment from Address 1: Country/Region field.</span></span>

   <span data-ttu-id="d5618-239">b.</span><span class="sxs-lookup"><span data-stu-id="d5618-239">b.</span></span>    <span data-ttu-id="d5618-240">アカウントの検索ベースの国コードフィールドの場合:</span><span class="sxs-lookup"><span data-stu-id="d5618-240">For a lookup-based country code field in Account:</span></span>

   - <span data-ttu-id="d5618-241">Account に新しいカスタムフィールドを追加し、[参照ベースのフィールド] で選択した値に基づいて、2文字の国コード (ISO 3166) を自動入力します。その逆も同様です。</span><span class="sxs-lookup"><span data-stu-id="d5618-241">Add a new custom field in Account and auto-populate it with two-letter country code (ISO 3166) based on the value selected in lookup-based field and vice-versa.</span></span>

   - <span data-ttu-id="d5618-242">上記の手順に従って、新しいカスタムフィールドを CRM とパートナーセンターの間で同期します。</span><span class="sxs-lookup"><span data-stu-id="d5618-242">Follow the steps above for non-lookup country code field to sync new custom field from CRM to and from Partner Center.</span></span>

- <span data-ttu-id="d5618-243">営業案件のフィールド: データを設定する必要がある営業案件の必須フィールドがある場合、 **Dynamics 365 フローから詳細を作成または取得**  し、CRM および update での **営業案件の作成または更新** に移動する **新しい営業案件のアクションを作成** して、ビジネス要件に基づいて必須フィールドに値を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="d5618-243">Opportunity fields: If there are mandatory fields in Opportunity that needs to be populated edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to **Create or update opportunity** in CRM and update **Create a new opportunity action** to assign values to the mandatory fields based on your business requirements.</span></span>

- <span data-ttu-id="d5618-244">潜在顧客のフィールド: リーダーに必須フィールドがあり、それを設定する必要がある場合は、 **Dynamics 365 フローから詳細を作成または取得**  し、CRM で [ **潜在顧客の作成または更新** ] に移動して、[更新] ビジネス要件に基づいて必須フィールドに値を割り当てる **新しい潜在顧客アクションを作成** します。</span><span class="sxs-lookup"><span data-stu-id="d5618-244">Lead fields: If there are mandatory fields in Lead that needs to be populated edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to **Create or update lead** in CRM and update **Create a new lead action** to assign values to the mandatory fields based on your business requirements.</span></span>

- <span data-ttu-id="d5618-245">顧客アカウント: 新しい紹介がパートナーセンターから CRM に同期されると、Power solution ソリューションでは、顧客の会社名と郵便番号を使用して CRM の既存のアカウントを検索しようとします。</span><span class="sxs-lookup"><span data-stu-id="d5618-245">Customer Account: When a new referral is synced from Partner Center to CRM, Power Automate solution tries to search for an existing account in CRM using customer company name and postal code.</span></span> <span data-ttu-id="d5618-246">見つからない場合は、新しい顧客アカウントが CRM で作成されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-246">If it does not find one, a new customer account will be created in CRM.</span></span> <span data-ttu-id="d5618-247">検索条件と新しいアカウント作成の詳細を更新するには、[カスタマイズ] を編集して **Dynamics 365 フローから詳細を作成または取得** し、CRM での **顧客アカウントの作成または取得** 、および **顧客アカウントの作成アクション** に移動します。</span><span class="sxs-lookup"><span data-stu-id="d5618-247">To update the search criteria and new account creation details, edit **[Customize] Create or Get Details from Dynamics 365 flow** and navigate to **Create or get customer account** in CRM and **Create customer account action**.</span></span>

## <a name="update-environment-variable"></a><span data-ttu-id="d5618-248">環境変数の更新</span><span class="sxs-lookup"><span data-stu-id="d5618-248">Update environment variable</span></span>

<span data-ttu-id="d5618-249">環境変数の値を更新するには:</span><span class="sxs-lookup"><span data-stu-id="d5618-249">To update an environment variable value:</span></span>

1. <span data-ttu-id="d5618-250">[ **ソリューション** ] ページにアクセスし、[ **既定のソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-250">Go to **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="d5618-251">[すべて] をクリックして **環境変数** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-251">Select **Environment Variable** by clicking All.</span></span>

2. <span data-ttu-id="d5618-252">更新する必要がある値の環境変数を選択し、3つのドットアイコンを使用して [ **編集** ] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d5618-252">Select the environment variable for the value that needs to be updated and click **Edit** using three dots icon.</span></span>

3. <span data-ttu-id="d5618-253">**新しい** 値オプションを使用して **現在の値** を更新し (既定値を更新しないでください)、値を指定します。</span><span class="sxs-lookup"><span data-stu-id="d5618-253">Update **Current Value** (do not update Default Value) using **New value** option and provide the value.</span></span> <span data-ttu-id="d5618-254">値は、変数のデータ型と一致する必要があります。たとえば、Yes/No データ型では Yes または No 値が許可されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-254">Value must match the Data type of the variable for e.g. Yes/No data type will accept either Yes or No value.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics-5.png" alt-text="既定値のエディットボックス":::

- <span data-ttu-id="d5618-256">エンドツーエンドの双方向の共同販売参照の同期</span><span class="sxs-lookup"><span data-stu-id="d5618-256">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="d5618-257">パワー自動化ソリューションをインストールし、構成し、カスタマイズしたら、Dynamics 365 とパートナーセンター間の共同販売参照の同期をテストできます。</span><span class="sxs-lookup"><span data-stu-id="d5618-257">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="d5618-258">前提条件</span><span class="sxs-lookup"><span data-stu-id="d5618-258">Pre-requisites</span></span>

<span data-ttu-id="d5618-259">パートナーセンターと Dynamics 365 CRM 間で紹介を同期するために、Power 区分ソリューションでは、Microsoft 固有の紹介フィールドが明確に示されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-259">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="d5618-260">この id により、販売者チームは、共同販売のために Microsoft と共有する参照を決定することができます。</span><span class="sxs-lookup"><span data-stu-id="d5618-260">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="d5618-261">カスタムフィールドとオブジェクトのセットが、ソリューションのインストールの一部として追加されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-261">A set of custom fields and objects will get added as part of the solution installation.</span></span> <span data-ttu-id="d5618-262">CRM 管理者ユーザーは、 **営業案件** のカスタムフィールドを使用して、別の crm セクションを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5618-262">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="d5618-263">次のカスタムフィールドは、CRM セクションの一部にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5618-263">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="d5618-264">**パートナーセンターとの同期**: 営業案件を Microsoft パートナーセンターと同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d5618-264">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center.</span></span> <span data-ttu-id="d5618-265">既定では、このフィールドの値は [いいえ] であり、Microsoft との営業案件を共有するには、販売者によって明示的に [はい] に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5618-265">By default, the value of this field is No and needs to be explicitly set to Yes by your seller to share an opportunity with Microsoft.</span></span> <span data-ttu-id="d5618-266">パートナーセンターから CRM に共有されている新しい紹介では、このフィールドの値が [はい] に設定されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-266">New referrals shared from Partner Center to CRM will have this field value set to Yes.</span></span>

- <span data-ttu-id="d5618-267">**参照識別子**: Microsoft パートナーセンターの紹介の読み取り専用識別子フィールド</span><span class="sxs-lookup"><span data-stu-id="d5618-267">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="d5618-268">**紹介リンク**: Microsoft パートナーセンターでの紹介への読み取り専用リンク</span><span class="sxs-lookup"><span data-stu-id="d5618-268">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>
- <span data-ttu-id="d5618-269">Microsoft の **ヘルプ** を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5618-269">**How can Microsoft help?**: Help required from Microsoft for the referral.</span></span> <span data-ttu-id="d5618-270">共同販売の紹介を作成するには、Microsoft からの適切なヘルプを選択してください。</span><span class="sxs-lookup"><span data-stu-id="d5618-270">To create a co-sell referral, select appropriate help required from Microsoft.</span></span> <span data-ttu-id="d5618-271">顧客の連絡先は、共同販売の紹介を作成する機会に関連付けられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5618-271">A customer contact must be associated to the Opportunity to create a co-sell referral.</span></span> <span data-ttu-id="d5618-272">共同販売以外の参照を作成するには、このフィールドの選択を解除します。</span><span class="sxs-lookup"><span data-stu-id="d5618-272">To create a non co-sell referral leave this field un-selected.</span></span> <span data-ttu-id="d5618-273">[適切なヘルプが必要] オプションを選択すると、非共同販売の推薦を、いつでも共同販売の紹介に変換できます。</span><span class="sxs-lookup"><span data-stu-id="d5618-273">A non co-sell referral can be converted to a co-sell referral anytime by selecting appropriate help required option.</span></span>

- <span data-ttu-id="d5618-274">**Microsoft パートナーセンターの参照の可視性**: Microsoft パートナーセンターの紹介の可視性を選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-274">**Microsoft Partner Center Referral Visibility**: Select visibility for Microsoft Partner Center Referral.</span></span> <span data-ttu-id="d5618-275">Microsoft の販売元に見えるようにすることで、共同販売以外の参照が共同販売に変換される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d5618-275">By making it visible to Microsoft sellers, a non co-sell referral may get converted to co-sell.</span></span> <span data-ttu-id="d5618-276">Microsoft ヘルプが必要な場合、既定では、Microsoft の販売者に参照が表示されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-276">When Microsoft help is required, referral is visible to Microsoft sellers by default.</span></span> <span data-ttu-id="d5618-277">参照可能としてマークすると、このフィールドを元に戻すことはできません。</span><span class="sxs-lookup"><span data-stu-id="d5618-277">Once marked as visible this field cannot be reverted.</span></span>

- <span data-ttu-id="d5618-278">**MICROSOFT CRM 識別子**: 共同販売の紹介が microsoft によって作成され、承認されると、このフィールドには MICROSOFT の CRM 識別子が表示されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-278">**Microsoft CRM Identifier**: When a co-sell referral is created and accepted by Microsoft, this field will get populated with Microsoft’s CRM identifier.</span></span>

- <span data-ttu-id="d5618-279">**製品: 廃止** : このフィールドを使用したり、CRM セクションに追加したりしないでください。旧バージョンとの互換性のためにのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="d5618-279">**Products: Obsolete** – do not use this field or add it to CRM section, it is available for backward compatibility only.</span></span> <span data-ttu-id="d5618-280">代わりに Microsoft Partner Center ソリューションを使用してください。</span><span class="sxs-lookup"><span data-stu-id="d5618-280">Use Microsoft Partner Center Solutions instead.</span></span>

- <span data-ttu-id="d5618-281">**監査**: パートナーセンターの紹介と同期するための読み取り専用の監査証跡</span><span class="sxs-lookup"><span data-stu-id="d5618-281">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

- <span data-ttu-id="d5618-282">**Microsoft パートナーセンターソリューション**: 共同販売の準備ができたソリューションまたは microsoft ソリューションを営業案件と関連付けるためのカスタムオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d5618-282">**Microsoft Partner Center Solutions**: A custom object to associate Co-sell ready solutions or Microsoft solutions with the opportunity.</span></span> <span data-ttu-id="d5618-283">営業案件から1つまたは複数のソリューションを追加または削除できます。</span><span class="sxs-lookup"><span data-stu-id="d5618-283">One or more solutions can be added and/or removed from the Opportunity.</span></span> <span data-ttu-id="d5618-284">Microsoft と共有する前に、少なくとも1つの共同販売準備完了または Microsoft ソリューションを営業案件に追加することが必須です。</span><span class="sxs-lookup"><span data-stu-id="d5618-284">It is mandatory to add at least one Co-sell ready or Microsoft solution to the Opportunity before sharing it with Microsoft.</span></span> <span data-ttu-id="d5618-285">このオブジェクトを営業案件に関連付けるには、CRM で営業案件フォームを更新します。</span><span class="sxs-lookup"><span data-stu-id="d5618-285">To associate this object to Opportunity, update the Opportunity form in CRM:</span></span>

  <span data-ttu-id="d5618-286">営業案件フォームで適切なタブを選択し、次に示すようにサブグリッドを追加します。</span><span class="sxs-lookup"><span data-stu-id="d5618-286">Select the appropriate tab in Opportunity form and add a sub-grid as shown below:</span></span>

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="営業案件フォーム":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{alt-text}":::



- <span data-ttu-id="d5618-289">Microsoft ソリューションを追加した後は、販売元が追加する必要がないように、共同販売ソリューションの詳細を事前に設定できます。</span><span class="sxs-lookup"><span data-stu-id="d5618-289">After adding Microsoft Solutions, you can pre-populate Co-sell ready solutions details so that your sellers don’t have to add them.</span></span> <span data-ttu-id="d5618-290">新しいソリューションの詳細を追加するには、CRM の [Microsoft ソリューションの詳細] オブジェクトにアクセスし、[ **レコードの追加** ] をクリックして1つのエントリを追加するか、 **Excel upload** を使用して複数のエントリを追加します。</span><span class="sxs-lookup"><span data-stu-id="d5618-290">To add a new solution detail, go to Microsoft Solution Details object in CRM and click on **Add Record** to add one entry or use **Excel upload** to add multiple entries.</span></span>

:::image type="content" source="images/dynamic-1a.png" alt-text="ソリューションの詳細":::

### <a name="scenarios"></a><span data-ttu-id="d5618-292">モデル</span><span class="sxs-lookup"><span data-stu-id="d5618-292">SCENARIOS:</span></span>

1. <span data-ttu-id="d5618-293">CRM で参照が作成または更新され、パートナーセンターで同期される場合の参照の同期:</span><span class="sxs-lookup"><span data-stu-id="d5618-293">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="d5618-294">CRM の **営業案件** セクションで可視性を持つユーザーを使用して、DYNAMICS 365 CRM 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="d5618-294">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="d5618-295">Dynamics 365 環境で "新しい営業案件" を作成するときに、[Microsoft パートナーセンター] セクションが表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="d5618-295">Ensure that the Microsoft Partner Center section  is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   :::image type="content" source="images/dynamic-2a.png" alt-text="新しい営業案件"::: 

   3. <span data-ttu-id="d5618-297">この機会をパートナーセンターと同期するには、カードビューで次のフィールドが設定されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="d5618-297">To synchronize this opportunity with Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="d5618-298">**Microsoft のヘルプ** を参照してください。共同販売紹介を作成するには、適切なヘルプオプションを選択してください。</span><span class="sxs-lookup"><span data-stu-id="d5618-298">**How can Microsoft help?**: To create a Co-sell referral select an appropriate help option.</span></span>

         :::image type="content" source="images/dynamic-3a.png" alt-text="カードビューで適切なフィールドを取得する方法":::

      - <span data-ttu-id="d5618-300">**顧客の連絡先**: 共同販売の紹介を作成するには、営業案件に顧客の連絡先を追加します。</span><span class="sxs-lookup"><span data-stu-id="d5618-300">**Customer Contact**: To create a Co-sell referral, add a customer contact to Opportunity.</span></span>
      - <span data-ttu-id="d5618-301">**パートナーセンターとの同期**: はい</span><span class="sxs-lookup"><span data-stu-id="d5618-301">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="d5618-302">Microsoft のソリューション: 参照を Microsoft と共有するには、有効な共同販売準備完了または Microsoft ソリューションを営業案件に追加します。</span><span class="sxs-lookup"><span data-stu-id="d5618-302">Microsoft Solutions: To share a referral with Microsoft, add a valid Co-sell ready or Microsoft solution to Opportunity.</span></span>
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="ソリューション ID":::

   4. <span data-ttu-id="d5618-304">営業案件が Dynamics 365 で作成され、[パートナーセンターとの同期] オプションが [はい] に設定されたら、10分待ってから、パートナーセンターアカウントにサインインします。</span><span class="sxs-lookup"><span data-stu-id="d5618-304">Once the opportunity is created in Dynamics 365 with Sync with Partner Center option set to Yes, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="d5618-305">参照は Dynamics 365 と参照識別子に同期されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-305">Your referrals will be synchronized with Dynamics 365 and Referral Identifier.</span></span> <span data-ttu-id="d5618-306">参照リンクが設定されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-306">Referral Link will get populated.</span></span> <span data-ttu-id="d5618-307">エラーが発生した場合は、[監査] フィールドにエラー情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-307">In case of a failure, the audit field will be populated with error information.</span></span>
     
    5. <span data-ttu-id="d5618-308">同様に、[パートナーセンターとの同期] オプションを [はい] に設定した場合は、Dynamics 365 CRM の営業案件を更新すると、パートナーセンターアカウントで変更が同期されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-308">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    6. <span data-ttu-id="d5618-309">パートナーセンターで正常に同期された営業案件は、Dynamics 365 の✔アイコンで識別されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-309">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="d5618-310">Microsoft パートナーセンターで参照が作成または更新され、Dynamics 365 環境で同期される場合の参照同期:</span><span class="sxs-lookup"><span data-stu-id="d5618-310">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="d5618-311">パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="d5618-311">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="d5618-312">左側のメニューから [ **紹介** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d5618-312">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="d5618-313">**新しい商談** オプションを選択して、パートナーセンターから新しい共同販売紹介を作成します。</span><span class="sxs-lookup"><span data-stu-id="d5618-313">Create a new Co-sell referral from Partner Center by selecting the  **New deal** option.</span></span>

   4. <span data-ttu-id="d5618-314">Dynamics 365 CRM 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="d5618-314">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="d5618-315">**[Open opportunity**] に移動します。</span><span class="sxs-lookup"><span data-stu-id="d5618-315">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="d5618-316">Microsoft パートナーセンターで作成された紹介が Dynamics 365 CRM で同期されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="d5618-316">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="d5618-317">同期された参照を選択すると、カードビューの詳細が設定されます。</span><span class="sxs-lookup"><span data-stu-id="d5618-317">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d5618-318">次の手順</span><span class="sxs-lookup"><span data-stu-id="d5618-318">Next steps</span></span>

- [<span data-ttu-id="d5618-319">見込み客を管理する</span><span class="sxs-lookup"><span data-stu-id="d5618-319">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="d5618-320">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="d5618-320">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="d5618-321">Microsoft Power の自動化プラットフォームの詳細</span><span class="sxs-lookup"><span data-stu-id="d5618-321">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="d5618-322">パートナー センター Webhook</span><span class="sxs-lookup"><span data-stu-id="d5618-322">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)