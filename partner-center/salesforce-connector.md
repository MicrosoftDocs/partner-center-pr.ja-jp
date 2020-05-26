---
title: Salesforce CRM パートナーセンターの共同販売コネクタ
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Salesforce CRM コネクタを使用して、Microsoft からの参照を取得します。
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: ad39bdde92611066d0dd0c56d8b9133f4d9dcaa9
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825699"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="1fd5c-103">Salesforce CRM の共同販売コネクタ-概要</span><span class="sxs-lookup"><span data-stu-id="1fd5c-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="1fd5c-104">適切なロール</span><span class="sxs-lookup"><span data-stu-id="1fd5c-104">Appropriate roles</span></span>

- <span data-ttu-id="1fd5c-105">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="1fd5c-105">Referrals admin</span></span>
- <span data-ttu-id="1fd5c-106">CRM のシステム管理者またはシステムカスタマイザー</span><span class="sxs-lookup"><span data-stu-id="1fd5c-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="1fd5c-107">パートナーセンターの共同販売コネクタを使用すると、販売元は CRM システム内から Microsoft と共同で販売することができます。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="1fd5c-108">パートナーセンターを使用して共同販売取引を管理するためのトレーニングを行う必要はありません。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="1fd5c-109">共同販売コネクタを使用すると、Microsoft の販売者に協力したり、Microsoft 販売者からの推薦を受け取ったり、紹介を受け入れたり拒否したりすることができます。また、商談価値や決算日などの取引データを変更したり、これらの共同販売取引に関するマイクロソフト販売者からの更新を受け取ることができます。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-109">Using the Co-sell connectors, you will be able to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, closing date etc. as well as receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="1fd5c-110">パートナーセンターではなく、選択した CRM 内での作業中に、これらすべてを実行できます。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-110">You can do all of this while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="1fd5c-111">このソリューションは、Microsoft のパワー自動化ソリューションに基づいており、Microsoft パートナーセンター Api を使用しています。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-111">The solution is based on Microsoft Power Automate Solution and uses Microsoft Partner Center APIs.</span></span>


## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="1fd5c-112">をインストールする前に-前提条件</span><span class="sxs-lookup"><span data-stu-id="1fd5c-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="1fd5c-113">**トピック**</span><span class="sxs-lookup"><span data-stu-id="1fd5c-113">**Topics**</span></span>   |<span data-ttu-id="1fd5c-114">**詳細**</span><span class="sxs-lookup"><span data-stu-id="1fd5c-114">**Details**</span></span>   |<span data-ttu-id="1fd5c-115">**リンク**</span><span class="sxs-lookup"><span data-stu-id="1fd5c-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="1fd5c-116">Microsoft Partner Network ID</span><span class="sxs-lookup"><span data-stu-id="1fd5c-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="1fd5c-117">有効な MPN ID が必要です</span><span class="sxs-lookup"><span data-stu-id="1fd5c-117">You need a valid MPN ID</span></span>|<span data-ttu-id="1fd5c-118">[MPN](https://partner.microsoft.com/)に参加するには</span><span class="sxs-lookup"><span data-stu-id="1fd5c-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="1fd5c-119">共同販売の準備完了</span><span class="sxs-lookup"><span data-stu-id="1fd5c-119">Co-sell ready</span></span>|<span data-ttu-id="1fd5c-120">お客様の IP/サービスソリューションは、共同販売の準備ができている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="1fd5c-121">Microsoft との販売</span><span class="sxs-lookup"><span data-stu-id="1fd5c-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="1fd5c-122">パートナー センター アカウント</span><span class="sxs-lookup"><span data-stu-id="1fd5c-122">Partner Center account</span></span>|<span data-ttu-id="1fd5c-123">パートナーセンターのテナントに関連付けられている MPN ID は、共同販売ソリューションに関連付けられている MPN ID と同じである必要があります。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="1fd5c-124">コネクタをデプロイする前に、パートナーセンターポータルで共同販売の紹介を確認できることを確認します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-124">Verify that you can see your co-sell referrals in Partner Center portal prior to deploying the connectors.</span></span>|[<span data-ttu-id="1fd5c-125">アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="1fd5c-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="1fd5c-126">パートナー センターのユーザー ロール</span><span class="sxs-lookup"><span data-stu-id="1fd5c-126">Partner Center user roles</span></span>|<span data-ttu-id="1fd5c-127">コネクタをインストールして使用する従業員は、参照管理者である必要があります</span><span class="sxs-lookup"><span data-stu-id="1fd5c-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="1fd5c-128">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="1fd5c-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="1fd5c-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="1fd5c-129">Salesforce CRM</span></span>|<span data-ttu-id="1fd5c-130">CRM ユーザーロールは、システム管理者またはシステムカスタマイザーです。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="1fd5c-131">Dynamics 365 でロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="1fd5c-131">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="1fd5c-132">パワー自動化フローアカウント</span><span class="sxs-lookup"><span data-stu-id="1fd5c-132">Power Automate Flow Account</span></span>|<span data-ttu-id="1fd5c-133">CRM システム管理者またはシステムカスタマイザー用のアクティブな[電源自動化](https://flow.microsoft.com)アカウント。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="1fd5c-134">そのユーザーは、インストールの前に少なくとも1回、[電源の自動](https://flow.microsoft.com)登録を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="1fd5c-135">Salesforce CRM のパートナーセンターの紹介同期をインストールする</span><span class="sxs-lookup"><span data-stu-id="1fd5c-135">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="1fd5c-136">[[パワー自動化](https://flow.microsoft.com)] にアクセスし、右上隅にある [**環境**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-136">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="1fd5c-137">これにより、使用可能な CRM インスタンスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-137">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="1fd5c-138">右上隅にあるドロップダウンから適切な CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-138">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="1fd5c-139">左側のナビゲーションバーで [**ソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-139">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="1fd5c-140">上部のメニューの [ **AppSource を開く**] リンクをクリックします。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-140">Click on the **Open AppSource** link on the top menu.</span></span>

