---
title: 調整ファイルの料金の種類 |パートナーセンター
ms.topic: article
ms.date: 08/26/2019
description: パートナーセンターの調整ファイルの料金の種類 (ライセンスベース、使用量ベース、1回限り)、クレジット、および割引。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 064ed6dda28f5a8ace64942d55ef2a6327528ff5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389810"
---
# <a name="understand-charge-types"></a><span data-ttu-id="e7249-103">料金の種類について</span><span class="sxs-lookup"><span data-stu-id="e7249-103">Understand charge types</span></span>

<span data-ttu-id="e7249-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="e7249-104">Applies to:</span></span>

- <span data-ttu-id="e7249-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="e7249-105">Partner Center</span></span>
- <span data-ttu-id="e7249-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="e7249-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="e7249-107">このトピックでは、請求書セクションと、調整ファイルに存在する可能性のある関連する料金の種類とのマッピングについて説明します。</span><span class="sxs-lookup"><span data-stu-id="e7249-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="e7249-108">請求書には、料金の概要が表示されます。</span><span class="sxs-lookup"><span data-stu-id="e7249-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="e7249-109">調整ファイルには、料金の種類など、行アイテムトランザクションの詳細な内訳が表示されます。</span><span class="sxs-lookup"><span data-stu-id="e7249-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="e7249-110">調整ファイルの詳細については、「[調整ファイルの使用方法](use-the-reconciliation-files.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7249-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="e7249-111">[使用量に基づく調整ファイル](usage-based-recon-files.md)と[ライセンスベースの調整ファイル](license-based-recon-files.md)はどちらも、使用状況に関連するトランザクションと料金 (使用されたユニットと関連する料金) のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="e7249-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="e7249-112">請求書に**調整**として表示される1回限りのクレジット、割引、返金は、調整ファイルには表示されません。</span><span class="sxs-lookup"><span data-stu-id="e7249-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="e7249-113">請求書の料金に種類をマップする</span><span class="sxs-lookup"><span data-stu-id="e7249-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="e7249-114">請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルターオプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="e7249-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="e7249-115">調整ファイルの料金の種類でフィルター処理して、請求書の料金を調整ファイルの一連の課金の内訳にマップします。</span><span class="sxs-lookup"><span data-stu-id="e7249-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="e7249-116">ライセンスベースの料金</span><span class="sxs-lookup"><span data-stu-id="e7249-116">License-based charges</span></span>

<span data-ttu-id="e7249-117">これらのライセンスベースの料金を請求書にマッピングするには、ライセンスベースのファイルから**Amount**列を合計します。</span><span class="sxs-lookup"><span data-stu-id="e7249-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="e7249-118">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="e7249-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e7249-119">料金の説明</span><span class="sxs-lookup"><span data-stu-id="e7249-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e7249-120">アクティブ化料金</span><span class="sxs-lookup"><span data-stu-id="e7249-120">Activation fee</span></span> | <span data-ttu-id="e7249-121">購入後にサブスクリプションを使用する場合に、顧客に請求される金額。</span><span class="sxs-lookup"><span data-stu-id="e7249-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="e7249-122">取り消し料金</span><span class="sxs-lookup"><span data-stu-id="e7249-122">Cancel fee</span></span> | <span data-ttu-id="e7249-123">日割りは、関連付けられたシートが変更された場合に、お客様に返金されます。</span><span class="sxs-lookup"><span data-stu-id="e7249-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="e7249-124">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="e7249-124">Cycle fee</span></span> | <span data-ttu-id="e7249-125">サブスクリプションに対する定期的な料金。</span><span class="sxs-lookup"><span data-stu-id="e7249-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="e7249-126">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="e7249-126">Cycle instance prorate</span></span> | <span data-ttu-id="e7249-127">関連付けられているシートが変更された場合に、日割り料金が顧客から評価されます。</span><span class="sxs-lookup"><span data-stu-id="e7249-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="e7249-128">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="e7249-128">Prorate fees when cancel</span></span> | <span data-ttu-id="e7249-129">キャンセル時のサービスの未使用部分の日割り返金。</span><span class="sxs-lookup"><span data-stu-id="e7249-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="e7249-130">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="e7249-130">Prorate fees when purchase</span></span> | <span data-ttu-id="e7249-131">年間請求書を使用する場合のサブスクリプションの料金の種類。</span><span class="sxs-lookup"><span data-stu-id="e7249-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="e7249-132">Purchase fee</span><span class="sxs-lookup"><span data-stu-id="e7249-132">Purchase fee</span></span> | <span data-ttu-id="e7249-133">毎月の課金を使用する場合のサブスクリプションの料金の種類。</span><span class="sxs-lookup"><span data-stu-id="e7249-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="e7249-134">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="e7249-134">Prorate fee when renew</span></span> | <span data-ttu-id="e7249-135">サブスクリプションの更新時の日割り料金。</span><span class="sxs-lookup"><span data-stu-id="e7249-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="e7249-136">Renew fee</span><span class="sxs-lookup"><span data-stu-id="e7249-136">Renew fee</span></span> | <span data-ttu-id="e7249-137">サブスクリプションの更新時の課金</span><span class="sxs-lookup"><span data-stu-id="e7249-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="e7249-138">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="e7249-138">Prorate fees when activate</span></span> | <span data-ttu-id="e7249-139">請求期間が終了するまで、ライセンス認証の > 日割り料金がかかります。</span><span class="sxs-lookup"><span data-stu-id="e7249-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="e7249-140">1回限りの料金</span><span class="sxs-lookup"><span data-stu-id="e7249-140">One-time charges</span></span>

