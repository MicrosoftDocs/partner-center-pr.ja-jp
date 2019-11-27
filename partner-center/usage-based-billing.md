---
title: 使用量ベースの課金 |パートナーセンター
ms.topic: article
ms.date: 11/21/2019
Description: パートナーセンターでの使用量ベースの課金に関する情報。毎月の使用率に対して課金されます。
author: MaggiePucciEvans
ms.author: evansma
keywords: 課金、使用量ベース、使用量
ms.localizationpriority: medium
ms.openlocfilehash: c92c6f9014a40a0f8804ba83ba7cc85939e90281
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389740"
---
# <a name="usage-based-billing"></a><span data-ttu-id="c2c4e-104">使用量ベースの課金</span><span class="sxs-lookup"><span data-stu-id="c2c4e-104">Usage-based billing</span></span>

- <span data-ttu-id="c2c4e-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="c2c4e-105">Partner Center</span></span>
- <span data-ttu-id="c2c4e-106">CSP プログラムのパートナー</span><span class="sxs-lookup"><span data-stu-id="c2c4e-106">Partners in the CSP program</span></span>

<span data-ttu-id="c2c4e-107">Azure サブスクリプションなどのオンライン サービスを購入すると、月単位の使用率に対して請求されます。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-107">When you buy online services such as Azure subscriptions, you’re billed for monthly usage rates.</span></span> <span data-ttu-id="c2c4e-108">使用量ベースのサービス (Azure など) は、消費量に基づく従量制で請求されます。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-108">Usage-based services, such as Azure, are billed according to metered rates, based on consumption.</span></span>

<span data-ttu-id="c2c4e-109">Microsoft の一部の製品とサービスでは "従量課金制" の請求モデルが使用されており、使用したサービスに対してのみ請求されます。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-109">Some Microsoft products and services use a "pay as you go" billing model, in which you are billed only for services used.</span></span> <span data-ttu-id="c2c4e-110">たとえば、Microsoft Azure ではこのモデルが使われています。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-110">For example, Microsoft Azure uses this model.</span></span> 

## <a name="usage-billing-frequency"></a><span data-ttu-id="c2c4e-111">使用量の請求頻度</span><span class="sxs-lookup"><span data-stu-id="c2c4e-111">Usage billing frequency</span></span>

<span data-ttu-id="c2c4e-112">使用量ベースの製品では、**毎月の課金**のみを利用できます。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-112">Only **monthly billing** is available for usage-based products.</span></span> <span data-ttu-id="c2c4e-113">毎月の課金の詳細については、「[月額料金と年間課金の相違点](billing-annual-monthly.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-113">For more information on monthly billing, see [Monthly and annual billing differences](billing-annual-monthly.md).</span></span>

<span data-ttu-id="c2c4e-114">使用量ベースのサブスクリプションは、**サブスクリプションの契約日**に月単位で課金されます。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-114">Usage-based subscriptions are billed monthly, in arrears, on the **subscription anniversary date**.</span></span> <span data-ttu-id="c2c4e-115">たとえば、サブスクリプションの契約日が15日の場合、サービス期間の12月15日から1月14日までの料金が請求されます。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-115">For example, if the subscription anniversary date is the 15th, you will be charged on January 15th for the service period of December 15th to January 14th.</span></span> <span data-ttu-id="c2c4e-116">サービス期間15月15日から2月14日まで、2月15日にもう一度料金が請求されます。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-116">You will be charged again on February 15th for the service period of January 15th to February 14th.</span></span> 

## <a name="usage-charges"></a><span data-ttu-id="c2c4e-117">利用料金</span><span class="sxs-lookup"><span data-stu-id="c2c4e-117">Usage charges</span></span>

<span data-ttu-id="c2c4e-118">サブスクリプションの契約日に生成された料金は、次の請求書と[調整ファイル](usage-based-recon-files.md)に表示されます。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-118">The charges that are generated on the subscription anniversary date will appear on the following invoice and [reconciliation file](usage-based-recon-files.md).</span></span>

<span data-ttu-id="c2c4e-119">請求書から漏れている使用量請求がある、または前月の使用量が当月の請求書で請求されている、といったことに気付く場合があります。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-119">You may occasionally notice that some usage charges are missing from your invoice, or that usage from a previous month is charged in the current month’s invoice.</span></span> <span data-ttu-id="c2c4e-120">これはエラーではありません。単に、サービスが発生した後でサービスにタイムスタンプが押されたことを意味します。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-120">This is not an error; it simply means that the service was timestamped after the services occurred.</span></span> <span data-ttu-id="c2c4e-121">請求サイクルの最後の 24 時間以内に報告された使用は、次の月の請求書に表示されます。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-121">Usage reported within 24 hours of the end of the billing cycle will appear on the next month’s bill.</span></span>

## <a name="cancelling-usage-based-subscriptions"></a><span data-ttu-id="c2c4e-122">使用量ベースのサブスクリプションの取り消し</span><span class="sxs-lookup"><span data-stu-id="c2c4e-122">Cancelling usage-based subscriptions</span></span>

<span data-ttu-id="c2c4e-123">使用量ベースのサブスクリプションは、いつでも中断できます。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-123">You can suspend usage-based subscriptions at any time.</span></span>

## <a name="pricing-for-usage"></a><span data-ttu-id="c2c4e-124">使用量の料金</span><span class="sxs-lookup"><span data-stu-id="c2c4e-124">Pricing for usage</span></span>

<span data-ttu-id="c2c4e-125">Azure CSP 価格表は毎月発行され、パートナー センターの [販売] > [料金とプラン] ページに掲載されます。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-125">The Azure CSP Price List is published monthly and can be found on the Partner Center Sell->Pricing and Offers page.</span></span> <span data-ttu-id="c2c4e-126">価格は毎日のように変化し、価格表の [変更履歴] タブに表示されますのでご注意ください。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-126">Please note prices can change daily and are reflected on the Change History tab of the Price List.</span></span>

<span data-ttu-id="c2c4e-127">使用料金は、1 日あたりの価格に基づいています。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-127">Usage charges are based on daily prices.</span></span> <span data-ttu-id="c2c4e-128">この価格がサービス期間中に変更された場合は、サービス期間が日割りとなり、それぞれの期間が適切な価格で別々の明細行に記載されます。</span><span class="sxs-lookup"><span data-stu-id="c2c4e-128">If the price changes during the service period you will see a billing line for each prorated service period and applicable price.</span></span>