![AppSource を開く](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="1fd5c-142">ポップアップ画面で、 **Salesforce のパートナーセンターの紹介コネクタ**を検索します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-142">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

6. <span data-ttu-id="1fd5c-143">[**今すぐ入手**する] ボタンをクリックし、[**続行**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-143">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="1fd5c-144">これにより、CRM (Dynamics 365) 環境を選択してアプリケーションをインストールできるページが開きます。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-144">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="1fd5c-145">使用条件に同意します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-145">Agree to terms and conditions.</span></span> 

8. <span data-ttu-id="1fd5c-146">その後、[ソリューションの**管理**] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-146">You are then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="1fd5c-147">ページの下部にある矢印ボタンを使用して、[パートナーセンターの紹介] に移動します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-147">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="1fd5c-148">[パートナーセンターの紹介] ソリューションの横に、[**インストールのスケジュール**] が表示されます。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-148">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="1fd5c-149">インストールには10-15 分かかります。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-149">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="1fd5c-150">インストールが完了したら、[Power の[自動化](https://flow.microsoft.com)] に戻り、左側のナビゲーション領域から [**ソリューション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-150">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="1fd5c-151">**Salesforce のパートナーセンターの紹介同期**は、[ソリューション] の一覧で確認できます。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-151">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="1fd5c-152">**Dynamics 365 のパートナーセンターの紹介同期**を選択します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-152">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="1fd5c-153">次の電源の自動化フローとエンティティを利用できます。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-153">The following Power Automate flows and entities are available:</span></span>

![使用可能な CRMS](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="1fd5c-155">ベストプラクティス: 運用前にテストする</span><span class="sxs-lookup"><span data-stu-id="1fd5c-155">Best Practice: Test before you go live</span></span>

<span data-ttu-id="1fd5c-156">運用環境でパワー自動化ソリューションをインストール、構成、およびカスタマイズする前に、必ずステージング CRM インスタンスでソリューションをテストしてください。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-156">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="1fd5c-157">ステージング環境/CRM インスタンスに Microsoft Power 自動ソリューションをインストールします。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-157">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="1fd5c-158">ソリューションのコピーを作成し、構成を実行し、ステージング環境でフローのカスタマイズを自動化します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-158">Make a copy of the solution and perform your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="1fd5c-159">ステージング/CRM インスタンスでソリューションをテストします。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-159">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="1fd5c-160">成功した場合は、運用インスタンスにマネージドソリューションとしてインポートします。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-160">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="1fd5c-161">ソリューションを構成する</span><span class="sxs-lookup"><span data-stu-id="1fd5c-161">Configure the solution</span></span>

1. <span data-ttu-id="1fd5c-162">CRM インスタンスにソリューションをインストールしたら、[ [Power の自動化](https://flow.microsoft.com/)] に戻ります。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-162">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="1fd5c-163">右上隅にある [**環境**] ドロップダウンで、パワー自動化ソリューションをインストールした CRM インスタンスを選択します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-163">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="1fd5c-164">次の3つのユーザーアカウントを関連付ける接続を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-164">You will need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="1fd5c-165">参照管理者の資格情報を持つパートナーセンターのユーザー</span><span class="sxs-lookup"><span data-stu-id="1fd5c-165">Partner Center user with referrals admin credentials</span></span> 
- <span data-ttu-id="1fd5c-166">パートナー センターのイベント</span><span class="sxs-lookup"><span data-stu-id="1fd5c-166">Partner Center Events</span></span>
- <span data-ttu-id="1fd5c-167">Power を使用した CRM 管理ソリューションのフローが自動化されます。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-167">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="1fd5c-168">a。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-168">a.</span></span> <span data-ttu-id="1fd5c-169">左側のナビゲーションバーから [**接続**] を選択し、一覧から "パートナーセンターの紹介" ソリューションを選択します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>
    <span data-ttu-id="1fd5c-170">b.</span><span class="sxs-lookup"><span data-stu-id="1fd5c-170">b.</span></span> <span data-ttu-id="1fd5c-171">[**接続の作成**] をクリックして接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-171">Create a connection by clicking **Create a connection**.</span></span> 

    ![接続を作成する](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="1fd5c-173">c.</span><span class="sxs-lookup"><span data-stu-id="1fd5c-173">c.</span></span> <span data-ttu-id="1fd5c-174">右上隅の検索バーで、**パートナーセンターの参照 (プレビュー)** を検索します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>
    <span data-ttu-id="1fd5c-175">d.</span><span class="sxs-lookup"><span data-stu-id="1fd5c-175">d.</span></span> <span data-ttu-id="1fd5c-176">参照管理者の資格情報ロールを使用して、パートナーセンターユーザーの接続を作成します。つまり.</span><span class="sxs-lookup"><span data-stu-id="1fd5c-176">Create a connection for your Partner Center user with the credentials role of Referrals admin. e.</span></span> <span data-ttu-id="1fd5c-177">次に、パートナーセンターのユーザーに、参照管理者の資格情報を使用してパートナーセンターのイベント接続を作成します。f.</span><span class="sxs-lookup"><span data-stu-id="1fd5c-177">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin. f.</span></span> <span data-ttu-id="1fd5c-178">CRM 管理者ユーザーの Common Data Service (現在の環境) の接続を作成します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-178">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="1fd5c-179">電源自動化フローを接続に関連付けるには、各パワー自動化フローを編集して、Common Data Service とパートナーセンターの紹介に接続します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-179">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="1fd5c-180">変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-180">Save the changes.</span></span>

5. <span data-ttu-id="1fd5c-181">パワー自動化フローを**有効に**します。</span><span class="sxs-lookup"><span data-stu-id="1fd5c-181">**Turn on** the the Power Automate flows.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1fd5c-182">次のステップ</span><span class="sxs-lookup"><span data-stu-id="1fd5c-182">Next steps</span></span>

- [<span data-ttu-id="1fd5c-183">Webhook を使用してリソース変更イベントを取得する</span><span class="sxs-lookup"><span data-stu-id="1fd5c-183">Use Webhooks to get resource change events</span></span>](referral-connector-webhooks.md)

- [<span data-ttu-id="1fd5c-184">Microsoft Power の自動化プラットフォームの詳細</span><span class="sxs-lookup"><span data-stu-id="1fd5c-184">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="1fd5c-185">見込み客を管理する</span><span class="sxs-lookup"><span data-stu-id="1fd5c-185">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="1fd5c-186">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="1fd5c-186">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
