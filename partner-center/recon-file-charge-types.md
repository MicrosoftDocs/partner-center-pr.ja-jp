---
title: 調整ファイルの料金の種類
ms.topic: article
ms.date: 06/05/2020
description: パートナーセンターの調整ファイルの料金の種類 (ライセンスベース、使用量ベース、1回限り)、クレジット、割引をご確認ください。
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c12bd8b08f3f72c42d788cb677888a7e3cde85a5
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2020
ms.locfileid: "87444776"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="bdabf-103">パートナーセンターの調整ファイルのさまざまな料金の種類を理解する</span><span class="sxs-lookup"><span data-stu-id="bdabf-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="bdabf-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="bdabf-104">**Applies to**</span></span>

- <span data-ttu-id="bdabf-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="bdabf-105">Partner Center</span></span>
- <span data-ttu-id="bdabf-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="bdabf-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="bdabf-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="bdabf-107">**Appropriate roles**</span></span>

- <span data-ttu-id="bdabf-108">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="bdabf-108">Admin agent</span></span>
- <span data-ttu-id="bdabf-109">課金管理者</span><span class="sxs-lookup"><span data-stu-id="bdabf-109">Billing admin</span></span>
- <span data-ttu-id="bdabf-110">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="bdabf-110">Global admin</span></span>

<span data-ttu-id="bdabf-111">このトピックでは、請求書セクションと、調整ファイルに存在する可能性のある関連する料金の種類とのマッピングについて説明します。</span><span class="sxs-lookup"><span data-stu-id="bdabf-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="bdabf-112">請求書には、料金の概要が表示されます。</span><span class="sxs-lookup"><span data-stu-id="bdabf-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="bdabf-113">調整ファイルには、料金の種類など、行アイテムトランザクションの詳細な内訳が表示されます。</span><span class="sxs-lookup"><span data-stu-id="bdabf-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="bdabf-114">調整ファイルの詳細については、「[調整ファイルの使用方法](use-the-reconciliation-files.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bdabf-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="bdabf-115">[使用量に基づく調整ファイル](usage-based-recon-files.md)と[ライセンスベースの調整ファイル](license-based-recon-files.md)はどちらも、使用状況に関連するトランザクションと料金 (使用されたユニットと関連する料金) のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="bdabf-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="bdabf-116">請求書に**調整**として表示される1回限りのクレジット、割引、返金は、調整ファイルには表示されません。</span><span class="sxs-lookup"><span data-stu-id="bdabf-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="bdabf-117">請求書の料金に種類をマップする</span><span class="sxs-lookup"><span data-stu-id="bdabf-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="bdabf-118">請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルターオプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="bdabf-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="bdabf-119">調整ファイルの料金の種類でフィルター処理して、請求書の料金を調整ファイルの一連の課金の内訳にマップします。</span><span class="sxs-lookup"><span data-stu-id="bdabf-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="bdabf-120">ライセンスベースの料金</span><span class="sxs-lookup"><span data-stu-id="bdabf-120">License-based charges</span></span>

