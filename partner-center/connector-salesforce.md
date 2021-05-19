---
title: Salesforce CRM サービスの共同販売パートナー センター
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Salesforce CRM を使用して、パートナー センターの紹介を同期します。 その後、販売者は CRM システム内から Microsoft と共同販売できます。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: fa9b35343e1251cfce5caff107de8dff344f4e68
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148416"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="d4285-104">Salesforce CRM のための共同販売コネクタ - 概要</span><span class="sxs-lookup"><span data-stu-id="d4285-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="d4285-105">**適切なロール**: 紹介管理者|CRM のシステム管理者またはシステム カスタマイザー</span><span class="sxs-lookup"><span data-stu-id="d4285-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="d4285-106">パートナー センター共同販売コネクタを使用すると、販売者は CRM システム内から Microsoft と共同販売できます。</span><span class="sxs-lookup"><span data-stu-id="d4285-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="d4285-107">共同販売の取引を管理するためにパートナー センタートレーニングする必要は" は"ない"。</span><span class="sxs-lookup"><span data-stu-id="d4285-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="d4285-108">共同販売コネクタを使用すると、新しい共同販売の紹介を作成して、Microsoft 販売者を引き付け、Microsoft 販売者から紹介を受け取り、紹介を受け入れる/拒否したり、取引価値や終了日などの取引データを変更することができます。</span><span class="sxs-lookup"><span data-stu-id="d4285-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="d4285-109">これらの共同販売取引については、Microsoft 販売者から更新プログラムを受け取る場合があります。</span><span class="sxs-lookup"><span data-stu-id="d4285-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="d4285-110">すべての紹介作業は、お客様が選択した CRM 内で作業する際に、お客様が行パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="d4285-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="d4285-111">このソリューションは Microsoft Power Automate Solution に基づいており、パートナー センター API を使用します。</span><span class="sxs-lookup"><span data-stu-id="d4285-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="d4285-112">インストールする前に - 前提条件</span><span class="sxs-lookup"><span data-stu-id="d4285-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="d4285-113">**トピック**</span><span class="sxs-lookup"><span data-stu-id="d4285-113">**Topics**</span></span>   |<span data-ttu-id="d4285-114">**詳細**</span><span class="sxs-lookup"><span data-stu-id="d4285-114">**Details**</span></span>   |<span data-ttu-id="d4285-115">**リンク**</span><span class="sxs-lookup"><span data-stu-id="d4285-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="d4285-116">Microsoft Partner Network ID</span><span class="sxs-lookup"><span data-stu-id="d4285-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="d4285-117">有効な MPN ID が必要です</span><span class="sxs-lookup"><span data-stu-id="d4285-117">You need a valid MPN ID</span></span>|<span data-ttu-id="d4285-118">[MPN に参加する方法](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="d4285-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="d4285-119">共同販売の準備完了</span><span class="sxs-lookup"><span data-stu-id="d4285-119">Co-sell ready</span></span>|<span data-ttu-id="d4285-120">IP/サービス ソリューションは共同販売の準備ができている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d4285-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="d4285-121">Microsoft で販売する</span><span class="sxs-lookup"><span data-stu-id="d4285-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="d4285-122">パートナー センター アカウント</span><span class="sxs-lookup"><span data-stu-id="d4285-122">Partner Center account</span></span>|<span data-ttu-id="d4285-123">共同販売ソリューションに関連付パートナー センター MPN ID は、共同販売ソリューションに関連付けられている MPN ID と同じである必要があります。</span><span class="sxs-lookup"><span data-stu-id="d4285-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="d4285-124">コネクタをデプロイする前に、ポータルで共同販売パートナー センター確認してください。</span><span class="sxs-lookup"><span data-stu-id="d4285-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="d4285-125">アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="d4285-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="d4285-126">パートナー センターのユーザー ロール</span><span class="sxs-lookup"><span data-stu-id="d4285-126">Partner Center user roles</span></span>|<span data-ttu-id="d4285-127">コネクタをインストールして使用する従業員は、紹介管理者である必要があります</span><span class="sxs-lookup"><span data-stu-id="d4285-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="d4285-128">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="d4285-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="d4285-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="d4285-129">Salesforce CRM</span></span>|<span data-ttu-id="d4285-130">CRM ユーザーロールは、システム管理者またはシステムカスタマイザーです。</span><span class="sxs-lookup"><span data-stu-id="d4285-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="d4285-131">Salesforce CRM でロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="d4285-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="d4285-132">パワー自動化フローアカウント</span><span class="sxs-lookup"><span data-stu-id="d4285-132">Power Automate Flow Account</span></span>|<span data-ttu-id="d4285-133">CRM システム管理者またはシステムカスタマイザー用のアクティブな [電源自動化](https://flow.microsoft.com) アカウント。</span><span class="sxs-lookup"><span data-stu-id="d4285-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="d4285-134">そのユーザーは、インストールの前に少なくとも1回、 [電源の自動](https://flow.microsoft.com) 登録を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="d4285-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="d4285-135">Microsoft カスタムフィールド用の Salesforce パッケージのインストール</span><span class="sxs-lookup"><span data-stu-id="d4285-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="d4285-136">パートナーセンターと Salesforce CRM 間で紹介を同期するために、Power solution の自動化ソリューションでは、Microsoft 固有の紹介フィールドを明確に識別する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d4285-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="d4285-137">このような境界は、パートナーの販売者チームが、共同販売のために Microsoft と共有する参照を決定する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="d4285-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="d4285-138">Salesforce で、 **メモ** をアクティブ化し、営業案件の関連リストに追加します。</span><span class="sxs-lookup"><span data-stu-id="d4285-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="d4285-139">参照</span><span class="sxs-lookup"><span data-stu-id="d4285-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="d4285-140">次の手順に従って **営業案件チーム** をアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="d4285-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="d4285-141">セットアップで、[ **クイック検索** ] ボックスを使用して営業案件チームの設定を検索します。</span><span class="sxs-lookup"><span data-stu-id="d4285-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="d4285-142">必要に応じて設定を定義します。</span><span class="sxs-lookup"><span data-stu-id="d4285-142">Define the settings as needed.</span></span>
[<span data-ttu-id="d4285-143">参照</span><span class="sxs-lookup"><span data-stu-id="d4285-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="d4285-144">Salesforce で、 [パッケージインストーラー](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)を使用してカスタムフィールドおよびオブジェクトをインストールします。</span><span class="sxs-lookup"><span data-stu-id="d4285-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="d4285-145">これを使用して、任意の会社にパッケージをインストールします。</span><span class="sxs-lookup"><span data-stu-id="d4285-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="d4285-146">サンドボックスにをインストールする場合は、URL の最初の部分をに置き換える必要があります。 http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="d4285-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="d4285-147">Salesforce で、 **営業案件** 関連の一覧に Microsoft ソリューションを追加します。</span><span class="sxs-lookup"><span data-stu-id="d4285-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="d4285-148">追加したら、 **レンチ** アイコンを選択し、プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d4285-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="d4285-149">ベストプラクティス: 運用前にテストする</span><span class="sxs-lookup"><span data-stu-id="d4285-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="d4285-150">運用環境でパワー自動化ソリューションをインストール、構成、およびカスタマイズする前に、必ずステージング CRM インスタンスでソリューションをテストしてください。</span><span class="sxs-lookup"><span data-stu-id="d4285-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="d4285-151">ステージング環境/CRM インスタンスに Microsoft Power 自動ソリューションをインストールします。</span><span class="sxs-lookup"><span data-stu-id="d4285-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="d4285-152">ソリューションのコピーを作成し、構成を実行しPower Automate環境でフローのカスタマイズを実行します。</span><span class="sxs-lookup"><span data-stu-id="d4285-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="d4285-153">ステージング/CRM インスタンスでソリューションをテストします。</span><span class="sxs-lookup"><span data-stu-id="d4285-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="d4285-154">成功した場合は、マネージド ソリューションとして実稼働インスタンスにインポートします。</span><span class="sxs-lookup"><span data-stu-id="d4285-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="d4285-155">Salesforce CRM パートナー センター参照同期をインストールする</span><span class="sxs-lookup"><span data-stu-id="d4285-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="d4285-156">[環境] [Power Automate](https://flow.microsoft.com) に移動し、右上隅 **にある** [環境] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="d4285-157">これにより、使用可能な CRM インスタンスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="d4285-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="d4285-158">右上隅のドロップダウンから適切な CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="d4285-159">左側の **ナビゲーション バー** で [ソリューション] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="d4285-160">上部の **メニューの [AppSource** を開く] リンクを選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource を開く":::

5. <span data-ttu-id="d4285-162">ポップアップ画面 **パートナー センターで Salesforce** の紹介コネクタを検索します。</span><span class="sxs-lookup"><span data-stu-id="d4285-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="d4285-164">[今すぐ **取得] ボタンを選択** し、[ 続行] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="d4285-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="d4285-165">これにより、Salesforce CRM 環境を選択してアプリケーションをインストールできるページが開きます。</span><span class="sxs-lookup"><span data-stu-id="d4285-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="d4285-166">使用条件に同意します。</span><span class="sxs-lookup"><span data-stu-id="d4285-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="利用可能な CRM":::

8. <span data-ttu-id="d4285-168">その後、[ソリューションの管理 **] ページに移動** します。</span><span class="sxs-lookup"><span data-stu-id="d4285-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="d4285-169">ページの下部パートナー センター矢印ボタンを使用して、[紹介] に移動します。</span><span class="sxs-lookup"><span data-stu-id="d4285-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="d4285-170">**[紹介]** ソリューションの横に、スケジュールパートナー センターインストールが表示されます。</span><span class="sxs-lookup"><span data-stu-id="d4285-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="d4285-171">インストールには 10 から 15 分かかります。</span><span class="sxs-lookup"><span data-stu-id="d4285-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="d4285-172">インストールが完了したら、[ソリューション] に戻り [Power Automate](https://flow.microsoft.com) 左側のナビゲーション領域から [ **ソリューション** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="d4285-173">**Salesforce のパートナーセンターの紹介同期** は、[ソリューション] の一覧で確認できます。</span><span class="sxs-lookup"><span data-stu-id="d4285-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="d4285-174">**Salesforce のパートナーセンター紹介同期** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="d4285-175">次の電源の自動化フローとエンティティを利用できます。</span><span class="sxs-lookup"><span data-stu-id="d4285-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce フロー":::



## <a name="configure-the-solution"></a><span data-ttu-id="d4285-177">ソリューションを構成する</span><span class="sxs-lookup"><span data-stu-id="d4285-177">Configure the solution</span></span>

1. <span data-ttu-id="d4285-178">CRM インスタンスにソリューションをインストールしたら、[ [Power の自動化](https://flow.microsoft.com/)] に戻ります。</span><span class="sxs-lookup"><span data-stu-id="d4285-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="d4285-179">右上隅にある [ **環境** ] ドロップダウンで、パワー自動化ソリューションをインストールした CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="d4285-180">次の3つのユーザーアカウントを関連付ける接続を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d4285-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="d4285-181">参照管理者の資格情報を持つパートナーセンターのユーザー</span><span class="sxs-lookup"><span data-stu-id="d4285-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="d4285-182">パートナー センターのイベント</span><span class="sxs-lookup"><span data-stu-id="d4285-182">Partner Center Events</span></span>
    - <span data-ttu-id="d4285-183">Power を使用した CRM 管理ソリューションのフローが自動化されます。</span><span class="sxs-lookup"><span data-stu-id="d4285-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="d4285-184">左側のナビゲーションバーから [ **接続** ] を選択し、一覧から "パートナーセンターの紹介" ソリューションを選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="d4285-185">[ **接続の作成**] をクリックして接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="d4285-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="接続を作成する":::

- <span data-ttu-id="d4285-187">右上隅の検索バーで、パートナーセンターの参照 (プレビュー) を検索します。</span><span class="sxs-lookup"><span data-stu-id="d4285-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="d4285-188">参照管理者の資格情報ロールを使用して、パートナーセンターユーザーの接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="d4285-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="d4285-189">次に、パートナーセンターのユーザーに、参照管理者の資格情報を使用してパートナーセンターのイベント接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="d4285-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="d4285-190">CRM 管理者ユーザーの Salesforce の接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="d4285-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="d4285-191">すべての接続を追加すると、環境内に次の接続が表示されます。</span><span class="sxs-lookup"><span data-stu-id="d4285-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="接続を監視する":::

### <a name="edit-the-connections"></a><span data-ttu-id="d4285-193">接続を編集する</span><span class="sxs-lookup"><span data-stu-id="d4285-193">Edit the connections</span></span>

1. <span data-ttu-id="d4285-194">[ソリューション] ページに戻り、[ **既定のソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="d4285-195">[**すべて**] をクリックして、[**接続の参照 (プレビュー)** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="コネクタの編集を開始します":::

2. <span data-ttu-id="d4285-197">3つのドットアイコンを選択して、各接続を個別に編集します。</span><span class="sxs-lookup"><span data-stu-id="d4285-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="d4285-198">関連する接続を追加します。</span><span class="sxs-lookup"><span data-stu-id="d4285-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="コネクタの編集":::

3. <span data-ttu-id="d4285-200">次の順序でフローを有効にします。</span><span class="sxs-lookup"><span data-stu-id="d4285-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="d4285-201">パートナーセンターの Webhook の登録 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d4285-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="d4285-202">パートナーセンターへの共同販売参照の作成-Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d4285-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="d4285-203">パートナーセンター: Microsoft 共同での Salesforce の参照の更新 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d4285-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="d4285-204">パートナーセンターから Salesforce へ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d4285-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="d4285-205">Salesforce からパートナーセンターへ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d4285-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="d4285-206">パートナーセンターへの Salesforce の営業案件 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d4285-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="d4285-207">パートナーセンターへの Salesforce Microsoft ソリューション (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="d4285-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="d4285-208">Webhook Api を使用してリソース変更イベントに登録する</span><span class="sxs-lookup"><span data-stu-id="d4285-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="d4285-209">パートナーセンターの Webhook Api を使用すると、リソース変更イベントに登録できます。</span><span class="sxs-lookup"><span data-stu-id="d4285-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="d4285-210">これらの変更イベントは、HTTP 投稿として url に送信されます。</span><span class="sxs-lookup"><span data-stu-id="d4285-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="d4285-211">Url を登録するには、 **パートナーセンターの Webhook 登録 (Insider Preview)** パワー自動化フローを選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="d4285-212">参照管理者の資格情報を持つパートナーセンターのユーザー (a.) に接続を追加します。パートナーセンターのイベントは、下に強調表示されています。</span><span class="sxs-lookup"><span data-stu-id="d4285-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="トリガー":::

3. <span data-ttu-id="d4285-214">これらの更新を行うと、次のように表示されます。</span><span class="sxs-lookup"><span data-stu-id="d4285-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="d4285-216">変更内容を保存し、[ **有効にする**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="d4285-217">パートナーセンターの webhook でイベントの変更をリッスンできるようにするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="d4285-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="d4285-218">[Salesforce **CRM パートナー センター (Insider Preview) にアクセスする] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="d4285-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="d4285-219">[編集] **アイコンを** 選択し **、[HTTP 要求を受信した場合] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="d4285-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="d4285-220">[コピー] **アイコン** を選択して、指定された HTTP POST URL をコピーします。</span><span class="sxs-lookup"><span data-stu-id="d4285-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL のコピー":::

8. <span data-ttu-id="d4285-222">次に、"パートナー センター Webhook 登録 (Insider Preview)" フローを選択しPower Automateを選択 **します**。</span><span class="sxs-lookup"><span data-stu-id="d4285-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="d4285-223">右側のウィンドウで [フローの実行] ウィンドウが開き、[続行] を選択 **します**。</span><span class="sxs-lookup"><span data-stu-id="d4285-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="d4285-224">次の詳細を入力します。</span><span class="sxs-lookup"><span data-stu-id="d4285-224">Enter the following details:</span></span>

    1. <span data-ttu-id="d4285-225">**Http トリガー エンドポイント**: 前の手順からコピーした URL</span><span class="sxs-lookup"><span data-stu-id="d4285-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="d4285-226">**登録するイベント**: "紹介作成" と "紹介更新"</span><span class="sxs-lookup"><span data-stu-id="d4285-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="d4285-227">**存在する場合は既存のトリガー エンドポイントを上書** きする: はい (既存のエンドポイントが上書きされます)。</span><span class="sxs-lookup"><span data-stu-id="d4285-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="d4285-228">[実行 **] を選択** し、[完了] **を選択します。**</span><span class="sxs-lookup"><span data-stu-id="d4285-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="d4285-229">Webhook は、イベントの作成と更新をリッスンできます。</span><span class="sxs-lookup"><span data-stu-id="d4285-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="d4285-230">同期手順をカスタマイズする</span><span class="sxs-lookup"><span data-stu-id="d4285-230">Customize synchronization steps</span></span>

<span data-ttu-id="d4285-231">パートナー センター と CRM システムの間で共同販売の紹介が同期される場合、パートナー センター PC で同期されるフィールドがここに一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="d4285-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="d4285-232">多くの場合、CRM システムは高度にカスタマイズされています。</span><span class="sxs-lookup"><span data-stu-id="d4285-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="d4285-233">データ フローをカスタマイズPower Automateできます。</span><span class="sxs-lookup"><span data-stu-id="d4285-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="d4285-234">フィールド マッピング ガイドに従い、必要に応じて、データ フローの手順で適切な変更Power Automateします。</span><span class="sxs-lookup"><span data-stu-id="d4285-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="d4285-235">Microsoft パートナー センターから CRM へのマッピングが提供されますが、CRM 環境に基づいて、フィールドをさらにカスタマイズすることもできます。</span><span class="sxs-lookup"><span data-stu-id="d4285-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="d4285-236">各フローの複数のステップPower Automateニーズに基づいてカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="d4285-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="d4285-237">使用可能なカスタマイズの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d4285-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="d4285-238">CRM 参照同期を使用して、パートナー センターイベントのフィールドをカスタマイズするには:</span><span class="sxs-lookup"><span data-stu-id="d4285-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="d4285-239">[Salesforce CRM パートナー センター (Insider Preview) にアクセスする] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="d4285-240">[ **編集** ] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="d4285-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="d4285-241">選択 **(スコープ) 潜在顧客または営業案件を同期** します。</span><span class="sxs-lookup"><span data-stu-id="d4285-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="d4285-242">作成イベントの CRM フィールドマッピングをカスタマイズするには、[ **新しい共有の営業案件]、[**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="d4285-243">[ **はい] の場合** はサブステップを選択し、 **CRM で [新しい営業案件の作成**] を展開します。</span><span class="sxs-lookup"><span data-stu-id="d4285-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="d4285-244">このセクションでマッピングを編集するには、[フィールドマッピングガイド] を使用します。</span><span class="sxs-lookup"><span data-stu-id="d4285-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="d4285-245">更新イベントの CRM フィールドマッピングをカスタマイズするには、[(スコープ) 潜在顧客または営業案件を同期する] ステップを選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="d4285-246">**営業案件の更新である場合は、** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="d4285-247">[ **はい] の場合** はサブステップを選択し、 **パートナーセンターと CRM の営業案件オブジェクト間の差異がある場合は**[] を展開します。</span><span class="sxs-lookup"><span data-stu-id="d4285-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="d4285-248">**既存の営業案件を更新** する場合は、[**はい]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="d4285-249">更新イベントの CRM から PC への参照同期のフィールドをカスタマイズするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="d4285-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="d4285-250">[ **編集**  ] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="d4285-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="d4285-251">[ **(スコープ)] を選択して、営業案件を同期** します。</span><span class="sxs-lookup"><span data-stu-id="d4285-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="d4285-252">更新イベントの CRM フィールドマッピング (フィールドマッピングガイドに基づく) をカスタマイズする場合は、 **パートナーセンターと CRM の潜在顧客オブジェクトが異なるかどうか** を選択してから、を選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="d4285-253">[ **はい] の場合** はサブステップを選択し、[ **営業案件データを使用して紹介を更新する**] ステップを展開します。</span><span class="sxs-lookup"><span data-stu-id="d4285-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="d4285-254">このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。</span><span class="sxs-lookup"><span data-stu-id="d4285-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="d4285-255">Create events の CRM to PC 参照同期のフィールドをカスタマイズするには</span><span class="sxs-lookup"><span data-stu-id="d4285-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="d4285-256">[ **編集**  ] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="d4285-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="d4285-257">**参照の同期を選択 (スコープ) します。**</span><span class="sxs-lookup"><span data-stu-id="d4285-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="d4285-258">[イベントの作成] で (フィールドマッピングガイドに基づいて) CRM フィールドマッピングをカスタマイズする場合は、[ **Microsoft の紹介を作成する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="d4285-259">このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。</span><span class="sxs-lookup"><span data-stu-id="d4285-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="d4285-260">エンドツーエンドの双方向の共同販売紹介の同期</span><span class="sxs-lookup"><span data-stu-id="d4285-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="d4285-261">Power Automate ソリューションをインストール、構成、カスタマイズしたら、Salesforce CRM と パートナー センター の間で共同販売紹介の同期をテストできます。</span><span class="sxs-lookup"><span data-stu-id="d4285-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="d4285-262">前提条件</span><span class="sxs-lookup"><span data-stu-id="d4285-262">Pre-requisites</span></span>

<span data-ttu-id="d4285-263">パートナー センター と Salesforce CRM 間で紹介を同期するには、Power Automate ソリューションで Microsoft 固有の紹介フィールドを明確に定義する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d4285-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="d4285-264">この識別により、販売者チームは、共同販売のために Microsoft と共有する紹介を決定できます。</span><span class="sxs-lookup"><span data-stu-id="d4285-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="d4285-265">カスタム フィールドのセットは、Salesforce CRM ソリューション営業案件パートナー センターの参照同期の一部として **使用** できます。</span><span class="sxs-lookup"><span data-stu-id="d4285-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="d4285-266">CRM 管理者ユーザーは、営業案件のカスタム フィールドを含む別の CRM セクション **を作成する** 必要があります。</span><span class="sxs-lookup"><span data-stu-id="d4285-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="d4285-267">次のカスタム フィールドは CRM セクションの一部である必要があります。</span><span class="sxs-lookup"><span data-stu-id="d4285-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="d4285-268">**[同期パートナー センター:** 営業案件を Microsoft パートナー センター と同期するかどうか</span><span class="sxs-lookup"><span data-stu-id="d4285-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="d4285-269">**紹介識別子**: Microsoft の参照用の読み取りパートナー センターフィールド</span><span class="sxs-lookup"><span data-stu-id="d4285-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="d4285-270">**紹介リンク**: Microsoft パートナー センター の紹介への読み取り専用パートナー センター</span><span class="sxs-lookup"><span data-stu-id="d4285-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="d4285-271">**Microsoft がどのように役立つのか**: 紹介に必要な Microsoft からのヘルプ</span><span class="sxs-lookup"><span data-stu-id="d4285-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="d4285-272">**製品**: この営業案件に関連付けられている製品の一覧</span><span class="sxs-lookup"><span data-stu-id="d4285-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="d4285-273">**監査**: 参照と同期する読み取り専用パートナー センター証跡</span><span class="sxs-lookup"><span data-stu-id="d4285-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="d4285-274">シナリオ：</span><span class="sxs-lookup"><span data-stu-id="d4285-274">SCENARIOS:</span></span>

1. <span data-ttu-id="d4285-275">CRM で紹介が作成または更新され、次の方法で同期された場合の紹介パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="d4285-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="d4285-276">CRM の [営業案件] セクションに表示されているユーザーを使用して、Salesforce CRM **環境に** サインインします。</span><span class="sxs-lookup"><span data-stu-id="d4285-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="d4285-277">Salesforce CRM 環境で "新しい営業案件" を作成するときに、次のセクションが存在する必要があります</span><span class="sxs-lookup"><span data-stu-id="d4285-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 環境":::

   3. <span data-ttu-id="d4285-279">この機会を Microsoft パートナー センター と同期するには、カード ビューで次のフィールドを設定してください。</span><span class="sxs-lookup"><span data-stu-id="d4285-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="d4285-280">"Sync with パートナー センター": はい</span><span class="sxs-lookup"><span data-stu-id="d4285-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="d4285-281">「Microsoft がどのように役立つか」: 次のオプションから選択してください。</span><span class="sxs-lookup"><span data-stu-id="d4285-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="d4285-282">製品: 製品のソリューション Id</span><span class="sxs-lookup"><span data-stu-id="d4285-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="d4285-283">[営業案件  **とパートナーセンターの同期** ] オプションを **[はい]** に設定したら、10分待ってから、パートナーセンターアカウントにサインインします。</span><span class="sxs-lookup"><span data-stu-id="d4285-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="d4285-284">参照は、Salesforce CRM と同期されます。</span><span class="sxs-lookup"><span data-stu-id="d4285-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="d4285-285">[パートナーセンターとの同期] オプションが [はい] に設定されている場合、Salesforce CRM で営業案件を更新すると、変更がパートナーセンターアカウントと同期されます。</span><span class="sxs-lookup"><span data-stu-id="d4285-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="d4285-286">パートナーセンターで正常に同期された営業案件は、Salesforce CRM の✔アイコンで識別されます。</span><span class="sxs-lookup"><span data-stu-id="d4285-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="d4285-287">Microsoft パートナーセンターで参照が作成または更新され、Salesforce CRM 環境で同期される場合の紹介の同期:</span><span class="sxs-lookup"><span data-stu-id="d4285-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="d4285-288">パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="d4285-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="d4285-289">左側のメニューから [ **紹介** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="d4285-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="d4285-290">[新しい取引] オプションをクリックして、パートナーセンターから新しい共同販売紹介を作成します。</span><span class="sxs-lookup"><span data-stu-id="d4285-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="d4285-291">Salesforce CRM 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="d4285-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="d4285-292">**[Open opportunity**] に移動します。</span><span class="sxs-lookup"><span data-stu-id="d4285-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="d4285-293">Microsoft パートナーセンターで作成された紹介が、Salesforce CRM で同期されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="d4285-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce の営業案件画面":::

    6. <span data-ttu-id="d4285-295">同期された参照を選択すると、カードビューの詳細が設定されます。</span><span class="sxs-lookup"><span data-stu-id="d4285-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d4285-296">次のステップ</span><span class="sxs-lookup"><span data-stu-id="d4285-296">Next steps</span></span>

- [<span data-ttu-id="d4285-297">見込み客を管理する</span><span class="sxs-lookup"><span data-stu-id="d4285-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="d4285-298">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="d4285-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="d4285-299">パートナー センター Webhook</span><span class="sxs-lookup"><span data-stu-id="d4285-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
