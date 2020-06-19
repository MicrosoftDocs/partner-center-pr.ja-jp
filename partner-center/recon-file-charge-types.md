---
title: 調整ファイルの料金の種類
ms.topic: article
ms.date: 06/05/2020
description: パートナーセンターの調整ファイルの料金の種類 (ライセンスベース、使用量ベース、1回限り)、クレジット、割引をご確認ください。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1ec4f4a483ecfd106f7ec41b85372e136524a046
ms.sourcegitcommit: 1796d3d0ec2e06a3792852377ff81127b4d22fe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2020
ms.locfileid: "84909110"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="75231-103">パートナーセンターの調整ファイルのさまざまな料金の種類を理解する</span><span class="sxs-lookup"><span data-stu-id="75231-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="75231-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="75231-104">**Applies to**</span></span>

- <span data-ttu-id="75231-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="75231-105">Partner Center</span></span>
- <span data-ttu-id="75231-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="75231-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="75231-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="75231-107">**Appropriate roles**</span></span>

- <span data-ttu-id="75231-108">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="75231-108">Admin agent</span></span>
- <span data-ttu-id="75231-109">課金管理者</span><span class="sxs-lookup"><span data-stu-id="75231-109">Billing admin</span></span>
- <span data-ttu-id="75231-110">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="75231-110">Global admin</span></span>

<span data-ttu-id="75231-111">このトピックでは、請求書セクションと、調整ファイルに存在する可能性のある関連する料金の種類とのマッピングについて説明します。</span><span class="sxs-lookup"><span data-stu-id="75231-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="75231-112">請求書には、料金の概要が表示されます。</span><span class="sxs-lookup"><span data-stu-id="75231-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="75231-113">調整ファイルには、料金の種類など、行アイテムトランザクションの詳細な内訳が表示されます。</span><span class="sxs-lookup"><span data-stu-id="75231-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="75231-114">調整ファイルの詳細については、「[調整ファイルの使用方法](use-the-reconciliation-files.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75231-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="75231-115">[使用量に基づく調整ファイル](usage-based-recon-files.md)と[ライセンスベースの調整ファイル](license-based-recon-files.md)はどちらも、使用状況に関連するトランザクションと料金 (使用されたユニットと関連する料金) のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="75231-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="75231-116">請求書に**調整**として表示される1回限りのクレジット、割引、返金は、調整ファイルには表示されません。</span><span class="sxs-lookup"><span data-stu-id="75231-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="75231-117">請求書の料金に種類をマップする</span><span class="sxs-lookup"><span data-stu-id="75231-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="75231-118">請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルターオプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="75231-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="75231-119">調整ファイルの料金の種類でフィルター処理して、請求書の料金を調整ファイルの一連の課金の内訳にマップします。</span><span class="sxs-lookup"><span data-stu-id="75231-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="75231-120">ライセンスベースの料金</span><span class="sxs-lookup"><span data-stu-id="75231-120">License-based charges</span></span>

