---
title: 調整ファイルの使用 | パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: 各料金が請求サイクルでの行項目の詳細なビューでは、パートナー センターから、調整ファイルをダウンロードします。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0d986ca81e77578ecbb79b909d8f2a8afc4777e4
ms.sourcegitcommit: 275d3eee5613d52f0ac7b8c78f7a7ddd74f56c9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/10/2019
ms.locfileid: "59430201"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="a2381-103">調整ファイルを使う</span><span class="sxs-lookup"><span data-stu-id="a2381-103">Use the reconciliation files</span></span>

**<span data-ttu-id="a2381-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="a2381-104">Applies to</span></span>**

-  <span data-ttu-id="a2381-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="a2381-105">Partner Center</span></span>
-  <span data-ttu-id="a2381-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="a2381-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="a2381-107">各料金が請求サイクルでの行項目の詳細なビューでは、パートナー センターから、調整ファイルをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="a2381-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="a2381-108">詳細には、各顧客のサブスクリプションの料金や、詳細なイベント (期間途中でのサブスクリプションへのシートの追加など) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a2381-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="a2381-109">書式設定の問題</span><span class="sxs-lookup"><span data-stu-id="a2381-109">Formatting issues</span></span>

<span data-ttu-id="a2381-110">場合によっては、偵察ファイルには、書式設定の問題があります。</span><span class="sxs-lookup"><span data-stu-id="a2381-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="a2381-111">(これに、たとえば、EN-US ロケールを使用しない場合。)これらの問題を修正するのには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="a2381-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="a2381-112">Excel では、.csv ファイルを開き、最初の列を選択します。</span><span class="sxs-lookup"><span data-stu-id="a2381-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="a2381-113">リボンで、次のように選択します。<strong>データ</strong>、し、<strong>列にテキスト</strong>します。</span><span class="sxs-lookup"><span data-stu-id="a2381-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="a2381-114">ウィザードの列にテキストを変換で次のように選択します。<strong>ファイルの種類の区切り</strong>、し、<strong>次</strong>。</span><span class="sxs-lookup"><span data-stu-id="a2381-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="a2381-115">区切り文字フィールドで、選択<strong>コンマ</strong>します。</span><span class="sxs-lookup"><span data-stu-id="a2381-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="a2381-116">場合<strong>タブ</strong>が既に選択されているおくことが可能にします。</span><span class="sxs-lookup"><span data-stu-id="a2381-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="a2381-117"><strong>[次へ]</strong> を選びます。</span><span class="sxs-lookup"><span data-stu-id="a2381-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="a2381-118">列のデータ形式のフィールドで選択<strong>日付。年 (mdy)</strong>、し、<strong>次</strong>します。</span><span class="sxs-lookup"><span data-stu-id="a2381-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="a2381-119">列のデータ形式のフィールドで選択<strong>テキスト</strong>列、および選択しすべて金額の<strong>完了</strong>します。</span><span class="sxs-lookup"><span data-stu-id="a2381-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="a2381-120">パートナーによって明細化します。</span><span class="sxs-lookup"><span data-stu-id="a2381-120">Itemize by partner</span></span>


<span data-ttu-id="a2381-121">インダイレクト モデルのパートナーは、ライセンス ベースの調整ファイルと使用量ベースの調整ファイルの両方で、これらの追加フィールドを使用してリセラーごとに明細を記載できます。</span><span class="sxs-lookup"><span data-stu-id="a2381-121">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="a2381-122">MPN ID</span><span class="sxs-lookup"><span data-stu-id="a2381-122">MPN ID</span></span></th>
<th><span data-ttu-id="a2381-123">説明</span><span class="sxs-lookup"><span data-stu-id="a2381-123">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="a2381-124">MPN ID</span><span class="sxs-lookup"><span data-stu-id="a2381-124">MPN ID</span></span></td>
<td><p><span data-ttu-id="a2381-125">CSP パートナー (直接または間接) の Microsoft Partner Network (MPN) IDです。</span><span class="sxs-lookup"><span data-stu-id="a2381-125">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-126">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="a2381-126">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="a2381-127">インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="a2381-127">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="a2381-128">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-128">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="a2381-129">これは、パートナー センターで特定のサブスクリプションについて示されるリセラー ID に対応します。</span><span class="sxs-lookup"><span data-stu-id="a2381-129">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="a2381-130">などの表示または更新、再販業者、パートナー センターのメニューから選択<strong>顧客</strong>、一覧から顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="a2381-130">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="a2381-131">顧客メニューの <strong>[サブスクリプション]</strong> を選び、一覧からサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="a2381-131">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="a2381-132"><strong>[更新]</strong> を選んで、<strong>[再販業者 (MPN ID)]</strong> を変更します。</span><span class="sxs-lookup"><span data-stu-id="a2381-132">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="a2381-133">CSP パートナーがお客様に直接サブスクリプションを販売した場合、パートナーの MPN ID が MPN ID とリセラーの MPN ID として 2 か所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="a2381-133">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="a2381-134">CSP パートナーのリセラーに MPN ID がない場合は、代わりに CSP パートナーの MPN ID がこの値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="a2381-134">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="a2381-135">CSP パートナーがリセラー ID を削除した場合、この値は -1 に設定されます。</span><span class="sxs-lookup"><span data-stu-id="a2381-135">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="a2381-136">ライセンス ベースのファイル フィールド</span><span class="sxs-lookup"><span data-stu-id="a2381-136">License-based file fields</span></span>


