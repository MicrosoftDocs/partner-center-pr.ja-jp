---
title: 調整ファイルの料金の種類
ms.topic: article
ms.date: 06/05/2020
description: パートナーセンターの調整ファイルの料金の種類 (ライセンスベース、使用量ベース、1回限り)、クレジット、割引をご確認ください。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f1fb7fdcc4ec56f0d5cf0eb26b62294235a5b908
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441600"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="b3308-103">パートナーセンターの調整ファイルのさまざまな料金の種類を理解する</span><span class="sxs-lookup"><span data-stu-id="b3308-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="b3308-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="b3308-104">**Applies to**</span></span>

- <span data-ttu-id="b3308-105">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="b3308-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="b3308-106">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="b3308-106">**Appropriate roles**</span></span>

- <span data-ttu-id="b3308-107">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="b3308-107">Admin agent</span></span>
- <span data-ttu-id="b3308-108">課金管理者</span><span class="sxs-lookup"><span data-stu-id="b3308-108">Billing admin</span></span>
- <span data-ttu-id="b3308-109">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="b3308-109">Global admin</span></span>

<span data-ttu-id="b3308-110">この記事では、請求書セクションと、調整ファイルに存在する可能性のある関連する料金の種類とのマッピングについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b3308-110">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="b3308-111">請求書には、料金の概要が表示されます。</span><span class="sxs-lookup"><span data-stu-id="b3308-111">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="b3308-112">調整ファイルには、料金の種類など、行アイテムトランザクションの詳細な内訳が表示されます。</span><span class="sxs-lookup"><span data-stu-id="b3308-112">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="b3308-113">調整ファイルの詳細については、「 [調整ファイルの使用方法](use-the-reconciliation-files.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3308-113">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="b3308-114">[使用量に基づく調整ファイル](usage-based-recon-files.md)と[ライセンスベースの調整ファイル](license-based-recon-files.md)はどちらも、使用状況に関連するトランザクションと料金 (使用されたユニットと関連する料金) のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="b3308-114">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="b3308-115">請求書に **調整** として表示される1回限りのクレジット、割引、返金は、調整ファイルには表示されません。</span><span class="sxs-lookup"><span data-stu-id="b3308-115">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="b3308-116">請求書の料金に種類をマップする</span><span class="sxs-lookup"><span data-stu-id="b3308-116">Map charge types to invoice charges</span></span>

<span data-ttu-id="b3308-117">請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルターオプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="b3308-117">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="b3308-118">調整ファイルの料金の種類でフィルター処理して、請求書の料金を調整ファイルの一連の課金の内訳にマップします。</span><span class="sxs-lookup"><span data-stu-id="b3308-118">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="b3308-119">ライセンスベースの料金</span><span class="sxs-lookup"><span data-stu-id="b3308-119">License-based charges</span></span>

