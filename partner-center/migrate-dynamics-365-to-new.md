---
title: Dynamics 365 Business Edition の移行
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 有効期限が切れる前に、資格のある Dynamics 365 Business Edition オファーを新しいバージョンに移行する方法について学習します。
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151527"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="586b7-103">Dynamics 365 Business Edition プランの新しいバージョンへの移行</span><span class="sxs-lookup"><span data-stu-id="586b7-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="586b7-104">**適切なロール**: グローバル管理者|ユーザー管理管理者|管理エージェント |セールス エージェント</span><span class="sxs-lookup"><span data-stu-id="586b7-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="586b7-105">2019 年 1 月 1 日より、Dynamics 365 Business Edition サブスクリプションをお持ちのお客様は、これらのレガシ オファーに更新できなくなりました。既存のサブスクリプションは、有効期限が切れると自動的に更新されません。</span><span class="sxs-lookup"><span data-stu-id="586b7-105">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="586b7-106">サブスクリプションの詳細ページで、サブスクリプションの状態が "[日付] の自動更新" から "[日付] に有効期限が切れる" に変わります。</span><span class="sxs-lookup"><span data-stu-id="586b7-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="586b7-107">顧客の継続性を確保するには、サブスクリプションの有効期限が切れているユーザーを、以下に示すサポートされているオプションに移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="586b7-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="586b7-108">顧客のサービス停止を回避するために、サブスクリプションの年間終了日より前に顧客を新しいサブスクリプションに移行することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="586b7-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="586b7-109">API (THE または パートナー センター) を使用する場合は、サブスクリプションの終了日を自動更新 = False プロパティと共に評価することで、期限切れのサブスクリプションを見つける可能性があります。</span><span class="sxs-lookup"><span data-stu-id="586b7-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="586b7-110">問題のサブスクリプションは、2019 年 1 月 1 日に auto renew=False に設定されます。</span><span class="sxs-lookup"><span data-stu-id="586b7-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="586b7-111">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="586b7-111">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="586b7-112">廃止される Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="586b7-112">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="586b7-113">Dynamics 365 for Finance and Operations (Business Edition)</span><span class="sxs-lookup"><span data-stu-id="586b7-113">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="586b7-114">Dynamics 365 for Team Members, Business edition</span><span class="sxs-lookup"><span data-stu-id="586b7-114">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="586b7-115">Dynamics Business Central - Dynamics 365 Business Edition の新しいオファー</span><span class="sxs-lookup"><span data-stu-id="586b7-115">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="586b7-116">新しい Dynamics Business Central オファーを使用すると、顧客は財務、販売、サービス、運用を接続して、ビジネス プロセスを効率化し、顧客とのやり取りを改善し、より良い意思決定を行えます。</span><span class="sxs-lookup"><span data-stu-id="586b7-116">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="586b7-117">Dynamics 365 Business Central はクラウドベースであり、クラウド ソリューション プロバイダー (CSP) プログラム パートナーのみを通じて利用できます。</span><span class="sxs-lookup"><span data-stu-id="586b7-117">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="586b7-118">Dynamics 365 Business Edition のお客様は、2020 年 6 月 30 日まで、新しい Business Central オファーの割引切り替え価格を受け取る資格があります。</span><span class="sxs-lookup"><span data-stu-id="586b7-118">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="586b7-119">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="586b7-119">Transition customers to new product plans</span></span>

 <span data-ttu-id="586b7-120">廃止された SKU から新しい SKU に顧客を移行するには、この順序で次の手順が必要です。</span><span class="sxs-lookup"><span data-stu-id="586b7-120">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="586b7-121">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="586b7-121">Purchase the new subscription</span></span>
- <span data-ttu-id="586b7-122">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="586b7-122">Reassign current user licenses</span></span>
- <span data-ttu-id="586b7-123">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="586b7-123">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="586b7-124">顧客の新しいプランを購入する</span><span class="sxs-lookup"><span data-stu-id="586b7-124">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="586b7-125">左側 **のナビゲーション** から [顧客] を選択し、新しいサブスクリプションに移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="586b7-125">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="586b7-126">[サブスクリプション **の追加] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="586b7-126">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="586b7-127">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="586b7-127">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="586b7-128">これで、お客様は古いサブスクリプションと新しいサブスクリプションの両方を使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="586b7-128">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="586b7-129">次の手順では、顧客のユーザーにライセンスを再割り当てします。</span><span class="sxs-lookup"><span data-stu-id="586b7-129">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="586b7-130">左側のナビゲーションから [ **Customers** ] を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="586b7-130">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="586b7-131">[ **ユーザーとライセンス**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="586b7-131">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="586b7-132">ライセンスをユーザーに再割り当てするには、ユーザーを選択し、[ **ライセンスの管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="586b7-132">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="586b7-133">[ **ライセンスの管理** 365] ページで、[Basic (限定されたプラン) のライセンス] チェックボックスをオンにして、顧客が移動しているサブスクリプションの新しいサービスプランを選択します。</span><span class="sxs-lookup"><span data-stu-id="586b7-133">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="586b7-134">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="586b7-134">Select **Submit**.</span></span> <span data-ttu-id="586b7-135">この操作は、新しいライセンスが必要なユーザーごとに行います。</span><span class="sxs-lookup"><span data-stu-id="586b7-135">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="586b7-136">新しいサブスクリプションにライセンスを移行したら、古いサブスクリプションを取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="586b7-136">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="586b7-137">左側のナビゲーションから [ **Customers** ] を選択し、移動する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="586b7-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="586b7-138">[サブスクリプションの詳細] ページで、古いサブスクリプションを " **中断** " に設定し、[ **送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="586b7-138">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="586b7-139">古いサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="586b7-139">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="586b7-140">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="586b7-140">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="586b7-141">お客様には、古いサブスクリプションに対して追加料金は発生しません。</span><span class="sxs-lookup"><span data-stu-id="586b7-141">Your customer will incur no additional costs for the old subscription.</span></span>
