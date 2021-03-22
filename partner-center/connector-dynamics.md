---
title: Dynamics 365 CRM パートナーセンターの共同販売コネクタ
description: パートナーセンターの紹介を Dynamics 365 CRM の共同販売コネクタと同期します。 その後、CRM システム内から Microsoft との共同販売を行うことができます。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 2082424f8203f0d9c50726e1e5ef7b3e3c39d6c2
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768773"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a><span data-ttu-id="8a747-104">Dynamics 365 CRM の共同販売コネクタの概要</span><span class="sxs-lookup"><span data-stu-id="8a747-104">Co-sell connector for Dynamics 365 CRM overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="8a747-105">適切なロール</span><span class="sxs-lookup"><span data-stu-id="8a747-105">Appropriate roles</span></span>

- <span data-ttu-id="8a747-106">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="8a747-106">Referrals admin</span></span>
- <span data-ttu-id="8a747-107">CRM のシステム管理者またはシステムカスタマイザー</span><span class="sxs-lookup"><span data-stu-id="8a747-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="8a747-108">パートナーセンターの共同販売コネクタを使用すると、販売元は CRM システム内から Microsoft と共同で販売することができます。</span><span class="sxs-lookup"><span data-stu-id="8a747-108">Partner Center co-sell connectors enable your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="8a747-109">パートナーセンターを使用して共同販売取引を管理するためのトレーニングを行う必要はありません。</span><span class="sxs-lookup"><span data-stu-id="8a747-109">They won't have to be trained to use Partner Center to manage co-sell deals.</span></span> <span data-ttu-id="8a747-110">共同販売コネクタを使用して、Microsoft 販売者に連絡したり、Microsoft 販売者からの推薦を受け取ったり、推薦を受け入れたり拒否したり、商談の価値や終了日などの取引データを変更したりするための新しい共同販売の紹介を作成します。</span><span class="sxs-lookup"><span data-stu-id="8a747-110">Use the co-sell connectors to create a new co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept or decline referrals, and modify deal data such as deal value and closing date.</span></span> <span data-ttu-id="8a747-111">また、これらの共同販売取引に関するマイクロソフト販売者からの更新を受け取ることもできます。</span><span class="sxs-lookup"><span data-stu-id="8a747-111">You can also receive any updates from the Microsoft sellers on these co-sell deals.</span></span> <span data-ttu-id="8a747-112">パートナーセンターではなく、選択した CRM ですべての紹介作業を管理できます。</span><span class="sxs-lookup"><span data-stu-id="8a747-112">You can manage all of your referrals work in the CRM of your choice rather than in Partner Center.</span></span>

<span data-ttu-id="8a747-113">このソリューションはパワー自動化に基づいており、パートナーセンター Api を使用します。</span><span class="sxs-lookup"><span data-stu-id="8a747-113">The solution is based on Power Automate and uses Partner Center APIs.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a747-114">前提条件</span><span class="sxs-lookup"><span data-stu-id="8a747-114">Prerequisites</span></span>

<span data-ttu-id="8a747-115">ソリューションをインストールする前に、次の前提条件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="8a747-115">Before you install the solution, make sure to meet the following prerequisites.</span></span>

