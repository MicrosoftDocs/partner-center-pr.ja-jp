---
title: 調整ファイル (パートナー センターの 21 vianet が運営) を使用して、
ms.topic: article
ms.date: 10/29/2018
description: 請求サイクルの各料金の詳しい行項目ビューについては、パートナー センターのダッシュボードから調整ファイルをダウンロードします。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.openlocfilehash: 30e3b7a7933678c4af079bb86aa1439559387f2b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132082"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="eaa54-103">調整ファイルを使う</span><span class="sxs-lookup"><span data-stu-id="eaa54-103">Use the reconciliation files</span></span>

<span data-ttu-id="eaa54-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="eaa54-104">**Applies to**</span></span>

-   <span data-ttu-id="eaa54-105">21Vianet が運営するパートナー センター</span><span class="sxs-lookup"><span data-stu-id="eaa54-105">Partner Center operated by 21Vianet</span></span>


<span data-ttu-id="eaa54-106">請求サイクルの各料金の詳しい行項目ビューについては、パートナー センターのダッシュボードから調整ファイルをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="eaa54-106">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="eaa54-107">詳細には、各顧客のサブスクリプションの料金や、詳細なイベント (期間途中でのサブスクリプションへのシートの追加など) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-107">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="eaa54-108">パートナーによって明細化します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-108">Itemize by partner</span></span>


<span data-ttu-id="eaa54-109">インダイレクト モデルのパートナーは、ライセンス ベースの調整ファイルと使用量ベースの調整ファイルの両方で、これらの追加フィールドを使用してリセラーごとに明細を記載できます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-109">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="eaa54-110">MPN ID</span><span class="sxs-lookup"><span data-stu-id="eaa54-110">MPN ID</span></span></th>
<th><span data-ttu-id="eaa54-111">説明</span><span class="sxs-lookup"><span data-stu-id="eaa54-111">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="eaa54-112">MPN ID</span><span class="sxs-lookup"><span data-stu-id="eaa54-112">MPN ID</span></span></td>
<td><p><span data-ttu-id="eaa54-113">CSP パートナー (直接または間接) の Microsoft Partner Network (MPN) IDです。</span><span class="sxs-lookup"><span data-stu-id="eaa54-113">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-114">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="eaa54-114">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="eaa54-115">インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-115">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="eaa54-116">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="eaa54-116">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="eaa54-117">これは、パートナー センターで特定のサブスクリプションについて示されるリセラー ID に対応します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-117">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="eaa54-118">リセラーを表示または更新するには、パートナー センター メニューで <strong>[顧客]</strong> を選び、一覧から顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-118">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="eaa54-119">顧客メニューの <strong>[サブスクリプション]</strong> を選び、一覧からサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-119">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="eaa54-120"><strong>[更新]</strong> を選んで、<strong>[再販業者 (MPN ID)]</strong> を変更します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-120">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="eaa54-121">CSP パートナーがお客様に直接サブスクリプションを販売した場合、パートナーの MPN ID が MPN ID とリセラーの MPN ID として 2 か所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-121">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="eaa54-122">CSP パートナーのリセラーに MPN ID がない場合は、代わりに CSP パートナーの MPN ID がこの値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-122">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="eaa54-123">CSP パートナーがリセラー ID を削除した場合、この値は -1 に設定されます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-123">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="eaa54-124">ライセンス ベースのファイル フィールド</span><span class="sxs-lookup"><span data-stu-id="eaa54-124">License-based file fields</span></span>


