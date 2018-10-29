---
title: 顧客向けに Azure の支出の予算を設定する | パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: 月末の Azure の請求金額が顧客にとって予期しない金額にならないように、パートナー センターで顧客ごとの月額予算を設定できます。
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 98b6a4839b599a43ba6c10506468be7dbd064d43
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/29/2018
ms.locfileid: "5794985"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="a91df-103">顧客向けに Azure の支出の予算を設定する</span><span class="sxs-lookup"><span data-stu-id="a91df-103">Set an Azure spending budget for your customers</span></span>

**<span data-ttu-id="a91df-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="a91df-104">Applies to</span></span>**

-  <span data-ttu-id="a91df-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="a91df-105">Partner Center</span></span>
-  <span data-ttu-id="a91df-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="a91df-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="a91df-107">Microsoft Cloud ドイツのパートナー センター</span><span class="sxs-lookup"><span data-stu-id="a91df-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="a91df-108">顧客が Azure の支出を予算内に収めることができるようにするため、月額支出予算を設定して Azure の請求が予想より高くならないようにすることができます。</span><span class="sxs-lookup"><span data-stu-id="a91df-108">To help customers manage their Azure spending, you can set a monthly spending budget so that their Azure bill isn’t higher than they anticipated.</span></span> <span data-ttu-id="a91df-109">Azure の支出予算を設定すると、月の途中に顧客の Azure 関連の支出を予算と比較できます。</span><span class="sxs-lookup"><span data-stu-id="a91df-109">Setting an Azure spending budget allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="a91df-110">この機能を使うと、次のことができます。</span><span class="sxs-lookup"><span data-stu-id="a91df-110">With this feature, you can:</span></span> 

-   <span data-ttu-id="a91df-111">顧客の支出が予算限度に近づいた場合にメールで通知を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="a91df-111">Be notified by email if a customer's spending is near the budget limit</span></span>
-   <span data-ttu-id="a91df-112">顧客の毎月の Azure コストの見込みを確認します。</span><span class="sxs-lookup"><span data-stu-id="a91df-112">Review your customers’ estimated Azure costs per month</span></span>
-   <span data-ttu-id="a91df-113">正しく構成されていないサービス、または詐欺を暗示する異常な利用状況の傾向を見つけます。</span><span class="sxs-lookup"><span data-stu-id="a91df-113">Spot a misconfigured service, or unusual usage trends that might suggest fraud</span></span>
-   <span data-ttu-id="a91df-114">お客様と連携して根本的な問題を特定し、コストを管理します。</span><span class="sxs-lookup"><span data-stu-id="a91df-114">Work with the customer to identify the root issue and manage costs</span></span>
-   <span data-ttu-id="a91df-115">貴社と顧客のニーズに合わせて、予算をより高い額に変更します。</span><span class="sxs-lookup"><span data-stu-id="a91df-115">Change the budget to a higher amount if you and your customer are comfortable with it</span></span>

<span data-ttu-id="a91df-116">Azure の支出データは推定値であり、実際の請求金額は異なることがあります。また、税、クレジット、調整額、または適用されることがあるその他の料金は値に反映されていません。</span><span class="sxs-lookup"><span data-stu-id="a91df-116">The Azure spending data is an estimate, actual billing amounts may vary, and the value does not reflect taxes, credits, adjustments, or other charges that may apply.</span></span> <span data-ttu-id="a91df-117">支出データは 1 日 1 回更新されます。</span><span class="sxs-lookup"><span data-stu-id="a91df-117">Spending data is refreshed once per day.</span></span> <span data-ttu-id="a91df-118">Azure ポータルでアカウント設定を変更しない限り、顧客の Azure サービスおよびリソースの使用は継続され、顧客に課金されます。</span><span class="sxs-lookup"><span data-stu-id="a91df-118">Customers will continue to use—and be charged for—Azure services and resources unless you change their account settings in the Azure portal.</span></span> 

> [!NOTE]  
> <span data-ttu-id="a91df-119">この機能はでサンド ボックスまたは Test in Production (TIP) アカウントで利用可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="a91df-119">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

