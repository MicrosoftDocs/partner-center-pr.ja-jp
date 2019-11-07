---
title: 顧客向けに Azure の支出の予算を設定する | パートナー センター
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターでは、お客様ごとに月額料金を設定して、その月の終わりに Azure の請求を予測できないようにすることができます。
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 03901b4b17c744c0c91d732331842f6cb579bf88
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/06/2019
ms.locfileid: "73654070"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="bd5a9-103">顧客の Azure 支出の予算の設定</span><span class="sxs-lookup"><span data-stu-id="bd5a9-103">Set an Azure spending budget for your customers</span></span>

<span data-ttu-id="bd5a9-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="bd5a9-104">**Applies to**</span></span>

-  <span data-ttu-id="bd5a9-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="bd5a9-105">Partner Center</span></span>
-  <span data-ttu-id="bd5a9-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="bd5a9-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="bd5a9-107">お客様が Azure の支出を管理できるように、毎月の支出予算を設定して、Azure の請求額が予想よりも高くならないようにすることができます。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-107">To help customers manage their Azure spending, you can set a monthly spending budget so that their Azure bill isn't higher than they anticipated.</span></span> <span data-ttu-id="bd5a9-108">Azure の支出予算を設定すると、月の途中に顧客の Azure 関連の支出を予算と比較できます。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-108">Setting an Azure spending budget allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="bd5a9-109">この機能を使うと、次のことができます。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-109">With this feature, you can:</span></span> 

-   <span data-ttu-id="bd5a9-110">顧客の支出が予算限度に近づいた場合にメールで通知を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-110">Be notified by email if a customer's spending is near the budget limit</span></span>
-   <span data-ttu-id="bd5a9-111">顧客の推定 Azure コストを月あたりに確認する</span><span class="sxs-lookup"><span data-stu-id="bd5a9-111">Review your customers' estimated Azure costs per month</span></span>
-   <span data-ttu-id="bd5a9-112">正しく構成されていないサービス、または詐欺を暗示する異常な利用状況の傾向を見つけます。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-112">Spot a misconfigured service, or unusual usage trends that might suggest fraud</span></span>
-   <span data-ttu-id="bd5a9-113">お客様と連携して根本的な問題を特定し、コストを管理します。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-113">Work with the customer to identify the root issue and manage costs</span></span>
-   <span data-ttu-id="bd5a9-114">貴社と顧客のニーズに合わせて、予算をより高い額に変更します。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-114">Change the budget to a higher amount if you and your customer are comfortable with it</span></span>

<span data-ttu-id="bd5a9-115">Azure の支出データは推定値であり、実際の請求金額は異なることがあります。また、税、クレジット、調整額、または適用されることがあるその他の料金は値に反映されていません。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-115">The Azure spending data is an estimate, actual billing amounts may vary, and the value does not reflect taxes, credits, adjustments, or other charges that may apply.</span></span> <span data-ttu-id="bd5a9-116">支出データは 1 日 1 回更新されます。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-116">Spending data is refreshed once per day.</span></span> <span data-ttu-id="bd5a9-117">Azure ポータルでアカウント設定を変更しない限り、顧客の Azure サービスおよびリソースの使用は継続され、顧客に課金されます。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-117">Customers will continue to use—and be charged for—Azure services and resources unless you change their account settings in the Azure portal.</span></span> 

> [!NOTE]  
> <span data-ttu-id="bd5a9-118">この機能は、サンドボックスまたは Test in Production (TIP) アカウントでは使用できません。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-118">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="bd5a9-119">**メール通知を有効にする**</span><span class="sxs-lookup"><span data-stu-id="bd5a9-119">**Turn on email notifications**</span></span>
1.  <span data-ttu-id="bd5a9-120">パートナー センター メニューで、 **[Azure 利用状況]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-120">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="bd5a9-121">顧客の使用量が予算の 80% に達した場合に通知を受け取るには、 **[メールの取得]** オプションをオンにします。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-121">Toggle on the **Get emails** option to be notified when customers use 80% or more of their budget.</span></span> <span data-ttu-id="bd5a9-122">これにより、Azure の請求を監視できます。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-122">This will help you keep an eye on your Azure bill.</span></span> <span data-ttu-id="bd5a9-123">通知を受け取る既定のメール アドレスを個人のアドレスなどに変更できます。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-123">You can change the default email address to a personal or any other email to receive notifications.</span></span>

<span data-ttu-id="bd5a9-124">**予算を設定する**</span><span class="sxs-lookup"><span data-stu-id="bd5a9-124">**Set a budget**</span></span>
1.  <span data-ttu-id="bd5a9-125">パートナー センター メニューで、 **[Azure 利用状況]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-125">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="bd5a9-126">予算を設定する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-126">Select the customer(s) you want to set a budget for.</span></span> 
3. <span data-ttu-id="bd5a9-127">**[毎月の予算]** ボックスに値を入力し、 **[適用]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-127">Enter a value in the **Monthly budget** box and then select **Apply**.</span></span>
4.  <span data-ttu-id="bd5a9-128">現在の支出を確認するには、このページに戻ります。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-128">To check current spending, return to this page.</span></span>
5.  <span data-ttu-id="bd5a9-129">個々の予算は、お客様の管理ページの **[Usage-based subscriptions]** (使用量ベースのサブスクリプション) で設定することもできます。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-129">Individual budgets can also be set under **Usage-based subscriptions** on a customer management page.</span></span>

<span data-ttu-id="bd5a9-130">**予算を削除する**</span><span class="sxs-lookup"><span data-stu-id="bd5a9-130">**Remove a budget**</span></span>
1.  <span data-ttu-id="bd5a9-131">パートナー センター メニューで、 **[Azure 利用状況]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-131">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="bd5a9-132">一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-132">Select customers from the list.</span></span>
3.  <span data-ttu-id="bd5a9-133">**[予算の削除]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-133">Select **Remove budget**.</span></span>

<span data-ttu-id="bd5a9-134">**明細コストを確認する**</span><span class="sxs-lookup"><span data-stu-id="bd5a9-134">**See itemized costs**</span></span>
1.  <span data-ttu-id="bd5a9-135">パートナー センター メニューで、 **[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-135">From the Partner Center menu, select **Customers**.</span></span>
2.  <span data-ttu-id="bd5a9-136">顧客の一覧からお客様を選びます。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-136">From the customer list, select a customer.</span></span>
3.  <span data-ttu-id="bd5a9-137">お客様の管理ページで、 **[Usage-based subscriptions]** (使用量ベースのサブスクリプション) からサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-137">On their customer management page, under **Usage-based subscriptions**, choose a subscription.</span></span> <span data-ttu-id="bd5a9-138">そのサブスクリプションの現在の推定使用量とサービスごとの明細コストの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="bd5a9-138">View its current estimated usage and a list of itemized costs by service.</span></span>


 

 



