---
title: Dynamics 365 と顧客エンゲージメント プランを Basic (修飾プラン) から新しいバージョンに移行 |パートナー センター
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales]、[Basic (修飾提供) のサブスクリプションから Customer Engagement プランは更新不要になったことができます。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 プラン、オファー、新しい Dynamics 365 の Sku を更新します。
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586945"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="f9e58-104">Dynamics 365 および Customer Engagement プランの Basic (対象プラン) から新しいバージョンへの移行</span><span class="sxs-lookup"><span data-stu-id="f9e58-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="f9e58-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="f9e58-105">**Applies to**</span></span>

-  <span data-ttu-id="f9e58-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="f9e58-106">Partner Center</span></span>

<span data-ttu-id="f9e58-107">Dynamics 365 for Sales で効果的な 2019 年 1 月 1日の顧客 (修飾提供) Basic サブスクリプションから Customer Engagement プランですこれらのレガシ プランを更新できなく/。有効期限が切れるときに、既存のサブスクリプションは自動的に更新されません。</span><span class="sxs-lookup"><span data-stu-id="f9e58-107">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="f9e58-108">サブスクリプションの詳細] ページで、サブスクリプションの状態は、「自動更新 [date]」から「有効期限 [date]」に変更されます。</span><span class="sxs-lookup"><span data-stu-id="f9e58-108">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="f9e58-109">お客様の継続性をできるように、以下に、サポートされているオプションに期限切れのサブスクリプションのあるものを移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f9e58-109">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="f9e58-110">お客様のサービスが中断することを避けるため、サブスクリプションの年間終了日前に新しいサブスクリプションにお客様を移行することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="f9e58-110">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="f9e58-111">(CREST またはパートナー センター) API を使用する場合、自動と共にサブスクリプションの終了日を評価することによって期限切れのサブスクリプションの更新を見つけることができます = False プロパティ。</span><span class="sxs-lookup"><span data-stu-id="f9e58-111">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="f9e58-112">対象のサブスクリプションは自動に設定されます更新 = False、2019 年 1 月 1 日を。</span><span class="sxs-lookup"><span data-stu-id="f9e58-112">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="f9e58-113">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="f9e58-113">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="f9e58-114">Dynamics 365 の提供が中止</span><span class="sxs-lookup"><span data-stu-id="f9e58-114">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="f9e58-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9e58-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9e58-116">Dynamics 365 for Faculty 販売の Enterprise Edition CRMOL basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9e58-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f9e58-117">Dynamics 365 の学生向け販売の Enterprise Edition CRMOL Basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9e58-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f9e58-118">Dynamics 365 for 販売の Enterprise Edition (政府機関向け価格) CRMOL Basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9e58-118">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9e58-119">Dynamics 365 営業の Enterprise Edition 用 CRM Basic (修飾プラン) 用の SA から</span><span class="sxs-lookup"><span data-stu-id="f9e58-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9e58-120">Dynamics 365 営業の Enterprise edition for Faculty CRM Basic (修飾プラン) 用の SA から</span><span class="sxs-lookup"><span data-stu-id="f9e58-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f9e58-121">学生向けの CRM Basic (修飾プラン) 用の SA から売上の Enterprise Edition 用 Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="f9e58-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f9e58-122">Dynamics 365 (政府機関向け価格) 販売の Enterprise Edition 用 CRM Basic (修飾プラン) 用の SA から</span><span class="sxs-lookup"><span data-stu-id="f9e58-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9e58-123">Dynamics 365 営業の Enterprise Edition のアドオンの CRM basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9e58-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9e58-124">Dynamics 365 営業の Enterprise Edition のアドオンの CRM basic (修飾プラン) for Faculty</span><span class="sxs-lookup"><span data-stu-id="f9e58-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f9e58-125">Dynamics 365 営業の Enterprise Edition のアドオンの学生向けの CRM basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9e58-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f9e58-126">Dynamics 365 営業の Enterprise Edition (政府機関向け価格) のアドオンの CRM basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9e58-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9e58-127">Dynamics 365 Customer Engagement プラン Enterprise Edition CRMOL Basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9e58-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9e58-128">Dynamics 365 Customer Engagement プラン Enterprise Edition (政府機関向け価格) CRMOL Basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9e58-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9e58-129">Dynamics 365 Customer Engagement プラン Enterprise Edition CRMOL Basic (修飾プラン) for Students</span><span class="sxs-lookup"><span data-stu-id="f9e58-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f9e58-130">Dynamics 365 Customer Engagement プラン Enterprise Edition CRMOL Basic (修飾プラン) for Faculty</span><span class="sxs-lookup"><span data-stu-id="f9e58-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f9e58-131">CRM Basic (修飾プラン) 用の SA から Dynamics 365 Customer Engagement プラン Enterprise Edition</span><span class="sxs-lookup"><span data-stu-id="f9e58-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9e58-132">Dynamics 365 Customer Engagement プラン Enterprise Edition (政府機関向け価格) CRM の Basic (修飾プラン) 用の SA から</span><span class="sxs-lookup"><span data-stu-id="f9e58-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9e58-133">学生向けの CRM Basic (修飾プラン) 用の SA から Dynamics 365 Customer Engagement プラン Enterprise Edition</span><span class="sxs-lookup"><span data-stu-id="f9e58-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f9e58-134">For Faculty CRM Basic (修飾プラン) 用の SA から Dynamics 365 Customer Engagement プラン Enterprise Edition</span><span class="sxs-lookup"><span data-stu-id="f9e58-134">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f9e58-135">Dynamics 365 Customer Engagement プラン Enterprise Edition アドオン CRM basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9e58-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9e58-136">Dynamics 365 Customer Engagement プラン Enterprise Edition (政府機関向け価格) アドオン CRM basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9e58-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9e58-137">Dynamics 365 Customer Engagement プラン Enterprise Edition アドオン CRM basic (修飾プラン) の学生向け</span><span class="sxs-lookup"><span data-stu-id="f9e58-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f9e58-138">Dynamics 365 Customer Engagement プラン Enterprise Edition アドオン for Faculty CRM basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9e58-138">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="f9e58-139">Dynamics 365 for Sales]、[プラン (修飾提供) Basic 置換から Customer Engagement の計画</span><span class="sxs-lookup"><span data-stu-id="f9e58-139">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="f9e58-140">**提供終了になったプラン**</span><span class="sxs-lookup"><span data-stu-id="f9e58-140">**Retired offers**</span></span>   

- <span data-ttu-id="f9e58-141">CRM Basic または CRMOL (修飾プラン) からの売り上げ高の Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="f9e58-141">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9e58-142">CRM Basic または CRMOL (修飾プラン) から Dynamics 365 Customer Engagement プラン</span><span class="sxs-lookup"><span data-stu-id="f9e58-142">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="f9e58-143">**置換オプション**</span><span class="sxs-lookup"><span data-stu-id="f9e58-143">**Replacement options**</span></span>
- <span data-ttu-id="f9e58-144">Dynamics 365 for Sales Professional (新規)</span><span class="sxs-lookup"><span data-stu-id="f9e58-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="f9e58-145">Dynamics 365 for Sales Professional (新規)</span><span class="sxs-lookup"><span data-stu-id="f9e58-145">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="f9e58-146">Dynamics 365 のカスタマー サービスについて</span><span class="sxs-lookup"><span data-stu-id="f9e58-146">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="f9e58-147">Dynamics 365 Customer Engagement プランまたは</span><span class="sxs-lookup"><span data-stu-id="f9e58-147">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="f9e58-148">Dynamics 365 のチーム メンバー</span><span class="sxs-lookup"><span data-stu-id="f9e58-148">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="f9e58-149">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="f9e58-149">Transition customers to new product plans</span></span>

<span data-ttu-id="f9e58-150">提供終了になった Sku から新しいものに顧客を移動すると、この順序で次の手順が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9e58-150">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="f9e58-151">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="f9e58-151">Purchase the new subscription</span></span>
- <span data-ttu-id="f9e58-152">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="f9e58-152">Reassign current user licenses</span></span>
- <span data-ttu-id="f9e58-153">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="f9e58-153">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="f9e58-154">お客様の新しいプランを購入します。</span><span class="sxs-lookup"><span data-stu-id="f9e58-154">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="f9e58-155">選択**顧客**から、左側のナビゲーションし、新しいサブスクリプションに移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="f9e58-155">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="f9e58-156">選択**サブスクリプション追加**します。</span><span class="sxs-lookup"><span data-stu-id="f9e58-156">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="f9e58-157">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="f9e58-157">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="f9e58-158">古いサブスクリプションと、新しい顧客になりますようになりました。</span><span class="sxs-lookup"><span data-stu-id="f9e58-158">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="f9e58-159">次の手順では、お客様のユーザーにライセンスを再割り当ています。</span><span class="sxs-lookup"><span data-stu-id="f9e58-159">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="f9e58-160">選択**顧客**から、左側のナビゲーションと選択し、顧客が移動します。</span><span class="sxs-lookup"><span data-stu-id="f9e58-160">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="f9e58-161">**[ユーザーとライセンス]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="f9e58-161">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="f9e58-162">ユーザーにライセンスを再割り当てするユーザーを選択し、**ライセンスを管理する**します。</span><span class="sxs-lookup"><span data-stu-id="f9e58-162">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="f9e58-163">**ライセンスを管理する** ページで、Dynamics 365 for Sales の消去/(修飾提供) Basic から Customer Engagement プランのライセンスのチェック ボックスとへの移行は、顧客サブスクリプションの新しいサービス プランを選択します。</span><span class="sxs-lookup"><span data-stu-id="f9e58-163">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="f9e58-164">**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="f9e58-164">Select **Submit**.</span></span> <span data-ttu-id="f9e58-165">これは、新しいライセンスが必要とする各ユーザーの行います。</span><span class="sxs-lookup"><span data-stu-id="f9e58-165">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="f9e58-166">経由でライセンスを新しいサブスクリプションに移行した後は、古いサブスクリプションをキャンセルできます。</span><span class="sxs-lookup"><span data-stu-id="f9e58-166">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="f9e58-167">選択**顧客**から、左側のナビゲーションと選択し、顧客が移動します。</span><span class="sxs-lookup"><span data-stu-id="f9e58-167">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="f9e58-168">サブスクリプションの詳細 ページで、古いサブスクリプションを設定**Suspended**選択**送信**します。</span><span class="sxs-lookup"><span data-stu-id="f9e58-168">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="f9e58-169">古いサブスクリプションが中断されていますし、新しいサブスクリプションがアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="f9e58-169">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="f9e58-170">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="f9e58-170">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="f9e58-171">お客様には、古いサブスクリプションの追加のコストは生じません。</span><span class="sxs-lookup"><span data-stu-id="f9e58-171">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



