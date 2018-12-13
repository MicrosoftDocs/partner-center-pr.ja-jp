---
title: Basic (修飾プラン) から新しいバージョンへし、Dynamics 365 Customer Engagement プランの移行 |パートナー センター
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales/Basic (修飾を提供) サブスクリプションから Customer Engagement プランは更新されなくなったことができます。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968272"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="f9bf0-103">Basic (修飾プラン) から新しいバージョンにし、Dynamics 365 Customer Engagement プランを移行します。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

**<span data-ttu-id="f9bf0-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="f9bf0-104">Applies to</span></span>**

-  <span data-ttu-id="f9bf0-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="f9bf0-105">Partner Center</span></span>

<span data-ttu-id="f9bf0-106">Dynamics 365 for Sales を 2019 年 1 月 1 日、ユーザーに効果的な Basic (修飾を提供) サブスクリプションから Customer Engagement プランことができますこれらのレガシ プランの更新できなく/。期限が切れたとき、既存のサブスクリプションは自動的に更新されません。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-106">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="f9bf0-107">サブスクリプションの詳細ページで、サブスクリプションの状態は、「自動更新 [日付]」から「有効期限 [日付]」に変更されます。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-107">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="f9bf0-108">顧客の継続性を確認するを以下に、サポートされているオプション近づいたサブスクリプションを持つを移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-108">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="f9bf0-109">お客様のサービスが中断することを避けるため、サブスクリプションの年間終了日前に新しいサブスクリプションにお客様を移行することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-109">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="f9bf0-110">API (CREST またはパートナー センター) を使用する場合、自動と共に、サブスクリプションの終了日を評価することによって有効期限が切れるサブスクリプションの更新を検索できます = False プロパティ。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-110">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="f9bf0-111">対象のサブスクリプションは自動的に設定されます renew = False 2019 年 1 月 1 日にします。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-111">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="f9bf0-112">パートナー様はお客様をいつでも新しいプランに移行することができます。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-112">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="f9bf0-113">廃止される Dynamics 365 をプランします。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-113">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="f9bf0-114">Dynamics 365 販売 Enterprise Edition CRMOL basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9bf0-115">Dynamics 365 for Faculty 販売 Enterprise エディション CRMOL basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f9bf0-116">Dynamics 365 for Students 販売 Enterprise エディション CRMOL basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f9bf0-117">Dynamics 365 販売 Enterprise Edition (政府機関向け価格) CRMOL basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-117">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9bf0-118">CRM Basic (修飾プラン) 用の SA から Dynamics 365 を販売 Enterprise エディション</span><span class="sxs-lookup"><span data-stu-id="f9bf0-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9bf0-119">教職員用の CRM Basic (修飾プラン) 用の SA から Dynamics 365 を販売 Enterprise エディション</span><span class="sxs-lookup"><span data-stu-id="f9bf0-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f9bf0-120">学生用の CRM Basic (修飾プラン) 用の SA から Dynamics 365 を販売 Enterprise エディション</span><span class="sxs-lookup"><span data-stu-id="f9bf0-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f9bf0-121">CRM Basic (修飾プラン) 用の SA から Dynamics 365 を販売 Enterprise エディションの (政府機関向け価格)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-121">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9bf0-122">Dynamics 365 販売 Enterprise エディションのアドオンの CRM basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9bf0-123">Dynamics 365 販売 Enterprise エディションのアドオンの教職員用の CRM basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f9bf0-124">Dynamics 365 販売 Enterprise エディションのアドオンの学生用の CRM basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f9bf0-125">Dynamics 365 販売 Enterprise Edition (政府機関向け価格) アドオンの CRM basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-125">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9bf0-126">Dynamics 365 顧客契約計画 Enterprise Edition CRMOL Basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-126">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9bf0-127">Dynamics 365 顧客契約計画 Enterprise Edition (政府機関向け価格) CRMOL Basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-127">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9bf0-128">Dynamics 365 顧客エンゲージメント計画 Enterprise Edition CRMOL Basic (修飾プラン) for Students</span><span class="sxs-lookup"><span data-stu-id="f9bf0-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f9bf0-129">Dynamics 365 顧客エンゲージメント計画 Enterprise Edition CRMOL Basic (修飾プラン) for Faculty</span><span class="sxs-lookup"><span data-stu-id="f9bf0-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f9bf0-130">CRM Basic (修飾プラン) 用の SA から Dynamics 365 顧客契約計画 Enterprise エディション</span><span class="sxs-lookup"><span data-stu-id="f9bf0-130">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9bf0-131">Dynamics 365 顧客契約計画 Enterprise エディション (政府機関向け価格) CRM Basic (修飾プラン) 用の SA から</span><span class="sxs-lookup"><span data-stu-id="f9bf0-131">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9bf0-132">学生用の CRM Basic (修飾プラン) 用の SA から Dynamics 365 顧客契約計画 Enterprise エディション</span><span class="sxs-lookup"><span data-stu-id="f9bf0-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f9bf0-133">教職員用の CRM Basic (修飾プラン) 用の SA から Dynamics 365 顧客契約計画 Enterprise エディション</span><span class="sxs-lookup"><span data-stu-id="f9bf0-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f9bf0-134">Dynamics 365 顧客契約計画 Enterprise エディションのアドオン CRM Basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-134">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9bf0-135">Dynamics 365 顧客契約計画 Enterprise Edition (政府機関向け価格) のアドオン CRM Basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-135">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9bf0-136">Dynamics 365 顧客契約計画 Enterprise エディションのアドオン学生用の CRM Basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f9bf0-137">Dynamics 365 顧客契約計画 Enterprise エディションのアドオン教職員用の CRM Basic (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="f9bf0-138">Dynamics 365 for Sales/計画 (修飾を提供) Basic 代替から Customer Engagement プラン</span><span class="sxs-lookup"><span data-stu-id="f9bf0-138">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

