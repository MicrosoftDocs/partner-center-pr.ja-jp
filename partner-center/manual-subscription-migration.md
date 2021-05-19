---
title: Qualified Dynamics 365 サブスクリプションの移行
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 既存のサブスクリプションの有効期限が切れる前に、qualified、basic Dynamics 365 サブスクリプションから新しいサブスクリプションに移行する方法について説明します。
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151646"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="7a2dd-103">Dynamics 365 および Customer Engagement プランの Basic (対象プラン) から新しいバージョンへの移行</span><span class="sxs-lookup"><span data-stu-id="7a2dd-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="7a2dd-104">**適切なロール**: 全体管理者 |ユーザー管理の管理者 |管理エージェント |営業担当者</span><span class="sxs-lookup"><span data-stu-id="7a2dd-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="7a2dd-105">2019年1月1日より、Basic (認定提供) サブスクリプションの Dynamics 365 for Sales/Customer Engagement プランをお持ちのお客様は、これらのレガシプランを更新できなくなります。既存のサブスクリプションは、有効期限が切れると自動的に更新されません。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-105">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="7a2dd-106">サブスクリプションの詳細ページで、[日付] の [自動更新] の [日付] にサブスクリプションの状態が [有効期限切れ] に変わります。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="7a2dd-107">顧客の継続性を確保するには、有効期限が切れたサブスクリプションを使用して、以下のサポートされているオプションに切り替える必要があります。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="7a2dd-108">顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="7a2dd-109">API (CREST またはパートナーセンター) を使用する場合は、サブスクリプションの終了日と自動更新 = False プロパティを評価することで、有効期限が切れたサブスクリプションを見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="7a2dd-110">該当するサブスクリプションは、2019年1月1日に自動更新 = False に設定されます。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="7a2dd-111">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-111">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="7a2dd-112">Dynamics 365 の提供終了</span><span class="sxs-lookup"><span data-stu-id="7a2dd-112">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="7a2dd-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="7a2dd-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7a2dd-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (認定オファー) for 教職員</span><span class="sxs-lookup"><span data-stu-id="7a2dd-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="7a2dd-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (認定オファー) for Students</span><span class="sxs-lookup"><span data-stu-id="7a2dd-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="7a2dd-116">Dynamics 365 for Sales Enterprise Edition (Government 価格) CRMOL Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="7a2dd-116">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7a2dd-117">Dynamics 365 for Sales Enterprise Edition for CRM Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="7a2dd-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7a2dd-118">Dynamics 365 for Sales Enterprise Edition for CRM Basic (認定オファー) for 教職員</span><span class="sxs-lookup"><span data-stu-id="7a2dd-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="7a2dd-119">学生向けの SA からの Dynamics 365 for Sales Enterprise Edition for CRM Basic (認定オファー)</span><span class="sxs-lookup"><span data-stu-id="7a2dd-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="7a2dd-120">Dynamics 365 for Sales Enterprise Edition (Government 価格) From CRM Basic (限定プラン)</span><span class="sxs-lookup"><span data-stu-id="7a2dd-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7a2dd-121">CRM Basic の Dynamics 365 for Sales Enterprise Edition Add-On (修飾プラン)</span><span class="sxs-lookup"><span data-stu-id="7a2dd-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7a2dd-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (資格のあるオファー) for Faculty</span><span class="sxs-lookup"><span data-stu-id="7a2dd-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="7a2dd-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (修飾オファー) for Students</span><span class="sxs-lookup"><span data-stu-id="7a2dd-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="7a2dd-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (限定オファー)</span><span class="sxs-lookup"><span data-stu-id="7a2dd-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7a2dd-125">Dynamics 365 Customer Engagement プラン Enterprise Edition CRMOL Basic (限定オファー)</span><span class="sxs-lookup"><span data-stu-id="7a2dd-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7a2dd-126">Dynamics 365 Customer Engagement プラン Enterprise Edition (Government 価格) CRMOL Basic (限定オファー)</span><span class="sxs-lookup"><span data-stu-id="7a2dd-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7a2dd-127">Dynamics 365 Customer Engagement プラン Enterprise Edition CRMOL Basic (限定オファー) for Students</span><span class="sxs-lookup"><span data-stu-id="7a2dd-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="7a2dd-128">Dynamics 365 Customer Engagement プラン Enterprise Edition CRMOL Basic (資格のあるオファー) for Faculty</span><span class="sxs-lookup"><span data-stu-id="7a2dd-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="7a2dd-129">Dynamics 365 Customer Engagement プラン Enterprise Edition SA for CRM Basic (限定オファー) から</span><span class="sxs-lookup"><span data-stu-id="7a2dd-129">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7a2dd-130">Dynamics 365 Customer Engagement プラン Enterprise Edition (Government 価格) FROM SA for CRM Basic (限定オファー)</span><span class="sxs-lookup"><span data-stu-id="7a2dd-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7a2dd-131">Dynamics 365 Customer Engagement プラン Enterprise Edition SA for CRM Basic (資格のあるオファー) から受講者向けプラン</span><span class="sxs-lookup"><span data-stu-id="7a2dd-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="7a2dd-132">Dynamics 365 Customer Engagement プラン Enterprise Edition CRM Basic (資格のあるオファー) for Faculty の SA から</span><span class="sxs-lookup"><span data-stu-id="7a2dd-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="7a2dd-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (限定オファー)</span><span class="sxs-lookup"><span data-stu-id="7a2dd-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7a2dd-134">Dynamics 365 Customer Engagement プラン Enterprise Edition CRM Basic (限定オファー) Add-On (Government 価格) プラン</span><span class="sxs-lookup"><span data-stu-id="7a2dd-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7a2dd-135">Dynamics 365 Customer Engagement プラン Enterprise Edition Add-On CRM Basic (適格オファー) for Students</span><span class="sxs-lookup"><span data-stu-id="7a2dd-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="7a2dd-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (資格のあるオファー) for Faculty</span><span class="sxs-lookup"><span data-stu-id="7a2dd-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="7a2dd-137">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (修飾オファー) 交換プラン</span><span class="sxs-lookup"><span data-stu-id="7a2dd-137">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="7a2dd-138">**廃止されたオファー**</span><span class="sxs-lookup"><span data-stu-id="7a2dd-138">**Retired offers**</span></span>   

