---
title: 有効な単価計算
ms.topic: how-to
ms.date: 04/02/2021
description: 有効な単価と計算方法について学習します。 この記事には、サンプル計算も含まれています。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147124"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="71fb9-104">Azure プランの消費に対する有効な単価の計算</span><span class="sxs-lookup"><span data-stu-id="71fb9-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="71fb9-105">**適切なロール**: 課金管理者</span><span class="sxs-lookup"><span data-stu-id="71fb9-105">**Appropriate roles**: Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="71fb9-106">有効な単価</span><span class="sxs-lookup"><span data-stu-id="71fb9-106">The effective unit price</span></span>

<span data-ttu-id="71fb9-107">有効な単価は、(リソース レベルではなく) メーター レベルで計算され、メーターの使用状況に応じて毎日調整されます。</span><span class="sxs-lookup"><span data-stu-id="71fb9-107">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="71fb9-108">次の 3 つの要因を使用して、有効な単価を計算します。</span><span class="sxs-lookup"><span data-stu-id="71fb9-108">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="71fb9-109">使用量。課金サイクル全体を通じて毎日監視されます</span><span class="sxs-lookup"><span data-stu-id="71fb9-109">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="71fb9-110">メーターの請求コスト</span><span class="sxs-lookup"><span data-stu-id="71fb9-110">Billable cost for the meter</span></span>
- <span data-ttu-id="71fb9-111">階層化 (該当する場合)</span><span class="sxs-lookup"><span data-stu-id="71fb9-111">Tiering (if applicable)</span></span>

<span data-ttu-id="71fb9-112">課金サイクル全体を通して毎日消費量を監視するために、有効な単価は変動します。</span><span class="sxs-lookup"><span data-stu-id="71fb9-112">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="71fb9-113">特定の請求サイクルの最終的な価格は、使用量の計算を停止し、請求期間を終了した後に使用できます。</span><span class="sxs-lookup"><span data-stu-id="71fb9-113">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="71fb9-114">小数点以下 4 桁目または 5 桁目以降の消費量のほとんどの変化が表示されます。</span><span class="sxs-lookup"><span data-stu-id="71fb9-114">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="71fb9-115">測定で階層化された価格が使用されているかどうかを確認する</span><span class="sxs-lookup"><span data-stu-id="71fb9-115">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="71fb9-116">メーターで階層化された価格が使用されるかどうかが分からない場合は、次の手順を使用して確認してください。</span><span class="sxs-lookup"><span data-stu-id="71fb9-116">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="71fb9-117">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="71fb9-117">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="71fb9-118">[販売 **] を** 選択し **、[価格とプラン] を** 選択してから、[Azure プランの **価格] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="71fb9-118">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="71fb9-119">ID で測定を見つけ、価格データをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="71fb9-119">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="71fb9-120">サンプル計算</span><span class="sxs-lookup"><span data-stu-id="71fb9-120">Sample calculation</span></span>

<span data-ttu-id="71fb9-121">次の表は、オープン期間中の有効な単価を計算する方法の例を示しています。</span><span class="sxs-lookup"><span data-stu-id="71fb9-121">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="71fb9-122">表では、次の値が適用されます。</span><span class="sxs-lookup"><span data-stu-id="71fb9-122">In the table, the following values apply:</span></span> 

- <span data-ttu-id="71fb9-123">**UP** = リソースの単価/時間 = 0.868</span><span class="sxs-lookup"><span data-stu-id="71fb9-123">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="71fb9-124">**Bcu** = 測定用の課金対象の消費単位</span><span class="sxs-lookup"><span data-stu-id="71fb9-124">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="71fb9-125">**BC** = メーターの課金対象コスト = BCU \* アップ \* 0.85。</span><span class="sxs-lookup"><span data-stu-id="71fb9-125">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="71fb9-126">これは、15% の PEC 割引の調整を反映しています。</span><span class="sxs-lookup"><span data-stu-id="71fb9-126">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="71fb9-127">次に、関数の下限を使用して、最小金額を請求するために、小数点の後の2桁に値を制限します。</span><span class="sxs-lookup"><span data-stu-id="71fb9-127">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="71fb9-128">**有効な単価** = bcu/BC</span><span class="sxs-lookup"><span data-stu-id="71fb9-128">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="71fb9-129">注: この例のメーターには、価格またはその他の割引のレベルはありません。割引率とその他の調整における有効な単価の係数です。</span><span class="sxs-lookup"><span data-stu-id="71fb9-129">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="71fb9-130">Date</span><span class="sxs-lookup"><span data-stu-id="71fb9-130">Date</span></span> | <span data-ttu-id="71fb9-131">BCU (課金対象の使用量単位)</span><span class="sxs-lookup"><span data-stu-id="71fb9-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="71fb9-132">BC (請求可能なコスト)</span><span class="sxs-lookup"><span data-stu-id="71fb9-132">BC (Billable cost)</span></span> | <span data-ttu-id="71fb9-133">有効な単価</span><span class="sxs-lookup"><span data-stu-id="71fb9-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="71fb9-134">3-8 月</span><span class="sxs-lookup"><span data-stu-id="71fb9-134">3-Aug</span></span> | <span data-ttu-id="71fb9-135">29</span><span class="sxs-lookup"><span data-stu-id="71fb9-135">29</span></span> | <span data-ttu-id="71fb9-136">21.39</span><span class="sxs-lookup"><span data-stu-id="71fb9-136">21.39</span></span> | <span data-ttu-id="71fb9-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="71fb9-137">0.737586206896552</span></span> |
| <span data-ttu-id="71fb9-138">10 ~ 8 月</span><span class="sxs-lookup"><span data-stu-id="71fb9-138">10-Aug</span></span> | <span data-ttu-id="71fb9-139">210.950039</span><span class="sxs-lookup"><span data-stu-id="71fb9-139">210.950039</span></span> | <span data-ttu-id="71fb9-140">155.63</span><span class="sxs-lookup"><span data-stu-id="71fb9-140">155.63</span></span> | <span data-ttu-id="71fb9-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="71fb9-141">0.737757626107858</span></span> |
| <span data-ttu-id="71fb9-142">25 ~ 8 月</span><span class="sxs-lookup"><span data-stu-id="71fb9-142">25-Aug</span></span> | <span data-ttu-id="71fb9-143">555.950039</span><span class="sxs-lookup"><span data-stu-id="71fb9-143">555.950039</span></span> | <span data-ttu-id="71fb9-144">410.17</span><span class="sxs-lookup"><span data-stu-id="71fb9-144">410.17</span></span> | <span data-ttu-id="71fb9-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="71fb9-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="71fb9-146">次のステップ</span><span class="sxs-lookup"><span data-stu-id="71fb9-146">Next steps</span></span>

- [<span data-ttu-id="71fb9-147">請求と税金</span><span class="sxs-lookup"><span data-stu-id="71fb9-147">Billing and taxes</span></span>](billing.md)