<span data-ttu-id="75231-121">これらのライセンスベースの料金を請求書にマッピングするには、ライセンスベースのファイルから**Amount**列を合計します。</span><span class="sxs-lookup"><span data-stu-id="75231-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="75231-122">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="75231-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="75231-123">料金の説明</span><span class="sxs-lookup"><span data-stu-id="75231-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="75231-124">アクティブ化料金</span><span class="sxs-lookup"><span data-stu-id="75231-124">Activation fee</span></span> | <span data-ttu-id="75231-125">購入後にサブスクリプションを使用する場合に、顧客に請求される金額。</span><span class="sxs-lookup"><span data-stu-id="75231-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="75231-126">取り消し料金</span><span class="sxs-lookup"><span data-stu-id="75231-126">Cancel fee</span></span> | <span data-ttu-id="75231-127">日割りは、関連付けられたシートが変更された場合に、お客様に返金されます。</span><span class="sxs-lookup"><span data-stu-id="75231-127">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="75231-128">Cancel instance prorate</span><span class="sxs-lookup"><span data-stu-id="75231-128">Cancel instance prorate</span></span> | <span data-ttu-id="75231-129">月単位のサブスクリプションを使用しているお客様がサブスクリプションを中断し、関連するシートが同じ月に変更された場合、日割り請求料金がキャンセルされます。</span><span class="sxs-lookup"><span data-stu-id="75231-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated seats changed within the same month.</span></span> |
| <span data-ttu-id="75231-130">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="75231-130">Cycle fee</span></span> | <span data-ttu-id="75231-131">サブスクリプションに対する定期的な料金。</span><span class="sxs-lookup"><span data-stu-id="75231-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="75231-132">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="75231-132">Cycle instance prorate</span></span> | <span data-ttu-id="75231-133">関連付けられているシートが変更された場合に、日割り料金が顧客から評価されます。</span><span class="sxs-lookup"><span data-stu-id="75231-133">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="75231-134">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="75231-134">Prorate fees when cancel</span></span> | <span data-ttu-id="75231-135">キャンセル時のサービスの未使用部分の日割り返金。</span><span class="sxs-lookup"><span data-stu-id="75231-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="75231-136">現在のオファリングからの変換時の edition 料金</span><span class="sxs-lookup"><span data-stu-id="75231-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="75231-137">現在の月単位のサブスクリプションから年間サブスクリプションに変換した後に、日割り料金が請求されます。</span><span class="sxs-lookup"><span data-stu-id="75231-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="75231-138">新しいオファリングに変換する場合の edition 料金</span><span class="sxs-lookup"><span data-stu-id="75231-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="75231-139">月単位のサブスクリプションを新しい年間サブスクリプションに変換した後に日割りで課金されます。</span><span class="sxs-lookup"><span data-stu-id="75231-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="75231-140">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="75231-140">Prorate fees when purchase</span></span> | <span data-ttu-id="75231-141">年間請求書を使用する場合のサブスクリプションの料金の種類。</span><span class="sxs-lookup"><span data-stu-id="75231-141">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="75231-142">Purchase fee</span><span class="sxs-lookup"><span data-stu-id="75231-142">Purchase fee</span></span> | <span data-ttu-id="75231-143">毎月の課金を使用する場合のサブスクリプションの料金の種類。</span><span class="sxs-lookup"><span data-stu-id="75231-143">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="75231-144">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="75231-144">Prorate fee when renew</span></span> | <span data-ttu-id="75231-145">サブスクリプションの更新時の日割り料金。</span><span class="sxs-lookup"><span data-stu-id="75231-145">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="75231-146">Renew fee</span><span class="sxs-lookup"><span data-stu-id="75231-146">Renew fee</span></span> | <span data-ttu-id="75231-147">サブスクリプションの更新時の課金</span><span class="sxs-lookup"><span data-stu-id="75231-147">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="75231-148">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="75231-148">Prorate fees when activate</span></span> | <span data-ttu-id="75231-149">請求期間が終了するまで、ライセンス認証から課金されます。</span><span class="sxs-lookup"><span data-stu-id="75231-149">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="75231-150">1回限りの料金</span><span class="sxs-lookup"><span data-stu-id="75231-150">One-time charges</span></span>

<span data-ttu-id="75231-151">この1回限りの料金を請求書にマップするには、ライセンスベースのファイルから**Amount**列を合計します。</span><span class="sxs-lookup"><span data-stu-id="75231-151">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="75231-152">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="75231-152">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="75231-153">料金の説明</span><span class="sxs-lookup"><span data-stu-id="75231-153">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="75231-154">新規</span><span class="sxs-lookup"><span data-stu-id="75231-154">New</span></span> | <span data-ttu-id="75231-155">新しい購入が作成されるときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="75231-155">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="75231-156">addQuantity</span><span class="sxs-lookup"><span data-stu-id="75231-156">addQuantity</span></span> | <span data-ttu-id="75231-157">元の購入の返金と、増加後の新しい数量の両方で使用されます。</span><span class="sxs-lookup"><span data-stu-id="75231-157">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="75231-158">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="75231-158">removeQuantity</span></span> | <span data-ttu-id="75231-159">元の購入の返金と、減少後の新しい数量の両方で使用されます。</span><span class="sxs-lookup"><span data-stu-id="75231-159">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="75231-160">キャンセル</span><span class="sxs-lookup"><span data-stu-id="75231-160">Cancel</span></span> | <span data-ttu-id="75231-161">サブスクリプションが取り消されたときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="75231-161">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="75231-162">Convert</span><span class="sxs-lookup"><span data-stu-id="75231-162">Convert</span></span> | <span data-ttu-id="75231-163">ライセンスをアップグレードするときに使用しますが、接続クライアント数は変更されません。</span><span class="sxs-lookup"><span data-stu-id="75231-163">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="75231-164">利用料金</span><span class="sxs-lookup"><span data-stu-id="75231-164">Usage charges</span></span>