- <span data-ttu-id="7a2dd-139">Dynamics 365 for Sales from CRM Basic または CRMOL Basic (限定オファー)</span><span class="sxs-lookup"><span data-stu-id="7a2dd-139">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="7a2dd-140">CRM Basic または CRMOL Basic (限定オファー) の Dynamics 365 Customer Engagement プラン</span><span class="sxs-lookup"><span data-stu-id="7a2dd-140">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="7a2dd-141">**置換オプション**</span><span class="sxs-lookup"><span data-stu-id="7a2dd-141">**Replacement options**</span></span>
- <span data-ttu-id="7a2dd-142">Dynamics 365 for Sales Professional (新規)</span><span class="sxs-lookup"><span data-stu-id="7a2dd-142">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="7a2dd-143">Dynamics 365 for Sales Professional (新規)</span><span class="sxs-lookup"><span data-stu-id="7a2dd-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="7a2dd-144">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="7a2dd-144">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="7a2dd-145">Dynamics 365 Customer Engagement プランまたは</span><span class="sxs-lookup"><span data-stu-id="7a2dd-145">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="7a2dd-146">Dynamics 365 チームメンバー</span><span class="sxs-lookup"><span data-stu-id="7a2dd-146">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="7a2dd-147">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="7a2dd-147">Transition customers to new product plans</span></span>

<span data-ttu-id="7a2dd-148">廃止された Sku から新しいバージョンに顧客を移動するには、次の手順を順番に実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-148">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="7a2dd-149">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="7a2dd-149">Purchase the new subscription</span></span>
- <span data-ttu-id="7a2dd-150">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="7a2dd-150">Reassign current user licenses</span></span>
- <span data-ttu-id="7a2dd-151">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="7a2dd-151">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="7a2dd-152">顧客の新しいプランを購入する</span><span class="sxs-lookup"><span data-stu-id="7a2dd-152">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="7a2dd-153">左側のナビゲーションから [ **Customers** ] を選択し、新しいサブスクリプションに移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-153">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="7a2dd-154">[ **サブスクリプションの追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-154">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="7a2dd-155">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-155">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="7a2dd-156">これで、お客様は古いサブスクリプションと新しいサブスクリプションの両方を使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-156">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="7a2dd-157">次の手順では、顧客のユーザーにライセンスを再割り当てします。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-157">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="7a2dd-158">左側のナビゲーションから [ **Customers** ] を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-158">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="7a2dd-159">[ **ユーザーとライセンス**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-159">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="7a2dd-160">ライセンスをユーザーに再割り当てするには、ユーザーを選択し、[ **ライセンスの管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-160">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="7a2dd-161">[ **ライセンスの管理** 365] ページで、[Basic (限定されたプラン) のライセンス] チェックボックスをオンにして、顧客が移動しているサブスクリプションの新しいサービスプランを選択します。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-161">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="7a2dd-162">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-162">Select **Submit**.</span></span> <span data-ttu-id="7a2dd-163">この操作は、新しいライセンスが必要なユーザーごとに行います。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-163">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="7a2dd-164">新しいサブスクリプションにライセンスを移行したら、古いサブスクリプションを取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-164">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="7a2dd-165">左側のナビゲーションから [ **Customers** ] を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="7a2dd-166">[サブスクリプションの詳細] ページで、古いサブスクリプションを " **中断** " に設定し、[ **送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-166">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="7a2dd-167">古いサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-167">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="7a2dd-168">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-168">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="7a2dd-169">お客様には、古いサブスクリプションに対して追加料金は発生しません。</span><span class="sxs-lookup"><span data-stu-id="7a2dd-169">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



