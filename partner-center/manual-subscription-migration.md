---
title: Dynamics 365 および Customer Engagement プランを基本 (認定提供) から新しいバージョンに移行する |パートナーセンター
ms.topic: article
ms.date: 12/12/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 既存のサブスクリプションの有効期限が切れる前に新しいサブスクリプションを購入し、ユーザーライセンスを再割り当てして、古いサブスクリプションをキャンセルする方法について説明します。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 プラン、更新プラン、新しい Dynamics 365 Sku
ms.openlocfilehash: 466f954af05a266fccba587007565e5d19d3af15
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004592"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="d32dc-104">Dynamics 365 および Customer Engagement プランの Basic (対象プラン) から新しいバージョンへの移行</span><span class="sxs-lookup"><span data-stu-id="d32dc-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="d32dc-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="d32dc-105">**Applies to**</span></span>

-  <span data-ttu-id="d32dc-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="d32dc-106">Partner Center</span></span>

<span data-ttu-id="d32dc-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="d32dc-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="d32dc-108">グローバル管理</span><span class="sxs-lookup"><span data-stu-id="d32dc-108">Global admin</span></span>
-   <span data-ttu-id="d32dc-109">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="d32dc-109">User admin</span></span>
-   <span data-ttu-id="d32dc-110">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="d32dc-110">Admin agent</span></span>
-   <span data-ttu-id="d32dc-111">販売代理店</span><span class="sxs-lookup"><span data-stu-id="d32dc-111">Sales agent</span></span>

<span data-ttu-id="d32dc-112">2019年1月1日より、Basic (認定提供) サブスクリプションの Dynamics 365 for Sales/Customer Engagement プランをお持ちのお客様は、これらのレガシプランを更新できなくなります。既存のサブスクリプションは、有効期限が切れると自動的に更新されません。</span><span class="sxs-lookup"><span data-stu-id="d32dc-112">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="d32dc-113">サブスクリプションの詳細ページで、[日付] の [自動更新] の [日付] にサブスクリプションの状態が [有効期限切れ] に変わります。</span><span class="sxs-lookup"><span data-stu-id="d32dc-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="d32dc-114">顧客の継続性を確保するには、有効期限が切れたサブスクリプションを使用して、以下のサポートされているオプションに切り替える必要があります。</span><span class="sxs-lookup"><span data-stu-id="d32dc-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="d32dc-115">顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="d32dc-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="d32dc-116">API (CREST またはパートナーセンター) を使用する場合は、サブスクリプションの終了日と自動更新 = False プロパティを評価することで、有効期限が切れたサブスクリプションを見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="d32dc-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="d32dc-117">該当するサブスクリプションは、2019年1月1日に自動更新 = False に設定されます。</span><span class="sxs-lookup"><span data-stu-id="d32dc-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="d32dc-118">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="d32dc-118">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="d32dc-119">Dynamics 365 の提供終了</span><span class="sxs-lookup"><span data-stu-id="d32dc-119">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="d32dc-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="d32dc-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d32dc-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (認定オファー) for 教職員</span><span class="sxs-lookup"><span data-stu-id="d32dc-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d32dc-122">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (認定オファー) for Students</span><span class="sxs-lookup"><span data-stu-id="d32dc-122">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d32dc-123">Dynamics 365 for Sales Enterprise Edition (Government 価格) CRMOL Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="d32dc-123">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d32dc-124">Dynamics 365 for Sales Enterprise Edition for CRM Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="d32dc-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d32dc-125">Dynamics 365 for Sales Enterprise Edition for CRM Basic (認定オファー) for 教職員</span><span class="sxs-lookup"><span data-stu-id="d32dc-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d32dc-126">学生向けの SA からの Dynamics 365 for Sales Enterprise Edition for CRM Basic (認定オファー)</span><span class="sxs-lookup"><span data-stu-id="d32dc-126">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d32dc-127">Dynamics 365 for Sales Enterprise Edition (Government 価格) From CRM Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="d32dc-127">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d32dc-128">CRM Basic 用 Dynamics 365 for Sales Enterprise Edition アドオン (修飾されるプラン)</span><span class="sxs-lookup"><span data-stu-id="d32dc-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d32dc-129">CRM Basic (認定オファー) 用の Dynamics 365 for Sales Enterprise Edition アドオン</span><span class="sxs-lookup"><span data-stu-id="d32dc-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d32dc-130">CRM Basic (認定オファー) for Students 用 Dynamics 365 for Sales Enterprise Edition アドオン</span><span class="sxs-lookup"><span data-stu-id="d32dc-130">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d32dc-131">CRM Basic 用 Dynamics 365 for Sales Enterprise Edition (Government 価格) アドオン (修飾されるプラン)</span><span class="sxs-lookup"><span data-stu-id="d32dc-131">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d32dc-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="d32dc-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d32dc-133">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government 価格) CRMOL Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="d32dc-133">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d32dc-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (認定オファー) for Students</span><span class="sxs-lookup"><span data-stu-id="d32dc-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d32dc-135">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (認定プラン) (教職員向け)</span><span class="sxs-lookup"><span data-stu-id="d32dc-135">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d32dc-136">Dynamics 365 Customer Engagement Plan Enterprise Edition for CRM Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="d32dc-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d32dc-137">Dynamics 365 カスタマーエンゲージメントプラン Enterprise Edition (Government 価格) (SA for CRM Basic) (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="d32dc-137">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d32dc-138">Dynamics 365 Customer Engagement Plan Enterprise Edition for CRM Basic (認定オファー) for Students</span><span class="sxs-lookup"><span data-stu-id="d32dc-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d32dc-139">Dynamics 365 カスタマーエンゲージメントプラン Enterprise Edition for CRM Basic (認定オファー) for 教職員</span><span class="sxs-lookup"><span data-stu-id="d32dc-139">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d32dc-140">Dynamics 365 Customer Engagement Plan Enterprise Edition アドオン for CRM Basic (修飾されるプラン)</span><span class="sxs-lookup"><span data-stu-id="d32dc-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d32dc-141">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government 価格) アドオン for CRM Basic (認定プラン)</span><span class="sxs-lookup"><span data-stu-id="d32dc-141">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d32dc-142">CRM Basic (修飾されるオファー) 用の Dynamics 365 カスタマーエンゲージメントプラン Enterprise Edition アドオン</span><span class="sxs-lookup"><span data-stu-id="d32dc-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d32dc-143">Dynamics 365 Customer Engagement Plan Enterprise Edition アドオン for CRM Basic (認定オファー) for 教職員</span><span class="sxs-lookup"><span data-stu-id="d32dc-143">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="d32dc-144">Basic (認定オファー) 置換プランからの Sales/Customer Engagement プランの Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="d32dc-144">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="d32dc-145">**提供終了**</span><span class="sxs-lookup"><span data-stu-id="d32dc-145">**Retired offers**</span></span>   