<span data-ttu-id="a2381-137">顧客の注文に対する料金を調整するには、調整ファイルの Syndication\_Partner\_Subscription\_Number とパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="a2381-137">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="a2381-138">列</span><span class="sxs-lookup"><span data-stu-id="a2381-138">Column</span></span></strong></td>
<td><strong><span data-ttu-id="a2381-139">説明</span><span class="sxs-lookup"><span data-stu-id="a2381-139">Description</span></span></strong></td>
<td><strong><span data-ttu-id="a2381-140">サンプル値</span><span class="sxs-lookup"><span data-stu-id="a2381-140">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-141">PartnerId</span><span class="sxs-lookup"><span data-stu-id="a2381-141">PartnerId</span></span></td>
<td><p><span data-ttu-id="a2381-142">特定の課金エンティティの一意の識別子 (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="a2381-142">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="a2381-143">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="a2381-143">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="a2381-144">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="a2381-144">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="a2381-145">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="a2381-145">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-146">CustomerID</span><span class="sxs-lookup"><span data-stu-id="a2381-146">CustomerID</span></span></td>
<td><p><span data-ttu-id="a2381-147">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-147">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="a2381-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="a2381-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-149">OrderID</span><span class="sxs-lookup"><span data-stu-id="a2381-149">OrderID</span></span></td>
<td><p><span data-ttu-id="a2381-150">Microsoft 請求プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="a2381-150">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="a2381-151">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="a2381-151">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="a2381-152">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="a2381-152">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-153">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="a2381-153">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="a2381-154">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="a2381-154">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="a2381-155">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="a2381-155">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="a2381-156">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="a2381-156">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="a2381-157">「Syndication_Partner_Subscription_Number」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a2381-157">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="a2381-158">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="a2381-158">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-159">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="a2381-159">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="a2381-160">サブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="a2381-160">Unique identifier for subscriptions.</span></span> <span data-ttu-id="a2381-161">お客様は同じプランで複数のサブスクリプションを持つことができるため、これは調整ファイルの分析で重要です。</span><span class="sxs-lookup"><span data-stu-id="a2381-161">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="a2381-162">このフィールドは、パートナー管理コンソールのサブスクリプション ID にマップされます。</span><span class="sxs-lookup"><span data-stu-id="a2381-162">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="a2381-163">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="a2381-163">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-164">OfferID</span><span class="sxs-lookup"><span data-stu-id="a2381-164">OfferID</span></span></td>
<td><p><span data-ttu-id="a2381-165">一意のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-165">Unique offer ID.</span></span> <span data-ttu-id="a2381-166">価格表に従った標準のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-166">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="a2381-167"><b>注意</b>:この値では、価格表からプラン ID が一致しません。</span><span class="sxs-lookup"><span data-stu-id="a2381-167"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="a2381-168">以下の DurableOfferID を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2381-168">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="a2381-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="a2381-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-170">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="a2381-170">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="a2381-171">価格表で定義されている一意の継続的なプラン ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-171">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="a2381-172"><b>注意</b>:この値は、価格表からプラン ID と一致します。</span><span class="sxs-lookup"><span data-stu-id="a2381-172"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="a2381-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="a2381-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-174">OfferName</span><span class="sxs-lookup"><span data-stu-id="a2381-174">OfferName</span></span></td>
<td><p><span data-ttu-id="a2381-175">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="a2381-175">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="a2381-176">Microsoft Office 365 (プラン E3)</span><span class="sxs-lookup"><span data-stu-id="a2381-176">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-177">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="a2381-177">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="a2381-178">サブスクリプションの開始日。注文が送信された日に設定されます。</span><span class="sxs-lookup"><span data-stu-id="a2381-178">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="a2381-179">サブスクリプションの開始日を終了日と共に確認することにより、顧客がサブスクリプションの最初の 1 年以内であるか、サブスクリプションが次の 1 年間更新されたかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="a2381-179">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="a2381-180">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="a2381-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="a2381-181">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="a2381-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-182">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="a2381-182">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="a2381-183">サブスクリプションの終了日:12 か月 + x 日間 (パートナーの請求日の連携) を開始日より後または更新日から 12 か月です。</span><span class="sxs-lookup"><span data-stu-id="a2381-183">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="a2381-184">更新時に、価格は最新の価格表に更新されます。</span><span class="sxs-lookup"><span data-stu-id="a2381-184">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="a2381-185">自動更新の前に、顧客とのやり取りが必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="a2381-185">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="a2381-186">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="a2381-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="a2381-187">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="a2381-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-188">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="a2381-188">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="a2381-189">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="a2381-189">Start day of the charges.</span></span></p>
<p><span data-ttu-id="a2381-190">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="a2381-190">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="a2381-191">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="a2381-191">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="a2381-192">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="a2381-192">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-193">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="a2381-193">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="a2381-194">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="a2381-194">End day of the charges.</span></span></p>
<p><span data-ttu-id="a2381-195">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="a2381-195">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="a2381-196">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="a2381-196">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="a2381-197">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="a2381-197">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-198">ChargeType</span><span class="sxs-lookup"><span data-stu-id="a2381-198">ChargeType</span></span></td>
<td><p><span data-ttu-id="a2381-199">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="a2381-199">The type of charge or adjustment.</span></span> <span data-ttu-id="a2381-200">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2381-200">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="a2381-201">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2381-201">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-202">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="a2381-202">UnitPrice</span></span></td>
<td><p><span data-ttu-id="a2381-203">シート単価 (購入時に価格表に公開されていた価格)。</span><span class="sxs-lookup"><span data-stu-id="a2381-203">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="a2381-204">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="a2381-204">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="a2381-205">6.82</span><span class="sxs-lookup"><span data-stu-id="a2381-205">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-206">Quantity</span><span class="sxs-lookup"><span data-stu-id="a2381-206">Quantity</span></span></td>
<td><p><span data-ttu-id="a2381-207">シート数。</span><span class="sxs-lookup"><span data-stu-id="a2381-207">Number of seats.</span></span> <span data-ttu-id="a2381-208">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="a2381-208">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="a2381-209">2</span><span class="sxs-lookup"><span data-stu-id="a2381-209">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-210">金額</span><span class="sxs-lookup"><span data-stu-id="a2381-210">Amount</span></span></td>
<td><p><span data-ttu-id="a2381-211">数量に対する合計価格。</span><span class="sxs-lookup"><span data-stu-id="a2381-211">Total of price for quantity.</span></span> <span data-ttu-id="a2381-212">金額の計算が、この顧客用の計算方法に一致することを確認するために役立ちます。</span><span class="sxs-lookup"><span data-stu-id="a2381-212">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="a2381-213">13.32</span><span class="sxs-lookup"><span data-stu-id="a2381-213">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-214">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="a2381-214">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="a2381-215">これらの料金に適用される割引額。</span><span class="sxs-lookup"><span data-stu-id="a2381-215">Amount of discount applied to these charges.</span></span> <span data-ttu-id="a2381-216">インセンティブの対象となる IUR または新しいサブスクリプションの場合も、この列に割引額が含まれます。</span><span class="sxs-lookup"><span data-stu-id="a2381-216">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="a2381-217">2.32</span><span class="sxs-lookup"><span data-stu-id="a2381-217">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-218">Subtotal</span><span class="sxs-lookup"><span data-stu-id="a2381-218">Subtotal</span></span></td>
<td><p><span data-ttu-id="a2381-219">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="a2381-219">Total before tax.</span></span> <span data-ttu-id="a2381-220">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="a2381-220">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="a2381-221">11</span><span class="sxs-lookup"><span data-stu-id="a2381-221">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-222">Tax</span><span class="sxs-lookup"><span data-stu-id="a2381-222">Tax</span></span></td>
<td><p><span data-ttu-id="a2381-223">市場に基づく、量の料金に税&#39;s 税法規と特定の状況です。</span><span class="sxs-lookup"><span data-stu-id="a2381-223">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="a2381-224">0</span><span class="sxs-lookup"><span data-stu-id="a2381-224">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-225">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="a2381-225">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="a2381-226">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="a2381-226">Total after tax.</span></span> <span data-ttu-id="a2381-227">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="a2381-227">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="a2381-228">11</span><span class="sxs-lookup"><span data-stu-id="a2381-228">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-229">通貨</span><span class="sxs-lookup"><span data-stu-id="a2381-229">Currency</span></span></td>
<td><p><span data-ttu-id="a2381-230">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="a2381-230">Currency type.</span></span> <span data-ttu-id="a2381-231">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="a2381-231">Each billing entity has only one currency.</span></span> <span data-ttu-id="a2381-232">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="a2381-232">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="a2381-233">EUR</span><span class="sxs-lookup"><span data-stu-id="a2381-233">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-234">CustomerName</span><span class="sxs-lookup"><span data-stu-id="a2381-234">CustomerName</span></span></td>
<td><p><span data-ttu-id="a2381-235">顧客&#39;パートナー センターで報告される組織名。</span><span class="sxs-lookup"><span data-stu-id="a2381-235">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="a2381-236">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="a2381-236">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="a2381-237">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="a2381-237">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-238">MPNID</span><span class="sxs-lookup"><span data-stu-id="a2381-238">MPNID</span></span></td>
<td><p><span data-ttu-id="a2381-239">CSP パートナーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="a2381-239">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="a2381-240">4390934</span><span class="sxs-lookup"><span data-stu-id="a2381-240">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-241">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="a2381-241">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="a2381-242">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-242">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="a2381-243">「<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">パートナーごとに明細を示す</a>」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a2381-243">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="a2381-244">4390934</span><span class="sxs-lookup"><span data-stu-id="a2381-244">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-245">DomainName</span><span class="sxs-lookup"><span data-stu-id="a2381-245">DomainName</span></span></td>
<td><p><span data-ttu-id="a2381-246">顧客&#39;のドメインの名前、顧客を識別するために使用します。</span><span class="sxs-lookup"><span data-stu-id="a2381-246">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="a2381-247">これを使用すると、顧客またはパートナーは O365 ポータルを使用して、バニティ/既定のドメインを更新できるように、ユーザーを一意に識別する必要がありますされません。</span><span class="sxs-lookup"><span data-stu-id="a2381-247">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="a2381-248">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a2381-248">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="a2381-249">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="a2381-249">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-250">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="a2381-250">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="a2381-251">サブスクリプションのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="a2381-251">Subscription nickname.</span></span> <span data-ttu-id="a2381-252">ニックネームが指定されていない場合、パートナー センターでは OfferName を使用します。</span><span class="sxs-lookup"><span data-stu-id="a2381-252">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="a2381-253">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="a2381-253">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-254">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="a2381-254">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="a2381-255">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="a2381-255">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="a2381-256">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="a2381-256">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="a2381-257">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span><span class="sxs-lookup"><span data-stu-id="a2381-257">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="a2381-258">ファイルの使用法に基づくフィールド</span><span class="sxs-lookup"><span data-stu-id="a2381-258">Usage-based file fields</span></span>


<span data-ttu-id="a2381-259">顧客の使用量に対する料金を調整するには、調整ファイルの ResellerID/ResellerName/ResellerBillableAccount、顧客名、およびパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="a2381-259">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="a2381-260">次のフィールドで、どのサービスが使用されるか、およびレートについて説明します。</span><span class="sxs-lookup"><span data-stu-id="a2381-260">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="a2381-261">列</span><span class="sxs-lookup"><span data-stu-id="a2381-261">Column</span></span></strong></td>
<td><strong><span data-ttu-id="a2381-262">説明</span><span class="sxs-lookup"><span data-stu-id="a2381-262">Description</span></span></strong></td>
<td><strong><span data-ttu-id="a2381-263">サンプル値</span><span class="sxs-lookup"><span data-stu-id="a2381-263">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-264">PartnerID</span><span class="sxs-lookup"><span data-stu-id="a2381-264">PartnerID</span></span></td>
<td><p><span data-ttu-id="a2381-265">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-265">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="a2381-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="a2381-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-267">PartnerName</span><span class="sxs-lookup"><span data-stu-id="a2381-267">PartnerName</span></span></td>
<td><p><span data-ttu-id="a2381-268">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="a2381-268">Partner Name.</span></span></p></td>
<td><span data-ttu-id="a2381-269">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="a2381-269">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-270">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="a2381-270">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="a2381-271">パートナーのアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-271">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="a2381-272">1010578050</span><span class="sxs-lookup"><span data-stu-id="a2381-272">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-273">CustomerName</span><span class="sxs-lookup"><span data-stu-id="a2381-273">CustomerName</span></span></td>
<td><p><span data-ttu-id="a2381-274">顧客&#39;パートナー センターで報告される組織名。</span><span class="sxs-lookup"><span data-stu-id="a2381-274">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="a2381-275">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="a2381-275">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="a2381-276">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="a2381-276">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-277">MPNID</span><span class="sxs-lookup"><span data-stu-id="a2381-277">MPNID</span></span></td>
<td><p><span data-ttu-id="a2381-278">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-278">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="a2381-279">4390934</span><span class="sxs-lookup"><span data-stu-id="a2381-279">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-280">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="a2381-280">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="a2381-281">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-281">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="a2381-282">「<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">パートナーごとに明細を示す</a>」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a2381-282">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="a2381-283">4390934</span><span class="sxs-lookup"><span data-stu-id="a2381-283">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-284">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="a2381-284">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="a2381-285">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="a2381-285">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="a2381-286">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="a2381-286">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-287">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="a2381-287">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="a2381-288">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="a2381-288">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="a2381-289">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="a2381-289">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="a2381-290">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="a2381-290">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-291">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="a2381-291">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="a2381-292">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="a2381-292">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="a2381-293">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="a2381-293">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="a2381-294">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="a2381-294">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-295">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="a2381-295">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="a2381-296">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="a2381-296">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="a2381-297">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="a2381-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="a2381-298">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="a2381-298">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="a2381-299">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="a2381-299">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-300">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="a2381-300">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="a2381-301">サービス プランのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="a2381-301">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="a2381-302">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="a2381-302">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-303">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="a2381-303">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="a2381-304">サービス プランの基幹業務</span><span class="sxs-lookup"><span data-stu-id="a2381-304">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="a2381-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="a2381-305">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-306">OrderID</span><span class="sxs-lookup"><span data-stu-id="a2381-306">OrderID</span></span></td>
<td><p><span data-ttu-id="a2381-307">Microsoft 請求プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="a2381-307">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="a2381-308">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="a2381-308">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="a2381-309">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="a2381-309">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-310">ServiceName</span><span class="sxs-lookup"><span data-stu-id="a2381-310">ServiceName</span></span></td>
<td><p><span data-ttu-id="a2381-311">対象の Azure サービスの名前。</span><span class="sxs-lookup"><span data-stu-id="a2381-311">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="a2381-312">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="a2381-312">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-313">ServiceType</span><span class="sxs-lookup"><span data-stu-id="a2381-313">ServiceType</span></span></td>
<td><p><span data-ttu-id="a2381-314">Windows Azure サービスの特定の種類。</span><span class="sxs-lookup"><span data-stu-id="a2381-314">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="a2381-315">Service Bus – Individual or Pack</span><span class="sxs-lookup"><span data-stu-id="a2381-315">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="a2381-316">SQL Azure database – Business or Web Edition</span><span class="sxs-lookup"><span data-stu-id="a2381-316">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-317">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="a2381-317">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="a2381-318">すべてのサービス データおよび価格設定構造の特定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="a2381-318">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="a2381-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="a2381-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-320">リソース名</span><span class="sxs-lookup"><span data-stu-id="a2381-320">Resource Name</span></span></td>
<td><p><span data-ttu-id="a2381-321">Azure リソースの名前。</span><span class="sxs-lookup"><span data-stu-id="a2381-321">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="a2381-322">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="a2381-322">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="a2381-323">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="a2381-323">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-324">Region</span><span class="sxs-lookup"><span data-stu-id="a2381-324">Region</span></span></td>
<td><p><span data-ttu-id="a2381-325">使用量が適用される地域。</span><span class="sxs-lookup"><span data-stu-id="a2381-325">The region the usage applies to.</span></span> <span data-ttu-id="a2381-326">料金は地域によって異なるため、主にデータ転送に料金を割り当てるために使われます。</span><span class="sxs-lookup"><span data-stu-id="a2381-326">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="a2381-327">Asia Pacific、Europe、Latin America、North America</span><span class="sxs-lookup"><span data-stu-id="a2381-327">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-328">SKU</span><span class="sxs-lookup"><span data-stu-id="a2381-328">SKU</span></span></td>
<td><p><span data-ttu-id="a2381-329">プランについての MSFT の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="a2381-329">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="a2381-330">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="a2381-330">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="a2381-331">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="a2381-331">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="a2381-332">特定の課金期間のサービスまたはリソースに対してさまざまなレートの明細を設定するための ID と数量。</span><span class="sxs-lookup"><span data-stu-id="a2381-332">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="a2381-333">Azure の階層化されたレーティングの場合は、一定数量の課金可能単位までは 1 つのレートがあり、その後に別のレートがあることがあります。</span><span class="sxs-lookup"><span data-stu-id="a2381-333">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="a2381-334">1</span><span class="sxs-lookup"><span data-stu-id="a2381-334">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-335">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="a2381-335">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="a2381-336">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="a2381-336">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="a2381-337">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="a2381-337">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="a2381-338">11</span><span class="sxs-lookup"><span data-stu-id="a2381-338">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-339">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="a2381-339">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="a2381-340">単位数はプランの一部として含まれます。</span><span class="sxs-lookup"><span data-stu-id="a2381-340">Units included as part of the offer.</span></span> <span data-ttu-id="a2381-341">通常、CSP には含まれません。</span><span class="sxs-lookup"><span data-stu-id="a2381-341">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="a2381-342">0</span><span class="sxs-lookup"><span data-stu-id="a2381-342">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="a2381-343">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="a2381-343">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="a2381-344">単位数はプランの一部として含まれず、パートナーが支払う必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2381-344">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="a2381-345">ConsumedQuantity - IncludedQuantity と同じです。</span><span class="sxs-lookup"><span data-stu-id="a2381-345">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="a2381-346">11</span><span class="sxs-lookup"><span data-stu-id="a2381-346">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-347">ListPrice</span><span class="sxs-lookup"><span data-stu-id="a2381-347">ListPrice</span></span></td>
<td><p><span data-ttu-id="a2381-348">サブスクリプションの開始日に有効な価格を提供します。</span><span class="sxs-lookup"><span data-stu-id="a2381-348">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="a2381-349">$0.0808</span><span class="sxs-lookup"><span data-stu-id="a2381-349">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-350">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="a2381-350">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="a2381-351">ListPrist と OverageQuantity を掛けて、最も近いセントに丸めます。</span><span class="sxs-lookup"><span data-stu-id="a2381-351">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="a2381-352">$0.085</span><span class="sxs-lookup"><span data-stu-id="a2381-352">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-353">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="a2381-353">TaxAmount</span></span></td>
<td><p><span data-ttu-id="a2381-354">市場に基づく、量の料金に税&#39;s 税法規と特定の状況です。</span><span class="sxs-lookup"><span data-stu-id="a2381-354">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="a2381-355">$0.08</span><span class="sxs-lookup"><span data-stu-id="a2381-355">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-356">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="a2381-356">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="a2381-357">税が適用されるときの税引き後の合計額。</span><span class="sxs-lookup"><span data-stu-id="a2381-357">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="a2381-358">$0.93</span><span class="sxs-lookup"><span data-stu-id="a2381-358">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-359">通貨</span><span class="sxs-lookup"><span data-stu-id="a2381-359">Currency</span></span></td>
<td><p><span data-ttu-id="a2381-360">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="a2381-360">Currency type.</span></span> <span data-ttu-id="a2381-361">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="a2381-361">Each billing entity has only one currency.</span></span> <span data-ttu-id="a2381-362">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="a2381-362">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="a2381-363">EUR</span><span class="sxs-lookup"><span data-stu-id="a2381-363">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-364">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="a2381-364">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="a2381-365">単位あたりの税込み価格。</span><span class="sxs-lookup"><span data-stu-id="a2381-365">Pretax price per unit.</span></span> <span data-ttu-id="a2381-366">PretaxCharges / OverageQuantity と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="a2381-366">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="a2381-367">$0.08</span><span class="sxs-lookup"><span data-stu-id="a2381-367">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-368">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="a2381-368">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="a2381-369">単位あたりの税引き後の価格。</span><span class="sxs-lookup"><span data-stu-id="a2381-369">Post tax price per unit.</span></span> <span data-ttu-id="a2381-370">PostTaxTotal / OverageQuantity、または PretaxEffectiveRate + 単位額あたりの税率と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="a2381-370">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="a2381-371">$0.08</span><span class="sxs-lookup"><span data-stu-id="a2381-371">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-372">ChargeType</span><span class="sxs-lookup"><span data-stu-id="a2381-372">ChargeType</span></span></td>
<td><p><span data-ttu-id="a2381-373">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="a2381-373">The type of charge or adjustment.</span></span> <span data-ttu-id="a2381-374">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2381-374">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="a2381-375">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2381-375">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-376">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="a2381-376">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="a2381-377">MSFT 課金プラットフォームの一意のアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-377">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="a2381-378">1280018095</span><span class="sxs-lookup"><span data-stu-id="a2381-378">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-379">UsageDate</span><span class="sxs-lookup"><span data-stu-id="a2381-379">UsageDate</span></span></td>
<td><p><span data-ttu-id="a2381-380">サービスの展開の日付。</span><span class="sxs-lookup"><span data-stu-id="a2381-380">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="a2381-381">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="a2381-381">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-382">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="a2381-382">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="a2381-383">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="a2381-383">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="a2381-384">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="a2381-384">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-385">MeteredService</span><span class="sxs-lookup"><span data-stu-id="a2381-385">MeteredService</span></span></td>
<td><p><span data-ttu-id="a2381-386">この列は、[Service Name] 列で特に識別されない可能性のある、個別の Microsoft Azure サービスの追跡に利用されます。</span><span class="sxs-lookup"><span data-stu-id="a2381-386">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="a2381-387">たとえば、データ転送は、[Service Name] 列で &quot;Microsoft Azure - All Services&quot; と報告されます。</span><span class="sxs-lookup"><span data-stu-id="a2381-387">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="a2381-388">この [MeteredService] 列は、利用に関連する特定のサービスを示します。</span><span class="sxs-lookup"><span data-stu-id="a2381-388">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="a2381-389">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="a2381-389">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-390">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="a2381-390">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="a2381-391">個々の Microsoft Azure サービスの内容を、MeteredService フィールドで提供されるレベルよりも明確にする小見出し。</span><span class="sxs-lookup"><span data-stu-id="a2381-391">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="a2381-392">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="a2381-392">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-393">Project</span><span class="sxs-lookup"><span data-stu-id="a2381-393">Project</span></span></td>
<td><p><span data-ttu-id="a2381-394">サービス インスタンスの顧客定義の名前</span><span class="sxs-lookup"><span data-stu-id="a2381-394">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="a2381-395">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="a2381-395">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-396">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="a2381-396">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="a2381-397">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="a2381-397">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="a2381-398">例: 1 か月 30 日間の中に、個別にプロビジョニングされた接続がある場合、Service Info 1 は "1.000000 Connections / 30 days" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="a2381-398">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="a2381-399">Service Bus 接続のプロビジョニングが 25 パックする必要があるし、その日に 1 つを利用して、その日、毎日の使用量明細を示す"25 接続/30 Days-Used:1.000000”.</span><span class="sxs-lookup"><span data-stu-id="a2381-399">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-400">CustomerID</span><span class="sxs-lookup"><span data-stu-id="a2381-400">CustomerID</span></span></td>
<td><p><span data-ttu-id="a2381-401">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-401">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="a2381-402">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="a2381-402">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a2381-403">DomainName</span><span class="sxs-lookup"><span data-stu-id="a2381-403">DomainName</span></span></td>
<td><p><span data-ttu-id="a2381-404">顧客&#39;のドメインの名前、顧客を識別するために使用します。</span><span class="sxs-lookup"><span data-stu-id="a2381-404">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="a2381-405">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a2381-405">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="a2381-406">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="a2381-406">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="a2381-407">Unit</span><span class="sxs-lookup"><span data-stu-id="a2381-407">Unit</span></span></td>
<td><p><span data-ttu-id="a2381-408">リソース名の単位</span><span class="sxs-lookup"><span data-stu-id="a2381-408">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="a2381-409">GB または HOURS</span><span class="sxs-lookup"><span data-stu-id="a2381-409">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="a2381-410">1 回だけ、定期的なファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="a2381-410">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="a2381-411">列</span><span class="sxs-lookup"><span data-stu-id="a2381-411">Column</span></span></th>
<th><span data-ttu-id="a2381-412">説明</span><span class="sxs-lookup"><span data-stu-id="a2381-412">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="a2381-413">PartnerId</span><span class="sxs-lookup"><span data-stu-id="a2381-413">PartnerId</span></span></td>
<td><p><span data-ttu-id="a2381-414">GUID 形式で、特定の課金エンティティの一意の Microsoft Azure Active Directory テナント識別子。</span><span class="sxs-lookup"><span data-stu-id="a2381-414">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="a2381-415">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="a2381-415">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="a2381-416">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="a2381-416">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-417">[Customer Id]</span><span class="sxs-lookup"><span data-stu-id="a2381-417">Customer Id</span></span></td>
<td><p><span data-ttu-id="a2381-418">一意な Microsoft Azure Active Directory テナント ID、GUID 形式で顧客を識別するために使用します。</span><span class="sxs-lookup"><span data-stu-id="a2381-418">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-419">顧客名</span><span class="sxs-lookup"><span data-stu-id="a2381-419">Customer Name</span></span></td>
<td><p><span data-ttu-id="a2381-420">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="a2381-420">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-421">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="a2381-421">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="a2381-422">顧客のドメイン名。顧客を特定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="a2381-422">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="a2381-423">これを使用すると、顧客またはパートナーは O365 ポータルを使用して、バニティ/既定のドメインを更新できるように、ユーザーを一意に識別する必要がありますされません。</span><span class="sxs-lookup"><span data-stu-id="a2381-423">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="a2381-424">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a2381-424">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-425">顧客の国</span><span class="sxs-lookup"><span data-stu-id="a2381-425">Customer Country</span></span></td>
<td><p><span data-ttu-id="a2381-426">顧客の在住国。</span><span class="sxs-lookup"><span data-stu-id="a2381-426">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-427">請求書番号</span><span class="sxs-lookup"><span data-stu-id="a2381-427">Invoice number</span></span></td>
<td><p><span data-ttu-id="a2381-428">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="a2381-428">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-429">MpnId</span><span class="sxs-lookup"><span data-stu-id="a2381-429">MpnId</span></span></td>
<td><p><span data-ttu-id="a2381-430">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-430">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-431">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="a2381-431">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="a2381-432">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-432">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-433">Order ID</span><span class="sxs-lookup"><span data-stu-id="a2381-433">Order ID</span></span></td>
<td><p><span data-ttu-id="a2381-434">マイクロソフト コマース プラットフォームでの注文の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a2381-434">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="a2381-435">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="a2381-435">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-436">発注日</span><span class="sxs-lookup"><span data-stu-id="a2381-436">Order date</span></span></td>
<td><p><span data-ttu-id="a2381-437">注文が作成された日付。</span><span class="sxs-lookup"><span data-stu-id="a2381-437">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-438">ProductId</span><span class="sxs-lookup"><span data-stu-id="a2381-438">ProductId</span></span></td>
<td><p><span data-ttu-id="a2381-439">製品の ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-439">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-440">SkuId</span><span class="sxs-lookup"><span data-stu-id="a2381-440">SkuId</span></span></td>
<td><p><span data-ttu-id="a2381-441">特定 SKU の ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-441">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-442">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="a2381-442">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="a2381-443">特定の可用性 の ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-443">The ID for a particular Availability.</span></span> <span data-ttu-id="a2381-444">"可用性" とは、特定の国、通貨、業界などで特定の SKU を購入可能かどうかを指します。</span><span class="sxs-lookup"><span data-stu-id="a2381-444">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-445">SKU 名</span><span class="sxs-lookup"><span data-stu-id="a2381-445">SKU Name</span></span></td>
<td><p><span data-ttu-id="a2381-446">特定 SKU のタイトル。</span><span class="sxs-lookup"><span data-stu-id="a2381-446">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-447">製品名</span><span class="sxs-lookup"><span data-stu-id="a2381-447">Product name</span></span></td>
<td><p><span data-ttu-id="a2381-448">製品の名前。</span><span class="sxs-lookup"><span data-stu-id="a2381-448">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-449">PublisherName</span><span class="sxs-lookup"><span data-stu-id="a2381-449">PublisherName</span></span></td>
<td><p><span data-ttu-id="a2381-450">製品のパブリッシャーの名前。</span><span class="sxs-lookup"><span data-stu-id="a2381-450">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-451">PublisherID</span><span class="sxs-lookup"><span data-stu-id="a2381-451">PublisherID</span></span></td>
<td><p><span data-ttu-id="a2381-452">このパブリッシャーに対して一意の ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-452">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-453">サブスクリプションの説明</span><span class="sxs-lookup"><span data-stu-id="a2381-453">Subscription Description</span></span></td>
<td><p><span data-ttu-id="a2381-454">サブスクリプションのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="a2381-454">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-455">サブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="a2381-455">Subscription ID</span></span></td>
<td><p><span data-ttu-id="a2381-456">マイクロソフト コマース プラットフォームでサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="a2381-456">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="a2381-457">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="a2381-457">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="a2381-458">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="a2381-458">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-459">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="a2381-459">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="a2381-460">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="a2381-460">Start day of the charges.</span></span> <span data-ttu-id="a2381-461">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="a2381-461">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-462">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="a2381-462">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="a2381-463">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="a2381-463">End day of the charges.</span></span> <span data-ttu-id="a2381-464">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="a2381-464">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-465">用語と Billingcycle</span><span class="sxs-lookup"><span data-stu-id="a2381-465">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="a2381-466">期間と購入の請求サイクルでします。</span><span class="sxs-lookup"><span data-stu-id="a2381-466">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="a2381-467">たとえば、「1 年、月単位です。」</span><span class="sxs-lookup"><span data-stu-id="a2381-467">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-468">請求の種類</span><span class="sxs-lookup"><span data-stu-id="a2381-468">Charge Type</span></span></td>
<td><p><span data-ttu-id="a2381-469">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="a2381-469">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-470">単価</span><span class="sxs-lookup"><span data-stu-id="a2381-470">Unit Price</span></span></td>
<td><p><span data-ttu-id="a2381-471">購入時、pricelist で発行される価格です。</span><span class="sxs-lookup"><span data-stu-id="a2381-471">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="a2381-472">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="a2381-472">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-473">効果的な単体の価格</span><span class="sxs-lookup"><span data-stu-id="a2381-473">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="a2381-474">調整が行われた後の単位の価格です。</span><span class="sxs-lookup"><span data-stu-id="a2381-474">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-475">Quantity</span><span class="sxs-lookup"><span data-stu-id="a2381-475">Quantity</span></span></td>
<td><p><span data-ttu-id="a2381-476">ユニットの数。</span><span class="sxs-lookup"><span data-stu-id="a2381-476">Number of units.</span></span> <span data-ttu-id="a2381-477">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="a2381-477">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-478">ユニットの種類</span><span class="sxs-lookup"><span data-stu-id="a2381-478">Unit type</span></span></td>
<td><p><span data-ttu-id="a2381-479">購入されているユニットの種類。</span><span class="sxs-lookup"><span data-stu-id="a2381-479">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-480">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="a2381-480">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="a2381-481">該当する何らかの割引の説明。</span><span class="sxs-lookup"><span data-stu-id="a2381-481">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-482">小計</span><span class="sxs-lookup"><span data-stu-id="a2381-482">Sub Total</span></span></td>
<td><p><span data-ttu-id="a2381-483">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="a2381-483">Total before tax.</span></span> <span data-ttu-id="a2381-484">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="a2381-484">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-485">売上税合計</span><span class="sxs-lookup"><span data-stu-id="a2381-485">Tax Total</span></span></td>
<td><p><span data-ttu-id="a2381-486">市場の税関連の規則や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="a2381-486">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-487">Total</span><span class="sxs-lookup"><span data-stu-id="a2381-487">Total</span></span></td>
<td><p><span data-ttu-id="a2381-488">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="a2381-488">Total after tax.</span></span> <span data-ttu-id="a2381-489">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="a2381-489">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-490">通貨</span><span class="sxs-lookup"><span data-stu-id="a2381-490">Currency</span></span></td>
<td><p><span data-ttu-id="a2381-491">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="a2381-491">Currency type.</span></span> <span data-ttu-id="a2381-492">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="a2381-492">Each billing entity has only one currency.</span></span> <span data-ttu-id="a2381-493">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="a2381-493">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-494">代替</span><span class="sxs-lookup"><span data-stu-id="a2381-494">AlternateID</span></span></td>
<td><p><span data-ttu-id="a2381-495">代替の識別子を注文 ID</span><span class="sxs-lookup"><span data-stu-id="a2381-495">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="a2381-496">評価の毎日の使用状況ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="a2381-496">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="a2381-497">列</span><span class="sxs-lookup"><span data-stu-id="a2381-497">Column</span></span></th>
<th><span data-ttu-id="a2381-498">説明</span><span class="sxs-lookup"><span data-stu-id="a2381-498">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="a2381-499">PartnerId</span><span class="sxs-lookup"><span data-stu-id="a2381-499">PartnerId</span></span></td>
<td><p><span data-ttu-id="a2381-500">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-500">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-501">PartnerName</span><span class="sxs-lookup"><span data-stu-id="a2381-501">PartnerName</span></span></td>
<td><p><span data-ttu-id="a2381-502">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="a2381-502">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-503">CustomerId</span><span class="sxs-lookup"><span data-stu-id="a2381-503">CustomerId</span></span></td>
<td><p><span data-ttu-id="a2381-504">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-504">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-505">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="a2381-505">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="a2381-506">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="a2381-506">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="a2381-507">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="a2381-507">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-508">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="a2381-508">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="a2381-509">顧客のドメイン名。</span><span class="sxs-lookup"><span data-stu-id="a2381-509">The customer’s domain name.</span></span> <span data-ttu-id="a2381-510">現在のアクティビティは使用できません。</span><span class="sxs-lookup"><span data-stu-id="a2381-510">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-511">顧客の国</span><span class="sxs-lookup"><span data-stu-id="a2381-511">Customer country</span></span></td>
<td><p><span data-ttu-id="a2381-512">顧客の在住国。</span><span class="sxs-lookup"><span data-stu-id="a2381-512">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-513">MPNID</span><span class="sxs-lookup"><span data-stu-id="a2381-513">MPNID</span></span></td>
<td><p><span data-ttu-id="a2381-514">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-514">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-515">Reseller MPNID</span><span class="sxs-lookup"><span data-stu-id="a2381-515">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="a2381-516">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-516">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="a2381-517">現在のアクティビティは使用できません。</span><span class="sxs-lookup"><span data-stu-id="a2381-517">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-518">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="a2381-518">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="a2381-519">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="a2381-519">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="a2381-520">現在のアクティビティは使用できません。</span><span class="sxs-lookup"><span data-stu-id="a2381-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-521">ProductId</span><span class="sxs-lookup"><span data-stu-id="a2381-521">ProductId</span></span></td>
<td><p><span data-ttu-id="a2381-522">製品の ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-522">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-523">SkuId</span><span class="sxs-lookup"><span data-stu-id="a2381-523">SkuId</span></span></td>
<td><p><span data-ttu-id="a2381-524">特定 SKU の ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-524">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-525">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="a2381-525">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="a2381-526">特定の可用性 の ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-526">The ID for a particular Availability.</span></span> <span data-ttu-id="a2381-527">"可用性" とは、特定の国、通貨、業界などで特定の SKU を購入可能かどうかを指します。</span><span class="sxs-lookup"><span data-stu-id="a2381-527">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-528">SKU 名</span><span class="sxs-lookup"><span data-stu-id="a2381-528">SKU Name</span></span></td>
<td><p><span data-ttu-id="a2381-529">特定 SKU のタイトル。</span><span class="sxs-lookup"><span data-stu-id="a2381-529">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-530">PublisherName</span><span class="sxs-lookup"><span data-stu-id="a2381-530">PublisherName</span></span></td>
<td><p><span data-ttu-id="a2381-531">パブリッシャーの名前。</span><span class="sxs-lookup"><span data-stu-id="a2381-531">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-532">PublisherID</span><span class="sxs-lookup"><span data-stu-id="a2381-532">PublisherID</span></span></td>
<td><p><span data-ttu-id="a2381-533">GUID 形式で、パブリッシャーの ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-533">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="a2381-534">現在のアクティビティは使用できません。</span><span class="sxs-lookup"><span data-stu-id="a2381-534">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="a2381-535">サブスクリプションの説明</span><span class="sxs-lookup"><span data-stu-id="a2381-535">Subscription Description</span></span></td>
<td><p><span data-ttu-id="a2381-536">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="a2381-536">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="a2381-537">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="a2381-537">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-538">サブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="a2381-538">Subscription ID</span></span></td>
<td><p><span data-ttu-id="a2381-539">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="a2381-539">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="a2381-540">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="a2381-540">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="a2381-541">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="a2381-541">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-542">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="a2381-542">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="a2381-543">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="a2381-543">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="a2381-544">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="a2381-544">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-545">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="a2381-545">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="a2381-546">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="a2381-546">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="a2381-547">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="a2381-547">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-548">使用日</span><span class="sxs-lookup"><span data-stu-id="a2381-548">Usage Date</span></span></td>
<td><p><span data-ttu-id="a2381-549">サービスの使用状況の日です。</span><span class="sxs-lookup"><span data-stu-id="a2381-549">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-550">メーターの種類</span><span class="sxs-lookup"><span data-stu-id="a2381-550">Meter Type</span></span></td>
<td><p><span data-ttu-id="a2381-551">測定の種類。</span><span class="sxs-lookup"><span data-stu-id="a2381-551">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-552">メーター カテゴリ</span><span class="sxs-lookup"><span data-stu-id="a2381-552">Meter Category</span></span></td>
<td><p><span data-ttu-id="a2381-553">使用状況の最上位のサービスです。</span><span class="sxs-lookup"><span data-stu-id="a2381-553">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-554">測定 Id</span><span class="sxs-lookup"><span data-stu-id="a2381-554">Meter Id</span></span></td>
<td><p><span data-ttu-id="a2381-555">使用されているメーターの ID。</span><span class="sxs-lookup"><span data-stu-id="a2381-555">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-556">測定サブカテゴリ</span><span class="sxs-lookup"><span data-stu-id="a2381-556">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="a2381-557">速度に影響を与える Azure サービスの型。</span><span class="sxs-lookup"><span data-stu-id="a2381-557">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-558">測定名</span><span class="sxs-lookup"><span data-stu-id="a2381-558">Meter Name</span></span></td>
<td><p><span data-ttu-id="a2381-559">消費しているメーターの測定単位。</span><span class="sxs-lookup"><span data-stu-id="a2381-559">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-560">メーター リージョン</span><span class="sxs-lookup"><span data-stu-id="a2381-560">Meter Region</span></span></td>
<td><p><span data-ttu-id="a2381-561">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="a2381-561">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-562">Unit</span><span class="sxs-lookup"><span data-stu-id="a2381-562">Unit</span></span></td>
<td><p><span data-ttu-id="a2381-563">リソース名の単位。</span><span class="sxs-lookup"><span data-stu-id="a2381-563">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-564">使用量</span><span class="sxs-lookup"><span data-stu-id="a2381-564">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="a2381-565">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="a2381-565">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="a2381-566">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="a2381-566">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-567">リソースの場所</span><span class="sxs-lookup"><span data-stu-id="a2381-567">Resource Location</span></span></td>
<td><p><span data-ttu-id="a2381-568">メーターが実行されているデータ センターです。</span><span class="sxs-lookup"><span data-stu-id="a2381-568">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-569">使用するサービス</span><span class="sxs-lookup"><span data-stu-id="a2381-569">Consumed Service</span></span></td>
<td><p><span data-ttu-id="a2381-570">使用して、Azure プラットフォーム サービスです。</span><span class="sxs-lookup"><span data-stu-id="a2381-570">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-571">リソース グループ</span><span class="sxs-lookup"><span data-stu-id="a2381-571">Resource Group</span></span></td>
<td><p><span data-ttu-id="a2381-572">デプロイされたメーターが実行されているリソース グループ。</span><span class="sxs-lookup"><span data-stu-id="a2381-572">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-573">リソース URI</span><span class="sxs-lookup"><span data-stu-id="a2381-573">Resource URI</span></span></td>
<td><p><span data-ttu-id="a2381-574">使用されているリソースの URI。</span><span class="sxs-lookup"><span data-stu-id="a2381-574">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-575">請求の種類</span><span class="sxs-lookup"><span data-stu-id="a2381-575">Charge type</span></span></td>
<td><p><span data-ttu-id="a2381-576">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="a2381-576">The type of charge or adjustment.</span></span> <span data-ttu-id="a2381-577">現在のアクティビティは使用できません。</span><span class="sxs-lookup"><span data-stu-id="a2381-577">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-578">単価</span><span class="sxs-lookup"><span data-stu-id="a2381-578">Unit price</span></span></td>
<td><p><span data-ttu-id="a2381-579">購入時、pricelist でパブリッシュされると、ライセンスあたりの価格。</span><span class="sxs-lookup"><span data-stu-id="a2381-579">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="a2381-580">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="a2381-580">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-581">Quantity</span><span class="sxs-lookup"><span data-stu-id="a2381-581">Quantity</span></span></td>
<td><p><span data-ttu-id="a2381-582">ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="a2381-582">Number of licenses.</span></span> <span data-ttu-id="a2381-583">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="a2381-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-584">ユニットの種類</span><span class="sxs-lookup"><span data-stu-id="a2381-584">Unit type</span></span></td>
<td><p><span data-ttu-id="a2381-585">メーターが課金単位の種類。</span><span class="sxs-lookup"><span data-stu-id="a2381-585">The type of unit the meter is charged in.</span></span> <span data-ttu-id="a2381-586">現在のアクティビティは使用できません。</span><span class="sxs-lookup"><span data-stu-id="a2381-586">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-587">前の税金を請求</span><span class="sxs-lookup"><span data-stu-id="a2381-587">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="a2381-588">税引き前に、の合計。</span><span class="sxs-lookup"><span data-stu-id="a2381-588">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-589">請求通貨</span><span class="sxs-lookup"><span data-stu-id="a2381-589">Billing currency</span></span></td>
<td><p><span data-ttu-id="a2381-590">顧客の地理的リージョン内の通貨</span><span class="sxs-lookup"><span data-stu-id="a2381-590">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-591">税込み合計を価格</span><span class="sxs-lookup"><span data-stu-id="a2381-591">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="a2381-592">価格の税が追加される前にします。</span><span class="sxs-lookup"><span data-stu-id="a2381-592">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-593">通貨の価格</span><span class="sxs-lookup"><span data-stu-id="a2381-593">Pricing currency</span></span></td>
<td><p><span data-ttu-id="a2381-594">Pricelist 通貨です。</span><span class="sxs-lookup"><span data-stu-id="a2381-594">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-595">サービス情報 1</span><span class="sxs-lookup"><span data-stu-id="a2381-595">Service Info 1</span></span></td>
<td><p><span data-ttu-id="a2381-596">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="a2381-596">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-597">サービス情報 2</span><span class="sxs-lookup"><span data-stu-id="a2381-597">Service Info 2</span></span></td>
<td><p><span data-ttu-id="a2381-598">省略可能なサービスに固有のメタデータをキャプチャするレガシ フィールドです。</span><span class="sxs-lookup"><span data-stu-id="a2381-598">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="a2381-599">Tags</span><span class="sxs-lookup"><span data-stu-id="a2381-599">Tags</span></span></td>
<td><p><span data-ttu-id="a2381-600">課金のレコードをグループ化の順序でメーターに割り当てるタグ。</span><span class="sxs-lookup"><span data-stu-id="a2381-600">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="a2381-601">たとえば、メーターを使用する部門ごとのコストを配布するのにタグを使用することができます。</span><span class="sxs-lookup"><span data-stu-id="a2381-601">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="a2381-602">追加情報</span><span class="sxs-lookup"><span data-stu-id="a2381-602">Additional Info</span></span></td>
<td><p><span data-ttu-id="a2381-603">追加情報は、他の列では説明しません。</span><span class="sxs-lookup"><span data-stu-id="a2381-603">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="a2381-604">請求書と調整ファイルの間の料金のマッピング</span><span class="sxs-lookup"><span data-stu-id="a2381-604">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="a2381-605">請求書は料金の概要を示し、調整ファイルは、課金の種類を含め、行項目のトランザクションの詳細な内訳を示します。</span><span class="sxs-lookup"><span data-stu-id="a2381-605">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="a2381-606">請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルター オプションを使用して、調整ファイルの課金の種類でフィルター処理し、請求書の課金を調整ファイルの一連の課金の内訳にマップします。</span><span class="sxs-lookup"><span data-stu-id="a2381-606">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="a2381-607">使用量ベースとライセンス ベースの調整ファイルには、使用量関連のトランザクションと料金 (消費された単位量および関連する料金) のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="a2381-607">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="a2381-608">請求書に “調整” として表示される単発のクレジット、割引、払い戻し金額は、調整ファイルに表示されません。</span><span class="sxs-lookup"><span data-stu-id="a2381-608">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="a2381-609">次の表に、請求書のセクションと、調整ファイルに表示される関連付けられた課金の種類とのマッピングを示します。</span><span class="sxs-lookup"><span data-stu-id="a2381-609">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="a2381-610">請求書の課金の説明</span><span class="sxs-lookup"><span data-stu-id="a2381-610">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="a2381-611">調整ファイルの課金の説明 (ChargeType 列)</span><span class="sxs-lookup"><span data-stu-id="a2381-611">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="a2381-612">この課金の意味</span><span class="sxs-lookup"><span data-stu-id="a2381-612">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="a2381-613">これらの ChargeTypes を請求書にマップする方法</span><span class="sxs-lookup"><span data-stu-id="a2381-613">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="a2381-614">ライセンスベースの料金</span><span class="sxs-lookup"><span data-stu-id="a2381-614">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="a2381-615">アクティブ化料金</span><span class="sxs-lookup"><span data-stu-id="a2381-615">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-616">購入したサブスクリプションを顧客が使用したときに顧客に課金される金額</span><span class="sxs-lookup"><span data-stu-id="a2381-616">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="a2381-617">ライセンスベースのファイルから、<strong>Amount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="a2381-617">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a2381-618">取り消し料金</span><span class="sxs-lookup"><span data-stu-id="a2381-618">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-619">関連付けられているシートが変更されたときに顧客に払い戻される日割り料金</span><span class="sxs-lookup"><span data-stu-id="a2381-619">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a2381-620">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="a2381-620">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-621">サブスクリプションの定期的な課金</span><span class="sxs-lookup"><span data-stu-id="a2381-621">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a2381-622">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="a2381-622">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-623">関連付けられているシートが変更されたときに顧客から評価される日割り料金</span><span class="sxs-lookup"><span data-stu-id="a2381-623">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a2381-624">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="a2381-624">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-625">取り消し時のサービスの未使用部分に対する日割りの払戻し額</span><span class="sxs-lookup"><span data-stu-id="a2381-625">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a2381-626">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="a2381-626">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-627">年次請求に使用する場合、サブスクリプションの料金タイプ</span><span class="sxs-lookup"><span data-stu-id="a2381-627">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a2381-628">Purchase fee</span><span class="sxs-lookup"><span data-stu-id="a2381-628">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-629">月額使用料を使用する場合、サブスクリプションの料金タイプ</span><span class="sxs-lookup"><span data-stu-id="a2381-629">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a2381-630">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="a2381-630">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-631">サブスクリプションの更新時の日割り料金</span><span class="sxs-lookup"><span data-stu-id="a2381-631">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="a2381-632">Renew fee</span><span class="sxs-lookup"><span data-stu-id="a2381-632">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-633">サブスクリプションの更新時の課金</span><span class="sxs-lookup"><span data-stu-id="a2381-633">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a2381-634">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="a2381-634">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-635">アクティブ化から課金期間の終了までの日割り料金</span><span class="sxs-lookup"><span data-stu-id="a2381-635">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="a2381-636">利用料金</span><span class="sxs-lookup"><span data-stu-id="a2381-636">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="a2381-637">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="a2381-637">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-638">現在の課金期間中に未払いの使用を取り消したときのアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="a2381-638">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="a2381-639">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="a2381-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a2381-640">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="a2381-640">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-641">現在の課金期間のアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="a2381-641">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="a2381-642">クレジット</span><span class="sxs-lookup"><span data-stu-id="a2381-642">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="a2381-643">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="a2381-643">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-644">税金を含む、行項目への一部または全部の払戻し</span><span class="sxs-lookup"><span data-stu-id="a2381-644">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-645">ライセンスベースのファイルから、<strong>TotalForCustomer</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="a2381-645">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="a2381-646">使用量ベースのファイルから、<strong>PostTaxTotal</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="a2381-646">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="a2381-647">使用量ベースの割引</span><span class="sxs-lookup"><span data-stu-id="a2381-647">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="a2381-648">Activation discount</span><span class="sxs-lookup"><span data-stu-id="a2381-648">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-649">サブスクリプションがアクティブ化されたときに適用される割引</span><span class="sxs-lookup"><span data-stu-id="a2381-649">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="a2381-650">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="a2381-650">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a2381-651">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="a2381-651">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-652">定期的な課金に適用される割引</span><span class="sxs-lookup"><span data-stu-id="a2381-652">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a2381-653">Renew discount</span><span class="sxs-lookup"><span data-stu-id="a2381-653">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-654">サブスクリプションの更新時に適用される割引</span><span class="sxs-lookup"><span data-stu-id="a2381-654">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a2381-655">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="a2381-655">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-656">割引が取り消されたときに適用される料金</span><span class="sxs-lookup"><span data-stu-id="a2381-656">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="a2381-657">ライセンスベースの割引</span><span class="sxs-lookup"><span data-stu-id="a2381-657">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="a2381-658">複数の種類の料金に適用される場合がある</span><span class="sxs-lookup"><span data-stu-id="a2381-658">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="a2381-659">ライセンスベースのファイルから、<strong>TotalOtherDiscount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="a2381-659">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a2381-660"><strong>税</strong>&nbsp;または&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="a2381-660"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="a2381-661">複数の種類の料金に適用される場合がある</span><span class="sxs-lookup"><span data-stu-id="a2381-661">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="a2381-662">例外:&quot;行項目を相殺&quot;税金が既に含まれています。</span><span class="sxs-lookup"><span data-stu-id="a2381-662">Exception: &quot;Offset a line item&quot; already includes taxes.</span></span> <span data-ttu-id="a2381-663">上記の「クレジット」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2381-663">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="a2381-664">税または付加価値税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="a2381-664">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="a2381-665">ライセンスベースのファイルから、<strong>Tax</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="a2381-665">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="a2381-666">使用量ベースのファイルから、<strong>TaxAmount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="a2381-666">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
