---
title: 調整ファイルの使用 | パートナー センター
ms.topic: article
ms.date: 03/15/2019
description: 請求サイクルの各料金の詳しい行項目ビューについては、パートナー センターから調整ファイルをダウンロードします。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: fca9897720412a77ac39c86ba31db411c58c2cb0
ms.sourcegitcommit: 1f9078d422af5f8514d79a6ab9c3444500abfe27
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/24/2019
ms.locfileid: "67343467"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="1a647-103">調整ファイルを使う</span><span class="sxs-lookup"><span data-stu-id="1a647-103">Use the reconciliation files</span></span>

<span data-ttu-id="1a647-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="1a647-104">**Applies to**</span></span>

-  <span data-ttu-id="1a647-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="1a647-105">Partner Center</span></span>
-  <span data-ttu-id="1a647-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="1a647-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="1a647-107">請求サイクルの各料金の詳しい行項目ビューについては、パートナー センターから調整ファイルをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="1a647-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="1a647-108">詳細には、各顧客のサブスクリプションの料金や、詳細なイベント (期間途中でのサブスクリプションへのシートの追加など) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1a647-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="1a647-109">書式設定の問題</span><span class="sxs-lookup"><span data-stu-id="1a647-109">Formatting issues</span></span>

<span data-ttu-id="1a647-110">調整ファイルに書式設定の問題が発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="1a647-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="1a647-111">(これは、たとえば、EN-US ロケールが使用されていない場合に発生することがあります。)これらの問題を修正するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="1a647-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="1a647-112">Excel で .csv ファイルを開き、最初の列を選択します。</span><span class="sxs-lookup"><span data-stu-id="1a647-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="1a647-113">リボンで <strong>[データ]</strong> を選択し、<strong>[区切り位置]</strong> を選択します。</span><span class="sxs-lookup"><span data-stu-id="1a647-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="1a647-114">区切り位置指定ウィザードで、<strong>[Delimited file type]\(区切られたファイルの種類\)</strong> を選択し、<strong>[次へ]</strong> を選択します。</span><span class="sxs-lookup"><span data-stu-id="1a647-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="1a647-115">[区切り文字] フィールドで、<strong>[コンマ]</strong> を選択します。</span><span class="sxs-lookup"><span data-stu-id="1a647-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="1a647-116"><strong>[タブ]</strong> が既に選択されている場合は、そのままで構いません。</span><span class="sxs-lookup"><span data-stu-id="1a647-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="1a647-117"><strong>[次へ]</strong> を選びます。</span><span class="sxs-lookup"><span data-stu-id="1a647-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="1a647-118">[列のデータ形式] フィールドで、<strong>日付:MDY</strong> を選択し、<strong>[次へ]</strong> を選択します。</span><span class="sxs-lookup"><span data-stu-id="1a647-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="1a647-119">[列のデータ形式] フィールドで、すべての金額の列で <strong>[テキスト]</strong> を選択し、<strong>[完了]</strong> を選択します。</span><span class="sxs-lookup"><span data-stu-id="1a647-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="1a647-120">大規模な偵察ファイルのダウンロード</span><span class="sxs-lookup"><span data-stu-id="1a647-120">Downloading a large recon file</span></span>

<span data-ttu-id="1a647-121">偵察ファイルは、非常に大きくし、ダウンロードするが困難な場合があります。</span><span class="sxs-lookup"><span data-stu-id="1a647-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="1a647-122">大規模な偵察ファイルをダウンロードする PowerShell スクリプトでは、次を参照してください。 [Get 請求書の品目](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items)します。</span><span class="sxs-lookup"><span data-stu-id="1a647-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="1a647-123">パートナーごとに明細を示す</span><span class="sxs-lookup"><span data-stu-id="1a647-123">Itemize by partner</span></span>


<span data-ttu-id="1a647-124">インダイレクト モデルのパートナーは、ライセンス ベースの調整ファイルと使用量ベースの調整ファイルの両方で、これらの追加フィールドを使用してリセラーごとに明細を記載できます。</span><span class="sxs-lookup"><span data-stu-id="1a647-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="1a647-125">MPN ID</span><span class="sxs-lookup"><span data-stu-id="1a647-125">MPN ID</span></span></th>
<th><span data-ttu-id="1a647-126">説明</span><span class="sxs-lookup"><span data-stu-id="1a647-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="1a647-127">MPN ID</span><span class="sxs-lookup"><span data-stu-id="1a647-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="1a647-128">CSP パートナー (直接または間接) の Microsoft Partner Network (MPN) IDです。</span><span class="sxs-lookup"><span data-stu-id="1a647-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-129">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="1a647-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="1a647-130">インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="1a647-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="1a647-131">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="1a647-132">これは、パートナー センターで特定のサブスクリプションについて示されるリセラー ID に対応します。</span><span class="sxs-lookup"><span data-stu-id="1a647-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="1a647-133">リセラーを表示または更新するには、パートナー センター メニューから <strong>[顧客]</strong> を選択し、一覧から顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="1a647-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="1a647-134">顧客メニューの <strong>[サブスクリプション]</strong> を選び、一覧からサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="1a647-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="1a647-135"><strong>[更新]</strong> を選んで、<strong>[再販業者 (MPN ID)]</strong> を変更します。</span><span class="sxs-lookup"><span data-stu-id="1a647-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="1a647-136">CSP パートナーがお客様に直接サブスクリプションを販売した場合、パートナーの MPN ID が MPN ID とリセラーの MPN ID として 2 か所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="1a647-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="1a647-137">CSP パートナーのリセラーに MPN ID がない場合は、代わりに CSP パートナーの MPN ID がこの値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="1a647-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="1a647-138">CSP パートナーがリセラー ID を削除した場合、この値は -1 に設定されます。</span><span class="sxs-lookup"><span data-stu-id="1a647-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="1a647-139">ライセンス ベースのファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="1a647-139">License-based file fields</span></span>


