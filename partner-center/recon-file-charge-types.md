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
ms.openlocfilehash: 5a1f45de59fc9dac6a443bb8a14c3a80b36ba3f7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855881"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="f395e-103">パートナーセンターの調整ファイルのさまざまな料金の種類を理解する</span><span class="sxs-lookup"><span data-stu-id="f395e-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="f395e-104">**適用対象**: パートナーセンター |米国政府向け Microsoft Cloud パートナーセンター</span><span class="sxs-lookup"><span data-stu-id="f395e-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="f395e-105">**適切なロール**: 管理エージェント |課金管理者 |全体管理者</span><span class="sxs-lookup"><span data-stu-id="f395e-105">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="f395e-106">この記事では、請求書セクションと、調整ファイルに存在する可能性のある関連する料金の種類とのマッピングについて説明します。</span><span class="sxs-lookup"><span data-stu-id="f395e-106">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="f395e-107">請求書には、料金の概要が表示されます。</span><span class="sxs-lookup"><span data-stu-id="f395e-107">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="f395e-108">調整ファイルには、料金の種類など、行アイテムトランザクションの詳細な内訳が表示されます。</span><span class="sxs-lookup"><span data-stu-id="f395e-108">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="f395e-109">調整ファイルの詳細については、「 [調整ファイルの使用方法](use-the-reconciliation-files.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f395e-109">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="f395e-110">[使用量に基づく調整ファイル](usage-based-recon-files.md)と[ライセンスベースの調整ファイル](license-based-recon-files.md)はどちらも、使用状況に関連するトランザクションと料金 (使用されたユニットと関連する料金) のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="f395e-110">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="f395e-111">請求書に **調整** として表示される1回限りのクレジット、割引、返金は、調整ファイルには表示されません。</span><span class="sxs-lookup"><span data-stu-id="f395e-111">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="f395e-112">請求書の料金に種類をマップする</span><span class="sxs-lookup"><span data-stu-id="f395e-112">Map charge types to invoice charges</span></span>

<span data-ttu-id="f395e-113">請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルターオプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="f395e-113">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="f395e-114">調整ファイルの料金の種類でフィルター処理して、請求書の料金を調整ファイルの一連の課金の内訳にマップします。</span><span class="sxs-lookup"><span data-stu-id="f395e-114">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="f395e-115">ライセンスベースの料金</span><span class="sxs-lookup"><span data-stu-id="f395e-115">License-based charges</span></span>

