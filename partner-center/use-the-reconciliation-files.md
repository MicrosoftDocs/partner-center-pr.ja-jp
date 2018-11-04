---
title: 調整ファイルを使う | パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: 請求サイクルの各料金の詳しい行項目ビューのためには、パートナー センターから、調整ファイルをダウンロードします。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.localizationpriority: medium
ms.openlocfilehash: 4b5fbab84c30743e4d91b32bf4cbd2bb8b950992
ms.sourcegitcommit: b433061dff8f667c81b623c33417fb490d8e3b4a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/04/2018
ms.locfileid: "6022235"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="5e7f1-103">調整ファイルを使う</span><span class="sxs-lookup"><span data-stu-id="5e7f1-103">Use the reconciliation files</span></span>

**<span data-ttu-id="5e7f1-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="5e7f1-104">Applies to</span></span>**

-  <span data-ttu-id="5e7f1-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="5e7f1-105">Partner Center</span></span>
-  <span data-ttu-id="5e7f1-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="5e7f1-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="5e7f1-107">Microsoft Cloud ドイツのパートナー センター</span><span class="sxs-lookup"><span data-stu-id="5e7f1-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="5e7f1-108">請求サイクルの各料金の詳しい行項目ビューのためには、パートナー センターから、調整ファイルをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="5e7f1-109">詳細には、各顧客のサブスクリプションの料金や、詳細なイベント (期間途中でのサブスクリプションへのシートの追加など) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="5e7f1-110">パートナーごとに明細を示す</span><span class="sxs-lookup"><span data-stu-id="5e7f1-110">Itemize by partner</span></span>


<span data-ttu-id="5e7f1-111">インダイレクト モデルのパートナーは、ライセンス ベースの調整ファイルと使用量ベースの調整ファイルの両方で、これらの追加フィールドを使用してリセラーごとに明細を記載できます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="5e7f1-112">MPN ID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-112">MPN ID</span></span></th>
<th><span data-ttu-id="5e7f1-113">説明</span><span class="sxs-lookup"><span data-stu-id="5e7f1-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="5e7f1-114">MPN ID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="5e7f1-115">CSP パートナー (直接または間接) の Microsoft Partner Network (MPN) IDです。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-116">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="5e7f1-117">インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="5e7f1-118">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="5e7f1-119">これは、パートナー センターで特定のサブスクリプションについて示されるリセラー ID に対応します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="5e7f1-120">リセラーを表示または更新プログラムから、パートナー センター メニューで、リセラーは、<strong>顧客</strong>を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-120">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="5e7f1-121">顧客メニューの <strong>[サブスクリプション]</strong> を選び、一覧からサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="5e7f1-122">
          <strong>[更新]</strong> を選んで、<strong>[再販業者 (MPN ID)]</strong> を変更します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="5e7f1-123">CSP パートナーがお客様に直接サブスクリプションを販売した場合、パートナーの MPN ID が MPN ID とリセラーの MPN ID として 2 か所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="5e7f1-124">CSP パートナーのリセラーに MPN ID がない場合は、代わりに CSP パートナーの MPN ID がこの値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="5e7f1-125">CSP パートナーがリセラー ID を削除した場合、この値は -1 に設定されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="5e7f1-126">ライセンス ベースのファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="5e7f1-126">License-based file fields</span></span>


