---
title: 調整ファイルを使う | パートナー センター
ms.topic: article
ms.date: 11/07/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 請求サイクルの各料金の詳しい行項目ビューについては、パートナー センターから調整ファイルをダウンロードします。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 217d5e9c068a07b51f74333f605daca8ab573c9a
ms.sourcegitcommit: 8425d3435892651e3e6cb1147cd3b268b2b1869b
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/07/2019
ms.locfileid: "73753853"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="b14d3-103">調整ファイルを使う</span><span class="sxs-lookup"><span data-stu-id="b14d3-103">Use the reconciliation files</span></span>

<span data-ttu-id="b14d3-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="b14d3-104">**Applies to**</span></span>

-  <span data-ttu-id="b14d3-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="b14d3-105">Partner Center</span></span>
-  <span data-ttu-id="b14d3-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="b14d3-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="b14d3-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="b14d3-107">**Appropriate roles**</span></span>

- <span data-ttu-id="b14d3-108">課金の管理</span><span class="sxs-lookup"><span data-stu-id="b14d3-108">Billing admin</span></span>
- <span data-ttu-id="b14d3-109">グローバル管理</span><span class="sxs-lookup"><span data-stu-id="b14d3-109">Global admin</span></span>

<span data-ttu-id="b14d3-110">請求サイクルの各料金の詳しい行項目ビューについては、パートナー センターから調整ファイルをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="b14d3-110">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="b14d3-111">詳細には、各顧客のサブスクリプションの料金や、詳細なイベント (期間途中でのサブスクリプションへのシートの追加など) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-111">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="b14d3-112">書式設定の問題</span><span class="sxs-lookup"><span data-stu-id="b14d3-112">Formatting issues</span></span>

<span data-ttu-id="b14d3-113">調整ファイルに書式設定の問題が発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-113">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="b14d3-114">(たとえば、EN-US ロケールが使用されていない場合に発生する可能性があります)。これらの問題を解決するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="b14d3-114">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="b14d3-115">Excel で .csv ファイルを開き、最初の列を選択します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-115">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="b14d3-116">リボンで <strong>[データ]</strong> を選択し、<strong>[区切り位置]</strong> を選択します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-116">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="b14d3-117">区切り位置指定ウィザードで、<strong>[Delimited file type]\(区切られたファイルの種類\)</strong> を選択し、<strong>[次へ]</strong> を選択します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-117">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="b14d3-118">[区切り文字] フィールドで、<strong>[コンマ]</strong> を選択します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-118">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="b14d3-119"><strong>[タブ]</strong> が既に選択されている場合は、そのままで構いません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-119">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="b14d3-120"><strong>[次へ]</strong> を選びます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-120">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="b14d3-121">[列のデータ形式] フィールドで、[ <strong>Date: MDY</strong>] を選択し、[<strong>次へ</strong>] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-121">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="b14d3-122">[列のデータ形式] フィールドで、すべての金額の列で <strong>[テキスト]</strong> を選択し、<strong>[完了]</strong> を選択します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-122">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="b14d3-123">大きな偵察ファイルをダウンロードしています</span><span class="sxs-lookup"><span data-stu-id="b14d3-123">Downloading a large recon file</span></span>

<span data-ttu-id="b14d3-124">Recon ファイルは非常に大きくなる可能性があり、ダウンロードが困難な場合があります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-124">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="b14d3-125">大きな偵察ファイルをダウンロードするための PowerShell スクリプトについては、「[請求書の品目を取得](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b14d3-125">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="b14d3-126">パートナーごとに明細を示す</span><span class="sxs-lookup"><span data-stu-id="b14d3-126">Itemize by partner</span></span>


<span data-ttu-id="b14d3-127">インダイレクト モデルのパートナーは、ライセンス ベースの調整ファイルと使用量ベースの調整ファイルの両方で、これらの追加フィールドを使用してリセラーごとに明細を記載できます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-127">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b14d3-128">MPN ID</span><span class="sxs-lookup"><span data-stu-id="b14d3-128">MPN ID</span></span></th>
<th><span data-ttu-id="b14d3-129">説明</span><span class="sxs-lookup"><span data-stu-id="b14d3-129">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="b14d3-130">MPN ID</span><span class="sxs-lookup"><span data-stu-id="b14d3-130">MPN ID</span></span></td>
<td><p><span data-ttu-id="b14d3-131">CSP パートナー (直接または間接) の Microsoft Partner Network (MPN) IDです。</span><span class="sxs-lookup"><span data-stu-id="b14d3-131">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-132">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="b14d3-132">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="b14d3-133">インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-133">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="b14d3-134">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-134">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b14d3-135">これは、パートナー センターで特定のサブスクリプションについて示されるリセラー ID に対応します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-135">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="b14d3-136">リセラーを表示または更新するには、パートナー センター メニューから <strong>[顧客]</strong> を選択し、一覧から顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-136">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="b14d3-137">顧客メニューの <strong>[サブスクリプション]</strong> を選び、一覧からサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-137">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="b14d3-138"><strong>[更新]</strong> を選んで、<strong>[再販業者 (MPN ID)]</strong> を変更します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-138">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="b14d3-139">CSP パートナーがお客様に直接サブスクリプションを販売した場合、パートナーの MPN ID が MPN ID とリセラーの MPN ID として 2 か所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-139">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="b14d3-140">CSP パートナーが MPN ID のない再販業者を持っている場合、この値は代わりにパートナーの MPN ID に設定されます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-140">If a CSP partner has a reseller with no MPN ID, this value is set to the partner's MPN ID instead.</span></span></p>
<p><span data-ttu-id="b14d3-141">CSP パートナーがリセラー ID を削除した場合、この値は -1 に設定されます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-141">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="b14d3-142">ライセンス ベースのファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="b14d3-142">License-based file fields</span></span>


