---
title: Salesforce CRM パートナーセンターの共同販売コネクタ
ms.topic: how-to
ms.date: 09/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターの紹介を Salesforce CRM と同期します。 販売元は、CRM システム内から Microsoft と共同で販売することができます。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 4b3817dafbd05edf0c50b062b52ac4814c767d04
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031465"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="505ac-104">Salesforce CRM のための共同販売コネクタ - 概要</span><span class="sxs-lookup"><span data-stu-id="505ac-104">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="505ac-105">適切なロール</span><span class="sxs-lookup"><span data-stu-id="505ac-105">Appropriate roles</span></span>

- <span data-ttu-id="505ac-106">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="505ac-106">Referrals admin</span></span>
- <span data-ttu-id="505ac-107">CRM のシステム管理者またはシステムカスタマイザー</span><span class="sxs-lookup"><span data-stu-id="505ac-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="505ac-108">パートナーセンターの共同販売コネクタを使用すると、販売元は CRM システム内から Microsoft と共同で販売することができます。</span><span class="sxs-lookup"><span data-stu-id="505ac-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="505ac-109">パートナーセンターを使用して共同販売取引を管理するためのトレーニングを行う必要はありません。</span><span class="sxs-lookup"><span data-stu-id="505ac-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="505ac-110">共同販売コネクタを使用して、Microsoft の販売者に連絡したり、Microsoft 販売者からの推薦を受け取ったり、紹介を受け入れたり拒否したりすることができます。また、商談の価値や決算日などの商談データを変更することもできます。</span><span class="sxs-lookup"><span data-stu-id="505ac-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="505ac-111">また、これらの共同販売取引に関するマイクロソフト販売者からの更新を受け取ることもできます。</span><span class="sxs-lookup"><span data-stu-id="505ac-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="505ac-112">パートナーセンターではなく、選択した CRM 内での作業中に、すべての紹介作業を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="505ac-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="505ac-113">このソリューションは、Microsoft のパワー自動化ソリューションに基づいており、パートナーセンター Api を使用しています。</span><span class="sxs-lookup"><span data-stu-id="505ac-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="505ac-114">をインストールする前に-前提条件</span><span class="sxs-lookup"><span data-stu-id="505ac-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="505ac-115">**トピック**</span><span class="sxs-lookup"><span data-stu-id="505ac-115">**Topics**</span></span>   |<span data-ttu-id="505ac-116">**詳細**</span><span class="sxs-lookup"><span data-stu-id="505ac-116">**Details**</span></span>   |<span data-ttu-id="505ac-117">**リンク**</span><span class="sxs-lookup"><span data-stu-id="505ac-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="505ac-118">Microsoft Partner Network ID</span><span class="sxs-lookup"><span data-stu-id="505ac-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="505ac-119">有効な MPN ID が必要です</span><span class="sxs-lookup"><span data-stu-id="505ac-119">You need a valid MPN ID</span></span>|<span data-ttu-id="505ac-120">[MPN](https://partner.microsoft.com/)に参加するには</span><span class="sxs-lookup"><span data-stu-id="505ac-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="505ac-121">共同販売の準備完了</span><span class="sxs-lookup"><span data-stu-id="505ac-121">Co-sell ready</span></span>|<span data-ttu-id="505ac-122">お客様の IP/サービスソリューションは、共同販売の準備ができている必要があります。</span><span class="sxs-lookup"><span data-stu-id="505ac-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="505ac-123">Microsoft との販売</span><span class="sxs-lookup"><span data-stu-id="505ac-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="505ac-124">パートナー センター アカウント</span><span class="sxs-lookup"><span data-stu-id="505ac-124">Partner Center account</span></span>|<span data-ttu-id="505ac-125">パートナーセンターのテナントに関連付けられている MPN ID は、共同販売ソリューションに関連付けられている MPN ID と同じである必要があります。</span><span class="sxs-lookup"><span data-stu-id="505ac-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="505ac-126">コネクタをデプロイする前に、パートナーセンターポータルで共同販売の紹介を確認できることを確認します。</span><span class="sxs-lookup"><span data-stu-id="505ac-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="505ac-127">アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="505ac-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="505ac-128">パートナー センターのユーザー ロール</span><span class="sxs-lookup"><span data-stu-id="505ac-128">Partner Center user roles</span></span>|<span data-ttu-id="505ac-129">コネクタをインストールして使用する従業員は、参照管理者である必要があります</span><span class="sxs-lookup"><span data-stu-id="505ac-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="505ac-130">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="505ac-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="505ac-131">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="505ac-131">Salesforce CRM</span></span>|<span data-ttu-id="505ac-132">CRM ユーザーロールは、システム管理者またはシステムカスタマイザーです。</span><span class="sxs-lookup"><span data-stu-id="505ac-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="505ac-133">Salesforce CRM でロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="505ac-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="505ac-134">パワー自動化フローアカウント</span><span class="sxs-lookup"><span data-stu-id="505ac-134">Power Automate Flow Account</span></span>|<span data-ttu-id="505ac-135">CRM システム管理者またはシステムカスタマイザー用のアクティブな [電源自動化](https://flow.microsoft.com) アカウント。</span><span class="sxs-lookup"><span data-stu-id="505ac-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="505ac-136">そのユーザーは、インストールの前に少なくとも1回、 [電源の自動](https://flow.microsoft.com) 登録を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="505ac-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="505ac-137">Microsoft カスタムフィールド用の Salesforce パッケージのインストール</span><span class="sxs-lookup"><span data-stu-id="505ac-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="505ac-138">パートナーセンターと Salesforce CRM 間で紹介を同期するために、Power solution の自動化ソリューションでは、Microsoft 固有の参照フィールドを明確に識別する必要があります。</span><span class="sxs-lookup"><span data-stu-id="505ac-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="505ac-139">このような境界は、パートナーの販売者チームが、共同販売のために Microsoft と共有する参照を決定する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="505ac-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="505ac-140">Salesforce で、 **メモ** をアクティブ化し、営業案件の関連リストに追加します。</span><span class="sxs-lookup"><span data-stu-id="505ac-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="505ac-141">参照</span><span class="sxs-lookup"><span data-stu-id="505ac-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="505ac-142">次の手順に従って **営業案件チーム** をアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="505ac-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="505ac-143">セットアップで、[ **クイック検索** ] ボックスを使用して営業案件チームの設定を検索します。</span><span class="sxs-lookup"><span data-stu-id="505ac-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="505ac-144">必要に応じて設定を定義します。</span><span class="sxs-lookup"><span data-stu-id="505ac-144">Define the settings as needed.</span></span>
[<span data-ttu-id="505ac-145">参照</span><span class="sxs-lookup"><span data-stu-id="505ac-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="505ac-146">Salesforce で、次のパッケージインストーラーを使用して、カスタムフィールドとオブジェクトをインストールします。</span><span class="sxs-lookup"><span data-stu-id="505ac-146">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="505ac-147">任意の会社にパッケージをインストールするには、 [ここ](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) を参照してください:</span><span class="sxs-lookup"><span data-stu-id="505ac-147">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) to install the package into any company:</span></span>


<span data-ttu-id="505ac-148">注: をサンドボックスにインストールする場合は、URL の最初の部分を次のように置き換える必要があります。 http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="505ac-148">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="505ac-149">Salesforce で、 **営業案件** 関連の一覧に Microsoft ソリューションを追加します。</span><span class="sxs-lookup"><span data-stu-id="505ac-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="505ac-150">追加したら、 **レンチ** アイコンをクリックし、プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="505ac-150">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="505ac-151">ベストプラクティス: 運用前にテストする</span><span class="sxs-lookup"><span data-stu-id="505ac-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="505ac-152">運用環境でパワー自動化ソリューションをインストール、構成、およびカスタマイズする前に、必ずステージング CRM インスタンスでソリューションをテストしてください。</span><span class="sxs-lookup"><span data-stu-id="505ac-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="505ac-153">ステージング環境/CRM インスタンスに Microsoft Power 自動ソリューションをインストールします。</span><span class="sxs-lookup"><span data-stu-id="505ac-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="505ac-154">ソリューションのコピーを作成し、構成を実行して、ステージング環境でフローのカスタマイズを自動化します。</span><span class="sxs-lookup"><span data-stu-id="505ac-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="505ac-155">ステージング/CRM インスタンスでソリューションをテストします。</span><span class="sxs-lookup"><span data-stu-id="505ac-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="505ac-156">成功した場合は、運用インスタンスにマネージドソリューションとしてインポートします。</span><span class="sxs-lookup"><span data-stu-id="505ac-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="505ac-157">Salesforce CRM のパートナーセンターの紹介同期をインストールする</span><span class="sxs-lookup"><span data-stu-id="505ac-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="505ac-158">[ [パワー自動化](https://flow.microsoft.com) ] にアクセスし、右上隅にある [ **環境** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="505ac-159">これにより、使用可能な CRM インスタンスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="505ac-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="505ac-160">右上隅にあるドロップダウンから適切な CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="505ac-161">左側のナビゲーションバーで [ **ソリューション** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="505ac-162">上部のメニューの [ **AppSource を開く** ] リンクをクリックします。</span><span class="sxs-lookup"><span data-stu-id="505ac-162">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource を開く":::

5. <span data-ttu-id="505ac-164">ポップアップ画面で、 **Salesforce のパートナーセンターの紹介コネクタ** を検索します。</span><span class="sxs-lookup"><span data-stu-id="505ac-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="AppSource を開く":::

6. <span data-ttu-id="505ac-166">[ **今すぐ入手** する] ボタンをクリックし、[ **続行**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="505ac-166">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="505ac-167">これにより、Salesforce CRM 環境を選択してアプリケーションをインストールできるページが開きます。</span><span class="sxs-lookup"><span data-stu-id="505ac-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="505ac-168">使用条件に同意します。</span><span class="sxs-lookup"><span data-stu-id="505ac-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="AppSource を開く":::

8. <span data-ttu-id="505ac-170">その後、[ **ソリューションの管理** ] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="505ac-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="505ac-171">ページの下部にある矢印ボタンを使用して、[パートナーセンターの紹介] に移動します。</span><span class="sxs-lookup"><span data-stu-id="505ac-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="505ac-172">[パートナーセンターの紹介] ソリューションの横に、[**インストールのスケジュール**] が表示されます。</span><span class="sxs-lookup"><span data-stu-id="505ac-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="505ac-173">インストールには10-15 分かかります。</span><span class="sxs-lookup"><span data-stu-id="505ac-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="505ac-174">インストールが完了したら、[Power の [自動化](https://flow.microsoft.com) ] に戻り、左側のナビゲーション領域から [ **ソリューション** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="505ac-175">**Salesforce のパートナーセンターの紹介同期**は、[ソリューション] の一覧で確認できます。</span><span class="sxs-lookup"><span data-stu-id="505ac-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="505ac-176">**Salesforce のパートナーセンター紹介同期**を選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="505ac-177">次の電源の自動化フローとエンティティを利用できます。</span><span class="sxs-lookup"><span data-stu-id="505ac-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="AppSource を開く":::



## <a name="configure-the-solution"></a><span data-ttu-id="505ac-179">ソリューションを構成する</span><span class="sxs-lookup"><span data-stu-id="505ac-179">Configure the solution</span></span>

1. <span data-ttu-id="505ac-180">CRM インスタンスにソリューションをインストールしたら、[ [Power の自動化](https://flow.microsoft.com/)] に戻ります。</span><span class="sxs-lookup"><span data-stu-id="505ac-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="505ac-181">右上隅にある [ **環境** ] ドロップダウンで、パワー自動化ソリューションをインストールした CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="505ac-182">次の3つのユーザーアカウントを関連付ける接続を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="505ac-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="505ac-183">参照管理者の資格情報を持つパートナーセンターのユーザー</span><span class="sxs-lookup"><span data-stu-id="505ac-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="505ac-184">パートナー センターのイベント</span><span class="sxs-lookup"><span data-stu-id="505ac-184">Partner Center Events</span></span>
    - <span data-ttu-id="505ac-185">Power を使用した CRM 管理ソリューションのフローが自動化されます。</span><span class="sxs-lookup"><span data-stu-id="505ac-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="505ac-186">左側のナビゲーションバーから [ **接続** ] を選択し、一覧から "パートナーセンターの紹介" ソリューションを選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="505ac-187">[ **接続の作成**] をクリックして接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="505ac-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="AppSource を開く":::

- <span data-ttu-id="505ac-189">右上隅の検索バーで、パートナーセンターの参照 (プレビュー) を検索します。</span><span class="sxs-lookup"><span data-stu-id="505ac-189">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="505ac-190">参照管理者の資格情報ロールを使用して、パートナーセンターユーザーの接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="505ac-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="505ac-191">次に、パートナーセンターのユーザーに、参照管理者の資格情報を使用してパートナーセンターのイベント接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="505ac-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="505ac-192">CRM 管理者ユーザーの Common Data Service (現在の環境) の接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="505ac-192">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

-  <span data-ttu-id="505ac-193">すべての接続を追加すると、環境内に次の接続が表示されます。</span><span class="sxs-lookup"><span data-stu-id="505ac-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="AppSource を開く":::

### <a name="edit-the-connections"></a><span data-ttu-id="505ac-195">接続を編集する</span><span class="sxs-lookup"><span data-stu-id="505ac-195">Edit the connections</span></span>

1. <span data-ttu-id="505ac-196">[ソリューション] ページに戻り、[ **既定のソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="505ac-197">[**すべて**] をクリックして、[**接続の参照 (プレビュー)** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="AppSource を開く":::

2. <span data-ttu-id="505ac-199">3つのドットアイコンを選択して、各接続を1つずつ編集します。</span><span class="sxs-lookup"><span data-stu-id="505ac-199">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="505ac-200">関連する接続を追加します。</span><span class="sxs-lookup"><span data-stu-id="505ac-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="AppSource を開く":::

3. <span data-ttu-id="505ac-202">次の順序でフローを有効にします。</span><span class="sxs-lookup"><span data-stu-id="505ac-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="505ac-203">パートナーセンターの Webhook の登録 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="505ac-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="505ac-204">パートナーセンターへの共同販売参照の作成-Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="505ac-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="505ac-205">パートナーセンター: Microsoft 共同での Salesforce の参照の更新 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="505ac-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="505ac-206">パートナーセンターから Salesforce へ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="505ac-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="505ac-207">Salesforce からパートナーセンターへ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="505ac-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="505ac-208">パートナーセンターへの Salesforce の営業案件 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="505ac-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="505ac-209">パートナーセンターへの Salesforce Microsoft ソリューション (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="505ac-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="505ac-210">Webhook Api を使用してリソース変更イベントに登録する</span><span class="sxs-lookup"><span data-stu-id="505ac-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="505ac-211">パートナーセンターの Webhook Api を使用すると、リソース変更イベントに登録できます。</span><span class="sxs-lookup"><span data-stu-id="505ac-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="505ac-212">これらの変更イベントは、HTTP 投稿として url に送信されます。</span><span class="sxs-lookup"><span data-stu-id="505ac-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="505ac-213">Url を登録するには、 **パートナーセンターの Webhook 登録 (Insider Preview)** パワー自動化フローを選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="505ac-214">参照管理者の資格情報を持つパートナーセンターのユーザー (a.) に接続を追加します。パートナーセンターのイベントは、下に強調表示されています。</span><span class="sxs-lookup"><span data-stu-id="505ac-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="AppSource を開く":::

3. <span data-ttu-id="505ac-216">これらの更新を行うと、次のように表示されます。</span><span class="sxs-lookup"><span data-stu-id="505ac-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="AppSource を開く":::

4. <span data-ttu-id="505ac-218">変更内容を保存し、[ **有効にする**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="505ac-219">パートナーセンターの webhook でイベントの変更をリッスンできるようにするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="505ac-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="505ac-220">[ **パートナーセンター] を**選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="505ac-221">[ **編集** ] アイコンを選択し、[ **HTTP 要求の受信時**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="505ac-222">**コピー**アイコンを選択して、指定された HTTP POST URL をコピーします。</span><span class="sxs-lookup"><span data-stu-id="505ac-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="AppSource を開く":::

8. <span data-ttu-id="505ac-224">次に、"パートナーセンターの Webhook の登録 (Insider Preview)" パワー自動化フローを選択し、[ **実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="505ac-225">右側のウィンドウで [実行フロー] ウィンドウが開いていることを確認し、[ **続行**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="505ac-225">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="505ac-226">次の詳細を入力します。</span><span class="sxs-lookup"><span data-stu-id="505ac-226">Enter the following details:</span></span>

    1. <span data-ttu-id="505ac-227">**Http トリガーエンドポイント**: 前の手順からコピーされた URL</span><span class="sxs-lookup"><span data-stu-id="505ac-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="505ac-228">**登録するイベント**: "紹介-作成" と "参照-更新"</span><span class="sxs-lookup"><span data-stu-id="505ac-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="505ac-229">**既存のトリガーエンドポイントがある場合は上書き**します (存在する場合は既存のエンドポイントを上書きします)。</span><span class="sxs-lookup"><span data-stu-id="505ac-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="505ac-230">[ **実行** ] を選択し、[完了] を選択し **ます。**</span><span class="sxs-lookup"><span data-stu-id="505ac-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="505ac-231">Webhook は、イベントの作成と更新をリッスンできるようになりました。</span><span class="sxs-lookup"><span data-stu-id="505ac-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="505ac-232">同期手順のカスタマイズ</span><span class="sxs-lookup"><span data-stu-id="505ac-232">Customize synchronization steps</span></span>

<span data-ttu-id="505ac-233">パートナーセンターと CRM システムの間で共同販売参照が同期されると、パートナーセンター PC で同期されるフィールドがここに表示されます。</span><span class="sxs-lookup"><span data-stu-id="505ac-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="505ac-234">多くの場合、CRM システムは高度にカスタマイズされています。</span><span class="sxs-lookup"><span data-stu-id="505ac-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="505ac-235">パワー自動化フローをカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="505ac-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="505ac-236">フィールドマッピングガイドに従って、必要に応じて、パワー自動化フローの手順に適切な変更を加えます。</span><span class="sxs-lookup"><span data-stu-id="505ac-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="505ac-237">Microsoft パートナーセンターから CRM へのマッピングが提供されますが、CRM 環境に基づいて、フィールドをさらにカスタマイズすることもできます。</span><span class="sxs-lookup"><span data-stu-id="505ac-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="505ac-238">各パワー自動化フローの複数の手順は、ニーズに応じてカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="505ac-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="505ac-239">使用可能なカスタマイズの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="505ac-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="505ac-240">パートナーセンターで作成または更新イベントのフィールドを CRM の参照同期にカスタマイズするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="505ac-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="505ac-241">[パートナーセンター] を選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="505ac-242">[ **編集** ] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="505ac-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="505ac-243">選択 **(スコープ) 潜在顧客または営業案件を同期**します。</span><span class="sxs-lookup"><span data-stu-id="505ac-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="505ac-244">作成イベントの CRM フィールドマッピングをカスタマイズするには、[ **新しい共有の営業案件]、[**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="505ac-245">[ **はい] の場合** はサブステップを選択し、 **CRM で [新しい営業案件の作成**] を展開します。</span><span class="sxs-lookup"><span data-stu-id="505ac-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="505ac-246">このセクションでマッピングを編集するには、[フィールドマッピングガイド] を使用します。</span><span class="sxs-lookup"><span data-stu-id="505ac-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="505ac-247">更新イベントの CRM フィールドマッピングをカスタマイズするには、[(スコープ) 潜在顧客または営業案件を同期する] ステップをクリックします。</span><span class="sxs-lookup"><span data-stu-id="505ac-247">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="505ac-248">**営業案件の更新である場合は、** を選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="505ac-249">[サブステップ **if yes]** を選択し、次に **パートナーセンターと CRM の営業案件オブジェクト間の差異がある場合**は、を展開します。</span><span class="sxs-lookup"><span data-stu-id="505ac-249">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="505ac-250">**既存の営業案件を更新**する場合は、[**はい]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="505ac-251">更新イベントの CRM から PC への参照同期のフィールドをカスタマイズするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="505ac-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="505ac-252">[ **編集**  ] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="505ac-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="505ac-253">[ **(スコープ)] を選択して、営業案件を同期**します。</span><span class="sxs-lookup"><span data-stu-id="505ac-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="505ac-254">更新イベントの CRM フィールドマッピング (フィールドマッピングガイドに基づく) をカスタマイズする場合は、 **パートナーセンターと CRM の潜在顧客オブジェクトが異なるかどうか**を選択してから、を選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="505ac-255">[ **はい] の場合** はサブステップを選択し、[ **営業案件データを使用して紹介を更新する**] ステップを展開します。</span><span class="sxs-lookup"><span data-stu-id="505ac-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="505ac-256">このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。</span><span class="sxs-lookup"><span data-stu-id="505ac-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="505ac-257">Create events の CRM to PC 参照同期のフィールドをカスタマイズするには</span><span class="sxs-lookup"><span data-stu-id="505ac-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="505ac-258">[ **編集**  ] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="505ac-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="505ac-259">**参照の同期を選択 (スコープ) します。**</span><span class="sxs-lookup"><span data-stu-id="505ac-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="505ac-260">[イベントの作成] で (フィールドマッピングガイドに基づいて) CRM フィールドマッピングをカスタマイズする場合は、[ **Microsoft の紹介を作成する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="505ac-261">このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。</span><span class="sxs-lookup"><span data-stu-id="505ac-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="505ac-262">エンドツーエンドの双方向の共同販売参照の同期</span><span class="sxs-lookup"><span data-stu-id="505ac-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="505ac-263">パワー自動化ソリューションをインストールし、構成し、カスタマイズしたら、Salesforce CRM とパートナーセンター間の共同販売参照の同期をテストできます。</span><span class="sxs-lookup"><span data-stu-id="505ac-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="505ac-264">前提条件</span><span class="sxs-lookup"><span data-stu-id="505ac-264">Pre-requisites</span></span>

<span data-ttu-id="505ac-265">パートナーセンターと Salesforce CRM 間で推薦を同期するには、Power 区別のソリューションで、Microsoft 固有の紹介フィールドを明確にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="505ac-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="505ac-266">この id により、販売者チームは、共同販売のために Microsoft と共有する参照を決定することができます。</span><span class="sxs-lookup"><span data-stu-id="505ac-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="505ac-267">Salesforce CRM ソリューションの **営業案件** エンティティのパートナーセンターの紹介同期の一部として、一連のカスタムフィールドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="505ac-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="505ac-268">CRM 管理者ユーザーは、 **営業案件** のカスタムフィールドを使用して、別の crm セクションを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="505ac-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="505ac-269">次のカスタムフィールドは、CRM セクションの一部にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="505ac-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="505ac-270">**パートナーセンターとの同期**: 営業案件を Microsoft パートナーセンターと同期するかどうか</span><span class="sxs-lookup"><span data-stu-id="505ac-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="505ac-271">**参照識別子**: Microsoft パートナーセンターの紹介の読み取り専用識別子フィールド</span><span class="sxs-lookup"><span data-stu-id="505ac-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="505ac-272">**紹介リンク**: Microsoft パートナーセンターでの紹介への読み取り専用リンク</span><span class="sxs-lookup"><span data-stu-id="505ac-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="505ac-273">Microsoft**ヘルプ**を参照してください。</span><span class="sxs-lookup"><span data-stu-id="505ac-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="505ac-274">**製品**: この営業案件に関連付けられている製品の一覧</span><span class="sxs-lookup"><span data-stu-id="505ac-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="505ac-275">**監査**: パートナーセンターの紹介と同期するための読み取り専用の監査証跡</span><span class="sxs-lookup"><span data-stu-id="505ac-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="505ac-276">モデル</span><span class="sxs-lookup"><span data-stu-id="505ac-276">SCENARIOS:</span></span>

1. <span data-ttu-id="505ac-277">CRM で参照が作成または更新され、パートナーセンターで同期される場合の参照の同期:</span><span class="sxs-lookup"><span data-stu-id="505ac-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="505ac-278">CRM の **営業案件** セクションで可視性を持つユーザーを使用して、Salesforce crm 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="505ac-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="505ac-279">Salesforce CRM 環境で "新しい営業案件" を作成するときに、次のセクションが存在することを確認します。</span><span class="sxs-lookup"><span data-stu-id="505ac-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="AppSource を開く":::

   3. <span data-ttu-id="505ac-281">この機会を Microsoft パートナーセンターと同期するには、カードビューで次のフィールドを設定していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="505ac-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="505ac-282">"パートナーセンターとの同期": はい</span><span class="sxs-lookup"><span data-stu-id="505ac-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="505ac-283">「Microsoft がどのように役立つか」: 次のオプションから選択してください。</span><span class="sxs-lookup"><span data-stu-id="505ac-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="505ac-284">製品: 製品のソリューション Id</span><span class="sxs-lookup"><span data-stu-id="505ac-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="505ac-285">[営業案件  **とパートナーセンターの同期** ] オプションを **[はい]** に設定したら、10分待ってから、パートナーセンターアカウントにサインインします。</span><span class="sxs-lookup"><span data-stu-id="505ac-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="505ac-286">参照は、Salesforce CRM と同期されます。</span><span class="sxs-lookup"><span data-stu-id="505ac-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="505ac-287">[パートナーセンターとの同期] オプションが [はい] に設定されている場合、Salesforce CRM で営業案件を更新すると、変更がパートナーセンターアカウントと同期されます。</span><span class="sxs-lookup"><span data-stu-id="505ac-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="505ac-288">パートナーセンターで正常に同期された営業案件は、Salesforce CRM の✔アイコンで識別されます。</span><span class="sxs-lookup"><span data-stu-id="505ac-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="505ac-289">Microsoft パートナーセンターで参照が作成または更新され、Salesforce CRM 環境で同期される場合の紹介の同期:</span><span class="sxs-lookup"><span data-stu-id="505ac-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="505ac-290">パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="505ac-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="505ac-291">左側のメニューから [ **紹介** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="505ac-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="505ac-292">[新しい取引] オプションをクリックして、パートナーセンターから新しい共同販売紹介を作成します。</span><span class="sxs-lookup"><span data-stu-id="505ac-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="505ac-293">Salesforce CRM 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="505ac-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="505ac-294">**[Open opportunity**] に移動します。</span><span class="sxs-lookup"><span data-stu-id="505ac-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="505ac-295">Microsoft パートナーセンターで作成された紹介が、Salesforce CRM で同期されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="505ac-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="AppSource を開く":::

    6. <span data-ttu-id="505ac-297">同期された参照を選択すると、カードビューの詳細が設定されます。</span><span class="sxs-lookup"><span data-stu-id="505ac-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="505ac-298">次の手順</span><span class="sxs-lookup"><span data-stu-id="505ac-298">Next steps</span></span>

- [<span data-ttu-id="505ac-299">見込み客を管理する</span><span class="sxs-lookup"><span data-stu-id="505ac-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="505ac-300">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="505ac-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="505ac-301">パートナー センター Webhook</span><span class="sxs-lookup"><span data-stu-id="505ac-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)