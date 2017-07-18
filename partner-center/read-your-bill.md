---
title: "請求書の記載事項 | パートナー センター"
description: "請求書には、当月のすべての料金 (プログラム、製品、顧客の料金) の要約が記載されます。 請求書は、パートナー センターのダッシュボードで利用できます。"
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.openlocfilehash: 65c3777c0bd35933f2622fc0de105c051001974e
ms.sourcegitcommit: e8b504fa98b3ec4c7c8fd954f63ea81299791906
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/01/2017
---
# <a name="read-your-bill"></a><span data-ttu-id="f339e-104">請求書の記載事項</span><span class="sxs-lookup"><span data-stu-id="f339e-104">Read your bill</span></span>

**<span data-ttu-id="f339e-105">適用対象</span><span class="sxs-lookup"><span data-stu-id="f339e-105">Applies to</span></span>**

-  <span data-ttu-id="f339e-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="f339e-106">Partner Center</span></span>
-  <span data-ttu-id="f339e-107">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="f339e-107">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="f339e-108">Microsoft Cloud ドイツのパートナー センター</span><span class="sxs-lookup"><span data-stu-id="f339e-108">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="f339e-109">請求書には、当月のすべての料金 (プログラム、製品、顧客の料金) の要約が記載されます。</span><span class="sxs-lookup"><span data-stu-id="f339e-109">Your invoice is a summary of all charges (across the program, products, and customers) for the current monthly period.</span></span> <span data-ttu-id="f339e-110">請求書は、パートナー センターのダッシュボードで利用できます。</span><span class="sxs-lookup"><span data-stu-id="f339e-110">It is available on the Partner Center Dashboard.</span></span>

