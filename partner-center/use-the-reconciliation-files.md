---
title: 調整ファイルの使用 | パートナー センター
description: 請求サイクルの各料金の詳しい行項目ビューについては、パートナー センターのダッシュボードから調整ファイルをダウンロードします。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 51716e8abedf83237050cb51bc76e54a954cd28b
ms.sourcegitcommit: ec00affdfc79c1346cf8df482ce39dae98e20772
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/28/2018
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="2dd79-103">調整ファイルの使用</span><span class="sxs-lookup"><span data-stu-id="2dd79-103">Use the reconciliation files</span></span>

**<span data-ttu-id="2dd79-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="2dd79-104">Applies to</span></span>**

-  <span data-ttu-id="2dd79-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="2dd79-105">Partner Center</span></span>
-  <span data-ttu-id="2dd79-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="2dd79-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="2dd79-107">Microsoft Cloud ドイツのパートナー センター</span><span class="sxs-lookup"><span data-stu-id="2dd79-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="2dd79-108">請求サイクルの各料金の詳しい行項目ビューについては、パートナー センターのダッシュボードから調整ファイルをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="2dd79-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="2dd79-109">詳細には、各顧客のサブスクリプションの料金や、詳細なイベント (期間途中でのサブスクリプションへのシートの追加など) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="2dd79-110">パートナーごとに明細を示す</span><span class="sxs-lookup"><span data-stu-id="2dd79-110">Itemize by partner</span></span>


<span data-ttu-id="2dd79-111">インダイレクト モデルのパートナーは、ライセンスベースの調整ファイルと使用量ベースの調整ファイルの両方で、これらの追加フィールドを使用してリセラーごとに明細を記載できます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="2dd79-112">MPN ID</span><span class="sxs-lookup"><span data-stu-id="2dd79-112">MPN ID</span></span></th>
<th><span data-ttu-id="2dd79-113">説明</span><span class="sxs-lookup"><span data-stu-id="2dd79-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="2dd79-114">MPN ID</span><span class="sxs-lookup"><span data-stu-id="2dd79-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="2dd79-115">CSP パートナー (直接または間接) の Microsoft Partner Network (MPN) IDです。</span><span class="sxs-lookup"><span data-stu-id="2dd79-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-116">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="2dd79-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="2dd79-117">インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="2dd79-118">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="2dd79-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="2dd79-119">これは、パートナー センターで特定のサブスクリプションについて示されるリセラー ID に対応します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="2dd79-120">リセラーを表示または更新するには、パートナー センター メニューで <strong>[顧客]</strong> を選び、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-120">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="2dd79-121">顧客メニューで <strong>[サブスクリプション]</strong> を選び、一覧からサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="2dd79-122"><strong>[更新]</strong> を選んで、<strong>[再販業者 (MPN ID)]</strong> を変更します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="2dd79-123">CSP パートナーがお客様に直接サブスクリプションを販売した場合、パートナーの MPN ID が MPN ID とリセラーの MPN ID として 2 か所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="2dd79-124">CSP パートナーのリセラーに MPN ID がない場合は、代わりに CSP パートナーの MPN ID がこの値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="2dd79-125">CSP パートナーがリセラー ID を削除した場合、この値は -1 に設定されます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="2dd79-126">ライセンスベースのファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="2dd79-126">License-based file fields</span></span>


