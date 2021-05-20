---
title: Dynamics 365 CRM の共同販売パートナー センター
description: Dynamics 365 CRM パートナー センター共同販売コネクタを使用して、顧客の紹介を同期します。 その後、CRM システム内から Microsoft と共同販売できます。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 035a819020097ddee2230b5541e1b477d4b34c14
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148467"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a><span data-ttu-id="db37b-104">Dynamics 365 CRM の共同販売コネクタの概要</span><span class="sxs-lookup"><span data-stu-id="db37b-104">Co-sell connector for Dynamics 365 CRM overview</span></span>

<span data-ttu-id="db37b-105">**適切なロール**: 紹介管理者|CRM のシステム管理者またはシステム カスタマイザー</span><span class="sxs-lookup"><span data-stu-id="db37b-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="db37b-106">パートナー センターコネクタを使用すると、販売者は CRM システム内から Microsoft と共同販売できます。</span><span class="sxs-lookup"><span data-stu-id="db37b-106">Partner Center co-sell connectors enable your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="db37b-107">共同販売取引を管理するために、パートナー センタートレーニングする必要は" は "ない"。</span><span class="sxs-lookup"><span data-stu-id="db37b-107">They won't have to be trained to use Partner Center to manage co-sell deals.</span></span> <span data-ttu-id="db37b-108">共同販売コネクタを使用して、新しい共同販売の紹介を作成して、Microsoft 販売者を引き付け、Microsoft 販売者から紹介を受け取り、紹介を受け入れるか拒否し、取引価値や終了日などの取引データを変更します。</span><span class="sxs-lookup"><span data-stu-id="db37b-108">Use the co-sell connectors to create a new co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept or decline referrals, and modify deal data such as deal value and closing date.</span></span> <span data-ttu-id="db37b-109">また、これらの共同販売取引に関する Microsoft 販売者から更新プログラムを受け取る場合があります。</span><span class="sxs-lookup"><span data-stu-id="db37b-109">You can also receive any updates from the Microsoft sellers on these co-sell deals.</span></span> <span data-ttu-id="db37b-110">すべての紹介作業は、顧客が選択した CRM で管理パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="db37b-110">You can manage all of your referrals work in the CRM of your choice rather than in Partner Center.</span></span>

<span data-ttu-id="db37b-111">このソリューションは、API のPower Automate基パートナー センターしています。</span><span class="sxs-lookup"><span data-stu-id="db37b-111">The solution is based on Power Automate and uses Partner Center APIs.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="db37b-112">前提条件</span><span class="sxs-lookup"><span data-stu-id="db37b-112">Prerequisites</span></span>

<span data-ttu-id="db37b-113">ソリューションをインストールする前に、次の前提条件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="db37b-113">Before you install the solution, make sure to meet the following prerequisites.</span></span>

