---
title: Salesforce CRM パートナーセンターの共同販売コネクタ
ms.topic: how-to
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターでの紹介を Salesforce CRM と同期する
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 4b96be195788ccc8b82aafd0bddb90dd34a672f9
ms.sourcegitcommit: 3329fd120d8d49a4831412b79e044678ec71b84c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/29/2020
ms.locfileid: "91422448"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="3b83b-103">Salesforce CRM のための共同販売コネクタ - 概要</span><span class="sxs-lookup"><span data-stu-id="3b83b-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="3b83b-104">適切なロール</span><span class="sxs-lookup"><span data-stu-id="3b83b-104">Appropriate roles</span></span>

- <span data-ttu-id="3b83b-105">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="3b83b-105">Referrals admin</span></span>
- <span data-ttu-id="3b83b-106">CRM のシステム管理者またはシステムカスタマイザー</span><span class="sxs-lookup"><span data-stu-id="3b83b-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="3b83b-107">パートナーセンターの共同販売コネクタを使用すると、販売元は CRM システム内から Microsoft と共同で販売することができます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="3b83b-108">パートナーセンターを使用して共同販売取引を管理するためのトレーニングを行う必要はありません。</span><span class="sxs-lookup"><span data-stu-id="3b83b-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="3b83b-109">共同販売コネクタを使用して、Microsoft の販売者に連絡したり、Microsoft 販売者からの推薦を受け取ったり、紹介を受け入れたり拒否したりすることができます。また、商談の価値や決算日などの商談データを変更することもできます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="3b83b-110">また、これらの共同販売取引に関するマイクロソフト販売者からの更新を受け取ることもできます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="3b83b-111">パートナーセンターではなく、選択した CRM 内での作業中に、すべての紹介作業を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="3b83b-112">このソリューションは、Microsoft のパワー自動化ソリューションに基づいており、パートナーセンター Api を使用しています。</span><span class="sxs-lookup"><span data-stu-id="3b83b-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="3b83b-113">をインストールする前に-前提条件</span><span class="sxs-lookup"><span data-stu-id="3b83b-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="3b83b-114">**トピック**</span><span class="sxs-lookup"><span data-stu-id="3b83b-114">**Topics**</span></span>   |<span data-ttu-id="3b83b-115">**詳細**</span><span class="sxs-lookup"><span data-stu-id="3b83b-115">**Details**</span></span>   |<span data-ttu-id="3b83b-116">**リンク**</span><span class="sxs-lookup"><span data-stu-id="3b83b-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="3b83b-117">Microsoft Partner Network ID</span><span class="sxs-lookup"><span data-stu-id="3b83b-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="3b83b-118">有効な MPN ID が必要です</span><span class="sxs-lookup"><span data-stu-id="3b83b-118">You need a valid MPN ID</span></span>|<span data-ttu-id="3b83b-119">[MPN](https://partner.microsoft.com/)に参加するには</span><span class="sxs-lookup"><span data-stu-id="3b83b-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="3b83b-120">共同販売の準備完了</span><span class="sxs-lookup"><span data-stu-id="3b83b-120">Co-sell ready</span></span>|<span data-ttu-id="3b83b-121">お客様の IP/サービスソリューションは、共同販売の準備ができている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b83b-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="3b83b-122">Microsoft との販売</span><span class="sxs-lookup"><span data-stu-id="3b83b-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="3b83b-123">パートナー センター アカウント</span><span class="sxs-lookup"><span data-stu-id="3b83b-123">Partner Center account</span></span>|<span data-ttu-id="3b83b-124">パートナーセンターのテナントに関連付けられている MPN ID は、共同販売ソリューションに関連付けられている MPN ID と同じである必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b83b-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="3b83b-125">コネクタをデプロイする前に、パートナーセンターポータルで共同販売の紹介を確認できることを確認します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="3b83b-126">アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="3b83b-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="3b83b-127">パートナー センターのユーザー ロール</span><span class="sxs-lookup"><span data-stu-id="3b83b-127">Partner Center user roles</span></span>|<span data-ttu-id="3b83b-128">コネクタをインストールして使用する従業員は、参照管理者である必要があります</span><span class="sxs-lookup"><span data-stu-id="3b83b-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="3b83b-129">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="3b83b-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="3b83b-130">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="3b83b-130">Salesforce CRM</span></span>|<span data-ttu-id="3b83b-131">CRM ユーザーロールは、システム管理者またはシステムカスタマイザーです。</span><span class="sxs-lookup"><span data-stu-id="3b83b-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="3b83b-132">Salesforce CRM でロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="3b83b-132">Assign roles in Salesforce CRM</span></span>](/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="3b83b-133">パワー自動化フローアカウント</span><span class="sxs-lookup"><span data-stu-id="3b83b-133">Power Automate Flow Account</span></span>|<span data-ttu-id="3b83b-134">CRM システム管理者またはシステムカスタマイザー用のアクティブな [電源自動化](https://flow.microsoft.com) アカウント。</span><span class="sxs-lookup"><span data-stu-id="3b83b-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="3b83b-135">そのユーザーは、インストールの前に少なくとも1回、 [電源の自動](https://flow.microsoft.com) 登録を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b83b-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="3b83b-136">Microsoft カスタムフィールド用の Salesforce パッケージのインストール</span><span class="sxs-lookup"><span data-stu-id="3b83b-136">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="3b83b-137">パートナーセンターと Salesforce CRM 間で紹介を同期するために、Power solution の自動化ソリューションでは、Microsoft 固有の参照フィールドを明確に識別する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b83b-137">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="3b83b-138">このような境界は、パートナーの販売者チームが、共同販売のために Microsoft と共有する参照を決定する機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-138">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="3b83b-139">Salesforce で、 **メモ** をアクティブ化し、営業案件の関連リストに追加します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-139">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="3b83b-140">参照</span><span class="sxs-lookup"><span data-stu-id="3b83b-140">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="3b83b-141">次の手順に従って **営業案件チーム** をアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-141">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="3b83b-142">セットアップで、[ **クイック検索** ] ボックスを使用して営業案件チームの設定を検索します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-142">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="3b83b-143">必要に応じて設定を定義します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-143">Define the settings as needed.</span></span>
[<span data-ttu-id="3b83b-144">参照</span><span class="sxs-lookup"><span data-stu-id="3b83b-144">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="3b83b-145">Salesforce で、次のパッケージインストーラーを使用して、カスタムフィールドとオブジェクトをインストールします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-145">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="3b83b-146">任意の会社にパッケージをインストールするには、 [ここ](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) を参照してください:</span><span class="sxs-lookup"><span data-stu-id="3b83b-146">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) to install the package into any company:</span></span>


<span data-ttu-id="3b83b-147">注: をサンドボックスにインストールする場合は、URL の最初の部分を次のように置き換える必要があります。 http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="3b83b-147">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="3b83b-148">Salesforce で、 **営業案件** 関連の一覧に Microsoft ソリューションを追加します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-148">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="3b83b-149">追加したら、 **レンチ** アイコンをクリックし、プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-149">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="3b83b-150">ベストプラクティス: 運用前にテストする</span><span class="sxs-lookup"><span data-stu-id="3b83b-150">Best Practice: Test before you go live</span></span>

<span data-ttu-id="3b83b-151">運用環境でパワー自動化ソリューションをインストール、構成、およびカスタマイズする前に、必ずステージング CRM インスタンスでソリューションをテストしてください。</span><span class="sxs-lookup"><span data-stu-id="3b83b-151">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="3b83b-152">ステージング環境/CRM インスタンスに Microsoft Power 自動ソリューションをインストールします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-152">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="3b83b-153">ソリューションのコピーを作成し、構成を実行して、ステージング環境でフローのカスタマイズを自動化します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-153">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="3b83b-154">ステージング/CRM インスタンスでソリューションをテストします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-154">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="3b83b-155">成功した場合は、運用インスタンスにマネージドソリューションとしてインポートします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-155">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="3b83b-156">Salesforce CRM のパートナーセンターの紹介同期をインストールする</span><span class="sxs-lookup"><span data-stu-id="3b83b-156">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="3b83b-157">[ [パワー自動化](https://flow.microsoft.com) ] にアクセスし、右上隅にある [ **環境** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-157">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="3b83b-158">これにより、使用可能な CRM インスタンスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-158">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="3b83b-159">右上隅にあるドロップダウンから適切な CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-159">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="3b83b-160">左側のナビゲーションバーで [ **ソリューション** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-160">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="3b83b-161">上部のメニューの [ **AppSource を開く** ] リンクをクリックします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-161">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource を開く":::

5. <span data-ttu-id="3b83b-163">ポップアップ画面で、 **Salesforce のパートナーセンターの紹介コネクタ** を検索します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-163">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="3b83b-165">[ **今すぐ入手** する] ボタンをクリックし、[ **続行**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-165">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="3b83b-166">これにより、Salesforce CRM 環境を選択してアプリケーションをインストールできるページが開きます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-166">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="3b83b-167">使用条件に同意します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-167">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="使用可能な CRMS":::

8. <span data-ttu-id="3b83b-169">その後、[ **ソリューションの管理** ] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-169">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="3b83b-170">ページの下部にある矢印ボタンを使用して、[パートナーセンターの紹介] に移動します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-170">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="3b83b-171">[パートナーセンターの紹介] ソリューションの横に、[**インストールのスケジュール**] が表示されます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-171">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="3b83b-172">インストールには10-15 分かかります。</span><span class="sxs-lookup"><span data-stu-id="3b83b-172">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="3b83b-173">インストールが完了したら、[Power の [自動化](https://flow.microsoft.com) ] に戻り、左側のナビゲーション領域から [ **ソリューション** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-173">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="3b83b-174">**Salesforce のパートナーセンターの紹介同期**は、[ソリューション] の一覧で確認できます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-174">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="3b83b-175">**Salesforce のパートナーセンター紹介同期**を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-175">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="3b83b-176">次の電源の自動化フローとエンティティを利用できます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-176">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce フロー":::



## <a name="configure-the-solution"></a><span data-ttu-id="3b83b-178">ソリューションの構成</span><span class="sxs-lookup"><span data-stu-id="3b83b-178">Configure the solution</span></span>

1. <span data-ttu-id="3b83b-179">CRM インスタンスにソリューションをインストールしたら、[ [Power の自動化](https://flow.microsoft.com/)] に戻ります。</span><span class="sxs-lookup"><span data-stu-id="3b83b-179">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="3b83b-180">右上隅にある [ **環境** ] ドロップダウンで、パワー自動化ソリューションをインストールした CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-180">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="3b83b-181">次の3つのユーザーアカウントを関連付ける接続を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b83b-181">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="3b83b-182">参照管理者の資格情報を持つパートナーセンターのユーザー</span><span class="sxs-lookup"><span data-stu-id="3b83b-182">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="3b83b-183">パートナー センターのイベント</span><span class="sxs-lookup"><span data-stu-id="3b83b-183">Partner Center Events</span></span>
    - <span data-ttu-id="3b83b-184">Power を使用した CRM 管理ソリューションのフローが自動化されます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-184">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="3b83b-185">左側のナビゲーションバーから [ **接続** ] を選択し、一覧から "パートナーセンターの紹介" ソリューションを選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-185">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="3b83b-186">[ **接続の作成**] をクリックして接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-186">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="接続を作成する":::

- <span data-ttu-id="3b83b-188">右上隅の検索バーで、パートナーセンターの参照 (プレビュー) を検索します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-188">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="3b83b-189">参照管理者の資格情報ロールを使用して、パートナーセンターユーザーの接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-189">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="3b83b-190">次に、パートナーセンターのユーザーに、参照管理者の資格情報を使用してパートナーセンターのイベント接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-190">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="3b83b-191">CRM 管理者ユーザーの Common Data Service (現在の環境) の接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-191">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

-  <span data-ttu-id="3b83b-192">すべての接続を追加すると、環境内に次の接続が表示されます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-192">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="接続を監視する":::

### <a name="edit-the-connections"></a><span data-ttu-id="3b83b-194">接続を編集する</span><span class="sxs-lookup"><span data-stu-id="3b83b-194">Edit the connections</span></span>

1. <span data-ttu-id="3b83b-195">[ソリューション] ページに戻り、[ **既定のソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-195">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="3b83b-196">[**すべて**] をクリックして、[**接続の参照 (プレビュー)** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-196">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="コネクタの編集を開始します":::

2. <span data-ttu-id="3b83b-198">3つのドットアイコンを選択して、各接続を1つずつ編集します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-198">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="3b83b-199">関連する接続を追加します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-199">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="コネクタの編集":::

3. <span data-ttu-id="3b83b-201">次の順序でフローを有効にします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-201">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="3b83b-202">パートナーセンターの Webhook の登録 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="3b83b-202">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="3b83b-203">パートナーセンターへの共同販売参照の作成-Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="3b83b-203">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="3b83b-204">パートナーセンター: Microsoft 共同での Salesforce の参照の更新 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="3b83b-204">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="3b83b-205">パートナーセンターから Salesforce へ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="3b83b-205">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="3b83b-206">Salesforce からパートナーセンターへ (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="3b83b-206">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="3b83b-207">パートナーセンターへの Salesforce の営業案件 (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="3b83b-207">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="3b83b-208">パートナーセンターへの Salesforce Microsoft ソリューション (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="3b83b-208">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="3b83b-209">Webhook Api を使用してリソース変更イベントに登録する</span><span class="sxs-lookup"><span data-stu-id="3b83b-209">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="3b83b-210">パートナーセンターの Webhook Api を使用すると、リソース変更イベントに登録できます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-210">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="3b83b-211">これらの変更イベントは、HTTP 投稿として url に送信されます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-211">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="3b83b-212">Url を登録するには、 **パートナーセンターの Webhook 登録 (Insider Preview)** パワー自動化フローを選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-212">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="3b83b-213">参照管理者の資格情報を持つパートナーセンターのユーザー (a.) に接続を追加します。パートナーセンターのイベントは、下に強調表示されています。</span><span class="sxs-lookup"><span data-stu-id="3b83b-213">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="トリガー":::

3. <span data-ttu-id="3b83b-215">これらの更新を行うと、次のように表示されます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-215">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="3b83b-217">変更内容を保存し、[ **有効にする**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-217">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="3b83b-218">パートナーセンターの webhook でイベントの変更をリッスンできるようにするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-218">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="3b83b-219">[ **パートナーセンター] を**選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-219">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="3b83b-220">[ **編集** ] アイコンを選択し、[ **HTTP 要求の受信時**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-220">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="3b83b-221">**コピー**アイコンを選択して、指定された HTTP POST URL をコピーします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-221">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL のコピー":::

8. <span data-ttu-id="3b83b-223">次に、"パートナーセンターの Webhook の登録 (Insider Preview)" パワー自動化フローを選択し、[ **実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-223">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="3b83b-224">右側のウィンドウで [実行フロー] ウィンドウが開いていることを確認し、[ **続行**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-224">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="3b83b-225">次の詳細を入力します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-225">Enter the following details:</span></span>

    1. <span data-ttu-id="3b83b-226">**Http トリガーエンドポイント**: 前の手順からコピーされた URL</span><span class="sxs-lookup"><span data-stu-id="3b83b-226">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="3b83b-227">**登録するイベント**: "紹介-作成" と "参照-更新"</span><span class="sxs-lookup"><span data-stu-id="3b83b-227">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="3b83b-228">**既存のトリガーエンドポイントがある場合は上書き**します (存在する場合は既存のエンドポイントを上書きします)。</span><span class="sxs-lookup"><span data-stu-id="3b83b-228">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="3b83b-229">[ **実行** ] を選択し、[完了] を選択し **ます。**</span><span class="sxs-lookup"><span data-stu-id="3b83b-229">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="3b83b-230">Webhook は、イベントの作成と更新をリッスンできるようになりました。</span><span class="sxs-lookup"><span data-stu-id="3b83b-230">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="3b83b-231">同期手順のカスタマイズ</span><span class="sxs-lookup"><span data-stu-id="3b83b-231">Customize synchronization steps</span></span>

<span data-ttu-id="3b83b-232">パートナーセンターと CRM システムの間で共同販売参照が同期されると、パートナーセンター PC で同期されるフィールドがここに表示されます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-232">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="3b83b-233">多くの場合、CRM システムは高度にカスタマイズされています。</span><span class="sxs-lookup"><span data-stu-id="3b83b-233">Often CRM systems are highly customized.</span></span> <span data-ttu-id="3b83b-234">パワー自動化フローをカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-234">You can customize the Power Automate flows.</span></span> <span data-ttu-id="3b83b-235">フィールドマッピングガイドに従って、必要に応じて、パワー自動化フローの手順に適切な変更を加えます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-235">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="3b83b-236">Microsoft パートナーセンターから CRM へのマッピングが提供されますが、CRM 環境に基づいて、フィールドをさらにカスタマイズすることもできます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-236">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="3b83b-237">各パワー自動化フローの複数の手順は、ニーズに応じてカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-237">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="3b83b-238">使用可能なカスタマイズの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-238">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="3b83b-239">パートナーセンターで作成または更新イベントのフィールドを CRM の参照同期にカスタマイズするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-239">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="3b83b-240">[パートナーセンター] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-240">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="3b83b-241">[ **編集** ] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-241">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="3b83b-242">選択 **(スコープ) 潜在顧客または営業案件を同期**します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-242">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="3b83b-243">作成イベントの CRM フィールドマッピングをカスタマイズするには、[ **新しい共有の営業案件]、[**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-243">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="3b83b-244">[ **はい] の場合** はサブステップを選択し、 **CRM で [新しい営業案件の作成**] を展開します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-244">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="3b83b-245">このセクションでマッピングを編集するには、[フィールドマッピングガイド] を使用します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-245">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="3b83b-246">更新イベントの CRM フィールドマッピングをカスタマイズするには、[(スコープ) 潜在顧客または営業案件を同期する] ステップをクリックします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-246">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="3b83b-247">**営業案件の更新である場合は、** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-247">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="3b83b-248">[サブステップ **if yes]** を選択し、次に **パートナーセンターと CRM の営業案件オブジェクト間の差異がある場合**は、を展開します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-248">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="3b83b-249">**既存の営業案件を更新**する場合は、[**はい]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-249">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="3b83b-250">更新イベントの CRM から PC への参照同期のフィールドをカスタマイズするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-250">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="3b83b-251">[ **編集**  ] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-251">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="3b83b-252">[ **(スコープ)] を選択して、営業案件を同期**します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-252">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="3b83b-253">更新イベントの CRM フィールドマッピング (フィールドマッピングガイドに基づく) をカスタマイズする場合は、 **パートナーセンターと CRM の潜在顧客オブジェクトが異なるかどうか**を選択してから、を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-253">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="3b83b-254">[ **はい] の場合** はサブステップを選択し、[ **営業案件データを使用して紹介を更新する**] ステップを展開します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-254">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="3b83b-255">このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-255">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="3b83b-256">Create events の CRM to PC 参照同期のフィールドをカスタマイズするには</span><span class="sxs-lookup"><span data-stu-id="3b83b-256">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="3b83b-257">[ **編集**  ] を選択して、パワー自動化フローを編集またはカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-257">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="3b83b-258">**参照の同期を選択 (スコープ) します。**</span><span class="sxs-lookup"><span data-stu-id="3b83b-258">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="3b83b-259">[イベントの作成] で (フィールドマッピングガイドに基づいて) CRM フィールドマッピングをカスタマイズする場合は、[ **Microsoft の紹介を作成する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-259">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="3b83b-260">このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-260">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="3b83b-261">エンドツーエンドの双方向の共同販売参照の同期</span><span class="sxs-lookup"><span data-stu-id="3b83b-261">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="3b83b-262">パワー自動化ソリューションをインストールし、構成し、カスタマイズしたら、Salesforce CRM とパートナーセンター間の共同販売参照の同期をテストできます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-262">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="3b83b-263">前提条件</span><span class="sxs-lookup"><span data-stu-id="3b83b-263">Pre-requisites</span></span>

<span data-ttu-id="3b83b-264">パートナーセンターと Salesforce CRM 間で推薦を同期するには、Power 区別のソリューションで、Microsoft 固有の紹介フィールドを明確にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b83b-264">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="3b83b-265">この id により、販売者チームは、共同販売のために Microsoft と共有する参照を決定することができます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-265">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="3b83b-266">Salesforce CRM ソリューションの **営業案件** エンティティのパートナーセンターの紹介同期の一部として、一連のカスタムフィールドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-266">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="3b83b-267">CRM 管理者ユーザーは、 **営業案件** のカスタムフィールドを使用して、別の crm セクションを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b83b-267">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="3b83b-268">次のカスタムフィールドは、CRM セクションの一部にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b83b-268">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="3b83b-269">**パートナーセンターとの同期**: 営業案件を Microsoft パートナーセンターと同期するかどうか</span><span class="sxs-lookup"><span data-stu-id="3b83b-269">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="3b83b-270">**参照識別子**: Microsoft パートナーセンターの紹介の読み取り専用識別子フィールド</span><span class="sxs-lookup"><span data-stu-id="3b83b-270">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="3b83b-271">**紹介リンク**: Microsoft パートナーセンターでの紹介への読み取り専用リンク</span><span class="sxs-lookup"><span data-stu-id="3b83b-271">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="3b83b-272">Microsoft**ヘルプ**を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b83b-272">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="3b83b-273">**製品**: この営業案件に関連付けられている製品の一覧</span><span class="sxs-lookup"><span data-stu-id="3b83b-273">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="3b83b-274">**監査**: パートナーセンターの紹介と同期するための読み取り専用の監査証跡</span><span class="sxs-lookup"><span data-stu-id="3b83b-274">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="3b83b-275">モデル</span><span class="sxs-lookup"><span data-stu-id="3b83b-275">SCENARIOS:</span></span>

1. <span data-ttu-id="3b83b-276">CRM で参照が作成または更新され、パートナーセンターで同期される場合の参照の同期:</span><span class="sxs-lookup"><span data-stu-id="3b83b-276">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="3b83b-277">CRM の **営業案件** セクションで可視性を持つユーザーを使用して、Salesforce crm 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-277">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="3b83b-278">Salesforce CRM 環境で "新しい営業案件" を作成するときに、次のセクションが存在することを確認します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-278">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 環境":::

   3. <span data-ttu-id="3b83b-280">この機会を Microsoft パートナーセンターと同期するには、カードビューで次のフィールドを設定していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-280">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="3b83b-281">"パートナーセンターとの同期": はい</span><span class="sxs-lookup"><span data-stu-id="3b83b-281">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="3b83b-282">「Microsoft がどのように役立つか」: 次のオプションから選択してください。</span><span class="sxs-lookup"><span data-stu-id="3b83b-282">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="3b83b-283">製品: 製品のソリューション Id</span><span class="sxs-lookup"><span data-stu-id="3b83b-283">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="3b83b-284">[営業案件  **とパートナーセンターの同期** ] オプションを **[はい]** に設定したら、10分待ってから、パートナーセンターアカウントにサインインします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-284">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="3b83b-285">参照は、Salesforce CRM と同期されます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-285">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="3b83b-286">[パートナーセンターとの同期] オプションが [はい] に設定されている場合、Salesforce CRM で営業案件を更新すると、変更がパートナーセンターアカウントと同期されます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-286">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="3b83b-287">パートナーセンターで正常に同期された営業案件は、Salesforce CRM の✔アイコンで識別されます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-287">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="3b83b-288">Microsoft パートナーセンターで参照が作成または更新され、Salesforce CRM 環境で同期される場合の紹介の同期:</span><span class="sxs-lookup"><span data-stu-id="3b83b-288">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="3b83b-289">パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-289">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="3b83b-290">左側のメニューから [ **紹介** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-290">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="3b83b-291">[新しい取引] オプションをクリックして、パートナーセンターから新しい共同販売紹介を作成します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-291">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="3b83b-292">Salesforce CRM 環境にサインインします。</span><span class="sxs-lookup"><span data-stu-id="3b83b-292">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="3b83b-293">**[Open opportunity**] に移動します。</span><span class="sxs-lookup"><span data-stu-id="3b83b-293">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="3b83b-294">Microsoft パートナーセンターで作成された紹介が、Salesforce CRM で同期されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="3b83b-294">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce の営業案件画面":::

    6. <span data-ttu-id="3b83b-296">同期された参照を選択すると、カードビューの詳細が設定されます。</span><span class="sxs-lookup"><span data-stu-id="3b83b-296">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3b83b-297">次の手順</span><span class="sxs-lookup"><span data-stu-id="3b83b-297">Next steps</span></span>

- [<span data-ttu-id="3b83b-298">見込み客を管理する</span><span class="sxs-lookup"><span data-stu-id="3b83b-298">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="3b83b-299">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="3b83b-299">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="3b83b-300">パートナー センター Webhook</span><span class="sxs-lookup"><span data-stu-id="3b83b-300">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)