<span data-ttu-id="75231-165">これらの使用料金を請求書にマッピングするには、使用量に基づくファイルから、[の**Ax料金**] 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="75231-165">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="75231-166">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="75231-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="75231-167">料金の説明</span><span class="sxs-lookup"><span data-stu-id="75231-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="75231-168">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="75231-168">Assess usage fee when cancel</span></span> | <span data-ttu-id="75231-169">現在の請求期間中に未払いの使用を取り消したときのアクセス利用料。</span><span class="sxs-lookup"><span data-stu-id="75231-169">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="75231-170">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="75231-170">Assess usage fee for current cycle</span></span> | <span data-ttu-id="75231-171">現在の請求期間のアクセス利用料。</span><span class="sxs-lookup"><span data-stu-id="75231-171">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="75231-172">謝辞</span><span class="sxs-lookup"><span data-stu-id="75231-172">Credits</span></span>

<span data-ttu-id="75231-173">これらのクレジットを請求書にマップするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="75231-173">To map these credits to your invoice:</span></span>

- <span data-ttu-id="75231-174">ライセンスベースのファイルから**Totalforcustomer**を合計します。</span><span class="sxs-lookup"><span data-stu-id="75231-174">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="75231-175">使用状況に基づくファイルから**PostTaxTotal**列を合計します。</span><span class="sxs-lookup"><span data-stu-id="75231-175">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="75231-176">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="75231-176">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="75231-177">料金の説明</span><span class="sxs-lookup"><span data-stu-id="75231-177">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="75231-178">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="75231-178">Offset a line item</span></span> | <span data-ttu-id="75231-179">税を含む、行項目の一部または全部の払い戻し。</span><span class="sxs-lookup"><span data-stu-id="75231-179">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="75231-180">使用量ベースの割引</span><span class="sxs-lookup"><span data-stu-id="75231-180">Usage-based discounts</span></span>

<span data-ttu-id="75231-181">これらの使用量に基づく割引を請求書にマップするには、使用量に基づくファイルから、[の**Ax料金**] 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="75231-181">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="75231-182">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="75231-182">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="75231-183">料金の説明</span><span class="sxs-lookup"><span data-stu-id="75231-183">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="75231-184">Activation discount</span><span class="sxs-lookup"><span data-stu-id="75231-184">Activation discount</span></span> | <span data-ttu-id="75231-185">サブスクリプションがアクティブになったときに適用される割引。</span><span class="sxs-lookup"><span data-stu-id="75231-185">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="75231-186">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="75231-186">Cycle discount</span></span> | <span data-ttu-id="75231-187">定期的な課金に適用される割引。</span><span class="sxs-lookup"><span data-stu-id="75231-187">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="75231-188">Renew discount</span><span class="sxs-lookup"><span data-stu-id="75231-188">Renew discount</span></span> | <span data-ttu-id="75231-189">サブスクリプションが更新されたときに適用される割引。</span><span class="sxs-lookup"><span data-stu-id="75231-189">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="75231-190">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="75231-190">Cancel discount</span></span> | <span data-ttu-id="75231-191">割引が取り消されたときに適用される料金。</span><span class="sxs-lookup"><span data-stu-id="75231-191">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="75231-192">ライセンスベースの割引</span><span class="sxs-lookup"><span data-stu-id="75231-192">License-based discounts</span></span>

<span data-ttu-id="75231-193">ライセンスベースの割引を請求書にマップするには、ライセンスベースのファイルの合計**割引**列を合計します。</span><span class="sxs-lookup"><span data-stu-id="75231-193">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="75231-194">*ライセンスベースの割引は、複数の種類の料金に適用できます。*</span><span class="sxs-lookup"><span data-stu-id="75231-194">*License-based discounts may be applied to multiple charge types.*</span></span>