- <span data-ttu-id="d32dc-146">CRM Basic または CRMOL Basic (修飾プラン) からの Sales の Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="d32dc-146">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d32dc-147">CRM Basic または CRMOL Basic (限定プラン) からの Dynamics 365 カスタマーエンゲージメントプラン</span><span class="sxs-lookup"><span data-stu-id="d32dc-147">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="d32dc-148">**置換オプション**</span><span class="sxs-lookup"><span data-stu-id="d32dc-148">**Replacement options**</span></span>
- <span data-ttu-id="d32dc-149">Dynamics 365 for Sales Professional (新規)</span><span class="sxs-lookup"><span data-stu-id="d32dc-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="d32dc-150">Dynamics 365 for Sales Professional (新規)</span><span class="sxs-lookup"><span data-stu-id="d32dc-150">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="d32dc-151">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="d32dc-151">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="d32dc-152">Dynamics 365 Customer Engagement プランまたは</span><span class="sxs-lookup"><span data-stu-id="d32dc-152">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="d32dc-153">Dynamics 365 チームメンバー</span><span class="sxs-lookup"><span data-stu-id="d32dc-153">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="d32dc-154">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="d32dc-154">Transition customers to new product plans</span></span>

<span data-ttu-id="d32dc-155">廃止された Sku から新しいバージョンに顧客を移動するには、次の手順を順番に実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d32dc-155">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="d32dc-156">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="d32dc-156">Purchase the new subscription</span></span>
- <span data-ttu-id="d32dc-157">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="d32dc-157">Reassign current user licenses</span></span>
- <span data-ttu-id="d32dc-158">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="d32dc-158">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="d32dc-159">顧客の新しいプランを購入する</span><span class="sxs-lookup"><span data-stu-id="d32dc-159">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="d32dc-160">左側のナビゲーションから **[Customers]** を選択し、新しいサブスクリプションに移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="d32dc-160">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="d32dc-161">**[サブスクリプションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d32dc-161">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="d32dc-162">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、 **[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="d32dc-162">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="d32dc-163">これで、お客様は古いサブスクリプションと新しいサブスクリプションの両方を使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="d32dc-163">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="d32dc-164">次の手順では、顧客のユーザーにライセンスを再割り当てします。</span><span class="sxs-lookup"><span data-stu-id="d32dc-164">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="d32dc-165">左側のナビゲーションから **[Customers]** を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="d32dc-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="d32dc-166">**[ユーザーとライセンス]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="d32dc-166">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="d32dc-167">ライセンスをユーザーに再割り当てするには、ユーザーを選択し、 **[ライセンスの管理]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d32dc-167">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="d32dc-168">[**ライセンスの管理**365] ページで、[Basic (限定されたプラン) のライセンス] チェックボックスをオンにして、顧客が移動しているサブスクリプションの新しいサービスプランを選択します。</span><span class="sxs-lookup"><span data-stu-id="d32dc-168">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="d32dc-169">**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="d32dc-169">Select **Submit**.</span></span> <span data-ttu-id="d32dc-170">この操作は、新しいライセンスが必要なユーザーごとに行います。</span><span class="sxs-lookup"><span data-stu-id="d32dc-170">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="d32dc-171">新しいサブスクリプションにライセンスを移行したら、古いサブスクリプションを取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="d32dc-171">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="d32dc-172">左側のナビゲーションから **[Customers]** を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="d32dc-172">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="d32dc-173">[サブスクリプションの詳細] ページで、古いサブスクリプションを "**中断**" に設定し、 **[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d32dc-173">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="d32dc-174">古いサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="d32dc-174">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="d32dc-175">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="d32dc-175">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="d32dc-176">お客様には、古いサブスクリプションに対して追加料金は発生しません。</span><span class="sxs-lookup"><span data-stu-id="d32dc-176">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