<span data-ttu-id="e7249-141">この1回限りの料金を請求書にマップするには、ライセンスベースのファイルから**Amount**列を合計します。</span><span class="sxs-lookup"><span data-stu-id="e7249-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="e7249-142">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="e7249-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e7249-143">料金の説明</span><span class="sxs-lookup"><span data-stu-id="e7249-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e7249-144">新規</span><span class="sxs-lookup"><span data-stu-id="e7249-144">New</span></span> | <span data-ttu-id="e7249-145">新しい購入が作成されるときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="e7249-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="e7249-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="e7249-146">addQuantity</span></span> | <span data-ttu-id="e7249-147">元の購入の返金と、増加後の新しい数量の両方で使用されます。</span><span class="sxs-lookup"><span data-stu-id="e7249-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="e7249-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="e7249-148">removeQuantity</span></span> | <span data-ttu-id="e7249-149">元の購入の返金と、減少後の新しい数量の両方で使用されます。</span><span class="sxs-lookup"><span data-stu-id="e7249-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="e7249-150">キャンセル</span><span class="sxs-lookup"><span data-stu-id="e7249-150">Cancel</span></span> | <span data-ttu-id="e7249-151">サブスクリプションが取り消されたときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="e7249-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="e7249-152">Convert</span><span class="sxs-lookup"><span data-stu-id="e7249-152">Convert</span></span> | <span data-ttu-id="e7249-153">ライセンスをアップグレードするときに使用しますが、接続クライアント数は変更されません。</span><span class="sxs-lookup"><span data-stu-id="e7249-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="e7249-154">利用料金</span><span class="sxs-lookup"><span data-stu-id="e7249-154">Usage charges</span></span>

<span data-ttu-id="e7249-155">これらの使用料金を請求書にマッピングするには、使用量に基づくファイルから、[の**Ax料金**] 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="e7249-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="e7249-156">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="e7249-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e7249-157">料金の説明</span><span class="sxs-lookup"><span data-stu-id="e7249-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e7249-158">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="e7249-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="e7249-159">現在の請求期間中に未払いの使用をキャンセルしたときのアクセス使用料。</span><span class="sxs-lookup"><span data-stu-id="e7249-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="e7249-160">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="e7249-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="e7249-161">現在の請求期間のアクセス使用料。</span><span class="sxs-lookup"><span data-stu-id="e7249-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="e7249-162">クレジット</span><span class="sxs-lookup"><span data-stu-id="e7249-162">Credits</span></span>

<span data-ttu-id="e7249-163">これらのクレジットを請求書にマップするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="e7249-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="e7249-164">ライセンスベースのファイルから**Totalforcustomer**を合計します。</span><span class="sxs-lookup"><span data-stu-id="e7249-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="e7249-165">使用状況に基づくファイルから**PostTaxTotal**列を合計します。</span><span class="sxs-lookup"><span data-stu-id="e7249-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="e7249-166">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="e7249-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e7249-167">料金の説明</span><span class="sxs-lookup"><span data-stu-id="e7249-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e7249-168">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="e7249-168">Offset a line item</span></span> | <span data-ttu-id="e7249-169">商品の一部または全体が税金を含む品目に返金します。</span><span class="sxs-lookup"><span data-stu-id="e7249-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="e7249-170">使用量ベースの割引</span><span class="sxs-lookup"><span data-stu-id="e7249-170">Usage-based discounts</span></span>

<span data-ttu-id="e7249-171">これらの使用量に基づく割引を請求書にマップするには、使用量に基づくファイルから、[の**Ax料金**] 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="e7249-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="e7249-172">料金の説明 (調整ファイルの ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="e7249-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e7249-173">料金の説明</span><span class="sxs-lookup"><span data-stu-id="e7249-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e7249-174">Activation discount</span><span class="sxs-lookup"><span data-stu-id="e7249-174">Activation discount</span></span> | <span data-ttu-id="e7249-175">サブスクリプションがアクティブになったときに適用される割引。</span><span class="sxs-lookup"><span data-stu-id="e7249-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="e7249-176">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="e7249-176">Cycle discount</span></span> | <span data-ttu-id="e7249-177">定期的な料金に適用される割引。</span><span class="sxs-lookup"><span data-stu-id="e7249-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="e7249-178">Renew discount</span><span class="sxs-lookup"><span data-stu-id="e7249-178">Renew discount</span></span> | <span data-ttu-id="e7249-179">サブスクリプションが更新されたときに適用される割引。</span><span class="sxs-lookup"><span data-stu-id="e7249-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="e7249-180">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="e7249-180">Cancel discount</span></span> | <span data-ttu-id="e7249-181">割引が取り消された場合に適用される料金。</span><span class="sxs-lookup"><span data-stu-id="e7249-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="e7249-182">ライセンスベースの割引</span><span class="sxs-lookup"><span data-stu-id="e7249-182">License-based discounts</span></span>

<span data-ttu-id="e7249-183">ライセンスベースの割引を請求書にマップするには、ライセンスベースのファイルの合計**割引**列を合計します。</span><span class="sxs-lookup"><span data-stu-id="e7249-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="e7249-184">*ライセンスベースの割引は、複数の種類の料金に適用できます。*</span><span class="sxs-lookup"><span data-stu-id="e7249-184">*License-based discounts may be applied to multiple charge types.*</span></span>