<span data-ttu-id="5e7f1-127">顧客の注文に対する料金を調整するには、調整ファイルの Syndication\_Partner\_Subscription\_Number とパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="5e7f1-128">列</span><span class="sxs-lookup"><span data-stu-id="5e7f1-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="5e7f1-129">説明</span><span class="sxs-lookup"><span data-stu-id="5e7f1-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="5e7f1-130">サンプル値</span><span class="sxs-lookup"><span data-stu-id="5e7f1-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-131">PartnerId</span><span class="sxs-lookup"><span data-stu-id="5e7f1-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="5e7f1-132">特定の課金エンティティの一意の識別子 (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="5e7f1-133">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="5e7f1-134">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="5e7f1-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="5e7f1-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="5e7f1-137">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="5e7f1-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="5e7f1-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-139">OrderID</span></span></td>
<td><p><span data-ttu-id="5e7f1-140">Microsoft 課金プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="5e7f1-141">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="5e7f1-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="5e7f1-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="5e7f1-144">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="5e7f1-145">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="5e7f1-146">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="5e7f1-147">「Syndication_Partner_Subscription_Number」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="5e7f1-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="5e7f1-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="5e7f1-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="5e7f1-150">サブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="5e7f1-151">お客様は同じプランで複数のサブスクリプションを持つことができるため、これは調整ファイルの分析で重要です。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="5e7f1-152">このフィールドは、パートナー管理コンソールのサブスクリプション ID にマップされます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="5e7f1-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="5e7f1-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-154">OfferID</span></span></td>
<td><p><span data-ttu-id="5e7f1-155">一意のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-155">Unique offer ID.</span></span> <span data-ttu-id="5e7f1-156">価格表に従った標準のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="5e7f1-157"><b>注</b>: この値は、価格表のプラン ID とは一致しません。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="5e7f1-158">以下の DurableOfferID を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="5e7f1-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="5e7f1-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="5e7f1-161">価格表で定義されている一意の継続的なプラン ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="5e7f1-162"><b>注</b>: この値は価格表のプラン ID と一致します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="5e7f1-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="5e7f1-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="5e7f1-164">OfferName</span></span></td>
<td><p><span data-ttu-id="5e7f1-165">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="5e7f1-166">Microsoft Office 365 (プラン E3)</span><span class="sxs-lookup"><span data-stu-id="5e7f1-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="5e7f1-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="5e7f1-168">サブスクリプションの開始日。注文が送信された日に設定されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="5e7f1-169">サブスクリプションの開始日を終了日と共に確認することにより、顧客がサブスクリプションの最初の 1 年以内であるか、サブスクリプションが次の 1 年間更新されたかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="5e7f1-170">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="5e7f1-171">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="5e7f1-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="5e7f1-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="5e7f1-173">サブスクリプション終了日: 開始日から 12 か月 + x 日後 (パートナーの請求日と合わせる) または更新日から 12 か月</span><span class="sxs-lookup"><span data-stu-id="5e7f1-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="5e7f1-174">更新時に、価格は最新の価格表に更新されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="5e7f1-175">自動更新の前に、顧客とのやり取りが必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="5e7f1-176">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="5e7f1-177">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="5e7f1-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="5e7f1-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="5e7f1-179">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="5e7f1-180">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="5e7f1-181">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="5e7f1-182">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="5e7f1-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="5e7f1-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="5e7f1-184">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="5e7f1-185">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="5e7f1-186">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="5e7f1-187">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="5e7f1-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="5e7f1-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="5e7f1-189">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-189">The type of charge or adjustment.</span></span> <span data-ttu-id="5e7f1-190">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="5e7f1-191">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="5e7f1-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="5e7f1-193">シート単価 (購入時に価格表に公開されていた価格)。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-193">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="5e7f1-194">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="5e7f1-195">6.82</span><span class="sxs-lookup"><span data-stu-id="5e7f1-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-196">Quantity</span><span class="sxs-lookup"><span data-stu-id="5e7f1-196">Quantity</span></span></td>
<td><p><span data-ttu-id="5e7f1-197">シート数。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-197">Number of seats.</span></span> <span data-ttu-id="5e7f1-198">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="5e7f1-199">2</span><span class="sxs-lookup"><span data-stu-id="5e7f1-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-200">Amount</span><span class="sxs-lookup"><span data-stu-id="5e7f1-200">Amount</span></span></td>
<td><p><span data-ttu-id="5e7f1-201">数量に対する合計価格。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-201">Total of price for quantity.</span></span> <span data-ttu-id="5e7f1-202">金額の計算が、この顧客用の計算方法に一致することを確認するために役立ちます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="5e7f1-203">13.32</span><span class="sxs-lookup"><span data-stu-id="5e7f1-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="5e7f1-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="5e7f1-205">これらの料金に適用される割引額。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="5e7f1-206">インセンティブの対象となる IUR または新しいサブスクリプションの場合も、この列に割引額が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="5e7f1-207">2.32</span><span class="sxs-lookup"><span data-stu-id="5e7f1-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-208">Subtotal</span><span class="sxs-lookup"><span data-stu-id="5e7f1-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="5e7f1-209">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-209">Total before tax.</span></span> <span data-ttu-id="5e7f1-210">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="5e7f1-211">11</span><span class="sxs-lookup"><span data-stu-id="5e7f1-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-212">Tax</span><span class="sxs-lookup"><span data-stu-id="5e7f1-212">Tax</span></span></td>
<td><p><span data-ttu-id="5e7f1-213">市場の税関連の規則や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="5e7f1-214">0</span><span class="sxs-lookup"><span data-stu-id="5e7f1-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="5e7f1-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="5e7f1-216">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-216">Total after tax.</span></span> <span data-ttu-id="5e7f1-217">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="5e7f1-218">11</span><span class="sxs-lookup"><span data-stu-id="5e7f1-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-219">Currency</span><span class="sxs-lookup"><span data-stu-id="5e7f1-219">Currency</span></span></td>
<td><p><span data-ttu-id="5e7f1-220">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-220">Currency type.</span></span> <span data-ttu-id="5e7f1-221">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="5e7f1-222">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="5e7f1-223">EUR</span><span class="sxs-lookup"><span data-stu-id="5e7f1-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="5e7f1-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="5e7f1-225">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="5e7f1-226">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="5e7f1-227">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="5e7f1-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-228">MPNID</span></span></td>
<td><p><span data-ttu-id="5e7f1-229">CSP パートナーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="5e7f1-230">4390934</span><span class="sxs-lookup"><span data-stu-id="5e7f1-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="5e7f1-232">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="5e7f1-233">「[パートナーごとに明細を示す](#itemizebypartner)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="5e7f1-234">4390934</span><span class="sxs-lookup"><span data-stu-id="5e7f1-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="5e7f1-235">DomainName</span></span></td>
<td><p><span data-ttu-id="5e7f1-236">顧客のドメイン名。顧客を特定できるようにするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-236">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="5e7f1-237">これは、顧客/パートナーが、O365 ポータル経由でバニティ/既定のドメインを更新すると、顧客を一意に識別していない使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-237">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="5e7f1-238">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-238">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="5e7f1-239">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="5e7f1-239">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-240">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="5e7f1-240">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="5e7f1-241">サブスクリプションのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-241">Subscription nickname.</span></span> <span data-ttu-id="5e7f1-242">ニックネームが指定されていない場合、パートナー センターでは OfferName を使用します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-242">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="5e7f1-243">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="5e7f1-243">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-244">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="5e7f1-244">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="5e7f1-245">価格表で定義されている、顧客が購入したサービス プランの名前 </span><span class="sxs-lookup"><span data-stu-id="5e7f1-245">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="5e7f1-246">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-246">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="5e7f1-247">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span><span class="sxs-lookup"><span data-stu-id="5e7f1-247">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="5e7f1-248">使用量ベースのファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="5e7f1-248">Usage-based file fields</span></span>