<span data-ttu-id="2dd79-127">顧客の注文に対する料金を調整するには、調整ファイルの Syndication\_Partner\_Subscription\_Number とパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="2dd79-128">列</span><span class="sxs-lookup"><span data-stu-id="2dd79-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="2dd79-129">説明</span><span class="sxs-lookup"><span data-stu-id="2dd79-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="2dd79-130">サンプル値</span><span class="sxs-lookup"><span data-stu-id="2dd79-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-131">PartnerId</span><span class="sxs-lookup"><span data-stu-id="2dd79-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="2dd79-132">特定の課金エンティティの一意の識別子 (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="2dd79-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="2dd79-133">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="2dd79-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="2dd79-134">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="2dd79-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="2dd79-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="2dd79-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="2dd79-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="2dd79-137">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="2dd79-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="2dd79-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="2dd79-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="2dd79-139">OrderID</span></span></td>
<td><p><span data-ttu-id="2dd79-140">Microsoft 課金プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="2dd79-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="2dd79-141">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="2dd79-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="2dd79-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="2dd79-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="2dd79-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="2dd79-144">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="2dd79-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="2dd79-145">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="2dd79-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="2dd79-146">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="2dd79-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="2dd79-147">「Syndication_Partner_Subscription_Number」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2dd79-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="2dd79-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="2dd79-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="2dd79-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="2dd79-150">サブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="2dd79-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="2dd79-151">お客様は同じプランで複数のサブスクリプションを持つことができるため、これは調整ファイルの分析で重要です。</span><span class="sxs-lookup"><span data-stu-id="2dd79-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="2dd79-152">このフィールドは、パートナー管理コンソールのサブスクリプション ID にマップされます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="2dd79-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="2dd79-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="2dd79-154">OfferID</span></span></td>
<td><p><span data-ttu-id="2dd79-155">一意のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="2dd79-155">Unique offer ID.</span></span> <span data-ttu-id="2dd79-156">価格表に従った標準のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="2dd79-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="2dd79-157"><b>注</b>: この値は、価格表のプラン ID とは一致しません。</span><span class="sxs-lookup"><span data-stu-id="2dd79-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="2dd79-158">以下の DurableOfferID を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2dd79-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="2dd79-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="2dd79-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="2dd79-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="2dd79-161">価格表で定義されている一意の継続的なプラン ID。</span><span class="sxs-lookup"><span data-stu-id="2dd79-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="2dd79-162"><b>注</b>: この値は価格表のプラン ID と一致します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="2dd79-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="2dd79-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="2dd79-164">OfferName</span></span></td>
<td><p><span data-ttu-id="2dd79-165">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="2dd79-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="2dd79-166">Microsoft Office 365 (プラン E3)</span><span class="sxs-lookup"><span data-stu-id="2dd79-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="2dd79-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="2dd79-168">サブスクリプションの開始日。注文が送信された日に設定されます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="2dd79-169">サブスクリプションの開始日を終了日と共に確認することにより、顧客がサブスクリプションの最初の 1 年以内であるか、サブスクリプションが次の 1 年間更新されたかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="2dd79-170">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="2dd79-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="2dd79-171">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="2dd79-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="2dd79-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="2dd79-173">サブスクリプション終了日: 開始日から 12 か月 + x 日後 (パートナーの請求日と合わせる) または更新日から 12 か月</span><span class="sxs-lookup"><span data-stu-id="2dd79-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="2dd79-174">更新時に、価格は最新の価格表に更新されます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="2dd79-175">自動更新の前に、顧客とのやり取りが必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="2dd79-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="2dd79-176">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="2dd79-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="2dd79-177">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="2dd79-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="2dd79-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="2dd79-179">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="2dd79-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="2dd79-180">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="2dd79-181">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="2dd79-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="2dd79-182">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="2dd79-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="2dd79-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="2dd79-184">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="2dd79-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="2dd79-185">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="2dd79-186">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="2dd79-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="2dd79-187">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="2dd79-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="2dd79-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="2dd79-189">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="2dd79-189">The type of charge or adjustment.</span></span> <span data-ttu-id="2dd79-190">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2dd79-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="2dd79-191">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2dd79-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="2dd79-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="2dd79-193">シート単価 (購入時に価格表に公開されていた価格)。</span><span class="sxs-lookup"><span data-stu-id="2dd79-193">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="2dd79-194">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="2dd79-195">6.82</span><span class="sxs-lookup"><span data-stu-id="2dd79-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-196">Quantity</span><span class="sxs-lookup"><span data-stu-id="2dd79-196">Quantity</span></span></td>
<td><p><span data-ttu-id="2dd79-197">シート数。</span><span class="sxs-lookup"><span data-stu-id="2dd79-197">Number of seats.</span></span> <span data-ttu-id="2dd79-198">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="2dd79-199">2</span><span class="sxs-lookup"><span data-stu-id="2dd79-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-200">Amount</span><span class="sxs-lookup"><span data-stu-id="2dd79-200">Amount</span></span></td>
<td><p><span data-ttu-id="2dd79-201">数量に対する合計価格。</span><span class="sxs-lookup"><span data-stu-id="2dd79-201">Total of price for quantity.</span></span> <span data-ttu-id="2dd79-202">金額の計算が、この顧客用の計算方法に一致することを確認するために役立ちます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="2dd79-203">13.32</span><span class="sxs-lookup"><span data-stu-id="2dd79-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="2dd79-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="2dd79-205">これらの料金に適用される割引額。</span><span class="sxs-lookup"><span data-stu-id="2dd79-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="2dd79-206">インセンティブの対象となる IUR または新しいサブスクリプションの場合も、この列に割引額が含まれます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="2dd79-207">2.32</span><span class="sxs-lookup"><span data-stu-id="2dd79-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-208">Subtotal</span><span class="sxs-lookup"><span data-stu-id="2dd79-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="2dd79-209">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="2dd79-209">Total before tax.</span></span> <span data-ttu-id="2dd79-210">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="2dd79-211">11</span><span class="sxs-lookup"><span data-stu-id="2dd79-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-212">Tax</span><span class="sxs-lookup"><span data-stu-id="2dd79-212">Tax</span></span></td>
<td><p><span data-ttu-id="2dd79-213">市場の税関連の規則や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="2dd79-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="2dd79-214">0</span><span class="sxs-lookup"><span data-stu-id="2dd79-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="2dd79-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="2dd79-216">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="2dd79-216">Total after tax.</span></span> <span data-ttu-id="2dd79-217">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="2dd79-218">11</span><span class="sxs-lookup"><span data-stu-id="2dd79-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-219">Currency</span><span class="sxs-lookup"><span data-stu-id="2dd79-219">Currency</span></span></td>
<td><p><span data-ttu-id="2dd79-220">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="2dd79-220">Currency type.</span></span> <span data-ttu-id="2dd79-221">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="2dd79-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="2dd79-222">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="2dd79-223">EUR</span><span class="sxs-lookup"><span data-stu-id="2dd79-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="2dd79-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="2dd79-225">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="2dd79-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="2dd79-226">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="2dd79-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="2dd79-227">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="2dd79-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="2dd79-228">MPNID</span></span></td>
<td><p><span data-ttu-id="2dd79-229">CSP パートナーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="2dd79-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="2dd79-230">4390934</span><span class="sxs-lookup"><span data-stu-id="2dd79-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="2dd79-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="2dd79-232">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="2dd79-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="2dd79-233">「[パートナーごとに明細を示す](#itemizebypartner)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2dd79-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="2dd79-234">4390934</span><span class="sxs-lookup"><span data-stu-id="2dd79-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="2dd79-235">DomainName</span></span></td>
<td><p><span data-ttu-id="2dd79-236">顧客のドメイン名。顧客を特定できるようにするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-236">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="2dd79-237">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="2dd79-237">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-238">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="2dd79-238">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="2dd79-239">サブスクリプションのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="2dd79-239">Subscription nickname.</span></span> <span data-ttu-id="2dd79-240">ニックネームが指定されていない場合、パートナー センターでは OfferName を使用します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-240">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="2dd79-241">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="2dd79-241">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-242">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="2dd79-242">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="2dd79-243">価格表で定義されている、顧客が購入したサービス プランの名前 </span><span class="sxs-lookup"><span data-stu-id="2dd79-243">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="2dd79-244">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="2dd79-244">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="2dd79-245">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span><span class="sxs-lookup"><span data-stu-id="2dd79-245">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="2dd79-246">使用量ベースのファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="2dd79-246">Usage-based file fields</span></span>


<span data-ttu-id="2dd79-247">顧客の使用量に対する料金を調整するには、調整ファイルの ResellerID/ResellerName/ResellerBillableAccount、顧客名、およびパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-247">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="2dd79-248">次のフィールドで、どのサービスが使用されるか、およびレートについて説明します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-248">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="2dd79-249">列</span><span class="sxs-lookup"><span data-stu-id="2dd79-249">Column</span></span></strong></td>
<td><strong><span data-ttu-id="2dd79-250">説明</span><span class="sxs-lookup"><span data-stu-id="2dd79-250">Description</span></span></strong></td>
<td><strong><span data-ttu-id="2dd79-251">サンプル値</span><span class="sxs-lookup"><span data-stu-id="2dd79-251">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-252">PartnerID</span><span class="sxs-lookup"><span data-stu-id="2dd79-252">PartnerID</span></span></td>
<td><p><span data-ttu-id="2dd79-253">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="2dd79-253">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="2dd79-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="2dd79-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-255">PartnerName</span><span class="sxs-lookup"><span data-stu-id="2dd79-255">PartnerName</span></span></td>
<td><p><span data-ttu-id="2dd79-256">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="2dd79-256">Partner Name.</span></span></p></td>
<td><span data-ttu-id="2dd79-257">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="2dd79-257">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-258">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="2dd79-258">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="2dd79-259">パートナーのアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="2dd79-259">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="2dd79-260">1010578050</span><span class="sxs-lookup"><span data-stu-id="2dd79-260">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-261">CustomerName</span><span class="sxs-lookup"><span data-stu-id="2dd79-261">CustomerName</span></span></td>
<td><p><span data-ttu-id="2dd79-262">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="2dd79-262">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="2dd79-263">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="2dd79-263">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="2dd79-264">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="2dd79-264">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-265">MPNID</span><span class="sxs-lookup"><span data-stu-id="2dd79-265">MPNID</span></span></td>
<td><p><span data-ttu-id="2dd79-266">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="2dd79-266">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="2dd79-267">4390934</span><span class="sxs-lookup"><span data-stu-id="2dd79-267">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-268">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="2dd79-268">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="2dd79-269">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="2dd79-269">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="2dd79-270">「[パートナーごとに明細を示す](#itemizebypartner)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2dd79-270">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="2dd79-271">4390934</span><span class="sxs-lookup"><span data-stu-id="2dd79-271">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-272">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="2dd79-272">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="2dd79-273">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="2dd79-273">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="2dd79-274">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="2dd79-274">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-275">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="2dd79-275">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="2dd79-276">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="2dd79-276">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="2dd79-277">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="2dd79-277">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="2dd79-278">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="2dd79-278">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-279">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="2dd79-279">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="2dd79-280">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="2dd79-280">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="2dd79-281">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="2dd79-281">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="2dd79-282">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="2dd79-282">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-283">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="2dd79-283">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="2dd79-284">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="2dd79-284">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="2dd79-285">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="2dd79-285">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="2dd79-286">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="2dd79-286">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="2dd79-287">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="2dd79-287">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-288">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="2dd79-288">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="2dd79-289">サービス プランのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="2dd79-289">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="2dd79-290">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="2dd79-290">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-291">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="2dd79-291">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="2dd79-292">サービス プランの基幹業務</span><span class="sxs-lookup"><span data-stu-id="2dd79-292">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="2dd79-293">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="2dd79-293">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-294">OrderID</span><span class="sxs-lookup"><span data-stu-id="2dd79-294">OrderID</span></span></td>
<td><p><span data-ttu-id="2dd79-295">Microsoft 課金プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="2dd79-295">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="2dd79-296">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="2dd79-296">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="2dd79-297">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="2dd79-297">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-298">ServiceName</span><span class="sxs-lookup"><span data-stu-id="2dd79-298">ServiceName</span></span></td>
<td><p><span data-ttu-id="2dd79-299">対象の Azure サービスの名前。</span><span class="sxs-lookup"><span data-stu-id="2dd79-299">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="2dd79-300">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="2dd79-300">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-301">ServiceType</span><span class="sxs-lookup"><span data-stu-id="2dd79-301">ServiceType</span></span></td>
<td><p><span data-ttu-id="2dd79-302">Windows Azure サービスの特定の種類。</span><span class="sxs-lookup"><span data-stu-id="2dd79-302">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="2dd79-303">Service Bus – Individual or Pack</span><span class="sxs-lookup"><span data-stu-id="2dd79-303">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="2dd79-304">SQL Azure database – Business or Web Edition</span><span class="sxs-lookup"><span data-stu-id="2dd79-304">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-305">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="2dd79-305">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="2dd79-306">すべてのサービス データおよび価格設定構造の特定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="2dd79-306">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="2dd79-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="2dd79-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-308">リソース名</span><span class="sxs-lookup"><span data-stu-id="2dd79-308">Resource Name</span></span></td>
<td><p><span data-ttu-id="2dd79-309">Azure リソースの名前。</span><span class="sxs-lookup"><span data-stu-id="2dd79-309">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="2dd79-310">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="2dd79-310">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="2dd79-311">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="2dd79-311">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-312">Region</span><span class="sxs-lookup"><span data-stu-id="2dd79-312">Region</span></span></td>
<td><p><span data-ttu-id="2dd79-313">使用量が適用される地域。</span><span class="sxs-lookup"><span data-stu-id="2dd79-313">The region the usage applies to.</span></span> <span data-ttu-id="2dd79-314">料金は地域によって異なるため、主にデータ転送に料金を割り当てるために使われます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-314">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="2dd79-315">Asia Pacific、Europe、Latin America、North America</span><span class="sxs-lookup"><span data-stu-id="2dd79-315">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-316">SKU</span><span class="sxs-lookup"><span data-stu-id="2dd79-316">SKU</span></span></td>
<td><p><span data-ttu-id="2dd79-317">プランについての MSFT の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="2dd79-317">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="2dd79-318">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="2dd79-318">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="2dd79-319">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="2dd79-319">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="2dd79-320">特定の課金期間のサービスまたはリソースに対してさまざまなレートの明細を設定するための ID と数量。</span><span class="sxs-lookup"><span data-stu-id="2dd79-320">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="2dd79-321">Azure の階層化されたレーティングの場合は、一定数量の課金可能単位までは 1 つのレートがあり、その後に別のレートがあることがあります。</span><span class="sxs-lookup"><span data-stu-id="2dd79-321">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="2dd79-322">1</span><span class="sxs-lookup"><span data-stu-id="2dd79-322">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-323">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="2dd79-323">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="2dd79-324">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="2dd79-324">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="2dd79-325">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-325">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="2dd79-326">11</span><span class="sxs-lookup"><span data-stu-id="2dd79-326">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-327">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="2dd79-327">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="2dd79-328">単位数はプランの一部として含まれます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-328">Units included as part of the offer.</span></span> <span data-ttu-id="2dd79-329">通常、CSP には含まれません。</span><span class="sxs-lookup"><span data-stu-id="2dd79-329">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="2dd79-330">0</span><span class="sxs-lookup"><span data-stu-id="2dd79-330">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="2dd79-331">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="2dd79-331">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="2dd79-332">単位数はプランの一部として含まれず、パートナーが支払う必要があります。</span><span class="sxs-lookup"><span data-stu-id="2dd79-332">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="2dd79-333">ConsumedQuantity - IncludedQuantity と同じです。</span><span class="sxs-lookup"><span data-stu-id="2dd79-333">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="2dd79-334">11</span><span class="sxs-lookup"><span data-stu-id="2dd79-334">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-335">ListPrice</span><span class="sxs-lookup"><span data-stu-id="2dd79-335">ListPrice</span></span></td>
<td><p><span data-ttu-id="2dd79-336">サブスクリプションの開始日に有効な価格を提供します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-336">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="2dd79-337">$0.0808</span><span class="sxs-lookup"><span data-stu-id="2dd79-337">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-338">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="2dd79-338">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="2dd79-339">ListPrist と OverageQuantity を掛けて、最も近いセントに丸めます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-339">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="2dd79-340">$0.085</span><span class="sxs-lookup"><span data-stu-id="2dd79-340">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-341">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="2dd79-341">TaxAmount</span></span></td>
<td><p><span data-ttu-id="2dd79-342">市場の税関連の規則や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="2dd79-342">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="2dd79-343">$0.08</span><span class="sxs-lookup"><span data-stu-id="2dd79-343">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-344">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="2dd79-344">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="2dd79-345">税が適用されるときの税引き後の合計額。</span><span class="sxs-lookup"><span data-stu-id="2dd79-345">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="2dd79-346">$0.93</span><span class="sxs-lookup"><span data-stu-id="2dd79-346">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-347">Currency</span><span class="sxs-lookup"><span data-stu-id="2dd79-347">Currency</span></span></td>
<td><p><span data-ttu-id="2dd79-348">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="2dd79-348">Currency type.</span></span> <span data-ttu-id="2dd79-349">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="2dd79-349">Each billing entity has only one currency.</span></span> <span data-ttu-id="2dd79-350">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-350">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="2dd79-351">EUR</span><span class="sxs-lookup"><span data-stu-id="2dd79-351">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-352">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="2dd79-352">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="2dd79-353">単位あたりの税込み価格。</span><span class="sxs-lookup"><span data-stu-id="2dd79-353">Pretax price per unit.</span></span> <span data-ttu-id="2dd79-354">PretaxCharges / OverageQuantity と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-354">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="2dd79-355">$0.08</span><span class="sxs-lookup"><span data-stu-id="2dd79-355">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-356">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="2dd79-356">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="2dd79-357">単位あたりの税引き後の価格。</span><span class="sxs-lookup"><span data-stu-id="2dd79-357">Post tax price per unit.</span></span> <span data-ttu-id="2dd79-358">PostTaxTotal / OverageQuantity、または PretaxEffectiveRate + 単位額あたりの税率と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-358">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="2dd79-359">$0.08</span><span class="sxs-lookup"><span data-stu-id="2dd79-359">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-360">ChargeType</span><span class="sxs-lookup"><span data-stu-id="2dd79-360">ChargeType</span></span></td>
<td><p><span data-ttu-id="2dd79-361">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="2dd79-361">The type of charge or adjustment.</span></span> <span data-ttu-id="2dd79-362">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2dd79-362">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="2dd79-363">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2dd79-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-364">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="2dd79-364">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="2dd79-365">MSFT 課金プラットフォームの一意のアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="2dd79-365">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="2dd79-366">1280018095</span><span class="sxs-lookup"><span data-stu-id="2dd79-366">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-367">UsageDate</span><span class="sxs-lookup"><span data-stu-id="2dd79-367">UsageDate</span></span></td>
<td><p><span data-ttu-id="2dd79-368">サービスの展開の日付。</span><span class="sxs-lookup"><span data-stu-id="2dd79-368">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="2dd79-369">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="2dd79-369">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-370">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="2dd79-370">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="2dd79-371">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-371">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="2dd79-372">East Asia、South East Asia、North Europe、West Europe、North Central US、South Central US</span><span class="sxs-lookup"><span data-stu-id="2dd79-372">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-373">MeteredService</span><span class="sxs-lookup"><span data-stu-id="2dd79-373">MeteredService</span></span></td>
<td><p><span data-ttu-id="2dd79-374">この列は、[Service Name] 列で特に識別されない可能性のある、個別の Microsoft Azure サービスの追跡に利用されます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-374">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="2dd79-375">たとえば、データ転送は、[Service Name] 列で &quot;Microsoft Azure - All Services&quot; と報告されます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-375">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="2dd79-376">この [MeteredService] 列は、利用に関連する特定のサービスを示します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-376">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="2dd79-377">AccessControl、CDN、Compute、Database、ServiceBus、Storage</span><span class="sxs-lookup"><span data-stu-id="2dd79-377">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-378">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="2dd79-378">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="2dd79-379">個々の Microsoft Azure サービスの内容を、MeteredService フィールドで提供されるレベルよりも明確にする小見出し。</span><span class="sxs-lookup"><span data-stu-id="2dd79-379">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="2dd79-380">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="2dd79-380">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-381">Project</span><span class="sxs-lookup"><span data-stu-id="2dd79-381">Project</span></span></td>
<td><p><span data-ttu-id="2dd79-382">サービス インスタンスの顧客定義の名前</span><span class="sxs-lookup"><span data-stu-id="2dd79-382">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="2dd79-383">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="2dd79-383">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-384">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="2dd79-384">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="2dd79-385">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="2dd79-385">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="2dd79-386">例: 1 か月 30 日間の中に、個別にプロビジョニングされた接続がある場合、Service Info 1 は "1.000000 Connections / 30 days" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-386">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="2dd79-387">プロビジョニングされた ServiceBus 接続が 25 パックあり、その日に 1 つを利用した場合、その日の 1 日の使用量の計算書には、"25 Connections / 30 Days – Used: 1.000000" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-387">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-388">CustomerID</span><span class="sxs-lookup"><span data-stu-id="2dd79-388">CustomerID</span></span></td>
<td><p><span data-ttu-id="2dd79-389">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="2dd79-389">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="2dd79-390">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="2dd79-390">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="2dd79-391">DomainName</span><span class="sxs-lookup"><span data-stu-id="2dd79-391">DomainName</span></span></td>
<td><p><span data-ttu-id="2dd79-392">顧客のドメイン名。顧客を特定できるようにするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-392">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="2dd79-393">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="2dd79-393">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="2dd79-394">Unit</span><span class="sxs-lookup"><span data-stu-id="2dd79-394">Unit</span></span></td>
<td><p><span data-ttu-id="2dd79-395">リソース名の単位</span><span class="sxs-lookup"><span data-stu-id="2dd79-395">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="2dd79-396">GB または HOURS</span><span class="sxs-lookup"><span data-stu-id="2dd79-396">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>



## <a href="" id="charge_types"></a><span data-ttu-id="2dd79-397">請求書と調整ファイルの間の課金のマッピング</span><span class="sxs-lookup"><span data-stu-id="2dd79-397">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="2dd79-398">請求書は料金の概要を示し、調整ファイルは、課金の種類を含め、行項目のトランザクションの詳細な内訳を示します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-398">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="2dd79-399">請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルター オプションを使用して、調整ファイルの課金の種類でフィルター処理し、請求書の課金を調整ファイルの一連の課金の内訳にマップします。</span><span class="sxs-lookup"><span data-stu-id="2dd79-399">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="2dd79-400">使用量ベースとライセンス ベースの調整ファイルには、使用量関連のトランザクションと料金 (消費された単位量および関連する料金) のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-400">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="2dd79-401">請求書に “調整” として表示される単発のクレジット、割引、払い戻し金額は、調整ファイルに表示されません。</span><span class="sxs-lookup"><span data-stu-id="2dd79-401">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="2dd79-402">次の表に、請求書のセクションと、調整ファイルに表示される関連付けられた課金の種類とのマッピングを示します。</span><span class="sxs-lookup"><span data-stu-id="2dd79-402">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="2dd79-403">請求書の課金の説明</span><span class="sxs-lookup"><span data-stu-id="2dd79-403">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="2dd79-404">調整ファイルの課金の説明 (ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="2dd79-404">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="2dd79-405">この課金の意味</span><span class="sxs-lookup"><span data-stu-id="2dd79-405">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="2dd79-406">これらの ChargeTypes を請求書にマップする方法</span><span class="sxs-lookup"><span data-stu-id="2dd79-406">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong><span data-ttu-id="2dd79-407">当月のサービス利用料金</span><span class="sxs-lookup"><span data-stu-id="2dd79-407">Recurring Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="2dd79-408">Activation fee</span><span class="sxs-lookup"><span data-stu-id="2dd79-408">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-409">購入したサブスクリプションを顧客が使用したときに顧客に課金される金額</span><span class="sxs-lookup"><span data-stu-id="2dd79-409">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="2dd79-410">ライセンスベースのファイルから、<strong>Amount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="2dd79-410">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2dd79-411">取り消し料金</span><span class="sxs-lookup"><span data-stu-id="2dd79-411">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-412">関連付けられているシートが変更されたときに顧客に払い戻される日割り料金</span><span class="sxs-lookup"><span data-stu-id="2dd79-412">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2dd79-413">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="2dd79-413">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-414">サブスクリプションの定期的な課金</span><span class="sxs-lookup"><span data-stu-id="2dd79-414">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2dd79-415">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="2dd79-415">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-416">関連付けられているシートが変更されたときに顧客から評価される日割り料金</span><span class="sxs-lookup"><span data-stu-id="2dd79-416">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2dd79-417">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="2dd79-417">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-418">取り消し時のサービスの未使用部分に対する日割りの払戻し額</span><span class="sxs-lookup"><span data-stu-id="2dd79-418">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2dd79-419">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="2dd79-419">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-420">購入時の日割りの料金</span><span class="sxs-lookup"><span data-stu-id="2dd79-420">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2dd79-421">Purchase fee</span><span class="sxs-lookup"><span data-stu-id="2dd79-421">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-422">サブスクリプションの最初の課金</span><span class="sxs-lookup"><span data-stu-id="2dd79-422">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2dd79-423">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="2dd79-423">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-424">サブスクリプションの更新時の日割り料金</span><span class="sxs-lookup"><span data-stu-id="2dd79-424">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2dd79-425">Renew fee</span><span class="sxs-lookup"><span data-stu-id="2dd79-425">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-426">サブスクリプションの更新時の課金</span><span class="sxs-lookup"><span data-stu-id="2dd79-426">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="2dd79-427">その他の製品とサービス</span><span class="sxs-lookup"><span data-stu-id="2dd79-427">Other Products and Services</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="2dd79-428">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="2dd79-428">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-429">アクティブ化から課金期間の終了までの日割り料金</span><span class="sxs-lookup"><span data-stu-id="2dd79-429">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-430">ライセンスベースのファイルから、<strong>Amount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="2dd79-430">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="2dd79-431">利用料金</span><span class="sxs-lookup"><span data-stu-id="2dd79-431">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="2dd79-432">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="2dd79-432">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-433">現在の課金期間中に未払いの使用を取り消したときのアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="2dd79-433">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="2dd79-434">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="2dd79-434">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2dd79-435">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="2dd79-435">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-436">現在の課金期間のアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="2dd79-436">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="2dd79-437">調整額</span><span class="sxs-lookup"><span data-stu-id="2dd79-437">Credits &amp; Adjustments</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="2dd79-438">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="2dd79-438">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-439">税金を含む、行項目への一部または全部の払戻し</span><span class="sxs-lookup"><span data-stu-id="2dd79-439">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-440">ライセンスベースのファイルから、<strong>TotalForCustomer</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="2dd79-440">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="2dd79-441">使用量ベースのファイルから、<strong>PostTaxTotal</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="2dd79-441">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="2dd79-442">その他の割引</span><span class="sxs-lookup"><span data-stu-id="2dd79-442">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="2dd79-443">(使用量ベース)</span><span class="sxs-lookup"><span data-stu-id="2dd79-443">(usage-based)</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="2dd79-444">Activation discount</span><span class="sxs-lookup"><span data-stu-id="2dd79-444">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-445">サブスクリプションがアクティブ化されたときに適用される割引</span><span class="sxs-lookup"><span data-stu-id="2dd79-445">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="2dd79-446">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="2dd79-446">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2dd79-447">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="2dd79-447">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-448">定期的な課金に適用される割引</span><span class="sxs-lookup"><span data-stu-id="2dd79-448">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="2dd79-449">Renew discount</span><span class="sxs-lookup"><span data-stu-id="2dd79-449">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-450">サブスクリプションの更新時に適用される割引</span><span class="sxs-lookup"><span data-stu-id="2dd79-450">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="2dd79-451">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="2dd79-451">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-452">割引が取り消されたときに適用される料金</span><span class="sxs-lookup"><span data-stu-id="2dd79-452">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="2dd79-453">その他の割引</span><span class="sxs-lookup"><span data-stu-id="2dd79-453">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="2dd79-454">(ライセンスベース)</span><span class="sxs-lookup"><span data-stu-id="2dd79-454">(license-based)</span></span></em></p>
</td>
<td>
<p><em><span data-ttu-id="2dd79-455">複数の種類の料金に適用される場合がある</span><span class="sxs-lookup"><span data-stu-id="2dd79-455">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="2dd79-456">ライセンスベースのファイルから、<strong>TotalOtherDiscount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="2dd79-456">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="2dd79-457"><strong>税</strong>&nbsp;または&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="2dd79-457"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="2dd79-458">複数の種類の料金に適用される場合がある</span><span class="sxs-lookup"><span data-stu-id="2dd79-458">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="2dd79-459">例外: "Offset a line item" には既に税が含まれます。</span><span class="sxs-lookup"><span data-stu-id="2dd79-459">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="2dd79-460">前の「調整額」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2dd79-460">See Credits &amp; Adjustments, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="2dd79-461">税または付加価値税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="2dd79-461">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="2dd79-462">ライセンスベースのファイルから、<strong>Tax</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="2dd79-462">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="2dd79-463">使用量ベースのファイルから、<strong>TaxAmount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="2dd79-463">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
