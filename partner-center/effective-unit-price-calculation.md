---
title: 有効な単価計算
ms.topic: how-to
ms.date: 04/02/2021
description: 有効な単価とその計算方法について説明します。 この記事には、サンプル計算も含まれています。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172219"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="7fe3a-104">Azure プランの使用の有効な単価計算</span><span class="sxs-lookup"><span data-stu-id="7fe3a-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="7fe3a-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="7fe3a-105">**Appropriate roles**</span></span>

- <span data-ttu-id="7fe3a-106">課金管理者</span><span class="sxs-lookup"><span data-stu-id="7fe3a-106">Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="7fe3a-107">有効な単価</span><span class="sxs-lookup"><span data-stu-id="7fe3a-107">The effective unit price</span></span>

<span data-ttu-id="7fe3a-108">有効な単価は、(リソースレベルではなく) メーターレベルで計算され、メーターの使用状況に応じて毎日調整されます。</span><span class="sxs-lookup"><span data-stu-id="7fe3a-108">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="7fe3a-109">次の3つの要素を使用して、有効な単価を計算します。</span><span class="sxs-lookup"><span data-stu-id="7fe3a-109">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="7fe3a-110">使用量 (請求サイクル全体で毎日監視されます)</span><span class="sxs-lookup"><span data-stu-id="7fe3a-110">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="7fe3a-111">メーターの課金対象コスト</span><span class="sxs-lookup"><span data-stu-id="7fe3a-111">Billable cost for the meter</span></span>
- <span data-ttu-id="7fe3a-112">階層化 (該当する場合)</span><span class="sxs-lookup"><span data-stu-id="7fe3a-112">Tiering (if applicable)</span></span>

<span data-ttu-id="7fe3a-113">請求サイクル全体にわたって使用量を毎日監視するため、有効な単価が変動します。</span><span class="sxs-lookup"><span data-stu-id="7fe3a-113">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="7fe3a-114">特定の請求サイクルの最終的な価格は、使用量の計算を停止し、請求期間を終了した後に利用可能になります。</span><span class="sxs-lookup"><span data-stu-id="7fe3a-114">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="7fe3a-115">ほとんどの変更は、4番目または5番目の小数点以下に表示されます。</span><span class="sxs-lookup"><span data-stu-id="7fe3a-115">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="7fe3a-116">メーターが階層化された価格を使用するかどうかを確認する</span><span class="sxs-lookup"><span data-stu-id="7fe3a-116">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="7fe3a-117">メーターが階層化された価格を使用しているかどうかわからない場合は、以下の手順を使用して確認してください。</span><span class="sxs-lookup"><span data-stu-id="7fe3a-117">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="7fe3a-118">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="7fe3a-118">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="7fe3a-119">[ **販売**] を選択し、[ **価格とオファー**] を選択して、[ **Azure プランの価格**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7fe3a-119">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="7fe3a-120">ID でメーターを見つけ、価格データをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="7fe3a-120">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="7fe3a-121">サンプル計算</span><span class="sxs-lookup"><span data-stu-id="7fe3a-121">Sample calculation</span></span>

<span data-ttu-id="7fe3a-122">次の表は、オープン期間中の有効な単価を計算する方法の例を示しています。</span><span class="sxs-lookup"><span data-stu-id="7fe3a-122">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="7fe3a-123">この表では、次の値が適用されます。</span><span class="sxs-lookup"><span data-stu-id="7fe3a-123">In the table, the following values apply:</span></span> 

- <span data-ttu-id="7fe3a-124">**UP** = リソースの単価/時間 = 0.868</span><span class="sxs-lookup"><span data-stu-id="7fe3a-124">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="7fe3a-125">**Bcu** = 測定用の課金対象の消費単位</span><span class="sxs-lookup"><span data-stu-id="7fe3a-125">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="7fe3a-126">**BC** = メーターの課金対象コスト = BCU \* アップ \* 0.85。</span><span class="sxs-lookup"><span data-stu-id="7fe3a-126">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="7fe3a-127">これは、15% の PEC 割引の調整を反映しています。</span><span class="sxs-lookup"><span data-stu-id="7fe3a-127">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="7fe3a-128">次に、関数の下限を使用して、最小金額を請求するために、小数点の後の2桁に値を制限します。</span><span class="sxs-lookup"><span data-stu-id="7fe3a-128">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="7fe3a-129">**有効な単価** = bcu/BC</span><span class="sxs-lookup"><span data-stu-id="7fe3a-129">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="7fe3a-130">注: この例のメーターには、価格またはその他の割引のレベルはありません。割引率とその他の調整における有効な単価の係数です。</span><span class="sxs-lookup"><span data-stu-id="7fe3a-130">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="7fe3a-131">Date</span><span class="sxs-lookup"><span data-stu-id="7fe3a-131">Date</span></span> | <span data-ttu-id="7fe3a-132">BCU (課金対象の使用量単位)</span><span class="sxs-lookup"><span data-stu-id="7fe3a-132">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="7fe3a-133">BC (請求可能なコスト)</span><span class="sxs-lookup"><span data-stu-id="7fe3a-133">BC (Billable cost)</span></span> | <span data-ttu-id="7fe3a-134">有効な単価</span><span class="sxs-lookup"><span data-stu-id="7fe3a-134">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="7fe3a-135">3-8 月</span><span class="sxs-lookup"><span data-stu-id="7fe3a-135">3-Aug</span></span> | <span data-ttu-id="7fe3a-136">29</span><span class="sxs-lookup"><span data-stu-id="7fe3a-136">29</span></span> | <span data-ttu-id="7fe3a-137">21.39</span><span class="sxs-lookup"><span data-stu-id="7fe3a-137">21.39</span></span> | <span data-ttu-id="7fe3a-138">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="7fe3a-138">0.737586206896552</span></span> |
| <span data-ttu-id="7fe3a-139">10 ~ 8 月</span><span class="sxs-lookup"><span data-stu-id="7fe3a-139">10-Aug</span></span> | <span data-ttu-id="7fe3a-140">210.950039</span><span class="sxs-lookup"><span data-stu-id="7fe3a-140">210.950039</span></span> | <span data-ttu-id="7fe3a-141">155.63</span><span class="sxs-lookup"><span data-stu-id="7fe3a-141">155.63</span></span> | <span data-ttu-id="7fe3a-142">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="7fe3a-142">0.737757626107858</span></span> |
| <span data-ttu-id="7fe3a-143">25 ~ 8 月</span><span class="sxs-lookup"><span data-stu-id="7fe3a-143">25-Aug</span></span> | <span data-ttu-id="7fe3a-144">555.950039</span><span class="sxs-lookup"><span data-stu-id="7fe3a-144">555.950039</span></span> | <span data-ttu-id="7fe3a-145">410.17</span><span class="sxs-lookup"><span data-stu-id="7fe3a-145">410.17</span></span> | <span data-ttu-id="7fe3a-146">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="7fe3a-146">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="7fe3a-147">次のステップ</span><span class="sxs-lookup"><span data-stu-id="7fe3a-147">Next steps</span></span>

- [<span data-ttu-id="7fe3a-148">請求と税金</span><span class="sxs-lookup"><span data-stu-id="7fe3a-148">Billing and taxes</span></span>](billing.md)
