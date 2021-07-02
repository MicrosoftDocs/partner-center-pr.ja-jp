---
title: Salesforce CRM パートナーセンターの共同販売コネクタ
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターの紹介を Salesforce CRM と同期します。 販売元は、CRM システム内から Microsoft と共同で販売することができます。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: 726e9071347e1590885b4bf82676f7767311f945
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173680"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="04db2-104">Salesforce CRM のための共同販売コネクタ - 概要</span><span class="sxs-lookup"><span data-stu-id="04db2-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="04db2-105">**適切なロール**: 紹介 admin |CRM のシステム管理者またはシステムカスタマイザー</span><span class="sxs-lookup"><span data-stu-id="04db2-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="04db2-106">パートナーセンターの共同販売コネクタを使用すると、販売元は CRM システム内から Microsoft と共同で販売することができます。</span><span class="sxs-lookup"><span data-stu-id="04db2-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="04db2-107">パートナーセンターを使用して共同販売取引を管理するためのトレーニングを行う必要はありません。</span><span class="sxs-lookup"><span data-stu-id="04db2-107">They won't have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="04db2-108">共同販売コネクタを使用して、Microsoft の販売者に連絡したり、Microsoft 販売者からの推薦を受け取ったり、紹介を受け入れたり拒否したりすることができます。また、商談の価値や決算日などの商談データを変更することもできます。</span><span class="sxs-lookup"><span data-stu-id="04db2-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="04db2-109">また、これらの共同販売取引に関するマイクロソフト販売者からの更新を受け取ることもできます。</span><span class="sxs-lookup"><span data-stu-id="04db2-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="04db2-110">パートナーセンターではなく、選択した CRM 内での作業中に、すべての紹介作業を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="04db2-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span>