**<span data-ttu-id="f9bf0-139">廃止されたプラン</span><span class="sxs-lookup"><span data-stu-id="f9bf0-139">Retired offers</span></span>**   

- <span data-ttu-id="f9bf0-140">Dynamics 365 for Sales から CRM Basic または CRMOL (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-140">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f9bf0-141">CRM Basic または CRMOL (修飾プラン) から Dynamics 365 Customer Engagement プラン</span><span class="sxs-lookup"><span data-stu-id="f9bf0-141">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

**<span data-ttu-id="f9bf0-142">代替オプション</span><span class="sxs-lookup"><span data-stu-id="f9bf0-142">Replacement options</span></span>**
- <span data-ttu-id="f9bf0-143">Dynamics 365 の販売 Professional (新機能)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="f9bf0-144">Dynamics 365 の販売 Professional (新機能)</span><span class="sxs-lookup"><span data-stu-id="f9bf0-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="f9bf0-145">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="f9bf0-145">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="f9bf0-146">Dynamics 365 Customer Engagement プランまたは</span><span class="sxs-lookup"><span data-stu-id="f9bf0-146">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="f9bf0-147">Dynamics 365 チームのメンバー</span><span class="sxs-lookup"><span data-stu-id="f9bf0-147">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="f9bf0-148">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="f9bf0-148">Transition customers to new product plans</span></span>

<span data-ttu-id="f9bf0-149">廃止された Sku から顧客を新しいものを移動するには、この順序で、次の手順が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-149">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="f9bf0-150">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="f9bf0-150">Purchase the new subscription</span></span>
- <span data-ttu-id="f9bf0-151">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="f9bf0-151">Reassign current user licenses</span></span>
- <span data-ttu-id="f9bf0-152">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="f9bf0-152">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="f9bf0-153">顧客の新しいプランを購入します。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-153">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="f9bf0-154">左側のナビゲーションから**顧客**を選択し、新しいサブスクリプションを移行する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-154">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="f9bf0-155">**[サブスクリプションの追加**を選択します。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-155">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="f9bf0-156">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-156">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="f9bf0-157">顧客以前のサブスクリプションと新しいの 1 つの両方がされます。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-157">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="f9bf0-158">次の手順では、顧客のユーザーへのライセンスをもう一度割り当てます。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-158">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="f9bf0-159">左側のナビゲーションから**顧客**を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-159">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="f9bf0-160">**[ユーザーとライセンス]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-160">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="f9bf0-161">ユーザーにライセンスを再割り当てするには、ユーザーを選択し、**ライセンスの管理**を選択します。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-161">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="f9bf0-162">**ライセンスの管理**] ページで、クリア for Sales、Dynamics 365/Basic (修飾提供) から Customer Engagement プランのライセンスのチェック ボックスと、お客様の移行先サブスクリプションの新しいサービス プランを選択します。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-162">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="f9bf0-163">**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-163">Select **Submit**.</span></span> <span data-ttu-id="f9bf0-164">これは、新しいライセンスを必要とする各ユーザーの行います。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-164">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="f9bf0-165">新しいサブスクリプションを経由でライセンスを移動した後は、以前のサブスクリプションを取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-165">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="f9bf0-166">左側のナビゲーションから**顧客**を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-166">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="f9bf0-167">サブスクリプションの詳細ページでは、以前のサブスクリプションを**中断**に設定し、**送信**を選択します。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-167">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="f9bf0-168">以前のサブスクリプションが一時停止できるようになりましたと新しいサブスクリプションがアクティブになっています。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-168">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="f9bf0-169">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-169">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="f9bf0-170">顧客が以前のサブスクリプションの追加コストが発生しません。</span><span class="sxs-lookup"><span data-stu-id="f9bf0-170">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