<span data-ttu-id="b3308-120">これらのライセンスベースの料金を請求書にマッピングするには、ライセンスベースのファイルから **Amount** 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="b3308-120">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="b3308-121">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="b3308-121">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b3308-122">料金の説明</span><span class="sxs-lookup"><span data-stu-id="b3308-122">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b3308-123">アクティブ化料金</span><span class="sxs-lookup"><span data-stu-id="b3308-123">Activation fee</span></span> | <span data-ttu-id="b3308-124">購入後にサブスクリプションを使用する場合に、顧客に請求される金額。</span><span class="sxs-lookup"><span data-stu-id="b3308-124">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="b3308-125">取り消し料金</span><span class="sxs-lookup"><span data-stu-id="b3308-125">Cancel fee</span></span> | <span data-ttu-id="b3308-126">関連付けられているライセンスが変更された場合、日割り料金がお客様に返金されます。</span><span class="sxs-lookup"><span data-stu-id="b3308-126">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="b3308-127">Cancel instance prorate</span><span class="sxs-lookup"><span data-stu-id="b3308-127">Cancel instance prorate</span></span> | <span data-ttu-id="b3308-128">月単位のサブスクリプションを使用しているお客様がサブスクリプションを一時停止し、関連するライセンスが同じ月に変更された場合、日割り請求料金がキャンセルされます</span><span class="sxs-lookup"><span data-stu-id="b3308-128">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="b3308-129">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="b3308-129">Cycle fee</span></span> | <span data-ttu-id="b3308-130">サブスクリプションに対する定期的な料金。</span><span class="sxs-lookup"><span data-stu-id="b3308-130">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="b3308-131">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="b3308-131">Cycle instance prorate</span></span> | <span data-ttu-id="b3308-132">関連付けられているライセンスが変更された場合、お客様からの日割り料金が請求されます。</span><span class="sxs-lookup"><span data-stu-id="b3308-132">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="b3308-133">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="b3308-133">Prorate fees when cancel</span></span> | <span data-ttu-id="b3308-134">キャンセル時のサービスの未使用部分の日割り返金。</span><span class="sxs-lookup"><span data-stu-id="b3308-134">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="b3308-135">現在のオファリングからの変換時の edition 料金</span><span class="sxs-lookup"><span data-stu-id="b3308-135">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="b3308-136">現在の月単位のサブスクリプションから年間サブスクリプションに変換した後に、日割り料金が請求されます。</span><span class="sxs-lookup"><span data-stu-id="b3308-136">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="b3308-137">新しいオファリングに変換する場合の edition 料金</span><span class="sxs-lookup"><span data-stu-id="b3308-137">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="b3308-138">月単位のサブスクリプションを新しい年間サブスクリプションに変換した後に日割りで課金されます。</span><span class="sxs-lookup"><span data-stu-id="b3308-138">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="b3308-139">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="b3308-139">Prorate fees when purchase</span></span> | <span data-ttu-id="b3308-140">月単位または年間請求書の両方を使用する場合のサブスクリプションの料金の種類。</span><span class="sxs-lookup"><span data-stu-id="b3308-140">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="b3308-141">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="b3308-141">Prorate fee when renew</span></span> | <span data-ttu-id="b3308-142">サブスクリプションの更新時の日割り料金。</span><span class="sxs-lookup"><span data-stu-id="b3308-142">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="b3308-143">Renew fee</span><span class="sxs-lookup"><span data-stu-id="b3308-143">Renew fee</span></span> | <span data-ttu-id="b3308-144">サブスクリプションの更新時の課金</span><span class="sxs-lookup"><span data-stu-id="b3308-144">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="b3308-145">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="b3308-145">Prorate fees when activate</span></span> | <span data-ttu-id="b3308-146">請求期間が終了するまで、ライセンス認証から課金されます。</span><span class="sxs-lookup"><span data-stu-id="b3308-146">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="b3308-147">1回限りの料金</span><span class="sxs-lookup"><span data-stu-id="b3308-147">One-time charges</span></span>

<span data-ttu-id="b3308-148">この1回限りの料金を請求書にマップするには、ライセンスベースのファイルから **Amount** 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="b3308-148">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="b3308-149">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="b3308-149">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b3308-150">料金の説明</span><span class="sxs-lookup"><span data-stu-id="b3308-150">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b3308-151">新規</span><span class="sxs-lookup"><span data-stu-id="b3308-151">New</span></span> | <span data-ttu-id="b3308-152">新しい購入が作成されるときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="b3308-152">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="b3308-153">addQuantity</span><span class="sxs-lookup"><span data-stu-id="b3308-153">addQuantity</span></span> | <span data-ttu-id="b3308-154">元の購入の返金と、増加後の新しい数量の両方で使用されます。</span><span class="sxs-lookup"><span data-stu-id="b3308-154">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="b3308-155">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="b3308-155">removeQuantity</span></span> | <span data-ttu-id="b3308-156">元の購入の返金と、減少後の新しい数量の両方で使用されます。</span><span class="sxs-lookup"><span data-stu-id="b3308-156">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="b3308-157">キャンセル</span><span class="sxs-lookup"><span data-stu-id="b3308-157">Cancel</span></span> | <span data-ttu-id="b3308-158">サブスクリプションが取り消されたときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="b3308-158">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="b3308-159">Convert</span><span class="sxs-lookup"><span data-stu-id="b3308-159">Convert</span></span> | <span data-ttu-id="b3308-160">ライセンスをアップグレードするときに、ライセンス数が変更されないままにする場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="b3308-160">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="b3308-161">利用料金</span><span class="sxs-lookup"><span data-stu-id="b3308-161">Usage charges</span></span>

