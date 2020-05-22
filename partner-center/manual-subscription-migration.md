---
title: Qualified Dynamics 365 サブスクリプションの移行
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 既存のサブスクリプションの有効期限が切れる前に、qualified、basic Dynamics 365 サブスクリプションから新しいサブスクリプションに移行する方法について説明します。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Dynamics 365 プラン、更新プラン、新しい Dynamics 365 Sku
ms.openlocfilehash: cac5717a1f7b27537faa694dcf665a69a7226483
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795990"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="f3c15-104">Dynamics 365 および Customer Engagement プランの Basic (対象プラン) から新しいバージョンへの移行</span><span class="sxs-lookup"><span data-stu-id="f3c15-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="f3c15-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="f3c15-105">**Applies to**</span></span>

-  <span data-ttu-id="f3c15-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="f3c15-106">Partner Center</span></span>

<span data-ttu-id="f3c15-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="f3c15-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="f3c15-108">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="f3c15-108">Global admin</span></span>
-   <span data-ttu-id="f3c15-109">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="f3c15-109">User admin</span></span>
-   <span data-ttu-id="f3c15-110">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="f3c15-110">Admin agent</span></span>
-   <span data-ttu-id="f3c15-111">販売代理店</span><span class="sxs-lookup"><span data-stu-id="f3c15-111">Sales agent</span></span>

<span data-ttu-id="f3c15-112">2019年1月1日より、Basic (認定提供) サブスクリプションの Dynamics 365 for Sales/Customer Engagement プランをお持ちのお客様は、これらのレガシプランを更新できなくなります。既存のサブスクリプションは、有効期限が切れると自動的に更新されません。</span><span class="sxs-lookup"><span data-stu-id="f3c15-112">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="f3c15-113">サブスクリプションの詳細ページで、[日付] の [自動更新] の [日付] にサブスクリプションの状態が [有効期限切れ] に変わります。</span><span class="sxs-lookup"><span data-stu-id="f3c15-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="f3c15-114">顧客の継続性を確保するには、有効期限が切れたサブスクリプションを使用して、以下のサポートされているオプションに切り替える必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3c15-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="f3c15-115">顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="f3c15-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="f3c15-116">API (CREST またはパートナーセンター) を使用する場合は、サブスクリプションの終了日と自動更新 = False プロパティを評価することで、有効期限が切れたサブスクリプションを見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="f3c15-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="f3c15-117">該当するサブスクリプションは、2019年1月1日に自動更新 = False に設定されます。</span><span class="sxs-lookup"><span data-stu-id="f3c15-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="f3c15-118">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="f3c15-118">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="f3c15-119">Dynamics 365 の提供終了</span><span class="sxs-lookup"><span data-stu-id="f3c15-119">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="f3c15-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="f3c15-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f3c15-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (認定オファー) for 教職員</span><span class="sxs-lookup"><span data-stu-id="f3c15-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f3c15-122">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (認定オファー) for Students</span><span class="sxs-lookup"><span data-stu-id="f3c15-122">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f3c15-123">Dynamics 365 for Sales Enterprise Edition (Government 価格) CRMOL Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="f3c15-123">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f3c15-124">Dynamics 365 for Sales Enterprise Edition for CRM Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="f3c15-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f3c15-125">Dynamics 365 for Sales Enterprise Edition for CRM Basic (認定オファー) for 教職員</span><span class="sxs-lookup"><span data-stu-id="f3c15-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f3c15-126">学生向けの SA からの Dynamics 365 for Sales Enterprise Edition for CRM Basic (認定オファー)</span><span class="sxs-lookup"><span data-stu-id="f3c15-126">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f3c15-127">Dynamics 365 for Sales Enterprise Edition (Government 価格) From CRM Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="f3c15-127">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f3c15-128">CRM Basic 用 Dynamics 365 for Sales Enterprise Edition アドオン (修飾されるプラン)</span><span class="sxs-lookup"><span data-stu-id="f3c15-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f3c15-129">CRM Basic (認定オファー) 用の Dynamics 365 for Sales Enterprise Edition アドオン</span><span class="sxs-lookup"><span data-stu-id="f3c15-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f3c15-130">CRM Basic (認定オファー) for Students 用 Dynamics 365 for Sales Enterprise Edition アドオン</span><span class="sxs-lookup"><span data-stu-id="f3c15-130">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f3c15-131">CRM Basic 用 Dynamics 365 for Sales Enterprise Edition (Government 価格) アドオン (修飾されるプラン)</span><span class="sxs-lookup"><span data-stu-id="f3c15-131">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f3c15-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="f3c15-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f3c15-133">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government 価格) CRMOL Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="f3c15-133">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f3c15-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (認定オファー) for Students</span><span class="sxs-lookup"><span data-stu-id="f3c15-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f3c15-135">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (認定プラン) (教職員向け)</span><span class="sxs-lookup"><span data-stu-id="f3c15-135">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f3c15-136">Dynamics 365 Customer Engagement Plan Enterprise Edition for CRM Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="f3c15-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f3c15-137">Dynamics 365 カスタマーエンゲージメントプラン Enterprise Edition (Government 価格) (SA for CRM Basic) (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="f3c15-137">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f3c15-138">Dynamics 365 Customer Engagement Plan Enterprise Edition for CRM Basic (認定オファー) for Students</span><span class="sxs-lookup"><span data-stu-id="f3c15-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f3c15-139">Dynamics 365 カスタマーエンゲージメントプラン Enterprise Edition for CRM Basic (認定オファー) for 教職員</span><span class="sxs-lookup"><span data-stu-id="f3c15-139">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f3c15-140">Dynamics 365 Customer Engagement Plan Enterprise Edition アドオン for CRM Basic (修飾されるプラン)</span><span class="sxs-lookup"><span data-stu-id="f3c15-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f3c15-141">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government 価格) アドオン for CRM Basic (認定プラン)</span><span class="sxs-lookup"><span data-stu-id="f3c15-141">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f3c15-142">CRM Basic (修飾されるオファー) 用の Dynamics 365 カスタマーエンゲージメントプラン Enterprise Edition アドオン</span><span class="sxs-lookup"><span data-stu-id="f3c15-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f3c15-143">Dynamics 365 Customer Engagement Plan Enterprise Edition アドオン for CRM Basic (認定オファー) for 教職員</span><span class="sxs-lookup"><span data-stu-id="f3c15-143">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="f3c15-144">Basic (認定オファー) 置換プランからの Sales/Customer Engagement プランの Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="f3c15-144">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="f3c15-145">**提供終了**</span><span class="sxs-lookup"><span data-stu-id="f3c15-145">**Retired offers**</span></span>   

