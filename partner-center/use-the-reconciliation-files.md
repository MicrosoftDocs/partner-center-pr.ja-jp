---
title: 調整ファイルを使う | パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: 請求サイクルの各料金の詳しい行項目ビューのためには、パートナー センターから、調整ファイルをダウンロードします。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 081afc547a0ff86010e06fcb5224a615a0075e34
ms.sourcegitcommit: 8bfd1358a0ef86e46bee2a1097d86de3c9e969e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "9122279"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="b84cb-103">調整ファイルを使う</span><span class="sxs-lookup"><span data-stu-id="b84cb-103">Use the reconciliation files</span></span>

**<span data-ttu-id="b84cb-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="b84cb-104">Applies to</span></span>**

-  <span data-ttu-id="b84cb-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="b84cb-105">Partner Center</span></span>
-  <span data-ttu-id="b84cb-106">Microsoft Cloud for US Government のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="b84cb-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="b84cb-107">請求サイクルの各料金の詳しい行項目ビューのためには、パートナー センターから、調整ファイルをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="b84cb-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="b84cb-108">詳細には、各顧客のサブスクリプションの料金や、詳細なイベント (期間途中でのサブスクリプションへのシートの追加など) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="b84cb-109">パートナーごとに明細を示す</span><span class="sxs-lookup"><span data-stu-id="b84cb-109">Itemize by partner</span></span>


<span data-ttu-id="b84cb-110">インダイレクト モデルのパートナーは、ライセンス ベースの調整ファイルと使用量ベースの調整ファイルの両方で、これらの追加フィールドを使用してリセラーごとに明細を記載できます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b84cb-111">MPN ID</span><span class="sxs-lookup"><span data-stu-id="b84cb-111">MPN ID</span></span></th>
<th><span data-ttu-id="b84cb-112">説明</span><span class="sxs-lookup"><span data-stu-id="b84cb-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="b84cb-113">MPN ID</span><span class="sxs-lookup"><span data-stu-id="b84cb-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="b84cb-114">CSP パートナー (直接または間接) の Microsoft Partner Network (MPN) IDです。</span><span class="sxs-lookup"><span data-stu-id="b84cb-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-115">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="b84cb-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="b84cb-116">インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="b84cb-117">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b84cb-118">これは、パートナー センターで特定のサブスクリプションについて示されるリセラー ID に対応します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="b84cb-119">リセラーを表示または更新プログラム、パートナー センター メニューから、リセラーは、<strong>顧客</strong>を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="b84cb-120">顧客メニューの <strong>[サブスクリプション]</strong> を選び、一覧からサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="b84cb-121">
          <strong>[更新]</strong> を選んで、<strong>[再販業者 (MPN ID)]</strong> を変更します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="b84cb-122">CSP パートナーがお客様に直接サブスクリプションを販売した場合、パートナーの MPN ID が MPN ID とリセラーの MPN ID として 2 か所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="b84cb-123">CSP パートナーのリセラーに MPN ID がない場合は、代わりに CSP パートナーの MPN ID がこの値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="b84cb-124">CSP パートナーがリセラー ID を削除した場合、この値は -1 に設定されます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="b84cb-125">ライセンス ベースのファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="b84cb-125">License-based file fields</span></span>


