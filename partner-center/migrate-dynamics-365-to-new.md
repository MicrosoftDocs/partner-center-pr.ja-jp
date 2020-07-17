---
title: Dynamics 365 Business Edition の移行
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 有効期限が切れる前に、限定された Dynamics 365 Business Edition のプランを新しいバージョンに移行する方法について説明します。
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436831"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="c8dda-103">Dynamics 365 Business Edition プランの新しいバージョンへの移行</span><span class="sxs-lookup"><span data-stu-id="c8dda-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="c8dda-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="c8dda-104">**Applies to**</span></span>

- <span data-ttu-id="c8dda-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="c8dda-105">Partner Center</span></span>

<span data-ttu-id="c8dda-106">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="c8dda-106">**Appropriate roles**</span></span>
- <span data-ttu-id="c8dda-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="c8dda-107">Global admin</span></span>
- <span data-ttu-id="c8dda-108">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="c8dda-108">User admin</span></span>
- <span data-ttu-id="c8dda-109">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="c8dda-109">Admin agent</span></span>
- <span data-ttu-id="c8dda-110">販売代理店</span><span class="sxs-lookup"><span data-stu-id="c8dda-110">Sales agent</span></span>

<span data-ttu-id="c8dda-111">2019年1月1日より、Dynamics 365 Business Edition サブスクリプションをお持ちのお客様は、これらの従来のプランに更新できなくなります。既存のサブスクリプションは、有効期限が切れると自動的に更新されません。</span><span class="sxs-lookup"><span data-stu-id="c8dda-111">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="c8dda-112">サブスクリプションの詳細ページで、[日付] の [自動更新] の [日付] にサブスクリプションの状態が [有効期限切れ] に変わります。</span><span class="sxs-lookup"><span data-stu-id="c8dda-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="c8dda-113">顧客の継続性を確保するには、有効期限が切れたサブスクリプションを使用して、以下のサポートされているオプションに切り替える必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8dda-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="c8dda-114">顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="c8dda-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="c8dda-115">API (CREST またはパートナーセンター) を使用する場合は、サブスクリプションの終了日と自動更新 = False プロパティを評価することで、有効期限が切れたサブスクリプションを見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="c8dda-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="c8dda-116">該当するサブスクリプションは、2019年1月1日に自動更新 = False に設定されます。</span><span class="sxs-lookup"><span data-stu-id="c8dda-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="c8dda-117">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="c8dda-117">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="c8dda-118">Dynamics 365 Business Edition が廃止されています</span><span class="sxs-lookup"><span data-stu-id="c8dda-118">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="c8dda-119">Dynamics 365 for Finance and Operations (Business Edition)</span><span class="sxs-lookup"><span data-stu-id="c8dda-119">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="c8dda-120">Dynamics 365 for Team Members, Business edition</span><span class="sxs-lookup"><span data-stu-id="c8dda-120">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="c8dda-121">Dynamics Business Central-Dynamics 365 Business Edition の新しいプラン</span><span class="sxs-lookup"><span data-stu-id="c8dda-121">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="c8dda-122">新しい Dynamics Business Central を利用することで、お客様は財務、営業、サービス、操作を接続して、ビジネスプロセスを効率化し、顧客とのやり取りを改善し、より良い意思決定を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="c8dda-122">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="c8dda-123">Dynamics 365 Business Central はクラウドベースであり、クラウドソリューションプロバイダー (CSP) プログラムパートナーのみが利用できます。</span><span class="sxs-lookup"><span data-stu-id="c8dda-123">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="c8dda-124">Dynamics 365 Business Edition のお客様は、2020年6月30日まで、新しい Business Central プランに対する割引された移行料金を受け取ることができます。</span><span class="sxs-lookup"><span data-stu-id="c8dda-124">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="c8dda-125">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="c8dda-125">Transition customers to new product plans</span></span>

 <span data-ttu-id="c8dda-126">廃止された Sku から新しいバージョンに顧客を移動するには、次の手順を順番に実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8dda-126">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="c8dda-127">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="c8dda-127">Purchase the new subscription</span></span>
- <span data-ttu-id="c8dda-128">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="c8dda-128">Reassign current user licenses</span></span>
- <span data-ttu-id="c8dda-129">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="c8dda-129">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="c8dda-130">顧客の新しいプランを購入する</span><span class="sxs-lookup"><span data-stu-id="c8dda-130">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="c8dda-131">左側のナビゲーションから [ **Customers** ] を選択し、新しいサブスクリプションに移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="c8dda-131">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="c8dda-132">[**サブスクリプションの追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c8dda-132">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="c8dda-133">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="c8dda-133">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="c8dda-134">これで、お客様は古いサブスクリプションと新しいサブスクリプションの両方を使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="c8dda-134">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="c8dda-135">次の手順では、顧客のユーザーにライセンスを再割り当てします。</span><span class="sxs-lookup"><span data-stu-id="c8dda-135">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="c8dda-136">左側のナビゲーションから [ **Customers** ] を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="c8dda-136">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="c8dda-137">[**ユーザーとライセンス**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c8dda-137">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="c8dda-138">ライセンスをユーザーに再割り当てするには、ユーザーを選択し、[**ライセンスの管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c8dda-138">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="c8dda-139">[**ライセンスの管理**365] ページで、[Basic (限定されたプラン) のライセンス] チェックボックスをオンにして、顧客が移動しているサブスクリプションの新しいサービスプランを選択します。</span><span class="sxs-lookup"><span data-stu-id="c8dda-139">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="c8dda-140">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="c8dda-140">Select **Submit**.</span></span> <span data-ttu-id="c8dda-141">この操作は、新しいライセンスが必要なユーザーごとに行います。</span><span class="sxs-lookup"><span data-stu-id="c8dda-141">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="c8dda-142">新しいサブスクリプションにライセンスを移行したら、古いサブスクリプションを取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="c8dda-142">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="c8dda-143">左側のナビゲーションから [ **Customers** ] を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="c8dda-143">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="c8dda-144">[サブスクリプションの詳細] ページで、古いサブスクリプションを "**中断**" に設定し、[**送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c8dda-144">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="c8dda-145">古いサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="c8dda-145">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="c8dda-146">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="c8dda-146">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="c8dda-147">お客様には、古いサブスクリプションに対して追加料金は発生しません。</span><span class="sxs-lookup"><span data-stu-id="c8dda-147">Your customer will incur no additional costs for the old subscription.</span></span>