<span data-ttu-id="b3308-162">これらの使用料金を請求書にマッピングするには、使用量に基づくファイルから、[の **Ax料金** ] 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="b3308-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="b3308-163">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="b3308-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b3308-164">料金の説明</span><span class="sxs-lookup"><span data-stu-id="b3308-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b3308-165">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="b3308-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="b3308-166">現在の請求期間中に未払いの使用を取り消したときのアクセス利用料。</span><span class="sxs-lookup"><span data-stu-id="b3308-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="b3308-167">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="b3308-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="b3308-168">現在の請求期間のアクセス利用料。</span><span class="sxs-lookup"><span data-stu-id="b3308-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="b3308-169">謝辞</span><span class="sxs-lookup"><span data-stu-id="b3308-169">Credits</span></span>

<span data-ttu-id="b3308-170">これらのクレジットを請求書にマップするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="b3308-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="b3308-171">ライセンスベースのファイルから **Totalforcustomer** を合計します。</span><span class="sxs-lookup"><span data-stu-id="b3308-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="b3308-172">使用状況に基づくファイルから **PostTaxTotal** 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="b3308-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="b3308-173">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="b3308-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b3308-174">料金の説明</span><span class="sxs-lookup"><span data-stu-id="b3308-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b3308-175">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="b3308-175">Offset a line item</span></span> | <span data-ttu-id="b3308-176">税を含む、行項目の一部または全部の払い戻し。</span><span class="sxs-lookup"><span data-stu-id="b3308-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="b3308-177">使用量ベースの割引</span><span class="sxs-lookup"><span data-stu-id="b3308-177">Usage-based discounts</span></span>

<span data-ttu-id="b3308-178">これらの使用量に基づく割引を請求書にマップするには、使用量に基づくファイルから、[の **Ax料金** ] 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="b3308-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="b3308-179">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="b3308-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="b3308-180">料金の説明</span><span class="sxs-lookup"><span data-stu-id="b3308-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="b3308-181">Activation discount</span><span class="sxs-lookup"><span data-stu-id="b3308-181">Activation discount</span></span> | <span data-ttu-id="b3308-182">サブスクリプションがアクティブになったときに適用される割引。</span><span class="sxs-lookup"><span data-stu-id="b3308-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="b3308-183">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="b3308-183">Cycle discount</span></span> | <span data-ttu-id="b3308-184">定期的な課金に適用される割引。</span><span class="sxs-lookup"><span data-stu-id="b3308-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="b3308-185">Renew discount</span><span class="sxs-lookup"><span data-stu-id="b3308-185">Renew discount</span></span> | <span data-ttu-id="b3308-186">サブスクリプションが更新されたときに適用される割引。</span><span class="sxs-lookup"><span data-stu-id="b3308-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="b3308-187">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="b3308-187">Cancel discount</span></span> | <span data-ttu-id="b3308-188">割引が取り消されたときに適用される料金。</span><span class="sxs-lookup"><span data-stu-id="b3308-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="b3308-189">ライセンスベースの割引</span><span class="sxs-lookup"><span data-stu-id="b3308-189">License-based discounts</span></span>

<span data-ttu-id="b3308-190">ライセンスベースの割引を請求書にマップするには、ライセンスベースのファイルの合計 **割引** 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="b3308-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="b3308-191">*ライセンスベースの割引は、複数の種類の料金に適用できます。*</span><span class="sxs-lookup"><span data-stu-id="b3308-191">*License-based discounts may be applied to multiple charge types.*</span></span>
