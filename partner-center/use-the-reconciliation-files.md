---
title: 調整ファイルの使用 | パートナー センター
ms.topic: article
ms.date: 07/08/2019
description: 請求サイクルの各料金の詳しい行項目ビューについては、パートナー センターから調整ファイルをダウンロードします。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 83be47cd9963d7e5f14b6c670cd57a8ab1d54011
ms.sourcegitcommit: 66afdaa662cfad217e29ba1f9e3a9ffd4349112f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/09/2019
ms.locfileid: "67694923"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="20e0a-103">調整ファイルを使う</span><span class="sxs-lookup"><span data-stu-id="20e0a-103">Use the reconciliation files</span></span>

<span data-ttu-id="20e0a-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="20e0a-104">**Applies to**</span></span>

-  <span data-ttu-id="20e0a-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="20e0a-105">Partner Center</span></span>
-  <span data-ttu-id="20e0a-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="20e0a-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="20e0a-107">請求サイクルの各料金の詳しい行項目ビューについては、パートナー センターから調整ファイルをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="20e0a-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="20e0a-108">詳細には、各顧客のサブスクリプションの料金や、詳細なイベント (期間途中でのサブスクリプションへのシートの追加など) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="20e0a-109">書式設定の問題</span><span class="sxs-lookup"><span data-stu-id="20e0a-109">Formatting issues</span></span>

<span data-ttu-id="20e0a-110">調整ファイルに書式設定の問題が発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="20e0a-111">(これは、たとえば、EN-US ロケールが使用されていない場合に発生することがあります。)これらの問題を修正するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="20e0a-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="20e0a-112">Excel で .csv ファイルを開き、最初の列を選択します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="20e0a-113">リボンで <strong>[データ]</strong> を選択し、<strong>[区切り位置]</strong> を選択します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="20e0a-114">区切り位置指定ウィザードで、<strong>[Delimited file type]\(区切られたファイルの種類\)</strong> を選択し、<strong>[次へ]</strong> を選択します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="20e0a-115">[区切り文字] フィールドで、<strong>[コンマ]</strong> を選択します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="20e0a-116"><strong>[タブ]</strong> が既に選択されている場合は、そのままで構いません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="20e0a-117"><strong>[次へ]</strong> を選びます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="20e0a-118">[列のデータ形式] フィールドで、<strong>日付:MDY</strong> を選択し、<strong>[次へ]</strong> を選択します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="20e0a-119">[列のデータ形式] フィールドで、すべての金額の列で <strong>[テキスト]</strong> を選択し、<strong>[完了]</strong> を選択します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="20e0a-120">大規模な偵察ファイルのダウンロード</span><span class="sxs-lookup"><span data-stu-id="20e0a-120">Downloading a large recon file</span></span>

<span data-ttu-id="20e0a-121">偵察ファイルは、非常に大きくし、ダウンロードするが困難な場合があります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="20e0a-122">大規模な偵察ファイルをダウンロードする PowerShell スクリプトでは、次を参照してください。 [Get 請求書の品目](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items)します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="20e0a-123">パートナーごとに明細を示す</span><span class="sxs-lookup"><span data-stu-id="20e0a-123">Itemize by partner</span></span>


<span data-ttu-id="20e0a-124">インダイレクト モデルのパートナーは、ライセンス ベースの調整ファイルと使用量ベースの調整ファイルの両方で、これらの追加フィールドを使用してリセラーごとに明細を記載できます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="20e0a-125">MPN ID</span><span class="sxs-lookup"><span data-stu-id="20e0a-125">MPN ID</span></span></th>
<th><span data-ttu-id="20e0a-126">説明</span><span class="sxs-lookup"><span data-stu-id="20e0a-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="20e0a-127">MPN ID</span><span class="sxs-lookup"><span data-stu-id="20e0a-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="20e0a-128">CSP パートナー (直接または間接) の Microsoft Partner Network (MPN) IDです。</span><span class="sxs-lookup"><span data-stu-id="20e0a-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-129">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="20e0a-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="20e0a-130">インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="20e0a-131">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="20e0a-132">これは、パートナー センターで特定のサブスクリプションについて示されるリセラー ID に対応します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="20e0a-133">リセラーを表示または更新するには、パートナー センター メニューから <strong>[顧客]</strong> を選択し、一覧から顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="20e0a-134">顧客メニューの <strong>[サブスクリプション]</strong> を選び、一覧からサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="20e0a-135"><strong>[更新]</strong> を選んで、<strong>[再販業者 (MPN ID)]</strong> を変更します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="20e0a-136">CSP パートナーがお客様に直接サブスクリプションを販売した場合、パートナーの MPN ID が MPN ID とリセラーの MPN ID として 2 か所に表示されます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="20e0a-137">CSP パートナーのリセラーに MPN ID がない場合は、代わりに CSP パートナーの MPN ID がこの値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="20e0a-138">CSP パートナーがリセラー ID を削除した場合、この値は -1 に設定されます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="20e0a-139">ライセンス ベースのファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="20e0a-139">License-based file fields</span></span>