<span data-ttu-id="5e7f1-249">顧客の使用量に対する料金を調整するには、調整ファイルの ResellerID/ResellerName/ResellerBillableAccount、顧客名、およびパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-249">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="5e7f1-250">次のフィールドで、どのサービスが使用されるか、およびレートについて説明します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-250">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="5e7f1-251">列</span><span class="sxs-lookup"><span data-stu-id="5e7f1-251">Column</span></span></strong></td>
<td><strong><span data-ttu-id="5e7f1-252">説明</span><span class="sxs-lookup"><span data-stu-id="5e7f1-252">Description</span></span></strong></td>
<td><strong><span data-ttu-id="5e7f1-253">サンプル値</span><span class="sxs-lookup"><span data-stu-id="5e7f1-253">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-254">PartnerID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-254">PartnerID</span></span></td>
<td><p><span data-ttu-id="5e7f1-255">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-255">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="5e7f1-256">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="5e7f1-256">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-257">PartnerName</span><span class="sxs-lookup"><span data-stu-id="5e7f1-257">PartnerName</span></span></td>
<td><p><span data-ttu-id="5e7f1-258">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-258">Partner Name.</span></span></p></td>
<td><span data-ttu-id="5e7f1-259">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="5e7f1-259">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-260">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-260">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="5e7f1-261">パートナーのアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-261">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="5e7f1-262">1010578050</span><span class="sxs-lookup"><span data-stu-id="5e7f1-262">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-263">CustomerName</span><span class="sxs-lookup"><span data-stu-id="5e7f1-263">CustomerName</span></span></td>
<td><p><span data-ttu-id="5e7f1-264">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-264">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="5e7f1-265">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-265">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="5e7f1-266">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="5e7f1-266">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-267">MPNID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-267">MPNID</span></span></td>
<td><p><span data-ttu-id="5e7f1-268">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-268">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="5e7f1-269">4390934</span><span class="sxs-lookup"><span data-stu-id="5e7f1-269">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-270">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-270">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="5e7f1-271">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-271">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="5e7f1-272">「[パートナーごとに明細を示す](#itemizebypartner)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-272">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="5e7f1-273">4390934</span><span class="sxs-lookup"><span data-stu-id="5e7f1-273">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-274">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="5e7f1-274">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="5e7f1-275">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-275">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="5e7f1-276">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="5e7f1-276">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-277">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="5e7f1-277">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="5e7f1-278">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-278">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="5e7f1-279">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-279">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="5e7f1-280">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="5e7f1-280">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-281">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="5e7f1-281">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="5e7f1-282">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-282">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="5e7f1-283">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-283">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="5e7f1-284">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="5e7f1-284">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-285">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-285">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="5e7f1-286">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-286">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="5e7f1-287">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-287">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="5e7f1-288">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-288">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="5e7f1-289">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="5e7f1-289">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-290">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="5e7f1-290">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="5e7f1-291">サービス プランのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-291">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="5e7f1-292">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="5e7f1-292">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-293">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="5e7f1-293">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="5e7f1-294">サービス プランの基幹業務</span><span class="sxs-lookup"><span data-stu-id="5e7f1-294">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="5e7f1-295">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="5e7f1-295">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-296">OrderID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-296">OrderID</span></span></td>
<td><p><span data-ttu-id="5e7f1-297">Microsoft 課金プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-297">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="5e7f1-298">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-298">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="5e7f1-299">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="5e7f1-299">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-300">ServiceName</span><span class="sxs-lookup"><span data-stu-id="5e7f1-300">ServiceName</span></span></td>
<td><p><span data-ttu-id="5e7f1-301">対象の Azure サービスの名前。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-301">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="5e7f1-302">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="5e7f1-302">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-303">ServiceType</span><span class="sxs-lookup"><span data-stu-id="5e7f1-303">ServiceType</span></span></td>
<td><p><span data-ttu-id="5e7f1-304">Windows Azure サービスの特定の種類。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-304">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="5e7f1-305">Service Bus – Individual or Pack</span><span class="sxs-lookup"><span data-stu-id="5e7f1-305">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="5e7f1-306">SQL Azure database – Business or Web Edition</span><span class="sxs-lookup"><span data-stu-id="5e7f1-306">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-307">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-307">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="5e7f1-308">すべてのサービス データおよび価格設定構造の特定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-308">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="5e7f1-309">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="5e7f1-309">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-310">リソース名</span><span class="sxs-lookup"><span data-stu-id="5e7f1-310">Resource Name</span></span></td>
<td><p><span data-ttu-id="5e7f1-311">Azure リソースの名前。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-311">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="5e7f1-312">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="5e7f1-312">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="5e7f1-313">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="5e7f1-313">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-314">Region</span><span class="sxs-lookup"><span data-stu-id="5e7f1-314">Region</span></span></td>
<td><p><span data-ttu-id="5e7f1-315">使用量が適用される地域。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-315">The region the usage applies to.</span></span> <span data-ttu-id="5e7f1-316">料金は地域によって異なるため、主にデータ転送に料金を割り当てるために使われます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-316">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="5e7f1-317">Asia Pacific、Europe、Latin America、North America</span><span class="sxs-lookup"><span data-stu-id="5e7f1-317">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-318">SKU</span><span class="sxs-lookup"><span data-stu-id="5e7f1-318">SKU</span></span></td>
<td><p><span data-ttu-id="5e7f1-319">プランについての MSFT の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="5e7f1-319">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="5e7f1-320">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="5e7f1-320">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="5e7f1-321">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="5e7f1-321">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="5e7f1-322">特定の課金期間のサービスまたはリソースに対してさまざまなレートの明細を設定するための ID と数量。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-322">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="5e7f1-323">Azure の階層化されたレーティングの場合は、一定数量の課金可能単位までは 1 つのレートがあり、その後に別のレートがあることがあります。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-323">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="5e7f1-324">1</span><span class="sxs-lookup"><span data-stu-id="5e7f1-324">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-325">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="5e7f1-325">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="5e7f1-326">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-326">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="5e7f1-327">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-327">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="5e7f1-328">11</span><span class="sxs-lookup"><span data-stu-id="5e7f1-328">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-329">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="5e7f1-329">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="5e7f1-330">単位数はプランの一部として含まれます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-330">Units included as part of the offer.</span></span> <span data-ttu-id="5e7f1-331">通常、CSP には含まれません。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-331">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="5e7f1-332">0</span><span class="sxs-lookup"><span data-stu-id="5e7f1-332">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="5e7f1-333">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="5e7f1-333">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="5e7f1-334">単位数はプランの一部として含まれず、パートナーが支払う必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-334">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="5e7f1-335">ConsumedQuantity - IncludedQuantity と同じです。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-335">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="5e7f1-336">11</span><span class="sxs-lookup"><span data-stu-id="5e7f1-336">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-337">ListPrice</span><span class="sxs-lookup"><span data-stu-id="5e7f1-337">ListPrice</span></span></td>
<td><p><span data-ttu-id="5e7f1-338">サブスクリプションの開始日に有効な価格を提供します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-338">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="5e7f1-339">$0.0808</span><span class="sxs-lookup"><span data-stu-id="5e7f1-339">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-340">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="5e7f1-340">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="5e7f1-341">ListPrist と OverageQuantity を掛けて、最も近いセントに丸めます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-341">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="5e7f1-342">$0.085</span><span class="sxs-lookup"><span data-stu-id="5e7f1-342">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-343">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="5e7f1-343">TaxAmount</span></span></td>
<td><p><span data-ttu-id="5e7f1-344">市場の税関連の規則や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-344">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="5e7f1-345">$0.08</span><span class="sxs-lookup"><span data-stu-id="5e7f1-345">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-346">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="5e7f1-346">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="5e7f1-347">税が適用されるときの税引き後の合計額。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-347">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="5e7f1-348">$0.93</span><span class="sxs-lookup"><span data-stu-id="5e7f1-348">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-349">Currency</span><span class="sxs-lookup"><span data-stu-id="5e7f1-349">Currency</span></span></td>
<td><p><span data-ttu-id="5e7f1-350">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-350">Currency type.</span></span> <span data-ttu-id="5e7f1-351">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-351">Each billing entity has only one currency.</span></span> <span data-ttu-id="5e7f1-352">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-352">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="5e7f1-353">EUR</span><span class="sxs-lookup"><span data-stu-id="5e7f1-353">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-354">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="5e7f1-354">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="5e7f1-355">単位あたりの税込み価格。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-355">Pretax price per unit.</span></span> <span data-ttu-id="5e7f1-356">PretaxCharges / OverageQuantity と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-356">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="5e7f1-357">$0.08</span><span class="sxs-lookup"><span data-stu-id="5e7f1-357">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-358">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="5e7f1-358">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="5e7f1-359">単位あたりの税引き後の価格。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-359">Post tax price per unit.</span></span> <span data-ttu-id="5e7f1-360">PostTaxTotal / OverageQuantity、または PretaxEffectiveRate + 単位額あたりの税率と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-360">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="5e7f1-361">$0.08</span><span class="sxs-lookup"><span data-stu-id="5e7f1-361">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-362">ChargeType</span><span class="sxs-lookup"><span data-stu-id="5e7f1-362">ChargeType</span></span></td>
<td><p><span data-ttu-id="5e7f1-363">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-363">The type of charge or adjustment.</span></span> <span data-ttu-id="5e7f1-364">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="5e7f1-365">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-365">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-366">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="5e7f1-366">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="5e7f1-367">MSFT 課金プラットフォームの一意のアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-367">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="5e7f1-368">1280018095</span><span class="sxs-lookup"><span data-stu-id="5e7f1-368">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-369">UsageDate</span><span class="sxs-lookup"><span data-stu-id="5e7f1-369">UsageDate</span></span></td>
<td><p><span data-ttu-id="5e7f1-370">サービスの展開の日付。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-370">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="5e7f1-371">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="5e7f1-371">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-372">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="5e7f1-372">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="5e7f1-373">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-373">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="5e7f1-374">East Asia、South East Asia、North Europe、West Europe、North Central US、South Central US</span><span class="sxs-lookup"><span data-stu-id="5e7f1-374">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-375">MeteredService</span><span class="sxs-lookup"><span data-stu-id="5e7f1-375">MeteredService</span></span></td>
<td><p><span data-ttu-id="5e7f1-376">この列は、[Service Name] 列で特に識別されない可能性のある、個別の Microsoft Azure サービスの追跡に利用されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-376">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="5e7f1-377">たとえば、データ転送は、[Service Name] 列で &quot;Microsoft Azure - All Services&quot; と報告されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-377">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="5e7f1-378">この [MeteredService] 列は、利用に関連する特定のサービスを示します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-378">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="5e7f1-379">AccessControl、CDN、Compute、Database、ServiceBus、Storage</span><span class="sxs-lookup"><span data-stu-id="5e7f1-379">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-380">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="5e7f1-380">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="5e7f1-381">個々の Microsoft Azure サービスの内容を、MeteredService フィールドで提供されるレベルよりも明確にする小見出し。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-381">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="5e7f1-382">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="5e7f1-382">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-383">Project</span><span class="sxs-lookup"><span data-stu-id="5e7f1-383">Project</span></span></td>
<td><p><span data-ttu-id="5e7f1-384">サービス インスタンスの顧客定義の名前</span><span class="sxs-lookup"><span data-stu-id="5e7f1-384">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="5e7f1-385">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="5e7f1-385">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-386">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="5e7f1-386">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="5e7f1-387">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-387">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="5e7f1-388">例: 1 か月 30 日間の中に、個別にプロビジョニングされた接続がある場合、Service Info 1 は "1.000000 Connections / 30 days" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-388">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="5e7f1-389">プロビジョニングされた ServiceBus 接続が 25 パックあり、その日に 1 つを利用した場合、その日の 1 日の使用量の計算書には、"25 Connections / 30 Days – Used: 1.000000" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-389">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-390">CustomerID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-390">CustomerID</span></span></td>
<td><p><span data-ttu-id="5e7f1-391">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-391">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="5e7f1-392">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="5e7f1-392">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="5e7f1-393">DomainName</span><span class="sxs-lookup"><span data-stu-id="5e7f1-393">DomainName</span></span></td>
<td><p><span data-ttu-id="5e7f1-394">顧客のドメイン名。顧客を特定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-394">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="5e7f1-395">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-395">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="5e7f1-396">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="5e7f1-396">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="5e7f1-397">Unit</span><span class="sxs-lookup"><span data-stu-id="5e7f1-397">Unit</span></span></td>
<td><p><span data-ttu-id="5e7f1-398">リソース名の単位</span><span class="sxs-lookup"><span data-stu-id="5e7f1-398">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="5e7f1-399">GB または HOURS</span><span class="sxs-lookup"><span data-stu-id="5e7f1-399">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="5e7f1-400">1 回限りの購入ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="5e7f1-400">One-time purchase file fields</span></span>

|**<span data-ttu-id="5e7f1-401">フィールド</span><span class="sxs-lookup"><span data-stu-id="5e7f1-401">Field</span></span>** |**<span data-ttu-id="5e7f1-402">説明</span><span class="sxs-lookup"><span data-stu-id="5e7f1-402">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="5e7f1-403">PartnerId</span><span class="sxs-lookup"><span data-stu-id="5e7f1-403">PartnerId</span></span> |<span data-ttu-id="5e7f1-404">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-404">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="5e7f1-405">CustomerId</span><span class="sxs-lookup"><span data-stu-id="5e7f1-405">CustomerId</span></span> |<span data-ttu-id="5e7f1-406">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-406">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="5e7f1-407">CustomerName</span><span class="sxs-lookup"><span data-stu-id="5e7f1-407">CustomerName</span></span> |<span data-ttu-id="5e7f1-408">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-408">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="5e7f1-409">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-409">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="5e7f1-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="5e7f1-410">CustomerDomainName</span></span> |<span data-ttu-id="5e7f1-411">顧客のドメイン名。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-411">The customer’s domain name.</span></span> |
|<span data-ttu-id="5e7f1-412">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="5e7f1-412">CustomerCountry</span></span> |<span data-ttu-id="5e7f1-413">顧客の在住国。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-413">The country in which the customer is located.</span></span> |
|<span data-ttu-id="5e7f1-414">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="5e7f1-414">InvoiceNumber</span></span> |<span data-ttu-id="5e7f1-415">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-415">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="5e7f1-416">MpnId</span><span class="sxs-lookup"><span data-stu-id="5e7f1-416">MpnId</span></span> |<span data-ttu-id="5e7f1-417">CSP パートナー (直接または間接) の MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-417">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="5e7f1-418">Reseller MPN ID</span><span class="sxs-lookup"><span data-stu-id="5e7f1-418">Reseller MPN ID</span></span> |<span data-ttu-id="5e7f1-419">間接モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-419">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="5e7f1-420">予約に対する登録リセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-420">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="5e7f1-421">これは、パートナー センターで特定の予約について示されるリセラー ID に対応します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-421">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="5e7f1-422">CSP パートナーが直接お客様に予約を販売した場合、パートナーの MPN ID が MPN ID とリセラーの MPN ID として 2 か所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-422">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="5e7f1-423">CSP パートナーのリセラーに MPN ID がない場合は、代わりに CSP パートナーの MPN ID がこの値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-423">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="5e7f1-424">CSP パートナーがリセラー ID を削除した場合、この値は -1 に設定されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-424">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="5e7f1-425">OrderId</span><span class="sxs-lookup"><span data-stu-id="5e7f1-425">OrderId</span></span> |<span data-ttu-id="5e7f1-426">Microsoft 請求プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-426">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="5e7f1-427">サポートに問い合わせる際に、Azure 予約の識別に有効な場合がありますが、調整用ではありません。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-427">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="5e7f1-428">OrderDate</span><span class="sxs-lookup"><span data-stu-id="5e7f1-428">OrderDate</span></span> |<span data-ttu-id="5e7f1-429">注文が作成された日付。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-429">The date the order was placed.</span></span> |
|<span data-ttu-id="5e7f1-430">ProductId</span><span class="sxs-lookup"><span data-stu-id="5e7f1-430">ProductId</span></span> |<span data-ttu-id="5e7f1-431">製品の ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-431">The ID for the product.</span></span> |
|<span data-ttu-id="5e7f1-432">SkuId</span><span class="sxs-lookup"><span data-stu-id="5e7f1-432">SkuId</span></span>  |<span data-ttu-id="5e7f1-433">特定 SKU の ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-433">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="5e7f1-434">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="5e7f1-434">AvailabilityId</span></span> |<span data-ttu-id="5e7f1-435">特定の可用性 の ID。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-435">The ID for a particular Availability.</span></span> <span data-ttu-id="5e7f1-436">"可用性" とは、特定の国、通貨、業界などで特定の SKU を購入可能かどうかを指します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-436">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="5e7f1-437">SkuName</span><span class="sxs-lookup"><span data-stu-id="5e7f1-437">SkuName</span></span>  |<span data-ttu-id="5e7f1-438">特定 SKU のタイトル。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-438">The title for a particular SKU.</span></span> |
|<span data-ttu-id="5e7f1-439">ProductName</span><span class="sxs-lookup"><span data-stu-id="5e7f1-439">ProductName</span></span> |<span data-ttu-id="5e7f1-440">製品の名前。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-440">The name of the product.</span></span> |
|<span data-ttu-id="5e7f1-441">ChargeType</span><span class="sxs-lookup"><span data-stu-id="5e7f1-441">ChargeType</span></span> |<span data-ttu-id="5e7f1-442">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-442">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="5e7f1-443">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="5e7f1-443">UnitPrice</span></span> |<span data-ttu-id="5e7f1-444">注文された製品ごとの価格。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-444">Price per product ordered.</span></span> |
|<span data-ttu-id="5e7f1-445">Quantity</span><span class="sxs-lookup"><span data-stu-id="5e7f1-445">Quantity</span></span> |<span data-ttu-id="5e7f1-446">注文された製品の数。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-446">Number of products ordered.</span></span> |
|<span data-ttu-id="5e7f1-447">Subtotal</span><span class="sxs-lookup"><span data-stu-id="5e7f1-447">Subtotal</span></span> |<span data-ttu-id="5e7f1-448">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-448">Total before tax.</span></span> <span data-ttu-id="5e7f1-449">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-449">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="5e7f1-450">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="5e7f1-450">TaxTotal</span></span> |<span data-ttu-id="5e7f1-451">該当するすべての税額の合計。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-451">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="5e7f1-452">Total</span><span class="sxs-lookup"><span data-stu-id="5e7f1-452">Total</span></span> |<span data-ttu-id="5e7f1-453">この購入の合計金額。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-453">The total amount of this purchase.</span></span> |
|<span data-ttu-id="5e7f1-454">Currency</span><span class="sxs-lookup"><span data-stu-id="5e7f1-454">Currency</span></span> |<span data-ttu-id="5e7f1-455">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-455">Currency type.</span></span> <span data-ttu-id="5e7f1-456">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-456">Each billing entity has only one currency.</span></span> <span data-ttu-id="5e7f1-457">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-457">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="5e7f1-458">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="5e7f1-458">DiscountDetails</span></span> |<span data-ttu-id="5e7f1-459">関連する割引の詳細を示す一覧。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-459">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="5e7f1-460">請求書と調整ファイルの間の課金のマッピング</span><span class="sxs-lookup"><span data-stu-id="5e7f1-460">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="5e7f1-461">請求書は料金の概要を示し、調整ファイルは、課金の種類を含め、行項目のトランザクションの詳細な内訳を示します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-461">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="5e7f1-462">請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルター オプションを使用して、調整ファイルの課金の種類でフィルター処理し、請求書の課金を調整ファイルの一連の課金の内訳にマップします。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-462">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="5e7f1-463">使用量ベースとライセンス ベースの調整ファイルには、使用量関連のトランザクションと料金 (消費された単位量および関連する料金) のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-463">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="5e7f1-464">請求書に “調整” として表示される単発のクレジット、割引、払い戻し金額は、調整ファイルに表示されません。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-464">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="5e7f1-465">次の表に、請求書のセクションと、調整ファイルに表示される関連付けられた課金の種類とのマッピングを示します。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-465">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="5e7f1-466">請求書の課金の説明</span><span class="sxs-lookup"><span data-stu-id="5e7f1-466">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="5e7f1-467">調整ファイルの課金の説明 (ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="5e7f1-467">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="5e7f1-468">この課金の意味</span><span class="sxs-lookup"><span data-stu-id="5e7f1-468">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="5e7f1-469">これらの ChargeTypes を請求書にマップする方法</span><span class="sxs-lookup"><span data-stu-id="5e7f1-469">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="5e7f1-470">ライセンス ベースの課金</span><span class="sxs-lookup"><span data-stu-id="5e7f1-470">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-471">Activation fee</span><span class="sxs-lookup"><span data-stu-id="5e7f1-471">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-472">購入したサブスクリプションを顧客が使用したときに顧客に課金される金額</span><span class="sxs-lookup"><span data-stu-id="5e7f1-472">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="5e7f1-473">ライセンスベースのファイルから、<strong>Amount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="5e7f1-473">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5e7f1-474">取り消し料金</span><span class="sxs-lookup"><span data-stu-id="5e7f1-474">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-475">関連付けられているシートが変更されたときに顧客に払い戻される日割り料金</span><span class="sxs-lookup"><span data-stu-id="5e7f1-475">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5e7f1-476">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="5e7f1-476">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-477">サブスクリプションの定期的な課金</span><span class="sxs-lookup"><span data-stu-id="5e7f1-477">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5e7f1-478">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="5e7f1-478">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-479">関連付けられているシートが変更されたときに顧客から評価される日割り料金</span><span class="sxs-lookup"><span data-stu-id="5e7f1-479">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5e7f1-480">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="5e7f1-480">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-481">取り消し時のサービスの未使用部分に対する日割りの払戻し額</span><span class="sxs-lookup"><span data-stu-id="5e7f1-481">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5e7f1-482">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="5e7f1-482">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-483">購入時の日割りの料金</span><span class="sxs-lookup"><span data-stu-id="5e7f1-483">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5e7f1-484">Purchase fee</span><span class="sxs-lookup"><span data-stu-id="5e7f1-484">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-485">サブスクリプションの最初の課金</span><span class="sxs-lookup"><span data-stu-id="5e7f1-485">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5e7f1-486">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="5e7f1-486">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-487">サブスクリプションの更新時の日割り料金</span><span class="sxs-lookup"><span data-stu-id="5e7f1-487">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="5e7f1-488">Renew fee</span><span class="sxs-lookup"><span data-stu-id="5e7f1-488">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-489">サブスクリプションの更新時の課金</span><span class="sxs-lookup"><span data-stu-id="5e7f1-489">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5e7f1-490">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="5e7f1-490">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-491">アクティブ化から課金期間の終了までの日割り料金</span><span class="sxs-lookup"><span data-stu-id="5e7f1-491">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="5e7f1-492">利用料金</span><span class="sxs-lookup"><span data-stu-id="5e7f1-492">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-493">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="5e7f1-493">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-494">現在の課金期間中に未払いの使用を取り消したときのアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="5e7f1-494">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="5e7f1-495">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="5e7f1-495">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5e7f1-496">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="5e7f1-496">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-497">現在の課金期間のアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="5e7f1-497">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="5e7f1-498">クレジット</span><span class="sxs-lookup"><span data-stu-id="5e7f1-498">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-499">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="5e7f1-499">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-500">税金を含む、行項目への一部または全部の払戻し</span><span class="sxs-lookup"><span data-stu-id="5e7f1-500">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-501">ライセンス ベースのファイルから、<strong>TotalForCustomer</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="5e7f1-501">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="5e7f1-502">使用量ベースのファイルから、<strong>PostTaxTotal</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="5e7f1-502">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="5e7f1-503">使用量ベースの割引</span><span class="sxs-lookup"><span data-stu-id="5e7f1-503">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-504">Activation discount</span><span class="sxs-lookup"><span data-stu-id="5e7f1-504">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-505">サブスクリプションがアクティブ化されたときに適用される割引</span><span class="sxs-lookup"><span data-stu-id="5e7f1-505">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="5e7f1-506">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="5e7f1-506">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5e7f1-507">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="5e7f1-507">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-508">定期的な課金に適用される割引</span><span class="sxs-lookup"><span data-stu-id="5e7f1-508">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5e7f1-509">Renew discount</span><span class="sxs-lookup"><span data-stu-id="5e7f1-509">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-510">サブスクリプションの更新時に適用される割引</span><span class="sxs-lookup"><span data-stu-id="5e7f1-510">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5e7f1-511">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="5e7f1-511">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-512">割引が取り消されたときに適用される料金</span><span class="sxs-lookup"><span data-stu-id="5e7f1-512">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="5e7f1-513">ライセンス ベースの割引</span><span class="sxs-lookup"><span data-stu-id="5e7f1-513">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="5e7f1-514">複数の種類の料金に適用される場合がある</span><span class="sxs-lookup"><span data-stu-id="5e7f1-514">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-515">ライセンス ベースのファイルから、<strong>TotalOtherDiscount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="5e7f1-515">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="5e7f1-516"><strong>税</strong>&nbsp;または&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="5e7f1-516"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="5e7f1-517">複数の種類の料金に適用される場合がある</span><span class="sxs-lookup"><span data-stu-id="5e7f1-517">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="5e7f1-518">例外: "Offset a line item" には既に税が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-518">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="5e7f1-519">上記のクレジットを参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e7f1-519">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-520">税または付加価値税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="5e7f1-520">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="5e7f1-521">ライセンス ベースのファイルから、<strong>Tax</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="5e7f1-521">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="5e7f1-522">使用量ベースのファイルから、<strong>TaxAmount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="5e7f1-522">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