<span data-ttu-id="bdabf-121">これらのライセンスベースの料金を請求書にマッピングするには、ライセンスベースのファイルから**Amount**列を合計します。</span><span class="sxs-lookup"><span data-stu-id="bdabf-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="bdabf-122">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="bdabf-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="bdabf-123">料金の説明</span><span class="sxs-lookup"><span data-stu-id="bdabf-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="bdabf-124">アクティブ化料金</span><span class="sxs-lookup"><span data-stu-id="bdabf-124">Activation fee</span></span> | <span data-ttu-id="bdabf-125">購入後にサブスクリプションを使用する場合に、顧客に請求される金額。</span><span class="sxs-lookup"><span data-stu-id="bdabf-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="bdabf-126">取り消し料金</span><span class="sxs-lookup"><span data-stu-id="bdabf-126">Cancel fee</span></span> | <span data-ttu-id="bdabf-127">関連付けられているライセンスが変更された場合、日割り料金がお客様に返金されます。</span><span class="sxs-lookup"><span data-stu-id="bdabf-127">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="bdabf-128">Cancel instance prorate</span><span class="sxs-lookup"><span data-stu-id="bdabf-128">Cancel instance prorate</span></span> | <span data-ttu-id="bdabf-129">月単位のサブスクリプションを使用しているお客様がサブスクリプションを一時停止し、関連するライセンスが同じ月に変更された場合、日割り請求料金がキャンセルされます</span><span class="sxs-lookup"><span data-stu-id="bdabf-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="bdabf-130">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="bdabf-130">Cycle fee</span></span> | <span data-ttu-id="bdabf-131">サブスクリプションに対する定期的な料金。</span><span class="sxs-lookup"><span data-stu-id="bdabf-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="bdabf-132">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="bdabf-132">Cycle instance prorate</span></span> | <span data-ttu-id="bdabf-133">関連付けられているライセンスが変更された場合、お客様からの日割り料金が請求されます。</span><span class="sxs-lookup"><span data-stu-id="bdabf-133">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="bdabf-134">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="bdabf-134">Prorate fees when cancel</span></span> | <span data-ttu-id="bdabf-135">キャンセル時のサービスの未使用部分の日割り返金。</span><span class="sxs-lookup"><span data-stu-id="bdabf-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="bdabf-136">現在のオファリングからの変換時の edition 料金</span><span class="sxs-lookup"><span data-stu-id="bdabf-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="bdabf-137">現在の月単位のサブスクリプションから年間サブスクリプションに変換した後に、日割り料金が請求されます。</span><span class="sxs-lookup"><span data-stu-id="bdabf-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="bdabf-138">新しいオファリングに変換する場合の edition 料金</span><span class="sxs-lookup"><span data-stu-id="bdabf-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="bdabf-139">月単位のサブスクリプションを新しい年間サブスクリプションに変換した後に日割りで課金されます。</span><span class="sxs-lookup"><span data-stu-id="bdabf-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="bdabf-140">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="bdabf-140">Prorate fees when purchase</span></span> | <span data-ttu-id="bdabf-141">年間請求書を使用する場合のサブスクリプションの料金の種類。</span><span class="sxs-lookup"><span data-stu-id="bdabf-141">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="bdabf-142">Purchase fee</span><span class="sxs-lookup"><span data-stu-id="bdabf-142">Purchase fee</span></span> | <span data-ttu-id="bdabf-143">毎月の課金を使用する場合のサブスクリプションの料金の種類。</span><span class="sxs-lookup"><span data-stu-id="bdabf-143">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="bdabf-144">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="bdabf-144">Prorate fee when renew</span></span> | <span data-ttu-id="bdabf-145">サブスクリプションの更新時の日割り料金。</span><span class="sxs-lookup"><span data-stu-id="bdabf-145">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="bdabf-146">Renew fee</span><span class="sxs-lookup"><span data-stu-id="bdabf-146">Renew fee</span></span> | <span data-ttu-id="bdabf-147">サブスクリプションの更新時の課金</span><span class="sxs-lookup"><span data-stu-id="bdabf-147">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="bdabf-148">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="bdabf-148">Prorate fees when activate</span></span> | <span data-ttu-id="bdabf-149">請求期間が終了するまで、ライセンス認証から課金されます。</span><span class="sxs-lookup"><span data-stu-id="bdabf-149">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="bdabf-150">1回限りの料金</span><span class="sxs-lookup"><span data-stu-id="bdabf-150">One-time charges</span></span>

<span data-ttu-id="bdabf-151">この1回限りの料金を請求書にマップするには、ライセンスベースのファイルから**Amount**列を合計します。</span><span class="sxs-lookup"><span data-stu-id="bdabf-151">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="bdabf-152">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="bdabf-152">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="bdabf-153">料金の説明</span><span class="sxs-lookup"><span data-stu-id="bdabf-153">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="bdabf-154">新規作成</span><span class="sxs-lookup"><span data-stu-id="bdabf-154">New</span></span> | <span data-ttu-id="bdabf-155">新しい購入が作成されるときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="bdabf-155">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="bdabf-156">addQuantity</span><span class="sxs-lookup"><span data-stu-id="bdabf-156">addQuantity</span></span> | <span data-ttu-id="bdabf-157">元の購入の返金と、増加後の新しい数量の両方で使用されます。</span><span class="sxs-lookup"><span data-stu-id="bdabf-157">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="bdabf-158">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="bdabf-158">removeQuantity</span></span> | <span data-ttu-id="bdabf-159">元の購入の返金と、減少後の新しい数量の両方で使用されます。</span><span class="sxs-lookup"><span data-stu-id="bdabf-159">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="bdabf-160">キャンセル</span><span class="sxs-lookup"><span data-stu-id="bdabf-160">Cancel</span></span> | <span data-ttu-id="bdabf-161">サブスクリプションが取り消されたときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="bdabf-161">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="bdabf-162">Convert</span><span class="sxs-lookup"><span data-stu-id="bdabf-162">Convert</span></span> | <span data-ttu-id="bdabf-163">ライセンスをアップグレードするときに、ライセンス数が変更されないままにする場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="bdabf-163">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="bdabf-164">利用料金</span><span class="sxs-lookup"><span data-stu-id="bdabf-164">Usage charges</span></span>