<span data-ttu-id="b84cb-126">顧客の注文に対する料金を調整するには、調整ファイルの Syndication\_Partner\_Subscription\_Number とパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="b84cb-127">列</span><span class="sxs-lookup"><span data-stu-id="b84cb-127">Column</span></span></strong></td>
<td><strong><span data-ttu-id="b84cb-128">説明</span><span class="sxs-lookup"><span data-stu-id="b84cb-128">Description</span></span></strong></td>
<td><strong><span data-ttu-id="b84cb-129">サンプル値</span><span class="sxs-lookup"><span data-stu-id="b84cb-129">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="b84cb-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="b84cb-131">特定の課金エンティティの一意の識別子 (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="b84cb-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="b84cb-132">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="b84cb-133">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="b84cb-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="b84cb-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="b84cb-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="b84cb-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="b84cb-136">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="b84cb-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="b84cb-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="b84cb-138">OrderID</span></span></td>
<td><p><span data-ttu-id="b84cb-139">Microsoft 課金プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b84cb-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="b84cb-140">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="b84cb-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="b84cb-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="b84cb-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="b84cb-143">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b84cb-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b84cb-144">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="b84cb-145">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="b84cb-146">「Syndication_Partner_Subscription_Number」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b84cb-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="b84cb-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="b84cb-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="b84cb-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="b84cb-149">サブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b84cb-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="b84cb-150">お客様は同じプランで複数のサブスクリプションを持つことができるため、これは調整ファイルの分析で重要です。</span><span class="sxs-lookup"><span data-stu-id="b84cb-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="b84cb-151">このフィールドは、パートナー管理コンソールのサブスクリプション ID にマップされます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="b84cb-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="b84cb-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="b84cb-153">OfferID</span></span></td>
<td><p><span data-ttu-id="b84cb-154">一意のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-154">Unique offer ID.</span></span> <span data-ttu-id="b84cb-155">価格表に従った標準のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="b84cb-156"><b>注</b>: この値は、価格表のプラン ID とは一致しません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="b84cb-157">以下の DurableOfferID を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b84cb-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="b84cb-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="b84cb-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="b84cb-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="b84cb-160">価格表で定義されている一意の継続的なプラン ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="b84cb-161"><b>注</b>: この値は価格表のプラン ID と一致します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="b84cb-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="b84cb-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="b84cb-163">OfferName</span></span></td>
<td><p><span data-ttu-id="b84cb-164">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="b84cb-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="b84cb-165">Microsoft Office 365 (プラン E3)</span><span class="sxs-lookup"><span data-stu-id="b84cb-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="b84cb-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="b84cb-167">サブスクリプションの開始日。注文が送信された日に設定されます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="b84cb-168">サブスクリプションの開始日を終了日と共に確認することにより、顧客がサブスクリプションの最初の 1 年以内であるか、サブスクリプションが次の 1 年間更新されたかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="b84cb-169">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b84cb-170">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b84cb-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="b84cb-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="b84cb-172">サブスクリプション終了日: 開始日から 12 か月 + x 日後 (パートナーの請求日と合わせる) または更新日から 12 か月</span><span class="sxs-lookup"><span data-stu-id="b84cb-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="b84cb-173">更新時に、価格は最新の価格表に更新されます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="b84cb-174">自動更新の前に、顧客とのやり取りが必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="b84cb-175">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b84cb-176">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b84cb-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b84cb-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b84cb-178">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="b84cb-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="b84cb-179">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="b84cb-180">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b84cb-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b84cb-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b84cb-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b84cb-183">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="b84cb-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="b84cb-184">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="b84cb-185">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="b84cb-186">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="b84cb-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="b84cb-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="b84cb-188">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="b84cb-188">The type of charge or adjustment.</span></span> <span data-ttu-id="b84cb-189">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b84cb-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="b84cb-190">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b84cb-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="b84cb-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="b84cb-192">シート単価 (購入時に価格表に公開されていた価格)。</span><span class="sxs-lookup"><span data-stu-id="b84cb-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b84cb-193">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="b84cb-194">6.82</span><span class="sxs-lookup"><span data-stu-id="b84cb-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-195">Quantity</span><span class="sxs-lookup"><span data-stu-id="b84cb-195">Quantity</span></span></td>
<td><p><span data-ttu-id="b84cb-196">シート数。</span><span class="sxs-lookup"><span data-stu-id="b84cb-196">Number of seats.</span></span> <span data-ttu-id="b84cb-197">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="b84cb-198">2</span><span class="sxs-lookup"><span data-stu-id="b84cb-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-199">Amount</span><span class="sxs-lookup"><span data-stu-id="b84cb-199">Amount</span></span></td>
<td><p><span data-ttu-id="b84cb-200">数量に対する合計価格。</span><span class="sxs-lookup"><span data-stu-id="b84cb-200">Total of price for quantity.</span></span> <span data-ttu-id="b84cb-201">金額の計算が、この顧客用の計算方法に一致することを確認するために役立ちます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="b84cb-202">13.32</span><span class="sxs-lookup"><span data-stu-id="b84cb-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="b84cb-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="b84cb-204">これらの料金に適用される割引額。</span><span class="sxs-lookup"><span data-stu-id="b84cb-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="b84cb-205">インセンティブの対象となる IUR または新しいサブスクリプションの場合も、この列に割引額が含まれます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="b84cb-206">2.32</span><span class="sxs-lookup"><span data-stu-id="b84cb-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-207">Subtotal</span><span class="sxs-lookup"><span data-stu-id="b84cb-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="b84cb-208">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="b84cb-208">Total before tax.</span></span> <span data-ttu-id="b84cb-209">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="b84cb-210">11</span><span class="sxs-lookup"><span data-stu-id="b84cb-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-211">Tax</span><span class="sxs-lookup"><span data-stu-id="b84cb-211">Tax</span></span></td>
<td><p><span data-ttu-id="b84cb-212">税金の額、market& #39; s 税関連の規則や特定の状況に基づきます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-212">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="b84cb-213">0</span><span class="sxs-lookup"><span data-stu-id="b84cb-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="b84cb-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="b84cb-215">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="b84cb-215">Total after tax.</span></span> <span data-ttu-id="b84cb-216">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="b84cb-217">11</span><span class="sxs-lookup"><span data-stu-id="b84cb-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-218">Currency</span><span class="sxs-lookup"><span data-stu-id="b84cb-218">Currency</span></span></td>
<td><p><span data-ttu-id="b84cb-219">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="b84cb-219">Currency type.</span></span> <span data-ttu-id="b84cb-220">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="b84cb-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="b84cb-221">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="b84cb-222">EUR</span><span class="sxs-lookup"><span data-stu-id="b84cb-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="b84cb-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="b84cb-224">Customer& #39; パートナー センターで報告される組織名。</span><span class="sxs-lookup"><span data-stu-id="b84cb-224">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="b84cb-225">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="b84cb-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="b84cb-226">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="b84cb-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="b84cb-227">MPNID</span></span></td>
<td><p><span data-ttu-id="b84cb-228">CSP パートナーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="b84cb-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="b84cb-229">4390934</span><span class="sxs-lookup"><span data-stu-id="b84cb-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="b84cb-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="b84cb-231">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b84cb-232">「<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">パートナーごとに明細を示す</a>」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b84cb-232">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="b84cb-233">4390934</span><span class="sxs-lookup"><span data-stu-id="b84cb-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="b84cb-234">DomainName</span></span></td>
<td><p><span data-ttu-id="b84cb-235">Customer& #39; のドメインの名前、顧客を識別するために使用します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-235">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="b84cb-236">これは、顧客/パートナーが、O365 ポータル経由でバニティ/既定のドメインを更新すると、顧客を一意に識別していない使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="b84cb-237">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="b84cb-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b84cb-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="b84cb-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="b84cb-240">サブスクリプションのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="b84cb-240">Subscription nickname.</span></span> <span data-ttu-id="b84cb-241">ニックネームが指定されていない場合、パートナー センターでは OfferName を使用します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="b84cb-242">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="b84cb-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="b84cb-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="b84cb-244">価格表で定義されている、顧客が購入したサービス プランの名前 </span><span class="sxs-lookup"><span data-stu-id="b84cb-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="b84cb-245">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="b84cb-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="b84cb-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span><span class="sxs-lookup"><span data-stu-id="b84cb-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="b84cb-247">使用量ベースのファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="b84cb-247">Usage-based file fields</span></span>