<span data-ttu-id="f395e-116">これらのライセンスベースの料金を請求書にマッピングするには、ライセンスベースのファイルから **Amount** 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="f395e-116">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="f395e-117">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="f395e-117">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="f395e-118">料金の説明</span><span class="sxs-lookup"><span data-stu-id="f395e-118">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="f395e-119">アクティブ化料金</span><span class="sxs-lookup"><span data-stu-id="f395e-119">Activation fee</span></span> | <span data-ttu-id="f395e-120">購入後にサブスクリプションを使用する場合に、顧客に請求される金額。</span><span class="sxs-lookup"><span data-stu-id="f395e-120">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="f395e-121">取り消し料金</span><span class="sxs-lookup"><span data-stu-id="f395e-121">Cancel fee</span></span> | <span data-ttu-id="f395e-122">関連付けられているライセンスが変更された場合、日割り料金がお客様に返金されます。</span><span class="sxs-lookup"><span data-stu-id="f395e-122">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="f395e-123">Cancel instance prorate</span><span class="sxs-lookup"><span data-stu-id="f395e-123">Cancel instance prorate</span></span> | <span data-ttu-id="f395e-124">月単位のサブスクリプションを使用しているお客様がサブスクリプションを一時停止し、関連するライセンスが同じ月に変更された場合、日割り請求料金がキャンセルされます</span><span class="sxs-lookup"><span data-stu-id="f395e-124">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="f395e-125">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="f395e-125">Cycle fee</span></span> | <span data-ttu-id="f395e-126">サブスクリプションに対する定期的な料金。</span><span class="sxs-lookup"><span data-stu-id="f395e-126">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="f395e-127">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="f395e-127">Cycle instance prorate</span></span> | <span data-ttu-id="f395e-128">関連付けられているライセンスが変更された場合、お客様からの日割り料金が請求されます。</span><span class="sxs-lookup"><span data-stu-id="f395e-128">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="f395e-129">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="f395e-129">Prorate fees when cancel</span></span> | <span data-ttu-id="f395e-130">キャンセル時のサービスの未使用部分の日割り返金。</span><span class="sxs-lookup"><span data-stu-id="f395e-130">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="f395e-131">現在のオファリングからの変換時の edition 料金</span><span class="sxs-lookup"><span data-stu-id="f395e-131">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="f395e-132">現在の月単位のサブスクリプションから年間サブスクリプションに変換した後に、日割り料金が請求されます。</span><span class="sxs-lookup"><span data-stu-id="f395e-132">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="f395e-133">新しいオファリングに変換する場合の edition 料金</span><span class="sxs-lookup"><span data-stu-id="f395e-133">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="f395e-134">月単位のサブスクリプションを新しい年間サブスクリプションに変換した後に日割りで課金されます。</span><span class="sxs-lookup"><span data-stu-id="f395e-134">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="f395e-135">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="f395e-135">Prorate fees when purchase</span></span> | <span data-ttu-id="f395e-136">月単位または年間請求書の両方を使用する場合のサブスクリプションの料金の種類。</span><span class="sxs-lookup"><span data-stu-id="f395e-136">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="f395e-137">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="f395e-137">Prorate fee when renew</span></span> | <span data-ttu-id="f395e-138">サブスクリプションの更新時の日割り料金。</span><span class="sxs-lookup"><span data-stu-id="f395e-138">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="f395e-139">Renew fee</span><span class="sxs-lookup"><span data-stu-id="f395e-139">Renew fee</span></span> | <span data-ttu-id="f395e-140">サブスクリプションの更新時の課金</span><span class="sxs-lookup"><span data-stu-id="f395e-140">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="f395e-141">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="f395e-141">Prorate fees when activate</span></span> | <span data-ttu-id="f395e-142">請求期間が終了するまで、ライセンス認証から課金されます。</span><span class="sxs-lookup"><span data-stu-id="f395e-142">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="f395e-143">1回限りの料金</span><span class="sxs-lookup"><span data-stu-id="f395e-143">One-time charges</span></span>

<span data-ttu-id="f395e-144">この1回限りの料金を請求書にマップするには、ライセンスベースのファイルから **Amount** 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="f395e-144">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="f395e-145">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="f395e-145">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="f395e-146">料金の説明</span><span class="sxs-lookup"><span data-stu-id="f395e-146">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="f395e-147">新規</span><span class="sxs-lookup"><span data-stu-id="f395e-147">New</span></span> | <span data-ttu-id="f395e-148">新しい購入が作成されるときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="f395e-148">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="f395e-149">addQuantity</span><span class="sxs-lookup"><span data-stu-id="f395e-149">addQuantity</span></span> | <span data-ttu-id="f395e-150">元の購入の返金と、増加後の新しい数量の両方で使用されます。</span><span class="sxs-lookup"><span data-stu-id="f395e-150">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="f395e-151">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="f395e-151">removeQuantity</span></span> | <span data-ttu-id="f395e-152">元の購入の返金と、減少後の新しい数量の両方で使用されます。</span><span class="sxs-lookup"><span data-stu-id="f395e-152">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="f395e-153">キャンセル</span><span class="sxs-lookup"><span data-stu-id="f395e-153">Cancel</span></span> | <span data-ttu-id="f395e-154">サブスクリプションが取り消されたときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="f395e-154">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="f395e-155">Convert</span><span class="sxs-lookup"><span data-stu-id="f395e-155">Convert</span></span> | <span data-ttu-id="f395e-156">ライセンスをアップグレードするときに、ライセンス数が変更されないままにする場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="f395e-156">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="f395e-157">利用料金</span><span class="sxs-lookup"><span data-stu-id="f395e-157">Usage charges</span></span>