<span data-ttu-id="20e0a-140">顧客の注文に対する料金を調整するには、調整ファイルの Syndication\_Partner\_Subscription\_Number とパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="20e0a-141"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="20e0a-142"><strong>説明</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="20e0a-143"><strong>サンプル値</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="20e0a-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="20e0a-145">特定の課金エンティティの一意の識別子 (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="20e0a-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="20e0a-146">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="20e0a-147">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="20e0a-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="20e0a-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="20e0a-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="20e0a-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="20e0a-150">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="20e0a-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="20e0a-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="20e0a-152">OrderID</span></span></td>
<td><p><span data-ttu-id="20e0a-153">Microsoft 請求プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20e0a-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="20e0a-154">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="20e0a-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="20e0a-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="20e0a-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="20e0a-157">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20e0a-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="20e0a-158">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="20e0a-159">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="20e0a-160">「Syndication_Partner_Subscription_Number」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="20e0a-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="20e0a-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="20e0a-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="20e0a-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="20e0a-163">サブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20e0a-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="20e0a-164">お客様は同じプランで複数のサブスクリプションを持つことができるため、これは調整ファイルの分析で重要です。</span><span class="sxs-lookup"><span data-stu-id="20e0a-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="20e0a-165">このフィールドは、パートナー管理コンソールのサブスクリプション ID にマップされます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="20e0a-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="20e0a-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="20e0a-167">OfferID</span></span></td>
<td><p><span data-ttu-id="20e0a-168">一意のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-168">Unique offer ID.</span></span> <span data-ttu-id="20e0a-169">価格表に従った標準のプラン ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="20e0a-170"><b>注意</b>:この値は、価格表のプラン ID とは一致しません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="20e0a-171">以下の DurableOfferID を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20e0a-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="20e0a-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="20e0a-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="20e0a-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="20e0a-174">価格表で定義されている一意の継続的なプラン ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="20e0a-175"><b>注意</b>:この値は価格表のプラン ID と一致します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="20e0a-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="20e0a-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="20e0a-177">OfferName</span></span></td>
<td><p><span data-ttu-id="20e0a-178">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="20e0a-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="20e0a-179">Microsoft Office 365 (プラン E3)</span><span class="sxs-lookup"><span data-stu-id="20e0a-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="20e0a-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="20e0a-181">サブスクリプションの開始日。注文が送信された日に設定されます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="20e0a-182">サブスクリプションの開始日を終了日と共に確認することにより、顧客がサブスクリプションの最初の 1 年以内であるか、サブスクリプションが次の 1 年間更新されたかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="20e0a-183">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20e0a-184">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="20e0a-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="20e0a-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="20e0a-186">サブスクリプション終了日:開始日から 12 か月 + x 日後 (パートナーの請求日と合わせる) または更新日から 12 か月。</span><span class="sxs-lookup"><span data-stu-id="20e0a-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="20e0a-187">更新時に、価格は最新の価格表に更新されます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="20e0a-188">自動更新の前に、顧客とのやり取りが必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="20e0a-189">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20e0a-190">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="20e0a-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="20e0a-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="20e0a-192">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="20e0a-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="20e0a-193">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="20e0a-194">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20e0a-195">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="20e0a-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="20e0a-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="20e0a-197">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="20e0a-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="20e0a-198">顧客がシート数を変更するときに、この数値を使用して 1 日あたり (日割り) の料金を計算します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="20e0a-199">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="20e0a-200">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="20e0a-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="20e0a-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="20e0a-202">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="20e0a-202">The type of charge or adjustment.</span></span> <span data-ttu-id="20e0a-203">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20e0a-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="20e0a-204">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20e0a-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="20e0a-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="20e0a-206">シート単価 (購入時に価格表に公開されていた価格)。</span><span class="sxs-lookup"><span data-stu-id="20e0a-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="20e0a-207">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="20e0a-208">6.82</span><span class="sxs-lookup"><span data-stu-id="20e0a-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-209">Quantity</span><span class="sxs-lookup"><span data-stu-id="20e0a-209">Quantity</span></span></td>
<td><p><span data-ttu-id="20e0a-210">シート数。</span><span class="sxs-lookup"><span data-stu-id="20e0a-210">Number of seats.</span></span> <span data-ttu-id="20e0a-211">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="20e0a-212">2</span><span class="sxs-lookup"><span data-stu-id="20e0a-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-213">金額</span><span class="sxs-lookup"><span data-stu-id="20e0a-213">Amount</span></span></td>
<td><p><span data-ttu-id="20e0a-214">数量に対する合計価格。</span><span class="sxs-lookup"><span data-stu-id="20e0a-214">Total of price for quantity.</span></span> <span data-ttu-id="20e0a-215">金額の計算が、この顧客用の計算方法に一致することを確認するために役立ちます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="20e0a-216">13.32</span><span class="sxs-lookup"><span data-stu-id="20e0a-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="20e0a-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="20e0a-218">これらの料金に適用される割引額。</span><span class="sxs-lookup"><span data-stu-id="20e0a-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="20e0a-219">インセンティブの対象となる IUR または新しいサブスクリプションの場合も、この列に割引額が含まれます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-219">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="20e0a-220">2.32</span><span class="sxs-lookup"><span data-stu-id="20e0a-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-221">Subtotal</span><span class="sxs-lookup"><span data-stu-id="20e0a-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="20e0a-222">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="20e0a-222">Total before tax.</span></span> <span data-ttu-id="20e0a-223">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="20e0a-224">11</span><span class="sxs-lookup"><span data-stu-id="20e0a-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-225">Tax</span><span class="sxs-lookup"><span data-stu-id="20e0a-225">Tax</span></span></td>
<td><p><span data-ttu-id="20e0a-226">市場の税制や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="20e0a-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="20e0a-227">0</span><span class="sxs-lookup"><span data-stu-id="20e0a-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="20e0a-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="20e0a-229">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="20e0a-229">Total after tax.</span></span> <span data-ttu-id="20e0a-230">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="20e0a-231">11</span><span class="sxs-lookup"><span data-stu-id="20e0a-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-232">通貨</span><span class="sxs-lookup"><span data-stu-id="20e0a-232">Currency</span></span></td>
<td><p><span data-ttu-id="20e0a-233">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="20e0a-233">Currency type.</span></span> <span data-ttu-id="20e0a-234">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="20e0a-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="20e0a-235">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="20e0a-236">EUR</span><span class="sxs-lookup"><span data-stu-id="20e0a-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="20e0a-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="20e0a-238">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="20e0a-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="20e0a-239">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="20e0a-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="20e0a-240">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="20e0a-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="20e0a-241">MPNID</span></span></td>
<td><p><span data-ttu-id="20e0a-242">CSP パートナーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="20e0a-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="20e0a-243">4390934</span><span class="sxs-lookup"><span data-stu-id="20e0a-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="20e0a-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="20e0a-245">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="20e0a-246">「<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">パートナーごとに明細を示す</a>」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="20e0a-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="20e0a-247">4390934</span><span class="sxs-lookup"><span data-stu-id="20e0a-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="20e0a-248">DomainName</span></span></td>
<td><p><span data-ttu-id="20e0a-249">顧客を特定するために使用する顧客のドメイン名。</span><span class="sxs-lookup"><span data-stu-id="20e0a-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="20e0a-250">顧客/パートナーは O365 ポータルからバニティ/既定のドメインを更新できるため、顧客を一意に識別するためにこれを使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="20e0a-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="20e0a-251">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="20e0a-252">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="20e0a-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="20e0a-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="20e0a-254">サブスクリプションのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="20e0a-254">Subscription nickname.</span></span> <span data-ttu-id="20e0a-255">ニックネームが指定されていない場合、パートナー センターでは OfferName を使用します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="20e0a-256">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="20e0a-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="20e0a-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="20e0a-258">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="20e0a-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="20e0a-259">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="20e0a-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="20e0a-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span><span class="sxs-lookup"><span data-stu-id="20e0a-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="20e0a-261">使用量ベースのファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="20e0a-261">Usage-based file fields</span></span>


