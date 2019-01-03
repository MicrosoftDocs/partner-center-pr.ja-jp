---
title: 調整ファイルを使う | パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: 請求サイクルの各料金の詳しい行項目ビューのためには、パートナー センターから、調整ファイルをダウンロードします。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.localizationpriority: medium
ms.openlocfilehash: 50af14ab0e8edf6cd4576be6615cd7238b23bd99
ms.sourcegitcommit: 9ea2f05f938ea22251f3719b61f03ccb71d3494f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/03/2019
ms.locfileid: "8990994"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="20a8a-103">調整ファイルを使う</span><span class="sxs-lookup"><span data-stu-id="20a8a-103">Use the reconciliation files</span></span>

**<span data-ttu-id="20a8a-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="20a8a-104">Applies to</span></span>**

-  <span data-ttu-id="20a8a-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="20a8a-105">Partner Center</span></span>
-  <span data-ttu-id="20a8a-106">Microsoft Cloud for US Government のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="20a8a-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="20a8a-107">請求サイクルの各料金の詳しい行項目ビューのためには、パートナー センターから、調整ファイルをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="20a8a-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="20a8a-108">詳細には、各顧客のサブスクリプションの料金や、詳細なイベント (期間途中でのサブスクリプションへのシートの追加など) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="20a8a-109">パートナーごとに明細を示す</span><span class="sxs-lookup"><span data-stu-id="20a8a-109">Itemize by partner</span></span>


<span data-ttu-id="20a8a-110">インダイレクト モデルのパートナーは、ライセンス ベースの調整ファイルと使用量ベースの調整ファイルの両方で、これらの追加フィールドを使用してリセラーごとに明細を記載できます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="20a8a-111">MPN ID</span><span class="sxs-lookup"><span data-stu-id="20a8a-111">MPN ID</span></span></th>
<th><span data-ttu-id="20a8a-112">説明</span><span class="sxs-lookup"><span data-stu-id="20a8a-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="20a8a-113">MPN ID</span><span class="sxs-lookup"><span data-stu-id="20a8a-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="20a8a-114">CSP パートナー (直接または間接) の Microsoft Partner Network (MPN) IDです。</span><span class="sxs-lookup"><span data-stu-id="20a8a-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-115">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="20a8a-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="20a8a-116">インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="20a8a-117">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="20a8a-118">これは、パートナー センターで特定のサブスクリプションについて示されるリセラー ID に対応します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="20a8a-119">リセラーを表示または更新プログラム、パートナー センター メニューから、リセラーは、<strong>顧客</strong>を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="20a8a-120">顧客メニューの <strong>[サブスクリプション]</strong> を選び、一覧からサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="20a8a-121">
          <strong>[更新]</strong> を選んで、<strong>[再販業者 (MPN ID)]</strong> を変更します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="20a8a-122">CSP パートナーがお客様に直接サブスクリプションを販売した場合、パートナーの MPN ID が MPN ID とリセラーの MPN ID として 2 か所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="20a8a-123">CSP パートナーのリセラーに MPN ID がない場合は、代わりに CSP パートナーの MPN ID がこの値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="20a8a-124">CSP パートナーがリセラー ID を削除した場合、この値は -1 に設定されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="20a8a-125">ライセンス ベースのファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="20a8a-125">License-based file fields</span></span>