- <span data-ttu-id="f3c15-146">CRM Basic または CRMOL Basic (修飾プラン) からの Sales の Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="f3c15-146">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f3c15-147">CRM Basic または CRMOL Basic (限定プラン) からの Dynamics 365 カスタマーエンゲージメントプラン</span><span class="sxs-lookup"><span data-stu-id="f3c15-147">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="f3c15-148">**置換オプション**</span><span class="sxs-lookup"><span data-stu-id="f3c15-148">**Replacement options**</span></span>
- <span data-ttu-id="f3c15-149">Dynamics 365 for Sales Professional (新規)</span><span class="sxs-lookup"><span data-stu-id="f3c15-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="f3c15-150">Dynamics 365 for Sales Professional (新規)</span><span class="sxs-lookup"><span data-stu-id="f3c15-150">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="f3c15-151">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="f3c15-151">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="f3c15-152">Dynamics 365 Customer Engagement プランまたは</span><span class="sxs-lookup"><span data-stu-id="f3c15-152">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="f3c15-153">Dynamics 365 チームメンバー</span><span class="sxs-lookup"><span data-stu-id="f3c15-153">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="f3c15-154">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="f3c15-154">Transition customers to new product plans</span></span>

<span data-ttu-id="f3c15-155">廃止された Sku から新しいバージョンに顧客を移動するには、次の手順を順番に実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3c15-155">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="f3c15-156">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="f3c15-156">Purchase the new subscription</span></span>
- <span data-ttu-id="f3c15-157">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="f3c15-157">Reassign current user licenses</span></span>
- <span data-ttu-id="f3c15-158">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="f3c15-158">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="f3c15-159">顧客の新しいプランを購入する</span><span class="sxs-lookup"><span data-stu-id="f3c15-159">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="f3c15-160">左側のナビゲーションから [ **Customers** ] を選択し、新しいサブスクリプションに移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="f3c15-160">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="f3c15-161">[**サブスクリプションの追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="f3c15-161">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="f3c15-162">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="f3c15-162">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="f3c15-163">これで、お客様は古いサブスクリプションと新しいサブスクリプションの両方を使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="f3c15-163">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="f3c15-164">次の手順では、顧客のユーザーにライセンスを再割り当てします。</span><span class="sxs-lookup"><span data-stu-id="f3c15-164">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="f3c15-165">左側のナビゲーションから [ **Customers** ] を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="f3c15-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="f3c15-166">[**ユーザーとライセンス**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="f3c15-166">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="f3c15-167">ライセンスをユーザーに再割り当てするには、ユーザーを選択し、[**ライセンスの管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="f3c15-167">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="f3c15-168">[**ライセンスの管理**365] ページで、[Basic (限定されたプラン) のライセンス] チェックボックスをオンにして、顧客が移動しているサブスクリプションの新しいサービスプランを選択します。</span><span class="sxs-lookup"><span data-stu-id="f3c15-168">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="f3c15-169">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="f3c15-169">Select **Submit**.</span></span> <span data-ttu-id="f3c15-170">この操作は、新しいライセンスが必要なユーザーごとに行います。</span><span class="sxs-lookup"><span data-stu-id="f3c15-170">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="f3c15-171">新しいサブスクリプションにライセンスを移行したら、古いサブスクリプションを取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="f3c15-171">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="f3c15-172">左側のナビゲーションから [ **Customers** ] を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="f3c15-172">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="f3c15-173">[サブスクリプションの詳細] ページで、古いサブスクリプションを "**中断**" に設定し、[**送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="f3c15-173">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="f3c15-174">古いサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="f3c15-174">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="f3c15-175">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="f3c15-175">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="f3c15-176">お客様には、古いサブスクリプションに対して追加料金は発生しません。</span><span class="sxs-lookup"><span data-stu-id="f3c15-176">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



