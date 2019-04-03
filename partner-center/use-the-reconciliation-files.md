---
title: 調整ファイルの使用 | パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: 各料金が請求サイクルでの行項目の詳細なビューでは、パートナー センターから、調整ファイルをダウンロードします。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 9997b01c76dacb736baa33f458def0b820753f1d
ms.sourcegitcommit: 9a2bda49446030e60251c9c913259472ff2eed9a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "57682510"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="1b89b-103">調整ファイルを使う</span><span class="sxs-lookup"><span data-stu-id="1b89b-103">Use the reconciliation files</span></span>

<span data-ttu-id="1b89b-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="1b89b-104">**Applies to**</span></span>

-  <span data-ttu-id="1b89b-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="1b89b-105">Partner Center</span></span>
-  <span data-ttu-id="1b89b-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="1b89b-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="1b89b-107">各料金が請求サイクルでの行項目の詳細なビューでは、パートナー センターから、調整ファイルをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="1b89b-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="1b89b-108">詳細には、各顧客のサブスクリプションの料金や、詳細なイベント (期間途中でのサブスクリプションへのシートの追加など) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="1b89b-109">パートナーによって明細化します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-109">Itemize by partner</span></span>


<span data-ttu-id="1b89b-110">インダイレクト モデルのパートナーは、ライセンス ベースの調整ファイルと使用量ベースの調整ファイルの両方で、これらの追加フィールドを使用してリセラーごとに明細を記載できます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="1b89b-111">MPN ID</span><span class="sxs-lookup"><span data-stu-id="1b89b-111">MPN ID</span></span></th>
<th><span data-ttu-id="1b89b-112">説明</span><span class="sxs-lookup"><span data-stu-id="1b89b-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="1b89b-113">MPN ID</span><span class="sxs-lookup"><span data-stu-id="1b89b-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="1b89b-114">CSP パートナー (直接または間接) の Microsoft Partner Network (MPN) IDです。</span><span class="sxs-lookup"><span data-stu-id="1b89b-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-115">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="1b89b-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="1b89b-116">インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="1b89b-117">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="1b89b-118">これは、パートナー センターで特定のサブスクリプションについて示されるリセラー ID に対応します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="1b89b-119">などの表示または更新、再販業者、パートナー センターのメニューから選択<strong>顧客</strong>、一覧から顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="1b89b-120">顧客メニューの <strong>[サブスクリプション]</strong> を選び、一覧からサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="1b89b-121"><strong>[更新]</strong> を選んで、<strong>[再販業者 (MPN ID)]</strong> を変更します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="1b89b-122">CSP パートナーがお客様に直接サブスクリプションを販売した場合、パートナーの MPN ID が MPN ID とリセラーの MPN ID として 2 か所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="1b89b-123">CSP パートナーのリセラーに MPN ID がない場合は、代わりに CSP パートナーの MPN ID がこの値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="1b89b-124">CSP パートナーがリセラー ID を削除した場合、この値は -1 に設定されます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="1b89b-125">ライセンス ベースのファイル フィールド</span><span class="sxs-lookup"><span data-stu-id="1b89b-125">License-based file fields</span></span>