<span data-ttu-id="bdabf-165">これらの使用料金を請求書にマッピングするには、使用量に基づくファイルから、[の**Ax料金**] 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="bdabf-165">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="bdabf-166">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="bdabf-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="bdabf-167">料金の説明</span><span class="sxs-lookup"><span data-stu-id="bdabf-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="bdabf-168">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="bdabf-168">Assess usage fee when cancel</span></span> | <span data-ttu-id="bdabf-169">現在の請求期間中に未払いの使用を取り消したときのアクセス利用料。</span><span class="sxs-lookup"><span data-stu-id="bdabf-169">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="bdabf-170">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="bdabf-170">Assess usage fee for current cycle</span></span> | <span data-ttu-id="bdabf-171">現在の請求期間のアクセス利用料。</span><span class="sxs-lookup"><span data-stu-id="bdabf-171">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="bdabf-172">謝辞</span><span class="sxs-lookup"><span data-stu-id="bdabf-172">Credits</span></span>

<span data-ttu-id="bdabf-173">これらのクレジットを請求書にマップするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="bdabf-173">To map these credits to your invoice:</span></span>

- <span data-ttu-id="bdabf-174">ライセンスベースのファイルから**Totalforcustomer**を合計します。</span><span class="sxs-lookup"><span data-stu-id="bdabf-174">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="bdabf-175">使用状況に基づくファイルから**PostTaxTotal**列を合計します。</span><span class="sxs-lookup"><span data-stu-id="bdabf-175">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="bdabf-176">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="bdabf-176">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="bdabf-177">料金の説明</span><span class="sxs-lookup"><span data-stu-id="bdabf-177">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="bdabf-178">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="bdabf-178">Offset a line item</span></span> | <span data-ttu-id="bdabf-179">税を含む、行項目の一部または全部の払い戻し。</span><span class="sxs-lookup"><span data-stu-id="bdabf-179">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="bdabf-180">使用量ベースの割引</span><span class="sxs-lookup"><span data-stu-id="bdabf-180">Usage-based discounts</span></span>

<span data-ttu-id="bdabf-181">これらの使用量に基づく割引を請求書にマップするには、使用量に基づくファイルから、[の**Ax料金**] 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="bdabf-181">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="bdabf-182">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="bdabf-182">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="bdabf-183">料金の説明</span><span class="sxs-lookup"><span data-stu-id="bdabf-183">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="bdabf-184">Activation discount</span><span class="sxs-lookup"><span data-stu-id="bdabf-184">Activation discount</span></span> | <span data-ttu-id="bdabf-185">サブスクリプションがアクティブになったときに適用される割引。</span><span class="sxs-lookup"><span data-stu-id="bdabf-185">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="bdabf-186">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="bdabf-186">Cycle discount</span></span> | <span data-ttu-id="bdabf-187">定期的な課金に適用される割引。</span><span class="sxs-lookup"><span data-stu-id="bdabf-187">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="bdabf-188">Renew discount</span><span class="sxs-lookup"><span data-stu-id="bdabf-188">Renew discount</span></span> | <span data-ttu-id="bdabf-189">サブスクリプションが更新されたときに適用される割引。</span><span class="sxs-lookup"><span data-stu-id="bdabf-189">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="bdabf-190">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="bdabf-190">Cancel discount</span></span> | <span data-ttu-id="bdabf-191">割引が取り消されたときに適用される料金。</span><span class="sxs-lookup"><span data-stu-id="bdabf-191">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="bdabf-192">ライセンスベースの割引</span><span class="sxs-lookup"><span data-stu-id="bdabf-192">License-based discounts</span></span>

<span data-ttu-id="bdabf-193">ライセンスベースの割引を請求書にマップするには、ライセンスベースのファイルの合計**割引**列を合計します。</span><span class="sxs-lookup"><span data-stu-id="bdabf-193">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="bdabf-194">*ライセンスベースの割引は、複数の種類の料金に適用できます。*</span><span class="sxs-lookup"><span data-stu-id="bdabf-194">*License-based discounts may be applied to multiple charge types.*</span></span>