**<span data-ttu-id="a91df-120">メール通知を有効にする</span><span class="sxs-lookup"><span data-stu-id="a91df-120">Turn on email notifications</span></span>**
1.  <span data-ttu-id="a91df-121">パートナー センター メニューで、 **Azure の支出**を選択します。</span><span class="sxs-lookup"><span data-stu-id="a91df-121">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="a91df-122">顧客の使用量が予算の 80% に達した場合に通知を受け取るには、**[メールの取得]** オプションをオンにします。</span><span class="sxs-lookup"><span data-stu-id="a91df-122">Toggle on the **Get emails** option to be notified when customers use 80% or more of their budget.</span></span> <span data-ttu-id="a91df-123">これにより、Azure の請求を監視できます。</span><span class="sxs-lookup"><span data-stu-id="a91df-123">This will help you keep an eye on your Azure bill.</span></span> <span data-ttu-id="a91df-124">通知を受け取る既定のメール アドレスを個人のアドレスなどに変更できます。</span><span class="sxs-lookup"><span data-stu-id="a91df-124">You can change the default email address to a personal or any other email to receive notifications.</span></span>

**<span data-ttu-id="a91df-125">予算を設定する</span><span class="sxs-lookup"><span data-stu-id="a91df-125">Set a budget</span></span>**
1.  <span data-ttu-id="a91df-126">パートナー センター メニューで、 **Azure の支出**を選択します。</span><span class="sxs-lookup"><span data-stu-id="a91df-126">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="a91df-127">予算を設定する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="a91df-127">Select the customer(s) you want to set a budget for.</span></span> 
3. <span data-ttu-id="a91df-128">**[毎月の予算]** ボックスに値を入力し、**[適用]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="a91df-128">Enter a value in the **Monthly budget** box and then select **Apply**.</span></span>
4.  <span data-ttu-id="a91df-129">現在の支出を確認するには、このページに戻ります。</span><span class="sxs-lookup"><span data-stu-id="a91df-129">To check current spending, return to this page.</span></span>
5.  <span data-ttu-id="a91df-130">個々の予算は、お客様の管理ページの **[Usage-based subscriptions]** (使用量ベースのサブスクリプション) で設定することもできます。</span><span class="sxs-lookup"><span data-stu-id="a91df-130">Individual budgets can also be set under **Usage-based subscriptions** on a customer management page.</span></span>

**<span data-ttu-id="a91df-131">予算を削除する</span><span class="sxs-lookup"><span data-stu-id="a91df-131">Remove a budget</span></span>**
1.  <span data-ttu-id="a91df-132">パートナー センター メニューで、 **Azure の支出**を選択します。</span><span class="sxs-lookup"><span data-stu-id="a91df-132">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="a91df-133">一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="a91df-133">Select customers from the list.</span></span>
3.  <span data-ttu-id="a91df-134">**[予算の削除]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="a91df-134">Select **Remove budget**.</span></span>

**<span data-ttu-id="a91df-135">明細コストを確認する</span><span class="sxs-lookup"><span data-stu-id="a91df-135">See itemized costs</span></span>**
1.  <span data-ttu-id="a91df-136">パートナー センター メニューで、**顧客**を選びます。</span><span class="sxs-lookup"><span data-stu-id="a91df-136">From the Partner Center menu, select **Customers**.</span></span>
2.  <span data-ttu-id="a91df-137">顧客の一覧からお客様を選びます。</span><span class="sxs-lookup"><span data-stu-id="a91df-137">From the customer list, select a customer.</span></span>
3.  <span data-ttu-id="a91df-138">お客様の管理ページで、**[Usage-based subscriptions]** (使用量ベースのサブスクリプション) からサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="a91df-138">On their customer management page, under **Usage-based subscriptions**, choose a subscription.</span></span> <span data-ttu-id="a91df-139">そのサブスクリプションの現在の推定使用量とサービスごとの明細コストの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="a91df-139">View its current estimated usage and a list of itemized costs by service.</span></span>


 

 



