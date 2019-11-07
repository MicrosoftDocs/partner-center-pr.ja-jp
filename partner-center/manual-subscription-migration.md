---
title: Dynamics 365 および Customer Engagement プランを基本 (認定提供) から新しいバージョンに移行する |パートナーセンター
ms.topic: article
ms.date: 12/12/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Basic (認定オファー) サブスクリプションからの Sales/Customer Engagement プランの Dynamics 365 を更新することはできなくなりました。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 プラン、更新プラン、新しい Dynamics 365 Sku
ms.openlocfilehash: 354846973227fd292514454dd6f648934e5156ef
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653310"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="a84bc-104">Dynamics 365 および Customer Engagement プランの Basic (対象プラン) から新しいバージョンへの移行</span><span class="sxs-lookup"><span data-stu-id="a84bc-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="a84bc-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="a84bc-105">**Applies to**</span></span>

-  <span data-ttu-id="a84bc-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="a84bc-106">Partner Center</span></span>

<span data-ttu-id="a84bc-107">2019年1月1日より、Basic (認定提供) サブスクリプションの Dynamics 365 for Sales/Customer Engagement プランをお持ちのお客様は、これらのレガシプランを更新できなくなります。既存のサブスクリプションは、有効期限が切れると自動的に更新されません。</span><span class="sxs-lookup"><span data-stu-id="a84bc-107">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="a84bc-108">サブスクリプションの詳細ページで、[日付] の [自動更新] の [日付] にサブスクリプションの状態が [有効期限切れ] に変わります。</span><span class="sxs-lookup"><span data-stu-id="a84bc-108">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="a84bc-109">顧客の継続性を確保するには、有効期限が切れたサブスクリプションを使用して、以下のサポートされているオプションに切り替える必要があります。</span><span class="sxs-lookup"><span data-stu-id="a84bc-109">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="a84bc-110">顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="a84bc-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="a84bc-111">API (CREST またはパートナーセンター) を使用する場合は、サブスクリプションの終了日と自動更新 = False プロパティを評価することで、有効期限が切れたサブスクリプションを見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="a84bc-111">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="a84bc-112">該当するサブスクリプションは、2019年1月1日に自動更新 = False に設定されます。</span><span class="sxs-lookup"><span data-stu-id="a84bc-112">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="a84bc-113">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="a84bc-113">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="a84bc-114">Dynamics 365 の提供終了</span><span class="sxs-lookup"><span data-stu-id="a84bc-114">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="a84bc-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="a84bc-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="a84bc-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (認定オファー) for 教職員</span><span class="sxs-lookup"><span data-stu-id="a84bc-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="a84bc-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (認定オファー) for Students</span><span class="sxs-lookup"><span data-stu-id="a84bc-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="a84bc-118">Dynamics 365 for Sales Enterprise Edition (Government 価格) CRMOL Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="a84bc-118">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="a84bc-119">Dynamics 365 for Sales Enterprise Edition for CRM Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="a84bc-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="a84bc-120">Dynamics 365 for Sales Enterprise Edition for CRM Basic (認定オファー) for 教職員</span><span class="sxs-lookup"><span data-stu-id="a84bc-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="a84bc-121">学生向けの SA からの Dynamics 365 for Sales Enterprise Edition for CRM Basic (認定オファー)</span><span class="sxs-lookup"><span data-stu-id="a84bc-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="a84bc-122">Dynamics 365 for Sales Enterprise Edition (Government 価格) From CRM Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="a84bc-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="a84bc-123">CRM Basic 用 Dynamics 365 for Sales Enterprise Edition アドオン (修飾されるプラン)</span><span class="sxs-lookup"><span data-stu-id="a84bc-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="a84bc-124">CRM Basic (認定オファー) 用の Dynamics 365 for Sales Enterprise Edition アドオン</span><span class="sxs-lookup"><span data-stu-id="a84bc-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="a84bc-125">CRM Basic (認定オファー) for Students 用 Dynamics 365 for Sales Enterprise Edition アドオン</span><span class="sxs-lookup"><span data-stu-id="a84bc-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="a84bc-126">CRM Basic 用 Dynamics 365 for Sales Enterprise Edition (Government 価格) アドオン (修飾されるプラン)</span><span class="sxs-lookup"><span data-stu-id="a84bc-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="a84bc-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="a84bc-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="a84bc-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government 価格) CRMOL Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="a84bc-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="a84bc-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (認定オファー) for Students</span><span class="sxs-lookup"><span data-stu-id="a84bc-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="a84bc-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (認定プラン) (教職員向け)</span><span class="sxs-lookup"><span data-stu-id="a84bc-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="a84bc-131">Dynamics 365 Customer Engagement Plan Enterprise Edition for CRM Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="a84bc-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="a84bc-132">Dynamics 365 カスタマーエンゲージメントプラン Enterprise Edition (Government 価格) (SA for CRM Basic) (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="a84bc-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="a84bc-133">Dynamics 365 Customer Engagement Plan Enterprise Edition for CRM Basic (認定オファー) for Students</span><span class="sxs-lookup"><span data-stu-id="a84bc-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="a84bc-134">Dynamics 365 カスタマーエンゲージメントプラン Enterprise Edition for CRM Basic (認定オファー) for 教職員</span><span class="sxs-lookup"><span data-stu-id="a84bc-134">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="a84bc-135">Dynamics 365 Customer Engagement Plan Enterprise Edition アドオン for CRM Basic (修飾されるプラン)</span><span class="sxs-lookup"><span data-stu-id="a84bc-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="a84bc-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government 価格) アドオン for CRM Basic (認定プラン)</span><span class="sxs-lookup"><span data-stu-id="a84bc-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="a84bc-137">CRM Basic (修飾されるオファー) 用の Dynamics 365 カスタマーエンゲージメントプラン Enterprise Edition アドオン</span><span class="sxs-lookup"><span data-stu-id="a84bc-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="a84bc-138">Dynamics 365 Customer Engagement Plan Enterprise Edition アドオン for CRM Basic (認定オファー) for 教職員</span><span class="sxs-lookup"><span data-stu-id="a84bc-138">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="a84bc-139">Basic (認定オファー) 置換プランからの Sales/Customer Engagement プランの Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a84bc-139">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="a84bc-140">**提供終了**</span><span class="sxs-lookup"><span data-stu-id="a84bc-140">**Retired offers**</span></span>   