<span data-ttu-id="20a8a-126">顧客の注文に対する料金を調整するには、調整ファイルの Syndication\_Partner\_Subscription\_Number とパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="20a8a-127">列</span><span class="sxs-lookup"><span data-stu-id="20a8a-127">Column</span></span></strong></td>
<td><strong><span data-ttu-id="20a8a-128">説明</span><span class="sxs-lookup"><span data-stu-id="20a8a-128">Description</span></span></strong></td>
<td><strong><span data-ttu-id="20a8a-129">サンプル値</span><span class="sxs-lookup"><span data-stu-id="20a8a-129">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="20a8a-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="20a8a-131">特定の課金エンティティの一意の識別子 (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="20a8a-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="20a8a-132">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="20a8a-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="20a8a-133">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="20a8a-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="20a8a-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="20a8a-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="20a8a-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="20a8a-136">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="20a8a-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="20a8a-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="20a8a-138">OrderID</span></span></td>
<td><p><span data-ttu-id="20a8a-139">Microsoft 課金プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20a8a-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="20a8a-140">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="20a8a-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="20a8a-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="20a8a-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="20a8a-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="20a8a-143">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20a8a-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="20a8a-144">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="20a8a-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="20a8a-145">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="20a8a-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="20a8a-146">「Syndication_Partner_Subscription_Number」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="20a8a-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="20a8a-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="20a8a-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="20a8a-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="20a8a-149">サブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20a8a-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="20a8a-150">お客様は同じプランで複数のサブスクリプションを持つことができるため、これは調整ファイルの分析で重要です。</span><span class="sxs-lookup"><span data-stu-id="20a8a-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="20a8a-151">このフィールドは、パートナー管理コンソールのサブスクリプション ID にマップされます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="20a8a-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="20a8a-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="20a8a-153">OfferID</span></span></td>
<td><p><span data-ttu-id="20a8a-154">一意のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-154">Unique offer ID.</span></span> <span data-ttu-id="20a8a-155">価格表に従った標準のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="20a8a-156"><b>注</b>: この値は、価格表のプラン ID とは一致しません。</span><span class="sxs-lookup"><span data-stu-id="20a8a-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="20a8a-157">以下の DurableOfferID を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20a8a-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="20a8a-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="20a8a-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="20a8a-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="20a8a-160">価格表で定義されている一意の継続的なプラン ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="20a8a-161"><b>注</b>: この値は価格表のプラン ID と一致します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="20a8a-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="20a8a-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="20a8a-163">OfferName</span></span></td>
<td><p><span data-ttu-id="20a8a-164">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="20a8a-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="20a8a-165">Microsoft Office 365 (プラン E3)</span><span class="sxs-lookup"><span data-stu-id="20a8a-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="20a8a-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="20a8a-167">サブスクリプションの開始日。注文が送信された日に設定されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="20a8a-168">サブスクリプションの開始日を終了日と共に確認することにより、顧客がサブスクリプションの最初の 1 年以内であるか、サブスクリプションが次の 1 年間更新されたかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="20a8a-169">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="20a8a-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20a8a-170">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="20a8a-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="20a8a-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="20a8a-172">サブスクリプション終了日: 開始日から 12 か月 + x 日後 (パートナーの請求日と合わせる) または更新日から 12 か月</span><span class="sxs-lookup"><span data-stu-id="20a8a-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="20a8a-173">更新時に、価格は最新の価格表に更新されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="20a8a-174">自動更新の前に、顧客とのやり取りが必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="20a8a-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="20a8a-175">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="20a8a-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20a8a-176">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="20a8a-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="20a8a-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="20a8a-178">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="20a8a-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="20a8a-179">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="20a8a-180">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="20a8a-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20a8a-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="20a8a-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="20a8a-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="20a8a-183">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="20a8a-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="20a8a-184">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="20a8a-185">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="20a8a-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="20a8a-186">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="20a8a-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="20a8a-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="20a8a-188">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="20a8a-188">The type of charge or adjustment.</span></span> <span data-ttu-id="20a8a-189">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20a8a-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="20a8a-190">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20a8a-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="20a8a-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="20a8a-192">シート単価 (購入時に価格表に公開されていた価格)。</span><span class="sxs-lookup"><span data-stu-id="20a8a-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="20a8a-193">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="20a8a-194">6.82</span><span class="sxs-lookup"><span data-stu-id="20a8a-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-195">Quantity</span><span class="sxs-lookup"><span data-stu-id="20a8a-195">Quantity</span></span></td>
<td><p><span data-ttu-id="20a8a-196">シート数。</span><span class="sxs-lookup"><span data-stu-id="20a8a-196">Number of seats.</span></span> <span data-ttu-id="20a8a-197">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="20a8a-198">2</span><span class="sxs-lookup"><span data-stu-id="20a8a-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-199">Amount</span><span class="sxs-lookup"><span data-stu-id="20a8a-199">Amount</span></span></td>
<td><p><span data-ttu-id="20a8a-200">数量に対する合計価格。</span><span class="sxs-lookup"><span data-stu-id="20a8a-200">Total of price for quantity.</span></span> <span data-ttu-id="20a8a-201">金額の計算が、この顧客用の計算方法に一致することを確認するために役立ちます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="20a8a-202">13.32</span><span class="sxs-lookup"><span data-stu-id="20a8a-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="20a8a-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="20a8a-204">これらの料金に適用される割引額。</span><span class="sxs-lookup"><span data-stu-id="20a8a-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="20a8a-205">インセンティブの対象となる IUR または新しいサブスクリプションの場合も、この列に割引額が含まれます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="20a8a-206">2.32</span><span class="sxs-lookup"><span data-stu-id="20a8a-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-207">Subtotal</span><span class="sxs-lookup"><span data-stu-id="20a8a-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="20a8a-208">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="20a8a-208">Total before tax.</span></span> <span data-ttu-id="20a8a-209">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="20a8a-210">11</span><span class="sxs-lookup"><span data-stu-id="20a8a-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-211">Tax</span><span class="sxs-lookup"><span data-stu-id="20a8a-211">Tax</span></span></td>
<td><p><span data-ttu-id="20a8a-212">市場の税関連の規則や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="20a8a-212">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="20a8a-213">0</span><span class="sxs-lookup"><span data-stu-id="20a8a-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="20a8a-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="20a8a-215">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="20a8a-215">Total after tax.</span></span> <span data-ttu-id="20a8a-216">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="20a8a-217">11</span><span class="sxs-lookup"><span data-stu-id="20a8a-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-218">Currency</span><span class="sxs-lookup"><span data-stu-id="20a8a-218">Currency</span></span></td>
<td><p><span data-ttu-id="20a8a-219">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="20a8a-219">Currency type.</span></span> <span data-ttu-id="20a8a-220">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="20a8a-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="20a8a-221">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="20a8a-222">EUR</span><span class="sxs-lookup"><span data-stu-id="20a8a-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="20a8a-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="20a8a-224">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="20a8a-224">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="20a8a-225">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="20a8a-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="20a8a-226">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="20a8a-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="20a8a-227">MPNID</span></span></td>
<td><p><span data-ttu-id="20a8a-228">CSP パートナーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="20a8a-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="20a8a-229">4390934</span><span class="sxs-lookup"><span data-stu-id="20a8a-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="20a8a-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="20a8a-231">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="20a8a-232">「[パートナーごとに明細を示す](#itemizebypartner)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="20a8a-232">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="20a8a-233">4390934</span><span class="sxs-lookup"><span data-stu-id="20a8a-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="20a8a-234">DomainName</span></span></td>
<td><p><span data-ttu-id="20a8a-235">顧客のドメイン名。顧客を特定できるようにするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-235">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="20a8a-236">これは、顧客/パートナーが、O365 ポータル経由でバニティ/既定のドメインを更新すると、顧客を一意に識別していない使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="20a8a-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="20a8a-237">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="20a8a-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="20a8a-238">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="20a8a-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="20a8a-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="20a8a-240">サブスクリプションのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="20a8a-240">Subscription nickname.</span></span> <span data-ttu-id="20a8a-241">ニックネームが指定されていない場合、パートナー センターでは OfferName を使用します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="20a8a-242">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="20a8a-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="20a8a-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="20a8a-244">価格表で定義されている、顧客が購入したサービス プランの名前 </span><span class="sxs-lookup"><span data-stu-id="20a8a-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="20a8a-245">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="20a8a-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="20a8a-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span><span class="sxs-lookup"><span data-stu-id="20a8a-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="20a8a-247">使用量ベースのファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="20a8a-247">Usage-based file fields</span></span>