<span data-ttu-id="f339e-111">料金の項目別明細については、関連する調整ファイルを使用します。</span><span class="sxs-lookup"><span data-stu-id="f339e-111">For itemized details about the charges, use the accompanying reconciliation files.</span></span> <span data-ttu-id="f339e-112">調整ファイルには、顧客への請求書の作成に使用される顧客 ID とサブスクリプション ID が含まれます。</span><span class="sxs-lookup"><span data-stu-id="f339e-112">The reconciliation files include the customer IDs and subscription IDs that you will use to create customer invoices.</span></span> <span data-ttu-id="f339e-113">詳しくは、「[調整ファイルの使用](use-the-reconciliation-files.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f339e-113">For more information, see [How to use the reconciliation files](use-the-reconciliation-files.md).</span></span>

## <a name="invoice-file-definitions"></a><span data-ttu-id="f339e-114">請求書ファイルの定義</span><span class="sxs-lookup"><span data-stu-id="f339e-114">Invoice file definitions</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="f339e-115">フィールド</span><span class="sxs-lookup"><span data-stu-id="f339e-115">Field</span></span></strong></td>
<td><strong><span data-ttu-id="f339e-116">説明</span><span class="sxs-lookup"><span data-stu-id="f339e-116">Description</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f339e-117">US FEIN</span><span class="sxs-lookup"><span data-stu-id="f339e-117">US FEIN</span></span></td>
<td><span data-ttu-id="f339e-118">連邦税の ID 番号。</span><span class="sxs-lookup"><span data-stu-id="f339e-118">Your Federal Tax ID Number.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f339e-119">顧客番号</span><span class="sxs-lookup"><span data-stu-id="f339e-119">Customer number</span></span></td>
<td><span data-ttu-id="f339e-120">お客様の番号。</span><span class="sxs-lookup"><span data-stu-id="f339e-120">Your customer number.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f339e-121">請求先</span><span class="sxs-lookup"><span data-stu-id="f339e-121">Bill to</span></span></td>
<td><span data-ttu-id="f339e-122">請求書の送付先となる住所。</span><span class="sxs-lookup"><span data-stu-id="f339e-122">The address where we send your invoice.</span></span> <span data-ttu-id="f339e-123">この住所を変更するには、パートナー センターのアカウント プロファイルを編集します。</span><span class="sxs-lookup"><span data-stu-id="f339e-123">To change this address, edit your Partner Center account profile.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f339e-124">当月サービス利用料金</span><span class="sxs-lookup"><span data-stu-id="f339e-124">Recurring charges</span></span></td>
<td><span data-ttu-id="f339e-125">購入した使用量ベースのライセンスに対する定額の月額 (または年額) 料金で、サービスの前に課金されます。</span><span class="sxs-lookup"><span data-stu-id="f339e-125">The flat monthly (or annual) charges for the purchased usage-based licenses, billed in advance of the service.</span></span> <span data-ttu-id="f339e-126">この数値は、ライセンスベースの調整ファイルの &quot;Subtotal&quot; 列 (T 列) にあるすべての料金の合計です。</span><span class="sxs-lookup"><span data-stu-id="f339e-126">This number is the sum of all charges in the &quot;Subtotal&quot; column in the License-based reconciliation file (column T).</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f339e-127">利用料金</span><span class="sxs-lookup"><span data-stu-id="f339e-127">Usage charges</span></span></td>
<td><span data-ttu-id="f339e-128">請求月の間に有効にした、または使用された Azure の利用料金 (新しいサービスやアプリケーションが含まれます)。</span><span class="sxs-lookup"><span data-stu-id="f339e-128">Azure usage, including new services or applications enabled and used during the billing month.</span></span> <span data-ttu-id="f339e-129">この数値は、使用量ベースの調整ファイルの &quot;PretaxCharges&quot; 列 (Z 列) にあるすべての料金の合計です。</span><span class="sxs-lookup"><span data-stu-id="f339e-129">This number is the sum of all charges in the &quot;PretaxCharges&quot; column in the Usage-based reconciliation file (column Z).</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f339e-130">調整額</span><span class="sxs-lookup"><span data-stu-id="f339e-130">Credits &amp; adjustments</span></span></td>
<td><span data-ttu-id="f339e-131">サブスクリプションに加えられた変更内容 (シートの増減など) に対するクレジットまたは調整の金額。</span><span class="sxs-lookup"><span data-stu-id="f339e-131">Credits or adjustments for changes made to subscriptions (example: seat increases or decreases).</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f339e-132">その他の割引</span><span class="sxs-lookup"><span data-stu-id="f339e-132">Other discounts</span></span></td>
<td><span data-ttu-id="f339e-133">たとえば、サブスクリプションの通常価格に対してお客様が受け取る割引です。</span><span class="sxs-lookup"><span data-stu-id="f339e-133">For example, the discount that the customer receives from the normal price of the subscription.</span></span> <span data-ttu-id="f339e-134">これは単価やライセンスではなく、定額で表示されます。</span><span class="sxs-lookup"><span data-stu-id="f339e-134">This is shown as a flat amount, not as a price per unit or license.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f339e-135">税</span><span class="sxs-lookup"><span data-stu-id="f339e-135">Taxes</span></span></td>
<td><span data-ttu-id="f339e-136">請求書の 2 ページ目から始まる明細セクションに示される、現在の合計料金に対する税金の合計。</span><span class="sxs-lookup"><span data-stu-id="f339e-136">The total tax for the current charges as totaled in the details section beginning on page 2 of the invoice.</span></span> <span data-ttu-id="f339e-137">この数値は、以下の列にあるすべての料金の合計です。</span><span class="sxs-lookup"><span data-stu-id="f339e-137">This number is the sum of all the charges in:</span></span>
<ul>
<li><span data-ttu-id="f339e-138">使用量ベースの調整ファイルの &quot;TaxAmount&quot; 列 (AA 列)、および</span><span class="sxs-lookup"><span data-stu-id="f339e-138">the &quot;TaxAmount&quot; column of the Usage-based reconciliation file (column AA), and</span></span></li>
<li><span data-ttu-id="f339e-139">ライセンスベースのファイルの &quot;Tax&quot; 列 (U 列)。</span><span class="sxs-lookup"><span data-stu-id="f339e-139">the &quot;Tax&quot; column of the License-based file (column U).</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f339e-140">当月の請求額合計</span><span class="sxs-lookup"><span data-stu-id="f339e-140">Total current charges</span></span></td>
<td><span data-ttu-id="f339e-141">支払い期限ごとの、請求期間の請求通貨での支払い額。</span><span class="sxs-lookup"><span data-stu-id="f339e-141">The amount due in your billing currency for the billing period, due by the payment due date.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f339e-142">お支払いについて</span><span class="sxs-lookup"><span data-stu-id="f339e-142">Payment instructions</span></span></td>
<td><span data-ttu-id="f339e-143">地域に基づく、請求書の支払い方法の説明です。</span><span class="sxs-lookup"><span data-stu-id="f339e-143">Describes how to pay your invoice, based on your region.</span></span> <span data-ttu-id="f339e-144">支払いを行うときには、常に請求書番号を含めます。</span><span class="sxs-lookup"><span data-stu-id="f339e-144">Always include your invoice number when making a payment.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f339e-145">請求書番号</span><span class="sxs-lookup"><span data-stu-id="f339e-145">Invoice no</span></span></td>
<td><span data-ttu-id="f339e-146">請求書の番号。</span><span class="sxs-lookup"><span data-stu-id="f339e-146">The number of your invoice.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f339e-147">課金期間</span><span class="sxs-lookup"><span data-stu-id="f339e-147">Billing period</span></span></td>
<td><span data-ttu-id="f339e-148">CSP パートナー様は、月 1 回または年 1 回請求されます。</span><span class="sxs-lookup"><span data-stu-id="f339e-148">CSP partners are billed either monthly or annually.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f339e-149">請求書作成日</span><span class="sxs-lookup"><span data-stu-id="f339e-149">Invoice date</span></span></td>
<td><span data-ttu-id="f339e-150">請求書を受け取る日付。</span><span class="sxs-lookup"><span data-stu-id="f339e-150">The date you receive your invoice.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f339e-151">支払期日</span><span class="sxs-lookup"><span data-stu-id="f339e-151">Payment due date</span></span></td>
<td><span data-ttu-id="f339e-152">この日付までに、お客様からの支払いが受領される必要があります。</span><span class="sxs-lookup"><span data-stu-id="f339e-152">Your payment must be received by this date.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f339e-153">顧客 PO</span><span class="sxs-lookup"><span data-stu-id="f339e-153">Customer PO</span></span></td>
<td><span data-ttu-id="f339e-154">お客様の注文書番号です。</span><span class="sxs-lookup"><span data-stu-id="f339e-154">Your purchase order number.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f339e-155">カスタマー サービス</span><span class="sxs-lookup"><span data-stu-id="f339e-155">Customer service</span></span></td>
<td><span data-ttu-id="f339e-156">カスタマー サービスにアクセスするための Web サイトのアドレス。</span><span class="sxs-lookup"><span data-stu-id="f339e-156">The website address to access customer service.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f339e-157">サービス利用者</span><span class="sxs-lookup"><span data-stu-id="f339e-157">Service recipient</span></span></td>
<td><span data-ttu-id="f339e-158">サービスが使われる住所。</span><span class="sxs-lookup"><span data-stu-id="f339e-158">The address where the service is used.</span></span> <span data-ttu-id="f339e-159">(これは、会社の審査に関連付けられている会社の正式な住所です。変更することはできません)。</span><span class="sxs-lookup"><span data-stu-id="f339e-159">(This is the legal company address associated with company vetting and cannot be changed.)</span></span></td>
</tr>
</tbody>
</table>

 

 

 