<span data-ttu-id="f395e-158">これらの使用料金を請求書にマッピングするには、使用量に基づくファイルから、[の **Ax料金** ] 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="f395e-158">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="f395e-159">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="f395e-159">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="f395e-160">料金の説明</span><span class="sxs-lookup"><span data-stu-id="f395e-160">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="f395e-161">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="f395e-161">Assess usage fee when cancel</span></span> | <span data-ttu-id="f395e-162">現在の請求期間中に未払いの使用を取り消したときのアクセス利用料。</span><span class="sxs-lookup"><span data-stu-id="f395e-162">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="f395e-163">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="f395e-163">Assess usage fee for current cycle</span></span> | <span data-ttu-id="f395e-164">現在の請求期間のアクセス利用料。</span><span class="sxs-lookup"><span data-stu-id="f395e-164">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="f395e-165">謝辞</span><span class="sxs-lookup"><span data-stu-id="f395e-165">Credits</span></span>

<span data-ttu-id="f395e-166">これらのクレジットを請求書にマップするには:</span><span class="sxs-lookup"><span data-stu-id="f395e-166">To map these credits to your invoice:</span></span>

- <span data-ttu-id="f395e-167">ライセンス ベース **のファイルの TotalForCustomer** を合計します。</span><span class="sxs-lookup"><span data-stu-id="f395e-167">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="f395e-168">使用状況ベース **のファイルから PostTaxTotal** 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="f395e-168">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="f395e-169">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="f395e-169">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="f395e-170">料金の説明</span><span class="sxs-lookup"><span data-stu-id="f395e-170">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="f395e-171">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="f395e-171">Offset a line item</span></span> | <span data-ttu-id="f395e-172">税を含む、行項目の一部または全部の払い戻し。</span><span class="sxs-lookup"><span data-stu-id="f395e-172">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="f395e-173">使用量ベースの割引</span><span class="sxs-lookup"><span data-stu-id="f395e-173">Usage-based discounts</span></span>

<span data-ttu-id="f395e-174">これらの使用量ベースの割引を請求書にマップするには、使用状況ベースのファイルから **PretaxCharges** 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="f395e-174">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="f395e-175">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="f395e-175">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="f395e-176">料金の説明</span><span class="sxs-lookup"><span data-stu-id="f395e-176">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="f395e-177">Activation discount</span><span class="sxs-lookup"><span data-stu-id="f395e-177">Activation discount</span></span> | <span data-ttu-id="f395e-178">サブスクリプションのアクティブ化時に適用される割引。</span><span class="sxs-lookup"><span data-stu-id="f395e-178">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="f395e-179">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="f395e-179">Cycle discount</span></span> | <span data-ttu-id="f395e-180">定期的な課金に適用される割引。</span><span class="sxs-lookup"><span data-stu-id="f395e-180">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="f395e-181">Renew discount</span><span class="sxs-lookup"><span data-stu-id="f395e-181">Renew discount</span></span> | <span data-ttu-id="f395e-182">サブスクリプションの更新時に適用される割引。</span><span class="sxs-lookup"><span data-stu-id="f395e-182">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="f395e-183">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="f395e-183">Cancel discount</span></span> | <span data-ttu-id="f395e-184">割引が取り消されたときに適用される料金。</span><span class="sxs-lookup"><span data-stu-id="f395e-184">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="f395e-185">ライセンスベースの割引</span><span class="sxs-lookup"><span data-stu-id="f395e-185">License-based discounts</span></span>

<span data-ttu-id="f395e-186">ライセンスベースの割引を請求書にマップするには、ライセンス ベースのファイルの **TotalOtherDiscount** 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="f395e-186">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="f395e-187">*ライセンスベースの割引は、複数の料金の種類に適用できます。*</span><span class="sxs-lookup"><span data-stu-id="f395e-187">*License-based discounts may be applied to multiple charge types.*</span></span>
