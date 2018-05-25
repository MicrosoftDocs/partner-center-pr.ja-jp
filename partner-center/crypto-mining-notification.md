---
title: クリプトマイニング アクティビティに関するパートナー ダッシュボード通知 | パートナー ダッシュボード
description: 発生している可能性があるクリプトマイニングに関する通知です。
author: v-petand
Keywords: crypto-mining, cryptocurrency mining, security
robots: noindex, nofollow
ms.openlocfilehash: 1e7e695ec19600fd1f32138982c8f609db168cc7
ms.sourcegitcommit: 2d3203dd5e2653af031a8009aa3b999a454acef5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/10/2018
---
# <a name="partner-dashboard-notification-for-cryptocurrency-mining-activity"></a><span data-ttu-id="ad412-103">クリプトマイニング (仮想通貨の採掘) アクティビティに関するパートナー ダッシュボード通知</span><span class="sxs-lookup"><span data-stu-id="ad412-103">Partner Dashboard notification for cryptocurrency mining activity</span></span>

**<span data-ttu-id="ad412-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="ad412-104">Applies to</span></span>**

-  <span data-ttu-id="ad412-105">パートナー ダッシュボード</span><span class="sxs-lookup"><span data-stu-id="ad412-105">Partner Dashboard</span></span>
-  <span data-ttu-id="ad412-106">CSP パートナー</span><span class="sxs-lookup"><span data-stu-id="ad412-106">CSP partners</span></span>

<span data-ttu-id="ad412-107">パートナー ダッシュボードに、クリプトマイニングに関する次のような通知が届くことがあります。</span><span class="sxs-lookup"><span data-stu-id="ad412-107">You may have received the following Partner Dashboard notification about cryptocurrency mining:</span></span>
 
![](images/crypto1.png)

<span data-ttu-id="ad412-108">この通知では、過去 1 週間以内に 1 つ以上の Azure サブスクリプションでクリプトマイニングが検出されたことをお知らせしています。</span><span class="sxs-lookup"><span data-stu-id="ad412-108">The purpose of this notification is to inform you that we've detected cryptocurrency mining on one or more of your Azure subscriptions within the past week.</span></span> <span data-ttu-id="ad412-109">クリプトマイニングは必ずしも不正行為に相当するとは限りません。</span><span class="sxs-lookup"><span data-stu-id="ad412-109">Cryptocurrency mining does not necessarily equal fraudulent activity.</span></span> <span data-ttu-id="ad412-110">ただし、Azure でのクリプトマイニング実行によるコストが金銭的な利益を上回る傾向にあるため、通常ではない行為であると言えます。</span><span class="sxs-lookup"><span data-stu-id="ad412-110">However, it's unusual because the cost of running cryptocurrency mining in Azure tends to outweigh any potential financial rewards.</span></span> <span data-ttu-id="ad412-111">皆様や皆様の顧客に影響する金融詐欺を防ぐには、次の手順をご検討ください。</span><span class="sxs-lookup"><span data-stu-id="ad412-111">To protect against financial fraud that may impact you or your customer, consider the following steps:</span></span>

1.  <span data-ttu-id="ad412-112">顧客のアカウントが良好な状態であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="ad412-112">Review and confirm that the customer account is in good standing.</span></span> <span data-ttu-id="ad412-113">通知をクリックすると、サブスクリプションに直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="ad412-113">You can access the subscription directly by clicking on the notification.</span></span>

2.  <span data-ttu-id="ad412-114">サブスクリプションの Azure 利用パターンを確認します。</span><span class="sxs-lookup"><span data-stu-id="ad412-114">Review Azure usage patterns for the subscription.</span></span> <span data-ttu-id="ad412-115">突発的な急増があれば、予想外のアクティビティを示している可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ad412-115">Sudden spikes may suggest unexpected activity.</span></span>

3.  <span data-ttu-id="ad412-116">顧客にご連絡のうえ、そのアクティビティが想定内のものであるかどうかをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="ad412-116">Contact the customer to confirm that the activity is expected.</span></span>

<span data-ttu-id="ad412-117">そのアクティビティが想定内のものである場合は、顧客の Azure サブスクリプションの詳細ページに戻り、クリプトマイニングが正当であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="ad412-117">If the activity is expected, return to the customer's Azure subscription detail page and confirm that the cryptocurrency mining is legitimate.</span></span> 


![](images/crypto2.png)

<span data-ttu-id="ad412-118">アクティビティが予想外のものである場合は、以下をご検討ください。</span><span class="sxs-lookup"><span data-stu-id="ad412-118">If the activity is unexpected, consider the following:</span></span>

1.  <span data-ttu-id="ad412-119">クリプトマイニング用の Azure リソースが不要であることを確認して削除します。これにより、Azure で料金がそれ以上発生することを回避できます。</span><span class="sxs-lookup"><span data-stu-id="ad412-119">Confirm that the Azure resources for cryptocurrency mining are not needed and delete them to avoid further Azure charges.</span></span>

2.  <span data-ttu-id="ad412-120">そもそも、そのリソースがどのように作成されたものであるのかを把握します。</span><span class="sxs-lookup"><span data-stu-id="ad412-120">Understand how the resources were created in the first place.</span></span> <span data-ttu-id="ad412-121">これには、Azure Resource Management ログによるリソース プロビジョニング アクティビティの確認が必要になることがあります。</span><span class="sxs-lookup"><span data-stu-id="ad412-121">This may require you to review the Azure Resource Management logs for resource provisioning activities.</span></span>

3.  <span data-ttu-id="ad412-122">サブスクリプションを作成したユーザーを確認する必要がある場合は、パートナー ダッシュボードのアクティビティ ログを確認します。</span><span class="sxs-lookup"><span data-stu-id="ad412-122">If you need to find out who created the subscription, review Partner Dashboard activity logs.</span></span>

<span data-ttu-id="ad412-123">クリプトマイニング アクティビティの検出はヒューリスティックに基づいたものであり、100% 正確ではない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ad412-123">Detection of cryptocurrency mining activities is based on heuristics and may not be 100% accurate.</span></span> <span data-ttu-id="ad412-124">不正行為やその他の許可されていないアクティビティに対する保護を行うには、ガバナンスと監視のシステムを備えてください。</span><span class="sxs-lookup"><span data-stu-id="ad412-124">Be sure to have governance and monitoring systems in place to protect against fraudulent or other unpermitted activities.</span></span> <span data-ttu-id="ad412-125">詳しくは、「[未払い、詐欺、不正使用](https://docs.microsoft.com/partner-center/non-payment--fraud--or-misuse)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="ad412-125">For more information, see [Non-payment, fraud, or misuse](https://docs.microsoft.com/partner-center/non-payment--fraud--or-misuse).</span></span>




