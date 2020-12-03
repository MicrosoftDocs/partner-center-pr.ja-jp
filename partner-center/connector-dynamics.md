---
title: Dynamics 365 CRM パートナーセンターの共同販売コネクタ
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターの紹介を Dynamics 365 CRM の共同販売コネクタと同期します。 販売元は、CRM システム内から Microsoft と共同で販売することができます。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 18a54bf777cb987e8f486f85afcf277e04c1055c
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556363"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="7cef0-104">Dynamics 365 CRM の共同販売コネクタ–概要</span><span class="sxs-lookup"><span data-stu-id="7cef0-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="7cef0-105">適切なロール</span><span class="sxs-lookup"><span data-stu-id="7cef0-105">Appropriate roles</span></span>

- <span data-ttu-id="7cef0-106">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="7cef0-106">Referrals admin</span></span>
- <span data-ttu-id="7cef0-107">CRM のシステム管理者またはシステムカスタマイザー</span><span class="sxs-lookup"><span data-stu-id="7cef0-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="7cef0-108">パートナーセンターの共同販売コネクタを使用すると、販売元は CRM システム内から Microsoft と共同で販売することができます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="7cef0-109">パートナーセンターを使用して共同販売取引を管理するためのトレーニングを行う必要はありません。</span><span class="sxs-lookup"><span data-stu-id="7cef0-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="7cef0-110">共同販売コネクタを使用して、Microsoft 販売者に連絡するための新しい共同販売参照を作成したり、Microsoft 販売者からの推薦を受け取ったり、紹介を受け入れたり拒否したり、商談の価値や終了日などの取引データを変更したりします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="7cef0-111">また、これらの共同販売取引に関するマイクロソフト販売者からの更新を受け取ることもできます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="7cef0-112">パートナーセンターではなく、選択した CRM 内ですべての紹介作業を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="7cef0-113">このソリューションは、Microsoft のパワー自動化ソリューションに基づいており、パートナーセンター Api を使用しています。</span><span class="sxs-lookup"><span data-stu-id="7cef0-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="7cef0-114">をインストールする前に-前提条件</span><span class="sxs-lookup"><span data-stu-id="7cef0-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="7cef0-115">**トピック**</span><span class="sxs-lookup"><span data-stu-id="7cef0-115">**Topics**</span></span>   |<span data-ttu-id="7cef0-116">**詳細**</span><span class="sxs-lookup"><span data-stu-id="7cef0-116">**Details**</span></span>   |<span data-ttu-id="7cef0-117">**リンク**</span><span class="sxs-lookup"><span data-stu-id="7cef0-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="7cef0-118">Microsoft Partner Network ID</span><span class="sxs-lookup"><span data-stu-id="7cef0-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="7cef0-119">有効な MPN ID が必要です</span><span class="sxs-lookup"><span data-stu-id="7cef0-119">You need a valid MPN ID</span></span>|<span data-ttu-id="7cef0-120">[MPN](https://partner.microsoft.com/)に参加するには</span><span class="sxs-lookup"><span data-stu-id="7cef0-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="7cef0-121">共同販売の準備完了</span><span class="sxs-lookup"><span data-stu-id="7cef0-121">Cosell ready</span></span>|<span data-ttu-id="7cef0-122">お客様の IP/サービスソリューションは、共同販売の準備ができている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7cef0-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="7cef0-123">Microsoft との販売</span><span class="sxs-lookup"><span data-stu-id="7cef0-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="7cef0-124">パートナー センター アカウント</span><span class="sxs-lookup"><span data-stu-id="7cef0-124">Partner Center account</span></span>|<span data-ttu-id="7cef0-125">パートナーセンターのテナントに関連付けられている MPN ID は、共同販売ソリューションに関連付けられている MPN ID と同じである必要があります。</span><span class="sxs-lookup"><span data-stu-id="7cef0-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="7cef0-126">コネクタをデプロイする前に、パートナーセンターポータルで共同販売の紹介を確認できることを確認します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="7cef0-127">アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="7cef0-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="7cef0-128">パートナー センターのユーザー ロール</span><span class="sxs-lookup"><span data-stu-id="7cef0-128">Partner Center user roles</span></span>|<span data-ttu-id="7cef0-129">コネクタをインストールして使用する従業員は、参照管理者である必要があります</span><span class="sxs-lookup"><span data-stu-id="7cef0-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="7cef0-130">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="7cef0-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="7cef0-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="7cef0-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="7cef0-132">CRM ユーザーロールは、システム管理者またはシステムカスタマイザーです。</span><span class="sxs-lookup"><span data-stu-id="7cef0-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="7cef0-133">Dynamics 365 でロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="7cef0-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="7cef0-134">パワー自動化フローアカウント</span><span class="sxs-lookup"><span data-stu-id="7cef0-134">Power Automate Flow Account</span></span>|<span data-ttu-id="7cef0-135">CRM システム管理者またはシステムカスタマイザー用のアクティブな [電源自動化](https://flow.microsoft.com) アカウント。</span><span class="sxs-lookup"><span data-stu-id="7cef0-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="7cef0-136">そのユーザーは、インストールの前に少なくとも1回、 [電源の自動](https://flow.microsoft.com) 登録を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="7cef0-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="7cef0-137">Dynamics 365 のパートナーセンターの紹介同期をインストールする (電源自動化ソリューション)</span><span class="sxs-lookup"><span data-stu-id="7cef0-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="7cef0-138">[ [パワー自動化](https://flow.microsoft.com) ] にアクセスし、右上隅にある [ **環境** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="7cef0-139">この手順では、使用可能な CRM インスタンスを表示します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="7cef0-140">右上隅にあるドロップダウンから適切な CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="7cef0-141">左側のナビゲーションバーで [ **ソリューション** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="7cef0-142">上部のメニューの [ **AppSource を開く** ] リンクをクリックします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource を開く":::

5. <span data-ttu-id="7cef0-144">ポップアップ画面で、 **Dynamics365 のパートナーセンターの紹介コネクタ** を検索します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="7cef0-145">[ **今すぐ入手** する] ボタンをクリックし、[ **続行**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="7cef0-146">これにより、CRM (Dynamics 365) 環境を選択してアプリケーションをインストールできるページが開きます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="7cef0-147">使用条件に同意します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="7cef0-148">その後、[ **ソリューションの管理** ] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="7cef0-149">ページの下部にある矢印ボタンを使用して、[パートナーセンターの紹介] に移動します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="7cef0-150">[パートナーセンターの紹介] ソリューションの横に、[**インストールのスケジュール**] が表示されます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="7cef0-151">インストールには10-15 分かかります。</span><span class="sxs-lookup"><span data-stu-id="7cef0-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="7cef0-152">インストールが完了したら、[Power の [自動化](https://flow.microsoft.com) ] に戻り、左側のナビゲーション領域から [ **ソリューション** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="7cef0-153">**Dynamics 365 のパートナーセンターの紹介同期** は、[ソリューション] の一覧で確認できます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="7cef0-154">**Dynamics 365 のパートナーセンターの紹介同期** を選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="7cef0-155">次の電源の自動化フローとエンティティを利用できます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="使用可能な CRMS":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="7cef0-157">ベストプラクティス: 運用前にテストする</span><span class="sxs-lookup"><span data-stu-id="7cef0-157">Best practice: test before you go live</span></span>

<span data-ttu-id="7cef0-158">運用環境でパワー自動化ソリューションをインストール、構成、およびカスタマイズする前に、必ずステージング CRM インスタンスでソリューションをテストしてください。</span><span class="sxs-lookup"><span data-stu-id="7cef0-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="7cef0-159">ステージング環境/CRM インスタンスに Microsoft Power 自動ソリューションをインストールします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="7cef0-160">ソリューションのコピーを作成し、構成を実行して、ステージング環境でフローのカスタマイズを自動化します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="7cef0-161">ステージング/CRM インスタンスでソリューションをテストします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="7cef0-162">成功した場合は、運用インスタンスにマネージドソリューションとしてインポートします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="7cef0-163">ソリューションの構成</span><span class="sxs-lookup"><span data-stu-id="7cef0-163">Configure the solution</span></span>

1. <span data-ttu-id="7cef0-164">CRM インスタンスにソリューションをインストールしたら、[ [Power の自動化](https://flow.microsoft.com/)] に戻ります。</span><span class="sxs-lookup"><span data-stu-id="7cef0-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="7cef0-165">右上隅にある [ **環境** ] ドロップダウンで、パワー自動化ソリューションをインストールした CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="7cef0-166">次の3つのユーザーアカウントを関連付ける接続を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7cef0-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="7cef0-167">参照管理者の資格情報を持つパートナーセンターのユーザー</span><span class="sxs-lookup"><span data-stu-id="7cef0-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="7cef0-168">パートナー センターのイベント</span><span class="sxs-lookup"><span data-stu-id="7cef0-168">Partner Center Events</span></span>

   - <span data-ttu-id="7cef0-169">Power を使用した CRM 管理ソリューションのフローが自動化されます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="7cef0-170">左側のナビゲーションバーから [ **接続** ] を選択し、一覧から "パートナーセンターの紹介" ソリューションを選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="7cef0-171">[ **接続の作成**] をクリックして接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="接続を作成する":::

      3. <span data-ttu-id="7cef0-173">右上隅の検索バーで、 **パートナーセンターの参照 (プレビュー)** を検索します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="7cef0-174">参照管理者の資格情報ロールを使用して、パートナーセンターユーザーの接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="7cef0-175">次に、パートナーセンターのユーザーに、参照管理者の資格情報を使用してパートナーセンターのイベント接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="7cef0-176">CRM 管理者ユーザーの Common Data Service (現在の環境) の接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
       
     
      7. <span data-ttu-id="7cef0-177">すべての接続を追加すると、環境内に次の接続が表示されます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-177">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="接続":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="7cef0-179">接続を編集する</span><span class="sxs-lookup"><span data-stu-id="7cef0-179">Edit the connections</span></span>

1. <span data-ttu-id="7cef0-180">[ **ソリューション** ] ページに戻り、[ **既定のソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-180">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="7cef0-181">[**すべて**] をクリックして、[**接続の参照 (プレビュー)** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-181">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="接続する":::

2. <span data-ttu-id="7cef0-183">3つのドットアイコンを選択して、各接続を1つずつ編集します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-183">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="7cef0-184">関連する接続を追加します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-184">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="一覧表示された接続"::: 

3.  <span data-ttu-id="7cef0-186">次の順序でフローを有効にします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-186">Turn on the flows in the following sequence:</span></span>
- <span data-ttu-id="7cef0-187">パートナーセンターの Webhook の登録 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7cef0-187">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="7cef0-188">パートナーセンターへの共同販売紹介– Dynamics 365 の作成 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7cef0-188">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="7cef0-189">パートナーセンターの Microsoft 共同販売参照の更新 Dynamics 365 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7cef0-189">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="7cef0-190">パートナーセンターから Dynamics 365 へ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7cef0-190">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="7cef0-191">Dynamics 365 からパートナーセンターへ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7cef0-191">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="7cef0-192">Dynamics 365 営業案件パートナーセンター (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7cef0-192">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="7cef0-193">Dynamics 365 Microsoft ソリューション (パートナーセンター) (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7cef0-193">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="7cef0-194">Webhook Api を使用してリソース変更イベントに登録する</span><span class="sxs-lookup"><span data-stu-id="7cef0-194">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="7cef0-195">パートナーセンターの Webhook Api を使用すると、リソース変更イベントに登録できます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-195">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="7cef0-196">これらの変更イベントは、HTTP 投稿として url に送信されます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-196">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="7cef0-197">Url を登録するには、 **パートナーセンターの Webhook 登録 (Insider Preview)** パワー自動化フローを選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-197">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="7cef0-198">参照管理者の資格情報を持つパートナーセンターのユーザー (a.) に接続を追加します。パートナーセンターのイベントは、下に強調表示されています。</span><span class="sxs-lookup"><span data-stu-id="7cef0-198">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="トリガー":::

3. <span data-ttu-id="7cef0-200">これらの更新を行うと、次のように表示されます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-200">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="7cef0-202">変更内容を保存し、[ **有効にする**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-202">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="7cef0-203">パートナーセンターの webhook でイベントの変更をリッスンできるようにするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-203">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="7cef0-204">[ **パートナーセンター] を Dynamics 365 (Insider Preview) に** 選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-204">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="7cef0-205">[ **編集** ] アイコンを選択し、[ **HTTP 要求の受信時**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-205">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="7cef0-206">**コピー** アイコンを選択して、指定された HTTP POST URL をコピーします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-206">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="URL のコピー":::

8. <span data-ttu-id="7cef0-208">次に、"パートナーセンターの Webhook の登録 (Insider Preview)" パワー自動化フローを選択し、[ **実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-208">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="7cef0-209">右側のウィンドウで [実行フロー] ウィンドウが開いていることを確認し、[ **続行**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-209">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="7cef0-210">次の詳細を入力します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-210">Enter the following details:</span></span>

    1. <span data-ttu-id="7cef0-211">**Http トリガーエンドポイント**: 前の手順からコピーされた URL</span><span class="sxs-lookup"><span data-stu-id="7cef0-211">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="7cef0-212">**登録するイベント**: "紹介-作成" と "参照-更新"</span><span class="sxs-lookup"><span data-stu-id="7cef0-212">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="7cef0-213">**既存のトリガーエンドポイントがある場合は上書き** します (存在する場合は既存のエンドポイントを上書きします)。</span><span class="sxs-lookup"><span data-stu-id="7cef0-213">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="7cef0-214">[ **実行** ] を選択し、[完了] を選択し **ます。**</span><span class="sxs-lookup"><span data-stu-id="7cef0-214">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="7cef0-215">Webhook は、イベントの作成と更新をリッスンできるようになりました。</span><span class="sxs-lookup"><span data-stu-id="7cef0-215">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="7cef0-216">同期手順のカスタマイズ</span><span class="sxs-lookup"><span data-stu-id="7cef0-216">Customize synchronization steps</span></span>

<span data-ttu-id="7cef0-217">パートナーセンターと CRM システムの間で共同販売参照が同期されると、パートナーセンター PC で同期されるフィールドがここに表示されます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-217">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="7cef0-218">多くの場合、CRM システムは高度にカスタマイズされています。</span><span class="sxs-lookup"><span data-stu-id="7cef0-218">Often CRM systems are highly customized.</span></span> <span data-ttu-id="7cef0-219">パワー自動化フローをカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-219">You can customize the Power Automate flows.</span></span> <span data-ttu-id="7cef0-220">フィールドマッピングガイドに従って、必要に応じて、パワー自動化フローの手順に適切な変更を加えます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-220">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="7cef0-221">Microsoft パートナーセンターから CRM へのマッピングが提供されますが、CRM 環境に基づいて、フィールドをさらにカスタマイズすることもできます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-221">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="7cef0-222">各パワー自動化フローの複数の手順は、ニーズに応じてカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-222">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="7cef0-223">使用可能なカスタマイズの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-223">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="7cef0-224">パートナーセンターで作成または更新イベントのフィールドを CRM の参照同期にカスタマイズするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-224">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="7cef0-225">a.</span><span class="sxs-lookup"><span data-stu-id="7cef0-225">a.</span></span> <span data-ttu-id="7cef0-226">[パートナーセンター] を選択して Dynamics 365 (Insider Preview) またはパートナーセンターから Salesforce へ (Insider Preview) を選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-226">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="7cef0-227">b.</span><span class="sxs-lookup"><span data-stu-id="7cef0-227">b.</span></span> <span data-ttu-id="7cef0-228">[ **編集** ] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-228">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="7cef0-229">c.</span><span class="sxs-lookup"><span data-stu-id="7cef0-229">c.</span></span> <span data-ttu-id="7cef0-230">選択 **(スコープ) 潜在顧客または営業案件を同期** します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-230">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="7cef0-231">イベントの作成用に (フィールドマッピングガイドに基づいて) CRM フィールドマッピングをカスタマイズするには、[ **新しい共有の営業案件]、[] の順** に選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-231">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="7cef0-232">[サブステップ **if]** を選択し、 **CRM で [新しい営業案件の作成**] を展開します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-232">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="7cef0-233">このセクションでマッピングを編集するには、[フィールドマッピングガイド] を使用します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-233">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="7cef0-234">d.</span><span class="sxs-lookup"><span data-stu-id="7cef0-234">d.</span></span> <span data-ttu-id="7cef0-235">更新イベントの CRM フィールドマッピングをカスタマイズする (フィールドマップガイドに基づく) 場合は、"(スコープ) 潜在顧客または営業案件の同期" ステップをクリックします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-235">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="7cef0-236">e.</span><span class="sxs-lookup"><span data-stu-id="7cef0-236">e.</span></span> <span data-ttu-id="7cef0-237">**営業案件の更新である場合は、** を選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-237">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="7cef0-238">[サブステップ **if yes]** を選択し、次に **パートナーセンターと CRM の営業案件オブジェクト間の差異がある場合** は、を展開します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-238">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="7cef0-239">f.</span><span class="sxs-lookup"><span data-stu-id="7cef0-239">f.</span></span> <span data-ttu-id="7cef0-240">**既存の営業案件を更新** する場合は、[**はい]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-240">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="7cef0-241">更新イベントの CRM から PC への参照同期のフィールドをカスタマイズするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-241">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="7cef0-242">a.</span><span class="sxs-lookup"><span data-stu-id="7cef0-242">a.</span></span> <span data-ttu-id="7cef0-243">[ **編集**  ] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-243">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="7cef0-244">b.</span><span class="sxs-lookup"><span data-stu-id="7cef0-244">b.</span></span> <span data-ttu-id="7cef0-245">[ **(スコープ)] を選択して、営業案件を同期** します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-245">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="7cef0-246">c.</span><span class="sxs-lookup"><span data-stu-id="7cef0-246">c.</span></span> <span data-ttu-id="7cef0-247">更新イベントの CRM フィールドマッピングをカスタマイズするに **は、パートナーセンターと crm の潜在顧客オブジェクトが異なるかどうか** を選択してから、を選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-247">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="7cef0-248">d.</span><span class="sxs-lookup"><span data-stu-id="7cef0-248">d.</span></span> <span data-ttu-id="7cef0-249">[ **はい] の場合** はサブステップを選択し、[ **営業案件データを使用して紹介を更新する**] ステップを展開します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-249">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="7cef0-250">このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-250">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="7cef0-251">Create events の CRM to PC 参照同期のフィールドをカスタマイズするには</span><span class="sxs-lookup"><span data-stu-id="7cef0-251">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="7cef0-252">a.</span><span class="sxs-lookup"><span data-stu-id="7cef0-252">a.</span></span> <span data-ttu-id="7cef0-253">[ **編集**  ] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-253">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="7cef0-254">b.</span><span class="sxs-lookup"><span data-stu-id="7cef0-254">b.</span></span> <span data-ttu-id="7cef0-255">**参照の同期を選択 (スコープ) します。**</span><span class="sxs-lookup"><span data-stu-id="7cef0-255">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="7cef0-256">c.</span><span class="sxs-lookup"><span data-stu-id="7cef0-256">c.</span></span> <span data-ttu-id="7cef0-257">[イベントの作成] で (フィールドマッピングガイドに基づいて) CRM フィールドマッピングをカスタマイズする場合は、[ **Microsoft の紹介を作成する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-257">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="7cef0-258">このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-258">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

<span data-ttu-id="7cef0-259">2つの環境変数が作成されます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-259">There are two environment variables created:</span></span>

- <span data-ttu-id="7cef0-260">チェックマーク: パートナーセンターと Dynamics 365 CRM の間で双方向に同期される営業案件以外にチェックマークアイコンが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-260">Checkmark: Signifies whether you would need a checkmark icon besides opportunities that are synchronized bi-directionally between Partner Center and Dynamics 365 CRM.</span></span>

- <span data-ttu-id="7cef0-261">共同販売機会の同期のみ: 共同販売機会のみを同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-261">Sync co-sell opportunities only: Signifies whether you want to synchronize only Co-sell opportunities.</span></span>

<span data-ttu-id="7cef0-262">環境変数の既定値の編集を選択できます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-262">You can choose to edit the default value for the environment variables.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="既定値のエディットボックス":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="7cef0-264">エンドツーエンドの双方向の共同販売参照の同期</span><span class="sxs-lookup"><span data-stu-id="7cef0-264">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="7cef0-265">パワー自動化ソリューションをインストールし、構成し、カスタマイズしたら、Dynamics 365 とパートナーセンター間の共同販売参照の同期をテストできます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-265">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="7cef0-266">前提条件</span><span class="sxs-lookup"><span data-stu-id="7cef0-266">Pre-requisites</span></span>

<span data-ttu-id="7cef0-267">パートナーセンターと Dynamics 365 CRM 間で紹介を同期するために、Power 区分ソリューションでは、Microsoft 固有の紹介フィールドが明確に示されます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-267">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="7cef0-268">この id により、販売者チームは、共同販売のために Microsoft と共有する参照を決定することができます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-268">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="7cef0-269">一連のカスタムフィールドは、 **営業案件** エンティティの一部として使用できます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-269">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="7cef0-270">CRM 管理者ユーザーは、 **営業案件** のカスタムフィールドを使用して、別の crm セクションを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7cef0-270">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="7cef0-271">次のカスタムフィールドは、CRM セクションの一部にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="7cef0-271">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="7cef0-272">**パートナーセンターとの同期**: 営業案件を Microsoft パートナーセンターと同期するかどうか</span><span class="sxs-lookup"><span data-stu-id="7cef0-272">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="7cef0-273">**参照識別子**: Microsoft パートナーセンターの紹介の読み取り専用識別子フィールド</span><span class="sxs-lookup"><span data-stu-id="7cef0-273">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="7cef0-274">**紹介リンク**: Microsoft パートナーセンターでの紹介への読み取り専用リンク</span><span class="sxs-lookup"><span data-stu-id="7cef0-274">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="7cef0-275">Microsoft の **ヘルプ** を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7cef0-275">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="7cef0-276">**製品**: この営業案件に関連付けられている製品の一覧</span><span class="sxs-lookup"><span data-stu-id="7cef0-276">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="7cef0-277">**監査**: パートナーセンターの紹介と同期するための読み取り専用の監査証跡</span><span class="sxs-lookup"><span data-stu-id="7cef0-277">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

<span data-ttu-id="7cef0-278">Dynamics 365 CRM の営業案件フォームを更新して、Products フィールドを含めるようにします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-278">Update the opportunity form in Dynamics 365 CRM to include Solutions for Products field.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="営業案件フォーム":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a><span data-ttu-id="7cef0-281">モデル</span><span class="sxs-lookup"><span data-stu-id="7cef0-281">SCENARIOS:</span></span>

1. <span data-ttu-id="7cef0-282">CRM で参照が作成または更新され、パートナーセンターで同期される場合の参照の同期:</span><span class="sxs-lookup"><span data-stu-id="7cef0-282">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="7cef0-283">CRM の **営業案件** セクションで可視性を持つユーザーを使用して、DYNAMICS 365 CRM 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-283">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="7cef0-284">Dynamics 365 環境で "新しい営業案件" を作成するときに、次のセクションが存在することを確認します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-284">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Dynamics 365 の Microsoft パートナーセンター情報を示すサンプルの営業案件セクション。":::

   3. <span data-ttu-id="7cef0-286">この機会を Microsoft パートナーセンターと同期するには、カードビューで次のフィールドを設定していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-286">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="7cef0-287">**パートナーセンターとの同期**: はい</span><span class="sxs-lookup"><span data-stu-id="7cef0-287">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="7cef0-288">**Microsoft のヘルプを使用する方法**: 次から選択してください。</span><span class="sxs-lookup"><span data-stu-id="7cef0-288">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Dynamics 365 のサンプルの営業案件セクションでは、microsoft パートナーセンターのヘルプオプションが表示されます。":::

      - <span data-ttu-id="7cef0-290">**製品**: 製品のソリューション id</span><span class="sxs-lookup"><span data-stu-id="7cef0-290">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="7cef0-291">営業案件が Dynamics 365 で作成され、[ **パートナーセンターとの同期** ] オプションが **[はい]** に設定されたら、10分待ってから、パートナーセンターアカウントにサインインします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-291">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="7cef0-292">参照は Dynamics 365 と同期されます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-292">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="7cef0-293">同様に、[パートナーセンターとの同期] オプションを [はい] に設定した場合は、Dynamics 365 CRM の営業案件を更新すると、パートナーセンターアカウントで変更が同期されます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-293">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="7cef0-294">パートナーセンターで正常に同期された営業案件は、Dynamics 365 の✔アイコンで識別されます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-294">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="7cef0-295">Microsoft パートナーセンターで参照が作成または更新され、Dynamics 365 環境で同期される場合の参照同期:</span><span class="sxs-lookup"><span data-stu-id="7cef0-295">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="7cef0-296">パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-296">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="7cef0-297">左側のメニューから [ **紹介** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-297">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="7cef0-298">[新しい取引] オプションをクリックして、パートナーセンターから新しい共同販売紹介を作成します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-298">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="7cef0-299">Dynamics 365 CRM 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="7cef0-299">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="7cef0-300">**[Open opportunity**] に移動します。</span><span class="sxs-lookup"><span data-stu-id="7cef0-300">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="7cef0-301">Microsoft パートナーセンターで作成された紹介が Dynamics 365 CRM で同期されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="7cef0-301">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="7cef0-302">同期された参照を選択すると、カードビューの詳細が設定されます。</span><span class="sxs-lookup"><span data-stu-id="7cef0-302">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7cef0-303">次の手順</span><span class="sxs-lookup"><span data-stu-id="7cef0-303">Next steps</span></span>

- [<span data-ttu-id="7cef0-304">見込み客を管理する</span><span class="sxs-lookup"><span data-stu-id="7cef0-304">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="7cef0-305">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="7cef0-305">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="7cef0-306">Microsoft Power の自動化プラットフォームの詳細</span><span class="sxs-lookup"><span data-stu-id="7cef0-306">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="7cef0-307">パートナー センター Webhook</span><span class="sxs-lookup"><span data-stu-id="7cef0-307">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)