<span data-ttu-id="b14d3-143">顧客の注文に対する料金を調整するには、調整ファイルの Syndication\_Partner\_Subscription\_Number とパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-143">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="b14d3-144"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-144"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="b14d3-145"><strong>説明</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-145"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="b14d3-146"><strong>サンプル値</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-146"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-147">PartnerId</span><span class="sxs-lookup"><span data-stu-id="b14d3-147">PartnerId</span></span></td>
<td><p><span data-ttu-id="b14d3-148">特定の課金エンティティの一意の識別子 (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="b14d3-148">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="b14d3-149">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-149">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="b14d3-150">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="b14d3-150">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="b14d3-151">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="b14d3-151">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-152">CustomerID</span><span class="sxs-lookup"><span data-stu-id="b14d3-152">CustomerID</span></span></td>
<td><p><span data-ttu-id="b14d3-153">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-153">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="b14d3-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="b14d3-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-155">OrderID</span><span class="sxs-lookup"><span data-stu-id="b14d3-155">OrderID</span></span></td>
<td><p><span data-ttu-id="b14d3-156">Microsoft 課金プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b14d3-156">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="b14d3-157">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-157">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="b14d3-158">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="b14d3-158">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-159">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="b14d3-159">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="b14d3-160">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b14d3-160">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b14d3-161">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-161">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="b14d3-162">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-162">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="b14d3-163">「Syndication_Partner_Subscription_Number」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b14d3-163">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="b14d3-164">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="b14d3-164">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-165">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="b14d3-165">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="b14d3-166">サブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b14d3-166">Unique identifier for subscriptions.</span></span> <span data-ttu-id="b14d3-167">お客様は同じプランで複数のサブスクリプションを持つことができるため、これは調整ファイルの分析で重要です。</span><span class="sxs-lookup"><span data-stu-id="b14d3-167">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="b14d3-168">このフィールドは、パートナー管理コンソールのサブスクリプション ID にマップされます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-168">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="b14d3-169">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="b14d3-169">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-170">OfferID</span><span class="sxs-lookup"><span data-stu-id="b14d3-170">OfferID</span></span></td>
<td><p><span data-ttu-id="b14d3-171">一意のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-171">Unique offer ID.</span></span> <span data-ttu-id="b14d3-172">価格表に従った標準のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-172">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="b14d3-173"><b>注</b>: この値は、価格表のプラン ID とは一致しません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-173"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="b14d3-174">以下の DurableOfferID を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b14d3-174">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="b14d3-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="b14d3-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-176">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="b14d3-176">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="b14d3-177">価格表で定義されている一意の継続的なプラン ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-177">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="b14d3-178"><b>注</b>: この値は価格表のプラン ID と一致します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-178"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="b14d3-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="b14d3-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-180">OfferName</span><span class="sxs-lookup"><span data-stu-id="b14d3-180">OfferName</span></span></td>
<td><p><span data-ttu-id="b14d3-181">価格表で定義されている、顧客が購入したサービス プランの名前</span><span class="sxs-lookup"><span data-stu-id="b14d3-181">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="b14d3-182">Microsoft Office 365 (プラン E3)</span><span class="sxs-lookup"><span data-stu-id="b14d3-182">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-183">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="b14d3-183">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="b14d3-184">サブスクリプションの開始日。注文が送信された日に設定されます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-184">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="b14d3-185">サブスクリプションの開始日を終了日と共に確認することにより、顧客がサブスクリプションの最初の 1 年以内であるか、サブスクリプションが次の 1 年間更新されたかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-185">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="b14d3-186">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b14d3-187">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b14d3-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-188">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="b14d3-188">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="b14d3-189">サブスクリプション終了日: 開始日から 12 か月 + x 日後 (パートナーの請求日と合わせる) または更新日から 12 か月</span><span class="sxs-lookup"><span data-stu-id="b14d3-189">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="b14d3-190">更新時に、価格は最新の価格表に更新されます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-190">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="b14d3-191">自動更新の前に、顧客とのやり取りが必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-191">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="b14d3-192">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-192">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b14d3-193">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b14d3-193">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-194">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b14d3-194">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b14d3-195">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="b14d3-195">Start day of the charges.</span></span></p>
<p><span data-ttu-id="b14d3-196">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-196">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="b14d3-197">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-197">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b14d3-198">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b14d3-198">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-199">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b14d3-199">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b14d3-200">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="b14d3-200">End day of the charges.</span></span></p>
<p><span data-ttu-id="b14d3-201">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-201">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="b14d3-202">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-202">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="b14d3-203">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="b14d3-203">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-204">ChargeType</span><span class="sxs-lookup"><span data-stu-id="b14d3-204">ChargeType</span></span></td>
<td><p><span data-ttu-id="b14d3-205">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="b14d3-205">The type of charge or adjustment.</span></span> <span data-ttu-id="b14d3-206">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b14d3-206">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="b14d3-207">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b14d3-207">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-208">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="b14d3-208">UnitPrice</span></span></td>
<td><p><span data-ttu-id="b14d3-209">シート単価 (購入時に価格表に公開されていた価格)。</span><span class="sxs-lookup"><span data-stu-id="b14d3-209">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b14d3-210">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-210">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="b14d3-211">6.82</span><span class="sxs-lookup"><span data-stu-id="b14d3-211">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-212">Quantity</span><span class="sxs-lookup"><span data-stu-id="b14d3-212">Quantity</span></span></td>
<td><p><span data-ttu-id="b14d3-213">シート数。</span><span class="sxs-lookup"><span data-stu-id="b14d3-213">Number of seats.</span></span> <span data-ttu-id="b14d3-214">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-214">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="b14d3-215">2</span><span class="sxs-lookup"><span data-stu-id="b14d3-215">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-216">Amount</span><span class="sxs-lookup"><span data-stu-id="b14d3-216">Amount</span></span></td>
<td><p><span data-ttu-id="b14d3-217">数量に対する合計価格。</span><span class="sxs-lookup"><span data-stu-id="b14d3-217">Total of price for quantity.</span></span> <span data-ttu-id="b14d3-218">金額の計算が、この顧客用の計算方法に一致することを確認するために役立ちます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-218">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="b14d3-219">13.32</span><span class="sxs-lookup"><span data-stu-id="b14d3-219">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-220">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="b14d3-220">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="b14d3-221">これらの料金に適用される割引額。</span><span class="sxs-lookup"><span data-stu-id="b14d3-221">Amount of discount applied to these charges.</span></span> <span data-ttu-id="b14d3-222">コンピテンシーまたはマップに含まれる製品ライセンス、またはインセンティブの対象となる新しいサブスクリプションには、このコラムの割引額も含まれます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-222">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="b14d3-223">2.32</span><span class="sxs-lookup"><span data-stu-id="b14d3-223">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-224">Subtotal</span><span class="sxs-lookup"><span data-stu-id="b14d3-224">Subtotal</span></span></td>
<td><p><span data-ttu-id="b14d3-225">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="b14d3-225">Total before tax.</span></span> <span data-ttu-id="b14d3-226">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-226">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="b14d3-227">11</span><span class="sxs-lookup"><span data-stu-id="b14d3-227">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-228">Tax</span><span class="sxs-lookup"><span data-stu-id="b14d3-228">Tax</span></span></td>
<td><p><span data-ttu-id="b14d3-229">市場の税制や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="b14d3-229">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="b14d3-230">0</span><span class="sxs-lookup"><span data-stu-id="b14d3-230">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-231">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="b14d3-231">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="b14d3-232">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="b14d3-232">Total after tax.</span></span> <span data-ttu-id="b14d3-233">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-233">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="b14d3-234">11</span><span class="sxs-lookup"><span data-stu-id="b14d3-234">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-235">Currency</span><span class="sxs-lookup"><span data-stu-id="b14d3-235">Currency</span></span></td>
<td><p><span data-ttu-id="b14d3-236">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="b14d3-236">Currency type.</span></span> <span data-ttu-id="b14d3-237">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="b14d3-237">Each billing entity has only one currency.</span></span> <span data-ttu-id="b14d3-238">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-238">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="b14d3-239">EUR</span><span class="sxs-lookup"><span data-stu-id="b14d3-239">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-240">CustomerName</span><span class="sxs-lookup"><span data-stu-id="b14d3-240">CustomerName</span></span></td>
<td><p><span data-ttu-id="b14d3-241">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="b14d3-241">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="b14d3-242">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="b14d3-242">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="b14d3-243">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="b14d3-243">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-244">MPNID</span><span class="sxs-lookup"><span data-stu-id="b14d3-244">MPNID</span></span></td>
<td><p><span data-ttu-id="b14d3-245">CSP パートナーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="b14d3-245">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="b14d3-246">4390934</span><span class="sxs-lookup"><span data-stu-id="b14d3-246">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-247">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="b14d3-247">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="b14d3-248">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-248">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b14d3-249">「<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">パートナーごとに明細を示す</a>」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b14d3-249">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="b14d3-250">4390934</span><span class="sxs-lookup"><span data-stu-id="b14d3-250">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-251">DomainName</span><span class="sxs-lookup"><span data-stu-id="b14d3-251">DomainName</span></span></td>
<td><p><span data-ttu-id="b14d3-252">顧客を特定するために使用する顧客のドメイン名。</span><span class="sxs-lookup"><span data-stu-id="b14d3-252">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="b14d3-253">顧客/パートナーは O365 ポータルからバニティ/既定のドメインを更新できるため、顧客を一意に識別するためにこれを使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="b14d3-253">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="b14d3-254">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-254">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="b14d3-255">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b14d3-255">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-256">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="b14d3-256">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="b14d3-257">サブスクリプションのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="b14d3-257">Subscription nickname.</span></span> <span data-ttu-id="b14d3-258">ニックネームが指定されていない場合、パートナー センターでは OfferName を使用します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-258">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="b14d3-259">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="b14d3-259">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-260">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="b14d3-260">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="b14d3-261">価格表で定義されている、顧客が購入したサービス プランの名前</span><span class="sxs-lookup"><span data-stu-id="b14d3-261">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="b14d3-262">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="b14d3-262">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="b14d3-263">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span><span class="sxs-lookup"><span data-stu-id="b14d3-263">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="b14d3-264">使用量ベースのファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="b14d3-264">Usage-based file fields</span></span>


<span data-ttu-id="b14d3-265">顧客の使用量に対する料金を調整するには、調整ファイルの ResellerID/ResellerName/ResellerBillableAccount、顧客名、およびパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-265">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="b14d3-266">次のフィールドで、どのサービスが使用されるか、およびレートについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-266">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="b14d3-267"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-267"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="b14d3-268"><strong>説明</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-268"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="b14d3-269"><strong>サンプル値</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-269"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-270">PartnerID</span><span class="sxs-lookup"><span data-stu-id="b14d3-270">PartnerID</span></span></td>
<td><p><span data-ttu-id="b14d3-271">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-271">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="b14d3-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="b14d3-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-273">PartnerName</span><span class="sxs-lookup"><span data-stu-id="b14d3-273">PartnerName</span></span></td>
<td><p><span data-ttu-id="b14d3-274">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="b14d3-274">Partner Name.</span></span></p></td>
<td><span data-ttu-id="b14d3-275">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="b14d3-275">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-276">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="b14d3-276">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="b14d3-277">パートナーのアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-277">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="b14d3-278">1010578050</span><span class="sxs-lookup"><span data-stu-id="b14d3-278">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-279">CustomerName</span><span class="sxs-lookup"><span data-stu-id="b14d3-279">CustomerName</span></span></td>
<td><p><span data-ttu-id="b14d3-280">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="b14d3-280">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="b14d3-281">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="b14d3-281">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="b14d3-282">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="b14d3-282">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-283">MPNID</span><span class="sxs-lookup"><span data-stu-id="b14d3-283">MPNID</span></span></td>
<td><p><span data-ttu-id="b14d3-284">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-284">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="b14d3-285">4390934</span><span class="sxs-lookup"><span data-stu-id="b14d3-285">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-286">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="b14d3-286">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="b14d3-287">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-287">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b14d3-288">「<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">パートナーごとに明細を示す</a>」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b14d3-288">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="b14d3-289">4390934</span><span class="sxs-lookup"><span data-stu-id="b14d3-289">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-290">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="b14d3-290">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="b14d3-291">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="b14d3-291">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="b14d3-292">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="b14d3-292">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-293">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b14d3-293">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b14d3-294">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="b14d3-294">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="b14d3-295">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-295">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b14d3-296">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="b14d3-296">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-297">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b14d3-297">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b14d3-298">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="b14d3-298">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="b14d3-299">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-299">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="b14d3-300">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="b14d3-300">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-301">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="b14d3-301">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="b14d3-302">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b14d3-302">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b14d3-303">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-303">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="b14d3-304">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-304">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="b14d3-305">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="b14d3-305">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-306">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="b14d3-306">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="b14d3-307">サービス プランのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="b14d3-307">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="b14d3-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b14d3-308">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-309">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="b14d3-309">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="b14d3-310">サービス プランの基幹業務</span><span class="sxs-lookup"><span data-stu-id="b14d3-310">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="b14d3-311">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b14d3-311">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-312">OrderID</span><span class="sxs-lookup"><span data-stu-id="b14d3-312">OrderID</span></span></td>
<td><p><span data-ttu-id="b14d3-313">Microsoft 課金プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b14d3-313">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="b14d3-314">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-314">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="b14d3-315">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="b14d3-315">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-316">ServiceName</span><span class="sxs-lookup"><span data-stu-id="b14d3-316">ServiceName</span></span></td>
<td><p><span data-ttu-id="b14d3-317">対象の Azure サービスの名前。</span><span class="sxs-lookup"><span data-stu-id="b14d3-317">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="b14d3-318">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="b14d3-318">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-319">ServiceType</span><span class="sxs-lookup"><span data-stu-id="b14d3-319">ServiceType</span></span></td>
<td><p><span data-ttu-id="b14d3-320">Windows Azure サービスの特定の種類。</span><span class="sxs-lookup"><span data-stu-id="b14d3-320">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="b14d3-321">Service Bus-個人またはパック</span><span class="sxs-lookup"><span data-stu-id="b14d3-321">Service Bus - Individual or Pack</span></span></li>
<li><span data-ttu-id="b14d3-322">SQL Azure database-Business Edition または Web Edition</span><span class="sxs-lookup"><span data-stu-id="b14d3-322">SQL Azure database - Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-323">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="b14d3-323">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="b14d3-324">すべてのサービス データおよび価格設定構造の特定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b14d3-324">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="b14d3-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="b14d3-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-326">リソース名</span><span class="sxs-lookup"><span data-stu-id="b14d3-326">Resource Name</span></span></td>
<td><p><span data-ttu-id="b14d3-327">Azure リソースの名前。</span><span class="sxs-lookup"><span data-stu-id="b14d3-327">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="b14d3-328">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="b14d3-328">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="b14d3-329">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="b14d3-329">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-330">Region</span><span class="sxs-lookup"><span data-stu-id="b14d3-330">Region</span></span></td>
<td><p><span data-ttu-id="b14d3-331">使用量が適用される地域。</span><span class="sxs-lookup"><span data-stu-id="b14d3-331">The region the usage applies to.</span></span> <span data-ttu-id="b14d3-332">料金は地域によって異なるため、主にデータ転送に料金を割り当てるために使われます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-332">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="b14d3-333">Asia Pacific、Europe、Latin America、North America</span><span class="sxs-lookup"><span data-stu-id="b14d3-333">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-334">SKU</span><span class="sxs-lookup"><span data-stu-id="b14d3-334">SKU</span></span></td>
<td><p><span data-ttu-id="b14d3-335">プランについての MSFT の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="b14d3-335">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="b14d3-336">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="b14d3-336">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="b14d3-337">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="b14d3-337">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="b14d3-338">特定の課金期間のサービスまたはリソースに対してさまざまなレートの明細を設定するための ID と数量。</span><span class="sxs-lookup"><span data-stu-id="b14d3-338">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="b14d3-339">Azure の階層化されたレーティングの場合は、一定数量の課金可能単位までは 1 つのレートがあり、その後に別のレートがあることがあります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-339">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="b14d3-340">1</span><span class="sxs-lookup"><span data-stu-id="b14d3-340">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-341">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="b14d3-341">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="b14d3-342">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="b14d3-342">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="b14d3-343">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-343">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="b14d3-344">11</span><span class="sxs-lookup"><span data-stu-id="b14d3-344">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-345">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="b14d3-345">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="b14d3-346">単位数はプランの一部として含まれます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-346">Units included as part of the offer.</span></span> <span data-ttu-id="b14d3-347">通常、CSP には含まれません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-347">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="b14d3-348">0</span><span class="sxs-lookup"><span data-stu-id="b14d3-348">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="b14d3-349">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="b14d3-349">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="b14d3-350">単位数はプランの一部として含まれず、パートナーが支払う必要があります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-350">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="b14d3-351">ConsumedQuantity - IncludedQuantity と同じです。</span><span class="sxs-lookup"><span data-stu-id="b14d3-351">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="b14d3-352">11</span><span class="sxs-lookup"><span data-stu-id="b14d3-352">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-353">ListPrice</span><span class="sxs-lookup"><span data-stu-id="b14d3-353">ListPrice</span></span></td>
<td><p><span data-ttu-id="b14d3-354">サブスクリプションの開始日に有効な価格を提供します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-354">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="b14d3-355">$0.0808</span><span class="sxs-lookup"><span data-stu-id="b14d3-355">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-356">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="b14d3-356">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="b14d3-357">ListPrist と OverageQuantity を掛けて、最も近いセントに丸めます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-357">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b14d3-358">$0.085</span><span class="sxs-lookup"><span data-stu-id="b14d3-358">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-359">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="b14d3-359">TaxAmount</span></span></td>
<td><p><span data-ttu-id="b14d3-360">市場の税制や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="b14d3-360">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="b14d3-361">$0.08</span><span class="sxs-lookup"><span data-stu-id="b14d3-361">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-362">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="b14d3-362">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="b14d3-363">税が適用されるときの税引き後の合計額。</span><span class="sxs-lookup"><span data-stu-id="b14d3-363">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="b14d3-364">$0.93</span><span class="sxs-lookup"><span data-stu-id="b14d3-364">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-365">Currency</span><span class="sxs-lookup"><span data-stu-id="b14d3-365">Currency</span></span></td>
<td><p><span data-ttu-id="b14d3-366">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="b14d3-366">Currency type.</span></span> <span data-ttu-id="b14d3-367">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="b14d3-367">Each billing entity has only one currency.</span></span> <span data-ttu-id="b14d3-368">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-368">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="b14d3-369">EUR</span><span class="sxs-lookup"><span data-stu-id="b14d3-369">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-370">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="b14d3-370">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="b14d3-371">単位あたりの税込み価格。</span><span class="sxs-lookup"><span data-stu-id="b14d3-371">Pretax price per unit.</span></span> <span data-ttu-id="b14d3-372">PretaxCharges / OverageQuantity と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-372">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b14d3-373">$0.08</span><span class="sxs-lookup"><span data-stu-id="b14d3-373">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-374">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="b14d3-374">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="b14d3-375">単位あたりの税引き後の価格。</span><span class="sxs-lookup"><span data-stu-id="b14d3-375">Post tax price per unit.</span></span> <span data-ttu-id="b14d3-376">PostTaxTotal / OverageQuantity、または PretaxEffectiveRate + 単位額あたりの税率と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-376">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b14d3-377">$0.08</span><span class="sxs-lookup"><span data-stu-id="b14d3-377">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-378">ChargeType</span><span class="sxs-lookup"><span data-stu-id="b14d3-378">ChargeType</span></span></td>
<td><p><span data-ttu-id="b14d3-379">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="b14d3-379">The type of charge or adjustment.</span></span> <span data-ttu-id="b14d3-380">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b14d3-380">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="b14d3-381">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b14d3-381">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-382">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="b14d3-382">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="b14d3-383">MSFT 課金プラットフォームの一意のアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-383">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="b14d3-384">1280018095</span><span class="sxs-lookup"><span data-stu-id="b14d3-384">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-385">UsageDate</span><span class="sxs-lookup"><span data-stu-id="b14d3-385">UsageDate</span></span></td>
<td><p><span data-ttu-id="b14d3-386">サービスの展開の日付。</span><span class="sxs-lookup"><span data-stu-id="b14d3-386">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="b14d3-387">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="b14d3-387">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-388">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="b14d3-388">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="b14d3-389">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-389">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="b14d3-390">East Asia、South East Asia、North Europe、West Europe、North Central US、South Central US</span><span class="sxs-lookup"><span data-stu-id="b14d3-390">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-391">MeteredService</span><span class="sxs-lookup"><span data-stu-id="b14d3-391">MeteredService</span></span></td>
<td><p><span data-ttu-id="b14d3-392">この列は、[Service Name] 列で特に識別されない可能性のある、個別の Microsoft Azure サービスの追跡に利用されます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-392">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="b14d3-393">たとえば、データ転送は、[Service Name] 列で &quot;Microsoft Azure - All Services&quot; と報告されます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-393">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="b14d3-394">この [MeteredService] 列は、利用に関連する特定のサービスを示します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-394">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="b14d3-395">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="b14d3-395">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-396">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="b14d3-396">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="b14d3-397">個々の Microsoft Azure サービスの内容を、MeteredService フィールドで提供されるレベルよりも明確にする小見出し。</span><span class="sxs-lookup"><span data-stu-id="b14d3-397">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="b14d3-398">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="b14d3-398">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-399">プロジェクト</span><span class="sxs-lookup"><span data-stu-id="b14d3-399">Project</span></span></td>
<td><p><span data-ttu-id="b14d3-400">サービス インスタンスの顧客定義の名前</span><span class="sxs-lookup"><span data-stu-id="b14d3-400">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="b14d3-401">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="b14d3-401">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-402">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="b14d3-402">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="b14d3-403">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="b14d3-403">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="b14d3-404">たとえば、30日の間に個別にプロビジョニングされた接続がある場合、サービス情報1は "1.000000 Connections/30 days" を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-404">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days".</span></span> <span data-ttu-id="b14d3-405">25個の提供会社の接続がプロビジョニングされていて、その日に1を使用したことがある場合、その日の毎日の使用状況は、"25 接続/30 日分の使用量: 1.000000" を示します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-405">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days - Used: 1.000000".</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-406">CustomerID</span><span class="sxs-lookup"><span data-stu-id="b14d3-406">CustomerID</span></span></td>
<td><p><span data-ttu-id="b14d3-407">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-407">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="b14d3-408">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="b14d3-408">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-409">DomainName</span><span class="sxs-lookup"><span data-stu-id="b14d3-409">DomainName</span></span></td>
<td><p><span data-ttu-id="b14d3-410">顧客を特定するために使用する顧客のドメイン名。</span><span class="sxs-lookup"><span data-stu-id="b14d3-410">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="b14d3-411">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-411">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="b14d3-412">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b14d3-412">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-413">Unit</span><span class="sxs-lookup"><span data-stu-id="b14d3-413">Unit</span></span></td>
<td><p><span data-ttu-id="b14d3-414">リソース名の単位</span><span class="sxs-lookup"><span data-stu-id="b14d3-414">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="b14d3-415">GB または HOURS</span><span class="sxs-lookup"><span data-stu-id="b14d3-415">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="b14d3-416">1 回限りおよび定期的なファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="b14d3-416">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b14d3-417">Column</span><span class="sxs-lookup"><span data-stu-id="b14d3-417">Column</span></span></th>
<th><span data-ttu-id="b14d3-418">説明</span><span class="sxs-lookup"><span data-stu-id="b14d3-418">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="b14d3-419">PartnerId</span><span class="sxs-lookup"><span data-stu-id="b14d3-419">PartnerId</span></span></td>
<td><p><span data-ttu-id="b14d3-420">特定の課金エンティティに対する一意の Microsoft Azure Active Directory テナント識別子 (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="b14d3-420">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="b14d3-421">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-421">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="b14d3-422">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="b14d3-422">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-423">Customer Id</span><span class="sxs-lookup"><span data-stu-id="b14d3-423">Customer Id</span></span></td>
<td><p><span data-ttu-id="b14d3-424">顧客を識別するために使用される、GUID 形式の一意の Microsoft Azure Active Directory テナント ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-424">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-425">顧客名</span><span class="sxs-lookup"><span data-stu-id="b14d3-425">Customer Name</span></span></td>
<td><p><span data-ttu-id="b14d3-426">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="b14d3-426">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-427">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="b14d3-427">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="b14d3-428">顧客のドメイン名。顧客を特定できるようにするために使用されます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-428">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="b14d3-429">顧客/パートナーは O365 ポータルからバニティ/既定のドメインを更新できるため、顧客を一意に識別するためにこれを使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="b14d3-429">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="b14d3-430">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-430">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-431">Customer Country</span><span class="sxs-lookup"><span data-stu-id="b14d3-431">Customer Country</span></span></td>
<td><p><span data-ttu-id="b14d3-432">顧客の在住国。</span><span class="sxs-lookup"><span data-stu-id="b14d3-432">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-433">請求書番号</span><span class="sxs-lookup"><span data-stu-id="b14d3-433">Invoice number</span></span></td>
<td><p><span data-ttu-id="b14d3-434">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="b14d3-434">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-435">MpnId</span><span class="sxs-lookup"><span data-stu-id="b14d3-435">MpnId</span></span></td>
<td><p><span data-ttu-id="b14d3-436">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-436">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-437">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="b14d3-437">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="b14d3-438">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-438">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-439">注文 ID</span><span class="sxs-lookup"><span data-stu-id="b14d3-439">Order ID</span></span></td>
<td><p><span data-ttu-id="b14d3-440">Microsoft コマース プラットフォームでの注文に対する一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b14d3-440">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="b14d3-441">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-441">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-442">発注日</span><span class="sxs-lookup"><span data-stu-id="b14d3-442">Order date</span></span></td>
<td><p><span data-ttu-id="b14d3-443">注文が作成された日付。</span><span class="sxs-lookup"><span data-stu-id="b14d3-443">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-444">ProductId</span><span class="sxs-lookup"><span data-stu-id="b14d3-444">ProductId</span></span></td>
<td><p><span data-ttu-id="b14d3-445">製品の ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-445">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-446">SkuId</span><span class="sxs-lookup"><span data-stu-id="b14d3-446">SkuId</span></span></td>
<td><p><span data-ttu-id="b14d3-447">特定 SKU の ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-447">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-448">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="b14d3-448">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="b14d3-449">特定の可用性 の ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-449">The ID for a particular Availability.</span></span> <span data-ttu-id="b14d3-450">"可用性" とは、特定の SKU が特定の国、通貨、業界セグメントなどで購入できるかどうかを意味します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-450">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-451">SKU Name</span><span class="sxs-lookup"><span data-stu-id="b14d3-451">SKU Name</span></span></td>
<td><p><span data-ttu-id="b14d3-452">特定 SKU のタイトル。</span><span class="sxs-lookup"><span data-stu-id="b14d3-452">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-453">製品名</span><span class="sxs-lookup"><span data-stu-id="b14d3-453">Product name</span></span></td>
<td><p><span data-ttu-id="b14d3-454">製品の名前。</span><span class="sxs-lookup"><span data-stu-id="b14d3-454">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-455">PublisherName</span><span class="sxs-lookup"><span data-stu-id="b14d3-455">PublisherName</span></span></td>
<td><p><span data-ttu-id="b14d3-456">製品の発行元の名前。</span><span class="sxs-lookup"><span data-stu-id="b14d3-456">The name of the product's publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-457">PublisherID</span><span class="sxs-lookup"><span data-stu-id="b14d3-457">PublisherID</span></span></td>
<td><p><span data-ttu-id="b14d3-458">この発行元の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-458">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-459">Subscription Description</span><span class="sxs-lookup"><span data-stu-id="b14d3-459">Subscription Description</span></span></td>
<td><p><span data-ttu-id="b14d3-460">サブスクリプションのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="b14d3-460">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-461">サブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="b14d3-461">Subscription ID</span></span></td>
<td><p><span data-ttu-id="b14d3-462">Microsoft コマース プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b14d3-462">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="b14d3-463">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-463">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="b14d3-464">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-464">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-465">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b14d3-465">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b14d3-466">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="b14d3-466">Start day of the charges.</span></span> <span data-ttu-id="b14d3-467">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-467">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-468">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b14d3-468">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b14d3-469">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="b14d3-469">End day of the charges.</span></span> <span data-ttu-id="b14d3-470">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-470">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-471">Term and Billingcycle</span><span class="sxs-lookup"><span data-stu-id="b14d3-471">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="b14d3-472">購入の期間と請求サイクル。</span><span class="sxs-lookup"><span data-stu-id="b14d3-472">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="b14d3-473">たとえば、"1 年間、毎月" のようになります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-473">For example, “1 Year, Monthly."</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-474">請求の種類</span><span class="sxs-lookup"><span data-stu-id="b14d3-474">Charge Type</span></span></td>
<td><p><span data-ttu-id="b14d3-475">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="b14d3-475">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-476">単価</span><span class="sxs-lookup"><span data-stu-id="b14d3-476">Unit Price</span></span></td>
<td><p><span data-ttu-id="b14d3-477">購入時に価格表に公開されていた価格。</span><span class="sxs-lookup"><span data-stu-id="b14d3-477">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b14d3-478">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-478">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-479">Effective Unit Price</span><span class="sxs-lookup"><span data-stu-id="b14d3-479">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="b14d3-480">調整が行われた後の単価。</span><span class="sxs-lookup"><span data-stu-id="b14d3-480">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-481">Quantity</span><span class="sxs-lookup"><span data-stu-id="b14d3-481">Quantity</span></span></td>
<td><p><span data-ttu-id="b14d3-482">ユニット数。</span><span class="sxs-lookup"><span data-stu-id="b14d3-482">Number of units.</span></span> <span data-ttu-id="b14d3-483">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-483">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-484">Unit type</span><span class="sxs-lookup"><span data-stu-id="b14d3-484">Unit type</span></span></td>
<td><p><span data-ttu-id="b14d3-485">購入したユニットの種類。</span><span class="sxs-lookup"><span data-stu-id="b14d3-485">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-486">PriceAdjustmentDescription</span><span class="sxs-lookup"><span data-stu-id="b14d3-486">PriceAdjustmentDescription</span></span></td>
<td><p><span data-ttu-id="b14d3-487">適用可能なすべての割引の説明。</span><span class="sxs-lookup"><span data-stu-id="b14d3-487">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-488">Sub Total</span><span class="sxs-lookup"><span data-stu-id="b14d3-488">Sub Total</span></span></td>
<td><p><span data-ttu-id="b14d3-489">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="b14d3-489">Total before tax.</span></span> <span data-ttu-id="b14d3-490">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-490">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-491">Tax Total</span><span class="sxs-lookup"><span data-stu-id="b14d3-491">Tax Total</span></span></td>
<td><p><span data-ttu-id="b14d3-492">市場の税関連の規則や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="b14d3-492">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-493">Total</span><span class="sxs-lookup"><span data-stu-id="b14d3-493">Total</span></span></td>
<td><p><span data-ttu-id="b14d3-494">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="b14d3-494">Total after tax.</span></span> <span data-ttu-id="b14d3-495">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-495">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-496">Currency</span><span class="sxs-lookup"><span data-stu-id="b14d3-496">Currency</span></span></td>
<td><p><span data-ttu-id="b14d3-497">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="b14d3-497">Currency type.</span></span> <span data-ttu-id="b14d3-498">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="b14d3-498">Each billing entity has only one currency.</span></span> <span data-ttu-id="b14d3-499">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-499">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-500">AlternateID</span><span class="sxs-lookup"><span data-stu-id="b14d3-500">AlternateID</span></span></td>
<td><p><span data-ttu-id="b14d3-501">注文 ID の代替識別子。</span><span class="sxs-lookup"><span data-stu-id="b14d3-501">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-502">Ic 周波数</span><span class="sxs-lookup"><span data-stu-id="b14d3-502">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="b14d3-503">毎月の課金が有効になると、毎月表示されます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-503">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="b14d3-504">それ以外の場合は空白です。</span><span class="sxs-lookup"><span data-stu-id="b14d3-504">Otherwise blank.</span></span> </p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-505">各販売数量</span><span class="sxs-lookup"><span data-stu-id="b14d3-505">BillableQuantity</span></span></td>
<td><p> <span data-ttu-id="b14d3-506">購入または消費されたユニットの合計を表します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-506">Represents the total units purchased or consumed.</span></span> </p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-507">PricingCurrency</span><span class="sxs-lookup"><span data-stu-id="b14d3-507">PricingCurrency</span></span></td>
<td><p> <span data-ttu-id="b14d3-508">リソースまたはプランの価格を一覧表示します</span><span class="sxs-lookup"><span data-stu-id="b14d3-508">Lists the price for resource or offer</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-509">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="b14d3-509">PCToBCExchangeRate</span></span> </td>
<td><p> <span data-ttu-id="b14d3-510">(顧客) 請求通貨に適用される換算レート</span><span class="sxs-lookup"><span data-stu-id="b14d3-510">Exchange rate applied for pricing currency to (customers) billing currency</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-511">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="b14d3-511">PCToBCExchangeRateDate</span></span> </td>
<td><p> <span data-ttu-id="b14d3-512">料金通貨換算率を決定する日付。</span><span class="sxs-lookup"><span data-stu-id="b14d3-512">Date at which pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-513">MeterDescription</span><span class="sxs-lookup"><span data-stu-id="b14d3-513">MeterDescription</span></span> </td>
<td><p> <span data-ttu-id="b14d3-514">従量課金ライン項目のメーターの説明</span><span class="sxs-lookup"><span data-stu-id="b14d3-514">Meter description for consumption line item</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="b14d3-515">毎日評価される使用量ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="b14d3-515">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b14d3-516">Column</span><span class="sxs-lookup"><span data-stu-id="b14d3-516">Column</span></span></th>
<th><span data-ttu-id="b14d3-517">説明</span><span class="sxs-lookup"><span data-stu-id="b14d3-517">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="b14d3-518">PartnerId</span><span class="sxs-lookup"><span data-stu-id="b14d3-518">PartnerId</span></span></td>
<td><p><span data-ttu-id="b14d3-519">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-519">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-520">PartnerName</span><span class="sxs-lookup"><span data-stu-id="b14d3-520">PartnerName</span></span></td>
<td><p><span data-ttu-id="b14d3-521">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="b14d3-521">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-522">CustomerId</span><span class="sxs-lookup"><span data-stu-id="b14d3-522">CustomerId</span></span></td>
<td><p><span data-ttu-id="b14d3-523">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-523">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-524">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="b14d3-524">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="b14d3-525">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="b14d3-525">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="b14d3-526">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="b14d3-526">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-527">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="b14d3-527">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="b14d3-528">顧客のドメイン名。</span><span class="sxs-lookup"><span data-stu-id="b14d3-528">The customer's domain name.</span></span> <span data-ttu-id="b14d3-529">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-529">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-530">Customer country</span><span class="sxs-lookup"><span data-stu-id="b14d3-530">Customer country</span></span></td>
<td><p><span data-ttu-id="b14d3-531">顧客の在住国。</span><span class="sxs-lookup"><span data-stu-id="b14d3-531">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-532">MPNID</span><span class="sxs-lookup"><span data-stu-id="b14d3-532">MPNID</span></span></td>
<td><p><span data-ttu-id="b14d3-533">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-533">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-534">Reseller MPNID</span><span class="sxs-lookup"><span data-stu-id="b14d3-534">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="b14d3-535">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-535">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b14d3-536">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-536">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-537">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="b14d3-537">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="b14d3-538">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="b14d3-538">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="b14d3-539">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-539">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-540">ProductId</span><span class="sxs-lookup"><span data-stu-id="b14d3-540">ProductId</span></span></td>
<td><p><span data-ttu-id="b14d3-541">製品の ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-541">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-542">SkuId</span><span class="sxs-lookup"><span data-stu-id="b14d3-542">SkuId</span></span></td>
<td><p><span data-ttu-id="b14d3-543">特定 SKU の ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-543">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-544">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="b14d3-544">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="b14d3-545">特定の可用性 の ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-545">The ID for a particular Availability.</span></span> <span data-ttu-id="b14d3-546">"可用性" とは、特定の SKU が特定の国、通貨、業界セグメントなどで購入できるかどうかを意味します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-546">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-547">SKU Name</span><span class="sxs-lookup"><span data-stu-id="b14d3-547">SKU Name</span></span></td>
<td><p><span data-ttu-id="b14d3-548">特定 SKU のタイトル。</span><span class="sxs-lookup"><span data-stu-id="b14d3-548">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-549">PublisherName</span><span class="sxs-lookup"><span data-stu-id="b14d3-549">PublisherName</span></span></td>
<td><p><span data-ttu-id="b14d3-550">発行元の名前。</span><span class="sxs-lookup"><span data-stu-id="b14d3-550">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-551">PublisherID</span><span class="sxs-lookup"><span data-stu-id="b14d3-551">PublisherID</span></span></td>
<td><p><span data-ttu-id="b14d3-552">発行元の ID (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="b14d3-552">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="b14d3-553">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-553">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-554">Subscription Description</span><span class="sxs-lookup"><span data-stu-id="b14d3-554">Subscription Description</span></span></td>
<td><p><span data-ttu-id="b14d3-555">価格表で定義されている、顧客が購入したサービス プランの名前</span><span class="sxs-lookup"><span data-stu-id="b14d3-555">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="b14d3-556">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="b14d3-556">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-557">サブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="b14d3-557">Subscription ID</span></span></td>
<td><p><span data-ttu-id="b14d3-558">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b14d3-558">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b14d3-559">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-559">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="b14d3-560">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-560">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-561">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b14d3-561">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b14d3-562">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="b14d3-562">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="b14d3-563">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-563">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-564">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b14d3-564">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b14d3-565">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="b14d3-565">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="b14d3-566">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="b14d3-566">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-567">Usage Date</span><span class="sxs-lookup"><span data-stu-id="b14d3-567">Usage Date</span></span></td>
<td><p><span data-ttu-id="b14d3-568">サービス使用の日付。</span><span class="sxs-lookup"><span data-stu-id="b14d3-568">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-569">Meter Type</span><span class="sxs-lookup"><span data-stu-id="b14d3-569">Meter Type</span></span></td>
<td><p><span data-ttu-id="b14d3-570">メーターの種類。</span><span class="sxs-lookup"><span data-stu-id="b14d3-570">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-571">Meter Category</span><span class="sxs-lookup"><span data-stu-id="b14d3-571">Meter Category</span></span></td>
<td><p><span data-ttu-id="b14d3-572">使用状況の最上位サービス。</span><span class="sxs-lookup"><span data-stu-id="b14d3-572">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-573">Meter Id</span><span class="sxs-lookup"><span data-stu-id="b14d3-573">Meter Id</span></span></td>
<td><p><span data-ttu-id="b14d3-574">使用されているメーターの ID。</span><span class="sxs-lookup"><span data-stu-id="b14d3-574">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-575">Meter Sub-category</span><span class="sxs-lookup"><span data-stu-id="b14d3-575">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="b14d3-576">速度に影響を与える可能性がある Azure サービスの種類。</span><span class="sxs-lookup"><span data-stu-id="b14d3-576">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-577">Meter Name</span><span class="sxs-lookup"><span data-stu-id="b14d3-577">Meter Name</span></span></td>
<td><p><span data-ttu-id="b14d3-578">使用しているメーターの測定単位。</span><span class="sxs-lookup"><span data-stu-id="b14d3-578">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-579">Meter Region</span><span class="sxs-lookup"><span data-stu-id="b14d3-579">Meter Region</span></span></td>
<td><p><span data-ttu-id="b14d3-580">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-580">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-581">Unit</span><span class="sxs-lookup"><span data-stu-id="b14d3-581">Unit</span></span></td>
<td><p><span data-ttu-id="b14d3-582">リソース名の単位。</span><span class="sxs-lookup"><span data-stu-id="b14d3-582">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-583">Consumed Quantity</span><span class="sxs-lookup"><span data-stu-id="b14d3-583">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="b14d3-584">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="b14d3-584">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="b14d3-585">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-585">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-586">Resource Location</span><span class="sxs-lookup"><span data-stu-id="b14d3-586">Resource Location</span></span></td>
<td><p><span data-ttu-id="b14d3-587">メーターが実行されているデータ センター。</span><span class="sxs-lookup"><span data-stu-id="b14d3-587">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-588">Consumed Service</span><span class="sxs-lookup"><span data-stu-id="b14d3-588">Consumed Service</span></span></td>
<td><p><span data-ttu-id="b14d3-589">使用した Azure プラットフォーム サービス。</span><span class="sxs-lookup"><span data-stu-id="b14d3-589">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="b14d3-590">Resource URI</span><span class="sxs-lookup"><span data-stu-id="b14d3-590">Resource URI</span></span></td>
<td><p><span data-ttu-id="b14d3-591">使用されているリソースの URI。</span><span class="sxs-lookup"><span data-stu-id="b14d3-591">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-592">請求の種類</span><span class="sxs-lookup"><span data-stu-id="b14d3-592">Charge type</span></span></td>
<td><p><span data-ttu-id="b14d3-593">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="b14d3-593">The type of charge or adjustment.</span></span> <span data-ttu-id="b14d3-594">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-594">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-595">単価</span><span class="sxs-lookup"><span data-stu-id="b14d3-595">Unit price</span></span></td>
<td><p><span data-ttu-id="b14d3-596">ライセンス単価 (購入時に価格表に公開されていた価格)。</span><span class="sxs-lookup"><span data-stu-id="b14d3-596">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b14d3-597">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-597">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-598">Quantity</span><span class="sxs-lookup"><span data-stu-id="b14d3-598">Quantity</span></span></td>
<td><p><span data-ttu-id="b14d3-599">ライセンス数。</span><span class="sxs-lookup"><span data-stu-id="b14d3-599">Number of licenses.</span></span> <span data-ttu-id="b14d3-600">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-600">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-601">Unit type</span><span class="sxs-lookup"><span data-stu-id="b14d3-601">Unit type</span></span></td>
<td><p><span data-ttu-id="b14d3-602">メーターが課金するユニットの種類。</span><span class="sxs-lookup"><span data-stu-id="b14d3-602">The type of unit the meter is charged in.</span></span> <span data-ttu-id="b14d3-603">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-603">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-604">Billing pre tax</span><span class="sxs-lookup"><span data-stu-id="b14d3-604">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="b14d3-605">税引き前の合計金額。</span><span class="sxs-lookup"><span data-stu-id="b14d3-605">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-606">Billing currency</span><span class="sxs-lookup"><span data-stu-id="b14d3-606">Billing currency</span></span></td>
<td><p><span data-ttu-id="b14d3-607">顧客の地域における通貨</span><span class="sxs-lookup"><span data-stu-id="b14d3-607">The currency in the customer's geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-608">Pricing pretax total</span><span class="sxs-lookup"><span data-stu-id="b14d3-608">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="b14d3-609">税金が追加される前の価格。</span><span class="sxs-lookup"><span data-stu-id="b14d3-609">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-610">Pricing currency</span><span class="sxs-lookup"><span data-stu-id="b14d3-610">Pricing currency</span></span></td>
<td><p><span data-ttu-id="b14d3-611">価格表の通貨。</span><span class="sxs-lookup"><span data-stu-id="b14d3-611">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-612">Service Info 1</span><span class="sxs-lookup"><span data-stu-id="b14d3-612">Service Info 1</span></span></td>
<td><p><span data-ttu-id="b14d3-613">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="b14d3-613">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b14d3-614">Service Info 2</span><span class="sxs-lookup"><span data-stu-id="b14d3-614">Service Info 2</span></span></td>
<td><p><span data-ttu-id="b14d3-615">省略可能なサービスに固有のメタデータをキャプチャするレガシ フィールド。</span><span class="sxs-lookup"><span data-stu-id="b14d3-615">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b14d3-616">Additional Info</span><span class="sxs-lookup"><span data-stu-id="b14d3-616">Additional Info</span></span></td>
<td><p><span data-ttu-id="b14d3-617">他の列で網羅されていないすべての追加情報。</span><span class="sxs-lookup"><span data-stu-id="b14d3-617">Any additional information not covered in other columns.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-618">EffectiveUnitPrice</span><span class="sxs-lookup"><span data-stu-id="b14d3-618">EffectiveUnitPrice</span></span></td>
<td><p> <span data-ttu-id="b14d3-619">ユニットごとに課金される実際の値 (これには割引、獲得クレジットなどが含まれます)。</span><span class="sxs-lookup"><span data-stu-id="b14d3-619">Actual value charged per unit (this includes discounts, earned credit etc).</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-620">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="b14d3-620">PCToBCExchangeRate</span></span> </td>
<td><p><span data-ttu-id="b14d3-621">(顧客) 請求通貨に適用される換算レート。</span><span class="sxs-lookup"><span data-stu-id="b14d3-621">Exchange rate applied for pricing currency to (customers) billing currency.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-622">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="b14d3-622">PCToBCExchangeRateDate</span></span> </td>
<td><p><span data-ttu-id="b14d3-623">料金の通貨換算率を決定する日付。</span><span class="sxs-lookup"><span data-stu-id="b14d3-623">Date at which the pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b14d3-624">EntitlementID</span><span class="sxs-lookup"><span data-stu-id="b14d3-624">EntitlementID</span></span></td>
<td><p><span data-ttu-id="b14d3-625">Azure subscriptionID を表します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-625">Represents Azure subscriptionID.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b14d3-626">EntitlementDescription</span><span class="sxs-lookup"><span data-stu-id="b14d3-626">EntitlementDescription</span></span></td>
<td><p><span data-ttu-id="b14d3-627">Azure サブスクリプションの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-627">Represents name of Azure subscription.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="b14d3-628">請求書と調整ファイルの間の課金のマッピング</span><span class="sxs-lookup"><span data-stu-id="b14d3-628">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="b14d3-629">請求書は料金の概要を示し、調整ファイルは、課金の種類を含め、行項目のトランザクションの詳細な内訳を示します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-629">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="b14d3-630">請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルター オプションを使用して、調整ファイルの課金の種類でフィルター処理し、請求書の課金を調整ファイルの一連の課金の内訳にマップします。</span><span class="sxs-lookup"><span data-stu-id="b14d3-630">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="b14d3-631">使用量ベースとライセンス ベースの調整ファイルには、使用量関連のトランザクションと料金 (消費された単位量および関連する料金) のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-631">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="b14d3-632">請求書に "調整" として表示される1回のクレジット、割引、返金は、調整ファイルには表示されません。</span><span class="sxs-lookup"><span data-stu-id="b14d3-632">One off credits, discounts or refunds which appear on the invoice as “Adjustments" are not shown in the reconciliation file.</span></span>

<span data-ttu-id="b14d3-633">次の表に、請求書のセクションと、調整ファイルに表示される関連付けられた課金の種類とのマッピングを示します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-633">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="b14d3-634"><strong>請求書の課金の説明</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-634"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-635"><strong>調整ファイルの課金の説明 (ChargeType 列)</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-635"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-636"><strong>この課金の意味</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-636"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-637"><strong>これらの ChargeTypes を請求書にマップする方法</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-637"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="b14d3-638"><strong>ライセンスベースの料金</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-638"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-639">アクティブ化料金</span><span class="sxs-lookup"><span data-stu-id="b14d3-639">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-640">購入したサブスクリプションを顧客が使用したときに顧客に課金される金額</span><span class="sxs-lookup"><span data-stu-id="b14d3-640">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="b14d3-641">ライセンス ベースのファイルから、<strong>Amount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b14d3-641">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-642">取り消し料金</span><span class="sxs-lookup"><span data-stu-id="b14d3-642">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-643">関連付けられているシートが変更されたときに顧客に払い戻される日割り料金</span><span class="sxs-lookup"><span data-stu-id="b14d3-643">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-644">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="b14d3-644">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-645">サブスクリプションの定期的な課金</span><span class="sxs-lookup"><span data-stu-id="b14d3-645">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-646">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="b14d3-646">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-647">関連付けられているシートが変更されたときに顧客から評価される日割り料金</span><span class="sxs-lookup"><span data-stu-id="b14d3-647">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-648">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="b14d3-648">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-649">取り消し時のサービスの未使用部分に対する日割りの払戻し額</span><span class="sxs-lookup"><span data-stu-id="b14d3-649">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-650">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="b14d3-650">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-651">年次請求を使用する場合のサブスクリプションの料金タイプ</span><span class="sxs-lookup"><span data-stu-id="b14d3-651">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-652">Purchase fee</span><span class="sxs-lookup"><span data-stu-id="b14d3-652">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-653">月次請求を使用する場合のサブスクリプションの料金タイプ</span><span class="sxs-lookup"><span data-stu-id="b14d3-653">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-654">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="b14d3-654">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-655">サブスクリプションの更新時の日割り料金</span><span class="sxs-lookup"><span data-stu-id="b14d3-655">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="b14d3-656">Renew fee</span><span class="sxs-lookup"><span data-stu-id="b14d3-656">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-657">サブスクリプションの更新時の課金</span><span class="sxs-lookup"><span data-stu-id="b14d3-657">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-658">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="b14d3-658">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-659">アクティブ化から課金期間の終了までの日割り料金</span><span class="sxs-lookup"><span data-stu-id="b14d3-659">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="b14d3-660"><strong>1回限りの料金</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-660"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="b14d3-661">新規</span><span class="sxs-lookup"><span data-stu-id="b14d3-661">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-662">新しい購入が作成されたときに使用されます</span><span class="sxs-lookup"><span data-stu-id="b14d3-662">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-663">addQuantity</span><span class="sxs-lookup"><span data-stu-id="b14d3-663">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-664">元の購入の返金と増加後の新しい数量の両方で使用されます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-664">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-665">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="b14d3-665">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-666">元の購入の返金と、減少後の新しい数量の両方で使用されます。</span><span class="sxs-lookup"><span data-stu-id="b14d3-666">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-667">[キャンセル]</span><span class="sxs-lookup"><span data-stu-id="b14d3-667">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-668">サブスクリプションが取り消されたときに使用されます</span><span class="sxs-lookup"><span data-stu-id="b14d3-668">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-669">Convert</span><span class="sxs-lookup"><span data-stu-id="b14d3-669">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-670">ライセンスがアップグレードされても、シート数が変更されていない場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="b14d3-670">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="b14d3-671"><strong>利用料金</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-671"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-672">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="b14d3-672">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-673">現在の課金期間中に未払いの使用を取り消したときのアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="b14d3-673">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="b14d3-674">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b14d3-674">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-675">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="b14d3-675">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-676">現在の課金期間のアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="b14d3-676">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="b14d3-677"><strong>クレジット</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-677"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-678">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="b14d3-678">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-679">税金を含む、行項目への一部または全部の払戻し</span><span class="sxs-lookup"><span data-stu-id="b14d3-679">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-680">ライセンス ベースのファイルから、<strong>TotalForCustomer</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b14d3-680">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="b14d3-681">使用量ベースのファイルから、<strong>PostTaxTotal</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b14d3-681">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="b14d3-682"><strong>使用量ベースの割引</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-682"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-683">Activation discount</span><span class="sxs-lookup"><span data-stu-id="b14d3-683">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-684">サブスクリプションがアクティブ化されたときに適用される割引</span><span class="sxs-lookup"><span data-stu-id="b14d3-684">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="b14d3-685">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b14d3-685">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-686">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="b14d3-686">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-687">定期的な課金に適用される割引</span><span class="sxs-lookup"><span data-stu-id="b14d3-687">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-688">Renew discount</span><span class="sxs-lookup"><span data-stu-id="b14d3-688">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-689">サブスクリプションの更新時に適用される割引</span><span class="sxs-lookup"><span data-stu-id="b14d3-689">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-690">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="b14d3-690">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-691">割引が取り消されたときに適用される料金</span><span class="sxs-lookup"><span data-stu-id="b14d3-691">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="b14d3-692"><strong>ライセンスベースの割引</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-692"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-693"><em>複数の種類の料金に適用される場合がある</em></span><span class="sxs-lookup"><span data-stu-id="b14d3-693"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="b14d3-694">ライセンス ベースのファイルから、<strong>TotalOtherDiscount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b14d3-694">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b14d3-695"><strong>税</strong>&nbsp;または&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="b14d3-695"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-696"><em>複数の種類の料金に適用される場合がある</em></span><span class="sxs-lookup"><span data-stu-id="b14d3-696"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="b14d3-697"><em>例外 &quot;Offset: 行項目 &quot; には、既に税が含まれています。上記のクレジットを参照してください。</em></span><span class="sxs-lookup"><span data-stu-id="b14d3-697"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-698">税または付加価値税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="b14d3-698">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="b14d3-699">ライセンス ベースのファイルから、<strong>Tax</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b14d3-699">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="b14d3-700">使用量ベースのファイルから、<strong>TaxAmount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="b14d3-700">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