<span data-ttu-id="1b89b-126">顧客の注文に対する料金を調整するには、調整ファイルの Syndication\_Partner\_Subscription\_Number とパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="1b89b-127"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-127"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="1b89b-128"><strong>[説明]</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-128"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="1b89b-129"><strong>サンプル値</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-129"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="1b89b-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="1b89b-131">特定の課金エンティティの一意の識別子 (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="1b89b-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="1b89b-132">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="1b89b-133">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="1b89b-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="1b89b-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="1b89b-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="1b89b-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="1b89b-136">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="1b89b-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="1b89b-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="1b89b-138">OrderID</span></span></td>
<td><p><span data-ttu-id="1b89b-139">Microsoft 請求プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1b89b-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="1b89b-140">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="1b89b-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="1b89b-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="1b89b-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="1b89b-143">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1b89b-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="1b89b-144">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="1b89b-145">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="1b89b-146">「Syndication_Partner_Subscription_Number」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1b89b-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="1b89b-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="1b89b-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="1b89b-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="1b89b-149">サブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1b89b-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="1b89b-150">お客様は同じプランで複数のサブスクリプションを持つことができるため、これは調整ファイルの分析で重要です。</span><span class="sxs-lookup"><span data-stu-id="1b89b-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="1b89b-151">このフィールドは、パートナー管理コンソールのサブスクリプション ID にマップされます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="1b89b-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="1b89b-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="1b89b-153">OfferID</span></span></td>
<td><p><span data-ttu-id="1b89b-154">一意のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-154">Unique offer ID.</span></span> <span data-ttu-id="1b89b-155">価格表に従った標準のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="1b89b-156"><b>注意</b>:この値では、価格表からプラン ID が一致しません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="1b89b-157">以下の DurableOfferID を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b89b-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="1b89b-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="1b89b-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="1b89b-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="1b89b-160">価格表で定義されている一意の継続的なプラン ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="1b89b-161"><b>注意</b>:この値は、価格表からプラン ID と一致します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="1b89b-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="1b89b-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="1b89b-163">OfferName</span></span></td>
<td><p><span data-ttu-id="1b89b-164">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="1b89b-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="1b89b-165">Microsoft Office 365 (プラン E3)</span><span class="sxs-lookup"><span data-stu-id="1b89b-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="1b89b-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="1b89b-167">サブスクリプションの開始日。注文が送信された日に設定されます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="1b89b-168">サブスクリプションの開始日を終了日と共に確認することにより、顧客がサブスクリプションの最初の 1 年以内であるか、サブスクリプションが次の 1 年間更新されたかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="1b89b-169">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1b89b-170">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="1b89b-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="1b89b-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="1b89b-172">サブスクリプションの終了日:12 か月 + x 日間 (パートナーの請求日の連携) を開始日より後または更新日から 12 か月です。</span><span class="sxs-lookup"><span data-stu-id="1b89b-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="1b89b-173">更新時に、価格は最新の価格表に更新されます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="1b89b-174">自動更新の前に、顧客とのやり取りが必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="1b89b-175">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1b89b-176">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="1b89b-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="1b89b-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="1b89b-178">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="1b89b-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="1b89b-179">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="1b89b-180">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1b89b-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="1b89b-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="1b89b-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="1b89b-183">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="1b89b-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="1b89b-184">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="1b89b-185">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="1b89b-186">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="1b89b-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="1b89b-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="1b89b-188">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="1b89b-188">The type of charge or adjustment.</span></span> <span data-ttu-id="1b89b-189">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b89b-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="1b89b-190">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b89b-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="1b89b-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="1b89b-192">シート単価 (購入時に価格表に公開されていた価格)。</span><span class="sxs-lookup"><span data-stu-id="1b89b-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="1b89b-193">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="1b89b-194">6.82</span><span class="sxs-lookup"><span data-stu-id="1b89b-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-195">数量</span><span class="sxs-lookup"><span data-stu-id="1b89b-195">Quantity</span></span></td>
<td><p><span data-ttu-id="1b89b-196">シート数。</span><span class="sxs-lookup"><span data-stu-id="1b89b-196">Number of seats.</span></span> <span data-ttu-id="1b89b-197">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="1b89b-198">2</span><span class="sxs-lookup"><span data-stu-id="1b89b-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-199">金額</span><span class="sxs-lookup"><span data-stu-id="1b89b-199">Amount</span></span></td>
<td><p><span data-ttu-id="1b89b-200">数量に対する合計価格。</span><span class="sxs-lookup"><span data-stu-id="1b89b-200">Total of price for quantity.</span></span> <span data-ttu-id="1b89b-201">金額の計算が、この顧客用の計算方法に一致することを確認するために役立ちます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="1b89b-202">13.32</span><span class="sxs-lookup"><span data-stu-id="1b89b-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="1b89b-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="1b89b-204">これらの料金に適用される割引額。</span><span class="sxs-lookup"><span data-stu-id="1b89b-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="1b89b-205">インセンティブの対象となる IUR または新しいサブスクリプションの場合も、この列に割引額が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="1b89b-206">2.32</span><span class="sxs-lookup"><span data-stu-id="1b89b-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-207">Subtotal</span><span class="sxs-lookup"><span data-stu-id="1b89b-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="1b89b-208">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="1b89b-208">Total before tax.</span></span> <span data-ttu-id="1b89b-209">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="1b89b-210">11</span><span class="sxs-lookup"><span data-stu-id="1b89b-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-211">Tax</span><span class="sxs-lookup"><span data-stu-id="1b89b-211">Tax</span></span></td>
<td><p><span data-ttu-id="1b89b-212">市場に基づく、量の料金に税&#39;s 税法規と特定の状況です。</span><span class="sxs-lookup"><span data-stu-id="1b89b-212">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="1b89b-213">0</span><span class="sxs-lookup"><span data-stu-id="1b89b-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="1b89b-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="1b89b-215">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="1b89b-215">Total after tax.</span></span> <span data-ttu-id="1b89b-216">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="1b89b-217">11</span><span class="sxs-lookup"><span data-stu-id="1b89b-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-218">通貨</span><span class="sxs-lookup"><span data-stu-id="1b89b-218">Currency</span></span></td>
<td><p><span data-ttu-id="1b89b-219">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="1b89b-219">Currency type.</span></span> <span data-ttu-id="1b89b-220">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="1b89b-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="1b89b-221">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="1b89b-222">EUR</span><span class="sxs-lookup"><span data-stu-id="1b89b-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="1b89b-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="1b89b-224">顧客&#39;パートナー センターで報告される組織名。</span><span class="sxs-lookup"><span data-stu-id="1b89b-224">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="1b89b-225">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="1b89b-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="1b89b-226">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="1b89b-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="1b89b-227">MPNID</span></span></td>
<td><p><span data-ttu-id="1b89b-228">CSP パートナーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="1b89b-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="1b89b-229">4390934</span><span class="sxs-lookup"><span data-stu-id="1b89b-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="1b89b-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="1b89b-231">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="1b89b-232">「<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">パートナーごとに明細を示す</a>」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1b89b-232">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="1b89b-233">4390934</span><span class="sxs-lookup"><span data-stu-id="1b89b-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="1b89b-234">DomainName</span></span></td>
<td><p><span data-ttu-id="1b89b-235">顧客&#39;のドメインの名前、顧客を識別するために使用します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-235">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="1b89b-236">これを使用すると、顧客またはパートナーは O365 ポータルを使用して、バニティ/既定のドメインを更新できるように、ユーザーを一意に識別する必要がありますされません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="1b89b-237">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="1b89b-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="1b89b-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="1b89b-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="1b89b-240">サブスクリプションのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="1b89b-240">Subscription nickname.</span></span> <span data-ttu-id="1b89b-241">ニックネームが指定されていない場合、パートナー センターでは OfferName を使用します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="1b89b-242">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="1b89b-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="1b89b-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="1b89b-244">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="1b89b-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="1b89b-245">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="1b89b-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="1b89b-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span><span class="sxs-lookup"><span data-stu-id="1b89b-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="1b89b-247">ファイルの使用法に基づくフィールド</span><span class="sxs-lookup"><span data-stu-id="1b89b-247">Usage-based file fields</span></span>


<span data-ttu-id="1b89b-248">顧客の使用量に対する料金を調整するには、調整ファイルの ResellerID/ResellerName/ResellerBillableAccount、顧客名、およびパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="1b89b-249">次のフィールドで、どのサービスが使用されるか、およびレートについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="1b89b-250"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-250"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="1b89b-251"><strong>[説明]</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-251"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="1b89b-252"><strong>サンプル値</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-252"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="1b89b-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="1b89b-254">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="1b89b-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="1b89b-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="1b89b-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="1b89b-257">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="1b89b-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="1b89b-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="1b89b-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="1b89b-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="1b89b-260">パートナーのアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="1b89b-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="1b89b-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="1b89b-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="1b89b-263">顧客&#39;パートナー センターで報告される組織名。</span><span class="sxs-lookup"><span data-stu-id="1b89b-263">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="1b89b-264">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="1b89b-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="1b89b-265">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="1b89b-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="1b89b-266">MPNID</span></span></td>
<td><p><span data-ttu-id="1b89b-267">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="1b89b-268">4390934</span><span class="sxs-lookup"><span data-stu-id="1b89b-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="1b89b-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="1b89b-270">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="1b89b-271">「<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">パートナーごとに明細を示す</a>」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1b89b-271">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="1b89b-272">4390934</span><span class="sxs-lookup"><span data-stu-id="1b89b-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="1b89b-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="1b89b-274">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="1b89b-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="1b89b-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="1b89b-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="1b89b-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="1b89b-277">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="1b89b-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="1b89b-278">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1b89b-279">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="1b89b-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="1b89b-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="1b89b-281">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="1b89b-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="1b89b-282">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="1b89b-283">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="1b89b-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="1b89b-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="1b89b-285">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1b89b-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="1b89b-286">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="1b89b-287">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="1b89b-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="1b89b-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="1b89b-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="1b89b-290">サービス プランのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="1b89b-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="1b89b-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="1b89b-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="1b89b-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="1b89b-293">サービス プランの基幹業務</span><span class="sxs-lookup"><span data-stu-id="1b89b-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="1b89b-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="1b89b-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="1b89b-295">OrderID</span></span></td>
<td><p><span data-ttu-id="1b89b-296">Microsoft 請求プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1b89b-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="1b89b-297">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="1b89b-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="1b89b-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="1b89b-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="1b89b-300">対象の Azure サービスの名前。</span><span class="sxs-lookup"><span data-stu-id="1b89b-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="1b89b-301">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="1b89b-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="1b89b-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="1b89b-303">Windows Azure サービスの特定の種類。</span><span class="sxs-lookup"><span data-stu-id="1b89b-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="1b89b-304">Service Bus – Individual or Pack</span><span class="sxs-lookup"><span data-stu-id="1b89b-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="1b89b-305">SQL Azure database – Business or Web Edition</span><span class="sxs-lookup"><span data-stu-id="1b89b-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="1b89b-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="1b89b-307">すべてのサービス データおよび価格設定構造の特定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1b89b-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="1b89b-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="1b89b-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-309">リソース名</span><span class="sxs-lookup"><span data-stu-id="1b89b-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="1b89b-310">Azure リソースの名前。</span><span class="sxs-lookup"><span data-stu-id="1b89b-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="1b89b-311">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="1b89b-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="1b89b-312">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="1b89b-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-313">Region</span><span class="sxs-lookup"><span data-stu-id="1b89b-313">Region</span></span></td>
<td><p><span data-ttu-id="1b89b-314">使用量が適用される地域。</span><span class="sxs-lookup"><span data-stu-id="1b89b-314">The region the usage applies to.</span></span> <span data-ttu-id="1b89b-315">料金は地域によって異なるため、主にデータ転送に料金を割り当てるために使われます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="1b89b-316">Asia Pacific、Europe、Latin America、North America</span><span class="sxs-lookup"><span data-stu-id="1b89b-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-317">SKU (SKU)</span><span class="sxs-lookup"><span data-stu-id="1b89b-317">SKU</span></span></td>
<td><p><span data-ttu-id="1b89b-318">プランについての MSFT の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="1b89b-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="1b89b-319">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="1b89b-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="1b89b-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="1b89b-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="1b89b-321">特定の課金期間のサービスまたはリソースに対してさまざまなレートの明細を設定するための ID と数量。</span><span class="sxs-lookup"><span data-stu-id="1b89b-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="1b89b-322">Azure の階層化されたレーティングの場合は、一定数量の課金可能単位までは 1 つのレートがあり、その後に別のレートがあることがあります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="1b89b-323">1</span><span class="sxs-lookup"><span data-stu-id="1b89b-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="1b89b-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="1b89b-325">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="1b89b-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="1b89b-326">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="1b89b-327">11</span><span class="sxs-lookup"><span data-stu-id="1b89b-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="1b89b-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="1b89b-329">単位数はプランの一部として含まれます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-329">Units included as part of the offer.</span></span> <span data-ttu-id="1b89b-330">通常、CSP には含まれません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="1b89b-331">0</span><span class="sxs-lookup"><span data-stu-id="1b89b-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="1b89b-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="1b89b-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="1b89b-333">単位数はプランの一部として含まれず、パートナーが支払う必要があります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="1b89b-334">ConsumedQuantity - IncludedQuantity と同じです。</span><span class="sxs-lookup"><span data-stu-id="1b89b-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="1b89b-335">11</span><span class="sxs-lookup"><span data-stu-id="1b89b-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="1b89b-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="1b89b-337">サブスクリプションの開始日に有効な価格を提供します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="1b89b-338">$0.0808</span><span class="sxs-lookup"><span data-stu-id="1b89b-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="1b89b-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="1b89b-340">ListPrist と OverageQuantity を掛けて、最も近いセントに丸めます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="1b89b-341">$0.085</span><span class="sxs-lookup"><span data-stu-id="1b89b-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="1b89b-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="1b89b-343">市場に基づく、量の料金に税&#39;s 税法規と特定の状況です。</span><span class="sxs-lookup"><span data-stu-id="1b89b-343">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="1b89b-344">$0.08</span><span class="sxs-lookup"><span data-stu-id="1b89b-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="1b89b-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="1b89b-346">税が適用されるときの税引き後の合計額。</span><span class="sxs-lookup"><span data-stu-id="1b89b-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="1b89b-347">$0.93</span><span class="sxs-lookup"><span data-stu-id="1b89b-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-348">通貨</span><span class="sxs-lookup"><span data-stu-id="1b89b-348">Currency</span></span></td>
<td><p><span data-ttu-id="1b89b-349">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="1b89b-349">Currency type.</span></span> <span data-ttu-id="1b89b-350">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="1b89b-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="1b89b-351">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="1b89b-352">EUR</span><span class="sxs-lookup"><span data-stu-id="1b89b-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="1b89b-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="1b89b-354">単位あたりの税込み価格。</span><span class="sxs-lookup"><span data-stu-id="1b89b-354">Pretax price per unit.</span></span> <span data-ttu-id="1b89b-355">PretaxCharges / OverageQuantity と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="1b89b-356">$0.08</span><span class="sxs-lookup"><span data-stu-id="1b89b-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="1b89b-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="1b89b-358">単位あたりの税引き後の価格。</span><span class="sxs-lookup"><span data-stu-id="1b89b-358">Post tax price per unit.</span></span> <span data-ttu-id="1b89b-359">PostTaxTotal / OverageQuantity、または PretaxEffectiveRate + 単位額あたりの税率と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="1b89b-360">$0.08</span><span class="sxs-lookup"><span data-stu-id="1b89b-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="1b89b-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="1b89b-362">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="1b89b-362">The type of charge or adjustment.</span></span> <span data-ttu-id="1b89b-363">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b89b-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="1b89b-364">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b89b-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="1b89b-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="1b89b-366">MSFT 課金プラットフォームの一意のアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="1b89b-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="1b89b-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="1b89b-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="1b89b-369">サービスの展開の日付。</span><span class="sxs-lookup"><span data-stu-id="1b89b-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="1b89b-370">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="1b89b-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="1b89b-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="1b89b-372">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="1b89b-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="1b89b-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="1b89b-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="1b89b-375">この列は、[Service Name] 列で特に識別されない可能性のある、個別の Microsoft Azure サービスの追跡に利用されます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="1b89b-376">たとえば、データ転送は、[Service Name] 列で &quot;Microsoft Azure - All Services&quot; と報告されます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="1b89b-377">この [MeteredService] 列は、利用に関連する特定のサービスを示します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="1b89b-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="1b89b-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="1b89b-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="1b89b-380">個々の Microsoft Azure サービスの内容を、MeteredService フィールドで提供されるレベルよりも明確にする小見出し。</span><span class="sxs-lookup"><span data-stu-id="1b89b-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="1b89b-381">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="1b89b-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-382">Project</span><span class="sxs-lookup"><span data-stu-id="1b89b-382">Project</span></span></td>
<td><p><span data-ttu-id="1b89b-383">サービス インスタンスの顧客定義の名前</span><span class="sxs-lookup"><span data-stu-id="1b89b-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="1b89b-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="1b89b-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="1b89b-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="1b89b-386">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="1b89b-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="1b89b-387">例: 1 か月 30 日間の中に、個別にプロビジョニングされた接続がある場合、Service Info 1 は "1.000000 Connections / 30 days" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="1b89b-388">Service Bus 接続のプロビジョニングが 25 パックする必要があるし、その日に 1 つを利用して、その日、毎日の使用量明細を示す"25 接続/30 Days-Used:1.000000”.</span><span class="sxs-lookup"><span data-stu-id="1b89b-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="1b89b-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="1b89b-390">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="1b89b-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="1b89b-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1b89b-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="1b89b-392">DomainName</span></span></td>
<td><p><span data-ttu-id="1b89b-393">顧客&#39;のドメインの名前、顧客を識別するために使用します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-393">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="1b89b-394">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="1b89b-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="1b89b-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="1b89b-396">Unit</span><span class="sxs-lookup"><span data-stu-id="1b89b-396">Unit</span></span></td>
<td><p><span data-ttu-id="1b89b-397">リソース名の単位</span><span class="sxs-lookup"><span data-stu-id="1b89b-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="1b89b-398">GB または HOURS</span><span class="sxs-lookup"><span data-stu-id="1b89b-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="1b89b-399">1 回だけ、定期的なファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="1b89b-399">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="1b89b-400">[列]</span><span class="sxs-lookup"><span data-stu-id="1b89b-400">Column</span></span></th>
<th><span data-ttu-id="1b89b-401">説明</span><span class="sxs-lookup"><span data-stu-id="1b89b-401">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="1b89b-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="1b89b-402">PartnerId</span></span></td>
<td><p><span data-ttu-id="1b89b-403">GUID 形式で、特定の課金エンティティの一意の Microsoft Azure Active Directory テナント識別子。</span><span class="sxs-lookup"><span data-stu-id="1b89b-403">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="1b89b-404">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-404">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="1b89b-405">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="1b89b-405">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-406">顧客 Id</span><span class="sxs-lookup"><span data-stu-id="1b89b-406">Customer Id</span></span></td>
<td><p><span data-ttu-id="1b89b-407">一意な Microsoft Azure Active Directory テナント ID、GUID 形式で顧客を識別するために使用します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-407">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-408">顧客名</span><span class="sxs-lookup"><span data-stu-id="1b89b-408">Customer Name</span></span></td>
<td><p><span data-ttu-id="1b89b-409">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="1b89b-409">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="1b89b-410">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="1b89b-411">顧客のドメイン名。顧客を特定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-411">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="1b89b-412">これを使用すると、顧客またはパートナーは O365 ポータルを使用して、バニティ/既定のドメインを更新できるように、ユーザーを一意に識別する必要がありますされません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-412">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="1b89b-413">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-413">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-414">顧客の国</span><span class="sxs-lookup"><span data-stu-id="1b89b-414">Customer Country</span></span></td>
<td><p><span data-ttu-id="1b89b-415">顧客の在住国。</span><span class="sxs-lookup"><span data-stu-id="1b89b-415">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-416">請求書番号</span><span class="sxs-lookup"><span data-stu-id="1b89b-416">Invoice number</span></span></td>
<td><p><span data-ttu-id="1b89b-417">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="1b89b-417">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-418">MpnId</span><span class="sxs-lookup"><span data-stu-id="1b89b-418">MpnId</span></span></td>
<td><p><span data-ttu-id="1b89b-419">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-419">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-420">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="1b89b-420">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="1b89b-421">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-421">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-422">注文 ID</span><span class="sxs-lookup"><span data-stu-id="1b89b-422">Order ID</span></span></td>
<td><p><span data-ttu-id="1b89b-423">マイクロソフト コマース プラットフォームでの注文の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="1b89b-423">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="1b89b-424">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-424">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-425">発注日</span><span class="sxs-lookup"><span data-stu-id="1b89b-425">Order date</span></span></td>
<td><p><span data-ttu-id="1b89b-426">注文が作成された日付。</span><span class="sxs-lookup"><span data-stu-id="1b89b-426">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-427">ProductId</span><span class="sxs-lookup"><span data-stu-id="1b89b-427">ProductId</span></span></td>
<td><p><span data-ttu-id="1b89b-428">製品の ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-428">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-429">SkuId</span><span class="sxs-lookup"><span data-stu-id="1b89b-429">SkuId</span></span></td>
<td><p><span data-ttu-id="1b89b-430">特定 SKU の ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-430">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-431">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="1b89b-431">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="1b89b-432">特定の可用性 の ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-432">The ID for a particular Availability.</span></span> <span data-ttu-id="1b89b-433">"可用性" とは、特定の国、通貨、業界などで特定の SKU を購入可能かどうかを指します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-433">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-434">SKU 名</span><span class="sxs-lookup"><span data-stu-id="1b89b-434">SKU Name</span></span></td>
<td><p><span data-ttu-id="1b89b-435">特定 SKU のタイトル。</span><span class="sxs-lookup"><span data-stu-id="1b89b-435">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-436">製品名</span><span class="sxs-lookup"><span data-stu-id="1b89b-436">Product name</span></span></td>
<td><p><span data-ttu-id="1b89b-437">製品の名前。</span><span class="sxs-lookup"><span data-stu-id="1b89b-437">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-438">PublisherName</span><span class="sxs-lookup"><span data-stu-id="1b89b-438">PublisherName</span></span></td>
<td><p><span data-ttu-id="1b89b-439">製品のパブリッシャーの名前。</span><span class="sxs-lookup"><span data-stu-id="1b89b-439">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-440">PublisherID</span><span class="sxs-lookup"><span data-stu-id="1b89b-440">PublisherID</span></span></td>
<td><p><span data-ttu-id="1b89b-441">このパブリッシャーに対して一意の ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-441">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-442">サブスクリプションの説明</span><span class="sxs-lookup"><span data-stu-id="1b89b-442">Subscription Description</span></span></td>
<td><p><span data-ttu-id="1b89b-443">サブスクリプションのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="1b89b-443">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-444">サブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="1b89b-444">Subscription ID</span></span></td>
<td><p><span data-ttu-id="1b89b-445">マイクロソフト コマース プラットフォームでサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1b89b-445">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="1b89b-446">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-446">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="1b89b-447">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-447">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-448">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="1b89b-448">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="1b89b-449">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="1b89b-449">Start day of the charges.</span></span> <span data-ttu-id="1b89b-450">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-450">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-451">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="1b89b-451">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="1b89b-452">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="1b89b-452">End day of the charges.</span></span> <span data-ttu-id="1b89b-453">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-453">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-454">用語と Billingcycle</span><span class="sxs-lookup"><span data-stu-id="1b89b-454">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="1b89b-455">期間と購入の請求サイクルでします。</span><span class="sxs-lookup"><span data-stu-id="1b89b-455">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="1b89b-456">たとえば、「1 年、月単位です。」</span><span class="sxs-lookup"><span data-stu-id="1b89b-456">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-457">請求の種類</span><span class="sxs-lookup"><span data-stu-id="1b89b-457">Charge Type</span></span></td>
<td><p><span data-ttu-id="1b89b-458">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="1b89b-458">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-459">単価</span><span class="sxs-lookup"><span data-stu-id="1b89b-459">Unit Price</span></span></td>
<td><p><span data-ttu-id="1b89b-460">購入時、pricelist で発行される価格です。</span><span class="sxs-lookup"><span data-stu-id="1b89b-460">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="1b89b-461">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-461">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-462">効果的な単体の価格</span><span class="sxs-lookup"><span data-stu-id="1b89b-462">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="1b89b-463">調整が行われた後の単位の価格です。</span><span class="sxs-lookup"><span data-stu-id="1b89b-463">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-464">数量</span><span class="sxs-lookup"><span data-stu-id="1b89b-464">Quantity</span></span></td>
<td><p><span data-ttu-id="1b89b-465">ユニットの数。</span><span class="sxs-lookup"><span data-stu-id="1b89b-465">Number of units.</span></span> <span data-ttu-id="1b89b-466">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-466">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-467">ユニットの種類</span><span class="sxs-lookup"><span data-stu-id="1b89b-467">Unit type</span></span></td>
<td><p><span data-ttu-id="1b89b-468">購入されているユニットの種類。</span><span class="sxs-lookup"><span data-stu-id="1b89b-468">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-469">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="1b89b-469">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="1b89b-470">該当する何らかの割引の説明。</span><span class="sxs-lookup"><span data-stu-id="1b89b-470">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-471">小計</span><span class="sxs-lookup"><span data-stu-id="1b89b-471">Sub Total</span></span></td>
<td><p><span data-ttu-id="1b89b-472">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="1b89b-472">Total before tax.</span></span> <span data-ttu-id="1b89b-473">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-473">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-474">売上税合計</span><span class="sxs-lookup"><span data-stu-id="1b89b-474">Tax Total</span></span></td>
<td><p><span data-ttu-id="1b89b-475">市場の税関連の規則や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="1b89b-475">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-476">Total</span><span class="sxs-lookup"><span data-stu-id="1b89b-476">Total</span></span></td>
<td><p><span data-ttu-id="1b89b-477">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="1b89b-477">Total after tax.</span></span> <span data-ttu-id="1b89b-478">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-478">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-479">通貨</span><span class="sxs-lookup"><span data-stu-id="1b89b-479">Currency</span></span></td>
<td><p><span data-ttu-id="1b89b-480">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="1b89b-480">Currency type.</span></span> <span data-ttu-id="1b89b-481">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="1b89b-481">Each billing entity has only one currency.</span></span> <span data-ttu-id="1b89b-482">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-482">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-483">代替</span><span class="sxs-lookup"><span data-stu-id="1b89b-483">AlternateID</span></span></td>
<td><p><span data-ttu-id="1b89b-484">代替の識別子を注文 ID</span><span class="sxs-lookup"><span data-stu-id="1b89b-484">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="1b89b-485">評価の毎日の使用状況ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="1b89b-485">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="1b89b-486">[列]</span><span class="sxs-lookup"><span data-stu-id="1b89b-486">Column</span></span></th>
<th><span data-ttu-id="1b89b-487">説明</span><span class="sxs-lookup"><span data-stu-id="1b89b-487">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="1b89b-488">PartnerId</span><span class="sxs-lookup"><span data-stu-id="1b89b-488">PartnerId</span></span></td>
<td><p><span data-ttu-id="1b89b-489">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-489">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-490">PartnerName</span><span class="sxs-lookup"><span data-stu-id="1b89b-490">PartnerName</span></span></td>
<td><p><span data-ttu-id="1b89b-491">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="1b89b-491">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-492">CustomerId</span><span class="sxs-lookup"><span data-stu-id="1b89b-492">CustomerId</span></span></td>
<td><p><span data-ttu-id="1b89b-493">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-493">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-494">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="1b89b-494">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="1b89b-495">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="1b89b-495">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="1b89b-496">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="1b89b-496">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-497">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="1b89b-497">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="1b89b-498">顧客のドメイン名。</span><span class="sxs-lookup"><span data-stu-id="1b89b-498">The customer’s domain name.</span></span> <span data-ttu-id="1b89b-499">現在のアクティビティは使用できません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-499">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-500">顧客の国</span><span class="sxs-lookup"><span data-stu-id="1b89b-500">Customer country</span></span></td>
<td><p><span data-ttu-id="1b89b-501">顧客の在住国。</span><span class="sxs-lookup"><span data-stu-id="1b89b-501">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-502">MPNID</span><span class="sxs-lookup"><span data-stu-id="1b89b-502">MPNID</span></span></td>
<td><p><span data-ttu-id="1b89b-503">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-503">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-504">Reseller MPNID</span><span class="sxs-lookup"><span data-stu-id="1b89b-504">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="1b89b-505">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-505">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="1b89b-506">現在のアクティビティは使用できません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-506">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-507">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="1b89b-507">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="1b89b-508">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="1b89b-508">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="1b89b-509">現在のアクティビティは使用できません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-509">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-510">ProductId</span><span class="sxs-lookup"><span data-stu-id="1b89b-510">ProductId</span></span></td>
<td><p><span data-ttu-id="1b89b-511">製品の ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-511">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-512">SkuId</span><span class="sxs-lookup"><span data-stu-id="1b89b-512">SkuId</span></span></td>
<td><p><span data-ttu-id="1b89b-513">特定 SKU の ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-513">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-514">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="1b89b-514">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="1b89b-515">特定の可用性 の ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-515">The ID for a particular Availability.</span></span> <span data-ttu-id="1b89b-516">"可用性" とは、特定の国、通貨、業界などで特定の SKU を購入可能かどうかを指します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-516">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-517">SKU 名</span><span class="sxs-lookup"><span data-stu-id="1b89b-517">SKU Name</span></span></td>
<td><p><span data-ttu-id="1b89b-518">特定 SKU のタイトル。</span><span class="sxs-lookup"><span data-stu-id="1b89b-518">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-519">PublisherName</span><span class="sxs-lookup"><span data-stu-id="1b89b-519">PublisherName</span></span></td>
<td><p><span data-ttu-id="1b89b-520">パブリッシャーの名前。</span><span class="sxs-lookup"><span data-stu-id="1b89b-520">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-521">PublisherID</span><span class="sxs-lookup"><span data-stu-id="1b89b-521">PublisherID</span></span></td>
<td><p><span data-ttu-id="1b89b-522">GUID 形式で、パブリッシャーの ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-522">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="1b89b-523">現在のアクティビティは使用できません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="1b89b-524">サブスクリプションの説明</span><span class="sxs-lookup"><span data-stu-id="1b89b-524">Subscription Description</span></span></td>
<td><p><span data-ttu-id="1b89b-525">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="1b89b-525">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="1b89b-526">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="1b89b-526">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-527">サブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="1b89b-527">Subscription ID</span></span></td>
<td><p><span data-ttu-id="1b89b-528">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1b89b-528">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="1b89b-529">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-529">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="1b89b-530">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-530">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-531">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="1b89b-531">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="1b89b-532">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="1b89b-532">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="1b89b-533">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-533">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-534">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="1b89b-534">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="1b89b-535">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="1b89b-535">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="1b89b-536">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="1b89b-536">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-537">使用日</span><span class="sxs-lookup"><span data-stu-id="1b89b-537">Usage Date</span></span></td>
<td><p><span data-ttu-id="1b89b-538">サービスの使用状況の日です。</span><span class="sxs-lookup"><span data-stu-id="1b89b-538">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-539">メーターの種類</span><span class="sxs-lookup"><span data-stu-id="1b89b-539">Meter Type</span></span></td>
<td><p><span data-ttu-id="1b89b-540">測定の種類。</span><span class="sxs-lookup"><span data-stu-id="1b89b-540">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-541">メーター カテゴリ</span><span class="sxs-lookup"><span data-stu-id="1b89b-541">Meter Category</span></span></td>
<td><p><span data-ttu-id="1b89b-542">使用状況の最上位のサービスです。</span><span class="sxs-lookup"><span data-stu-id="1b89b-542">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-543">測定 Id</span><span class="sxs-lookup"><span data-stu-id="1b89b-543">Meter Id</span></span></td>
<td><p><span data-ttu-id="1b89b-544">使用されているメーターの ID。</span><span class="sxs-lookup"><span data-stu-id="1b89b-544">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-545">測定サブカテゴリ</span><span class="sxs-lookup"><span data-stu-id="1b89b-545">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="1b89b-546">速度に影響を与える Azure サービスの型。</span><span class="sxs-lookup"><span data-stu-id="1b89b-546">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-547">測定名</span><span class="sxs-lookup"><span data-stu-id="1b89b-547">Meter Name</span></span></td>
<td><p><span data-ttu-id="1b89b-548">消費しているメーターの測定単位。</span><span class="sxs-lookup"><span data-stu-id="1b89b-548">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-549">メーター リージョン</span><span class="sxs-lookup"><span data-stu-id="1b89b-549">Meter Region</span></span></td>
<td><p><span data-ttu-id="1b89b-550">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-550">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-551">Unit</span><span class="sxs-lookup"><span data-stu-id="1b89b-551">Unit</span></span></td>
<td><p><span data-ttu-id="1b89b-552">リソース名の単位。</span><span class="sxs-lookup"><span data-stu-id="1b89b-552">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-553">使用量</span><span class="sxs-lookup"><span data-stu-id="1b89b-553">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="1b89b-554">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="1b89b-554">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="1b89b-555">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-555">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-556">リソースの場所</span><span class="sxs-lookup"><span data-stu-id="1b89b-556">Resource Location</span></span></td>
<td><p><span data-ttu-id="1b89b-557">メーターが実行されているデータ センターです。</span><span class="sxs-lookup"><span data-stu-id="1b89b-557">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-558">使用するサービス</span><span class="sxs-lookup"><span data-stu-id="1b89b-558">Consumed Service</span></span></td>
<td><p><span data-ttu-id="1b89b-559">使用して、Azure プラットフォーム サービスです。</span><span class="sxs-lookup"><span data-stu-id="1b89b-559">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-560">リソース グループ</span><span class="sxs-lookup"><span data-stu-id="1b89b-560">Resource Group</span></span></td>
<td><p><span data-ttu-id="1b89b-561">デプロイされたメーターが実行されているリソース グループ。</span><span class="sxs-lookup"><span data-stu-id="1b89b-561">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-562">リソース URI</span><span class="sxs-lookup"><span data-stu-id="1b89b-562">Resource URI</span></span></td>
<td><p><span data-ttu-id="1b89b-563">使用されているリソースの URI。</span><span class="sxs-lookup"><span data-stu-id="1b89b-563">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-564">請求の種類</span><span class="sxs-lookup"><span data-stu-id="1b89b-564">Charge type</span></span></td>
<td><p><span data-ttu-id="1b89b-565">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="1b89b-565">The type of charge or adjustment.</span></span> <span data-ttu-id="1b89b-566">現在のアクティビティは使用できません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-566">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-567">単価</span><span class="sxs-lookup"><span data-stu-id="1b89b-567">Unit price</span></span></td>
<td><p><span data-ttu-id="1b89b-568">購入時、pricelist でパブリッシュされると、ライセンスあたりの価格。</span><span class="sxs-lookup"><span data-stu-id="1b89b-568">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="1b89b-569">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-569">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-570">数量</span><span class="sxs-lookup"><span data-stu-id="1b89b-570">Quantity</span></span></td>
<td><p><span data-ttu-id="1b89b-571">ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="1b89b-571">Number of licenses.</span></span> <span data-ttu-id="1b89b-572">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-572">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-573">ユニットの種類</span><span class="sxs-lookup"><span data-stu-id="1b89b-573">Unit type</span></span></td>
<td><p><span data-ttu-id="1b89b-574">メーターが課金単位の種類。</span><span class="sxs-lookup"><span data-stu-id="1b89b-574">The type of unit the meter is charged in.</span></span> <span data-ttu-id="1b89b-575">現在のアクティビティは使用できません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-575">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-576">前の税金を請求</span><span class="sxs-lookup"><span data-stu-id="1b89b-576">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="1b89b-577">税引き前に、の合計。</span><span class="sxs-lookup"><span data-stu-id="1b89b-577">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-578">請求通貨</span><span class="sxs-lookup"><span data-stu-id="1b89b-578">Billing currency</span></span></td>
<td><p><span data-ttu-id="1b89b-579">顧客の地理的リージョン内の通貨</span><span class="sxs-lookup"><span data-stu-id="1b89b-579">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-580">税込み合計を価格</span><span class="sxs-lookup"><span data-stu-id="1b89b-580">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="1b89b-581">価格の税が追加される前にします。</span><span class="sxs-lookup"><span data-stu-id="1b89b-581">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-582">通貨の価格</span><span class="sxs-lookup"><span data-stu-id="1b89b-582">Pricing currency</span></span></td>
<td><p><span data-ttu-id="1b89b-583">Pricelist 通貨です。</span><span class="sxs-lookup"><span data-stu-id="1b89b-583">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-584">サービス情報 1</span><span class="sxs-lookup"><span data-stu-id="1b89b-584">Service Info 1</span></span></td>
<td><p><span data-ttu-id="1b89b-585">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="1b89b-585">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-586">サービス情報 2</span><span class="sxs-lookup"><span data-stu-id="1b89b-586">Service Info 2</span></span></td>
<td><p><span data-ttu-id="1b89b-587">省略可能なサービスに固有のメタデータをキャプチャするレガシ フィールドです。</span><span class="sxs-lookup"><span data-stu-id="1b89b-587">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1b89b-588">Tags</span><span class="sxs-lookup"><span data-stu-id="1b89b-588">Tags</span></span></td>
<td><p><span data-ttu-id="1b89b-589">課金のレコードをグループ化の順序でメーターに割り当てるタグ。</span><span class="sxs-lookup"><span data-stu-id="1b89b-589">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="1b89b-590">たとえば、メーターを使用する部門ごとのコストを配布するのにタグを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-590">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1b89b-591">追加情報</span><span class="sxs-lookup"><span data-stu-id="1b89b-591">Additional Info</span></span></td>
<td><p><span data-ttu-id="1b89b-592">追加情報は、他の列では説明しません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-592">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="1b89b-593">請求書と調整ファイルの間の料金のマッピング</span><span class="sxs-lookup"><span data-stu-id="1b89b-593">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="1b89b-594">請求書は料金の概要を示し、調整ファイルは、課金の種類を含め、行項目のトランザクションの詳細な内訳を示します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-594">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="1b89b-595">請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルター オプションを使用して、調整ファイルの課金の種類でフィルター処理し、請求書の課金を調整ファイルの一連の課金の内訳にマップします。</span><span class="sxs-lookup"><span data-stu-id="1b89b-595">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="1b89b-596">使用量ベースとライセンス ベースの調整ファイルには、使用量関連のトランザクションと料金 (消費された単位量および関連する料金) のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1b89b-596">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="1b89b-597">請求書に “調整” として表示される単発のクレジット、割引、払い戻し金額は、調整ファイルに表示されません。</span><span class="sxs-lookup"><span data-stu-id="1b89b-597">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="1b89b-598">次の表に、請求書のセクションと、調整ファイルに表示される関連付けられた課金の種類とのマッピングを示します。</span><span class="sxs-lookup"><span data-stu-id="1b89b-598">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="1b89b-599"><strong>請求書の料金の説明</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-599"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-600"><strong>調整ファイルの料金の説明 (ChargeType 列)</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-600"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-601"><strong>この料金は何ですか。</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-601"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-602"><strong>請求書にこれら ChargeTypes をマップする方法</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-602"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="1b89b-603"><strong>ライセンス ベースの料金</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-603"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-604">アクティブ化料金</span><span class="sxs-lookup"><span data-stu-id="1b89b-604">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-605">購入したサブスクリプションを顧客が使用したときに顧客に課金される金額</span><span class="sxs-lookup"><span data-stu-id="1b89b-605">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="1b89b-606">ライセンスベースのファイルから、<strong>Amount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1b89b-606">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1b89b-607">取り消し料金</span><span class="sxs-lookup"><span data-stu-id="1b89b-607">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-608">関連付けられているシートが変更されたときに顧客に払い戻される日割り料金</span><span class="sxs-lookup"><span data-stu-id="1b89b-608">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1b89b-609">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="1b89b-609">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-610">サブスクリプションの定期的な課金</span><span class="sxs-lookup"><span data-stu-id="1b89b-610">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1b89b-611">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="1b89b-611">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-612">関連付けられているシートが変更されたときに顧客から評価される日割り料金</span><span class="sxs-lookup"><span data-stu-id="1b89b-612">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1b89b-613">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="1b89b-613">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-614">取り消し時のサービスの未使用部分に対する日割りの払戻し額</span><span class="sxs-lookup"><span data-stu-id="1b89b-614">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1b89b-615">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="1b89b-615">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-616">年次請求に使用する場合、サブスクリプションの料金タイプ</span><span class="sxs-lookup"><span data-stu-id="1b89b-616">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1b89b-617">Purchase fee</span><span class="sxs-lookup"><span data-stu-id="1b89b-617">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-618">月額使用料を使用する場合、サブスクリプションの料金タイプ</span><span class="sxs-lookup"><span data-stu-id="1b89b-618">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1b89b-619">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="1b89b-619">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-620">サブスクリプションの更新時の日割り料金</span><span class="sxs-lookup"><span data-stu-id="1b89b-620">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="1b89b-621">Renew fee</span><span class="sxs-lookup"><span data-stu-id="1b89b-621">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-622">サブスクリプションの更新時の課金</span><span class="sxs-lookup"><span data-stu-id="1b89b-622">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1b89b-623">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="1b89b-623">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-624">アクティブ化から課金期間の終了までの日割り料金</span><span class="sxs-lookup"><span data-stu-id="1b89b-624">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="1b89b-625"><strong>利用料金</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-625"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-626">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="1b89b-626">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-627">現在の課金期間中に未払いの使用を取り消したときのアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="1b89b-627">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="1b89b-628">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1b89b-628">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1b89b-629">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="1b89b-629">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-630">現在の課金期間のアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="1b89b-630">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1b89b-631"><strong>クレジット</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-631"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-632">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="1b89b-632">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-633">税金を含む、行項目への一部または全部の払戻し</span><span class="sxs-lookup"><span data-stu-id="1b89b-633">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-634">ライセンスベースのファイルから、<strong>TotalForCustomer</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1b89b-634">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="1b89b-635">使用量ベースのファイルから、<strong>PostTaxTotal</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1b89b-635">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="1b89b-636"><strong>使用法に基づく割引</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-636"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-637">Activation discount</span><span class="sxs-lookup"><span data-stu-id="1b89b-637">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-638">サブスクリプションがアクティブ化されたときに適用される割引</span><span class="sxs-lookup"><span data-stu-id="1b89b-638">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="1b89b-639">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1b89b-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1b89b-640">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="1b89b-640">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-641">定期的な課金に適用される割引</span><span class="sxs-lookup"><span data-stu-id="1b89b-641">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1b89b-642">Renew discount</span><span class="sxs-lookup"><span data-stu-id="1b89b-642">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-643">サブスクリプションの更新時に適用される割引</span><span class="sxs-lookup"><span data-stu-id="1b89b-643">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1b89b-644">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="1b89b-644">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-645">割引が取り消されたときに適用される料金</span><span class="sxs-lookup"><span data-stu-id="1b89b-645">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="1b89b-646"><strong>ライセンス ベースの割引</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-646"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-647"><em>複数の料金の種類に適用できます。</em></span><span class="sxs-lookup"><span data-stu-id="1b89b-647"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="1b89b-648">ライセンスベースのファイルから、<strong>TotalOtherDiscount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1b89b-648">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1b89b-649"><strong>税</strong>&nbsp;または&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="1b89b-649"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-650"><em>複数の料金の種類に適用できます。</em></span><span class="sxs-lookup"><span data-stu-id="1b89b-650"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="1b89b-651"><em>例外:&quot;行項目を相殺&quot;税金が既に含まれています。上記のクレジットを参照してください。</em></span><span class="sxs-lookup"><span data-stu-id="1b89b-651"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-652">税または付加価値税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="1b89b-652">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="1b89b-653">ライセンスベースのファイルから、<strong>Tax</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1b89b-653">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="1b89b-654">使用量ベースのファイルから、<strong>TaxAmount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1b89b-654">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