<span data-ttu-id="20e0a-262">顧客の使用量に対する料金を調整するには、調整ファイルの ResellerID/ResellerName/ResellerBillableAccount、顧客名、およびパートナー センターのサブスクリプション ID を比較します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="20e0a-263">次のフィールドで、どのサービスが使用されるか、およびレートについて説明します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="20e0a-264"><strong>列</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="20e0a-265"><strong>説明</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="20e0a-266"><strong>サンプル値</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="20e0a-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="20e0a-268">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="20e0a-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="20e0a-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="20e0a-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="20e0a-271">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="20e0a-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="20e0a-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="20e0a-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="20e0a-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="20e0a-274">パートナーのアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="20e0a-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="20e0a-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="20e0a-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="20e0a-277">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="20e0a-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="20e0a-278">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="20e0a-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="20e0a-279">Test Customer A</span><span class="sxs-lookup"><span data-stu-id="20e0a-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="20e0a-280">MPNID</span></span></td>
<td><p><span data-ttu-id="20e0a-281">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="20e0a-282">4390934</span><span class="sxs-lookup"><span data-stu-id="20e0a-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="20e0a-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="20e0a-284">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="20e0a-285">「<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">パートナーごとに明細を示す</a>」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="20e0a-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="20e0a-286">4390934</span><span class="sxs-lookup"><span data-stu-id="20e0a-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="20e0a-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="20e0a-288">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="20e0a-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="20e0a-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="20e0a-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="20e0a-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="20e0a-291">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="20e0a-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="20e0a-292">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20e0a-293">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="20e0a-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="20e0a-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="20e0a-295">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="20e0a-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="20e0a-296">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="20e0a-297">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="20e0a-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="20e0a-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="20e0a-299">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20e0a-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="20e0a-300">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="20e0a-301">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="20e0a-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="20e0a-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="20e0a-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="20e0a-304">サービス プランのニックネーム。</span><span class="sxs-lookup"><span data-stu-id="20e0a-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="20e0a-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="20e0a-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="20e0a-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="20e0a-307">サービス プランの基幹業務</span><span class="sxs-lookup"><span data-stu-id="20e0a-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="20e0a-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="20e0a-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="20e0a-309">OrderID</span></span></td>
<td><p><span data-ttu-id="20e0a-310">Microsoft 請求プラットフォームでの注文の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20e0a-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="20e0a-311">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="20e0a-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="20e0a-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="20e0a-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="20e0a-314">対象の Azure サービスの名前。</span><span class="sxs-lookup"><span data-stu-id="20e0a-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="20e0a-315">VIRTUAL MACHINES</span><span class="sxs-lookup"><span data-stu-id="20e0a-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="20e0a-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="20e0a-317">Windows Azure サービスの特定の種類。</span><span class="sxs-lookup"><span data-stu-id="20e0a-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="20e0a-318">Service Bus – Individual or Pack</span><span class="sxs-lookup"><span data-stu-id="20e0a-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="20e0a-319">SQL Azure database – Business or Web Edition</span><span class="sxs-lookup"><span data-stu-id="20e0a-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="20e0a-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="20e0a-321">すべてのサービス データおよび価格設定構造の特定の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20e0a-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="20e0a-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="20e0a-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-323">リソース名</span><span class="sxs-lookup"><span data-stu-id="20e0a-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="20e0a-324">Azure リソースの名前。</span><span class="sxs-lookup"><span data-stu-id="20e0a-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="20e0a-325">Data Transfer In (GB)</span><span class="sxs-lookup"><span data-stu-id="20e0a-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="20e0a-326">Data Transfer Out (GB)</span><span class="sxs-lookup"><span data-stu-id="20e0a-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-327">Region</span><span class="sxs-lookup"><span data-stu-id="20e0a-327">Region</span></span></td>
<td><p><span data-ttu-id="20e0a-328">使用量が適用される地域。</span><span class="sxs-lookup"><span data-stu-id="20e0a-328">The region the usage applies to.</span></span> <span data-ttu-id="20e0a-329">料金は地域によって異なるため、主にデータ転送に料金を割り当てるために使われます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="20e0a-330">Asia Pacific、Europe、Latin America、North America</span><span class="sxs-lookup"><span data-stu-id="20e0a-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-331">SKU</span><span class="sxs-lookup"><span data-stu-id="20e0a-331">SKU</span></span></td>
<td><p><span data-ttu-id="20e0a-332">プランについての MSFT の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="20e0a-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="20e0a-333">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="20e0a-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="20e0a-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="20e0a-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="20e0a-335">特定の課金期間のサービスまたはリソースに対してさまざまなレートの明細を設定するための ID と数量。</span><span class="sxs-lookup"><span data-stu-id="20e0a-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="20e0a-336">Azure の階層化されたレーティングの場合は、一定数量の課金可能単位までは 1 つのレートがあり、その後に別のレートがあることがあります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="20e0a-337">1</span><span class="sxs-lookup"><span data-stu-id="20e0a-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="20e0a-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="20e0a-339">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="20e0a-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="20e0a-340">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="20e0a-341">11</span><span class="sxs-lookup"><span data-stu-id="20e0a-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="20e0a-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="20e0a-343">単位数はプランの一部として含まれます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-343">Units included as part of the offer.</span></span> <span data-ttu-id="20e0a-344">通常、CSP には含まれません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="20e0a-345">0</span><span class="sxs-lookup"><span data-stu-id="20e0a-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="20e0a-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="20e0a-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="20e0a-347">単位数はプランの一部として含まれず、パートナーが支払う必要があります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="20e0a-348">ConsumedQuantity - IncludedQuantity と同じです。</span><span class="sxs-lookup"><span data-stu-id="20e0a-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="20e0a-349">11</span><span class="sxs-lookup"><span data-stu-id="20e0a-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="20e0a-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="20e0a-351">サブスクリプションの開始日に有効な価格を提供します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="20e0a-352">$0.0808</span><span class="sxs-lookup"><span data-stu-id="20e0a-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="20e0a-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="20e0a-354">ListPrist と OverageQuantity を掛けて、最も近いセントに丸めます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="20e0a-355">$0.085</span><span class="sxs-lookup"><span data-stu-id="20e0a-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="20e0a-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="20e0a-357">市場の税制や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="20e0a-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="20e0a-358">$0.08</span><span class="sxs-lookup"><span data-stu-id="20e0a-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="20e0a-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="20e0a-360">税が適用されるときの税引き後の合計額。</span><span class="sxs-lookup"><span data-stu-id="20e0a-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="20e0a-361">$0.93</span><span class="sxs-lookup"><span data-stu-id="20e0a-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-362">通貨</span><span class="sxs-lookup"><span data-stu-id="20e0a-362">Currency</span></span></td>
<td><p><span data-ttu-id="20e0a-363">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="20e0a-363">Currency type.</span></span> <span data-ttu-id="20e0a-364">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="20e0a-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="20e0a-365">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="20e0a-366">EUR</span><span class="sxs-lookup"><span data-stu-id="20e0a-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="20e0a-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="20e0a-368">単位あたりの税込み価格。</span><span class="sxs-lookup"><span data-stu-id="20e0a-368">Pretax price per unit.</span></span> <span data-ttu-id="20e0a-369">PretaxCharges / OverageQuantity と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="20e0a-370">$0.08</span><span class="sxs-lookup"><span data-stu-id="20e0a-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="20e0a-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="20e0a-372">単位あたりの税引き後の価格。</span><span class="sxs-lookup"><span data-stu-id="20e0a-372">Post tax price per unit.</span></span> <span data-ttu-id="20e0a-373">PostTaxTotal / OverageQuantity、または PretaxEffectiveRate + 単位額あたりの税率と同じで、最も近いセントに丸められます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="20e0a-374">$0.08</span><span class="sxs-lookup"><span data-stu-id="20e0a-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="20e0a-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="20e0a-376">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="20e0a-376">The type of charge or adjustment.</span></span> <span data-ttu-id="20e0a-377">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20e0a-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="20e0a-378">「<a href="#charge_types">請求書と調整ファイルの間の課金のマッピング</a>」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20e0a-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="20e0a-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="20e0a-380">MSFT 課金プラットフォームの一意のアカウント ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="20e0a-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="20e0a-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="20e0a-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="20e0a-383">サービスの展開の日付。</span><span class="sxs-lookup"><span data-stu-id="20e0a-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="20e0a-384">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="20e0a-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="20e0a-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="20e0a-386">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="20e0a-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span><span class="sxs-lookup"><span data-stu-id="20e0a-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="20e0a-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="20e0a-389">この列は、[Service Name] 列で特に識別されない可能性のある、個別の Microsoft Azure サービスの追跡に利用されます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="20e0a-390">たとえば、データ転送は、[Service Name] 列で &quot;Microsoft Azure - All Services&quot; と報告されます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="20e0a-391">この [MeteredService] 列は、利用に関連する特定のサービスを示します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="20e0a-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span><span class="sxs-lookup"><span data-stu-id="20e0a-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="20e0a-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="20e0a-394">個々の Microsoft Azure サービスの内容を、MeteredService フィールドで提供されるレベルよりも明確にする小見出し。</span><span class="sxs-lookup"><span data-stu-id="20e0a-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="20e0a-395">EXTERNAL</span><span class="sxs-lookup"><span data-stu-id="20e0a-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-396">Project</span><span class="sxs-lookup"><span data-stu-id="20e0a-396">Project</span></span></td>
<td><p><span data-ttu-id="20e0a-397">サービス インスタンスの顧客定義の名前</span><span class="sxs-lookup"><span data-stu-id="20e0a-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="20e0a-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="20e0a-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="20e0a-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="20e0a-400">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="20e0a-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="20e0a-401">例: 1 か月 30 日間の中に、個別にプロビジョニングされた接続がある場合、Service Info 1 は "1.000000 Connections / 30 days" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="20e0a-402">プロビジョニングされた ServiceBus 接続が 25 パックあり、その日のうちに 1 つを利用した場合、その日の 1 日の使用量の計算書には、"25 Connections / 30 Days – Used:1.000000" と表示されます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="20e0a-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="20e0a-404">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="20e0a-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="20e0a-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20e0a-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="20e0a-406">DomainName</span></span></td>
<td><p><span data-ttu-id="20e0a-407">顧客を特定するために使用する顧客のドメイン名。</span><span class="sxs-lookup"><span data-stu-id="20e0a-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="20e0a-408">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="20e0a-409">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="20e0a-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="20e0a-410">Unit</span><span class="sxs-lookup"><span data-stu-id="20e0a-410">Unit</span></span></td>
<td><p><span data-ttu-id="20e0a-411">リソース名の単位</span><span class="sxs-lookup"><span data-stu-id="20e0a-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="20e0a-412">GB または HOURS</span><span class="sxs-lookup"><span data-stu-id="20e0a-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="20e0a-413">1 回限りおよび定期的なファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="20e0a-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="20e0a-414">列</span><span class="sxs-lookup"><span data-stu-id="20e0a-414">Column</span></span></th>
<th><span data-ttu-id="20e0a-415">説明</span><span class="sxs-lookup"><span data-stu-id="20e0a-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="20e0a-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="20e0a-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="20e0a-417">特定の課金エンティティに対する一意の Microsoft Azure Active Directory テナント識別子 (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="20e0a-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="20e0a-418">調整には必要ありませんが、有用な情報である場合があります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="20e0a-419">すべての行で同じです。</span><span class="sxs-lookup"><span data-stu-id="20e0a-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-420">Customer Id</span><span class="sxs-lookup"><span data-stu-id="20e0a-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="20e0a-421">顧客を識別するために使用される、GUID 形式の一意の Microsoft Azure Active Directory テナント ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-422">顧客名</span><span class="sxs-lookup"><span data-stu-id="20e0a-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="20e0a-423">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="20e0a-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="20e0a-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="20e0a-425">顧客のドメイン名。顧客を特定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="20e0a-426">顧客/パートナーは O365 ポータルからバニティ/既定のドメインを更新できるため、顧客を一意に識別するためにこれを使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="20e0a-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="20e0a-427">このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-428">Customer Country</span><span class="sxs-lookup"><span data-stu-id="20e0a-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="20e0a-429">顧客の在住国。</span><span class="sxs-lookup"><span data-stu-id="20e0a-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-430">請求書番号</span><span class="sxs-lookup"><span data-stu-id="20e0a-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="20e0a-431">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="20e0a-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="20e0a-432">MpnId</span></span></td>
<td><p><span data-ttu-id="20e0a-433">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-434">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="20e0a-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="20e0a-435">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-436">Order ID</span><span class="sxs-lookup"><span data-stu-id="20e0a-436">Order ID</span></span></td>
<td><p><span data-ttu-id="20e0a-437">Microsoft コマース プラットフォームでの注文に対する一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20e0a-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="20e0a-438">サポートに問い合わせる際に、注文の識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-439">発注日</span><span class="sxs-lookup"><span data-stu-id="20e0a-439">Order date</span></span></td>
<td><p><span data-ttu-id="20e0a-440">注文が作成された日付。</span><span class="sxs-lookup"><span data-stu-id="20e0a-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="20e0a-441">ProductId</span></span></td>
<td><p><span data-ttu-id="20e0a-442">製品の ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="20e0a-443">SkuId</span></span></td>
<td><p><span data-ttu-id="20e0a-444">特定 SKU の ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="20e0a-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="20e0a-446">特定の可用性 の ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-446">The ID for a particular Availability.</span></span> <span data-ttu-id="20e0a-447">"可用性" とは、特定の国、通貨、業界などで特定の SKU を購入可能かどうかを指します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-448">SKU Name</span><span class="sxs-lookup"><span data-stu-id="20e0a-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="20e0a-449">特定 SKU のタイトル。</span><span class="sxs-lookup"><span data-stu-id="20e0a-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-450">製品名</span><span class="sxs-lookup"><span data-stu-id="20e0a-450">Product name</span></span></td>
<td><p><span data-ttu-id="20e0a-451">製品の名前。</span><span class="sxs-lookup"><span data-stu-id="20e0a-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="20e0a-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="20e0a-453">製品の発行元の名前。</span><span class="sxs-lookup"><span data-stu-id="20e0a-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="20e0a-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="20e0a-455">この発行元の一意の ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-456">Subscription Description</span><span class="sxs-lookup"><span data-stu-id="20e0a-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="20e0a-457">サブスクリプションのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="20e0a-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-458">サブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="20e0a-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="20e0a-459">Microsoft コマース プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20e0a-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="20e0a-460">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="20e0a-461">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="20e0a-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="20e0a-463">課金の開始日。</span><span class="sxs-lookup"><span data-stu-id="20e0a-463">Start day of the charges.</span></span> <span data-ttu-id="20e0a-464">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="20e0a-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="20e0a-466">課金の終了日。</span><span class="sxs-lookup"><span data-stu-id="20e0a-466">End day of the charges.</span></span> <span data-ttu-id="20e0a-467">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-468">Term and Billingcycle</span><span class="sxs-lookup"><span data-stu-id="20e0a-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="20e0a-469">購入の期間と請求サイクル。</span><span class="sxs-lookup"><span data-stu-id="20e0a-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="20e0a-470">例: “1 Year, Monthly” (1 年、月単位)。</span><span class="sxs-lookup"><span data-stu-id="20e0a-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-471">請求の種類</span><span class="sxs-lookup"><span data-stu-id="20e0a-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="20e0a-472">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="20e0a-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-473">単価</span><span class="sxs-lookup"><span data-stu-id="20e0a-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="20e0a-474">購入時に価格表に公開されていた価格。</span><span class="sxs-lookup"><span data-stu-id="20e0a-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="20e0a-475">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-476">Effective Unit Price</span><span class="sxs-lookup"><span data-stu-id="20e0a-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="20e0a-477">調整が行われた後の単価。</span><span class="sxs-lookup"><span data-stu-id="20e0a-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-478">Quantity</span><span class="sxs-lookup"><span data-stu-id="20e0a-478">Quantity</span></span></td>
<td><p><span data-ttu-id="20e0a-479">ユニット数。</span><span class="sxs-lookup"><span data-stu-id="20e0a-479">Number of units.</span></span> <span data-ttu-id="20e0a-480">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-481">Unit type</span><span class="sxs-lookup"><span data-stu-id="20e0a-481">Unit type</span></span></td>
<td><p><span data-ttu-id="20e0a-482">購入したユニットの種類。</span><span class="sxs-lookup"><span data-stu-id="20e0a-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="20e0a-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="20e0a-484">適用可能なすべての割引の説明。</span><span class="sxs-lookup"><span data-stu-id="20e0a-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-485">Sub Total</span><span class="sxs-lookup"><span data-stu-id="20e0a-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="20e0a-486">合計額 (税抜)。</span><span class="sxs-lookup"><span data-stu-id="20e0a-486">Total before tax.</span></span> <span data-ttu-id="20e0a-487">割引の場合、小計が、予想される合計と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-488">Tax Total</span><span class="sxs-lookup"><span data-stu-id="20e0a-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="20e0a-489">市場の税関連の規則や特定の状況に基づく税金の額。</span><span class="sxs-lookup"><span data-stu-id="20e0a-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-490">Total</span><span class="sxs-lookup"><span data-stu-id="20e0a-490">Total</span></span></td>
<td><p><span data-ttu-id="20e0a-491">合計額 (税込)。</span><span class="sxs-lookup"><span data-stu-id="20e0a-491">Total after tax.</span></span> <span data-ttu-id="20e0a-492">請求書に課税されるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-493">通貨</span><span class="sxs-lookup"><span data-stu-id="20e0a-493">Currency</span></span></td>
<td><p><span data-ttu-id="20e0a-494">通貨の種類。</span><span class="sxs-lookup"><span data-stu-id="20e0a-494">Currency type.</span></span> <span data-ttu-id="20e0a-495">各課金エンティティの通貨は 1 つのみです。</span><span class="sxs-lookup"><span data-stu-id="20e0a-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="20e0a-496">最初の請求書と一致し、その後で、主要な課金プラットフォームの更新と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="20e0a-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="20e0a-498">注文 ID の代替識別子。</span><span class="sxs-lookup"><span data-stu-id="20e0a-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="20e0a-499">毎日評価される使用量ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="20e0a-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="20e0a-500">列</span><span class="sxs-lookup"><span data-stu-id="20e0a-500">Column</span></span></th>
<th><span data-ttu-id="20e0a-501">説明</span><span class="sxs-lookup"><span data-stu-id="20e0a-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="20e0a-502">PartnerId</span><span class="sxs-lookup"><span data-stu-id="20e0a-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="20e0a-503">GUID 形式のパートナー ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="20e0a-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="20e0a-505">パートナー名。</span><span class="sxs-lookup"><span data-stu-id="20e0a-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-506">CustomerId</span><span class="sxs-lookup"><span data-stu-id="20e0a-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="20e0a-507">顧客を識別するために使用される、GUID 形式の一意の Microsoft ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="20e0a-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="20e0a-509">パートナー センターで報告される顧客の組織名。</span><span class="sxs-lookup"><span data-stu-id="20e0a-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="20e0a-510">これは、システムの情報を使って請求書を調整するために非常に重要です。</span><span class="sxs-lookup"><span data-stu-id="20e0a-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="20e0a-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="20e0a-512">顧客のドメイン名。</span><span class="sxs-lookup"><span data-stu-id="20e0a-512">The customer’s domain name.</span></span> <span data-ttu-id="20e0a-513">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-514">Customer country</span><span class="sxs-lookup"><span data-stu-id="20e0a-514">Customer country</span></span></td>
<td><p><span data-ttu-id="20e0a-515">顧客の在住国。</span><span class="sxs-lookup"><span data-stu-id="20e0a-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-516">MPNID</span><span class="sxs-lookup"><span data-stu-id="20e0a-516">MPNID</span></span></td>
<td><p><span data-ttu-id="20e0a-517">CSP パートナーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-518">Reseller MPNID</span><span class="sxs-lookup"><span data-stu-id="20e0a-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="20e0a-519">サブスクリプションの登録のあるリセラーの MPN ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="20e0a-520">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="20e0a-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="20e0a-522">指定されたトランザクションが含まれる請求書番号。</span><span class="sxs-lookup"><span data-stu-id="20e0a-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="20e0a-523">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-524">ProductId</span><span class="sxs-lookup"><span data-stu-id="20e0a-524">ProductId</span></span></td>
<td><p><span data-ttu-id="20e0a-525">製品の ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="20e0a-526">SkuId</span></span></td>
<td><p><span data-ttu-id="20e0a-527">特定 SKU の ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="20e0a-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="20e0a-529">特定の可用性 の ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-529">The ID for a particular Availability.</span></span> <span data-ttu-id="20e0a-530">"可用性" とは、特定の国、通貨、業界などで特定の SKU を購入可能かどうかを指します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-531">SKU Name</span><span class="sxs-lookup"><span data-stu-id="20e0a-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="20e0a-532">特定 SKU のタイトル。</span><span class="sxs-lookup"><span data-stu-id="20e0a-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="20e0a-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="20e0a-534">発行元の名前。</span><span class="sxs-lookup"><span data-stu-id="20e0a-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="20e0a-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="20e0a-536">発行元の ID (GUID 形式)。</span><span class="sxs-lookup"><span data-stu-id="20e0a-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="20e0a-537">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="20e0a-538">Subscription Description</span><span class="sxs-lookup"><span data-stu-id="20e0a-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="20e0a-539">価格表で定義されている、顧客が購入したサービス プランの名前。</span><span class="sxs-lookup"><span data-stu-id="20e0a-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="20e0a-540">(これはプラン名と同一のフィールドです)。</span><span class="sxs-lookup"><span data-stu-id="20e0a-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-541">サブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="20e0a-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="20e0a-542">Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="20e0a-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="20e0a-543">サポートに問い合わせる際に、サブスクリプションの識別に有効な場合がありますが、調整には有用ではありません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="20e0a-544">これは、パートナー管理コンソールのサブスクリプション ID と同じではありません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="20e0a-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="20e0a-546">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの開始日。</span><span class="sxs-lookup"><span data-stu-id="20e0a-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="20e0a-547">時刻は常に、その日の始まりの時刻 (0:00) になります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="20e0a-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="20e0a-549">前の課金サイクルからの潜在的な未請求の使用状況データの日付を提示するときを除く、課金サイクルの終了日。</span><span class="sxs-lookup"><span data-stu-id="20e0a-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="20e0a-550">時刻は常に、その日の終わりの時刻 (23:59) になります。</span><span class="sxs-lookup"><span data-stu-id="20e0a-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-551">Usage Date</span><span class="sxs-lookup"><span data-stu-id="20e0a-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="20e0a-552">サービス使用の日付。</span><span class="sxs-lookup"><span data-stu-id="20e0a-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-553">Meter Type</span><span class="sxs-lookup"><span data-stu-id="20e0a-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="20e0a-554">メーターの種類。</span><span class="sxs-lookup"><span data-stu-id="20e0a-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-555">Meter Category</span><span class="sxs-lookup"><span data-stu-id="20e0a-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="20e0a-556">使用状況の最上位サービス。</span><span class="sxs-lookup"><span data-stu-id="20e0a-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-557">Meter Id</span><span class="sxs-lookup"><span data-stu-id="20e0a-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="20e0a-558">使用されているメーターの ID。</span><span class="sxs-lookup"><span data-stu-id="20e0a-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-559">Meter Sub-category</span><span class="sxs-lookup"><span data-stu-id="20e0a-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="20e0a-560">速度に影響を与える可能性がある Azure サービスの種類。</span><span class="sxs-lookup"><span data-stu-id="20e0a-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-561">Meter Name</span><span class="sxs-lookup"><span data-stu-id="20e0a-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="20e0a-562">使用しているメーターの測定単位。</span><span class="sxs-lookup"><span data-stu-id="20e0a-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-563">Meter Region</span><span class="sxs-lookup"><span data-stu-id="20e0a-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="20e0a-564">この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-565">Unit</span><span class="sxs-lookup"><span data-stu-id="20e0a-565">Unit</span></span></td>
<td><p><span data-ttu-id="20e0a-566">リソース名の単位。</span><span class="sxs-lookup"><span data-stu-id="20e0a-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-567">Consumed Quantity</span><span class="sxs-lookup"><span data-stu-id="20e0a-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="20e0a-568">レポート期間のサービスの使用量 (時間、GB など)。</span><span class="sxs-lookup"><span data-stu-id="20e0a-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="20e0a-569">前のレポート期間から課金していない使用も含まれます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-570">Resource Location</span><span class="sxs-lookup"><span data-stu-id="20e0a-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="20e0a-571">メーターが実行されているデータ センター。</span><span class="sxs-lookup"><span data-stu-id="20e0a-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-572">Consumed Service</span><span class="sxs-lookup"><span data-stu-id="20e0a-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="20e0a-573">使用した Azure プラットフォーム サービス。</span><span class="sxs-lookup"><span data-stu-id="20e0a-573">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="20e0a-574">Resource URI</span><span class="sxs-lookup"><span data-stu-id="20e0a-574">Resource URI</span></span></td>
<td><p><span data-ttu-id="20e0a-575">使用されているリソースの URI。</span><span class="sxs-lookup"><span data-stu-id="20e0a-575">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-576">請求の種類</span><span class="sxs-lookup"><span data-stu-id="20e0a-576">Charge type</span></span></td>
<td><p><span data-ttu-id="20e0a-577">課金または調整の種類。</span><span class="sxs-lookup"><span data-stu-id="20e0a-577">The type of charge or adjustment.</span></span> <span data-ttu-id="20e0a-578">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-578">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-579">単価</span><span class="sxs-lookup"><span data-stu-id="20e0a-579">Unit price</span></span></td>
<td><p><span data-ttu-id="20e0a-580">ライセンス単価 (購入時に価格表に公開されていた価格)。</span><span class="sxs-lookup"><span data-stu-id="20e0a-580">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="20e0a-581">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-581">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-582">Quantity</span><span class="sxs-lookup"><span data-stu-id="20e0a-582">Quantity</span></span></td>
<td><p><span data-ttu-id="20e0a-583">ライセンス数。</span><span class="sxs-lookup"><span data-stu-id="20e0a-583">Number of licenses.</span></span> <span data-ttu-id="20e0a-584">調整中に、請求システムに格納された情報と一致することを確認します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-584">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-585">Unit type</span><span class="sxs-lookup"><span data-stu-id="20e0a-585">Unit type</span></span></td>
<td><p><span data-ttu-id="20e0a-586">メーターが課金するユニットの種類。</span><span class="sxs-lookup"><span data-stu-id="20e0a-586">The type of unit the meter is charged in.</span></span> <span data-ttu-id="20e0a-587">現在のアクティビティには使用できません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-587">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-588">Billing pre tax</span><span class="sxs-lookup"><span data-stu-id="20e0a-588">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="20e0a-589">税引き前の合計金額。</span><span class="sxs-lookup"><span data-stu-id="20e0a-589">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-590">Billing currency</span><span class="sxs-lookup"><span data-stu-id="20e0a-590">Billing currency</span></span></td>
<td><p><span data-ttu-id="20e0a-591">顧客の地理的領域での通貨</span><span class="sxs-lookup"><span data-stu-id="20e0a-591">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-592">Pricing pretax total</span><span class="sxs-lookup"><span data-stu-id="20e0a-592">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="20e0a-593">税金が追加される前の価格。</span><span class="sxs-lookup"><span data-stu-id="20e0a-593">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-594">Pricing currency</span><span class="sxs-lookup"><span data-stu-id="20e0a-594">Pricing currency</span></span></td>
<td><p><span data-ttu-id="20e0a-595">価格表の通貨。</span><span class="sxs-lookup"><span data-stu-id="20e0a-595">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20e0a-596">Service Info 1</span><span class="sxs-lookup"><span data-stu-id="20e0a-596">Service Info 1</span></span></td>
<td><p><span data-ttu-id="20e0a-597">特定の日にプロビジョニングされ、利用された ServiceBus 接続の数。</span><span class="sxs-lookup"><span data-stu-id="20e0a-597">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-598">Service Info 2</span><span class="sxs-lookup"><span data-stu-id="20e0a-598">Service Info 2</span></span></td>
<td><p><span data-ttu-id="20e0a-599">省略可能なサービスに固有のメタデータをキャプチャするレガシ フィールド。</span><span class="sxs-lookup"><span data-stu-id="20e0a-599">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20e0a-600">Additional Info</span><span class="sxs-lookup"><span data-stu-id="20e0a-600">Additional Info</span></span></td>
<td><p><span data-ttu-id="20e0a-601">他の列で網羅されていないすべての追加情報。</span><span class="sxs-lookup"><span data-stu-id="20e0a-601">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="20e0a-602">請求書と調整ファイルの間の課金のマッピング</span><span class="sxs-lookup"><span data-stu-id="20e0a-602">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="20e0a-603">請求書は料金の概要を示し、調整ファイルは、課金の種類を含め、行項目のトランザクションの詳細な内訳を示します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-603">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="20e0a-604">請求書と調整ファイルの間で請求金額を相互参照するには、Microsoft Excel のフィルター オプションを使用して、調整ファイルの課金の種類でフィルター処理し、請求書の課金を調整ファイルの一連の課金の内訳にマップします。</span><span class="sxs-lookup"><span data-stu-id="20e0a-604">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="20e0a-605">使用量ベースとライセンス ベースの調整ファイルには、使用量関連のトランザクションと料金 (消費された単位量および関連する料金) のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-605">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="20e0a-606">請求書に “調整” として表示される単発のクレジット、割引、払い戻し金額は、調整ファイルに表示されません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-606">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="20e0a-607">次の表に、請求書のセクションと、調整ファイルに表示される関連付けられた課金の種類とのマッピングを示します。</span><span class="sxs-lookup"><span data-stu-id="20e0a-607">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="20e0a-608"><strong>請求書の課金の説明</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-608"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-609"><strong>調整ファイルの課金の説明 (ChargeType 列)</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-609"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-610"><strong>この課金の意味</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-610"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-611"><strong>これらの ChargeTypes を請求書にマップする方法</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-611"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="20e0a-612"><strong>ライセンスベースの料金</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-612"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-613">アクティブ化料金</span><span class="sxs-lookup"><span data-stu-id="20e0a-613">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-614">購入したサブスクリプションを顧客が使用したときに顧客に課金される金額</span><span class="sxs-lookup"><span data-stu-id="20e0a-614">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="20e0a-615">ライセンスベースのファイルから、<strong>Amount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20e0a-615">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-616">取り消し料金</span><span class="sxs-lookup"><span data-stu-id="20e0a-616">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-617">関連付けられているシートが変更されたときに顧客に払い戻される日割り料金</span><span class="sxs-lookup"><span data-stu-id="20e0a-617">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-618">Cycle fee</span><span class="sxs-lookup"><span data-stu-id="20e0a-618">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-619">サブスクリプションの定期的な課金</span><span class="sxs-lookup"><span data-stu-id="20e0a-619">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-620">Cycle instance prorate</span><span class="sxs-lookup"><span data-stu-id="20e0a-620">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-621">関連付けられているシートが変更されたときに顧客から評価される日割り料金</span><span class="sxs-lookup"><span data-stu-id="20e0a-621">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-622">Prorate fees when cancel</span><span class="sxs-lookup"><span data-stu-id="20e0a-622">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-623">取り消し時のサービスの未使用部分に対する日割りの払戻し額</span><span class="sxs-lookup"><span data-stu-id="20e0a-623">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-624">Prorate fees when purchase</span><span class="sxs-lookup"><span data-stu-id="20e0a-624">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-625">年次請求を使用する場合のサブスクリプションの料金タイプ</span><span class="sxs-lookup"><span data-stu-id="20e0a-625">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-626">Purchase fee</span><span class="sxs-lookup"><span data-stu-id="20e0a-626">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-627">月次請求を使用する場合のサブスクリプションの料金タイプ</span><span class="sxs-lookup"><span data-stu-id="20e0a-627">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-628">Prorate fee when renew</span><span class="sxs-lookup"><span data-stu-id="20e0a-628">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-629">サブスクリプションの更新時の日割り料金</span><span class="sxs-lookup"><span data-stu-id="20e0a-629">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="20e0a-630">Renew fee</span><span class="sxs-lookup"><span data-stu-id="20e0a-630">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-631">サブスクリプションの更新時の課金</span><span class="sxs-lookup"><span data-stu-id="20e0a-631">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-632">Prorate fees when activate</span><span class="sxs-lookup"><span data-stu-id="20e0a-632">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-633">アクティブ化から課金期間の終了までの日割り料金</span><span class="sxs-lookup"><span data-stu-id="20e0a-633">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="20e0a-634"><strong>1 回限りの料金</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-634"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="20e0a-635">新規</span><span class="sxs-lookup"><span data-stu-id="20e0a-635">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-636">新しい発注を作成するときに使用</span><span class="sxs-lookup"><span data-stu-id="20e0a-636">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-637">addQuantity</span><span class="sxs-lookup"><span data-stu-id="20e0a-637">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-638">増加した後、元の購入と新しい数量の両方、返金で使用されます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-638">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-639">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="20e0a-639">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-640">減少後の元の購入と新しい数量の両方、返金で使用されます。</span><span class="sxs-lookup"><span data-stu-id="20e0a-640">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-641">Cancel</span><span class="sxs-lookup"><span data-stu-id="20e0a-641">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-642">サブスクリプションが取り消されたときに使用</span><span class="sxs-lookup"><span data-stu-id="20e0a-642">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-643">Convert</span><span class="sxs-lookup"><span data-stu-id="20e0a-643">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-644">ライセンスのアップグレードが接続クライアントの数は変更されません。</span><span class="sxs-lookup"><span data-stu-id="20e0a-644">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="20e0a-645"><strong>利用料金</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-645"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-646">Assess usage fee when cancel</span><span class="sxs-lookup"><span data-stu-id="20e0a-646">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-647">現在の課金期間中に未払いの使用を取り消したときのアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="20e0a-647">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="20e0a-648">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20e0a-648">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-649">Assess usage fee for current cycle</span><span class="sxs-lookup"><span data-stu-id="20e0a-649">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-650">現在の課金期間のアクセス利用料</span><span class="sxs-lookup"><span data-stu-id="20e0a-650">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="20e0a-651"><strong>クレジット</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-651"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-652">Offset a line item</span><span class="sxs-lookup"><span data-stu-id="20e0a-652">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-653">税金を含む、行項目への一部または全部の払戻し</span><span class="sxs-lookup"><span data-stu-id="20e0a-653">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-654">ライセンスベースのファイルから、<strong>TotalForCustomer</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20e0a-654">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="20e0a-655">使用量ベースのファイルから、<strong>PostTaxTotal</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20e0a-655">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="20e0a-656"><strong>使用量ベースの割引</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-656"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-657">Activation discount</span><span class="sxs-lookup"><span data-stu-id="20e0a-657">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-658">サブスクリプションがアクティブ化されたときに適用される割引</span><span class="sxs-lookup"><span data-stu-id="20e0a-658">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="20e0a-659">使用量ベースのファイルから、<strong>PretaxCharges</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20e0a-659">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-660">Cycle discount</span><span class="sxs-lookup"><span data-stu-id="20e0a-660">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-661">定期的な課金に適用される割引</span><span class="sxs-lookup"><span data-stu-id="20e0a-661">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-662">Renew discount</span><span class="sxs-lookup"><span data-stu-id="20e0a-662">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-663">サブスクリプションの更新時に適用される割引</span><span class="sxs-lookup"><span data-stu-id="20e0a-663">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-664">Cancel discount</span><span class="sxs-lookup"><span data-stu-id="20e0a-664">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-665">割引が取り消されたときに適用される料金</span><span class="sxs-lookup"><span data-stu-id="20e0a-665">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="20e0a-666"><strong>ライセンスベースの割引</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-666"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-667"><em>複数の種類の料金に適用される場合がある</em></span><span class="sxs-lookup"><span data-stu-id="20e0a-667"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="20e0a-668">ライセンスベースのファイルから、<strong>TotalOtherDiscount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20e0a-668">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20e0a-669"><strong>税</strong>&nbsp;または&nbsp;<strong>VAT</strong></span><span class="sxs-lookup"><span data-stu-id="20e0a-669"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-670"><em>複数の種類の料金に適用される場合がある</em></span><span class="sxs-lookup"><span data-stu-id="20e0a-670"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="20e0a-671"><em>例外:&quot;Offset a line item&quot; には既に税が含まれています。上記の「クレジット」を参照してください。</em></span><span class="sxs-lookup"><span data-stu-id="20e0a-671"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-672">税または付加価値税 (VAT)</span><span class="sxs-lookup"><span data-stu-id="20e0a-672">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="20e0a-673">ライセンスベースのファイルから、<strong>Tax</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20e0a-673">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="20e0a-674">使用量ベースのファイルから、<strong>TaxAmount</strong> 列を合計する</span><span class="sxs-lookup"><span data-stu-id="20e0a-674">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