<span data-ttu-id="20a8a-248">顧客の使用量に対する料金を調整するには、調整ファイルの ResellerID/ResellerName/ResellerBillableAccount、顧客名、およびパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="20a8a-249">次のフィールドで、どのサービスが使用されるか、およびレートについて説明します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="20a8a-250">列</span><span class="sxs-lookup"><span data-stu-id="20a8a-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="20a8a-251">説明</span><span class="sxs-lookup"><span data-stu-id="20a8a-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="20a8a-252">サンプル値</span><span class="sxs-lookup"><span data-stu-id="20a8a-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="20a8a-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="20a8a-254">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="20a8a-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="20a8a-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="20a8a-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="20a8a-257">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="20a8a-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="20a8a-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="20a8a-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="20a8a-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="20a8a-260">パートナーのアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="20a8a-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="20a8a-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="20a8a-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="20a8a-263">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="20a8a-263">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="20a8a-264">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="20a8a-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="20a8a-265">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="20a8a-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="20a8a-266">MPNID</span></span></td>
<td><p><span data-ttu-id="20a8a-267">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="20a8a-268">4390934</span><span class="sxs-lookup"><span data-stu-id="20a8a-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="20a8a-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="20a8a-270">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="20a8a-271">「[パートナーごとに明細を示す](#itemizebypartner)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="20a8a-271">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="20a8a-272">4390934</span><span class="sxs-lookup"><span data-stu-id="20a8a-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="20a8a-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="20a8a-274">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="20a8a-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="20a8a-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="20a8a-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="20a8a-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="20a8a-277">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="20a8a-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="20a8a-278">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="20a8a-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20a8a-279">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="20a8a-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="20a8a-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="20a8a-281">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="20a8a-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="20a8a-282">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="20a8a-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="20a8a-283">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="20a8a-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="20a8a-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="20a8a-285">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20a8a-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="20a8a-286">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="20a8a-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="20a8a-287">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="20a8a-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="20a8a-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="20a8a-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="20a8a-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="20a8a-290">サービス プランのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="20a8a-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="20a8a-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="20a8a-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="20a8a-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="20a8a-293">サービス プランの基幹業務</span><span class="sxs-lookup"><span data-stu-id="20a8a-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="20a8a-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="20a8a-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="20a8a-295">OrderID</span></span></td>
<td><p><span data-ttu-id="20a8a-296">Microsoft 課金プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20a8a-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="20a8a-297">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="20a8a-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="20a8a-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="20a8a-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="20a8a-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="20a8a-300">対象の Azure サービスの名前。</span><span class="sxs-lookup"><span data-stu-id="20a8a-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="20a8a-301">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="20a8a-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="20a8a-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="20a8a-303">Windows Azure サービスの特定の種類。</span><span class="sxs-lookup"><span data-stu-id="20a8a-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="20a8a-304">Service Bus – Individual or Pack</span><span class="sxs-lookup"><span data-stu-id="20a8a-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="20a8a-305">SQL Azure database – Business or Web Edition</span><span class="sxs-lookup"><span data-stu-id="20a8a-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="20a8a-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="20a8a-307">すべてのサービス データおよび価格設定構造の特定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20a8a-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="20a8a-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="20a8a-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-309">リソース名</span><span class="sxs-lookup"><span data-stu-id="20a8a-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="20a8a-310">Azure リソースの名前。</span><span class="sxs-lookup"><span data-stu-id="20a8a-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="20a8a-311">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="20a8a-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="20a8a-312">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="20a8a-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-313">Region</span><span class="sxs-lookup"><span data-stu-id="20a8a-313">Region</span></span></td>
<td><p><span data-ttu-id="20a8a-314">使用量が適用される地域。</span><span class="sxs-lookup"><span data-stu-id="20a8a-314">The region the usage applies to.</span></span> <span data-ttu-id="20a8a-315">料金は地域によって異なるため、主にデータ転送に料金を割り当てるために使われます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="20a8a-316">Asia Pacific、Europe、Latin America、North America</span><span class="sxs-lookup"><span data-stu-id="20a8a-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-317">SKU</span><span class="sxs-lookup"><span data-stu-id="20a8a-317">SKU</span></span></td>
<td><p><span data-ttu-id="20a8a-318">プランについての MSFT の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="20a8a-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="20a8a-319">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="20a8a-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="20a8a-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="20a8a-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="20a8a-321">特定の課金期間のサービスまたはリソースに対してさまざまなレートの明細を設定するための ID と数量。</span><span class="sxs-lookup"><span data-stu-id="20a8a-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="20a8a-322">Azure の階層化されたレーティングの場合は、一定数量の課金可能単位までは 1 つのレートがあり、その後に別のレートがあることがあります。</span><span class="sxs-lookup"><span data-stu-id="20a8a-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="20a8a-323">1</span><span class="sxs-lookup"><span data-stu-id="20a8a-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="20a8a-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="20a8a-325">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="20a8a-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="20a8a-326">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="20a8a-327">11</span><span class="sxs-lookup"><span data-stu-id="20a8a-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="20a8a-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="20a8a-329">単位数はプランの一部として含まれます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-329">Units included as part of the offer.</span></span> <span data-ttu-id="20a8a-330">通常、CSP には含まれません。</span><span class="sxs-lookup"><span data-stu-id="20a8a-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="20a8a-331">0</span><span class="sxs-lookup"><span data-stu-id="20a8a-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="20a8a-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="20a8a-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="20a8a-333">単位数はプランの一部として含まれず、パートナーが支払う必要があります。</span><span class="sxs-lookup"><span data-stu-id="20a8a-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="20a8a-334">ConsumedQuantity - IncludedQuantity と同じです。</span><span class="sxs-lookup"><span data-stu-id="20a8a-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="20a8a-335">11</span><span class="sxs-lookup"><span data-stu-id="20a8a-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="20a8a-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="20a8a-337">サブスクリプションの開始日に有効な価格を提供します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="20a8a-338">$0.0808</span><span class="sxs-lookup"><span data-stu-id="20a8a-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="20a8a-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="20a8a-340">ListPrist と OverageQuantity を掛けて、最も近いセントに丸めます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="20a8a-341">$0.085</span><span class="sxs-lookup"><span data-stu-id="20a8a-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="20a8a-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="20a8a-343">市場の税関連の規則や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="20a8a-343">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="20a8a-344">$0.08</span><span class="sxs-lookup"><span data-stu-id="20a8a-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="20a8a-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="20a8a-346">税が適用されるときの税引き後の合計額。</span><span class="sxs-lookup"><span data-stu-id="20a8a-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="20a8a-347">$0.93</span><span class="sxs-lookup"><span data-stu-id="20a8a-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-348">Currency</span><span class="sxs-lookup"><span data-stu-id="20a8a-348">Currency</span></span></td>
<td><p><span data-ttu-id="20a8a-349">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="20a8a-349">Currency type.</span></span> <span data-ttu-id="20a8a-350">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="20a8a-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="20a8a-351">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="20a8a-352">EUR</span><span class="sxs-lookup"><span data-stu-id="20a8a-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="20a8a-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="20a8a-354">単位あたりの税込み価格。</span><span class="sxs-lookup"><span data-stu-id="20a8a-354">Pretax price per unit.</span></span> <span data-ttu-id="20a8a-355">PretaxCharges / OverageQuantity と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="20a8a-356">$0.08</span><span class="sxs-lookup"><span data-stu-id="20a8a-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="20a8a-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="20a8a-358">単位あたりの税引き後の価格。</span><span class="sxs-lookup"><span data-stu-id="20a8a-358">Post tax price per unit.</span></span> <span data-ttu-id="20a8a-359">PostTaxTotal / OverageQuantity、または PretaxEffectiveRate + 単位額あたりの税率と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="20a8a-360">$0.08</span><span class="sxs-lookup"><span data-stu-id="20a8a-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="20a8a-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="20a8a-362">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="20a8a-362">The type of charge or adjustment.</span></span> <span data-ttu-id="20a8a-363">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20a8a-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="20a8a-364">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20a8a-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="20a8a-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="20a8a-366">MSFT 課金プラットフォームの一意のアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="20a8a-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="20a8a-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="20a8a-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="20a8a-369">サービスの展開の日付。</span><span class="sxs-lookup"><span data-stu-id="20a8a-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="20a8a-370">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="20a8a-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="20a8a-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="20a8a-372">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="20a8a-373">East Asia、South East Asia、North Europe、West Europe、North Central US、South Central US</span><span class="sxs-lookup"><span data-stu-id="20a8a-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="20a8a-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="20a8a-375">この列は、[Service Name] 列で特に識別されない可能性のある、個別の Microsoft Azure サービスの追跡に利用されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="20a8a-376">たとえば、データ転送は、[Service Name] 列で &quot;Microsoft Azure - All Services&quot; と報告されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="20a8a-377">この [MeteredService] 列は、利用に関連する特定のサービスを示します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="20a8a-378">AccessControl、CDN、Compute、Database、ServiceBus、Storage</span><span class="sxs-lookup"><span data-stu-id="20a8a-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="20a8a-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="20a8a-380">個々の Microsoft Azure サービスの内容を、MeteredService フィールドで提供されるレベルよりも明確にする小見出し。</span><span class="sxs-lookup"><span data-stu-id="20a8a-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="20a8a-381">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="20a8a-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-382">Project</span><span class="sxs-lookup"><span data-stu-id="20a8a-382">Project</span></span></td>
<td><p><span data-ttu-id="20a8a-383">サービス インスタンスの顧客定義の名前</span><span class="sxs-lookup"><span data-stu-id="20a8a-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="20a8a-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="20a8a-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="20a8a-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="20a8a-386">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="20a8a-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="20a8a-387">例: 1 か月 30 日間の中に、個別にプロビジョニングされた接続がある場合、Service Info 1 は "1.000000 Connections / 30 days" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="20a8a-388">プロビジョニングされた ServiceBus 接続が 25 パックあり、その日に 1 つを利用した場合、その日の 1 日の使用量の計算書には、"25 Connections / 30 Days – Used: 1.000000" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="20a8a-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="20a8a-390">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="20a8a-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="20a8a-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20a8a-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="20a8a-392">DomainName</span></span></td>
<td><p><span data-ttu-id="20a8a-393">顧客のドメイン名。顧客を特定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-393">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="20a8a-394">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="20a8a-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="20a8a-395">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="20a8a-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="20a8a-396">Unit</span><span class="sxs-lookup"><span data-stu-id="20a8a-396">Unit</span></span></td>
<td><p><span data-ttu-id="20a8a-397">リソース名の単位</span><span class="sxs-lookup"><span data-stu-id="20a8a-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="20a8a-398">GB または HOURS</span><span class="sxs-lookup"><span data-stu-id="20a8a-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="20a8a-399">1 回限りの購入ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="20a8a-399">One-time purchase file fields</span></span>

|**<span data-ttu-id="20a8a-400">フィールド</span><span class="sxs-lookup"><span data-stu-id="20a8a-400">Field</span></span>** |**<span data-ttu-id="20a8a-401">説明</span><span class="sxs-lookup"><span data-stu-id="20a8a-401">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="20a8a-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="20a8a-402">PartnerId</span></span> |<span data-ttu-id="20a8a-403">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-403">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="20a8a-404">CustomerId</span><span class="sxs-lookup"><span data-stu-id="20a8a-404">CustomerId</span></span> |<span data-ttu-id="20a8a-405">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-405">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="20a8a-406">CustomerName</span><span class="sxs-lookup"><span data-stu-id="20a8a-406">CustomerName</span></span> |<span data-ttu-id="20a8a-407">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="20a8a-407">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="20a8a-408">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="20a8a-408">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="20a8a-409">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="20a8a-409">CustomerDomainName</span></span> |<span data-ttu-id="20a8a-410">顧客のドメイン名。</span><span class="sxs-lookup"><span data-stu-id="20a8a-410">The customer’s domain name.</span></span> |
|<span data-ttu-id="20a8a-411">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="20a8a-411">CustomerCountry</span></span> |<span data-ttu-id="20a8a-412">顧客の在住国。</span><span class="sxs-lookup"><span data-stu-id="20a8a-412">The country in which the customer is located.</span></span> |
|<span data-ttu-id="20a8a-413">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="20a8a-413">InvoiceNumber</span></span> |<span data-ttu-id="20a8a-414">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="20a8a-414">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="20a8a-415">MpnId</span><span class="sxs-lookup"><span data-stu-id="20a8a-415">MpnId</span></span> |<span data-ttu-id="20a8a-416">CSP パートナー (直接または間接) の MPN ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-416">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="20a8a-417">Reseller MPN ID</span><span class="sxs-lookup"><span data-stu-id="20a8a-417">Reseller MPN ID</span></span> |<span data-ttu-id="20a8a-418">間接モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-418">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="20a8a-419">予約に対する登録リセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-419">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="20a8a-420">これは、パートナー センターで特定の予約について示されるリセラー ID に対応します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-420">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="20a8a-421">CSP パートナーが直接お客様に予約を販売した場合、パートナーの MPN ID が MPN ID とリセラーの MPN ID として 2 か所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-421">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="20a8a-422">CSP パートナーのリセラーに MPN ID がない場合は、代わりに CSP パートナーの MPN ID がこの値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-422">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="20a8a-423">CSP パートナーがリセラー ID を削除した場合、この値は -1 に設定されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-423">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="20a8a-424">OrderId</span><span class="sxs-lookup"><span data-stu-id="20a8a-424">OrderId</span></span> |<span data-ttu-id="20a8a-425">Microsoft 請求プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20a8a-425">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="20a8a-426">サポートに問い合わせる際に、Azure 予約の識別に有効な場合がありますが、調整用ではありません。</span><span class="sxs-lookup"><span data-stu-id="20a8a-426">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="20a8a-427">OrderDate</span><span class="sxs-lookup"><span data-stu-id="20a8a-427">OrderDate</span></span> |<span data-ttu-id="20a8a-428">注文が作成された日付。</span><span class="sxs-lookup"><span data-stu-id="20a8a-428">The date the order was placed.</span></span> |
|<span data-ttu-id="20a8a-429">ProductId</span><span class="sxs-lookup"><span data-stu-id="20a8a-429">ProductId</span></span> |<span data-ttu-id="20a8a-430">製品の ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-430">The ID for the product.</span></span> |
|<span data-ttu-id="20a8a-431">SkuId</span><span class="sxs-lookup"><span data-stu-id="20a8a-431">SkuId</span></span>  |<span data-ttu-id="20a8a-432">特定 SKU の ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-432">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="20a8a-433">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="20a8a-433">AvailabilityId</span></span> |<span data-ttu-id="20a8a-434">特定の可用性 の ID。</span><span class="sxs-lookup"><span data-stu-id="20a8a-434">The ID for a particular Availability.</span></span> <span data-ttu-id="20a8a-435">"可用性" とは、特定の国、通貨、業界などで特定の SKU を購入可能かどうかを指します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-435">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="20a8a-436">SkuName</span><span class="sxs-lookup"><span data-stu-id="20a8a-436">SkuName</span></span>  |<span data-ttu-id="20a8a-437">特定 SKU のタイトル。</span><span class="sxs-lookup"><span data-stu-id="20a8a-437">The title for a particular SKU.</span></span> |
|<span data-ttu-id="20a8a-438">ProductName</span><span class="sxs-lookup"><span data-stu-id="20a8a-438">ProductName</span></span> |<span data-ttu-id="20a8a-439">製品の名前。</span><span class="sxs-lookup"><span data-stu-id="20a8a-439">The name of the product.</span></span> |
|<span data-ttu-id="20a8a-440">ChargeType</span><span class="sxs-lookup"><span data-stu-id="20a8a-440">ChargeType</span></span> |<span data-ttu-id="20a8a-441">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="20a8a-441">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="20a8a-442">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="20a8a-442">UnitPrice</span></span> |<span data-ttu-id="20a8a-443">注文された製品ごとの価格。</span><span class="sxs-lookup"><span data-stu-id="20a8a-443">Price per product ordered.</span></span> |
|<span data-ttu-id="20a8a-444">Quantity</span><span class="sxs-lookup"><span data-stu-id="20a8a-444">Quantity</span></span> |<span data-ttu-id="20a8a-445">注文された製品の数。</span><span class="sxs-lookup"><span data-stu-id="20a8a-445">Number of products ordered.</span></span> |
|<span data-ttu-id="20a8a-446">Subtotal</span><span class="sxs-lookup"><span data-stu-id="20a8a-446">Subtotal</span></span> |<span data-ttu-id="20a8a-447">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="20a8a-447">Total before tax.</span></span> <span data-ttu-id="20a8a-448">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-448">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="20a8a-449">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="20a8a-449">TaxTotal</span></span> |<span data-ttu-id="20a8a-450">該当するすべての税額の合計。</span><span class="sxs-lookup"><span data-stu-id="20a8a-450">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="20a8a-451">Total</span><span class="sxs-lookup"><span data-stu-id="20a8a-451">Total</span></span> |<span data-ttu-id="20a8a-452">この購入の合計金額。</span><span class="sxs-lookup"><span data-stu-id="20a8a-452">The total amount of this purchase.</span></span> |
|<span data-ttu-id="20a8a-453">Currency</span><span class="sxs-lookup"><span data-stu-id="20a8a-453">Currency</span></span> |<span data-ttu-id="20a8a-454">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="20a8a-454">Currency type.</span></span> <span data-ttu-id="20a8a-455">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="20a8a-455">Each billing entity has only one currency.</span></span> <span data-ttu-id="20a8a-456">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-456">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="20a8a-457">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="20a8a-457">DiscountDetails</span></span> |<span data-ttu-id="20a8a-458">関連する割引の詳細を示す一覧。</span><span class="sxs-lookup"><span data-stu-id="20a8a-458">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="20a8a-459">請求書と調整ファイルの間の課金のマッピング</span><span class="sxs-lookup"><span data-stu-id="20a8a-459">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="20a8a-460">請求書は料金の概要を示し、調整ファイルは、課金の種類を含め、行項目のトランザクションの詳細な内訳を示します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-460">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="20a8a-461">請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルター オプションを使用して、調整ファイルの課金の種類でフィルター処理し、請求書の課金を調整ファイルの一連の課金の内訳にマップします。</span><span class="sxs-lookup"><span data-stu-id="20a8a-461">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="20a8a-462">使用量ベースとライセンス ベースの調整ファイルには、使用量関連のトランザクションと料金 (消費された単位量および関連する料金) のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-462">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="20a8a-463">請求書に “調整” として表示される単発のクレジット、割引、払い戻し金額は、調整ファイルに表示されません。</span><span class="sxs-lookup"><span data-stu-id="20a8a-463">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="20a8a-464">次の表に、請求書のセクションと、調整ファイルに表示される関連付けられた課金の種類とのマッピングを示します。</span><span class="sxs-lookup"><span data-stu-id="20a8a-464">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="20a8a-465">請求書の課金の説明</span><span class="sxs-lookup"><span data-stu-id="20a8a-465">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="20a8a-466">調整ファイルの課金の説明 (ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="20a8a-466">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="20a8a-467">この課金の意味</span><span class="sxs-lookup"><span data-stu-id="20a8a-467">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="20a8a-468">これらの ChargeTypes を請求書にマップする方法</span><span class="sxs-lookup"><span data-stu-id="20a8a-468">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="20a8a-469">ライセンス ベースの課金</span><span class="sxs-lookup"><span data-stu-id="20a8a-469">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="20a8a-470">Activation fee</span><span class="sxs-lookup"><span data-stu-id="20a8a-470">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-471">購入したサブスクリプションを顧客が使用したときに顧客に課金される金額</span><span class="sxs-lookup"><span data-stu-id="20a8a-471">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="20a8a-472">ライセンスベースのファイルから、<strong>Amount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20a8a-472">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20a8a-473">取り消し料金</span><span class="sxs-lookup"><span data-stu-id="20a8a-473">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-474">関連付けられているシートが変更されたときに顧客に払い戻される日割り料金</span><span class="sxs-lookup"><span data-stu-id="20a8a-474">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20a8a-475">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="20a8a-475">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-476">サブスクリプションの定期的な課金</span><span class="sxs-lookup"><span data-stu-id="20a8a-476">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20a8a-477">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="20a8a-477">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-478">関連付けられているシートが変更されたときに顧客から評価される日割り料金</span><span class="sxs-lookup"><span data-stu-id="20a8a-478">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20a8a-479">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="20a8a-479">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-480">取り消し時のサービスの未使用部分に対する日割りの払戻し額</span><span class="sxs-lookup"><span data-stu-id="20a8a-480">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20a8a-481">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="20a8a-481">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-482">年次請求を使用する場合、サブスクリプションの請求の種類</span><span class="sxs-lookup"><span data-stu-id="20a8a-482">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20a8a-483">Purchase fee</span><span class="sxs-lookup"><span data-stu-id="20a8a-483">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-484">月次請求を使用する場合、サブスクリプションの請求の種類</span><span class="sxs-lookup"><span data-stu-id="20a8a-484">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20a8a-485">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="20a8a-485">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-486">サブスクリプションの更新時の日割り料金</span><span class="sxs-lookup"><span data-stu-id="20a8a-486">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="20a8a-487">Renew fee</span><span class="sxs-lookup"><span data-stu-id="20a8a-487">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-488">サブスクリプションの更新時の課金</span><span class="sxs-lookup"><span data-stu-id="20a8a-488">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20a8a-489">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="20a8a-489">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-490">アクティブ化から課金期間の終了までの日割り料金</span><span class="sxs-lookup"><span data-stu-id="20a8a-490">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="20a8a-491">利用料金</span><span class="sxs-lookup"><span data-stu-id="20a8a-491">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="20a8a-492">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="20a8a-492">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-493">現在の課金期間中に未払いの使用を取り消したときのアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="20a8a-493">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="20a8a-494">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20a8a-494">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20a8a-495">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="20a8a-495">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-496">現在の課金期間のアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="20a8a-496">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="20a8a-497">クレジット</span><span class="sxs-lookup"><span data-stu-id="20a8a-497">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="20a8a-498">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="20a8a-498">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-499">税金を含む、行項目への一部または全部の払戻し</span><span class="sxs-lookup"><span data-stu-id="20a8a-499">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-500">ライセンス ベースのファイルから、<strong>TotalForCustomer</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20a8a-500">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="20a8a-501">使用量ベースのファイルから、<strong>PostTaxTotal</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20a8a-501">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="20a8a-502">使用量ベースの割引</span><span class="sxs-lookup"><span data-stu-id="20a8a-502">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="20a8a-503">Activation discount</span><span class="sxs-lookup"><span data-stu-id="20a8a-503">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-504">サブスクリプションがアクティブ化されたときに適用される割引</span><span class="sxs-lookup"><span data-stu-id="20a8a-504">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="20a8a-505">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20a8a-505">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20a8a-506">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="20a8a-506">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-507">定期的な課金に適用される割引</span><span class="sxs-lookup"><span data-stu-id="20a8a-507">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20a8a-508">Renew discount</span><span class="sxs-lookup"><span data-stu-id="20a8a-508">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-509">サブスクリプションの更新時に適用される割引</span><span class="sxs-lookup"><span data-stu-id="20a8a-509">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20a8a-510">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="20a8a-510">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-511">割引が取り消されたときに適用される料金</span><span class="sxs-lookup"><span data-stu-id="20a8a-511">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="20a8a-512">ライセンス ベースの割引</span><span class="sxs-lookup"><span data-stu-id="20a8a-512">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="20a8a-513">複数の種類の料金に適用される場合がある</span><span class="sxs-lookup"><span data-stu-id="20a8a-513">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="20a8a-514">ライセンス ベースのファイルから、<strong>TotalOtherDiscount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20a8a-514">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20a8a-515"><strong>税</strong>&nbsp;または&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="20a8a-515"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="20a8a-516">複数の種類の料金に適用される場合がある</span><span class="sxs-lookup"><span data-stu-id="20a8a-516">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="20a8a-517">例外: "Offset a line item" には既に税が含まれます。</span><span class="sxs-lookup"><span data-stu-id="20a8a-517">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="20a8a-518">上記のクレジットを参照してください。</span><span class="sxs-lookup"><span data-stu-id="20a8a-518">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="20a8a-519">税または付加価値税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="20a8a-519">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="20a8a-520">ライセンス ベースのファイルから、<strong>Tax</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20a8a-520">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="20a8a-521">使用量ベースのファイルから、<strong>TaxAmount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20a8a-521">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