|<span data-ttu-id="db37b-114">**トピック**</span><span class="sxs-lookup"><span data-stu-id="db37b-114">**Topics**</span></span>   |<span data-ttu-id="db37b-115">**詳細**</span><span class="sxs-lookup"><span data-stu-id="db37b-115">**Details**</span></span>   |<span data-ttu-id="db37b-116">**リンク**</span><span class="sxs-lookup"><span data-stu-id="db37b-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="db37b-117">Microsoft Partner Network (MPN) ID</span><span class="sxs-lookup"><span data-stu-id="db37b-117">Microsoft Partner Network (MPN) ID</span></span> |<span data-ttu-id="db37b-118">有効な MPN ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="db37b-118">You need a valid MPN ID.</span></span>|[<span data-ttu-id="db37b-119">パートナー ネットワークに参加する</span><span class="sxs-lookup"><span data-stu-id="db37b-119">Join the Partner Network</span></span>](https://partner.microsoft.com/)|
|<span data-ttu-id="db37b-120">共同販売の準備完了</span><span class="sxs-lookup"><span data-stu-id="db37b-120">Co-sell ready</span></span>|<span data-ttu-id="db37b-121">IP/サービス ソリューションは共同販売の準備ができている必要があります。</span><span class="sxs-lookup"><span data-stu-id="db37b-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="db37b-122">Microsoft で販売する</span><span class="sxs-lookup"><span data-stu-id="db37b-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)|
|<span data-ttu-id="db37b-123">パートナー センター アカウント</span><span class="sxs-lookup"><span data-stu-id="db37b-123">Partner Center account</span></span>|<span data-ttu-id="db37b-124">新しいテナントに関連付パートナー センター MPN ID は、共同販売ソリューションに関連付けられている MPN ID と同じである必要があります。</span><span class="sxs-lookup"><span data-stu-id="db37b-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your co-sell solution.</span></span> <span data-ttu-id="db37b-125">コネクタをデプロイする前に、パートナー センターポータルに共同販売の紹介が表示されるのを確認します。</span><span class="sxs-lookup"><span data-stu-id="db37b-125">Verify that you can see your co-sell referrals in the Partner Center portal before you deploy the connectors.</span></span>|[<span data-ttu-id="db37b-126">アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="db37b-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="db37b-127">パートナー センターのユーザー ロール</span><span class="sxs-lookup"><span data-stu-id="db37b-127">Partner Center user roles</span></span>|<span data-ttu-id="db37b-128">コネクタをインストールして使用する従業員は、紹介管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="db37b-128">The employee who will install and use the connectors must be a Referrals admin.</span></span>|[<span data-ttu-id="db37b-129">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="db37b-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="db37b-130">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="db37b-130">Dynamics 365 CRM</span></span>|<span data-ttu-id="db37b-131">CRM ユーザー ロールは、システム管理者またはシステム カスタマイザーです。</span><span class="sxs-lookup"><span data-stu-id="db37b-131">The CRM user role is System admin or System customizer.</span></span>|[<span data-ttu-id="db37b-132">Dynamics 365 でロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="db37b-132">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="db37b-133">パワー自動化フローアカウント</span><span class="sxs-lookup"><span data-stu-id="db37b-133">Power Automate flow account</span></span>|<span data-ttu-id="db37b-134">テスト、ステージング、および運用のためのデータベースを使用して、新しい運用環境を作成します。</span><span class="sxs-lookup"><span data-stu-id="db37b-134">Create a new production environment with a database for testing, staging, and production.</span></span> <span data-ttu-id="db37b-135">データベースを含む既存の運用環境がある場合は、再利用できます。</span><span class="sxs-lookup"><span data-stu-id="db37b-135">If you have an existing production environment with a database, it can be reused.</span></span> <span data-ttu-id="db37b-136">コネクタソリューションをインストールするユーザーには、電源自動化ライセンスとこの環境へのアクセスが必要です。</span><span class="sxs-lookup"><span data-stu-id="db37b-136">The user who's going to install the connector solution must have a Power Automate license and access to this environment.</span></span> <span data-ttu-id="db37b-137">インストールが失敗した場合に、進行状況を監視し、詳細情報を [Power の自動化](https://flow.microsoft.com/) に取り込むことができます。</span><span class="sxs-lookup"><span data-stu-id="db37b-137">You can monitor the progress and get more information in [Power Automate](https://flow.microsoft.com/) if the installation fails.</span></span> <span data-ttu-id="db37b-138">[**ソリューション**] の [**履歴の表示**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-138">Select **See history** under **Solutions**.</span></span>|[<span data-ttu-id="db37b-139">環境の作成または管理</span><span class="sxs-lookup"><span data-stu-id="db37b-139">Create or manage environment</span></span>](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="db37b-140">Dynamics 365 のパートナーセンターの紹介同期をインストールする (電源自動化ソリューション)</span><span class="sxs-lookup"><span data-stu-id="db37b-140">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate solution)</span></span>

1. <span data-ttu-id="db37b-141">[ [パワー自動化](https://flow.microsoft.com)] にアクセスし、右上隅にある [ **環境** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-141">Go to [Power Automate](https://flow.microsoft.com), and select **Environments** in the upper-right corner.</span></span> <span data-ttu-id="db37b-142">この手順では、使用可能な CRM インスタンスを表示します。</span><span class="sxs-lookup"><span data-stu-id="db37b-142">This step will show you the available CRM instances.</span></span>

1. <span data-ttu-id="db37b-143">右上隅にあるドロップダウンリストから適切な CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-143">Select the appropriate CRM instance from the drop-down list in the upper-right corner.</span></span>

1. <span data-ttu-id="db37b-144">左側の [ **ソリューション** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-144">Select **Solutions** on the left.</span></span>

1. <span data-ttu-id="db37b-145">上部のメニューの [ **AppSource を開く** ] リンクを選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-145">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="開いている AppSource を示すスクリーンショット。":::

1. <span data-ttu-id="db37b-147">ポップアップ画面で、 **Dynamics 365 のパートナーセンターの紹介コネクタ** を検索します。</span><span class="sxs-lookup"><span data-stu-id="db37b-147">Search for **Partner Center Referrals Connectors for Dynamics 365** in the pop-up screen.</span></span>  

1. <span data-ttu-id="db37b-148">[ **今すぐ入手** する] ボタンを選択し、[ **続行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-148">Select the **Get it now** button, and then select **Continue**.</span></span>

1. <span data-ttu-id="db37b-149">CRM (Dynamics 365) 環境を選択してアプリケーションをインストールできるページが表示されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-149">A page appears where you can select the CRM (Dynamics 365) environment to install the application.</span></span> <span data-ttu-id="db37b-150">使用条件に同意します。</span><span class="sxs-lookup"><span data-stu-id="db37b-150">Agree to the terms and conditions.</span></span>

1. <span data-ttu-id="db37b-151">進行状況を監視することができます。インストールが失敗した場合は、[**ソリューション**] の [**履歴の表示**] を選択して、Power の自動化の詳細を確認できます。</span><span class="sxs-lookup"><span data-stu-id="db37b-151">You can monitor the progress and, if the installation fails, you can get more details in Power Automate by selecting **See history** under **Solutions**.</span></span>

1. <span data-ttu-id="db37b-152">インストールが完了したら、[ソリューション] に戻 [りPower Automate](https://flow.microsoft.com) 左側の **[ソリューション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-152">After the installation is complete, go back to [Power Automate](https://flow.microsoft.com) and select **Solutions** on the left.</span></span> <span data-ttu-id="db37b-153">**パートナー センター Dynamics 365** の紹介の同期がソリューションの一覧で **使用** できます。</span><span class="sxs-lookup"><span data-stu-id="db37b-153">**Partner Center Referrals Synchronization for Dynamics 365** is now available in the **Solutions** list.</span></span>

1. <span data-ttu-id="db37b-154">**[Dynamics 365 パートナー センター参照の同期] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="db37b-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="db37b-155">次のPower Automateとエンティティを使用できます。</span><span class="sxs-lookup"><span data-stu-id="db37b-155">The following Power Automate flows and entities are available.</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="使用可能な CRM を示すスクリーンショット。":::

## <a name="test-before-you-go-live"></a><span data-ttu-id="db37b-157">ライブに進む前にテストする</span><span class="sxs-lookup"><span data-stu-id="db37b-157">Test before you go live</span></span>

<span data-ttu-id="db37b-158">実稼働環境で Power Automate ソリューションをインストール、構成、カスタマイズする前に、ステージング CRM インスタンスでソリューションをテストしてください。</span><span class="sxs-lookup"><span data-stu-id="db37b-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span> <span data-ttu-id="db37b-159">次のことを行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="db37b-159">You'll need to:</span></span>

- <span data-ttu-id="db37b-160">ステージング環境POWER AUTOMATE CRM インスタンスに新しいソリューションをインストールします。</span><span class="sxs-lookup"><span data-stu-id="db37b-160">Install the Power Automate solution on a staging environment CRM instance.</span></span>
- <span data-ttu-id="db37b-161">ステージング環境でPower Automateソリューションを構成およびカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="db37b-161">Configure and customize the Power Automate solution in a staging environment.</span></span>
- <span data-ttu-id="db37b-162">ステージング CRM インスタンスでソリューションをテストします。</span><span class="sxs-lookup"><span data-stu-id="db37b-162">Test the solution on a staging CRM instance.</span></span>
- <span data-ttu-id="db37b-163">テストが成功したら、マネージド ソリューションとして実稼働インスタンスにインポートします。</span><span class="sxs-lookup"><span data-stu-id="db37b-163">After a successful test, import as a managed solution to the production instance.</span></span>

## <a name="configure-the-solution"></a><span data-ttu-id="db37b-164">ソリューションを構成する</span><span class="sxs-lookup"><span data-stu-id="db37b-164">Configure the solution</span></span>

1. <span data-ttu-id="db37b-165">CRM インスタンスにソリューションをインストールしたら、 に戻[Power Automate。](https://flow.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="db37b-165">After you've installed the solution in your CRM instance, go back to [Power Automate](https://flow.microsoft.com/).</span></span>

1. <span data-ttu-id="db37b-166">右上隅の **[環境** ] ドロップダウン リストから、新しいソリューションをインストールした CRM インスタンスPower Automateします。</span><span class="sxs-lookup"><span data-stu-id="db37b-166">From the **Environments** drop-down list in the upper-right corner, select the CRM instance where you installed the Power Automate solution.</span></span>

1. <span data-ttu-id="db37b-167">3 つのユーザー アカウントを関連付ける接続を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="db37b-167">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="db37b-168">パートナー センター管理者の資格情報を持つユーザーを追加する</span><span class="sxs-lookup"><span data-stu-id="db37b-168">Partner Center user with Referrals admin credentials</span></span>
   - <span data-ttu-id="db37b-169">パートナー センターのイベント</span><span class="sxs-lookup"><span data-stu-id="db37b-169">Partner Center Events</span></span>
   - <span data-ttu-id="db37b-170">ソリューション内のPower Automateを含む CRM 管理者</span><span class="sxs-lookup"><span data-stu-id="db37b-170">CRM admin with the Power Automate flows in the solution</span></span>

   1. <span data-ttu-id="db37b-171">左側 **の [** 接続] を選択し、一 **覧パートナー センター [** 紹介] ソリューションを選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-171">Select **Connections** on the left, and select the **Partner Center Referrals** solution from the list.</span></span>

   1. <span data-ttu-id="db37b-172">[接続の作成] を選択 **して接続を作成します**。</span><span class="sxs-lookup"><span data-stu-id="db37b-172">Create a connection by selecting **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="[接続の作成] を示すスクリーンショット。":::

   1. <span data-ttu-id="db37b-174">右上隅 **のパートナー センターで** 、紹介 (プレビュー) を検索します。</span><span class="sxs-lookup"><span data-stu-id="db37b-174">Search for **Partner Center Referrals (preview)** in the search bar in the upper-right corner.</span></span>

   1. <span data-ttu-id="db37b-175">参照管理者の資格情報ロールを使用して、パートナーセンターユーザーの接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="db37b-175">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   1. <span data-ttu-id="db37b-176">次に、参照管理者の資格情報を使用して、パートナーセンターのユーザーにパートナーセンターのイベント接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="db37b-176">Next, create a Partner Center Events connection for your Partner Center user with the Referrals admin credentials.</span></span>

   1. <span data-ttu-id="db37b-177">CRM 管理者ユーザーの Common Data Service (現在の環境) の接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="db37b-177">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
     
   1. <span data-ttu-id="db37b-178">すべての接続を追加すると、環境内に次の接続が表示されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-178">After you've added all the connections, you should see the following connections in your environment.</span></span>

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="接続を示すスクリーンショット。":::

## <a name="edit-the-connections"></a><span data-ttu-id="db37b-180">接続を編集する</span><span class="sxs-lookup"><span data-stu-id="db37b-180">Edit the connections</span></span>

1. <span data-ttu-id="db37b-181">[ **ソリューション** ] ページに戻り、[ **既定のソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-181">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="db37b-182">[**すべて**] を選択して、[**接続の参照 (プレビュー)** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-182">Select **Connection Reference (preview)** by selecting **All**.</span></span>

   :::image type="content" source="images/connection-reference-video.gif" alt-text="接続の編集を示すスクリーンショット。":::

1. <span data-ttu-id="db37b-184">各接続を個別に編集するには、省略記号アイコンを選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-184">Edit each of the connections individually by selecting the ellipsis icon.</span></span> <span data-ttu-id="db37b-185">関連する接続を追加します。</span><span class="sxs-lookup"><span data-stu-id="db37b-185">Add the relevant connections.</span></span>

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="接続の一覧を示すスクリーンショット。":::

1.  <span data-ttu-id="db37b-187">[ **ソリューション** ] ページに戻り、 **Dynamics 365 のパートナーセンター紹介同期** を選択し、次の順序で各フローの横にある省略記号アイコンを選択してフローを有効にします。</span><span class="sxs-lookup"><span data-stu-id="db37b-187">Return to the **Solutions** page, select **Partner Center Referrals Synchronization for Dynamics 365**, and turn on the flow by selecting the ellipsis icon next to each flow in the following sequence.</span></span> <span data-ttu-id="db37b-188">フローを有効にしている間に問題が発生した場合は、「 [カスタマイズの手順](connector-dynamics.md#customize-synchronization-steps) と [トラブルシューティングの手順](connectors-troubleshoot.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db37b-188">If you encounter any issues while you turn on the flow, see [Customization steps](connector-dynamics.md#customize-synchronization-steps) and [Troubleshooting steps](connectors-troubleshoot.md).</span></span>

<span data-ttu-id="db37b-189">次の順序でフローを有効にします。</span><span class="sxs-lookup"><span data-stu-id="db37b-189">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="db37b-190">パートナーセンターの Webhook の登録 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="db37b-190">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="db37b-191">パートナーセンターへの共同販売紹介– Dynamics 365 の作成 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="db37b-191">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="db37b-192">カスタマイズDynamics 365 フローから詳細を作成または取得します。</span><span class="sxs-lookup"><span data-stu-id="db37b-192">[Customize] Create or Get Details from Dynamics 365 flow</span></span>
- <span data-ttu-id="db37b-193">パートナーセンターから Dynamics 365-ヘルパー (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="db37b-193">Partner Center to Dynamics 365 - Helper (Insider Preview)</span></span>
- <span data-ttu-id="db37b-194">パートナーセンターの Microsoft 共同販売参照の更新 Dynamics 365 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="db37b-194">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="db37b-195">パートナー センター Dynamics 365 へのアクセス (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="db37b-195">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="db37b-196">Dynamics 365 から パートナー センター (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="db37b-196">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="db37b-197">Dynamics 365 Opportunity to パートナー センター (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="db37b-197">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="db37b-198">Dynamics 365 Microsoft Solutions to パートナー センター (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="db37b-198">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="db37b-199">Webhook API を使用してリソース変更イベントに登録する</span><span class="sxs-lookup"><span data-stu-id="db37b-199">Use webhook APIs to register for resource change events</span></span>

<span data-ttu-id="db37b-200">Webhook API パートナー センター使用して、リソース変更イベントに登録できます。</span><span class="sxs-lookup"><span data-stu-id="db37b-200">You can use the Partner Center webhook APIs to register for resource change events.</span></span> <span data-ttu-id="db37b-201">これらの変更イベントは、HTTP 投稿として URL に送信されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-201">These change events are sent to your URL as HTTP posts.</span></span>

1. <span data-ttu-id="db37b-202">[パートナー センター **Dynamics 365 (Insider Preview) にアクセスする] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="db37b-202">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

1. <span data-ttu-id="db37b-203">[編集] **アイコンを** 選択し、 **[HTTP 要求を受信した場合] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="db37b-203">Select the **Edit** icon, and select **When a HTTP request is received**.</span></span>

1. <span data-ttu-id="db37b-204">[コピー] **アイコン** を選択して、指定された HTTP POST URL をコピーします。</span><span class="sxs-lookup"><span data-stu-id="db37b-204">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/webhook-video.gif" alt-text="Webhook を使用してリソースの変更を登録する方法を示すスクリーンショット。":::

1. <span data-ttu-id="db37b-206">**[Webhook のパートナー センター (Insider Preview)** フローを選択しPower Automate実行] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="db37b-206">Select the **Partner Center Webhook Registration (Insider Preview)** Power Automate flow, and then select **Run**.</span></span>

1. <span data-ttu-id="db37b-207">右側のウィンドウで **[フローの実行** ] ウィンドウが開き、[続行] を選択 **します**。</span><span class="sxs-lookup"><span data-stu-id="db37b-207">Ensure that the **Run flow** window opens in the right pane, and select **Continue**.</span></span>

1. <span data-ttu-id="db37b-208">次の詳細を入力します。</span><span class="sxs-lookup"><span data-stu-id="db37b-208">Enter the following details:</span></span>

   - <span data-ttu-id="db37b-209">**Http トリガー エンドポイント**: この URL は、前の手順からコピーされました。</span><span class="sxs-lookup"><span data-stu-id="db37b-209">**Http Trigger Endpoint**: This URL was copied from an earlier step.</span></span>
   - <span data-ttu-id="db37b-210">**登録するイベント**: 使用可能なすべてのイベント (**紹介** で作成されたイベント、紹介が **更新** されたイベント、 **関連** する紹介で作成された イベント、および関連する紹介が更新された イベント) **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="db37b-210">**Events to Register**: Select all available events (**referral-created**, **referral-updated**, **related-referral-created**, and **related-referral-updated**).</span></span>
   - <span data-ttu-id="db37b-211">**既存のトリガー エンドポイントが存在する場合は上書きしますか?**: はい。</span><span class="sxs-lookup"><span data-stu-id="db37b-211">**Overwrite existing trigger endpoints if present?**: Yes.</span></span> <span data-ttu-id="db37b-212">特定の Webhook イベントに登録できる URL は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="db37b-212">Only one URL can be registered for a given webhook event.</span></span>

1. <span data-ttu-id="db37b-213">[フロー **の実行] を** 選択し、[完了] を **選択します。**</span><span class="sxs-lookup"><span data-stu-id="db37b-213">Select **Run flow**, and then select **Done.**</span></span>

<span data-ttu-id="db37b-214">Webhook は、イベントをリッスン、作成、および更新できます。</span><span class="sxs-lookup"><span data-stu-id="db37b-214">The webhook can now listen to, create, and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="db37b-215">同期手順をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="db37b-215">Customize synchronization steps</span></span>

<span data-ttu-id="db37b-216">CRM システムは高度にカスタマイズされており、CRM のセットアップに基づいて、パワー自動化ソリューションをカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="db37b-216">CRM systems are highly customized, and you can customize the Power Automate solution based on your CRM setup.</span></span> <span data-ttu-id="db37b-217">パートナーセンターと CRM システムの間で共同販売参照が同期されると、パートナーセンター PC で同期されるフィールドが、 [カスタムフィールドマッピングガイド](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)に一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-217">When co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on the Partner Center PC are listed in the [Custom field mapping guide](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).</span></span>

<span data-ttu-id="db37b-218">フィールドマッピングガイドに従って、必要に応じて、Dynamics 365 フローまたは環境変数 **の [カスタマイズ]** で、適切な変更を行います。</span><span class="sxs-lookup"><span data-stu-id="db37b-218">Follow the field mapping guide, and if necessary, make appropriate changes in **[Customize] Create or Get Details from Dynamics 365 flow** or environment variables.</span></span> <span data-ttu-id="db37b-219">今後のソリューションのアップグレードに影響を与える可能性があるため、パワー自動化ソリューションの他のフローは更新しないでください。</span><span class="sxs-lookup"><span data-stu-id="db37b-219">Don't update any other flows in the Power Automate solution because it can affect future solution upgrades.</span></span>

<span data-ttu-id="db37b-220">次のカスタマイズを使用できます。</span><span class="sxs-lookup"><span data-stu-id="db37b-220">The following customizations are available:</span></span>

- <span data-ttu-id="db37b-221">**営業案件名にチェックマークを表示** する: 既定では、パートナーセンターと DYNAMICS 365 CRM の間の同期が正常に行われていることを示すために、営業案件名の横にチェックマークが表示されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-221">**Display check mark in the opportunity name**: By default, a check mark will be displayed next to the opportunity name to indicate that synchronization between Partner Center and Dynamics 365 CRM is happening successfully.</span></span> <span data-ttu-id="db37b-222">同様に、同期に失敗した場合は、クロスマークが表示されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-222">Similarly, a cross mark will be displayed if synchronization fails.</span></span> <span data-ttu-id="db37b-223">営業案件名にチェックマークまたは十字マークが追加されないようにするには、 **営業案件名環境変数の表示チェックマーク** の現在の値を [いいえ] に設定します。</span><span class="sxs-lookup"><span data-stu-id="db37b-223">To avoid adding a check or cross mark in the opportunity name, set the current value of the **Display check mark in the opportunity name** environment variable to No.</span></span>
- <span data-ttu-id="db37b-224">**取引値**: 既定では、パートナーセンターからの取引値は CRM の **estimatedvalue** との間で同期されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-224">**Deal value**: By default, the deal value from Partner Center will be synced to and from **estimatedvalue** in the CRM.</span></span> <span data-ttu-id="db37b-225">取引値の同期元として CRM に別のフィールドがある場合は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="db37b-225">If you have a different field in the CRM for the deal value to sync from:</span></span>

  - <span data-ttu-id="db37b-226">Dynamics 365 環境変数の **取引値** フィールド名を CRM のフィールド名で更新します。</span><span class="sxs-lookup"><span data-stu-id="db37b-226">Update the **Deal value** field name in the Dynamics 365 environment variable with the CRM's field name.</span></span> <span data-ttu-id="db37b-227">表示名ではなく、フィールドの名前を指定していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="db37b-227">Make sure that you provide the field's name, not its display name.</span></span>
  - <span data-ttu-id="db37b-228">編集 **[カスタマイズ] Dynamics 365 フローから詳細を作成または取得** し、crm での **営業案件の作成または更新** に関するページに移動して、 **新しい営業案件を作成** し、 **既存の営業** 案件のアクションを更新して、crm の適切なフィールドに **DealValue** 値を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="db37b-228">Edit **[Customize] Create or Get Details from Dynamics 365 flow**, and go to **Create or update opportunity** in CRM and update **Create a new opportunity** and **Update existing opportunity** actions to assign the **DealValue** value to the correct field in the CRM.</span></span> <span data-ttu-id="db37b-229">また、[**推定収益**] フィールドから **DealValue** の割り当てを削除します。</span><span class="sxs-lookup"><span data-stu-id="db37b-229">Also, remove the **DealValue** assignment from the **Estimated Revenue** field.</span></span>

- <span data-ttu-id="db37b-230">**顧客アカウントの国コード**: 新しい紹介を作成するときに、2文字の国コード (ISO 3166) を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="db37b-230">**Customer Account Country Code**: It's mandatory to provide a two-letter country code (ISO 3166) when you create a new referral.</span></span> <span data-ttu-id="db37b-231">既定では、国コードは CRM のアカウントの address1_country **フィールドと** 同期されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-231">By default, the country code will be synced to and from the account's **address1_country** field in the CRM.</span></span> <span data-ttu-id="db37b-232">国コードを同期する CRM に別のフィールドがある場合:</span><span class="sxs-lookup"><span data-stu-id="db37b-232">If you have a different field in the CRM for the country code to sync from:</span></span>

   - <span data-ttu-id="db37b-233">2 文字のコードを含むアカウントの非lookup 国コード フィールドの場合:</span><span class="sxs-lookup"><span data-stu-id="db37b-233">For a nonlookup country code field in the account that contains a two-letter code:</span></span>
     - <span data-ttu-id="db37b-234">Dynamics 365 環境変数の Customer **Account Country Code** フィールド名を CRM のフィールド名で更新します。</span><span class="sxs-lookup"><span data-stu-id="db37b-234">Update the **Customer Account Country Code** field name in the Dynamics 365 environment variable with the CRM's field name.</span></span> <span data-ttu-id="db37b-235">表示名ではなく、フィールドの名前を指定してください。</span><span class="sxs-lookup"><span data-stu-id="db37b-235">Make sure that you provide the field's name, not its display name.</span></span>
     - <span data-ttu-id="db37b-236">**[カスタマイズ] Dynamics 365** フローから詳細を作成または取得し、CRM アクションで顧客アカウントを作成または取得するに移動して、CRM の正しいフィールドに Country 値を割り当てる。</span><span class="sxs-lookup"><span data-stu-id="db37b-236">Edit **[Customize] Create or Get Details from Dynamics 365 flow**, and go to **Create or get customer account** in the CRM action to assign a **Country** value to the correct field in the CRM.</span></span> <span data-ttu-id="db37b-237">また、[住所 1: **国** /地域] フィールドから Country 値 **の割り当てを削除** します。</span><span class="sxs-lookup"><span data-stu-id="db37b-237">Also, remove the **Country** value assignment from the **Address 1: Country/Region** field.</span></span>

   - <span data-ttu-id="db37b-238">アカウントの参照ベースの国コード フィールドの場合:</span><span class="sxs-lookup"><span data-stu-id="db37b-238">For a lookup-based country code field in the account:</span></span>
     - <span data-ttu-id="db37b-239">アカウントに新しいカスタム フィールドを追加し、ルックアップ ベースのフィールドで選択した値に基づいて、2 文字の国コード (ISO 3166) を自動的に設定します。その逆も同様です。</span><span class="sxs-lookup"><span data-stu-id="db37b-239">Add a new custom field in the account, and auto-populate it with a two-letter country code (ISO 3166) based on the value selected in the lookup-based field and vice versa.</span></span>
     - <span data-ttu-id="db37b-240">非lookup 国コード フィールドの前の手順に従って、CRM の新しいカスタム フィールドと、その間で新しいカスタム フィールドを同期パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="db37b-240">Follow the preceding steps for the nonlookup country code field to sync a new custom field from the CRM to and from Partner Center.</span></span>

- <span data-ttu-id="db37b-241">**営業** 案件フィールド: 営業案件に入力する必要がある必須フィールドがある場合は、[カスタマイズ **] Dynamics 365** フローから [詳細の作成または取得] を編集し、CRMでの営業案件の作成または更新に関するページに移動し、更新ビジネス要件に基づいて必須フィールドに値を割り当てる新しい営業案件アクションを作成します。</span><span class="sxs-lookup"><span data-stu-id="db37b-241">**Opportunity fields**: If there are mandatory fields in **Opportunity** that need to be populated, edit **[Customize] Create or Get Details from Dynamics 365 flow** and go to **Create or update opportunity** in the CRM and update **Create a new opportunity action** to assign values to the mandatory fields based on your business requirements.</span></span>
- <span data-ttu-id="db37b-242">リード **フィールド:** リードに入力する必要がある必須フィールドがある場合は、[カスタマイズ **] Dynamics 365** フローから [詳細の作成または取得] を編集し、CRM の[リードの作成または更新] に移動して、ビジネス要件に基づいて必須フィールドに値を割り当てる新しいリード アクションの作成に関するページを更新します。</span><span class="sxs-lookup"><span data-stu-id="db37b-242">**Lead fields**: If there are mandatory fields in **Lead** that need to be populated, edit **[Customize] Create or Get Details from Dynamics 365 flow** and go to **Create or update lead** in the CRM and update **Create a new lead action** to assign values to the mandatory fields based on your business requirements.</span></span>
- <span data-ttu-id="db37b-243">**顧客アカウント**: 新しい紹介がパートナーセンターから crm に同期されると、Power Solution の自動化ソリューションでは、顧客の会社名と郵便番号を使用して crm 内の既存のアカウントの検索を試みます。</span><span class="sxs-lookup"><span data-stu-id="db37b-243">**Customer account**: When a new referral is synced from Partner Center to the CRM, the Power Automate solution tries to search for an existing account in the CRM by using the customer company name and postal code.</span></span> <span data-ttu-id="db37b-244">見つからない場合は、新しい顧客アカウントが CRM で作成されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-244">If it doesn't find one, a new customer account will be created in the CRM.</span></span> <span data-ttu-id="db37b-245">検索条件と新しいアカウントの作成の詳細を更新するには、[カスタマイズ] を編集して **Dynamics 365 フローの詳細を作成または取得** し、CRM で **顧客アカウントを作成または取得** する **アクション** を作成します。</span><span class="sxs-lookup"><span data-stu-id="db37b-245">To update the search criteria and new account creation details, edit **[Customize] Create or Get Details from Dynamics 365 flow** and go to **Create or get customer account** in the CRM and **Create customer account action**.</span></span>

## <a name="update-environment-variable"></a><span data-ttu-id="db37b-246">環境変数の更新</span><span class="sxs-lookup"><span data-stu-id="db37b-246">Update environment variable</span></span>

<span data-ttu-id="db37b-247">環境変数の値を更新するには:</span><span class="sxs-lookup"><span data-stu-id="db37b-247">To update an environment variable value:</span></span>

1. <span data-ttu-id="db37b-248">[ **ソリューション** ] ページにアクセスし、[ **既定のソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-248">Go to the **Solutions** page, and select **Default Solution**.</span></span> <span data-ttu-id="db37b-249">[**すべて**] を選択して **環境変数** を選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-249">Select **Environment Variable** by selecting **All**.</span></span>

1. <span data-ttu-id="db37b-250">更新する必要がある値の環境変数を選択し、省略記号アイコンを使用して [ **編集** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-250">Select the environment variable for the value that needs to be updated, and select **Edit** by using the ellipsis icon.</span></span>

1. <span data-ttu-id="db37b-251">[**新しい値**] オプションを使用して値を指定することにより、**現在の値** を更新します (**既定値** を更新しません)。</span><span class="sxs-lookup"><span data-stu-id="db37b-251">Update **Current Value** (don't update **Default Value**) by using the **New value** option and providing the value.</span></span> <span data-ttu-id="db37b-252">値は、変数のデータ型と一致している必要があります。</span><span class="sxs-lookup"><span data-stu-id="db37b-252">The value must match the data type of the variable.</span></span> <span data-ttu-id="db37b-253">たとえば、Yes または No データ型は、Yes または No のいずれかの値を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="db37b-253">For example, the Yes or No data type will accept either the Yes or No value.</span></span>

   :::image type="content" source="images/environment-variables-video.gif" alt-text="環境変数の更新を示すスクリーンショット。":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a><span data-ttu-id="db37b-255">エンドツーエンドの双方向の共同販売参照の同期</span><span class="sxs-lookup"><span data-stu-id="db37b-255">End-to-end bidirectional co-sell referral synchronization</span></span>

<span data-ttu-id="db37b-256">パワー自動化ソリューションのインストール、構成、およびカスタマイズが完了したら、Dynamics 365 とパートナーセンター間の共同販売参照の同期をテストできます。</span><span class="sxs-lookup"><span data-stu-id="db37b-256">After you've installed, configured, and customized the Power Automate solution, you can test for co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="db37b-257">前提条件</span><span class="sxs-lookup"><span data-stu-id="db37b-257">Prerequisites</span></span>

<span data-ttu-id="db37b-258">パートナーセンターと Dynamics 365 CRM 間で紹介を同期するために、Power 区分ソリューションでは、Microsoft 固有の紹介フィールドが明確に示されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-258">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="db37b-259">この id により、販売者チームは、共同販売のために Microsoft と共有する参照を決定することができます。</span><span class="sxs-lookup"><span data-stu-id="db37b-259">This identification gives your seller teams the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="db37b-260">カスタムフィールドとオブジェクトのセットが、ソリューションのインストールの一部として追加されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-260">A set of custom fields and objects will be added as part of the solution installation.</span></span> <span data-ttu-id="db37b-261">CRM 管理者ユーザーは、 **営業案件** のカスタムフィールドを使用して、別の crm セクションを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="db37b-261">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="db37b-262">次のカスタムフィールドは、CRM セクションの一部にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="db37b-262">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="db37b-263">**[同期] パートナー センター:** 営業案件を他のユーザーと同期パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="db37b-263">**Sync with Partner Center**: Whether to sync the opportunity with Partner Center.</span></span> <span data-ttu-id="db37b-264">既定では、このフィールドの値は [いいえ] で、Microsoft と営業案件を共有するには、販売者が明示的に [はい] に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="db37b-264">By default, the value of this field is No and needs to be explicitly set to Yes by your seller to share an opportunity with Microsoft.</span></span> <span data-ttu-id="db37b-265">CRM から CRM に共有されるパートナー センター、このフィールドの値は [はい] に設定されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-265">New referrals shared from Partner Center to CRM will have this field value set to Yes.</span></span>
- <span data-ttu-id="db37b-266">**紹介識別子**: 参照の参照の読み取りパートナー センターフィールド。</span><span class="sxs-lookup"><span data-stu-id="db37b-266">**Referral Identifier**: A read-only identifier field for the Partner Center referral.</span></span>
- <span data-ttu-id="db37b-267">**紹介リンク**: ページ内の紹介への読み取りパートナー センター。</span><span class="sxs-lookup"><span data-stu-id="db37b-267">**Referral Link**: A read-only link to the referral in Partner Center.</span></span>
- <span data-ttu-id="db37b-268">**Microsoft が支援する方法:** 紹介に Microsoft から必要なヘルプ。</span><span class="sxs-lookup"><span data-stu-id="db37b-268">**How can Microsoft help?**: Help required from Microsoft for the referral.</span></span> <span data-ttu-id="db37b-269">共同販売の紹介を作成するには、Microsoft に必要な適切なヘルプを選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-269">To create a co-sell referral, select the appropriate help required from Microsoft.</span></span> <span data-ttu-id="db37b-270">顧客の連絡先は、共同販売の紹介を作成する機会に関連付けられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="db37b-270">A customer contact must be associated to the opportunity to create a co-sell referral.</span></span> <span data-ttu-id="db37b-271">共同販売以外の紹介を作成するには、このフィールドを選択しない必要があります。</span><span class="sxs-lookup"><span data-stu-id="db37b-271">To create a non-co-sell referral, don't select this field.</span></span> <span data-ttu-id="db37b-272">共同販売以外の紹介は、ヘルプが必要な適切なオプションを選択することで、いつでも共同販売の紹介に変換できます。</span><span class="sxs-lookup"><span data-stu-id="db37b-272">A non-co-sell referral can be converted to a co-sell referral anytime by selecting the appropriate help-required option.</span></span>
- <span data-ttu-id="db37b-273">**Microsoft パートナー センターの参照の可視性**: 参照の表示を選択パートナー センターします。</span><span class="sxs-lookup"><span data-stu-id="db37b-273">**Microsoft Partner Center Referral Visibility**: Select visibility for the Partner Center referral.</span></span> <span data-ttu-id="db37b-274">Microsoft の販売者に表示することで、共同販売以外の紹介が共同販売に変換される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="db37b-274">By making it visible to Microsoft sellers, a non-co-sell referral might get converted to co-sell.</span></span> <span data-ttu-id="db37b-275">Microsoft のヘルプが必要な場合、紹介は既定で Microsoft 販売者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-275">When Microsoft help is required, the referral is visible to Microsoft sellers by default.</span></span> <span data-ttu-id="db37b-276">このフィールドが表示済みとしてマークされた後は、元に戻す必要があります。</span><span class="sxs-lookup"><span data-stu-id="db37b-276">After this field is marked as visible, it can't be reverted.</span></span>
- <span data-ttu-id="db37b-277">**Microsoft CRM 識別子**: 共同販売の紹介が作成され、Microsoft によって受け入れられると、このフィールドに Microsoft の CRM 識別子が入力されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-277">**Microsoft CRM Identifier**: When a co-sell referral is created and accepted by Microsoft, this field will get populated with Microsoft's CRM identifier.</span></span>
- <span data-ttu-id="db37b-278">**製品: 廃止**: このフィールドを使用したり、CRM セクションに追加したりしません。</span><span class="sxs-lookup"><span data-stu-id="db37b-278">**Products: Obsolete**: Don't use this field or add it to the CRM section.</span></span> <span data-ttu-id="db37b-279">旧バージョンとの互換性のためにのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="db37b-279">It's available for backward compatibility only.</span></span> <span data-ttu-id="db37b-280">代わりにパートナー センターソリューションを使用してください。</span><span class="sxs-lookup"><span data-stu-id="db37b-280">Use Partner Center solutions instead.</span></span>
- <span data-ttu-id="db37b-281">**監査**: 参照と同期する読み取りパートナー センター証跡。</span><span class="sxs-lookup"><span data-stu-id="db37b-281">**Audit**: A read-only audit trail for syncing with Partner Center referrals.</span></span>
- <span data-ttu-id="db37b-282">**Microsoft パートナー センター ソリューション**: 共同販売対応ソリューションまたは Microsoft ソリューションを機会に関連付けるカスタム オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="db37b-282">**Microsoft Partner Center Solutions**: A custom object to associate co-sell ready solutions or Microsoft solutions with the opportunity.</span></span> <span data-ttu-id="db37b-283">営業案件から1つまたは複数のソリューションを追加または削除できます。</span><span class="sxs-lookup"><span data-stu-id="db37b-283">One or more solutions can be added or removed from the opportunity.</span></span> <span data-ttu-id="db37b-284">Microsoft と共有する前に、少なくとも1つの共同販売準備完了または Microsoft ソリューションを営業案件に追加することが必須です。</span><span class="sxs-lookup"><span data-stu-id="db37b-284">It's mandatory to add at least one co-sell ready or Microsoft solution to the opportunity before you share it with Microsoft.</span></span> <span data-ttu-id="db37b-285">このオブジェクトを営業案件に関連付けるには、CRM で **営業案件** フォームを更新します。</span><span class="sxs-lookup"><span data-stu-id="db37b-285">To associate this object to the opportunity, update the **Opportunity** form in the CRM.</span></span>

  <span data-ttu-id="db37b-286">**営業案件** フォームで適切なタブを選択し、次に示すようにサブグリッドを追加します。</span><span class="sxs-lookup"><span data-stu-id="db37b-286">Select the appropriate tab on the **Opportunity** form, and add a subgrid as shown here.</span></span>

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="営業案件フォームを示すスクリーンショット。":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Microsoft ソリューションを示すスクリーンショット。":::

- <span data-ttu-id="db37b-289">Microsoft ソリューションを追加した後は、販売元が追加する必要がないように、共同販売の準備ができたソリューションの詳細を事前に設定できます。</span><span class="sxs-lookup"><span data-stu-id="db37b-289">After you add Microsoft solutions, you can prepopulate co-sell ready solution details so that your sellers don't have to add them.</span></span> <span data-ttu-id="db37b-290">新しいソリューションの詳細を追加するには、CRM の Microsoft Solution Details オブジェクトにアクセスし、[ **レコードの追加** ] を選択して1つのエントリを追加するか、 **Excel upload** を使用して複数のエントリを追加します。</span><span class="sxs-lookup"><span data-stu-id="db37b-290">To add a new solution detail, go to the Microsoft Solution Details object in the CRM and select **Add Record** to add one entry or use **Excel upload** to add multiple entries.</span></span>

  :::image type="content" source="images/dynamic-1a.png" alt-text="新しい Microsoft ソリューションの詳細を示すスクリーンショット。":::

### <a name="scenarios"></a><span data-ttu-id="db37b-292">シナリオ</span><span class="sxs-lookup"><span data-stu-id="db37b-292">Scenarios</span></span>

1. <span data-ttu-id="db37b-293">CRM で参照が作成または更新され、パートナーセンターで同期される場合の参照同期:</span><span class="sxs-lookup"><span data-stu-id="db37b-293">Referral synchronization when referral is created or updated in the CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="db37b-294">CRM の **営業案件** セクションで可視性を持つユーザーを使用して、DYNAMICS 365 CRM 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="db37b-294">Sign in to your Dynamics 365 CRM environment with the user who has visibility in the **Opportunity** section of the CRM.</span></span>

   1. <span data-ttu-id="db37b-295">Dynamics 365 環境で新しい営業案件を作成するときに、[ **Microsoft パートナーセンター** ] セクションが表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="db37b-295">Ensure that the **Microsoft Partner Center** section is present when you create a new opportunity in the Dynamics 365 environment.</span></span>

      :::image type="content" source="images/dynamic-2a.png" alt-text="新しい営業案件を示すスクリーンショット。":::

   1. <span data-ttu-id="db37b-297">この機会をパートナーセンターと同期するには、カードビューで次のフィールドが設定されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="db37b-297">To synchronize this opportunity with Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="db37b-298">**Microsoft のヘルプについ** て教えてください。共同販売の紹介を作成するには、適切なヘルプオプションを選択してください。</span><span class="sxs-lookup"><span data-stu-id="db37b-298">**How can Microsoft help?**: To create a co-sell referral, select an appropriate help option.</span></span>

         :::image type="content" source="images/dynamic-3a.png" alt-text="カードビューで適切なフィールドを取得する方法を示すスクリーンショット。":::

      - <span data-ttu-id="db37b-300">**顧客の連絡先**: 共同販売の紹介を作成するには、営業案件に顧客の連絡先を追加します。</span><span class="sxs-lookup"><span data-stu-id="db37b-300">**Customer contact**: To create a co-sell referral, add a customer contact to the opportunity.</span></span>
      - <span data-ttu-id="db37b-301">**パートナーセンターとの同期**: はい。</span><span class="sxs-lookup"><span data-stu-id="db37b-301">**Sync With Partner Center**: Yes.</span></span>
      - <span data-ttu-id="db37b-302">**Microsoft のソリューション**: 参照を microsoft と共有するには、有効な共同販売準備完了または microsoft ソリューションを営業案件に追加します。</span><span class="sxs-lookup"><span data-stu-id="db37b-302">**Microsoft Solutions**: To share a referral with Microsoft, add a valid co-sell ready or Microsoft solution to the opportunity.</span></span>
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="ソリューション ID を示すスクリーンショット。":::

   1. <span data-ttu-id="db37b-304">Dynamics 365 で営業案件が作成され、[同期と同期] オプションパートナー センター [は **い** ] に設定された後、10 分待ちます。</span><span class="sxs-lookup"><span data-stu-id="db37b-304">After the opportunity is created in Dynamics 365 with the **Sync With Partner Center** option set to Yes, wait 10 minutes.</span></span> <span data-ttu-id="db37b-305">次に、自分のアカウントパートナー センターします。</span><span class="sxs-lookup"><span data-stu-id="db37b-305">Then sign in to your Partner Center account.</span></span> <span data-ttu-id="db37b-306">紹介は Dynamics 365 および参照識別子 と **同期されます**。</span><span class="sxs-lookup"><span data-stu-id="db37b-306">Your referrals will be synchronized with Dynamics 365 and **Referral Identifier**.</span></span> <span data-ttu-id="db37b-307">**紹介リンク** が設定されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-307">**Referral Link** will get populated.</span></span> <span data-ttu-id="db37b-308">エラーが発生した場合は、[監査] **フィールド** にエラー情報が入力されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-308">If there's a failure, the **Audit** field will be populated with error information.</span></span>
     
    1. <span data-ttu-id="db37b-309">同様に、[ **パートナー センター** と同期する ] オプションが [はい] に設定されている営業案件の場合は、Dynamics 365 CRM で営業案件を更新すると、パートナー センター アカウントで変更が同期されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-309">Likewise, for an opportunity that had the **Sync With Partner Center** option set to Yes, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    1. <span data-ttu-id="db37b-310">Dynamics 365 では、パートナー センターと正常に同期✔が識別されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-310">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

1. <span data-ttu-id="db37b-311">Dynamics 365 環境で参照が作成または更新パートナー センター同期された場合の紹介の同期:</span><span class="sxs-lookup"><span data-stu-id="db37b-311">Referral synchronization when the referral is created or updated in Partner Center and synchronized in the Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="db37b-312">ダッシュボード にサインインパートナー センター [します](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="db37b-312">Sign in to your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   1. <span data-ttu-id="db37b-313">左側 **のメニューから [** 紹介] を選択します。</span><span class="sxs-lookup"><span data-stu-id="db37b-313">Select **Referrals** from the left menu.</span></span>

   1. <span data-ttu-id="db37b-314">[新しい取引] オプションを選択して、パートナー センターから新しい **共同販売の紹介を作成** します。</span><span class="sxs-lookup"><span data-stu-id="db37b-314">Create a new co-sell referral from Partner Center by selecting the **New deal** option.</span></span>

   1. <span data-ttu-id="db37b-315">Dynamics 365 CRM 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="db37b-315">Sign in to your Dynamics 365 CRM environment.</span></span>

   1. <span data-ttu-id="db37b-316">[Open **Opportunities] に移動します**。</span><span class="sxs-lookup"><span data-stu-id="db37b-316">Go to **Open Opportunities**.</span></span> <span data-ttu-id="db37b-317">このページで作成パートナー センター Dynamics 365 CRM で同期されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-317">The referral created in Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   1. <span data-ttu-id="db37b-318">同期された紹介を選択すると、カード ビューの詳細が設定されます。</span><span class="sxs-lookup"><span data-stu-id="db37b-318">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="db37b-319">次のステップ</span><span class="sxs-lookup"><span data-stu-id="db37b-319">Next steps</span></span>

- [<span data-ttu-id="db37b-320">見込み客を管理する</span><span class="sxs-lookup"><span data-stu-id="db37b-320">Manage leads</span></span>](manage-leads.md)
- [<span data-ttu-id="db37b-321">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="db37b-321">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
- [<span data-ttu-id="db37b-322">Microsoft Power Automate プラットフォームの詳細</span><span class="sxs-lookup"><span data-stu-id="db37b-322">More about Microsoft Power Automate platform</span></span>](/power-automate/)
- [<span data-ttu-id="db37b-323">パートナー センター Webhook</span><span class="sxs-lookup"><span data-stu-id="db37b-323">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