<span data-ttu-id="b84cb-248">顧客の使用量に対する料金を調整するには、調整ファイルの ResellerID/ResellerName/ResellerBillableAccount、顧客名、およびパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="b84cb-249">次のフィールドで、どのサービスが使用されるか、およびレートについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="b84cb-250">列</span><span class="sxs-lookup"><span data-stu-id="b84cb-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="b84cb-251">説明</span><span class="sxs-lookup"><span data-stu-id="b84cb-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="b84cb-252">サンプル値</span><span class="sxs-lookup"><span data-stu-id="b84cb-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="b84cb-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="b84cb-254">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="b84cb-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="b84cb-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="b84cb-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="b84cb-257">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="b84cb-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="b84cb-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="b84cb-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="b84cb-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="b84cb-260">パートナーのアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="b84cb-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="b84cb-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="b84cb-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="b84cb-263">Customer& #39; パートナー センターで報告される組織名。</span><span class="sxs-lookup"><span data-stu-id="b84cb-263">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="b84cb-264">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="b84cb-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="b84cb-265">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="b84cb-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="b84cb-266">MPNID</span></span></td>
<td><p><span data-ttu-id="b84cb-267">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="b84cb-268">4390934</span><span class="sxs-lookup"><span data-stu-id="b84cb-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="b84cb-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="b84cb-270">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b84cb-271">「<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">パートナーごとに明細を示す</a>」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b84cb-271">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="b84cb-272">4390934</span><span class="sxs-lookup"><span data-stu-id="b84cb-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="b84cb-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="b84cb-274">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="b84cb-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="b84cb-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="b84cb-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b84cb-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b84cb-277">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="b84cb-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="b84cb-278">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b84cb-279">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="b84cb-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b84cb-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b84cb-281">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="b84cb-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="b84cb-282">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="b84cb-283">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="b84cb-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="b84cb-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="b84cb-285">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b84cb-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b84cb-286">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="b84cb-287">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="b84cb-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="b84cb-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="b84cb-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="b84cb-290">サービス プランのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="b84cb-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="b84cb-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b84cb-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="b84cb-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="b84cb-293">サービス プランの基幹業務</span><span class="sxs-lookup"><span data-stu-id="b84cb-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="b84cb-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b84cb-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="b84cb-295">OrderID</span></span></td>
<td><p><span data-ttu-id="b84cb-296">Microsoft 課金プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b84cb-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="b84cb-297">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="b84cb-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="b84cb-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="b84cb-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="b84cb-300">対象の Azure サービスの名前。</span><span class="sxs-lookup"><span data-stu-id="b84cb-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="b84cb-301">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="b84cb-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="b84cb-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="b84cb-303">Windows Azure サービスの特定の種類。</span><span class="sxs-lookup"><span data-stu-id="b84cb-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="b84cb-304">Service Bus – Individual or Pack</span><span class="sxs-lookup"><span data-stu-id="b84cb-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="b84cb-305">SQL Azure database – Business or Web Edition</span><span class="sxs-lookup"><span data-stu-id="b84cb-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="b84cb-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="b84cb-307">すべてのサービス データおよび価格設定構造の特定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b84cb-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="b84cb-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="b84cb-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-309">リソース名</span><span class="sxs-lookup"><span data-stu-id="b84cb-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="b84cb-310">Azure リソースの名前。</span><span class="sxs-lookup"><span data-stu-id="b84cb-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="b84cb-311">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="b84cb-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="b84cb-312">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="b84cb-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-313">Region</span><span class="sxs-lookup"><span data-stu-id="b84cb-313">Region</span></span></td>
<td><p><span data-ttu-id="b84cb-314">使用量が適用される地域。</span><span class="sxs-lookup"><span data-stu-id="b84cb-314">The region the usage applies to.</span></span> <span data-ttu-id="b84cb-315">料金は地域によって異なるため、主にデータ転送に料金を割り当てるために使われます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="b84cb-316">Asia Pacific、Europe、Latin America、North America</span><span class="sxs-lookup"><span data-stu-id="b84cb-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-317">SKU</span><span class="sxs-lookup"><span data-stu-id="b84cb-317">SKU</span></span></td>
<td><p><span data-ttu-id="b84cb-318">プランについての MSFT の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="b84cb-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="b84cb-319">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="b84cb-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="b84cb-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="b84cb-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="b84cb-321">特定の課金期間のサービスまたはリソースに対してさまざまなレートの明細を設定するための ID と数量。</span><span class="sxs-lookup"><span data-stu-id="b84cb-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="b84cb-322">Azure の階層化されたレーティングの場合は、一定数量の課金可能単位までは 1 つのレートがあり、その後に別のレートがあることがあります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="b84cb-323">1</span><span class="sxs-lookup"><span data-stu-id="b84cb-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="b84cb-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="b84cb-325">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="b84cb-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="b84cb-326">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="b84cb-327">11</span><span class="sxs-lookup"><span data-stu-id="b84cb-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="b84cb-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="b84cb-329">単位数はプランの一部として含まれます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-329">Units included as part of the offer.</span></span> <span data-ttu-id="b84cb-330">通常、CSP には含まれません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="b84cb-331">0</span><span class="sxs-lookup"><span data-stu-id="b84cb-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="b84cb-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="b84cb-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="b84cb-333">単位数はプランの一部として含まれず、パートナーが支払う必要があります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="b84cb-334">ConsumedQuantity - IncludedQuantity と同じです。</span><span class="sxs-lookup"><span data-stu-id="b84cb-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="b84cb-335">11</span><span class="sxs-lookup"><span data-stu-id="b84cb-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="b84cb-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="b84cb-337">サブスクリプションの開始日に有効な価格を提供します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="b84cb-338">$0.0808</span><span class="sxs-lookup"><span data-stu-id="b84cb-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="b84cb-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="b84cb-340">ListPrist と OverageQuantity を掛けて、最も近いセントに丸めます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b84cb-341">$0.085</span><span class="sxs-lookup"><span data-stu-id="b84cb-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="b84cb-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="b84cb-343">税金の額、market& #39; s 税関連の規則や特定の状況に基づきます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-343">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="b84cb-344">$0.08</span><span class="sxs-lookup"><span data-stu-id="b84cb-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="b84cb-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="b84cb-346">税が適用されるときの税引き後の合計額。</span><span class="sxs-lookup"><span data-stu-id="b84cb-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="b84cb-347">$0.93</span><span class="sxs-lookup"><span data-stu-id="b84cb-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-348">Currency</span><span class="sxs-lookup"><span data-stu-id="b84cb-348">Currency</span></span></td>
<td><p><span data-ttu-id="b84cb-349">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="b84cb-349">Currency type.</span></span> <span data-ttu-id="b84cb-350">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="b84cb-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="b84cb-351">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="b84cb-352">EUR</span><span class="sxs-lookup"><span data-stu-id="b84cb-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="b84cb-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="b84cb-354">単位あたりの税込み価格。</span><span class="sxs-lookup"><span data-stu-id="b84cb-354">Pretax price per unit.</span></span> <span data-ttu-id="b84cb-355">PretaxCharges / OverageQuantity と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b84cb-356">$0.08</span><span class="sxs-lookup"><span data-stu-id="b84cb-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="b84cb-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="b84cb-358">単位あたりの税引き後の価格。</span><span class="sxs-lookup"><span data-stu-id="b84cb-358">Post tax price per unit.</span></span> <span data-ttu-id="b84cb-359">PostTaxTotal / OverageQuantity、または PretaxEffectiveRate + 単位額あたりの税率と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b84cb-360">$0.08</span><span class="sxs-lookup"><span data-stu-id="b84cb-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="b84cb-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="b84cb-362">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="b84cb-362">The type of charge or adjustment.</span></span> <span data-ttu-id="b84cb-363">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b84cb-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="b84cb-364">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b84cb-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="b84cb-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="b84cb-366">MSFT 課金プラットフォームの一意のアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="b84cb-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="b84cb-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="b84cb-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="b84cb-369">サービスの展開の日付。</span><span class="sxs-lookup"><span data-stu-id="b84cb-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="b84cb-370">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="b84cb-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="b84cb-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="b84cb-372">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="b84cb-373">East Asia、South East Asia、North Europe、West Europe、North Central US、South Central US</span><span class="sxs-lookup"><span data-stu-id="b84cb-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="b84cb-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="b84cb-375">この列は、[Service Name] 列で特に識別されない可能性のある、個別の Microsoft Azure サービスの追跡に利用されます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="b84cb-376">たとえば、データ転送は、[Service Name] 列で &quot;Microsoft Azure - All Services&quot; と報告されます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="b84cb-377">この [MeteredService] 列は、利用に関連する特定のサービスを示します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="b84cb-378">AccessControl、CDN、Compute、Database、ServiceBus、Storage</span><span class="sxs-lookup"><span data-stu-id="b84cb-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="b84cb-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="b84cb-380">個々の Microsoft Azure サービスの内容を、MeteredService フィールドで提供されるレベルよりも明確にする小見出し。</span><span class="sxs-lookup"><span data-stu-id="b84cb-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="b84cb-381">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="b84cb-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-382">Project</span><span class="sxs-lookup"><span data-stu-id="b84cb-382">Project</span></span></td>
<td><p><span data-ttu-id="b84cb-383">サービス インスタンスの顧客定義の名前</span><span class="sxs-lookup"><span data-stu-id="b84cb-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="b84cb-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="b84cb-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="b84cb-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="b84cb-386">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="b84cb-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="b84cb-387">例: 1 か月 30 日間の中に、個別にプロビジョニングされた接続がある場合、Service Info 1 は "1.000000 Connections / 30 days" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="b84cb-388">プロビジョニングされた ServiceBus 接続が 25 パックあり、その日に 1 つを利用した場合、その日の 1 日の使用量の計算書には、"25 Connections / 30 Days – Used: 1.000000" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="b84cb-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="b84cb-390">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="b84cb-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="b84cb-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b84cb-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="b84cb-392">DomainName</span></span></td>
<td><p><span data-ttu-id="b84cb-393">Customer& #39; のドメインの名前、顧客を識別するために使用します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-393">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="b84cb-394">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="b84cb-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b84cb-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="b84cb-396">Unit</span><span class="sxs-lookup"><span data-stu-id="b84cb-396">Unit</span></span></td>
<td><p><span data-ttu-id="b84cb-397">リソース名の単位</span><span class="sxs-lookup"><span data-stu-id="b84cb-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="b84cb-398">GB または HOURS</span><span class="sxs-lookup"><span data-stu-id="b84cb-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="b84cb-399">1 回限りと定期的なファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="b84cb-399">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b84cb-400">列</span><span class="sxs-lookup"><span data-stu-id="b84cb-400">Column</span></span></th>
<th><span data-ttu-id="b84cb-401">説明</span><span class="sxs-lookup"><span data-stu-id="b84cb-401">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="b84cb-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="b84cb-402">PartnerId</span></span></td>
<td><p><span data-ttu-id="b84cb-403">GUID 形式の特定の課金エンティティの一意の Microsoft Azure Active Directory テナント識別子です。</span><span class="sxs-lookup"><span data-stu-id="b84cb-403">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="b84cb-404">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-404">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="b84cb-405">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="b84cb-405">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-406">顧客 Id</span><span class="sxs-lookup"><span data-stu-id="b84cb-406">Customer Id</span></span></td>
<td><p><span data-ttu-id="b84cb-407">一意な Microsoft Azure Active Directory テナント ID、GUID 形式、顧客を識別するために使用します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-407">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-408">顧客名</span><span class="sxs-lookup"><span data-stu-id="b84cb-408">Customer Name</span></span></td>
<td><p><span data-ttu-id="b84cb-409">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="b84cb-409">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="b84cb-410">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="b84cb-411">顧客のドメイン名。顧客を特定できるようにするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-411">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="b84cb-412">これは、顧客/パートナーが、O365 ポータル経由でバニティ/既定のドメインを更新すると、顧客を一意に識別していない使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-412">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="b84cb-413">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-413">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-414">顧客の国</span><span class="sxs-lookup"><span data-stu-id="b84cb-414">Customer Country</span></span></td>
<td><p><span data-ttu-id="b84cb-415">顧客の在住国。</span><span class="sxs-lookup"><span data-stu-id="b84cb-415">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-416">請求書番号</span><span class="sxs-lookup"><span data-stu-id="b84cb-416">Invoice number</span></span></td>
<td><p><span data-ttu-id="b84cb-417">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="b84cb-417">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-418">MpnId</span><span class="sxs-lookup"><span data-stu-id="b84cb-418">MpnId</span></span></td>
<td><p><span data-ttu-id="b84cb-419">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-419">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-420">リセラー MpnId</span><span class="sxs-lookup"><span data-stu-id="b84cb-420">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="b84cb-421">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-421">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-422">注文 ID</span><span class="sxs-lookup"><span data-stu-id="b84cb-422">Order ID</span></span></td>
<td><p><span data-ttu-id="b84cb-423">Microsoft のコマース プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b84cb-423">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="b84cb-424">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-424">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-425">発注日</span><span class="sxs-lookup"><span data-stu-id="b84cb-425">Order date</span></span></td>
<td><p><span data-ttu-id="b84cb-426">注文が作成された日付。</span><span class="sxs-lookup"><span data-stu-id="b84cb-426">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-427">ProductId</span><span class="sxs-lookup"><span data-stu-id="b84cb-427">ProductId</span></span></td>
<td><p><span data-ttu-id="b84cb-428">製品の ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-428">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-429">SkuId</span><span class="sxs-lookup"><span data-stu-id="b84cb-429">SkuId</span></span></td>
<td><p><span data-ttu-id="b84cb-430">特定 SKU の ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-430">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-431">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="b84cb-431">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="b84cb-432">特定の可用性 の ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-432">The ID for a particular Availability.</span></span> <span data-ttu-id="b84cb-433">"可用性" とは、特定の国、通貨、業界などで特定の SKU を購入可能かどうかを指します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-433">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-434">SKU の名前</span><span class="sxs-lookup"><span data-stu-id="b84cb-434">SKU Name</span></span></td>
<td><p><span data-ttu-id="b84cb-435">特定 SKU のタイトル。</span><span class="sxs-lookup"><span data-stu-id="b84cb-435">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-436">Product name (製品名)</span><span class="sxs-lookup"><span data-stu-id="b84cb-436">Product name</span></span></td>
<td><p><span data-ttu-id="b84cb-437">製品の名前。</span><span class="sxs-lookup"><span data-stu-id="b84cb-437">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-438">PublisherName</span><span class="sxs-lookup"><span data-stu-id="b84cb-438">PublisherName</span></span></td>
<td><p><span data-ttu-id="b84cb-439">製品の発行元の名前。</span><span class="sxs-lookup"><span data-stu-id="b84cb-439">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-440">PublisherID</span><span class="sxs-lookup"><span data-stu-id="b84cb-440">PublisherID</span></span></td>
<td><p><span data-ttu-id="b84cb-441">この発行者の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-441">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-442">サブスクリプションの説明</span><span class="sxs-lookup"><span data-stu-id="b84cb-442">Subscription Description</span></span></td>
<td><p><span data-ttu-id="b84cb-443">サブスクリプションのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="b84cb-443">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-444">サブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="b84cb-444">Subscription ID</span></span></td>
<td><p><span data-ttu-id="b84cb-445">Microsoft のコマース プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b84cb-445">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="b84cb-446">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-446">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="b84cb-447">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-447">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-448">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b84cb-448">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b84cb-449">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="b84cb-449">Start day of the charges.</span></span> <span data-ttu-id="b84cb-450">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-450">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-451">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b84cb-451">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b84cb-452">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="b84cb-452">End day of the charges.</span></span> <span data-ttu-id="b84cb-453">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-453">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-454">用語と Billingcycle</span><span class="sxs-lookup"><span data-stu-id="b84cb-454">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="b84cb-455">期間の長さと、その購入に対する請求サイクルします。</span><span class="sxs-lookup"><span data-stu-id="b84cb-455">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="b84cb-456">たとえば、「1 年、月単位。」</span><span class="sxs-lookup"><span data-stu-id="b84cb-456">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-457">請求の種類</span><span class="sxs-lookup"><span data-stu-id="b84cb-457">Charge Type</span></span></td>
<td><p><span data-ttu-id="b84cb-458">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="b84cb-458">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-459">単価</span><span class="sxs-lookup"><span data-stu-id="b84cb-459">Unit Price</span></span></td>
<td><p><span data-ttu-id="b84cb-460">購入時に価格で公開されると価格です。</span><span class="sxs-lookup"><span data-stu-id="b84cb-460">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b84cb-461">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-461">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-462">効果的な単価</span><span class="sxs-lookup"><span data-stu-id="b84cb-462">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="b84cb-463">単価調整が行われた後。</span><span class="sxs-lookup"><span data-stu-id="b84cb-463">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-464">数量</span><span class="sxs-lookup"><span data-stu-id="b84cb-464">Quantity</span></span></td>
<td><p><span data-ttu-id="b84cb-465">単位数。</span><span class="sxs-lookup"><span data-stu-id="b84cb-465">Number of units.</span></span> <span data-ttu-id="b84cb-466">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-466">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-467">ユニットの種類</span><span class="sxs-lookup"><span data-stu-id="b84cb-467">Unit type</span></span></td>
<td><p><span data-ttu-id="b84cb-468">購入単位の種類。</span><span class="sxs-lookup"><span data-stu-id="b84cb-468">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-469">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="b84cb-469">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="b84cb-470">適用される割引について説明します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-470">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-471">サブ合計</span><span class="sxs-lookup"><span data-stu-id="b84cb-471">Sub Total</span></span></td>
<td><p><span data-ttu-id="b84cb-472">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="b84cb-472">Total before tax.</span></span> <span data-ttu-id="b84cb-473">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-473">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-474">税の合計</span><span class="sxs-lookup"><span data-stu-id="b84cb-474">Tax Total</span></span></td>
<td><p><span data-ttu-id="b84cb-475">市場の税関連の規則や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="b84cb-475">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-476">Total</span><span class="sxs-lookup"><span data-stu-id="b84cb-476">Total</span></span></td>
<td><p><span data-ttu-id="b84cb-477">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="b84cb-477">Total after tax.</span></span> <span data-ttu-id="b84cb-478">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-478">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-479">Currency</span><span class="sxs-lookup"><span data-stu-id="b84cb-479">Currency</span></span></td>
<td><p><span data-ttu-id="b84cb-480">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="b84cb-480">Currency type.</span></span> <span data-ttu-id="b84cb-481">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="b84cb-481">Each billing entity has only one currency.</span></span> <span data-ttu-id="b84cb-482">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-482">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-483">AlternateID</span><span class="sxs-lookup"><span data-stu-id="b84cb-483">AlternateID</span></span></td>
<td><p><span data-ttu-id="b84cb-484">代替の識別子を ID</span><span class="sxs-lookup"><span data-stu-id="b84cb-484">An alternate identifier to an ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="b84cb-485">毎日日割りの使用状況ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="b84cb-485">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b84cb-486">列</span><span class="sxs-lookup"><span data-stu-id="b84cb-486">Column</span></span></th>
<th><span data-ttu-id="b84cb-487">説明</span><span class="sxs-lookup"><span data-stu-id="b84cb-487">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="b84cb-488">PartnerId</span><span class="sxs-lookup"><span data-stu-id="b84cb-488">PartnerId</span></span></td>
<td><p><span data-ttu-id="b84cb-489">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-489">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-490">PartnerName</span><span class="sxs-lookup"><span data-stu-id="b84cb-490">PartnerName</span></span></td>
<td><p><span data-ttu-id="b84cb-491">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="b84cb-491">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-492">CustomerId</span><span class="sxs-lookup"><span data-stu-id="b84cb-492">CustomerId</span></span></td>
<td><p><span data-ttu-id="b84cb-493">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-493">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-494">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="b84cb-494">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="b84cb-495">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="b84cb-495">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="b84cb-496">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="b84cb-496">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-497">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="b84cb-497">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="b84cb-498">顧客のドメイン名。</span><span class="sxs-lookup"><span data-stu-id="b84cb-498">The customer’s domain name.</span></span> <span data-ttu-id="b84cb-499">現在のアクティビティは利用できません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-499">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-500">顧客の国</span><span class="sxs-lookup"><span data-stu-id="b84cb-500">Customer country</span></span></td>
<td><p><span data-ttu-id="b84cb-501">顧客の在住国。</span><span class="sxs-lookup"><span data-stu-id="b84cb-501">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-502">MPNID</span><span class="sxs-lookup"><span data-stu-id="b84cb-502">MPNID</span></span></td>
<td><p><span data-ttu-id="b84cb-503">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-503">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-504">リセラー MPNID</span><span class="sxs-lookup"><span data-stu-id="b84cb-504">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="b84cb-505">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-505">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b84cb-506">現在のアクティビティは利用できません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-506">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-507">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="b84cb-507">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="b84cb-508">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="b84cb-508">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="b84cb-509">現在のアクティビティは利用できません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-509">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-510">ProductId</span><span class="sxs-lookup"><span data-stu-id="b84cb-510">ProductId</span></span></td>
<td><p><span data-ttu-id="b84cb-511">製品の ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-511">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-512">SkuId</span><span class="sxs-lookup"><span data-stu-id="b84cb-512">SkuId</span></span></td>
<td><p><span data-ttu-id="b84cb-513">特定 SKU の ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-513">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-514">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="b84cb-514">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="b84cb-515">特定の可用性 の ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-515">The ID for a particular Availability.</span></span> <span data-ttu-id="b84cb-516">"可用性" とは、特定の国、通貨、業界などで特定の SKU を購入可能かどうかを指します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-516">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-517">SKU の名前</span><span class="sxs-lookup"><span data-stu-id="b84cb-517">SKU Name</span></span></td>
<td><p><span data-ttu-id="b84cb-518">特定 SKU のタイトル。</span><span class="sxs-lookup"><span data-stu-id="b84cb-518">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-519">PublisherName</span><span class="sxs-lookup"><span data-stu-id="b84cb-519">PublisherName</span></span></td>
<td><p><span data-ttu-id="b84cb-520">発行元の名前です。</span><span class="sxs-lookup"><span data-stu-id="b84cb-520">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-521">PublisherID</span><span class="sxs-lookup"><span data-stu-id="b84cb-521">PublisherID</span></span></td>
<td><p><span data-ttu-id="b84cb-522">発行元は、GUID 形式の ID です。</span><span class="sxs-lookup"><span data-stu-id="b84cb-522">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="b84cb-523">現在のアクティビティは利用できません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="b84cb-524">サブスクリプションの説明</span><span class="sxs-lookup"><span data-stu-id="b84cb-524">Subscription Description</span></span></td>
<td><p><span data-ttu-id="b84cb-525">価格表で定義されている、顧客が購入したサービス プランの名前 </span><span class="sxs-lookup"><span data-stu-id="b84cb-525">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="b84cb-526">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="b84cb-526">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-527">サブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="b84cb-527">Subscription ID</span></span></td>
<td><p><span data-ttu-id="b84cb-528">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b84cb-528">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b84cb-529">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-529">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="b84cb-530">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-530">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-531">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b84cb-531">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b84cb-532">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="b84cb-532">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="b84cb-533">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-533">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-534">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b84cb-534">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b84cb-535">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="b84cb-535">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="b84cb-536">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="b84cb-536">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-537">使用日</span><span class="sxs-lookup"><span data-stu-id="b84cb-537">Usage Date</span></span></td>
<td><p><span data-ttu-id="b84cb-538">サービスの使用状況の日付です。</span><span class="sxs-lookup"><span data-stu-id="b84cb-538">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-539">計の種類</span><span class="sxs-lookup"><span data-stu-id="b84cb-539">Meter Type</span></span></td>
<td><p><span data-ttu-id="b84cb-540">メーターの種類です。</span><span class="sxs-lookup"><span data-stu-id="b84cb-540">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-541">メーター カテゴリ</span><span class="sxs-lookup"><span data-stu-id="b84cb-541">Meter Category</span></span></td>
<td><p><span data-ttu-id="b84cb-542">使用率の最上位レベルのサービスです。</span><span class="sxs-lookup"><span data-stu-id="b84cb-542">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-543">メーター Id</span><span class="sxs-lookup"><span data-stu-id="b84cb-543">Meter Id</span></span></td>
<td><p><span data-ttu-id="b84cb-544">使用されているメーターの ID。</span><span class="sxs-lookup"><span data-stu-id="b84cb-544">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-545">メーター サブ カテゴリ</span><span class="sxs-lookup"><span data-stu-id="b84cb-545">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="b84cb-546">レートに影響を与える Azure サービスの種類です。</span><span class="sxs-lookup"><span data-stu-id="b84cb-546">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-547">メーター名</span><span class="sxs-lookup"><span data-stu-id="b84cb-547">Meter Name</span></span></td>
<td><p><span data-ttu-id="b84cb-548">消費されるメーター計測単位です。</span><span class="sxs-lookup"><span data-stu-id="b84cb-548">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-549">メーター地域</span><span class="sxs-lookup"><span data-stu-id="b84cb-549">Meter Region</span></span></td>
<td><p><span data-ttu-id="b84cb-550">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-550">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-551">Unit</span><span class="sxs-lookup"><span data-stu-id="b84cb-551">Unit</span></span></td>
<td><p><span data-ttu-id="b84cb-552">リソース名の単位です。</span><span class="sxs-lookup"><span data-stu-id="b84cb-552">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-553">消費数量</span><span class="sxs-lookup"><span data-stu-id="b84cb-553">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="b84cb-554">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="b84cb-554">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="b84cb-555">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-555">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-556">リソースの場所</span><span class="sxs-lookup"><span data-stu-id="b84cb-556">Resource Location</span></span></td>
<td><p><span data-ttu-id="b84cb-557">メーターが実行されているデータ センターです。</span><span class="sxs-lookup"><span data-stu-id="b84cb-557">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-558">サービスの盗用</span><span class="sxs-lookup"><span data-stu-id="b84cb-558">Consumed Service</span></span></td>
<td><p><span data-ttu-id="b84cb-559">使用して、Azure プラットフォーム サービスです。</span><span class="sxs-lookup"><span data-stu-id="b84cb-559">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-560">リソース グループ</span><span class="sxs-lookup"><span data-stu-id="b84cb-560">Resource Group</span></span></td>
<td><p><span data-ttu-id="b84cb-561">展開されたメーターが実行されているリソース グループです。</span><span class="sxs-lookup"><span data-stu-id="b84cb-561">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-562">リソース URI</span><span class="sxs-lookup"><span data-stu-id="b84cb-562">Resource URI</span></span></td>
<td><p><span data-ttu-id="b84cb-563">使用されているリソースの URI。</span><span class="sxs-lookup"><span data-stu-id="b84cb-563">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-564">請求の種類</span><span class="sxs-lookup"><span data-stu-id="b84cb-564">Charge type</span></span></td>
<td><p><span data-ttu-id="b84cb-565">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="b84cb-565">The type of charge or adjustment.</span></span> <span data-ttu-id="b84cb-566">現在のアクティビティは利用できません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-566">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-567">単価</span><span class="sxs-lookup"><span data-stu-id="b84cb-567">Unit price</span></span></td>
<td><p><span data-ttu-id="b84cb-568">購入時に価格で公開されると、ライセンスあたりの価格。</span><span class="sxs-lookup"><span data-stu-id="b84cb-568">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b84cb-569">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-569">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-570">数量</span><span class="sxs-lookup"><span data-stu-id="b84cb-570">Quantity</span></span></td>
<td><p><span data-ttu-id="b84cb-571">ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="b84cb-571">Number of licenses.</span></span> <span data-ttu-id="b84cb-572">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-572">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-573">ユニットの種類</span><span class="sxs-lookup"><span data-stu-id="b84cb-573">Unit type</span></span></td>
<td><p><span data-ttu-id="b84cb-574">メーターが充電ユニットの種類です。</span><span class="sxs-lookup"><span data-stu-id="b84cb-574">The type of unit the meter is charged in.</span></span> <span data-ttu-id="b84cb-575">現在のアクティビティは利用できません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-575">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-576">前の税金を請求</span><span class="sxs-lookup"><span data-stu-id="b84cb-576">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="b84cb-577">税金の前に合計金額。</span><span class="sxs-lookup"><span data-stu-id="b84cb-577">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-578">請求通貨</span><span class="sxs-lookup"><span data-stu-id="b84cb-578">Billing currency</span></span></td>
<td><p><span data-ttu-id="b84cb-579">顧客の地理的な地域の通貨</span><span class="sxs-lookup"><span data-stu-id="b84cb-579">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-580">価格の税込みの合計</span><span class="sxs-lookup"><span data-stu-id="b84cb-580">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="b84cb-581">価格の税金が追加される前にします。</span><span class="sxs-lookup"><span data-stu-id="b84cb-581">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-582">通貨の価格</span><span class="sxs-lookup"><span data-stu-id="b84cb-582">Pricing currency</span></span></td>
<td><p><span data-ttu-id="b84cb-583">価格表に使われた通貨。</span><span class="sxs-lookup"><span data-stu-id="b84cb-583">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-584">サービスは 1</span><span class="sxs-lookup"><span data-stu-id="b84cb-584">Service Info 1</span></span></td>
<td><p><span data-ttu-id="b84cb-585">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="b84cb-585">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-586">サービスは 2</span><span class="sxs-lookup"><span data-stu-id="b84cb-586">Service Info 2</span></span></td>
<td><p><span data-ttu-id="b84cb-587">省略可能なサービスに固有のメタデータをキャプチャする従来のフィールドです。</span><span class="sxs-lookup"><span data-stu-id="b84cb-587">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b84cb-588">タグ</span><span class="sxs-lookup"><span data-stu-id="b84cb-588">Tags</span></span></td>
<td><p><span data-ttu-id="b84cb-589">請求レコードをグループ化するために、メーターに割り当てるタグ。</span><span class="sxs-lookup"><span data-stu-id="b84cb-589">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="b84cb-590">たとえば、メーターを使用する部門によってコストを配布するのにタグを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-590">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b84cb-591">追加情報</span><span class="sxs-lookup"><span data-stu-id="b84cb-591">Additional Info</span></span></td>
<td><p><span data-ttu-id="b84cb-592">その他の情報の他の列では説明しません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-592">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="b84cb-593">請求書と調整ファイルの間の課金のマッピング</span><span class="sxs-lookup"><span data-stu-id="b84cb-593">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="b84cb-594">請求書は料金の概要を示し、調整ファイルは、課金の種類を含め、行項目のトランザクションの詳細な内訳を示します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-594">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="b84cb-595">請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルター オプションを使用して、調整ファイルの課金の種類でフィルター処理し、請求書の課金を調整ファイルの一連の課金の内訳にマップします。</span><span class="sxs-lookup"><span data-stu-id="b84cb-595">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="b84cb-596">使用量ベースとライセンス ベースの調整ファイルには、使用量関連のトランザクションと料金 (消費された単位量および関連する料金) のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-596">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="b84cb-597">請求書に “調整” として表示される単発のクレジット、割引、払い戻し金額は、調整ファイルに表示されません。</span><span class="sxs-lookup"><span data-stu-id="b84cb-597">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="b84cb-598">次の表に、請求書のセクションと、調整ファイルに表示される関連付けられた課金の種類とのマッピングを示します。</span><span class="sxs-lookup"><span data-stu-id="b84cb-598">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="b84cb-599">請求書の課金の説明</span><span class="sxs-lookup"><span data-stu-id="b84cb-599">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="b84cb-600">調整ファイルの課金の説明 (ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="b84cb-600">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="b84cb-601">この課金の意味</span><span class="sxs-lookup"><span data-stu-id="b84cb-601">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="b84cb-602">これらの ChargeTypes を請求書にマップする方法</span><span class="sxs-lookup"><span data-stu-id="b84cb-602">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="b84cb-603">ライセンス ベースの課金</span><span class="sxs-lookup"><span data-stu-id="b84cb-603">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b84cb-604">Activation fee</span><span class="sxs-lookup"><span data-stu-id="b84cb-604">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-605">購入したサブスクリプションを顧客が使用したときに顧客に課金される金額</span><span class="sxs-lookup"><span data-stu-id="b84cb-605">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="b84cb-606">ライセンスベースのファイルから、<strong>Amount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b84cb-606">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b84cb-607">取り消し料金</span><span class="sxs-lookup"><span data-stu-id="b84cb-607">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-608">関連付けられているシートが変更されたときに顧客に払い戻される日割り料金</span><span class="sxs-lookup"><span data-stu-id="b84cb-608">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b84cb-609">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="b84cb-609">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-610">サブスクリプションの定期的な課金</span><span class="sxs-lookup"><span data-stu-id="b84cb-610">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b84cb-611">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="b84cb-611">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-612">関連付けられているシートが変更されたときに顧客から評価される日割り料金</span><span class="sxs-lookup"><span data-stu-id="b84cb-612">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b84cb-613">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="b84cb-613">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-614">取り消し時のサービスの未使用部分に対する日割りの払戻し額</span><span class="sxs-lookup"><span data-stu-id="b84cb-614">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b84cb-615">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="b84cb-615">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-616">年次請求を使用する場合、サブスクリプションの請求の種類</span><span class="sxs-lookup"><span data-stu-id="b84cb-616">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b84cb-617">Purchase fee</span><span class="sxs-lookup"><span data-stu-id="b84cb-617">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-618">月次請求を使用する場合、サブスクリプションの請求の種類</span><span class="sxs-lookup"><span data-stu-id="b84cb-618">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b84cb-619">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="b84cb-619">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-620">サブスクリプションの更新時の日割り料金</span><span class="sxs-lookup"><span data-stu-id="b84cb-620">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="b84cb-621">Renew fee</span><span class="sxs-lookup"><span data-stu-id="b84cb-621">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-622">サブスクリプションの更新時の課金</span><span class="sxs-lookup"><span data-stu-id="b84cb-622">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b84cb-623">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="b84cb-623">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-624">アクティブ化から課金期間の終了までの日割り料金</span><span class="sxs-lookup"><span data-stu-id="b84cb-624">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="b84cb-625">利用料金</span><span class="sxs-lookup"><span data-stu-id="b84cb-625">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b84cb-626">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="b84cb-626">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-627">現在の課金期間中に未払いの使用を取り消したときのアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="b84cb-627">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="b84cb-628">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b84cb-628">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b84cb-629">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="b84cb-629">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-630">現在の課金期間のアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="b84cb-630">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="b84cb-631">クレジット</span><span class="sxs-lookup"><span data-stu-id="b84cb-631">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b84cb-632">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="b84cb-632">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-633">税金を含む、行項目への一部または全部の払戻し</span><span class="sxs-lookup"><span data-stu-id="b84cb-633">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-634">ライセンス ベースのファイルから、<strong>TotalForCustomer</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b84cb-634">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="b84cb-635">使用量ベースのファイルから、<strong>PostTaxTotal</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b84cb-635">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="b84cb-636">使用量ベースの割引</span><span class="sxs-lookup"><span data-stu-id="b84cb-636">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b84cb-637">Activation discount</span><span class="sxs-lookup"><span data-stu-id="b84cb-637">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-638">サブスクリプションがアクティブ化されたときに適用される割引</span><span class="sxs-lookup"><span data-stu-id="b84cb-638">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="b84cb-639">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b84cb-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b84cb-640">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="b84cb-640">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-641">定期的な課金に適用される割引</span><span class="sxs-lookup"><span data-stu-id="b84cb-641">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b84cb-642">Renew discount</span><span class="sxs-lookup"><span data-stu-id="b84cb-642">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-643">サブスクリプションの更新時に適用される割引</span><span class="sxs-lookup"><span data-stu-id="b84cb-643">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b84cb-644">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="b84cb-644">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-645">割引が取り消されたときに適用される料金</span><span class="sxs-lookup"><span data-stu-id="b84cb-645">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="b84cb-646">ライセンス ベースの割引</span><span class="sxs-lookup"><span data-stu-id="b84cb-646">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="b84cb-647">複数の種類の料金に適用される場合がある</span><span class="sxs-lookup"><span data-stu-id="b84cb-647">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="b84cb-648">ライセンス ベースのファイルから、<strong>TotalOtherDiscount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b84cb-648">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b84cb-649"><strong>税</strong>&nbsp;または&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="b84cb-649"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="b84cb-650">複数の種類の料金に適用される場合がある</span><span class="sxs-lookup"><span data-stu-id="b84cb-650">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="b84cb-651">例外:&quot;行項目のオフセット&quot;既に税が含まれます。</span><span class="sxs-lookup"><span data-stu-id="b84cb-651">Exception: &quot;Offset a line item&quot; already includes taxes.</span></span> <span data-ttu-id="b84cb-652">上記のクレジットを参照してください。</span><span class="sxs-lookup"><span data-stu-id="b84cb-652">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="b84cb-653">税または付加価値税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="b84cb-653">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="b84cb-654">ライセンス ベースのファイルから、<strong>Tax</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b84cb-654">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="b84cb-655">使用量ベースのファイルから、<strong>TaxAmount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b84cb-655">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