- <span data-ttu-id="a84bc-141">CRM Basic または CRMOL Basic (修飾プラン) からの Sales の Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a84bc-141">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="a84bc-142">CRM Basic または CRMOL Basic (限定プラン) からの Dynamics 365 カスタマーエンゲージメントプラン</span><span class="sxs-lookup"><span data-stu-id="a84bc-142">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="a84bc-143">**置換オプション**</span><span class="sxs-lookup"><span data-stu-id="a84bc-143">**Replacement options**</span></span>
- <span data-ttu-id="a84bc-144">Dynamics 365 for Sales Professional (新規)</span><span class="sxs-lookup"><span data-stu-id="a84bc-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="a84bc-145">Dynamics 365 for Sales Professional (新規)</span><span class="sxs-lookup"><span data-stu-id="a84bc-145">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="a84bc-146">顧客サービスの Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a84bc-146">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="a84bc-147">Dynamics 365 Customer Engagement プランまたは</span><span class="sxs-lookup"><span data-stu-id="a84bc-147">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="a84bc-148">Dynamics 365 チームメンバー</span><span class="sxs-lookup"><span data-stu-id="a84bc-148">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="a84bc-149">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="a84bc-149">Transition customers to new product plans</span></span>

<span data-ttu-id="a84bc-150">廃止された Sku から新しいバージョンに顧客を移動するには、次の手順を順番に実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a84bc-150">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="a84bc-151">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="a84bc-151">Purchase the new subscription</span></span>
- <span data-ttu-id="a84bc-152">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="a84bc-152">Reassign current user licenses</span></span>
- <span data-ttu-id="a84bc-153">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="a84bc-153">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="a84bc-154">顧客の新しいプランを購入する</span><span class="sxs-lookup"><span data-stu-id="a84bc-154">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="a84bc-155">左側のナビゲーションから **[Customers]** を選択し、新しいサブスクリプションに移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="a84bc-155">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="a84bc-156">**[サブスクリプションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a84bc-156">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="a84bc-157">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、 **[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="a84bc-157">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="a84bc-158">これで、お客様は古いサブスクリプションと新しいサブスクリプションの両方を使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="a84bc-158">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="a84bc-159">次の手順では、顧客のユーザーにライセンスを再割り当てします。</span><span class="sxs-lookup"><span data-stu-id="a84bc-159">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="a84bc-160">左側のナビゲーションから **[Customers]** を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="a84bc-160">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="a84bc-161">**[ユーザーとライセンス]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="a84bc-161">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="a84bc-162">ライセンスをユーザーに再割り当てするには、ユーザーを選択し、 **[ライセンスの管理]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a84bc-162">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="a84bc-163">[**ライセンスの管理**365] ページで、[Basic (限定されたプラン) のライセンス] チェックボックスをオンにして、顧客が移動しているサブスクリプションの新しいサービスプランを選択します。</span><span class="sxs-lookup"><span data-stu-id="a84bc-163">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="a84bc-164">**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="a84bc-164">Select **Submit**.</span></span> <span data-ttu-id="a84bc-165">この操作は、新しいライセンスが必要なユーザーごとに行います。</span><span class="sxs-lookup"><span data-stu-id="a84bc-165">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="a84bc-166">新しいサブスクリプションにライセンスを移行したら、古いサブスクリプションを取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="a84bc-166">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="a84bc-167">左側のナビゲーションから **[Customers]** を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="a84bc-167">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="a84bc-168">[サブスクリプションの詳細] ページで、古いサブスクリプションを "**中断**" に設定し、 **[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a84bc-168">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="a84bc-169">古いサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="a84bc-169">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="a84bc-170">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="a84bc-170">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="a84bc-171">お客様には、古いサブスクリプションに対して追加料金は発生しません。</span><span class="sxs-lookup"><span data-stu-id="a84bc-171">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



