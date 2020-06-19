---
title: Dynamics 365 Business Edition の移行
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 有効期限が切れる前に、限定された Dynamics 365 Business Edition のプランを新しいバージョンに移行する方法について説明します。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Dynamics 365 プラン、更新プラン、新しい Dynamics 365 Sku
ms.openlocfilehash: 9675f607d183c5d427371de4f09f088fd267c573
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/18/2020
ms.locfileid: "84992078"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="7c5b3-104">Dynamics 365 Business Edition プランの新しいバージョンへの移行</span><span class="sxs-lookup"><span data-stu-id="7c5b3-104">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="7c5b3-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="7c5b3-105">**Applies to**</span></span>

- <span data-ttu-id="7c5b3-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="7c5b3-106">Partner Center</span></span>

<span data-ttu-id="7c5b3-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="7c5b3-107">**Appropriate roles**</span></span>
- <span data-ttu-id="7c5b3-108">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="7c5b3-108">Global admin</span></span>
- <span data-ttu-id="7c5b3-109">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="7c5b3-109">User admin</span></span>
- <span data-ttu-id="7c5b3-110">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="7c5b3-110">Admin agent</span></span>
- <span data-ttu-id="7c5b3-111">販売代理店</span><span class="sxs-lookup"><span data-stu-id="7c5b3-111">Sales agent</span></span>

<span data-ttu-id="7c5b3-112">2019年1月1日より、Dynamics 365 Business Edition サブスクリプションをお持ちのお客様は、これらの従来のプランに更新できなくなります。既存のサブスクリプションは、有効期限が切れると自動的に更新されません。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-112">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="7c5b3-113">サブスクリプションの詳細ページで、[日付] の [自動更新] の [日付] にサブスクリプションの状態が [有効期限切れ] に変わります。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="7c5b3-114">顧客の継続性を確保するには、有効期限が切れたサブスクリプションを使用して、以下のサポートされているオプションに切り替える必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="7c5b3-115">顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="7c5b3-116">API (CREST またはパートナーセンター) を使用する場合は、サブスクリプションの終了日と自動更新 = False プロパティを評価することで、有効期限が切れたサブスクリプションを見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="7c5b3-117">該当するサブスクリプションは、2019年1月1日に自動更新 = False に設定されます。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="7c5b3-118">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-118">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="7c5b3-119">Dynamics 365 Business Edition が廃止されています</span><span class="sxs-lookup"><span data-stu-id="7c5b3-119">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="7c5b3-120">Dynamics 365 for Finance and Operations (Business Edition)</span><span class="sxs-lookup"><span data-stu-id="7c5b3-120">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="7c5b3-121">Dynamics 365 for Team Members, Business edition</span><span class="sxs-lookup"><span data-stu-id="7c5b3-121">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="7c5b3-122">Dynamics Business Central-Dynamics 365 Business Edition の新しいプラン</span><span class="sxs-lookup"><span data-stu-id="7c5b3-122">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="7c5b3-123">新しい Dynamics Business Central を利用することで、お客様は財務、営業、サービス、操作を接続して、ビジネスプロセスを効率化し、顧客とのやり取りを改善し、より良い意思決定を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-123">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="7c5b3-124">Dynamics 365 Business Central はクラウドベースであり、クラウドソリューションプロバイダー (CSP) プログラムパートナーのみが利用できます。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-124">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="7c5b3-125">Dynamics 365 Business Edition のお客様は、2020年6月30日まで、新しい Business Central プランに対する割引された移行料金を受け取ることができます。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-125">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="7c5b3-126">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="7c5b3-126">Transition customers to new product plans</span></span>

 <span data-ttu-id="7c5b3-127">廃止された Sku から新しいバージョンに顧客を移動するには、次の手順を順番に実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-127">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="7c5b3-128">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="7c5b3-128">Purchase the new subscription</span></span>
- <span data-ttu-id="7c5b3-129">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="7c5b3-129">Reassign current user licenses</span></span>
- <span data-ttu-id="7c5b3-130">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="7c5b3-130">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="7c5b3-131">顧客の新しいプランを購入する</span><span class="sxs-lookup"><span data-stu-id="7c5b3-131">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="7c5b3-132">左側のナビゲーションから [ **Customers** ] を選択し、新しいサブスクリプションに移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-132">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="7c5b3-133">[**サブスクリプションの追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-133">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="7c5b3-134">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-134">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="7c5b3-135">これで、お客様は古いサブスクリプションと新しいサブスクリプションの両方を使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-135">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="7c5b3-136">次の手順では、顧客のユーザーにライセンスを再割り当てします。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-136">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="7c5b3-137">左側のナビゲーションから [ **Customers** ] を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="7c5b3-138">[**ユーザーとライセンス**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-138">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="7c5b3-139">ライセンスをユーザーに再割り当てするには、ユーザーを選択し、[**ライセンスの管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-139">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="7c5b3-140">[**ライセンスの管理**365] ページで、[Basic (限定されたプラン) のライセンス] チェックボックスをオンにして、顧客が移動しているサブスクリプションの新しいサービスプランを選択します。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-140">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="7c5b3-141">**[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-141">Select **Submit**.</span></span> <span data-ttu-id="7c5b3-142">この操作は、新しいライセンスが必要なユーザーごとに行います。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-142">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="7c5b3-143">新しいサブスクリプションにライセンスを移行したら、古いサブスクリプションを取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-143">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="7c5b3-144">左側のナビゲーションから [ **Customers** ] を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-144">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="7c5b3-145">[サブスクリプションの詳細] ページで、古いサブスクリプションを "**中断**" に設定し、[**送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-145">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="7c5b3-146">古いサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-146">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="7c5b3-147">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-147">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="7c5b3-148">お客様には、古いサブスクリプションに対して追加料金は発生しません。</span><span class="sxs-lookup"><span data-stu-id="7c5b3-148">Your customer will incur no additional costs for the old subscription.</span></span>
