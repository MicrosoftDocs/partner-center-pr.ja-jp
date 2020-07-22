---
title: 使用量ベースの課金
ms.topic: article
ms.date: 06/05/2020
Description: 使用量ベースの課金の詳細については、パートナーセンターを参照してください。毎月の使用率について課金されます。
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 33fbbe006d4ae92251e22f541af3a6fdc928f3ef
ms.sourcegitcommit: 54f823f0e02e0e7add737d78de74d8eba8d9f381
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/22/2020
ms.locfileid: "86875218"
---
# <a name="understand-usage-based-billing-for-monthly-pay-as-you-go-consumption-of-services"></a><span data-ttu-id="9d619-103">月額、従量課金制のサービスの使用量ベースの課金について</span><span class="sxs-lookup"><span data-stu-id="9d619-103">Understand usage-based billing for monthly, pay-as-you-go consumption of services</span></span>

- <span data-ttu-id="9d619-104">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="9d619-104">Partner Center</span></span>
- <span data-ttu-id="9d619-105">CSP プログラムのパートナー</span><span class="sxs-lookup"><span data-stu-id="9d619-105">Partners in the CSP program</span></span>

<span data-ttu-id="9d619-106">Azure サブスクリプションなどのオンラインサービスを購入すると、毎月の使用率に対して課金されます。</span><span class="sxs-lookup"><span data-stu-id="9d619-106">When you buy online services such as Azure subscriptions, you're billed for monthly usage rates.</span></span> <span data-ttu-id="9d619-107">使用量ベースのサービス (Azure など) は、消費量に基づく従量制で請求されます。</span><span class="sxs-lookup"><span data-stu-id="9d619-107">Usage-based services, such as Azure, are billed according to metered rates, based on consumption.</span></span>

<span data-ttu-id="9d619-108">Microsoft の一部の製品とサービスでは "従量課金制" の請求モデルが使用されており、使用したサービスに対してのみ請求されます。</span><span class="sxs-lookup"><span data-stu-id="9d619-108">Some Microsoft products and services use a "pay as you go" billing model, in which you are billed only for services used.</span></span> <span data-ttu-id="9d619-109">たとえば、Microsoft Azure ではこのモデルが使われています。</span><span class="sxs-lookup"><span data-stu-id="9d619-109">For example, Microsoft Azure uses this model.</span></span> 

## <a name="usage-billing-frequency"></a><span data-ttu-id="9d619-110">使用量の請求頻度</span><span class="sxs-lookup"><span data-stu-id="9d619-110">Usage billing frequency</span></span>

<span data-ttu-id="9d619-111">使用量ベースの製品では、**毎月の課金**のみを利用できます。</span><span class="sxs-lookup"><span data-stu-id="9d619-111">Only **monthly billing** is available for usage-based products.</span></span> <span data-ttu-id="9d619-112">毎月の課金の詳細については、「[月額料金と年間課金の相違点](billing-annual-monthly.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d619-112">For more information on monthly billing, see [Monthly and annual billing differences](billing-annual-monthly.md).</span></span>

<span data-ttu-id="9d619-113">使用量ベースのサブスクリプションは、**サブスクリプションの契約日**に月単位で課金されます。</span><span class="sxs-lookup"><span data-stu-id="9d619-113">Usage-based subscriptions are billed monthly, in arrears, on the **subscription anniversary date**.</span></span> <span data-ttu-id="9d619-114">たとえば、サブスクリプションの契約日が15日の場合、サービス期間15月15日から1月14日までの料金が請求されます。</span><span class="sxs-lookup"><span data-stu-id="9d619-114">For example, if the subscription anniversary date is the 15th, you will be charged on January 15 for the service period of December 15 to January 14.</span></span> <span data-ttu-id="9d619-115">1月15日から2月14日のサービス期間中は、2月15日にもう一度料金が請求されます。</span><span class="sxs-lookup"><span data-stu-id="9d619-115">You will be charged again on February 15 for the service period of January 15 to February 14.</span></span>

## <a name="usage-charges"></a><span data-ttu-id="9d619-116">利用料金</span><span class="sxs-lookup"><span data-stu-id="9d619-116">Usage charges</span></span>

<span data-ttu-id="9d619-117">サブスクリプションの契約日に生成された料金は、次の請求書と[調整ファイル](usage-based-recon-files.md)に表示されます。</span><span class="sxs-lookup"><span data-stu-id="9d619-117">The charges that are generated on the subscription anniversary date will appear on the following invoice and [reconciliation file](usage-based-recon-files.md).</span></span>

<span data-ttu-id="9d619-118">場合によっては、請求書に使用料が不足しているか、前月の使用量が当月の請求書に請求されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9d619-118">You may occasionally notice that some usage charges are missing from your invoice, or that usage from a previous month is charged in the current month's invoice.</span></span> <span data-ttu-id="9d619-119">これはエラーではありません。単に、サービスが発生した後でサービスにタイムスタンプが押されたことを意味します。</span><span class="sxs-lookup"><span data-stu-id="9d619-119">This is not an error; it simply means that the service was timestamped after the services occurred.</span></span> <span data-ttu-id="9d619-120">請求サイクルが終了してから24時間以内に報告された使用量は、翌月の請求書に表示されます。</span><span class="sxs-lookup"><span data-stu-id="9d619-120">Usage reported within 24 hours of the end of the billing cycle will appear on the next month's bill.</span></span>

## <a name="cancelling-usage-based-subscriptions"></a><span data-ttu-id="9d619-121">使用量ベースのサブスクリプションの取り消し</span><span class="sxs-lookup"><span data-stu-id="9d619-121">Cancelling usage-based subscriptions</span></span>

<span data-ttu-id="9d619-122">使用量ベースのサブスクリプションは、いつでも中断できます。</span><span class="sxs-lookup"><span data-stu-id="9d619-122">You can suspend usage-based subscriptions at any time.</span></span>

## <a name="pricing-for-usage"></a><span data-ttu-id="9d619-123">使用量の料金</span><span class="sxs-lookup"><span data-stu-id="9d619-123">Pricing for usage</span></span>

<span data-ttu-id="9d619-124">Azure CSP 価格表は毎月発行され、パートナー センターの [販売] > [料金とプラン] ページに掲載されます。</span><span class="sxs-lookup"><span data-stu-id="9d619-124">The Azure CSP Price List is published monthly and can be found on the Partner Center Sell->Pricing and Offers page.</span></span> <span data-ttu-id="9d619-125">価格は毎日のように変化し、価格表の [変更履歴] タブに表示されますのでご注意ください。</span><span class="sxs-lookup"><span data-stu-id="9d619-125">Please note prices can change daily and are reflected on the Change History tab of the Price List.</span></span>

<span data-ttu-id="9d619-126">使用料金は、1 日あたりの価格に基づいています。</span><span class="sxs-lookup"><span data-stu-id="9d619-126">Usage charges are based on daily prices.</span></span> <span data-ttu-id="9d619-127">この価格がサービス期間中に変更された場合は、サービス期間が日割りとなり、それぞれの期間が適切な価格で別々の明細行に記載されます。</span><span class="sxs-lookup"><span data-stu-id="9d619-127">If the price changes during the service period you will see a billing line for each prorated service period and applicable price.</span></span>