|<span data-ttu-id="8a747-116">**トピック**</span><span class="sxs-lookup"><span data-stu-id="8a747-116">**Topics**</span></span>   |<span data-ttu-id="8a747-117">**詳細**</span><span class="sxs-lookup"><span data-stu-id="8a747-117">**Details**</span></span>   |<span data-ttu-id="8a747-118">**リンク**</span><span class="sxs-lookup"><span data-stu-id="8a747-118">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="8a747-119">Microsoft Partner Network (MPN) ID</span><span class="sxs-lookup"><span data-stu-id="8a747-119">Microsoft Partner Network (MPN) ID</span></span> |<span data-ttu-id="8a747-120">有効な MPN ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a747-120">You need a valid MPN ID.</span></span>|[<span data-ttu-id="8a747-121">パートナーネットワークに参加する</span><span class="sxs-lookup"><span data-stu-id="8a747-121">Join the Partner Network</span></span>](https://partner.microsoft.com/)|
|<span data-ttu-id="8a747-122">共同販売の準備完了</span><span class="sxs-lookup"><span data-stu-id="8a747-122">Co-sell ready</span></span>|<span data-ttu-id="8a747-123">お客様の IP/サービスソリューションは、共同販売の準備ができている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a747-123">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="8a747-124">Microsoft との販売</span><span class="sxs-lookup"><span data-stu-id="8a747-124">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)|
|<span data-ttu-id="8a747-125">パートナー センター アカウント</span><span class="sxs-lookup"><span data-stu-id="8a747-125">Partner Center account</span></span>|<span data-ttu-id="8a747-126">パートナーセンターのテナントに関連付けられている MPN ID は、共同販売ソリューションに関連付けられている MPN ID と同じである必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a747-126">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your co-sell solution.</span></span> <span data-ttu-id="8a747-127">コネクタをデプロイする前に、パートナーセンターポータルで共同販売参照を確認できることを確認します。</span><span class="sxs-lookup"><span data-stu-id="8a747-127">Verify that you can see your co-sell referrals in the Partner Center portal before you deploy the connectors.</span></span>|[<span data-ttu-id="8a747-128">アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="8a747-128">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="8a747-129">パートナー センターのユーザー ロール</span><span class="sxs-lookup"><span data-stu-id="8a747-129">Partner Center user roles</span></span>|<span data-ttu-id="8a747-130">コネクタをインストールして使用する従業員は、参照管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a747-130">The employee who will install and use the connectors must be a Referrals admin.</span></span>|[<span data-ttu-id="8a747-131">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="8a747-131">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="8a747-132">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="8a747-132">Dynamics 365 CRM</span></span>|<span data-ttu-id="8a747-133">CRM ユーザーロールは、システム管理者またはシステムカスタマイザーです。</span><span class="sxs-lookup"><span data-stu-id="8a747-133">The CRM user role is System admin or System customizer.</span></span>|[<span data-ttu-id="8a747-134">Dynamics 365 でロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="8a747-134">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="8a747-135">パワー自動化フローアカウント</span><span class="sxs-lookup"><span data-stu-id="8a747-135">Power Automate flow account</span></span>|<span data-ttu-id="8a747-136">テスト、ステージング、および運用のためのデータベースを使用して、新しい運用環境を作成します。</span><span class="sxs-lookup"><span data-stu-id="8a747-136">Create a new production environment with a database for testing, staging, and production.</span></span> <span data-ttu-id="8a747-137">データベースを含む既存の運用環境がある場合は、再利用できます。</span><span class="sxs-lookup"><span data-stu-id="8a747-137">If you have an existing production environment with a database, it can be reused.</span></span> <span data-ttu-id="8a747-138">コネクタソリューションをインストールするユーザーには、電源自動化ライセンスとこの環境へのアクセスが必要です。</span><span class="sxs-lookup"><span data-stu-id="8a747-138">The user who's going to install the connector solution must have a Power Automate license and access to this environment.</span></span> <span data-ttu-id="8a747-139">インストールが失敗した場合に、進行状況を監視し、詳細情報を [Power の自動化](https://flow.microsoft.com/) に取り込むことができます。</span><span class="sxs-lookup"><span data-stu-id="8a747-139">You can monitor the progress and get more information in [Power Automate](https://flow.microsoft.com/) if the installation fails.</span></span> <span data-ttu-id="8a747-140">[**ソリューション**] の [**履歴の表示**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-140">Select **See history** under **Solutions**.</span></span>|[<span data-ttu-id="8a747-141">環境の作成または管理</span><span class="sxs-lookup"><span data-stu-id="8a747-141">Create or manage environment</span></span>](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="8a747-142">Dynamics 365 のパートナーセンターの紹介同期をインストールする (電源自動化ソリューション)</span><span class="sxs-lookup"><span data-stu-id="8a747-142">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate solution)</span></span>

1. <span data-ttu-id="8a747-143">[ [パワー自動化](https://flow.microsoft.com)] にアクセスし、右上隅にある [ **環境** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-143">Go to [Power Automate](https://flow.microsoft.com), and select **Environments** in the upper-right corner.</span></span> <span data-ttu-id="8a747-144">この手順では、使用可能な CRM インスタンスを表示します。</span><span class="sxs-lookup"><span data-stu-id="8a747-144">This step will show you the available CRM instances.</span></span>

1. <span data-ttu-id="8a747-145">右上隅にあるドロップダウンリストから適切な CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-145">Select the appropriate CRM instance from the drop-down list in the upper-right corner.</span></span>

1. <span data-ttu-id="8a747-146">左側の [ **ソリューション** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-146">Select **Solutions** on the left.</span></span>

1. <span data-ttu-id="8a747-147">上部のメニューの [ **AppSource を開く** ] リンクを選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-147">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="開いている AppSource を示すスクリーンショット。":::

1. <span data-ttu-id="8a747-149">ポップアップ画面で、 **Dynamics 365 のパートナーセンターの紹介コネクタ** を検索します。</span><span class="sxs-lookup"><span data-stu-id="8a747-149">Search for **Partner Center Referrals Connectors for Dynamics 365** in the pop-up screen.</span></span>  

1. <span data-ttu-id="8a747-150">[ **今すぐ入手** する] ボタンを選択し、[ **続行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-150">Select the **Get it now** button, and then select **Continue**.</span></span>

1. <span data-ttu-id="8a747-151">CRM (Dynamics 365) 環境を選択してアプリケーションをインストールできるページが表示されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-151">A page appears where you can select the CRM (Dynamics 365) environment to install the application.</span></span> <span data-ttu-id="8a747-152">使用条件に同意します。</span><span class="sxs-lookup"><span data-stu-id="8a747-152">Agree to the terms and conditions.</span></span>

1. <span data-ttu-id="8a747-153">進行状況を監視することができます。インストールが失敗した場合は、[**ソリューション**] の [**履歴の表示**] を選択して、Power の自動化の詳細を確認できます。</span><span class="sxs-lookup"><span data-stu-id="8a747-153">You can monitor the progress and, if the installation fails, you can get more details in Power Automate by selecting **See history** under **Solutions**.</span></span>

1. <span data-ttu-id="8a747-154">インストールが完了したら、[Power の [自動化](https://flow.microsoft.com) ] に戻り、左側の [ **ソリューション** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-154">After the installation is complete, go back to [Power Automate](https://flow.microsoft.com) and select **Solutions** on the left.</span></span> <span data-ttu-id="8a747-155">**Dynamics 365 のパートナーセンターの推薦同期** が、[ **ソリューション** ] の一覧で使用できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8a747-155">**Partner Center Referrals Synchronization for Dynamics 365** is now available in the **Solutions** list.</span></span>

1. <span data-ttu-id="8a747-156">**Dynamics 365 のパートナーセンターの紹介同期** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-156">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="8a747-157">次の電源の自動化フローとエンティティを利用できます。</span><span class="sxs-lookup"><span data-stu-id="8a747-157">The following Power Automate flows and entities are available.</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="使用可能な CRMs を示すスクリーンショット。":::

## <a name="test-before-you-go-live"></a><span data-ttu-id="8a747-159">ライブに移行する前にテストする</span><span class="sxs-lookup"><span data-stu-id="8a747-159">Test before you go live</span></span>

<span data-ttu-id="8a747-160">運用環境でパワー自動化ソリューションをインストール、構成、およびカスタマイズする前に、必ずステージング CRM インスタンスでソリューションをテストしてください。</span><span class="sxs-lookup"><span data-stu-id="8a747-160">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span> <span data-ttu-id="8a747-161">次のことを行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a747-161">You'll need to:</span></span>

- <span data-ttu-id="8a747-162">電源自動化ソリューションをステージング環境の CRM インスタンスにインストールします。</span><span class="sxs-lookup"><span data-stu-id="8a747-162">Install the Power Automate solution on a staging environment CRM instance.</span></span>
- <span data-ttu-id="8a747-163">ステージング環境でパワー自動化ソリューションを構成し、カスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="8a747-163">Configure and customize the Power Automate solution in a staging environment.</span></span>
- <span data-ttu-id="8a747-164">ステージング CRM インスタンスでソリューションをテストします。</span><span class="sxs-lookup"><span data-stu-id="8a747-164">Test the solution on a staging CRM instance.</span></span>
- <span data-ttu-id="8a747-165">テストが正常に完了したら、管理ソリューションとして実稼働インスタンスにインポートします。</span><span class="sxs-lookup"><span data-stu-id="8a747-165">After a successful test, import as a managed solution to the production instance.</span></span>

## <a name="configure-the-solution"></a><span data-ttu-id="8a747-166">ソリューションの構成</span><span class="sxs-lookup"><span data-stu-id="8a747-166">Configure the solution</span></span>

1. <span data-ttu-id="8a747-167">CRM インスタンスにソリューションをインストールした後、[ [Power 自動](https://flow.microsoft.com/)] に戻ります。</span><span class="sxs-lookup"><span data-stu-id="8a747-167">After you've installed the solution in your CRM instance, go back to [Power Automate](https://flow.microsoft.com/).</span></span>

1. <span data-ttu-id="8a747-168">右上隅にある [ **環境** ] ドロップダウンリストで、パワー自動化ソリューションをインストールした CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-168">From the **Environments** drop-down list in the upper-right corner, select the CRM instance where you installed the Power Automate solution.</span></span>

1. <span data-ttu-id="8a747-169">次の3つのユーザーアカウントを関連付ける接続を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a747-169">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="8a747-170">参照管理者の資格情報を持つパートナーセンターのユーザー</span><span class="sxs-lookup"><span data-stu-id="8a747-170">Partner Center user with Referrals admin credentials</span></span>
   - <span data-ttu-id="8a747-171">パートナー センターのイベント</span><span class="sxs-lookup"><span data-stu-id="8a747-171">Partner Center Events</span></span>
   - <span data-ttu-id="8a747-172">Power を使用した CRM 管理ソリューションのフローの自動化</span><span class="sxs-lookup"><span data-stu-id="8a747-172">CRM admin with the Power Automate flows in the solution</span></span>

   1. <span data-ttu-id="8a747-173">左側の [ **接続** ] を選択し、一覧から [ **パートナーセンターの紹介** ] ソリューションを選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-173">Select **Connections** on the left, and select the **Partner Center Referrals** solution from the list.</span></span>

   1. <span data-ttu-id="8a747-174">接続を作成するに **は、[接続の作成**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-174">Create a connection by selecting **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="接続の作成を示すスクリーンショット。":::

   1. <span data-ttu-id="8a747-176">右上隅の検索バーで、 **パートナーセンターの参照 (プレビュー)** を検索します。</span><span class="sxs-lookup"><span data-stu-id="8a747-176">Search for **Partner Center Referrals (preview)** in the search bar in the upper-right corner.</span></span>

   1. <span data-ttu-id="8a747-177">参照管理者の資格情報ロールを使用して、パートナーセンターユーザーの接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="8a747-177">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   1. <span data-ttu-id="8a747-178">次に、参照管理者の資格情報を使用して、パートナーセンターのユーザーにパートナーセンターのイベント接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="8a747-178">Next, create a Partner Center Events connection for your Partner Center user with the Referrals admin credentials.</span></span>

   1. <span data-ttu-id="8a747-179">CRM 管理者ユーザーの Common Data Service (現在の環境) の接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="8a747-179">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
     
   1. <span data-ttu-id="8a747-180">すべての接続を追加すると、環境内に次の接続が表示されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-180">After you've added all the connections, you should see the following connections in your environment.</span></span>

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="接続を示すスクリーンショット。":::

## <a name="edit-the-connections"></a><span data-ttu-id="8a747-182">接続を編集する</span><span class="sxs-lookup"><span data-stu-id="8a747-182">Edit the connections</span></span>

1. <span data-ttu-id="8a747-183">[ **ソリューション** ] ページに戻り、[ **既定のソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-183">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="8a747-184">[**すべて**] を選択して、[**接続の参照 (プレビュー)** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-184">Select **Connection Reference (preview)** by selecting **All**.</span></span>

   :::image type="content" source="images/connection-reference-video.gif" alt-text="接続の編集を示すスクリーンショット。":::

1. <span data-ttu-id="8a747-186">省略記号アイコンを選択して、各接続を1つずつ編集します。</span><span class="sxs-lookup"><span data-stu-id="8a747-186">Edit each of the connections one by one by selecting the ellipsis icon.</span></span> <span data-ttu-id="8a747-187">関連する接続を追加します。</span><span class="sxs-lookup"><span data-stu-id="8a747-187">Add the relevant connections.</span></span>

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="接続の一覧を示すスクリーンショット。":::

1.  <span data-ttu-id="8a747-189">[ **ソリューション** ] ページに戻り、 **Dynamics 365 のパートナーセンター紹介同期** を選択し、次の順序で各フローの横にある省略記号アイコンを選択してフローを有効にします。</span><span class="sxs-lookup"><span data-stu-id="8a747-189">Return to the **Solutions** page, select **Partner Center Referrals Synchronization for Dynamics 365**, and turn on the flow by selecting the ellipsis icon next to each flow in the following sequence.</span></span> <span data-ttu-id="8a747-190">フローを有効にしている間に問題が発生した場合は、「 [カスタマイズの手順](connector-dynamics.md#customize-synchronization-steps) と [トラブルシューティングの手順](connectors-troubleshoot.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a747-190">If you encounter any issues while you turn on the flow, see [Customization steps](connector-dynamics.md#customize-synchronization-steps) and [Troubleshooting steps](connectors-troubleshoot.md).</span></span>

<span data-ttu-id="8a747-191">次の順序でフローを有効にします。</span><span class="sxs-lookup"><span data-stu-id="8a747-191">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="8a747-192">パートナーセンターの Webhook の登録 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="8a747-192">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="8a747-193">パートナーセンターへの共同販売紹介– Dynamics 365 の作成 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="8a747-193">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="8a747-194">カスタマイズDynamics 365 フローから詳細を作成または取得します。</span><span class="sxs-lookup"><span data-stu-id="8a747-194">[Customize] Create or Get Details from Dynamics 365 flow</span></span>
- <span data-ttu-id="8a747-195">パートナーセンターから Dynamics 365-ヘルパー (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="8a747-195">Partner Center to Dynamics 365 - Helper (Insider Preview)</span></span>
- <span data-ttu-id="8a747-196">パートナーセンターの Microsoft 共同販売参照の更新 Dynamics 365 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="8a747-196">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="8a747-197">パートナーセンターから Dynamics 365 へ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="8a747-197">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="8a747-198">Dynamics 365 からパートナーセンターへ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="8a747-198">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="8a747-199">Dynamics 365 営業案件パートナーセンター (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="8a747-199">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="8a747-200">Dynamics 365 Microsoft ソリューション (パートナーセンター) (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="8a747-200">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="8a747-201">Webhook Api を使用してリソース変更イベントに登録する</span><span class="sxs-lookup"><span data-stu-id="8a747-201">Use webhook APIs to register for resource change events</span></span>

<span data-ttu-id="8a747-202">パートナーセンターの webhook Api を使用して、リソース変更イベントの登録を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="8a747-202">You can use the Partner Center webhook APIs to register for resource change events.</span></span> <span data-ttu-id="8a747-203">これらの変更イベントは、HTTP 投稿として URL に送信されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-203">These change events are sent to your URL as HTTP posts.</span></span>

1. <span data-ttu-id="8a747-204">[ **パートナーセンター] を Dynamics 365 (Insider Preview) に** 選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-204">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

1. <span data-ttu-id="8a747-205">[ **編集** ] アイコンを選択し、[ **HTTP 要求の受信時**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-205">Select the **Edit** icon, and select **When a HTTP request is received**.</span></span>

1. <span data-ttu-id="8a747-206">**コピー** アイコンを選択して、指定された HTTP POST URL をコピーします。</span><span class="sxs-lookup"><span data-stu-id="8a747-206">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/webhook-video.gif" alt-text="Webhook を使用してリソースの変更を登録する方法を示すスクリーンショット。":::

1. <span data-ttu-id="8a747-208">**パートナーセンターの Webhook 登録 (Insider Preview)** パワー自動化フローを選択し、[**実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-208">Select the **Partner Center Webhook Registration (Insider Preview)** Power Automate flow, and then select **Run**.</span></span>

1. <span data-ttu-id="8a747-209">[フローの **実行** ] ウィンドウが右ペインに表示されていることを確認し、[ **続行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-209">Ensure that the **Run flow** window opens in the right pane, and select **Continue**.</span></span>

1. <span data-ttu-id="8a747-210">次の詳細を入力します。</span><span class="sxs-lookup"><span data-stu-id="8a747-210">Enter the following details:</span></span>

   - <span data-ttu-id="8a747-211">**Http トリガーエンドポイント**: この URL は、前の手順からコピーされました。</span><span class="sxs-lookup"><span data-stu-id="8a747-211">**Http Trigger Endpoint**: This URL was copied from an earlier step.</span></span>
   - <span data-ttu-id="8a747-212">**登録するイベント**: 使用可能なすべてのイベントを選択します (**紹介-作成**、 **参照-更新**、 **関連付けら** れている参照の作成、関連する紹介- **更新**)。</span><span class="sxs-lookup"><span data-stu-id="8a747-212">**Events to Register**: Select all available events (**referral-created**, **referral-updated**, **related-referral-created**, and **related-referral-updated**).</span></span>
   - <span data-ttu-id="8a747-213">**既存のトリガーエンドポイントが存在する場合は上書きしますか?**: はい。</span><span class="sxs-lookup"><span data-stu-id="8a747-213">**Overwrite existing trigger endpoints if present?**: Yes.</span></span> <span data-ttu-id="8a747-214">特定の webhook イベントに登録できる URL は1つだけです。</span><span class="sxs-lookup"><span data-stu-id="8a747-214">Only one URL can be registered for a given webhook event.</span></span>

1. <span data-ttu-id="8a747-215">[ **実行フロー**] を選択し、[完了] を選択し **ます。**</span><span class="sxs-lookup"><span data-stu-id="8a747-215">Select **Run flow**, and then select **Done.**</span></span>

<span data-ttu-id="8a747-216">Webhook は、イベントのリッスン、作成、および更新を行うことができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8a747-216">The webhook can now listen to, create, and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="8a747-217">同期手順のカスタマイズ</span><span class="sxs-lookup"><span data-stu-id="8a747-217">Customize synchronization steps</span></span>

<span data-ttu-id="8a747-218">CRM システムは高度にカスタマイズされており、CRM のセットアップに基づいて、パワー自動化ソリューションをカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="8a747-218">CRM systems are highly customized, and you can customize the Power Automate solution based on your CRM setup.</span></span> <span data-ttu-id="8a747-219">パートナーセンターと CRM システムの間で共同販売参照が同期されると、パートナーセンター PC で同期されるフィールドが、 [カスタムフィールドマッピングガイド](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)に一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-219">When co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on the Partner Center PC are listed in the [Custom field mapping guide](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).</span></span>

<span data-ttu-id="8a747-220">フィールドマッピングガイドに従って、必要に応じて、Dynamics 365 フローまたは環境変数 **の [カスタマイズ]** で、適切な変更を行います。</span><span class="sxs-lookup"><span data-stu-id="8a747-220">Follow the field mapping guide, and if necessary, make appropriate changes in **[Customize] Create or Get Details from Dynamics 365 flow** or environment variables.</span></span> <span data-ttu-id="8a747-221">今後のソリューションのアップグレードに影響を与える可能性があるため、パワー自動化ソリューションの他のフローは更新しないでください。</span><span class="sxs-lookup"><span data-stu-id="8a747-221">Don't update any other flows in the Power Automate solution because it can affect future solution upgrades.</span></span>

<span data-ttu-id="8a747-222">次のカスタマイズを使用できます。</span><span class="sxs-lookup"><span data-stu-id="8a747-222">The following customizations are available:</span></span>

- <span data-ttu-id="8a747-223">**営業案件名にチェックマークを表示** する: 既定では、パートナーセンターと DYNAMICS 365 CRM の間の同期が正常に行われていることを示すために、営業案件名の横にチェックマークが表示されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-223">**Display check mark in the opportunity name**: By default, a check mark will be displayed next to the opportunity name to indicate that synchronization between Partner Center and Dynamics 365 CRM is happening successfully.</span></span> <span data-ttu-id="8a747-224">同様に、同期に失敗した場合は、クロスマークが表示されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-224">Similarly, a cross mark will be displayed if synchronization fails.</span></span> <span data-ttu-id="8a747-225">営業案件名にチェックマークまたは十字マークが追加されないようにするには、 **営業案件名環境変数の表示チェックマーク** の現在の値を [いいえ] に設定します。</span><span class="sxs-lookup"><span data-stu-id="8a747-225">To avoid adding a check or cross mark in the opportunity name, set the current value of the **Display check mark in the opportunity name** environment variable to No.</span></span>
- <span data-ttu-id="8a747-226">**取引値**: 既定では、パートナーセンターからの取引値は CRM の **estimatedvalue** との間で同期されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-226">**Deal value**: By default, the deal value from Partner Center will be synced to and from **estimatedvalue** in the CRM.</span></span> <span data-ttu-id="8a747-227">取引値の同期元として CRM に別のフィールドがある場合は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="8a747-227">If you have a different field in the CRM for the deal value to sync from:</span></span>

  - <span data-ttu-id="8a747-228">Dynamics 365 環境変数の **取引値** フィールド名を CRM のフィールド名で更新します。</span><span class="sxs-lookup"><span data-stu-id="8a747-228">Update the **Deal value** field name in the Dynamics 365 environment variable with the CRM's field name.</span></span> <span data-ttu-id="8a747-229">表示名ではなく、フィールドの名前を指定していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="8a747-229">Make sure that you provide the field's name, not its display name.</span></span>
  - <span data-ttu-id="8a747-230">編集 **[カスタマイズ] Dynamics 365 フローから詳細を作成または取得** し、crm での **営業案件の作成または更新** に関するページに移動して、 **新しい営業案件を作成** し、 **既存の営業** 案件のアクションを更新して、crm の適切なフィールドに **DealValue** 値を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="8a747-230">Edit **[Customize] Create or Get Details from Dynamics 365 flow**, and go to **Create or update opportunity** in CRM and update **Create a new opportunity** and **Update existing opportunity** actions to assign the **DealValue** value to the correct field in the CRM.</span></span> <span data-ttu-id="8a747-231">また、[**推定収益**] フィールドから **DealValue** の割り当てを削除します。</span><span class="sxs-lookup"><span data-stu-id="8a747-231">Also, remove the **DealValue** assignment from the **Estimated Revenue** field.</span></span>

- <span data-ttu-id="8a747-232">**顧客アカウントの国コード**: 新しい紹介を作成するときに、2文字の国コード (ISO 3166) を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a747-232">**Customer Account Country Code**: It's mandatory to provide a two-letter country code (ISO 3166) when you create a new referral.</span></span> <span data-ttu-id="8a747-233">既定では、国コードは CRM のアカウントの **address1_country** フィールドと同期されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-233">By default, the country code will be synced to and from the account's **address1_country** field in the CRM.</span></span> <span data-ttu-id="8a747-234">同期する国コード用の別のフィールドが CRM にある場合は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="8a747-234">If you have a different field in the CRM for the country code to sync from:</span></span>

   - <span data-ttu-id="8a747-235">2文字のコードが含まれているアカウント内の非ルックアップの国コードフィールドの場合:</span><span class="sxs-lookup"><span data-stu-id="8a747-235">For a nonlookup country code field in the account that contains a two-letter code:</span></span>
     - <span data-ttu-id="8a747-236">Dynamics 365 環境変数の **顧客アカウントの国コード** フィールド名を CRM のフィールド名で更新します。</span><span class="sxs-lookup"><span data-stu-id="8a747-236">Update the **Customer Account Country Code** field name in the Dynamics 365 environment variable with the CRM's field name.</span></span> <span data-ttu-id="8a747-237">表示名ではなく、フィールドの名前を指定していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="8a747-237">Make sure that you provide the field's name, not its display name.</span></span>
     - <span data-ttu-id="8a747-238">**[カスタマイズ] Dynamics 365 フローから詳細を作成または取得** し、crm アクションの [**顧客アカウントの作成または取得**] に移動して、crm の適切なフィールドに **国** の値を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="8a747-238">Edit **[Customize] Create or Get Details from Dynamics 365 flow**, and go to **Create or get customer account** in the CRM action to assign a **Country** value to the correct field in the CRM.</span></span> <span data-ttu-id="8a747-239">また、[**住所 1: 国/地域**] フィールドから **country** 値の割り当てを削除します。</span><span class="sxs-lookup"><span data-stu-id="8a747-239">Also, remove the **Country** value assignment from the **Address 1: Country/Region** field.</span></span>

   - <span data-ttu-id="8a747-240">アカウントの検索ベースの国コードフィールドの場合:</span><span class="sxs-lookup"><span data-stu-id="8a747-240">For a lookup-based country code field in the account:</span></span>
     - <span data-ttu-id="8a747-241">アカウントに新しいカスタムフィールドを追加し、参照ベースのフィールドで選択した値に基づいて、2文字の国コード (ISO 3166) を自動的に入力します。逆も同様です。</span><span class="sxs-lookup"><span data-stu-id="8a747-241">Add a new custom field in the account, and auto-populate it with a two-letter country code (ISO 3166) based on the value selected in the lookup-based field and vice versa.</span></span>
     - <span data-ttu-id="8a747-242">この前の手順に従って、新しいカスタムフィールドを CRM とパートナーセンターの間で同期します。</span><span class="sxs-lookup"><span data-stu-id="8a747-242">Follow the preceding steps for the nonlookup country code field to sync a new custom field from the CRM to and from Partner Center.</span></span>

- <span data-ttu-id="8a747-243">**営業案件のフィールド**: データを設定する必要がある **営業案件** の必須フィールドがある場合は、[カスタマイズ] を編集して **Dynamics 365 フローの詳細を作成または取得** し、CRM で [ **営業案件の作成または更新** ] を開き、ビジネス要件に基づいて必須フィールドに値を割り当てる **新しい営業案件アクションを作成** します。</span><span class="sxs-lookup"><span data-stu-id="8a747-243">**Opportunity fields**: If there are mandatory fields in **Opportunity** that need to be populated, edit **[Customize] Create or Get Details from Dynamics 365 flow** and go to **Create or update opportunity** in the CRM and update **Create a new opportunity action** to assign values to the mandatory fields based on your business requirements.</span></span>
- <span data-ttu-id="8a747-244">**潜在顧客のフィールド**: **潜在顧客** に入力が必要な必須フィールドがある場合、[カスタマイズ] を編集して **Dynamics 365 フローから詳細を作成または取得** し、CRM で [ **潜在顧客の作成または更新** ] に移動して、ビジネス要件に基づいて必須フィールドに値を割り当てる **新しい潜在顧客アクションを作成** します。</span><span class="sxs-lookup"><span data-stu-id="8a747-244">**Lead fields**: If there are mandatory fields in **Lead** that need to be populated, edit **[Customize] Create or Get Details from Dynamics 365 flow** and go to **Create or update lead** in the CRM and update **Create a new lead action** to assign values to the mandatory fields based on your business requirements.</span></span>
- <span data-ttu-id="8a747-245">**顧客アカウント**: 新しい紹介がパートナーセンターから crm に同期されると、Power Solution の自動化ソリューションでは、顧客の会社名と郵便番号を使用して crm 内の既存のアカウントの検索を試みます。</span><span class="sxs-lookup"><span data-stu-id="8a747-245">**Customer account**: When a new referral is synced from Partner Center to the CRM, the Power Automate solution tries to search for an existing account in the CRM by using the customer company name and postal code.</span></span> <span data-ttu-id="8a747-246">見つからない場合は、新しい顧客アカウントが CRM で作成されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-246">If it doesn't find one, a new customer account will be created in the CRM.</span></span> <span data-ttu-id="8a747-247">検索条件と新しいアカウントの作成の詳細を更新するには、[カスタマイズ] を編集して **Dynamics 365 フローの詳細を作成または取得** し、CRM で **顧客アカウントを作成または取得** する **アクション** を作成します。</span><span class="sxs-lookup"><span data-stu-id="8a747-247">To update the search criteria and new account creation details, edit **[Customize] Create or Get Details from Dynamics 365 flow** and go to **Create or get customer account** in the CRM and **Create customer account action**.</span></span>

## <a name="update-environment-variable"></a><span data-ttu-id="8a747-248">環境変数の更新</span><span class="sxs-lookup"><span data-stu-id="8a747-248">Update environment variable</span></span>

<span data-ttu-id="8a747-249">環境変数の値を更新するには:</span><span class="sxs-lookup"><span data-stu-id="8a747-249">To update an environment variable value:</span></span>

1. <span data-ttu-id="8a747-250">[ **ソリューション** ] ページにアクセスし、[ **既定のソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-250">Go to the **Solutions** page, and select **Default Solution**.</span></span> <span data-ttu-id="8a747-251">[**すべて**] を選択して **環境変数** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-251">Select **Environment Variable** by selecting **All**.</span></span>

1. <span data-ttu-id="8a747-252">更新する必要がある値の環境変数を選択し、省略記号アイコンを使用して [ **編集** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-252">Select the environment variable for the value that needs to be updated, and select **Edit** by using the ellipsis icon.</span></span>

1. <span data-ttu-id="8a747-253">[**新しい値**] オプションを使用して値を指定することにより、**現在の値** を更新します (**既定値** を更新しません)。</span><span class="sxs-lookup"><span data-stu-id="8a747-253">Update **Current Value** (don't update **Default Value**) by using the **New value** option and providing the value.</span></span> <span data-ttu-id="8a747-254">値は、変数のデータ型と一致している必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a747-254">The value must match the data type of the variable.</span></span> <span data-ttu-id="8a747-255">たとえば、Yes または No データ型は、Yes または No のいずれかの値を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="8a747-255">For example, the Yes or No data type will accept either the Yes or No value.</span></span>

   :::image type="content" source="images/environment-variables-video.gif" alt-text="環境変数の更新を示すスクリーンショット。":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a><span data-ttu-id="8a747-257">エンドツーエンドの双方向の共同販売参照の同期</span><span class="sxs-lookup"><span data-stu-id="8a747-257">End-to-end bidirectional co-sell referral synchronization</span></span>

<span data-ttu-id="8a747-258">パワー自動化ソリューションのインストール、構成、およびカスタマイズが完了したら、Dynamics 365 とパートナーセンター間の共同販売参照の同期をテストできます。</span><span class="sxs-lookup"><span data-stu-id="8a747-258">After you've installed, configured, and customized the Power Automate solution, you can test for co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="8a747-259">前提条件</span><span class="sxs-lookup"><span data-stu-id="8a747-259">Prerequisites</span></span>

<span data-ttu-id="8a747-260">パートナーセンターと Dynamics 365 CRM 間で紹介を同期するために、Power 区分ソリューションでは、Microsoft 固有の紹介フィールドが明確に示されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-260">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="8a747-261">この id により、販売者チームは、共同販売のために Microsoft と共有する参照を決定することができます。</span><span class="sxs-lookup"><span data-stu-id="8a747-261">This identification gives your seller teams the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="8a747-262">カスタムフィールドとオブジェクトのセットが、ソリューションのインストールの一部として追加されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-262">A set of custom fields and objects will be added as part of the solution installation.</span></span> <span data-ttu-id="8a747-263">CRM 管理者ユーザーは、 **営業案件** のカスタムフィールドを使用して、別の crm セクションを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a747-263">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="8a747-264">次のカスタムフィールドは、CRM セクションの一部にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a747-264">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="8a747-265">**パートナーセンターとの同期**: パートナーセンターとの営業案件を同期するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8a747-265">**Sync with Partner Center**: Whether to sync the opportunity with Partner Center.</span></span> <span data-ttu-id="8a747-266">既定では、このフィールドの値は [いいえ] であり、Microsoft との営業案件を共有するには、販売者によって明示的に [はい] に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a747-266">By default, the value of this field is No and needs to be explicitly set to Yes by your seller to share an opportunity with Microsoft.</span></span> <span data-ttu-id="8a747-267">パートナーセンターから CRM に共有されている新しい紹介では、このフィールドの値が [はい] に設定されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-267">New referrals shared from Partner Center to CRM will have this field value set to Yes.</span></span>
- <span data-ttu-id="8a747-268">**参照識別子**: パートナーセンターの紹介の読み取り専用識別子フィールドです。</span><span class="sxs-lookup"><span data-stu-id="8a747-268">**Referral Identifier**: A read-only identifier field for the Partner Center referral.</span></span>
- <span data-ttu-id="8a747-269">**紹介リンク**: パートナーセンターでの紹介への読み取り専用リンク。</span><span class="sxs-lookup"><span data-stu-id="8a747-269">**Referral Link**: A read-only link to the referral in Partner Center.</span></span>
- <span data-ttu-id="8a747-270">Microsoft の **ヘルプ** を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a747-270">**How can Microsoft help?**: Help required from Microsoft for the referral.</span></span> <span data-ttu-id="8a747-271">共同販売の紹介を作成するには、Microsoft からの適切なヘルプを選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-271">To create a co-sell referral, select the appropriate help required from Microsoft.</span></span> <span data-ttu-id="8a747-272">顧客の連絡先は、共同販売の紹介を作成する機会に関連付けられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a747-272">A customer contact must be associated to the opportunity to create a co-sell referral.</span></span> <span data-ttu-id="8a747-273">共同販売以外の推薦を作成するには、このフィールドを選択しないでください。</span><span class="sxs-lookup"><span data-stu-id="8a747-273">To create a non-co-sell referral, don't select this field.</span></span> <span data-ttu-id="8a747-274">共同販売以外の推薦は、適切なヘルプを必要とするオプションを選択することで、いつでも共同販売の紹介に変換できます。</span><span class="sxs-lookup"><span data-stu-id="8a747-274">A non-co-sell referral can be converted to a co-sell referral anytime by selecting the appropriate help-required option.</span></span>
- <span data-ttu-id="8a747-275">**Microsoft パートナーセンターの参照の可視性**: パートナーセンターの紹介の可視性を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-275">**Microsoft Partner Center Referral Visibility**: Select visibility for the Partner Center referral.</span></span> <span data-ttu-id="8a747-276">Microsoft の販売元に見えるようにすることで、共同販売以外の参照が共同販売に変換される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="8a747-276">By making it visible to Microsoft sellers, a non-co-sell referral might get converted to co-sell.</span></span> <span data-ttu-id="8a747-277">Microsoft ヘルプが必要な場合、既定では、Microsoft の販売者に参照が表示されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-277">When Microsoft help is required, the referral is visible to Microsoft sellers by default.</span></span> <span data-ttu-id="8a747-278">このフィールドを表示済みとしてマークした後は、元に戻すことはできません。</span><span class="sxs-lookup"><span data-stu-id="8a747-278">After this field is marked as visible, it can't be reverted.</span></span>
- <span data-ttu-id="8a747-279">**MICROSOFT CRM 識別子**: 共同販売の紹介が microsoft によって作成され、承認されると、このフィールドには MICROSOFT の CRM 識別子が表示されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-279">**Microsoft CRM Identifier**: When a co-sell referral is created and accepted by Microsoft, this field will get populated with Microsoft's CRM identifier.</span></span>
- <span data-ttu-id="8a747-280">**製品: 廃止**: このフィールドを使用したり、CRM セクションに追加したりしないでください。</span><span class="sxs-lookup"><span data-stu-id="8a747-280">**Products: Obsolete**: Don't use this field or add it to the CRM section.</span></span> <span data-ttu-id="8a747-281">旧バージョンとの互換性のためにのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="8a747-281">It's available for backward compatibility only.</span></span> <span data-ttu-id="8a747-282">代わりに、パートナーセンターソリューションを使用してください。</span><span class="sxs-lookup"><span data-stu-id="8a747-282">Use Partner Center solutions instead.</span></span>
- <span data-ttu-id="8a747-283">**Audit**: パートナーセンターの紹介と同期するための読み取り専用の監査証跡。</span><span class="sxs-lookup"><span data-stu-id="8a747-283">**Audit**: A read-only audit trail for syncing with Partner Center referrals.</span></span>
- <span data-ttu-id="8a747-284">**Microsoft パートナーセンターソリューション**: 共同販売の準備ができたソリューションまたは microsoft ソリューションを営業案件と関連付けるためのカスタムオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8a747-284">**Microsoft Partner Center Solutions**: A custom object to associate co-sell ready solutions or Microsoft solutions with the opportunity.</span></span> <span data-ttu-id="8a747-285">営業案件から1つまたは複数のソリューションを追加または削除できます。</span><span class="sxs-lookup"><span data-stu-id="8a747-285">One or more solutions can be added or removed from the opportunity.</span></span> <span data-ttu-id="8a747-286">Microsoft と共有する前に、少なくとも1つの共同販売準備完了または Microsoft ソリューションを営業案件に追加することが必須です。</span><span class="sxs-lookup"><span data-stu-id="8a747-286">It's mandatory to add at least one co-sell ready or Microsoft solution to the opportunity before you share it with Microsoft.</span></span> <span data-ttu-id="8a747-287">このオブジェクトを営業案件に関連付けるには、CRM で **営業案件** フォームを更新します。</span><span class="sxs-lookup"><span data-stu-id="8a747-287">To associate this object to the opportunity, update the **Opportunity** form in the CRM.</span></span>

  <span data-ttu-id="8a747-288">**営業案件** フォームで適切なタブを選択し、次に示すようにサブグリッドを追加します。</span><span class="sxs-lookup"><span data-stu-id="8a747-288">Select the appropriate tab on the **Opportunity** form, and add a subgrid as shown here.</span></span>

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="営業案件フォームを示すスクリーンショット。":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Microsoft ソリューションを示すスクリーンショット。":::

- <span data-ttu-id="8a747-291">Microsoft ソリューションを追加した後は、販売元が追加する必要がないように、共同販売の準備ができたソリューションの詳細を事前に設定できます。</span><span class="sxs-lookup"><span data-stu-id="8a747-291">After you add Microsoft solutions, you can prepopulate co-sell ready solution details so that your sellers don't have to add them.</span></span> <span data-ttu-id="8a747-292">新しいソリューションの詳細を追加するには、CRM の Microsoft Solution Details オブジェクトにアクセスし、[ **レコードの追加** ] を選択して1つのエントリを追加するか、 **Excel upload** を使用して複数のエントリを追加します。</span><span class="sxs-lookup"><span data-stu-id="8a747-292">To add a new solution detail, go to the Microsoft Solution Details object in the CRM and select **Add Record** to add one entry or use **Excel upload** to add multiple entries.</span></span>

  :::image type="content" source="images/dynamic-1a.png" alt-text="新しい Microsoft ソリューションの詳細を示すスクリーンショット。":::

### <a name="scenarios"></a><span data-ttu-id="8a747-294">シナリオ</span><span class="sxs-lookup"><span data-stu-id="8a747-294">Scenarios</span></span>

1. <span data-ttu-id="8a747-295">CRM で参照が作成または更新され、パートナーセンターで同期される場合の参照同期:</span><span class="sxs-lookup"><span data-stu-id="8a747-295">Referral synchronization when referral is created or updated in the CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="8a747-296">CRM の **営業案件** セクションで可視性を持つユーザーを使用して、DYNAMICS 365 CRM 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="8a747-296">Sign in to your Dynamics 365 CRM environment with the user who has visibility in the **Opportunity** section of the CRM.</span></span>

   1. <span data-ttu-id="8a747-297">Dynamics 365 環境で新しい営業案件を作成するときに、[ **Microsoft パートナーセンター** ] セクションが表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="8a747-297">Ensure that the **Microsoft Partner Center** section is present when you create a new opportunity in the Dynamics 365 environment.</span></span>

      :::image type="content" source="images/dynamic-2a.png" alt-text="新しい営業案件を示すスクリーンショット。":::

   1. <span data-ttu-id="8a747-299">この機会をパートナーセンターと同期するには、カードビューで次のフィールドが設定されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="8a747-299">To synchronize this opportunity with Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="8a747-300">**Microsoft のヘルプについ** て教えてください。共同販売の紹介を作成するには、適切なヘルプオプションを選択してください。</span><span class="sxs-lookup"><span data-stu-id="8a747-300">**How can Microsoft help?**: To create a co-sell referral, select an appropriate help option.</span></span>

         :::image type="content" source="images/dynamic-3a.png" alt-text="カードビューで適切なフィールドを取得する方法を示すスクリーンショット。":::

      - <span data-ttu-id="8a747-302">**顧客の連絡先**: 共同販売の紹介を作成するには、営業案件に顧客の連絡先を追加します。</span><span class="sxs-lookup"><span data-stu-id="8a747-302">**Customer contact**: To create a co-sell referral, add a customer contact to the opportunity.</span></span>
      - <span data-ttu-id="8a747-303">**パートナーセンターとの同期**: はい。</span><span class="sxs-lookup"><span data-stu-id="8a747-303">**Sync With Partner Center**: Yes.</span></span>
      - <span data-ttu-id="8a747-304">**Microsoft のソリューション**: 参照を microsoft と共有するには、有効な共同販売準備完了または microsoft ソリューションを営業案件に追加します。</span><span class="sxs-lookup"><span data-stu-id="8a747-304">**Microsoft Solutions**: To share a referral with Microsoft, add a valid co-sell ready or Microsoft solution to the opportunity.</span></span>
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="ソリューション ID を示すスクリーンショット。":::

   1. <span data-ttu-id="8a747-306">Dynamics 365 で営業案件を作成し、[ **パートナーセンターとの同期** ] オプションを [はい] に設定した後、10分間待機します。</span><span class="sxs-lookup"><span data-stu-id="8a747-306">After the opportunity is created in Dynamics 365 with the **Sync With Partner Center** option set to Yes, wait 10 minutes.</span></span> <span data-ttu-id="8a747-307">次に、パートナーセンターアカウントにサインインします。</span><span class="sxs-lookup"><span data-stu-id="8a747-307">Then sign in to your Partner Center account.</span></span> <span data-ttu-id="8a747-308">参照は Dynamics 365 と **参照識別子** に同期されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-308">Your referrals will be synchronized with Dynamics 365 and **Referral Identifier**.</span></span> <span data-ttu-id="8a747-309">**参照リンク** が設定されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-309">**Referral Link** will get populated.</span></span> <span data-ttu-id="8a747-310">エラーが発生した場合は、[ **監査** ] フィールドにエラー情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-310">If there's a failure, the **Audit** field will be populated with error information.</span></span>
     
    1. <span data-ttu-id="8a747-311">同様に、[ **パートナーセンターとの同期** ] オプションを [はい] に設定した場合は、DYNAMICS 365 CRM の営業案件を更新すると、パートナーセンターアカウントで変更が同期されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-311">Likewise, for an opportunity that had the **Sync With Partner Center** option set to Yes, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    1. <span data-ttu-id="8a747-312">パートナーセンターで正常に同期された営業案件は、Dynamics 365 の✔アイコンで識別されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-312">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

1. <span data-ttu-id="8a747-313">参照がパートナーセンターで作成または更新され、Dynamics 365 環境で同期される場合の参照同期:</span><span class="sxs-lookup"><span data-stu-id="8a747-313">Referral synchronization when the referral is created or updated in Partner Center and synchronized in the Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="8a747-314">パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="8a747-314">Sign in to your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   1. <span data-ttu-id="8a747-315">左側のメニューから [ **紹介** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a747-315">Select **Referrals** from the left menu.</span></span>

   1. <span data-ttu-id="8a747-316">**新しい商談** オプションを選択して、パートナーセンターから新しい共同販売紹介を作成します。</span><span class="sxs-lookup"><span data-stu-id="8a747-316">Create a new co-sell referral from Partner Center by selecting the **New deal** option.</span></span>

   1. <span data-ttu-id="8a747-317">Dynamics 365 CRM 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="8a747-317">Sign in to your Dynamics 365 CRM environment.</span></span>

   1. <span data-ttu-id="8a747-318">**オープンチャンス** にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="8a747-318">Go to **Open Opportunities**.</span></span> <span data-ttu-id="8a747-319">パートナーセンターで作成された紹介が Dynamics 365 CRM で同期されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8a747-319">The referral created in Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   1. <span data-ttu-id="8a747-320">同期された参照を選択すると、カードビューの詳細が設定されます。</span><span class="sxs-lookup"><span data-stu-id="8a747-320">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8a747-321">次の手順</span><span class="sxs-lookup"><span data-stu-id="8a747-321">Next steps</span></span>

- [<span data-ttu-id="8a747-322">見込み客を管理する</span><span class="sxs-lookup"><span data-stu-id="8a747-322">Manage leads</span></span>](manage-leads.md)
- [<span data-ttu-id="8a747-323">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="8a747-323">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
- [<span data-ttu-id="8a747-324">Microsoft Power の自動化プラットフォームの詳細</span><span class="sxs-lookup"><span data-stu-id="8a747-324">More about Microsoft Power Automate platform</span></span>](/power-automate/)
- [<span data-ttu-id="8a747-325">パートナー センター Webhook</span><span class="sxs-lookup"><span data-stu-id="8a747-325">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