<span data-ttu-id="eaa54-125">顧客の注文に対する料金を調整するには、調整ファイルの Syndication\_Partner\_Subscription\_Number とパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-125">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="eaa54-126"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-126"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="eaa54-127"><strong>説明</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-127"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="eaa54-128"><strong>サンプル値</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-128"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-129">PartnerId</span><span class="sxs-lookup"><span data-stu-id="eaa54-129">PartnerId</span></span></td>
<td><p><span data-ttu-id="eaa54-130">特定の課金エンティティの一意の識別子 (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="eaa54-130">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="eaa54-131">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="eaa54-131">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="eaa54-132">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="eaa54-132">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="eaa54-133">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="eaa54-133">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-134">CustomerID</span><span class="sxs-lookup"><span data-stu-id="eaa54-134">CustomerID</span></span></td>
<td><p><span data-ttu-id="eaa54-135">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="eaa54-135">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="eaa54-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="eaa54-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-137">OrderID</span><span class="sxs-lookup"><span data-stu-id="eaa54-137">OrderID</span></span></td>
<td><p><span data-ttu-id="eaa54-138">Microsoft 請求プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="eaa54-138">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="eaa54-139">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="eaa54-139">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="eaa54-140">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="eaa54-140">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-141">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="eaa54-141">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="eaa54-142">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="eaa54-142">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="eaa54-143">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="eaa54-143">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="eaa54-144">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="eaa54-144">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="eaa54-145">「Syndication_Partner_Subscription_Number」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="eaa54-145">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="eaa54-146">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="eaa54-146">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-147">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="eaa54-147">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="eaa54-148">サブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="eaa54-148">Unique identifier for subscriptions.</span></span> <span data-ttu-id="eaa54-149">お客様は同じプランで複数のサブスクリプションを持つことができるため、これは調整ファイルの分析で重要です。</span><span class="sxs-lookup"><span data-stu-id="eaa54-149">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="eaa54-150">このフィールドは、パートナー管理コンソールのサブスクリプション ID にマップされます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-150">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="eaa54-151">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="eaa54-151">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-152">OfferID</span><span class="sxs-lookup"><span data-stu-id="eaa54-152">OfferID</span></span></td>
<td><p><span data-ttu-id="eaa54-153">一意のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="eaa54-153">Unique offer ID.</span></span> <span data-ttu-id="eaa54-154">価格表に従った標準のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="eaa54-154">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="eaa54-155"><b>注意</b>:この値では、価格表からプラン ID が一致しません。</span><span class="sxs-lookup"><span data-stu-id="eaa54-155"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="eaa54-156">以下の DurableOfferID を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eaa54-156">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="eaa54-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="eaa54-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-158">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="eaa54-158">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="eaa54-159">価格表で定義されている一意の継続的なプラン ID。</span><span class="sxs-lookup"><span data-stu-id="eaa54-159">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="eaa54-160"><b>注意</b>:この値は、価格表からプラン ID と一致します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-160"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="eaa54-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="eaa54-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-162">OfferName</span><span class="sxs-lookup"><span data-stu-id="eaa54-162">OfferName</span></span></td>
<td><p><span data-ttu-id="eaa54-163">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="eaa54-163">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="eaa54-164">Microsoft Office 365 (プラン E3)</span><span class="sxs-lookup"><span data-stu-id="eaa54-164">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-165">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="eaa54-165">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="eaa54-166">サブスクリプションの開始日。注文が送信された日に設定されます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-166">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="eaa54-167">サブスクリプションの開始日を終了日と共に確認することにより、顧客がサブスクリプションの最初の 1 年以内であるか、サブスクリプションが次の 1 年間更新されたかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-167">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="eaa54-168">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="eaa54-168">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="eaa54-169">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="eaa54-169">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-170">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="eaa54-170">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="eaa54-171">サブスクリプションの終了日:12 か月 + x 日間 (パートナーの請求日の連携) を開始日より後または更新日から 12 か月です。</span><span class="sxs-lookup"><span data-stu-id="eaa54-171">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="eaa54-172">更新時に、価格は最新の価格表に更新されます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-172">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="eaa54-173">自動更新の前に、顧客とのやり取りが必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="eaa54-173">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="eaa54-174">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="eaa54-174">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="eaa54-175">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="eaa54-175">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-176">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="eaa54-176">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="eaa54-177">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="eaa54-177">Start day of the charges.</span></span></p>
<p><span data-ttu-id="eaa54-178">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-178">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="eaa54-179">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="eaa54-179">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="eaa54-180">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="eaa54-180">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-181">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="eaa54-181">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="eaa54-182">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="eaa54-182">End day of the charges.</span></span></p>
<p><span data-ttu-id="eaa54-183">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-183">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="eaa54-184">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="eaa54-184">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="eaa54-185">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="eaa54-185">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-186">ChargeType</span><span class="sxs-lookup"><span data-stu-id="eaa54-186">ChargeType</span></span></td>
<td><p><span data-ttu-id="eaa54-187">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="eaa54-187">The type of charge or adjustment.</span></span> <span data-ttu-id="eaa54-188">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eaa54-188">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="eaa54-189">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eaa54-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-190">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="eaa54-190">UnitPrice</span></span></td>
<td><p><span data-ttu-id="eaa54-191">シートごとの価格。</span><span class="sxs-lookup"><span data-stu-id="eaa54-191">Price per seat.</span></span> <span data-ttu-id="eaa54-192">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-192">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="eaa54-193">6.82</span><span class="sxs-lookup"><span data-stu-id="eaa54-193">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-194">Quantity</span><span class="sxs-lookup"><span data-stu-id="eaa54-194">Quantity</span></span></td>
<td><p><span data-ttu-id="eaa54-195">シート数。</span><span class="sxs-lookup"><span data-stu-id="eaa54-195">Number of seats.</span></span> <span data-ttu-id="eaa54-196">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-196">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="eaa54-197">2</span><span class="sxs-lookup"><span data-stu-id="eaa54-197">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-198">金額</span><span class="sxs-lookup"><span data-stu-id="eaa54-198">Amount</span></span></td>
<td><p><span data-ttu-id="eaa54-199">数量に対する合計価格。</span><span class="sxs-lookup"><span data-stu-id="eaa54-199">Total of price for quantity.</span></span> <span data-ttu-id="eaa54-200">金額の計算が、この顧客用の計算方法に一致することを確認するために役立ちます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-200">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="eaa54-201">13.32</span><span class="sxs-lookup"><span data-stu-id="eaa54-201">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-202">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="eaa54-202">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="eaa54-203">これらの料金に適用される割引額。</span><span class="sxs-lookup"><span data-stu-id="eaa54-203">Amount of discount applied to these charges.</span></span> <span data-ttu-id="eaa54-204">インセンティブの対象となる IUR または新しいサブスクリプションの場合も、この列に割引額が含まれます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-204">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="eaa54-205">2.32</span><span class="sxs-lookup"><span data-stu-id="eaa54-205">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-206">Subtotal</span><span class="sxs-lookup"><span data-stu-id="eaa54-206">Subtotal</span></span></td>
<td><p><span data-ttu-id="eaa54-207">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="eaa54-207">Total before tax.</span></span> <span data-ttu-id="eaa54-208">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-208">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="eaa54-209">11</span><span class="sxs-lookup"><span data-stu-id="eaa54-209">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-210">Tax</span><span class="sxs-lookup"><span data-stu-id="eaa54-210">Tax</span></span></td>
<td><p><span data-ttu-id="eaa54-211">市場の税関連の規則や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="eaa54-211">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="eaa54-212">0</span><span class="sxs-lookup"><span data-stu-id="eaa54-212">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-213">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="eaa54-213">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="eaa54-214">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="eaa54-214">Total after tax.</span></span> <span data-ttu-id="eaa54-215">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-215">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="eaa54-216">11</span><span class="sxs-lookup"><span data-stu-id="eaa54-216">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-217">通貨</span><span class="sxs-lookup"><span data-stu-id="eaa54-217">Currency</span></span></td>
<td><p><span data-ttu-id="eaa54-218">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="eaa54-218">Currency type.</span></span> <span data-ttu-id="eaa54-219">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="eaa54-219">Each billing entity has only one currency.</span></span> <span data-ttu-id="eaa54-220">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-220">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="eaa54-221">CNY</span><span class="sxs-lookup"><span data-stu-id="eaa54-221">CNY</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-222">CustomerName</span><span class="sxs-lookup"><span data-stu-id="eaa54-222">CustomerName</span></span></td>
<td><p><span data-ttu-id="eaa54-223">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="eaa54-223">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="eaa54-224">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="eaa54-224">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="eaa54-225">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="eaa54-225">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-226">MPNID</span><span class="sxs-lookup"><span data-stu-id="eaa54-226">MPNID</span></span></td>
<td><p><span data-ttu-id="eaa54-227">CSP パートナーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="eaa54-227">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="eaa54-228">4390934</span><span class="sxs-lookup"><span data-stu-id="eaa54-228">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-229">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="eaa54-229">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="eaa54-230">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="eaa54-230">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="eaa54-231">「[パートナーごとに明細を示す](#itemizebypartner)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="eaa54-231">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="eaa54-232">4390934</span><span class="sxs-lookup"><span data-stu-id="eaa54-232">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-233">DomainName</span><span class="sxs-lookup"><span data-stu-id="eaa54-233">DomainName</span></span></td>
<td><p><span data-ttu-id="eaa54-234">顧客のドメイン名。顧客を特定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-234">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="eaa54-235">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="eaa54-235">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-236">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="eaa54-236">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="eaa54-237">サブスクリプションのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="eaa54-237">Subscription nickname.</span></span> <span data-ttu-id="eaa54-238">ニックネームが指定されていない場合、パートナー センターでは OfferName を使用します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-238">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="eaa54-239">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="eaa54-239">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-240">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="eaa54-240">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="eaa54-241">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="eaa54-241">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="eaa54-242">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="eaa54-242">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="eaa54-243">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span><span class="sxs-lookup"><span data-stu-id="eaa54-243">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="eaa54-244">ファイルの使用法に基づくフィールド</span><span class="sxs-lookup"><span data-stu-id="eaa54-244">Usage-based file fields</span></span>


<span data-ttu-id="eaa54-245">顧客の使用量に対する料金を調整するには、調整ファイルの ResellerID/ResellerName/ResellerBillableAccount、顧客名、およびパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-245">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="eaa54-246">次のフィールドで、どのサービスが使用されるか、およびレートについて説明します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-246">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="eaa54-247"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-247"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="eaa54-248"><strong>説明</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-248"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="eaa54-249"><strong>サンプル値</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-249"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-250">PartnerID</span><span class="sxs-lookup"><span data-stu-id="eaa54-250">PartnerID</span></span></td>
<td><p><span data-ttu-id="eaa54-251">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="eaa54-251">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="eaa54-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="eaa54-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-253">PartnerName</span><span class="sxs-lookup"><span data-stu-id="eaa54-253">PartnerName</span></span></td>
<td><p><span data-ttu-id="eaa54-254">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="eaa54-254">Partner Name.</span></span></p></td>
<td><span data-ttu-id="eaa54-255">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="eaa54-255">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-256">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="eaa54-256">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="eaa54-257">パートナーのアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="eaa54-257">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="eaa54-258">1010578050</span><span class="sxs-lookup"><span data-stu-id="eaa54-258">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-259">CustomerName</span><span class="sxs-lookup"><span data-stu-id="eaa54-259">CustomerName</span></span></td>
<td><p><span data-ttu-id="eaa54-260">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="eaa54-260">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="eaa54-261">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="eaa54-261">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="eaa54-262">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="eaa54-262">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-263">MPNID</span><span class="sxs-lookup"><span data-stu-id="eaa54-263">MPNID</span></span></td>
<td><p><span data-ttu-id="eaa54-264">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="eaa54-264">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="eaa54-265">4390934</span><span class="sxs-lookup"><span data-stu-id="eaa54-265">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-266">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="eaa54-266">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="eaa54-267">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="eaa54-267">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="eaa54-268">「[パートナーごとに明細を示す](#itemizebypartner)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="eaa54-268">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="eaa54-269">4390934</span><span class="sxs-lookup"><span data-stu-id="eaa54-269">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-270">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="eaa54-270">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="eaa54-271">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="eaa54-271">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="eaa54-272">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="eaa54-272">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-273">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="eaa54-273">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="eaa54-274">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="eaa54-274">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="eaa54-275">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="eaa54-275">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="eaa54-276">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="eaa54-276">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-277">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="eaa54-277">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="eaa54-278">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="eaa54-278">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="eaa54-279">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="eaa54-279">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="eaa54-280">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="eaa54-280">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-281">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="eaa54-281">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="eaa54-282">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="eaa54-282">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="eaa54-283">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="eaa54-283">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="eaa54-284">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="eaa54-284">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="eaa54-285">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="eaa54-285">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-286">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="eaa54-286">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="eaa54-287">サービス プランのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="eaa54-287">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="eaa54-288">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="eaa54-288">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-289">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="eaa54-289">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="eaa54-290">サービス プランの基幹業務</span><span class="sxs-lookup"><span data-stu-id="eaa54-290">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="eaa54-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="eaa54-291">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-292">OrderID</span><span class="sxs-lookup"><span data-stu-id="eaa54-292">OrderID</span></span></td>
<td><p><span data-ttu-id="eaa54-293">Microsoft 請求プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="eaa54-293">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="eaa54-294">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="eaa54-294">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="eaa54-295">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="eaa54-295">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-296">ServiceName</span><span class="sxs-lookup"><span data-stu-id="eaa54-296">ServiceName</span></span></td>
<td><p><span data-ttu-id="eaa54-297">対象の Azure サービスの名前。</span><span class="sxs-lookup"><span data-stu-id="eaa54-297">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="eaa54-298">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="eaa54-298">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-299">ServiceType</span><span class="sxs-lookup"><span data-stu-id="eaa54-299">ServiceType</span></span></td>
<td><p><span data-ttu-id="eaa54-300">Windows Azure サービスの特定の種類。</span><span class="sxs-lookup"><span data-stu-id="eaa54-300">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="eaa54-301">Service Bus – Individual or Pack</span><span class="sxs-lookup"><span data-stu-id="eaa54-301">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="eaa54-302">SQL Azure database – Business or Web Edition</span><span class="sxs-lookup"><span data-stu-id="eaa54-302">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-303">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="eaa54-303">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="eaa54-304">すべてのサービス データおよび価格設定構造の特定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="eaa54-304">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="eaa54-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="eaa54-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-306">リソース名</span><span class="sxs-lookup"><span data-stu-id="eaa54-306">Resource Name</span></span></td>
<td><p><span data-ttu-id="eaa54-307">Azure リソースの名前。</span><span class="sxs-lookup"><span data-stu-id="eaa54-307">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="eaa54-308">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="eaa54-308">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="eaa54-309">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="eaa54-309">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-310">Region</span><span class="sxs-lookup"><span data-stu-id="eaa54-310">Region</span></span></td>
<td><p><span data-ttu-id="eaa54-311">使用量が適用される地域。</span><span class="sxs-lookup"><span data-stu-id="eaa54-311">The region the usage applies to.</span></span> <span data-ttu-id="eaa54-312">料金は地域によって異なるため、主にデータ転送に料金を割り当てるために使われます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-312">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="eaa54-313">Asia Pacific、Europe、Latin America、North America</span><span class="sxs-lookup"><span data-stu-id="eaa54-313">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-314">SKU</span><span class="sxs-lookup"><span data-stu-id="eaa54-314">SKU</span></span></td>
<td><p><span data-ttu-id="eaa54-315">プランについての MSFT の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="eaa54-315">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="eaa54-316">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="eaa54-316">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="eaa54-317">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="eaa54-317">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="eaa54-318">特定の課金期間のサービスまたはリソースに対してさまざまなレートの明細を設定するための ID と数量。</span><span class="sxs-lookup"><span data-stu-id="eaa54-318">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="eaa54-319">Azure の階層化されたレーティングの場合は、一定数量の課金可能単位までは 1 つのレートがあり、その後に別のレートがあることがあります。</span><span class="sxs-lookup"><span data-stu-id="eaa54-319">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="eaa54-320">1</span><span class="sxs-lookup"><span data-stu-id="eaa54-320">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-321">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="eaa54-321">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="eaa54-322">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="eaa54-322">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="eaa54-323">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-323">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="eaa54-324">11</span><span class="sxs-lookup"><span data-stu-id="eaa54-324">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-325">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="eaa54-325">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="eaa54-326">単位数はプランの一部として含まれます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-326">Units included as part of the offer.</span></span> <span data-ttu-id="eaa54-327">通常、CSP には含まれません。</span><span class="sxs-lookup"><span data-stu-id="eaa54-327">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="eaa54-328">0</span><span class="sxs-lookup"><span data-stu-id="eaa54-328">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="eaa54-329">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="eaa54-329">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="eaa54-330">単位数はプランの一部として含まれず、パートナーが支払う必要があります。</span><span class="sxs-lookup"><span data-stu-id="eaa54-330">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="eaa54-331">ConsumedQuantity - IncludedQuantity と同じです。</span><span class="sxs-lookup"><span data-stu-id="eaa54-331">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="eaa54-332">11</span><span class="sxs-lookup"><span data-stu-id="eaa54-332">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-333">ListPrice</span><span class="sxs-lookup"><span data-stu-id="eaa54-333">ListPrice</span></span></td>
<td><p><span data-ttu-id="eaa54-334">サブスクリプションの開始日に有効な価格を提供します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-334">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="eaa54-335">$0.0808</span><span class="sxs-lookup"><span data-stu-id="eaa54-335">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-336">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="eaa54-336">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="eaa54-337">ListPrist と OverageQuantity を掛けて、最も近いセントに丸めます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-337">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="eaa54-338">$0.085</span><span class="sxs-lookup"><span data-stu-id="eaa54-338">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-339">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="eaa54-339">TaxAmount</span></span></td>
<td><p><span data-ttu-id="eaa54-340">市場の税関連の規則や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="eaa54-340">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="eaa54-341">$0.08</span><span class="sxs-lookup"><span data-stu-id="eaa54-341">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-342">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="eaa54-342">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="eaa54-343">税が適用されるときの税引き後の合計額。</span><span class="sxs-lookup"><span data-stu-id="eaa54-343">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="eaa54-344">$0.93</span><span class="sxs-lookup"><span data-stu-id="eaa54-344">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-345">通貨</span><span class="sxs-lookup"><span data-stu-id="eaa54-345">Currency</span></span></td>
<td><p><span data-ttu-id="eaa54-346">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="eaa54-346">Currency type.</span></span> <span data-ttu-id="eaa54-347">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="eaa54-347">Each billing entity has only one currency.</span></span> <span data-ttu-id="eaa54-348">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-348">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="eaa54-349">CNY</span><span class="sxs-lookup"><span data-stu-id="eaa54-349">CNY</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-350">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="eaa54-350">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="eaa54-351">単位あたりの税込み価格。</span><span class="sxs-lookup"><span data-stu-id="eaa54-351">Pretax price per unit.</span></span> <span data-ttu-id="eaa54-352">PretaxCharges / OverageQuantity と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-352">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="eaa54-353">$0.08</span><span class="sxs-lookup"><span data-stu-id="eaa54-353">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-354">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="eaa54-354">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="eaa54-355">単位あたりの税引き後の価格。</span><span class="sxs-lookup"><span data-stu-id="eaa54-355">Post tax price per unit.</span></span> <span data-ttu-id="eaa54-356">PostTaxTotal / OverageQuantity、または PretaxEffectiveRate + 単位額あたりの税率と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-356">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="eaa54-357">$0.08</span><span class="sxs-lookup"><span data-stu-id="eaa54-357">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-358">ChargeType</span><span class="sxs-lookup"><span data-stu-id="eaa54-358">ChargeType</span></span></td>
<td><p><span data-ttu-id="eaa54-359">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="eaa54-359">The type of charge or adjustment.</span></span> <span data-ttu-id="eaa54-360">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eaa54-360">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="eaa54-361">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eaa54-361">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-362">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="eaa54-362">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="eaa54-363">MSFT 課金プラットフォームの一意のアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="eaa54-363">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="eaa54-364">1280018095</span><span class="sxs-lookup"><span data-stu-id="eaa54-364">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-365">UsageDate</span><span class="sxs-lookup"><span data-stu-id="eaa54-365">UsageDate</span></span></td>
<td><p><span data-ttu-id="eaa54-366">サービスの展開の日付。</span><span class="sxs-lookup"><span data-stu-id="eaa54-366">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="eaa54-367">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="eaa54-367">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-368">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="eaa54-368">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="eaa54-369">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-369">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="eaa54-370">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="eaa54-370">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-371">MeteredService</span><span class="sxs-lookup"><span data-stu-id="eaa54-371">MeteredService</span></span></td>
<td><p><span data-ttu-id="eaa54-372">この列は、[Service Name] 列で特に識別されない可能性のある、個別の Microsoft Azure サービスの追跡に利用されます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-372">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="eaa54-373">たとえば、データ転送は、[Service Name] 列で &quot;Microsoft Azure - All Services&quot; と報告されます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-373">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="eaa54-374">この [MeteredService] 列は、利用に関連する特定のサービスを示します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-374">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="eaa54-375">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="eaa54-375">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-376">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="eaa54-376">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="eaa54-377">個々の Microsoft Azure サービスの内容を、MeteredService フィールドで提供されるレベルよりも明確にする小見出し。</span><span class="sxs-lookup"><span data-stu-id="eaa54-377">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="eaa54-378">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="eaa54-378">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-379">Project</span><span class="sxs-lookup"><span data-stu-id="eaa54-379">Project</span></span></td>
<td><p><span data-ttu-id="eaa54-380">サービス インスタンスの顧客定義の名前</span><span class="sxs-lookup"><span data-stu-id="eaa54-380">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="eaa54-381">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="eaa54-381">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-382">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="eaa54-382">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="eaa54-383">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="eaa54-383">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="eaa54-384">例: 1 か月 30 日間の中に、個別にプロビジョニングされた接続がある場合、Service Info 1 は "1.000000 Connections / 30 days" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="eaa54-384">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="eaa54-385">Service Bus 接続のプロビジョニングが 25 パックする必要があるし、その日に 1 つを利用して、その日、毎日の使用量明細を示す"25 接続/30 Days-Used:1.000000”.</span><span class="sxs-lookup"><span data-stu-id="eaa54-385">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="eaa54-386">CustomerID</span><span class="sxs-lookup"><span data-stu-id="eaa54-386">CustomerID</span></span></td>
<td><p><span data-ttu-id="eaa54-387">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="eaa54-387">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="eaa54-388">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="eaa54-388">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="eaa54-389">DomainName</span><span class="sxs-lookup"><span data-stu-id="eaa54-389">DomainName</span></span></td>
<td><p><span data-ttu-id="eaa54-390">顧客のドメイン名。顧客を特定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-390">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="eaa54-391">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="eaa54-391">example.onmicrosoft.com</span></span></td></tr>
</tbody>
</table>



## <a href="" id="charge_types"></a><span data-ttu-id="eaa54-392">請求書と調整ファイルの間の料金のマッピング</span><span class="sxs-lookup"><span data-stu-id="eaa54-392">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="eaa54-393">請求書は料金の概要を示し、調整ファイルは、課金の種類を含め、行項目のトランザクションの詳細な内訳を示します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-393">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="eaa54-394">請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルター オプションを使用して、調整ファイルの課金の種類でフィルター処理し、請求書の課金を調整ファイルの一連の課金の内訳にマップします。</span><span class="sxs-lookup"><span data-stu-id="eaa54-394">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="eaa54-395">次の表に、請求書のセクションと、調整ファイルに表示される関連付けられた課金の種類とのマッピングを示します。</span><span class="sxs-lookup"><span data-stu-id="eaa54-395">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="eaa54-396"><strong>請求書の料金の説明</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-396"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-397"><strong>調整ファイルの料金の説明 (ChargeType 列)</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-397"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-398"><strong>この料金は何ですか。</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-398"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-399"><strong>請求書にこれら ChargeTypes をマップする方法</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-399"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><span data-ttu-id="eaa54-400"><strong>利用料金</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-400"><strong>Recurring Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-401">Cancel instance prorate</span><span class="sxs-lookup"><span data-stu-id="eaa54-401">Cancel instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-402">関連付けられているシートが変更されたときに顧客に払い戻される日割り料金</span><span class="sxs-lookup"><span data-stu-id="eaa54-402">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="eaa54-403">ライセンスベースのファイルから、<strong>Amount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="eaa54-403">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="eaa54-404">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="eaa54-404">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-405">サブスクリプションの定期的な課金</span><span class="sxs-lookup"><span data-stu-id="eaa54-405">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="eaa54-406">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="eaa54-406">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-407">関連付けられているシートが変更されたときに顧客から評価される日割り料金</span><span class="sxs-lookup"><span data-stu-id="eaa54-407">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="eaa54-408">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="eaa54-408">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-409">取り消し時のサービスの未使用部分に対する日割りの払戻し額</span><span class="sxs-lookup"><span data-stu-id="eaa54-409">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="eaa54-410">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="eaa54-410">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-411">購入時の日割りの料金</span><span class="sxs-lookup"><span data-stu-id="eaa54-411">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="eaa54-412">Purchase fee</span><span class="sxs-lookup"><span data-stu-id="eaa54-412">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-413">サブスクリプションの最初の課金</span><span class="sxs-lookup"><span data-stu-id="eaa54-413">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="eaa54-414">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="eaa54-414">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-415">サブスクリプションの更新時の日割り料金</span><span class="sxs-lookup"><span data-stu-id="eaa54-415">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="eaa54-416">Renew fee</span><span class="sxs-lookup"><span data-stu-id="eaa54-416">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-417">サブスクリプションの更新時の課金</span><span class="sxs-lookup"><span data-stu-id="eaa54-417">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="eaa54-418"><strong>その他の製品およびサービス</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-418"><strong>Other Products and Services</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-419">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="eaa54-419">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-420">アクティブ化から課金期間の終了までの日割り料金</span><span class="sxs-lookup"><span data-stu-id="eaa54-420">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-421">ライセンスベースのファイルから、<strong>Amount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="eaa54-421">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="eaa54-422"><strong>利用料金</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-422"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-423">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="eaa54-423">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-424">現在の課金期間中に未払いの使用を取り消したときのアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="eaa54-424">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="eaa54-425">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="eaa54-425">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="eaa54-426">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="eaa54-426">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-427">現在の課金期間のアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="eaa54-427">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="eaa54-428"><strong>クレジット&amp;の調整</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-428"><strong>Credits &amp; Adjustments</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-429">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="eaa54-429">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-430">税金を含む、行項目への一部または全部の払戻し</span><span class="sxs-lookup"><span data-stu-id="eaa54-430">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-431">ライセンスベースのファイルから、<strong>TotalForCustomer</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="eaa54-431">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="eaa54-432">使用量ベースのファイルから、<strong>PostTaxTotal</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="eaa54-432">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><span data-ttu-id="eaa54-433"><strong>他の割引</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-433"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="eaa54-434">
<em>(使用法に基づく)</em></span><span class="sxs-lookup"><span data-stu-id="eaa54-434">
<em>(usage-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-435">Activation discount</span><span class="sxs-lookup"><span data-stu-id="eaa54-435">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-436">サブスクリプションがアクティブ化されたときに適用される割引</span><span class="sxs-lookup"><span data-stu-id="eaa54-436">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="eaa54-437">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="eaa54-437">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="eaa54-438">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="eaa54-438">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-439">定期的な課金に適用される割引</span><span class="sxs-lookup"><span data-stu-id="eaa54-439">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="eaa54-440">Renew discount</span><span class="sxs-lookup"><span data-stu-id="eaa54-440">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-441">サブスクリプションの更新時に適用される割引</span><span class="sxs-lookup"><span data-stu-id="eaa54-441">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="eaa54-442">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="eaa54-442">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-443">割引が取り消されたときに適用される料金</span><span class="sxs-lookup"><span data-stu-id="eaa54-443">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="eaa54-444"><strong>他の割引</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-444"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="eaa54-445">
<em>(ライセンス ベース)</em></span><span class="sxs-lookup"><span data-stu-id="eaa54-445">
<em>(license-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-446"><em>複数の料金の種類に適用できます。</em></span><span class="sxs-lookup"><span data-stu-id="eaa54-446"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="eaa54-447">ライセンスベースのファイルから、<strong>TotalOtherDiscount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="eaa54-447">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="eaa54-448"><strong>税</strong>&nbsp;または&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="eaa54-448"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-449"><em>複数の料金の種類に適用できます。</em></span><span class="sxs-lookup"><span data-stu-id="eaa54-449"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="eaa54-450"><em>例外:「行項目を相殺」では、税金既に含まれています。クレジットを参照してください。&amp;調整上、します。</em></span><span class="sxs-lookup"><span data-stu-id="eaa54-450"><em>Exception: "Offset a line item" already includes taxes. See Credits &amp; Adjustments, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-451">税または付加価値税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="eaa54-451">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="eaa54-452">ライセンスベースのファイルから、<strong>Tax</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="eaa54-452">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="eaa54-453">使用量ベースのファイルから、<strong>TaxAmount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="eaa54-453">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