<span data-ttu-id="1a647-140">顧客の注文に対する料金を調整するには、調整ファイルの Syndication\_Partner\_Subscription\_Number とパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="1a647-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="1a647-141"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="1a647-142"><strong>説明</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="1a647-143"><strong>サンプル値</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="1a647-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="1a647-145">特定の課金エンティティの一意の識別子 (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="1a647-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="1a647-146">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="1a647-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="1a647-147">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="1a647-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="1a647-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="1a647-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="1a647-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="1a647-150">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="1a647-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="1a647-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="1a647-152">OrderID</span></span></td>
<td><p><span data-ttu-id="1a647-153">Microsoft 請求プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1a647-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="1a647-154">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="1a647-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="1a647-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="1a647-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="1a647-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="1a647-157">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1a647-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="1a647-158">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="1a647-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="1a647-159">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="1a647-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="1a647-160">「Syndication_Partner_Subscription_Number」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1a647-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="1a647-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="1a647-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="1a647-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="1a647-163">サブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1a647-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="1a647-164">お客様は同じプランで複数のサブスクリプションを持つことができるため、これは調整ファイルの分析で重要です。</span><span class="sxs-lookup"><span data-stu-id="1a647-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="1a647-165">このフィールドは、パートナー管理コンソールのサブスクリプション ID にマップされます。</span><span class="sxs-lookup"><span data-stu-id="1a647-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="1a647-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="1a647-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="1a647-167">OfferID</span></span></td>
<td><p><span data-ttu-id="1a647-168">一意のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-168">Unique offer ID.</span></span> <span data-ttu-id="1a647-169">価格表に従った標準のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="1a647-170"><b>注意</b>:この値は、価格表のプラン ID とは一致しません。</span><span class="sxs-lookup"><span data-stu-id="1a647-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="1a647-171">以下の DurableOfferID を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a647-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="1a647-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="1a647-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="1a647-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="1a647-174">価格表で定義されている一意の継続的なプラン ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="1a647-175"><b>注意</b>:この値は価格表のプラン ID と一致します。</span><span class="sxs-lookup"><span data-stu-id="1a647-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="1a647-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="1a647-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="1a647-177">OfferName</span></span></td>
<td><p><span data-ttu-id="1a647-178">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="1a647-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="1a647-179">Microsoft Office 365 (プラン E3)</span><span class="sxs-lookup"><span data-stu-id="1a647-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="1a647-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="1a647-181">サブスクリプションの開始日。注文が送信された日に設定されます。</span><span class="sxs-lookup"><span data-stu-id="1a647-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="1a647-182">サブスクリプションの開始日を終了日と共に確認することにより、顧客がサブスクリプションの最初の 1 年以内であるか、サブスクリプションが次の 1 年間更新されたかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="1a647-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="1a647-183">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="1a647-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1a647-184">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="1a647-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="1a647-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="1a647-186">サブスクリプション終了日:開始日から 12 か月 + x 日後 (パートナーの請求日と合わせる) または更新日から 12 か月。</span><span class="sxs-lookup"><span data-stu-id="1a647-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="1a647-187">更新時に、価格は最新の価格表に更新されます。</span><span class="sxs-lookup"><span data-stu-id="1a647-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="1a647-188">自動更新の前に、顧客とのやり取りが必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="1a647-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="1a647-189">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="1a647-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1a647-190">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="1a647-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="1a647-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="1a647-192">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="1a647-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="1a647-193">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="1a647-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="1a647-194">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="1a647-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1a647-195">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="1a647-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="1a647-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="1a647-197">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="1a647-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="1a647-198">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="1a647-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="1a647-199">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="1a647-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="1a647-200">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="1a647-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="1a647-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="1a647-202">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="1a647-202">The type of charge or adjustment.</span></span> <span data-ttu-id="1a647-203">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a647-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="1a647-204">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a647-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="1a647-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="1a647-206">シート単価 (購入時に価格表に公開されていた価格)。</span><span class="sxs-lookup"><span data-stu-id="1a647-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="1a647-207">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1a647-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="1a647-208">6.82</span><span class="sxs-lookup"><span data-stu-id="1a647-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-209">Quantity</span><span class="sxs-lookup"><span data-stu-id="1a647-209">Quantity</span></span></td>
<td><p><span data-ttu-id="1a647-210">シート数。</span><span class="sxs-lookup"><span data-stu-id="1a647-210">Number of seats.</span></span> <span data-ttu-id="1a647-211">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1a647-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="1a647-212">2</span><span class="sxs-lookup"><span data-stu-id="1a647-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-213">金額</span><span class="sxs-lookup"><span data-stu-id="1a647-213">Amount</span></span></td>
<td><p><span data-ttu-id="1a647-214">数量に対する合計価格。</span><span class="sxs-lookup"><span data-stu-id="1a647-214">Total of price for quantity.</span></span> <span data-ttu-id="1a647-215">金額の計算が、この顧客用の計算方法に一致することを確認するために役立ちます。</span><span class="sxs-lookup"><span data-stu-id="1a647-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="1a647-216">13.32</span><span class="sxs-lookup"><span data-stu-id="1a647-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="1a647-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="1a647-218">これらの料金に適用される割引額。</span><span class="sxs-lookup"><span data-stu-id="1a647-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="1a647-219">インセンティブの対象となる IUR または新しいサブスクリプションの場合も、この列に割引額が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1a647-219">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="1a647-220">2.32</span><span class="sxs-lookup"><span data-stu-id="1a647-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-221">Subtotal</span><span class="sxs-lookup"><span data-stu-id="1a647-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="1a647-222">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="1a647-222">Total before tax.</span></span> <span data-ttu-id="1a647-223">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1a647-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="1a647-224">11</span><span class="sxs-lookup"><span data-stu-id="1a647-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-225">Tax</span><span class="sxs-lookup"><span data-stu-id="1a647-225">Tax</span></span></td>
<td><p><span data-ttu-id="1a647-226">市場の税制や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="1a647-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="1a647-227">0</span><span class="sxs-lookup"><span data-stu-id="1a647-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="1a647-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="1a647-229">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="1a647-229">Total after tax.</span></span> <span data-ttu-id="1a647-230">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="1a647-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="1a647-231">11</span><span class="sxs-lookup"><span data-stu-id="1a647-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-232">通貨</span><span class="sxs-lookup"><span data-stu-id="1a647-232">Currency</span></span></td>
<td><p><span data-ttu-id="1a647-233">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="1a647-233">Currency type.</span></span> <span data-ttu-id="1a647-234">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="1a647-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="1a647-235">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1a647-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="1a647-236">EUR</span><span class="sxs-lookup"><span data-stu-id="1a647-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="1a647-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="1a647-238">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="1a647-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="1a647-239">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="1a647-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="1a647-240">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="1a647-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="1a647-241">MPNID</span></span></td>
<td><p><span data-ttu-id="1a647-242">CSP パートナーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="1a647-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="1a647-243">4390934</span><span class="sxs-lookup"><span data-stu-id="1a647-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="1a647-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="1a647-245">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="1a647-246">「<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">パートナーごとに明細を示す</a>」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1a647-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="1a647-247">4390934</span><span class="sxs-lookup"><span data-stu-id="1a647-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="1a647-248">DomainName</span></span></td>
<td><p><span data-ttu-id="1a647-249">顧客を特定するために使用する顧客のドメイン名。</span><span class="sxs-lookup"><span data-stu-id="1a647-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="1a647-250">顧客/パートナーは O365 ポータルからバニティ/既定のドメインを更新できるため、顧客を一意に識別するためにこれを使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="1a647-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="1a647-251">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1a647-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="1a647-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="1a647-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="1a647-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="1a647-254">サブスクリプションのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="1a647-254">Subscription nickname.</span></span> <span data-ttu-id="1a647-255">ニックネームが指定されていない場合、パートナー センターでは OfferName を使用します。</span><span class="sxs-lookup"><span data-stu-id="1a647-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="1a647-256">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="1a647-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="1a647-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="1a647-258">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="1a647-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="1a647-259">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="1a647-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="1a647-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span><span class="sxs-lookup"><span data-stu-id="1a647-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="1a647-261">使用量ベースのファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="1a647-261">Usage-based file fields</span></span>


<span data-ttu-id="1a647-262">顧客の使用量に対する料金を調整するには、調整ファイルの ResellerID/ResellerName/ResellerBillableAccount、顧客名、およびパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="1a647-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="1a647-263">次のフィールドで、どのサービスが使用されるか、およびレートについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1a647-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="1a647-264"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="1a647-265"><strong>説明</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="1a647-266"><strong>サンプル値</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="1a647-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="1a647-268">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="1a647-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="1a647-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="1a647-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="1a647-271">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="1a647-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="1a647-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="1a647-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="1a647-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="1a647-274">パートナーのアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="1a647-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="1a647-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="1a647-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="1a647-277">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="1a647-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="1a647-278">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="1a647-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="1a647-279">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="1a647-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="1a647-280">MPNID</span></span></td>
<td><p><span data-ttu-id="1a647-281">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="1a647-282">4390934</span><span class="sxs-lookup"><span data-stu-id="1a647-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="1a647-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="1a647-284">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="1a647-285">「<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">パートナーごとに明細を示す</a>」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1a647-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="1a647-286">4390934</span><span class="sxs-lookup"><span data-stu-id="1a647-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="1a647-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="1a647-288">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="1a647-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="1a647-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="1a647-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="1a647-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="1a647-291">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="1a647-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="1a647-292">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="1a647-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="1a647-293">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="1a647-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="1a647-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="1a647-295">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="1a647-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="1a647-296">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="1a647-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="1a647-297">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="1a647-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="1a647-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="1a647-299">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1a647-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="1a647-300">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="1a647-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="1a647-301">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="1a647-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="1a647-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="1a647-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="1a647-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="1a647-304">サービス プランのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="1a647-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="1a647-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="1a647-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="1a647-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="1a647-307">サービス プランの基幹業務</span><span class="sxs-lookup"><span data-stu-id="1a647-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="1a647-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="1a647-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="1a647-309">OrderID</span></span></td>
<td><p><span data-ttu-id="1a647-310">Microsoft 請求プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1a647-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="1a647-311">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="1a647-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="1a647-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="1a647-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="1a647-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="1a647-314">対象の Azure サービスの名前。</span><span class="sxs-lookup"><span data-stu-id="1a647-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="1a647-315">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="1a647-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="1a647-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="1a647-317">Windows Azure サービスの特定の種類。</span><span class="sxs-lookup"><span data-stu-id="1a647-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="1a647-318">Service Bus – Individual or Pack</span><span class="sxs-lookup"><span data-stu-id="1a647-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="1a647-319">SQL Azure database – Business or Web Edition</span><span class="sxs-lookup"><span data-stu-id="1a647-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="1a647-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="1a647-321">すべてのサービス データおよび価格設定構造の特定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1a647-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="1a647-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="1a647-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-323">リソース名</span><span class="sxs-lookup"><span data-stu-id="1a647-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="1a647-324">Azure リソースの名前。</span><span class="sxs-lookup"><span data-stu-id="1a647-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="1a647-325">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="1a647-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="1a647-326">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="1a647-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-327">Region</span><span class="sxs-lookup"><span data-stu-id="1a647-327">Region</span></span></td>
<td><p><span data-ttu-id="1a647-328">使用量が適用される地域。</span><span class="sxs-lookup"><span data-stu-id="1a647-328">The region the usage applies to.</span></span> <span data-ttu-id="1a647-329">料金は地域によって異なるため、主にデータ転送に料金を割り当てるために使われます。</span><span class="sxs-lookup"><span data-stu-id="1a647-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="1a647-330">Asia Pacific、Europe、Latin America、North America</span><span class="sxs-lookup"><span data-stu-id="1a647-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-331">SKU</span><span class="sxs-lookup"><span data-stu-id="1a647-331">SKU</span></span></td>
<td><p><span data-ttu-id="1a647-332">プランについての MSFT の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="1a647-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="1a647-333">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="1a647-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="1a647-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="1a647-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="1a647-335">特定の課金期間のサービスまたはリソースに対してさまざまなレートの明細を設定するための ID と数量。</span><span class="sxs-lookup"><span data-stu-id="1a647-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="1a647-336">Azure の階層化されたレーティングの場合は、一定数量の課金可能単位までは 1 つのレートがあり、その後に別のレートがあることがあります。</span><span class="sxs-lookup"><span data-stu-id="1a647-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="1a647-337">1</span><span class="sxs-lookup"><span data-stu-id="1a647-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="1a647-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="1a647-339">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="1a647-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="1a647-340">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="1a647-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="1a647-341">11</span><span class="sxs-lookup"><span data-stu-id="1a647-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="1a647-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="1a647-343">単位数はプランの一部として含まれます。</span><span class="sxs-lookup"><span data-stu-id="1a647-343">Units included as part of the offer.</span></span> <span data-ttu-id="1a647-344">通常、CSP には含まれません。</span><span class="sxs-lookup"><span data-stu-id="1a647-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="1a647-345">0</span><span class="sxs-lookup"><span data-stu-id="1a647-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="1a647-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="1a647-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="1a647-347">単位数はプランの一部として含まれず、パートナーが支払う必要があります。</span><span class="sxs-lookup"><span data-stu-id="1a647-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="1a647-348">ConsumedQuantity - IncludedQuantity と同じです。</span><span class="sxs-lookup"><span data-stu-id="1a647-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="1a647-349">11</span><span class="sxs-lookup"><span data-stu-id="1a647-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="1a647-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="1a647-351">サブスクリプションの開始日に有効な価格を提供します。</span><span class="sxs-lookup"><span data-stu-id="1a647-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="1a647-352">$0.0808</span><span class="sxs-lookup"><span data-stu-id="1a647-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="1a647-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="1a647-354">ListPrist と OverageQuantity を掛けて、最も近いセントに丸めます。</span><span class="sxs-lookup"><span data-stu-id="1a647-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="1a647-355">$0.085</span><span class="sxs-lookup"><span data-stu-id="1a647-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="1a647-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="1a647-357">市場の税制や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="1a647-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="1a647-358">$0.08</span><span class="sxs-lookup"><span data-stu-id="1a647-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="1a647-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="1a647-360">税が適用されるときの税引き後の合計額。</span><span class="sxs-lookup"><span data-stu-id="1a647-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="1a647-361">$0.93</span><span class="sxs-lookup"><span data-stu-id="1a647-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-362">通貨</span><span class="sxs-lookup"><span data-stu-id="1a647-362">Currency</span></span></td>
<td><p><span data-ttu-id="1a647-363">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="1a647-363">Currency type.</span></span> <span data-ttu-id="1a647-364">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="1a647-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="1a647-365">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1a647-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="1a647-366">EUR</span><span class="sxs-lookup"><span data-stu-id="1a647-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="1a647-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="1a647-368">単位あたりの税込み価格。</span><span class="sxs-lookup"><span data-stu-id="1a647-368">Pretax price per unit.</span></span> <span data-ttu-id="1a647-369">PretaxCharges / OverageQuantity と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="1a647-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="1a647-370">$0.08</span><span class="sxs-lookup"><span data-stu-id="1a647-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="1a647-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="1a647-372">単位あたりの税引き後の価格。</span><span class="sxs-lookup"><span data-stu-id="1a647-372">Post tax price per unit.</span></span> <span data-ttu-id="1a647-373">PostTaxTotal / OverageQuantity、または PretaxEffectiveRate + 単位額あたりの税率と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="1a647-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="1a647-374">$0.08</span><span class="sxs-lookup"><span data-stu-id="1a647-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="1a647-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="1a647-376">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="1a647-376">The type of charge or adjustment.</span></span> <span data-ttu-id="1a647-377">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a647-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="1a647-378">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a647-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="1a647-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="1a647-380">MSFT 課金プラットフォームの一意のアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="1a647-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="1a647-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="1a647-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="1a647-383">サービスの展開の日付。</span><span class="sxs-lookup"><span data-stu-id="1a647-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="1a647-384">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="1a647-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="1a647-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="1a647-386">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="1a647-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="1a647-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="1a647-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="1a647-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="1a647-389">この列は、[Service Name] 列で特に識別されない可能性のある、個別の Microsoft Azure サービスの追跡に利用されます。</span><span class="sxs-lookup"><span data-stu-id="1a647-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="1a647-390">たとえば、データ転送は、[Service Name] 列で &quot;Microsoft Azure - All Services&quot; と報告されます。</span><span class="sxs-lookup"><span data-stu-id="1a647-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="1a647-391">この [MeteredService] 列は、利用に関連する特定のサービスを示します。</span><span class="sxs-lookup"><span data-stu-id="1a647-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="1a647-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="1a647-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="1a647-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="1a647-394">個々の Microsoft Azure サービスの内容を、MeteredService フィールドで提供されるレベルよりも明確にする小見出し。</span><span class="sxs-lookup"><span data-stu-id="1a647-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="1a647-395">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="1a647-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-396">Project</span><span class="sxs-lookup"><span data-stu-id="1a647-396">Project</span></span></td>
<td><p><span data-ttu-id="1a647-397">サービス インスタンスの顧客定義の名前</span><span class="sxs-lookup"><span data-stu-id="1a647-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="1a647-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="1a647-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="1a647-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="1a647-400">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="1a647-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="1a647-401">例: 1 か月 30 日間の中に、個別にプロビジョニングされた接続がある場合、Service Info 1 は "1.000000 Connections / 30 days" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="1a647-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="1a647-402">プロビジョニングされた ServiceBus 接続が 25 パックあり、その日のうちに 1 つを利用した場合、その日の 1 日の使用量の計算書には、"25 Connections / 30 Days – Used:1.000000" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="1a647-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="1a647-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="1a647-404">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="1a647-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="1a647-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="1a647-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="1a647-406">DomainName</span></span></td>
<td><p><span data-ttu-id="1a647-407">顧客を特定するために使用する顧客のドメイン名。</span><span class="sxs-lookup"><span data-stu-id="1a647-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="1a647-408">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1a647-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="1a647-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="1a647-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="1a647-410">Unit</span><span class="sxs-lookup"><span data-stu-id="1a647-410">Unit</span></span></td>
<td><p><span data-ttu-id="1a647-411">リソース名の単位</span><span class="sxs-lookup"><span data-stu-id="1a647-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="1a647-412">GB または HOURS</span><span class="sxs-lookup"><span data-stu-id="1a647-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="1a647-413">1 回限りおよび定期的なファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="1a647-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="1a647-414">列</span><span class="sxs-lookup"><span data-stu-id="1a647-414">Column</span></span></th>
<th><span data-ttu-id="1a647-415">説明</span><span class="sxs-lookup"><span data-stu-id="1a647-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="1a647-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="1a647-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="1a647-417">特定の課金エンティティに対する一意の Microsoft Azure Active Directory テナント識別子 (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="1a647-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="1a647-418">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="1a647-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="1a647-419">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="1a647-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-420">Customer Id</span><span class="sxs-lookup"><span data-stu-id="1a647-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="1a647-421">顧客を識別するために使用される、GUID 形式の一意の Microsoft Azure Active Directory テナント ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-422">顧客名</span><span class="sxs-lookup"><span data-stu-id="1a647-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="1a647-423">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="1a647-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="1a647-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="1a647-425">顧客のドメイン名。顧客を特定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="1a647-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="1a647-426">顧客/パートナーは O365 ポータルからバニティ/既定のドメインを更新できるため、顧客を一意に識別するためにこれを使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="1a647-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="1a647-427">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1a647-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-428">Customer Country</span><span class="sxs-lookup"><span data-stu-id="1a647-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="1a647-429">顧客の在住国。</span><span class="sxs-lookup"><span data-stu-id="1a647-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-430">請求書番号</span><span class="sxs-lookup"><span data-stu-id="1a647-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="1a647-431">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="1a647-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="1a647-432">MpnId</span></span></td>
<td><p><span data-ttu-id="1a647-433">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-434">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="1a647-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="1a647-435">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-436">Order ID</span><span class="sxs-lookup"><span data-stu-id="1a647-436">Order ID</span></span></td>
<td><p><span data-ttu-id="1a647-437">Microsoft コマース プラットフォームでの注文に対する一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1a647-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="1a647-438">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="1a647-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-439">発注日</span><span class="sxs-lookup"><span data-stu-id="1a647-439">Order date</span></span></td>
<td><p><span data-ttu-id="1a647-440">注文が作成された日付。</span><span class="sxs-lookup"><span data-stu-id="1a647-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="1a647-441">ProductId</span></span></td>
<td><p><span data-ttu-id="1a647-442">製品の ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="1a647-443">SkuId</span></span></td>
<td><p><span data-ttu-id="1a647-444">特定 SKU の ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="1a647-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="1a647-446">特定の可用性 の ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-446">The ID for a particular Availability.</span></span> <span data-ttu-id="1a647-447">"可用性" とは、特定の国、通貨、業界などで特定の SKU を購入可能かどうかを指します。</span><span class="sxs-lookup"><span data-stu-id="1a647-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-448">SKU Name</span><span class="sxs-lookup"><span data-stu-id="1a647-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="1a647-449">特定 SKU のタイトル。</span><span class="sxs-lookup"><span data-stu-id="1a647-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-450">製品名</span><span class="sxs-lookup"><span data-stu-id="1a647-450">Product name</span></span></td>
<td><p><span data-ttu-id="1a647-451">製品の名前。</span><span class="sxs-lookup"><span data-stu-id="1a647-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="1a647-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="1a647-453">製品の発行元の名前。</span><span class="sxs-lookup"><span data-stu-id="1a647-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="1a647-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="1a647-455">この発行元の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-456">Subscription Description</span><span class="sxs-lookup"><span data-stu-id="1a647-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="1a647-457">サブスクリプションのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="1a647-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-458">サブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="1a647-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="1a647-459">Microsoft コマース プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1a647-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="1a647-460">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="1a647-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="1a647-461">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="1a647-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="1a647-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="1a647-463">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="1a647-463">Start day of the charges.</span></span> <span data-ttu-id="1a647-464">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="1a647-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="1a647-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="1a647-466">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="1a647-466">End day of the charges.</span></span> <span data-ttu-id="1a647-467">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="1a647-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-468">Term and Billingcycle</span><span class="sxs-lookup"><span data-stu-id="1a647-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="1a647-469">購入の期間と請求サイクル。</span><span class="sxs-lookup"><span data-stu-id="1a647-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="1a647-470">例: “1 Year, Monthly” (1 年、月単位)。</span><span class="sxs-lookup"><span data-stu-id="1a647-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-471">請求の種類</span><span class="sxs-lookup"><span data-stu-id="1a647-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="1a647-472">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="1a647-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-473">単価</span><span class="sxs-lookup"><span data-stu-id="1a647-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="1a647-474">購入時に価格表に公開されていた価格。</span><span class="sxs-lookup"><span data-stu-id="1a647-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="1a647-475">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1a647-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-476">Effective Unit Price</span><span class="sxs-lookup"><span data-stu-id="1a647-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="1a647-477">調整が行われた後の単価。</span><span class="sxs-lookup"><span data-stu-id="1a647-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-478">Quantity</span><span class="sxs-lookup"><span data-stu-id="1a647-478">Quantity</span></span></td>
<td><p><span data-ttu-id="1a647-479">ユニット数。</span><span class="sxs-lookup"><span data-stu-id="1a647-479">Number of units.</span></span> <span data-ttu-id="1a647-480">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1a647-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-481">Unit type</span><span class="sxs-lookup"><span data-stu-id="1a647-481">Unit type</span></span></td>
<td><p><span data-ttu-id="1a647-482">購入したユニットの種類。</span><span class="sxs-lookup"><span data-stu-id="1a647-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="1a647-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="1a647-484">適用可能なすべての割引の説明。</span><span class="sxs-lookup"><span data-stu-id="1a647-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-485">Sub Total</span><span class="sxs-lookup"><span data-stu-id="1a647-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="1a647-486">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="1a647-486">Total before tax.</span></span> <span data-ttu-id="1a647-487">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1a647-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-488">Tax Total</span><span class="sxs-lookup"><span data-stu-id="1a647-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="1a647-489">市場の税関連の規則や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="1a647-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-490">Total</span><span class="sxs-lookup"><span data-stu-id="1a647-490">Total</span></span></td>
<td><p><span data-ttu-id="1a647-491">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="1a647-491">Total after tax.</span></span> <span data-ttu-id="1a647-492">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="1a647-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-493">通貨</span><span class="sxs-lookup"><span data-stu-id="1a647-493">Currency</span></span></td>
<td><p><span data-ttu-id="1a647-494">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="1a647-494">Currency type.</span></span> <span data-ttu-id="1a647-495">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="1a647-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="1a647-496">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1a647-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="1a647-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="1a647-498">注文 ID の代替識別子。</span><span class="sxs-lookup"><span data-stu-id="1a647-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="1a647-499">毎日評価される使用量ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="1a647-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="1a647-500">列</span><span class="sxs-lookup"><span data-stu-id="1a647-500">Column</span></span></th>
<th><span data-ttu-id="1a647-501">説明</span><span class="sxs-lookup"><span data-stu-id="1a647-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="1a647-502">PartnerId</span><span class="sxs-lookup"><span data-stu-id="1a647-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="1a647-503">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="1a647-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="1a647-505">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="1a647-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-506">CustomerId</span><span class="sxs-lookup"><span data-stu-id="1a647-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="1a647-507">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="1a647-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="1a647-509">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="1a647-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="1a647-510">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="1a647-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="1a647-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="1a647-512">顧客のドメイン名。</span><span class="sxs-lookup"><span data-stu-id="1a647-512">The customer’s domain name.</span></span> <span data-ttu-id="1a647-513">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="1a647-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-514">Customer country</span><span class="sxs-lookup"><span data-stu-id="1a647-514">Customer country</span></span></td>
<td><p><span data-ttu-id="1a647-515">顧客の在住国。</span><span class="sxs-lookup"><span data-stu-id="1a647-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-516">MPNID</span><span class="sxs-lookup"><span data-stu-id="1a647-516">MPNID</span></span></td>
<td><p><span data-ttu-id="1a647-517">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-518">Reseller MPNID</span><span class="sxs-lookup"><span data-stu-id="1a647-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="1a647-519">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="1a647-520">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="1a647-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="1a647-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="1a647-522">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="1a647-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="1a647-523">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="1a647-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-524">ProductId</span><span class="sxs-lookup"><span data-stu-id="1a647-524">ProductId</span></span></td>
<td><p><span data-ttu-id="1a647-525">製品の ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="1a647-526">SkuId</span></span></td>
<td><p><span data-ttu-id="1a647-527">特定 SKU の ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="1a647-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="1a647-529">特定の可用性 の ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-529">The ID for a particular Availability.</span></span> <span data-ttu-id="1a647-530">"可用性" とは、特定の国、通貨、業界などで特定の SKU を購入可能かどうかを指します。</span><span class="sxs-lookup"><span data-stu-id="1a647-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-531">SKU Name</span><span class="sxs-lookup"><span data-stu-id="1a647-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="1a647-532">特定 SKU のタイトル。</span><span class="sxs-lookup"><span data-stu-id="1a647-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="1a647-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="1a647-534">発行元の名前。</span><span class="sxs-lookup"><span data-stu-id="1a647-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="1a647-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="1a647-536">発行元の ID (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="1a647-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="1a647-537">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="1a647-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="1a647-538">Subscription Description</span><span class="sxs-lookup"><span data-stu-id="1a647-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="1a647-539">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="1a647-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="1a647-540">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="1a647-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-541">サブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="1a647-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="1a647-542">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="1a647-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="1a647-543">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="1a647-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="1a647-544">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="1a647-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="1a647-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="1a647-546">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="1a647-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="1a647-547">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="1a647-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="1a647-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="1a647-549">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="1a647-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="1a647-550">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="1a647-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-551">Usage Date</span><span class="sxs-lookup"><span data-stu-id="1a647-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="1a647-552">サービス使用の日付。</span><span class="sxs-lookup"><span data-stu-id="1a647-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-553">Meter Type</span><span class="sxs-lookup"><span data-stu-id="1a647-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="1a647-554">メーターの種類。</span><span class="sxs-lookup"><span data-stu-id="1a647-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-555">Meter Category</span><span class="sxs-lookup"><span data-stu-id="1a647-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="1a647-556">使用状況の最上位サービス。</span><span class="sxs-lookup"><span data-stu-id="1a647-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-557">Meter Id</span><span class="sxs-lookup"><span data-stu-id="1a647-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="1a647-558">使用されているメーターの ID。</span><span class="sxs-lookup"><span data-stu-id="1a647-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-559">Meter Sub-category</span><span class="sxs-lookup"><span data-stu-id="1a647-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="1a647-560">速度に影響を与える可能性がある Azure サービスの種類。</span><span class="sxs-lookup"><span data-stu-id="1a647-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-561">Meter Name</span><span class="sxs-lookup"><span data-stu-id="1a647-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="1a647-562">使用しているメーターの測定単位。</span><span class="sxs-lookup"><span data-stu-id="1a647-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-563">Meter Region</span><span class="sxs-lookup"><span data-stu-id="1a647-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="1a647-564">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="1a647-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-565">Unit</span><span class="sxs-lookup"><span data-stu-id="1a647-565">Unit</span></span></td>
<td><p><span data-ttu-id="1a647-566">リソース名の単位。</span><span class="sxs-lookup"><span data-stu-id="1a647-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-567">Consumed Quantity</span><span class="sxs-lookup"><span data-stu-id="1a647-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="1a647-568">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="1a647-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="1a647-569">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="1a647-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-570">Resource Location</span><span class="sxs-lookup"><span data-stu-id="1a647-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="1a647-571">メーターが実行されているデータ センター。</span><span class="sxs-lookup"><span data-stu-id="1a647-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-572">Consumed Service</span><span class="sxs-lookup"><span data-stu-id="1a647-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="1a647-573">使用した Azure プラットフォーム サービス。</span><span class="sxs-lookup"><span data-stu-id="1a647-573">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-574">リソース グループ</span><span class="sxs-lookup"><span data-stu-id="1a647-574">Resource Group</span></span></td>
<td><p><span data-ttu-id="1a647-575">デプロイされたメーターが実行されているリソース グループ。</span><span class="sxs-lookup"><span data-stu-id="1a647-575">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-576">Resource URI</span><span class="sxs-lookup"><span data-stu-id="1a647-576">Resource URI</span></span></td>
<td><p><span data-ttu-id="1a647-577">使用されているリソースの URI。</span><span class="sxs-lookup"><span data-stu-id="1a647-577">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-578">請求の種類</span><span class="sxs-lookup"><span data-stu-id="1a647-578">Charge type</span></span></td>
<td><p><span data-ttu-id="1a647-579">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="1a647-579">The type of charge or adjustment.</span></span> <span data-ttu-id="1a647-580">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="1a647-580">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-581">単価</span><span class="sxs-lookup"><span data-stu-id="1a647-581">Unit price</span></span></td>
<td><p><span data-ttu-id="1a647-582">ライセンス単価 (購入時に価格表に公開されていた価格)。</span><span class="sxs-lookup"><span data-stu-id="1a647-582">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="1a647-583">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1a647-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-584">Quantity</span><span class="sxs-lookup"><span data-stu-id="1a647-584">Quantity</span></span></td>
<td><p><span data-ttu-id="1a647-585">ライセンス数。</span><span class="sxs-lookup"><span data-stu-id="1a647-585">Number of licenses.</span></span> <span data-ttu-id="1a647-586">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="1a647-586">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-587">Unit type</span><span class="sxs-lookup"><span data-stu-id="1a647-587">Unit type</span></span></td>
<td><p><span data-ttu-id="1a647-588">メーターが課金するユニットの種類。</span><span class="sxs-lookup"><span data-stu-id="1a647-588">The type of unit the meter is charged in.</span></span> <span data-ttu-id="1a647-589">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="1a647-589">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-590">Billing pre tax</span><span class="sxs-lookup"><span data-stu-id="1a647-590">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="1a647-591">税引き前の合計金額。</span><span class="sxs-lookup"><span data-stu-id="1a647-591">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-592">Billing currency</span><span class="sxs-lookup"><span data-stu-id="1a647-592">Billing currency</span></span></td>
<td><p><span data-ttu-id="1a647-593">顧客の地理的領域での通貨</span><span class="sxs-lookup"><span data-stu-id="1a647-593">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-594">Pricing pretax total</span><span class="sxs-lookup"><span data-stu-id="1a647-594">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="1a647-595">税金が追加される前の価格。</span><span class="sxs-lookup"><span data-stu-id="1a647-595">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-596">Pricing currency</span><span class="sxs-lookup"><span data-stu-id="1a647-596">Pricing currency</span></span></td>
<td><p><span data-ttu-id="1a647-597">価格表の通貨。</span><span class="sxs-lookup"><span data-stu-id="1a647-597">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-598">Service Info 1</span><span class="sxs-lookup"><span data-stu-id="1a647-598">Service Info 1</span></span></td>
<td><p><span data-ttu-id="1a647-599">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="1a647-599">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-600">Service Info 2</span><span class="sxs-lookup"><span data-stu-id="1a647-600">Service Info 2</span></span></td>
<td><p><span data-ttu-id="1a647-601">省略可能なサービスに固有のメタデータをキャプチャするレガシ フィールド。</span><span class="sxs-lookup"><span data-stu-id="1a647-601">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="1a647-602">Tags</span><span class="sxs-lookup"><span data-stu-id="1a647-602">Tags</span></span></td>
<td><p><span data-ttu-id="1a647-603">課金レコードをグループ化するためにメーターに割り当てるタグ。</span><span class="sxs-lookup"><span data-stu-id="1a647-603">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="1a647-604">たとえば、タグを使用して、メーターを使用している部門ごとにコストを分配することができます。</span><span class="sxs-lookup"><span data-stu-id="1a647-604">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="1a647-605">Additional Info</span><span class="sxs-lookup"><span data-stu-id="1a647-605">Additional Info</span></span></td>
<td><p><span data-ttu-id="1a647-606">他の列で網羅されていないすべての追加情報。</span><span class="sxs-lookup"><span data-stu-id="1a647-606">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="1a647-607">請求書と調整ファイルの間の課金のマッピング</span><span class="sxs-lookup"><span data-stu-id="1a647-607">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="1a647-608">請求書は料金の概要を示し、調整ファイルは、課金の種類を含め、行項目のトランザクションの詳細な内訳を示します。</span><span class="sxs-lookup"><span data-stu-id="1a647-608">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="1a647-609">請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルター オプションを使用して、調整ファイルの課金の種類でフィルター処理し、請求書の課金を調整ファイルの一連の課金の内訳にマップします。</span><span class="sxs-lookup"><span data-stu-id="1a647-609">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="1a647-610">使用量ベースとライセンス ベースの調整ファイルには、使用量関連のトランザクションと料金 (消費された単位量および関連する料金) のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1a647-610">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="1a647-611">請求書に “調整” として表示される単発のクレジット、割引、払い戻し金額は、調整ファイルに表示されません。</span><span class="sxs-lookup"><span data-stu-id="1a647-611">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="1a647-612">次の表に、請求書のセクションと、調整ファイルに表示される関連付けられた課金の種類とのマッピングを示します。</span><span class="sxs-lookup"><span data-stu-id="1a647-612">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="1a647-613"><strong>請求書の課金の説明</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-613"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-614"><strong>調整ファイルの課金の説明 (ChargeType 列)</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-614"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-615"><strong>この課金の意味</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-615"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-616"><strong>これらの ChargeTypes を請求書にマップする方法</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-616"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="1a647-617"><strong>ライセンスベースの料金</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-617"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-618">アクティブ化料金</span><span class="sxs-lookup"><span data-stu-id="1a647-618">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-619">購入したサブスクリプションを顧客が使用したときに顧客に課金される金額</span><span class="sxs-lookup"><span data-stu-id="1a647-619">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="1a647-620">ライセンスベースのファイルから、<strong>Amount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1a647-620">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-621">取り消し料金</span><span class="sxs-lookup"><span data-stu-id="1a647-621">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-622">関連付けられているシートが変更されたときに顧客に払い戻される日割り料金</span><span class="sxs-lookup"><span data-stu-id="1a647-622">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-623">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="1a647-623">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-624">サブスクリプションの定期的な課金</span><span class="sxs-lookup"><span data-stu-id="1a647-624">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-625">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="1a647-625">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-626">関連付けられているシートが変更されたときに顧客から評価される日割り料金</span><span class="sxs-lookup"><span data-stu-id="1a647-626">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-627">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="1a647-627">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-628">取り消し時のサービスの未使用部分に対する日割りの払戻し額</span><span class="sxs-lookup"><span data-stu-id="1a647-628">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-629">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="1a647-629">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-630">年次請求を使用する場合のサブスクリプションの料金タイプ</span><span class="sxs-lookup"><span data-stu-id="1a647-630">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-631">Purchase fee</span><span class="sxs-lookup"><span data-stu-id="1a647-631">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-632">月次請求を使用する場合のサブスクリプションの料金タイプ</span><span class="sxs-lookup"><span data-stu-id="1a647-632">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-633">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="1a647-633">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-634">サブスクリプションの更新時の日割り料金</span><span class="sxs-lookup"><span data-stu-id="1a647-634">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="1a647-635">Renew fee</span><span class="sxs-lookup"><span data-stu-id="1a647-635">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-636">サブスクリプションの更新時の課金</span><span class="sxs-lookup"><span data-stu-id="1a647-636">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-637">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="1a647-637">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-638">アクティブ化から課金期間の終了までの日割り料金</span><span class="sxs-lookup"><span data-stu-id="1a647-638">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="1a647-639"><strong>1 回限りの料金</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-639"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="1a647-640">新規</span><span class="sxs-lookup"><span data-stu-id="1a647-640">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-641">新しい発注を作成するときに使用</span><span class="sxs-lookup"><span data-stu-id="1a647-641">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-642">addQuantity</span><span class="sxs-lookup"><span data-stu-id="1a647-642">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-643">増加した後、元の購入と新しい数量の両方、返金で使用されます。</span><span class="sxs-lookup"><span data-stu-id="1a647-643">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-644">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="1a647-644">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-645">減少後の元の購入と新しい数量の両方、返金で使用されます。</span><span class="sxs-lookup"><span data-stu-id="1a647-645">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-646">Cancel</span><span class="sxs-lookup"><span data-stu-id="1a647-646">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-647">サブスクリプションが取り消されたときに使用</span><span class="sxs-lookup"><span data-stu-id="1a647-647">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-648">Convert</span><span class="sxs-lookup"><span data-stu-id="1a647-648">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-649">ライセンスのアップグレードが接続クライアントの数は変更されません。</span><span class="sxs-lookup"><span data-stu-id="1a647-649">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="1a647-650"><strong>利用料金</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-650"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-651">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="1a647-651">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-652">現在の課金期間中に未払いの使用を取り消したときのアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="1a647-652">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="1a647-653">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1a647-653">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-654">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="1a647-654">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-655">現在の課金期間のアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="1a647-655">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="1a647-656"><strong>クレジット</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-656"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-657">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="1a647-657">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-658">税金を含む、行項目への一部または全部の払戻し</span><span class="sxs-lookup"><span data-stu-id="1a647-658">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-659">ライセンスベースのファイルから、<strong>TotalForCustomer</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1a647-659">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="1a647-660">使用量ベースのファイルから、<strong>PostTaxTotal</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1a647-660">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="1a647-661"><strong>使用量ベースの割引</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-661"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-662">Activation discount</span><span class="sxs-lookup"><span data-stu-id="1a647-662">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-663">サブスクリプションがアクティブ化されたときに適用される割引</span><span class="sxs-lookup"><span data-stu-id="1a647-663">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="1a647-664">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1a647-664">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-665">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="1a647-665">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-666">定期的な課金に適用される割引</span><span class="sxs-lookup"><span data-stu-id="1a647-666">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-667">Renew discount</span><span class="sxs-lookup"><span data-stu-id="1a647-667">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-668">サブスクリプションの更新時に適用される割引</span><span class="sxs-lookup"><span data-stu-id="1a647-668">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-669">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="1a647-669">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-670">割引が取り消されたときに適用される料金</span><span class="sxs-lookup"><span data-stu-id="1a647-670">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="1a647-671"><strong>ライセンスベースの割引</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-671"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-672"><em>複数の種類の料金に適用される場合がある</em></span><span class="sxs-lookup"><span data-stu-id="1a647-672"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="1a647-673">ライセンスベースのファイルから、<strong>TotalOtherDiscount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1a647-673">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="1a647-674"><strong>税</strong>&nbsp;または&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="1a647-674"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-675"><em>複数の種類の料金に適用される場合がある</em></span><span class="sxs-lookup"><span data-stu-id="1a647-675"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="1a647-676"><em>例外:&quot;Offset a line item&quot; には既に税が含まれています。上記の「クレジット」を参照してください。</em></span><span class="sxs-lookup"><span data-stu-id="1a647-676"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-677">税または付加価値税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="1a647-677">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="1a647-678">ライセンスベースのファイルから、<strong>Tax</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1a647-678">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="1a647-679">使用量ベースのファイルから、<strong>TaxAmount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="1a647-679">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