<span data-ttu-id="04db2-111">このソリューションは、Microsoft Power Automate ソリューションに基づいており、パートナーセンター api を使用します。</span><span class="sxs-lookup"><span data-stu-id="04db2-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="04db2-112">をインストールする前に-前提条件</span><span class="sxs-lookup"><span data-stu-id="04db2-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="04db2-113">**トピック**</span><span class="sxs-lookup"><span data-stu-id="04db2-113">**Topics**</span></span>|<span data-ttu-id="04db2-114">**詳細**</span><span class="sxs-lookup"><span data-stu-id="04db2-114">**Details**</span></span>|<span data-ttu-id="04db2-115">**リンク**</span><span class="sxs-lookup"><span data-stu-id="04db2-115">**Links**</span></span>|
|--------------|--------------------|------|
|<span data-ttu-id="04db2-116">Microsoft Partner Network ID</span><span class="sxs-lookup"><span data-stu-id="04db2-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="04db2-117">有効な MPN ID が必要です</span><span class="sxs-lookup"><span data-stu-id="04db2-117">You need a valid MPN ID</span></span>|<span data-ttu-id="04db2-118">[MPN](https://partner.microsoft.com/)に参加するには</span><span class="sxs-lookup"><span data-stu-id="04db2-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="04db2-119">共同販売の準備完了</span><span class="sxs-lookup"><span data-stu-id="04db2-119">Co-sell ready</span></span>|<span data-ttu-id="04db2-120">お客様の IP/サービスソリューションは、共同販売の準備ができている必要があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="04db2-121">Microsoft との販売</span><span class="sxs-lookup"><span data-stu-id="04db2-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)|
|<span data-ttu-id="04db2-122">パートナー センター アカウント</span><span class="sxs-lookup"><span data-stu-id="04db2-122">Partner Center account</span></span>|<span data-ttu-id="04db2-123">パートナーセンターのテナントに関連付けられている MPN ID は、共同販売ソリューションに関連付けられている MPN ID と同じである必要があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="04db2-124">コネクタをデプロイする前に、パートナーセンターポータルで共同販売の紹介を確認できることを確認します。</span><span class="sxs-lookup"><span data-stu-id="04db2-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="04db2-125">アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="04db2-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="04db2-126">パートナー センターのユーザー ロール</span><span class="sxs-lookup"><span data-stu-id="04db2-126">Partner Center user roles</span></span>|<span data-ttu-id="04db2-127">コネクタをインストールして使用する従業員は、参照管理者である必要があります</span><span class="sxs-lookup"><span data-stu-id="04db2-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="04db2-128">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="04db2-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="04db2-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="04db2-129">Salesforce CRM</span></span>|<span data-ttu-id="04db2-130">CRM ユーザーロールは、システム管理者またはシステムカスタマイザーです。</span><span class="sxs-lookup"><span data-stu-id="04db2-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="04db2-131">Salesforce CRM でロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="04db2-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="04db2-132">Flow アカウントの Power Automate</span><span class="sxs-lookup"><span data-stu-id="04db2-132">Power Automate Flow Account</span></span>|<span data-ttu-id="04db2-133">テスト、ステージング、および運用のためのデータベースを使用して、新しい運用環境を作成します。</span><span class="sxs-lookup"><span data-stu-id="04db2-133">Create a new production environment with a database for testing, staging, and production.</span></span> <span data-ttu-id="04db2-134">データベースを含む既存の運用環境がある場合は、再利用できます。</span><span class="sxs-lookup"><span data-stu-id="04db2-134">If you have an existing production environment with a database, it can be reused.</span></span> <span data-ttu-id="04db2-135">コネクタソリューションをインストールするユーザーには、Power Automate ライセンスとこの環境へのアクセス権が必要です。</span><span class="sxs-lookup"><span data-stu-id="04db2-135">The user who's going to install the connector solution must have a Power Automate license and access to this environment.</span></span> <span data-ttu-id="04db2-136">インストールが失敗した場合は、進行状況を監視し、 [Power Automate](https://flow.microsoft.com/)の詳細情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="04db2-136">You can monitor the progress and get more information in [Power Automate](https://flow.microsoft.com/) if the installation fails.</span></span> <span data-ttu-id="04db2-137">[**ソリューション**] の [**履歴の表示**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-137">Select **See history** under **Solutions**.</span></span>|[<span data-ttu-id="04db2-138">環境の作成または管理</span><span class="sxs-lookup"><span data-stu-id="04db2-138">Create or manage environment</span></span>](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="04db2-139">Microsoft カスタムフィールド用の Salesforce パッケージのインストール</span><span class="sxs-lookup"><span data-stu-id="04db2-139">Installation of Salesforce Package for Microsoft Custom Fields</span></span>

<span data-ttu-id="04db2-140">パートナーセンターと Salesforce CRM 間で紹介を同期するには、Power Automate ソリューションで、Microsoft 固有の紹介フィールドを明確に識別する必要があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-140">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="04db2-141">このような境界は、パートナーの販売者チームが、共同販売のために Microsoft と共有する参照を決定する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="04db2-141">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="04db2-142">Salesforce で、 **メモ** をアクティブ化し、営業案件の関連リストに追加します。</span><span class="sxs-lookup"><span data-stu-id="04db2-142">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> [<span data-ttu-id="04db2-143">参照</span><span class="sxs-lookup"><span data-stu-id="04db2-143">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. <span data-ttu-id="04db2-144">次の手順に従って **営業案件チーム** をアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="04db2-144">Activate **Opportunity teams** by following the steps:</span></span>
    - <span data-ttu-id="04db2-145">セットアップで、[**クイック検索**] ボックスを使用して営業案件チームの設定を検索します。</span><span class="sxs-lookup"><span data-stu-id="04db2-145">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="04db2-146">必要に応じて設定を定義します。</span><span class="sxs-lookup"><span data-stu-id="04db2-146">Define the settings as needed.</span></span> [<span data-ttu-id="04db2-147">参照</span><span class="sxs-lookup"><span data-stu-id="04db2-147">Reference</span></span>](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. <span data-ttu-id="04db2-148">Salesforce で、 [パッケージインストーラー](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)を使用してカスタムフィールドおよびオブジェクトをインストールします。</span><span class="sxs-lookup"><span data-stu-id="04db2-148">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="04db2-149">このインストーラーを使用して、任意の会社にパッケージをインストールします。</span><span class="sxs-lookup"><span data-stu-id="04db2-149">Use this installer to install the package into any company.</span></span>

    >[!NOTE]
    ><span data-ttu-id="04db2-150">をサンドボックスにインストールする場合は、URL の最初の部分をに置き換える必要があり `http://test.salesforce.com` ます。</span><span class="sxs-lookup"><span data-stu-id="04db2-150">If you are installing into a sandbox, you must replace the initial portion of the URL with `http://test.salesforce.com`.</span></span>

1. <span data-ttu-id="04db2-151">Salesforce で、 **営業案件** 関連の一覧に Microsoft ソリューションを追加します。</span><span class="sxs-lookup"><span data-stu-id="04db2-151">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="04db2-152">追加したら、 **レンチ** アイコンを選択し、プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="04db2-152">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="04db2-153">ベストプラクティス: 運用前にテストする</span><span class="sxs-lookup"><span data-stu-id="04db2-153">Best Practice: Test before you go live</span></span>

<span data-ttu-id="04db2-154">運用環境で Power Automate ソリューションをインストール、構成、およびカスタマイズする前に、必ずステージング CRM インスタンスでソリューションをテストしてください。</span><span class="sxs-lookup"><span data-stu-id="04db2-154">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="04db2-155">Microsoft Power Automate ソリューションをステージング環境/CRM インスタンスにインストールします。</span><span class="sxs-lookup"><span data-stu-id="04db2-155">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="04db2-156">ソリューションのコピーを作成し、構成を実行して、ステージング環境でフローのカスタマイズを Power Automate します。</span><span class="sxs-lookup"><span data-stu-id="04db2-156">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="04db2-157">ステージング/CRM インスタンスでソリューションをテストします。</span><span class="sxs-lookup"><span data-stu-id="04db2-157">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="04db2-158">成功した場合は、運用インスタンスにマネージドソリューションとしてインポートします。</span><span class="sxs-lookup"><span data-stu-id="04db2-158">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="04db2-159">Salesforce CRM のパートナーセンターの紹介同期をインストールする</span><span class="sxs-lookup"><span data-stu-id="04db2-159">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="04db2-160">[Power Automate](https://flow.microsoft.com)にアクセスし、右上隅にある [**環境**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-160">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="04db2-161">これにより、使用可能な CRM インスタンスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-161">This will show you the available CRM instances.</span></span>

1. <span data-ttu-id="04db2-162">右上隅にあるドロップダウンリストから適切な CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-162">Select the appropriate CRM instance from the drop-down list in the upper-right corner.</span></span>

1. <span data-ttu-id="04db2-163">左側のナビゲーションバーで [ **ソリューション** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-163">Select **Solutions** on the left navigation bar.</span></span>

1. <span data-ttu-id="04db2-164">上部のメニューの [ **AppSource を開く** ] リンクを選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-164">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="AppSource を開きます。":::

1. <span data-ttu-id="04db2-166">ポップアップ画面で、 **Salesforce のパートナーセンターの紹介コネクタ** を検索します。</span><span class="sxs-lookup"><span data-stu-id="04db2-166">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="今すぐ入手できるスクリーンショットです。":::

1. <span data-ttu-id="04db2-168">[ **今すぐ入手** する] ボタンを選択し、[ **続行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-168">Select the **Get it now** button, and then select **Continue**.</span></span>

1. <span data-ttu-id="04db2-169">次のページで、アプリケーションをインストールする Salesforce CRM 環境を選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-169">In the next page, select the Salesforce CRM environment to install the application.</span></span> <span data-ttu-id="04db2-170">使用条件に同意します。</span><span class="sxs-lookup"><span data-stu-id="04db2-170">Agree to the terms and conditions.</span></span>

1. <span data-ttu-id="04db2-171">その後、[ **ソリューションの管理** ] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="04db2-171">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="04db2-172">ページの下部にある矢印ボタンを使用して、[パートナーセンターの紹介] に移動します。</span><span class="sxs-lookup"><span data-stu-id="04db2-172">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="04db2-173">[パートナーセンターの紹介] ソリューションの横に、[**インストールのスケジュール**] が表示されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-173">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="04db2-174">インストールには10-15 分かかります。</span><span class="sxs-lookup"><span data-stu-id="04db2-174">Installation will take 10-15 minutes.</span></span>

1. <span data-ttu-id="04db2-175">インストールが完了したら、[ [Power Automate](https://flow.microsoft.com)に戻り、[左側のナビゲーション領域] から [**ソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-175">After the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="04db2-176">[ソリューション] の一覧で、 **Salesforce のパートナーセンターの紹介同期** が使用できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="04db2-176">Notice that **Partner Center Referrals Synchronization for Salesforce** is now available in the Solutions list.</span></span>

1. <span data-ttu-id="04db2-177">**Salesforce のパートナーセンター紹介同期** を選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-177">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="04db2-178">次の Power Automate フローとエンティティを使用できます。</span><span class="sxs-lookup"><span data-stu-id="04db2-178">The following Power Automate flows and entities are available:</span></span>

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Salesforce フロー。":::

## <a name="configure-the-solution"></a><span data-ttu-id="04db2-180">ソリューションを構成する</span><span class="sxs-lookup"><span data-stu-id="04db2-180">Configure the solution</span></span>

1. <span data-ttu-id="04db2-181">CRM インスタンスにソリューションをインストールしたら、[ [Power Automate](https://flow.microsoft.com/)に戻ります。</span><span class="sxs-lookup"><span data-stu-id="04db2-181">After you've installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

1. <span data-ttu-id="04db2-182">右上隅にある [**環境**] ドロップダウンで、Power Automate ソリューションをインストールした CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-182">From the **Environments** drop-down in the upper-right corner, select the CRM instance where you installed the Power Automate solution.</span></span>

1. <span data-ttu-id="04db2-183">次の3つのユーザーアカウントを関連付ける接続を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-183">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="04db2-184">参照管理者の資格情報を持つパートナーセンターのユーザー</span><span class="sxs-lookup"><span data-stu-id="04db2-184">Partner Center user with referrals admin credentials</span></span>
   - <span data-ttu-id="04db2-185">パートナー センターのイベント</span><span class="sxs-lookup"><span data-stu-id="04db2-185">Partner Center Events</span></span>
   - <span data-ttu-id="04db2-186">ソリューション内の Power Automate フローを持つ CRM 管理者</span><span class="sxs-lookup"><span data-stu-id="04db2-186">CRM admin with the Power Automate flows in the solution</span></span>

   1. <span data-ttu-id="04db2-187">左側のナビゲーションバーから [ **接続** ] を選択し、一覧から [ **パートナーセンターの紹介** ] ソリューションを選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-187">Select **Connections** from the left navigation bar, and select the **Partner Center Referrals** solution from the list.</span></span>

   1. <span data-ttu-id="04db2-188">接続を作成するに **は、[接続の作成**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-188">Create a connection by selecting **Create a connection**.</span></span>

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="接続の作成を示すスクリーンショット。":::

   1. <span data-ttu-id="04db2-190">右上隅の検索バーで、 **パートナーセンターの参照 (プレビュー)** を検索します。</span><span class="sxs-lookup"><span data-stu-id="04db2-190">Search for **Partner Center Referrals (preview)** in the search bar in the upper-right corner.</span></span>

   1. <span data-ttu-id="04db2-191">参照管理者の資格情報ロールを使用して、パートナーセンターユーザーの接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="04db2-191">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   1. <span data-ttu-id="04db2-192">次に、パートナーセンターのユーザーに、参照管理者の資格情報を使用してパートナーセンターのイベント接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="04db2-192">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

   1. <span data-ttu-id="04db2-193">CRM 管理者ユーザーの Salesforce の接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="04db2-193">Create a connection for Salesforce for the CRM administrator user.</span></span>
  
   1. <span data-ttu-id="04db2-194">CRM 管理者ユーザーの Microsoft Dataverse 接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="04db2-194">Create a connection for Microsoft Dataverse for the CRM administrator user.</span></span>

   1. <span data-ttu-id="04db2-195">すべての接続を追加すると、環境内に次の接続が表示されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-195">After you've added all the Connections, you should see the following connections in your environment:</span></span>

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="接続を監視する方法を示すスクリーンショット。":::

### <a name="edit-the-connections"></a><span data-ttu-id="04db2-197">接続を編集する</span><span class="sxs-lookup"><span data-stu-id="04db2-197">Edit the connections</span></span>

1. <span data-ttu-id="04db2-198">[ **ソリューション** ] ページに戻り、[ **既定のソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-198">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="04db2-199">[**すべて**] をクリックして、[**接続の参照 (プレビュー)** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-199">Select **Connection Reference (preview)** by clicking **All**.</span></span>

   :::image type="content" source="images/connection-reference-video.gif" alt-text="接続の編集を示すスクリーンショット。":::

1. <span data-ttu-id="04db2-201">省略記号アイコンを選択して、各接続を個別に編集します。</span><span class="sxs-lookup"><span data-stu-id="04db2-201">Edit each of the Connections individually by selecting the ellipsis icon.</span></span> <span data-ttu-id="04db2-202">関連する接続を追加します。</span><span class="sxs-lookup"><span data-stu-id="04db2-202">Add the relevant connections.</span></span>

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="atht のスクリーンショットは、コネクタを編集する方法を示しています。":::

1. <span data-ttu-id="04db2-204">次の順序でフローを有効にする:</span><span class="sxs-lookup"><span data-stu-id="04db2-204">Turn on the flows in the following sequence:</span></span>
   - <span data-ttu-id="04db2-205">パートナー センター Webhook 登録 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="04db2-205">Partner Center Webhook Registration (Insider Preview)</span></span>
   - <span data-ttu-id="04db2-206">[カスタマイズ]Salesforce から詳細を作成または取得する</span><span class="sxs-lookup"><span data-stu-id="04db2-206">[Customize] Create or Get Details from Salesforce</span></span>
   - <span data-ttu-id="04db2-207">共同販売サービスをReferral-Salesforceするパートナー センター (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="04db2-207">Create Co-sell Referral-Salesforce to Partner Center (Insider Preview)</span></span>
   - <span data-ttu-id="04db2-208">パートナー センターに Microsoft 共同販売紹介の更新プログラムを追加する (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="04db2-208">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>  
   - <span data-ttu-id="04db2-209">パートナー センター Salesforce へのアクセス (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="04db2-209">Partner Center to Salesforce (Insider Preview)</span></span>
   - <span data-ttu-id="04db2-210">Salesforce から パートナー センター (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="04db2-210">Salesforce to Partner Center (Insider Preview)</span></span>
   - <span data-ttu-id="04db2-211">Salesforce Opportunity to パートナー センター (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="04db2-211">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
   - <span data-ttu-id="04db2-212">Salesforce Microsoft Solutions to パートナー センター (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="04db2-212">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="04db2-213">Webhook API を使用してリソース変更イベントに登録する</span><span class="sxs-lookup"><span data-stu-id="04db2-213">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="04db2-214">Webhook API パートナー センター使用して、リソース変更イベントに登録できます。</span><span class="sxs-lookup"><span data-stu-id="04db2-214">You can use the Partner Center webhook APIs to register for resource change events.</span></span> <span data-ttu-id="04db2-215">これらの変更イベントは、HTTP 投稿として URL に送信されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-215">These change events are sent to your URL as HTTP posts.</span></span>

1. <span data-ttu-id="04db2-216">[Salesforce **CRM パートナー センター (Insider Preview) にアクセスする] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="04db2-216">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

1. <span data-ttu-id="04db2-217">[編集] **アイコンを選択し** 、 **[HTTP 要求を受信した場合] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="04db2-217">Select the **Edit icon** and select **When an HTTP request is received**.</span></span>

1. <span data-ttu-id="04db2-218">[コピー] **アイコンを** 選択して、指定された **HTTP POST URL をコピーします**。</span><span class="sxs-lookup"><span data-stu-id="04db2-218">Select the **Copy** icon to copy the provided **HTTP POST URL**.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL をコピーする方法を示すスクリーンショット。":::

1. <span data-ttu-id="04db2-220">**[Webhook のパートナー センター (Insider Preview)** フローを選択しPower Automate実行] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="04db2-220">Select the **Partner Center Webhook Registration (Insider Preview)** Power Automate flow, and then select **Run**.</span></span>

1. <span data-ttu-id="04db2-221">右側のウィンドウで **[フローの実行** ] ウィンドウが開き、[続行] を選択 **します**。</span><span class="sxs-lookup"><span data-stu-id="04db2-221">Ensure that the **Run flow** window opens in the right pane, and select **Continue**.</span></span>

1. <span data-ttu-id="04db2-222">次の詳細を入力します。</span><span class="sxs-lookup"><span data-stu-id="04db2-222">Enter the following details:</span></span>

   - <span data-ttu-id="04db2-223">**Http トリガー エンドポイント**: この URL は、前の手順からコピーされました。</span><span class="sxs-lookup"><span data-stu-id="04db2-223">**Http Trigger Endpoint**: This URL was copied from an earlier step.</span></span>
   - <span data-ttu-id="04db2-224">**登録するイベント**: 使用可能なすべてのイベント (**紹介** で作成されたイベント、紹介が **更新** されたイベント、 **関連** する紹介で作成された イベント、および関連する紹介が更新された イベント) **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="04db2-224">**Events to Register**: Select all available events (**referral-created**, **referral-updated**, **related-referral-created**, and **related-referral-updated**).</span></span>
   - <span data-ttu-id="04db2-225">**既存のトリガー エンドポイントが存在する場合は上書きしますか?**: はい。</span><span class="sxs-lookup"><span data-stu-id="04db2-225">**Overwrite existing trigger endpoints if present?**: Yes.</span></span> <span data-ttu-id="04db2-226">特定の Webhook イベントに登録できる URL は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="04db2-226">Only one URL can be registered for a given webhook event.</span></span>

1. <span data-ttu-id="04db2-227">[フロー **の実行] を** 選択し、[完了] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="04db2-227">Select **Run flow**, and then select **Done**.</span></span>

<span data-ttu-id="04db2-228">Webhook は、イベントをリッスン、作成、および更新できます。</span><span class="sxs-lookup"><span data-stu-id="04db2-228">The webhook can now listen to, create, and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="04db2-229">同期手順をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="04db2-229">Customize synchronization steps</span></span>

<span data-ttu-id="04db2-230">CRM システムは高度にカスタマイズされ、CRM のセットアップにPower Automateソリューションをカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="04db2-230">CRM systems are highly customized, and you can customize the Power Automate solution based on your CRM setup.</span></span> <span data-ttu-id="04db2-231">パートナー センター と CRM システムの間で共同販売の紹介が同期される場合、パートナー センター PC で同期されるフィールドは、カスタム フィールド マッピング ガイド の一覧に [表示されます](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)。</span><span class="sxs-lookup"><span data-stu-id="04db2-231">When co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on the Partner Center PC are listed in the [Custom field mapping guide](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).</span></span>

<span data-ttu-id="04db2-232">フィールド マッピング ガイドに従い、必要に応じて、[カスタマイズ **] Salesforce** または環境変数から詳細を作成または取得するに関するページで適切な変更を行います。</span><span class="sxs-lookup"><span data-stu-id="04db2-232">Follow the field mapping guide, and if necessary, make appropriate changes in **[Customize] Create or Get Details from Salesforce** or environment variables.</span></span> <span data-ttu-id="04db2-233">将来のソリューションのアップグレードに影響を与える可能性Power Automateソリューション内の他のフローは更新しない。</span><span class="sxs-lookup"><span data-stu-id="04db2-233">Don't update any other flows in the Power Automate solution because it can affect future solution upgrades.</span></span>

<span data-ttu-id="04db2-234">次のカスタマイズを使用できます。</span><span class="sxs-lookup"><span data-stu-id="04db2-234">The following customizations are available:</span></span>

- <span data-ttu-id="04db2-235">**営業案件名に** チェック マークを表示する: 既定では、営業案件名の横にチェック マークが表示され、パートナー センター と Salesforce CRM の間の同期が正常に行っていることを示します。</span><span class="sxs-lookup"><span data-stu-id="04db2-235">**Display check mark in the opportunity name**: By default, a check mark will be displayed next to the opportunity name to indicate that synchronization between Partner Center and Salesforce CRM is happening successfully.</span></span> <span data-ttu-id="04db2-236">同様に、同期に失敗した場合はクロス マークが表示されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-236">Similarly, a cross mark will be displayed if synchronization fails.</span></span> <span data-ttu-id="04db2-237">営業案件名にチェック マークまたはクロス マークを追加しないようにするには、営業案件名環境変数の [表示] チェック マークの現在の値を [いいえ] に設定します。</span><span class="sxs-lookup"><span data-stu-id="04db2-237">To avoid adding a check or cross mark in the opportunity name, set the current value of the **Display check mark in the opportunity name** environment variable to No.</span></span>

- <span data-ttu-id="04db2-238">**ステージ名**:</span><span class="sxs-lookup"><span data-stu-id="04db2-238">**Stage name**:</span></span>

  - <span data-ttu-id="04db2-239">**アクティブなステージ** 名: Salesforce の営業案件の営業パイプラインのステージです。</span><span class="sxs-lookup"><span data-stu-id="04db2-239">**Active stage name**: This is the stage in an opportunity's sales pipeline in Salesforce.</span></span>  <span data-ttu-id="04db2-240">アクティブなステージを表し、アクティブなステージで受け入れ可能な状態の紹介とパートナー センター。</span><span class="sxs-lookup"><span data-stu-id="04db2-240">It represents an active stage and is equivalent to a referral in accepted state in Partner Center.</span></span> <span data-ttu-id="04db2-241">これは、オンホールド ステージの後の販売パイプラインの次のステージになります。</span><span class="sxs-lookup"><span data-stu-id="04db2-241">This can be the next stage in the sales pipeline after the on-hold stage.</span></span> <span data-ttu-id="04db2-242">営業案件の販売ステージを保留ステージからアクティブステージに移動すると、パートナー センター での紹介が受け入れされ、変更の同期が開始されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-242">Moving Opportunity's sales stage out of the on-hold stage into active stage will accept the referral in Partner Center and changes will start synchronizing.</span></span>

  - <span data-ttu-id="04db2-243">**保留ステージ名**: Salesforce の営業案件の営業パイプライン内のステージの名前。</span><span class="sxs-lookup"><span data-stu-id="04db2-243">**On-hold stage name**: Name of the stage in an opportunity's sales pipeline in Salesforce.</span></span> <span data-ttu-id="04db2-244">これは、保留ステージを表します。</span><span class="sxs-lookup"><span data-stu-id="04db2-244">It represents an on-hold stage.</span></span> <span data-ttu-id="04db2-245">まだ受け入れされていない Microsoft から共有される新しい共同販売紹介は、Salesforce のこのステージに設定されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-245">New co-sell referrals shared from Microsoft that are not yet accepted will be set to this stage in Salesforce.</span></span> <span data-ttu-id="04db2-246">保留ステージ中に営業案件に加えた変更は、その営業案件とパートナー センター。</span><span class="sxs-lookup"><span data-stu-id="04db2-246">Any changes made in an opportunity while it is on-hold stage will not synchronize to Partner Center.</span></span> <span data-ttu-id="04db2-247">この保留ステージから営業案件の販売ステージを移動すると、営業案件のパートナー センター受け入れ、変更の同期が開始されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-247">Moving Opportunity's sales stage out of this on-hold stage will accept the referral in Partner Center and changes will start synchronizing.</span></span>

- <span data-ttu-id="04db2-248">**顧客アカウントの国番号**: 新しい紹介を作成するときに、2 文字の国番号 (ISO 3166) を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-248">**Customer Account Country Code**: It is mandatory to provide a two-letter country code (ISO 3166) when you create a new referral.</span></span> <span data-ttu-id="04db2-249">既定では、国コードは Salesforce のアカウントの **BillingCountry** フィールドと同期されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-249">By default, the country code will be synced to and from the account's **BillingCountry** field in Salesforce.</span></span> <span data-ttu-id="04db2-250">同期する国コードの Salesforce に別のフィールドがある場合:</span><span class="sxs-lookup"><span data-stu-id="04db2-250">If you have a different field in Salesforce for the country code to sync from:</span></span>

  - <span data-ttu-id="04db2-251">2 文字のコードを含むアカウントの非lookup 国コード フィールドの場合:</span><span class="sxs-lookup"><span data-stu-id="04db2-251">For a nonlookup country code field in the account that contains a two-letter code:</span></span>

    - <span data-ttu-id="04db2-252">Salesforce 環境変数 **の Customer Account Country Code** フィールド名を CRM のフィールド名で更新します。</span><span class="sxs-lookup"><span data-stu-id="04db2-252">Update the **Customer Account Country Code** field name in the Salesforce environment variable with the CRM's field name.</span></span> <span data-ttu-id="04db2-253">表示名ではなく、フィールドの名前を指定してください。</span><span class="sxs-lookup"><span data-stu-id="04db2-253">Make sure that you provide the field's name, not its display name.</span></span>

    - <span data-ttu-id="04db2-254">[**カスタマイズ] Salesforce** の [作成] または [詳細の取得] を編集し、[CRMアクションで顧客アカウントを作成または取得する] に移動して **、CRM** の正しいフィールドに Country 値を割り当てる。</span><span class="sxs-lookup"><span data-stu-id="04db2-254">Edit **[Customize] Create or Get Details from Salesforce**, and go to **Create or get customer account in CRM** action to assign a **Country** value to the correct field in the CRM.</span></span> <span data-ttu-id="04db2-255">また、BillingCountry **から Country** 値の割 **り当てを削除します**。</span><span class="sxs-lookup"><span data-stu-id="04db2-255">Also, remove the **Country** value assignment from the **BillingCountry**.</span></span>

  - <span data-ttu-id="04db2-256">アカウントの参照ベースの国コード フィールドの場合:</span><span class="sxs-lookup"><span data-stu-id="04db2-256">For a lookup-based country code field in the account:</span></span>

    - <span data-ttu-id="04db2-257">アカウントに新しいカスタム フィールドを追加し、ルックアップ ベースのフィールドで選択した値に基づいて、2 文字の国コード (ISO 3166) を自動的に設定します。その逆も同様です。</span><span class="sxs-lookup"><span data-stu-id="04db2-257">Add a new custom field in the account, and auto-populate it with a two-letter country code (ISO 3166) based on the value selected in the lookup-based field and vice versa.</span></span>

    - <span data-ttu-id="04db2-258">非lookup 国コード フィールドの前の手順に従って、CRM の新しいカスタム フィールドと、その間で新しいカスタム フィールドを同期パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="04db2-258">Follow the preceding steps for the nonlookup country code field to sync a new custom field from the CRM to and from Partner Center.</span></span>

- <span data-ttu-id="04db2-259">**取引値**: 既定では、CRM の Amount パートナー センターとの間で同期されるトランザクションの **取引** 値。</span><span class="sxs-lookup"><span data-stu-id="04db2-259">**Deal value**: By default, the deal value from Partner Center will be synchronized to and from **Amount** in the CRM.</span></span> <span data-ttu-id="04db2-260">CRM に、取引値を同期する別のフィールドがある場合:</span><span class="sxs-lookup"><span data-stu-id="04db2-260">If you have a different field in the CRM for the deal value to synchronize from:</span></span>

  - <span data-ttu-id="04db2-261">Salesforce 環境変数 **の Deal 値** フィールド名を CRM のフィールド名で更新します。</span><span class="sxs-lookup"><span data-stu-id="04db2-261">Update the **Deal value** field name in the Salesforce environment variable with the CRM's field name.</span></span> <span data-ttu-id="04db2-262">表示名ではなく、フィールドの名前を指定してください。</span><span class="sxs-lookup"><span data-stu-id="04db2-262">Make sure that you provide the field's name, not its display name.</span></span>

  - <span data-ttu-id="04db2-263">**[カスタマイズ] Salesforce** から詳細を作成または取得し、[CRM での営業案件の作成または更新] に移動し、[新しい営業案件の作成] と [既存の営業案件の更新] アクションの両方を更新して、Salesforce の正しいフィールドに **DealValue** を割り当てる。</span><span class="sxs-lookup"><span data-stu-id="04db2-263">Edit **[Customize] Create or Get Details from Salesforce** and go to **Create or update opportunity** in CRM and update both **Create a new opportunity** and **Update existing opportunity** actions to assign the **DealValue** to the correct field in Salesforce.</span></span>

- <span data-ttu-id="04db2-264">**取引値の通貨コード**: Salesforce の取引価値通貨コード フィールドの名前。</span><span class="sxs-lookup"><span data-stu-id="04db2-264">**Deal value currency code**: Name of the deal value currency code field in Salesforce.</span></span> <span data-ttu-id="04db2-265">このフィールド API 名は、Microsoft パートナー センター で紹介を作成または更新するときに、営業案件の取引価値の通貨コードを取得するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-265">This field API name will be used to get Opportunity's deal value currency code when creating or updating referral in Microsoft Partner Center.</span></span> <span data-ttu-id="04db2-266">取引値の通貨コード フィールドが既定のフィールド **CurrencyIsoCode** と異なる場合は、この環境変数の現在の値を更新します。</span><span class="sxs-lookup"><span data-stu-id="04db2-266">If deal value currency code field is different than default field **CurrencyIsoCode**, update the current value of this environment variable.</span></span>

  - <span data-ttu-id="04db2-267">Salesforce 環境変数 **の Deal 値の通貨** フィールド名を CRM のフィールド名で更新します。</span><span class="sxs-lookup"><span data-stu-id="04db2-267">Update the **Deal value currency** field name in the Salesforce environment variable with the CRM's field name.</span></span> <span data-ttu-id="04db2-268">表示名ではなく、フィールドの名前を指定してください。</span><span class="sxs-lookup"><span data-stu-id="04db2-268">Make sure that you provide the field's name, not its display name.</span></span>

  - <span data-ttu-id="04db2-269">**[カスタマイズ] Salesforce** から詳細を作成または取得し、[CRM での営業案件の作成または更新] に移動し、[新しい営業案件の作成] と [既存の営業案件の更新] アクションの両方を更新して、Salesforce の正しいフィールドに **DealValueCurrency** を割り当てる。</span><span class="sxs-lookup"><span data-stu-id="04db2-269">Edit **[Customize] Create or Get Details from Salesforce** and go to **Create or update opportunity** in CRM and update both **Create a new opportunity** and **Update existing opportunity** actions to assign the **DealValueCurrency** to the correct field in Salesforce.</span></span>

- <span data-ttu-id="04db2-270">**[共同販売の** 機会の同期] : **[は** い] に設定すると、共同販売とパイプライン共有の営業案件だけが、パートナー センター Salesforce に同期されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-270">**Sync Co-sell opportunity**: If set to **yes**, only co-sell and pipeline sharing opportunities will be synchronized from Partner Center to Salesforce.</span></span> <span data-ttu-id="04db2-271">[いいえ] **に設定** すると、リード、共同販売、パイプライン共有の機会が、パートナー センター Salesforce に同期されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-271">If set to **no**, leads, co-sell, and pipeline sharing opportunities will be synchronized from Partner Center to Salesforce.</span></span> <span data-ttu-id="04db2-272">この変数は、Salesforce から パートナー センター に同期される機会には影響を与パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="04db2-272">This variable does not have any impact on the opportunities synchronized from Salesforce to Partner Center.</span></span>

## <a name="update-environment-variable"></a><span data-ttu-id="04db2-273">環境変数を更新する</span><span class="sxs-lookup"><span data-stu-id="04db2-273">Update environment variable</span></span>

<span data-ttu-id="04db2-274">環境変数の値を更新するには:</span><span class="sxs-lookup"><span data-stu-id="04db2-274">To update an environment variable value:</span></span>

1. <span data-ttu-id="04db2-275">[ソリューション] ページ **に移動** し、[既定のソリューション] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="04db2-275">Go to the **Solutions** page, and select **Default Solution**.</span></span> <span data-ttu-id="04db2-276">[すべて **] を選択** して[環境変数] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="04db2-276">Select **Environment Variable** by selecting **All**.</span></span>

1. <span data-ttu-id="04db2-277">更新する必要がある値の環境変数を選択し、省略記号アイコンを使用して [編集] を選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-277">Select the environment variable for the value that needs to be updated, and select **Edit** by using the ellipsis icon.</span></span>

1. <span data-ttu-id="04db2-278">[**新しい値]** オプションを **使用して値** を指定して、現在の値を更新します (既定値は更新されません)。</span><span class="sxs-lookup"><span data-stu-id="04db2-278">Update **Current Value** (don't update **Default Value**) by using the **New value** option and providing the value.</span></span> <span data-ttu-id="04db2-279">値は、変数のデータ型と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-279">The value must match the data type of the variable.</span></span> <span data-ttu-id="04db2-280">たとえば、 [はい] または [いいえ] のデータ型は、[はい] または [いいえ] の値を受け入れる場合があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-280">For example, the Yes or No data type will accept either the Yes or No value.</span></span>

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="環境変数の更新を示すスクリーンショット。":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="04db2-282">エンドツーエンドの双方向の共同販売紹介の同期</span><span class="sxs-lookup"><span data-stu-id="04db2-282">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="04db2-283">Power Automate ソリューションをインストール、構成、カスタマイズしたら、Salesforce CRM と パートナー センター の間で共同販売紹介の同期をテストできます。</span><span class="sxs-lookup"><span data-stu-id="04db2-283">After you've installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="04db2-284">前提条件</span><span class="sxs-lookup"><span data-stu-id="04db2-284">Pre-requisites</span></span>

<span data-ttu-id="04db2-285">パートナー センター と Salesforce CRM 間で紹介を同期するには、Power Automate ソリューションで Microsoft 固有の紹介フィールドを明確に定義する必要があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-285">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="04db2-286">この識別により、販売者チームは、共同販売のために Microsoft と共有する紹介を決定できます。</span><span class="sxs-lookup"><span data-stu-id="04db2-286">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="04db2-287">カスタム フィールドのセットは、Salesforce CRM ソリューション営業案件パートナー センターの参照同期の一部として **使用** できます。</span><span class="sxs-lookup"><span data-stu-id="04db2-287">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="04db2-288">CRM 管理者ユーザーは、営業案件のカスタム フィールドを含む別の CRM セクション **を作成する** 必要があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-288">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="04db2-289">次のカスタム フィールドは CRM セクションの一部である必要があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-289">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="04db2-290">**[同期] パートナー センター:** 営業案件を他のユーザーと同期パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="04db2-290">**Sync with Partner Center**: Whether to sync the opportunity with Partner Center.</span></span> <span data-ttu-id="04db2-291">既定では、このフィールドの値は [いいえ] で、Microsoft と営業案件を共有するには、販売者が明示的に [はい] に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-291">By default, the value of this field is No and needs to be explicitly set to Yes by your seller to share an opportunity with Microsoft.</span></span> <span data-ttu-id="04db2-292">CRM から CRM に共有されるパートナー センター、このフィールドの値は [はい] に設定されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-292">New referrals shared from Partner Center to CRM will have this field value set to Yes.</span></span>

- <span data-ttu-id="04db2-293">**紹介識別子**: Microsoft の参照用の読み取りパートナー センターフィールド。</span><span class="sxs-lookup"><span data-stu-id="04db2-293">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral.</span></span>

- <span data-ttu-id="04db2-294">**紹介リンク**: Microsoft サービスの紹介への読み取りパートナー センター。</span><span class="sxs-lookup"><span data-stu-id="04db2-294">**Referral Link**: A read-only link to the referral in Microsoft Partner Center.</span></span>

- <span data-ttu-id="04db2-295">**Microsoft がどのように役立つのか**: 紹介に必要な Microsoft からのヘルプ。</span><span class="sxs-lookup"><span data-stu-id="04db2-295">**How can Microsoft help**: Help required from Microsoft for the referral.</span></span> <span data-ttu-id="04db2-296">共同販売の紹介を作成するには、Microsoft に必要な適切なヘルプを選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-296">To create a co-sell referral, select the appropriate help required from Microsoft.</span></span> <span data-ttu-id="04db2-297">顧客の連絡先は、共同販売の紹介を作成する機会に関連付けられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-297">A customer contact must be associated to the opportunity to create a co-sell referral.</span></span> <span data-ttu-id="04db2-298">共同販売以外の紹介を作成するには、このフィールドを選択しない必要があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-298">To create a non-co-sell referral, don't select this field.</span></span> <span data-ttu-id="04db2-299">共同販売以外の紹介は、ヘルプが必要な適切なオプションを選択することで、いつでも共同販売の紹介に変換できます。</span><span class="sxs-lookup"><span data-stu-id="04db2-299">A non-co-sell referral can be converted to a co-sell referral anytime by selecting the appropriate help-required option.</span></span>

- <span data-ttu-id="04db2-300">**Microsoft パートナー センターの参照の可視性**: 参照の表示を選択パートナー センターします。</span><span class="sxs-lookup"><span data-stu-id="04db2-300">**Microsoft Partner Center Referral Visibility**: Select visibility for the Partner Center referral.</span></span> <span data-ttu-id="04db2-301">Microsoft の販売者に表示することで、共同販売以外の紹介が共同販売に変換される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-301">By making it visible to Microsoft sellers, a non-co-sell referral might get converted to co-sell.</span></span> <span data-ttu-id="04db2-302">Microsoft のヘルプが必要な場合、紹介は既定で Microsoft 販売者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-302">When Microsoft help is required, the referral is visible to Microsoft sellers by default.</span></span> <span data-ttu-id="04db2-303">このフィールドが表示済みとしてマークされた後は、元に戻す必要があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-303">After this field is marked as visible, it can't be reverted.</span></span>

- <span data-ttu-id="04db2-304">**Microsoft CRM識別子**: 共同販売の紹介が作成され、Microsoft によって受け入れられると、このフィールドに Microsoft の CRM 識別子が入力されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-304">**Microsoft CRM Identifier**: When a co-sell referral is created and accepted by Microsoft, this field will get populated with Microsoft's CRM identifier.</span></span>

- <span data-ttu-id="04db2-305">**Microsoft パートナー センター ソリューション**: 共同販売対応ソリューションまたは Microsoft ソリューションを機会に関連付けるカスタム オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="04db2-305">**Microsoft Partner Center Solutions**: A custom object to associate co-sell ready solutions or Microsoft solutions with the opportunity.</span></span> <span data-ttu-id="04db2-306">1 つ以上のソリューションを営業案件に追加または削除できます。</span><span class="sxs-lookup"><span data-stu-id="04db2-306">One or more solutions can be added or removed from the opportunity.</span></span> <span data-ttu-id="04db2-307">Microsoft と共有する前に、営業案件に少なくとも 1 つの共同販売準備完了または Microsoft ソリューションを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-307">It's mandatory to add at least one co-sell ready or Microsoft solution to the opportunity before you share it with Microsoft.</span></span> <span data-ttu-id="04db2-308">このオブジェクトを営業案件に関連付けるには、CRM の **営業案件** フォームを更新します。</span><span class="sxs-lookup"><span data-stu-id="04db2-308">To associate this object to the opportunity, update the **Opportunity** form in the CRM.</span></span>

- <span data-ttu-id="04db2-309">**監査**: 参照と同期する読み取り専用パートナー センター証跡</span><span class="sxs-lookup"><span data-stu-id="04db2-309">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="04db2-310">シナリオ</span><span class="sxs-lookup"><span data-stu-id="04db2-310">SCENARIOS</span></span>

1. <span data-ttu-id="04db2-311">CRM で紹介が作成または更新され、次の方法で同期された場合の紹介パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="04db2-311">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="04db2-312">CRM の [営業案件] セクションに表示されているユーザーを使用して、Salesforce CRM **環境に** サインインします。</span><span class="sxs-lookup"><span data-stu-id="04db2-312">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   1. <span data-ttu-id="04db2-313">Salesforce CRM 環境で新しい営業案件 **を作成パートナー センター、** セクション [Microsoft **パートナー センター]** が存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="04db2-313">Ensure that the section, **Microsoft Partner Center** is present when you create a **New Opportunity** in Salesforce CRM environment.</span></span>

   1. <span data-ttu-id="04db2-314">Salesforce CRM の [パートナー センター] アイコンを使用して、✔に同期された案件が特定されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-314">Opportunities that are synchronized successfully with Partner Center will be identified with ✔ icon in Salesforce CRM.</span></span>
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Salesforce 環境のスクリーンショット。":::

   1. <span data-ttu-id="04db2-316">この機会を Microsoft パートナー センター と同期するには、カード ビューで次のフィールドを設定してください。</span><span class="sxs-lookup"><span data-stu-id="04db2-316">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="04db2-317">**Microsoft が支援する方法:** 共同販売の紹介を作成するには、適切なヘルプ オプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-317">**How can Microsoft help?**: To create a co-sell referral, select an appropriate help option.</span></span>

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="カード ビューで適切なフィールドを取得する方法を示すスクリーンショット。":::

      - <span data-ttu-id="04db2-319">**[同期と同期パートナー センター:** はい</span><span class="sxs-lookup"><span data-stu-id="04db2-319">**Sync with Partner Center**: Yes</span></span>
      - <span data-ttu-id="04db2-320">**顧客の連絡先**: 共同販売の紹介を作成するには、営業案件に顧客の連絡先を追加します。</span><span class="sxs-lookup"><span data-stu-id="04db2-320">**Customer contact**: To create a co-sell referral, add a customer contact to the opportunity.</span></span>
      - <span data-ttu-id="04db2-321">**Microsoft ソリューション**: Microsoft と紹介を共有するには、有効な共同販売準備完了または Microsoft ソリューションを営業案件に追加します。</span><span class="sxs-lookup"><span data-stu-id="04db2-321">**Microsoft Solutions**: To share a referral with Microsoft, add a valid co-sell ready or Microsoft solution to the opportunity.</span></span>

   1. <span data-ttu-id="04db2-322">[Sync with パートナー センター] オプションを [はい]**に設定した後**、10 分間待ち、自分のアカウントパートナー センターします。</span><span class="sxs-lookup"><span data-stu-id="04db2-322">After you have set the opportunity **Sync with Partner Center** option to **Yes**, wait for 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="04db2-323">紹介は Salesforce CRM と同期され、紹介リンクが設定されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-323">Your referrals will be synchronized with Salesforce CRM, and Referral Link will get populated.</span></span> <span data-ttu-id="04db2-324">エラーが発生した場合は、[監査] フィールドにエラー情報が入力されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-324">If there's a failure, the Audit field will be populated with error information.</span></span>

   1. <span data-ttu-id="04db2-325">同様に、[**パートナー センター と** 同期する ] オプションが [はい] に設定されている場合は、Salesforce CRM で営業案件を更新すると、変更は パートナー センター アカウントと同期されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-325">Similarly, when the **Sync with Partner Center** option is set to **Yes**, if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

2. <span data-ttu-id="04db2-326">Microsoft パートナー センターで紹介が作成または更新され、Salesforce CRM 環境で同期された場合の紹介の同期:</span><span class="sxs-lookup"><span data-stu-id="04db2-326">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="04db2-327">ダッシュボード にサインインパートナー センター [します](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="04db2-327">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    1. <span data-ttu-id="04db2-328">左側 **のメニューから** [紹介] を選択します。</span><span class="sxs-lookup"><span data-stu-id="04db2-328">Select **Referrals** from the left-hand menu.</span></span>

    1. <span data-ttu-id="04db2-329">[新しい取引] オプションをクリックパートナー センター新しい共同販売紹介を作成します。</span><span class="sxs-lookup"><span data-stu-id="04db2-329">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    1. <span data-ttu-id="04db2-330">Salesforce CRM 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="04db2-330">Sign into your Salesforce CRM environment.</span></span>

    1. <span data-ttu-id="04db2-331">[Open **Opportunities] に移動します**。</span><span class="sxs-lookup"><span data-stu-id="04db2-331">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="04db2-332">Microsoft パートナー センターで作成された紹介は、Salesforce CRM で同期されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-332">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

    1. <span data-ttu-id="04db2-333">同期された紹介を選択すると、カード ビューの詳細が設定されます。</span><span class="sxs-lookup"><span data-stu-id="04db2-333">When you select a synchronized referral, the card view details are populated.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Salesforce 営業案件ページのスクリーンショット。":::

>[!NOTE]
><span data-ttu-id="04db2-335">**デプロイに関するヘルプが必要ですか?**</span><span class="sxs-lookup"><span data-stu-id="04db2-335">**Need help with deployment?**</span></span>
><span data-ttu-id="04db2-336">共同販売紹介コネクタのデプロイに関するサポートについては、パートナー テクニカル コンサルタントに問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="04db2-336">For assistance with your Co-sell referral connector deployment, you can engage a Partner Technical Consultant.</span></span> <span data-ttu-id="04db2-337">実装を成功に向け、デプロイのサポートとベスト プラクティスを提供できます。</span><span class="sxs-lookup"><span data-stu-id="04db2-337">They can provide deployment assistance and best practices for a successful implementation.</span></span>
>
><span data-ttu-id="04db2-338">詳細については、「技術プリ [セールスおよびデプロイ サービス要求を送信する方法」を参照してください。](technical-benefits.md)</span><span class="sxs-lookup"><span data-stu-id="04db2-338">For more information, see [How to Submit a technical presales and deployment services request](technical-benefits.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="04db2-339">次のステップ</span><span class="sxs-lookup"><span data-stu-id="04db2-339">Next steps</span></span>

- [<span data-ttu-id="04db2-340">見込み客を管理する</span><span class="sxs-lookup"><span data-stu-id="04db2-340">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="04db2-341">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="04db2-341">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="04db2-342">パートナー センター Webhook</span><span class="sxs-lookup"><span data-stu-id="04db2-342">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
