---
title: Azure プラン - 請求 | パートナー センター
ms.topic: article
ms.date: 10/04/2019
description: 請求書と調整ファイルの構造について説明します
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 28e670635ca7fcff60041fcb5c93b3ddd5e4069d
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171299"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="d1ba8-103">CSP の新しいコマース エクスペリエンス - Azure の請求</span><span class="sxs-lookup"><span data-stu-id="d1ba8-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="d1ba8-104">Azure プランの請求は、調整された 1 つの請求日とカレンダーの月単位の請求期間を使用することで、請求エクスペリエンスが簡単になりました。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-104">Billing under the Azure plan is a simplified billing experience by using an aligned single billing date and calendar month-based billing period.</span></span> <span data-ttu-id="d1ba8-105">請求プラットフォームの詳細については、[Partner Center Modern Commerce Operating Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-105">For information on the billing platform, read  [Partner Center Modern Commerce Operating Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="d1ba8-106">請求の要点の概要</span><span class="sxs-lookup"><span data-stu-id="d1ba8-106">Summary of billing essentials</span></span>

- <span data-ttu-id="d1ba8-107">**請求日**:請求書と調整ファイルは、パートナー センター ダッシュボード/API で 8 日 (UTC 時間の午前 0 時) までに取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-107">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="d1ba8-108">**請求書の請求期間**:請求書の請求期間は、10/1 から 10/31、11/1 から 11/30 のように、カレンダーの月に合わせて調整されます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-108">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="d1ba8-109">**料金サービス期間**:料金はカレンダーの月に合わせて調整されます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-109">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="d1ba8-110">たとえば、請求先パートナーが 10/15 に Azure プランを介して Azure サービスを追加し、顧客が 10/15 に Azure サービスの使用を開始した場合、請求先パートナーは、サービス期間 10/15 から 10/31 の顧客の使用量に対して、11/8 に請求書/調整を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-110">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="d1ba8-111">12/8 に生成される翌月の請求書には、サービス期間 11/1 から 11/31 のすべての料金が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-111">The next month’s invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="d1ba8-112">**請求書の支払い条件**:請求日から 60 日以内。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-112">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="d1ba8-113">**請求書の通貨**:パートナーには、顧客の国の割り当て通貨で引き続き請求されます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-113">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="d1ba8-114">たとえば、請求先パートナーの拠点がアイルランドにあり、顧客が英国、ノルウェー、およびドイツに住んでいる場合、請求先パートナーは英国ポンド、ノルウェー クローネ、およびユーロの請求書/調整を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-114">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="d1ba8-115">**パートナー インセンティブ**:請求月の末日から 45 日以内に支払われます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-115">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

##  <a name="access-your-invoices-and-recon-files"></a><span data-ttu-id="d1ba8-116">請求書および調整ファイルにアクセスする</span><span class="sxs-lookup"><span data-stu-id="d1ba8-116">Access your invoices and recon files</span></span>

<span data-ttu-id="d1ba8-117">請求書を表示できる状態になると、会社の全体管理者または請求管理者にはメールが送信されます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-117">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> 

<span data-ttu-id="d1ba8-118">**請求書および調整ファイルにアクセスするには**</span><span class="sxs-lookup"><span data-stu-id="d1ba8-118">**To access the invoice and recon file**</span></span>

1. <span data-ttu-id="d1ba8-119">パートナー センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-119">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="d1ba8-120">パートナー センター メニューで **[請求]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-120">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="d1ba8-121">**[Calendar-based]\(カレンダーベース\)** のタブと、目的の通貨を選択します。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-121">Select the tab for the **Calendar-based** and currency you are interested in.</span></span>

![請求](images/azure/billing1.png)

4. <span data-ttu-id="d1ba8-123">**[Invoice and Recon file]\(請求書および調整ファイル\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-123">Select **Invoice and Recon file**.</span></span>  

<span data-ttu-id="d1ba8-124">過去の請求書および調整ファイルを表示するには、下の [請求履歴] 行を展開します。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-124">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="d1ba8-125">請求書の読み方</span><span class="sxs-lookup"><span data-stu-id="d1ba8-125">Read the invoice</span></span>

1. <span data-ttu-id="d1ba8-126">請求書は、毎月 8 日までに取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-126">Invoice will be available no later than the 8th of each month.</span></span>

2. <span data-ttu-id="d1ba8-127">パートナーには、60 日後に支払われます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-127">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="d1ba8-128">請求期間は、10/1 から 10/31 など、カレンダーの 1 か月間が対象になります。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-128">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="d1ba8-129">料金に調整額は含まれていません (金額に "管理対象のサービスのパートナー獲得クレジット" は含まれていません)。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-129">Charges are net of adjustments (amount is net of “Partner earned credit for services managed”).</span></span>

5. <span data-ttu-id="d1ba8-130">請求の詳細については、請求書および調整ファイルと毎日評価される使用量ファイルを確認します。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-130">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

![請求書](images/azure/invoice1.png)

## <a name="read-the-recon-file"></a><span data-ttu-id="d1ba8-132">調整ファイルの読み方</span><span class="sxs-lookup"><span data-stu-id="d1ba8-132">Read the recon file</span></span>

1. <span data-ttu-id="d1ba8-133">調整ファイルの各 Azure サブスクリプション メーターには、最大 2 行の請求明細が記載される場合があります。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-133">Each Azure subscription meter may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="d1ba8-134">メーターが、カレンダーの 1 か月間を通して何らかの種類の割引またはクレジット (階層 1 の割引やマネージド サービスのパートナー獲得クレジットなど) の対象となる場合、調整ファイルには 1 行の請求明細のみが記載されます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-134">If the meter qualified for any type of discount or credit (such as tier 1 discounts or the Partner earned credit for managed services) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="d1ba8-135">列 **PriceAdjusmentDescription** では、割引または獲得クレジットが参照されます。実効単価は、パートナー獲得クレジットまたはその他の割引を差し引いた小売価格になります。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-135">The column **PriceAdjusmentDescription** will reference the discount or earned credit; the effective unit price will be the retail price minus partner earned credit or any other discounts.</span></span>

3. <span data-ttu-id="d1ba8-136">メーターが、カレンダーの 1 か月間を通してマネージド サービスのパートナー獲得クレジットの対象とならない場合、調整ファイルに記載される請求明細は 1 行のみであり、実効単価は小売価格 (つまり単価) になります。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-136">If the meter didn’t qualify for the Partner earned credit for managed services throughout the entire calendar month, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="d1ba8-137">メーターが、1 か月間の一部について**マネージド サービスのパートナー獲得クレジット**の対象となる場合、調整ファイルには 2 行の請求明細が記載されます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-137">If the meter qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="d1ba8-138">1 行目はメーターが対象となる日数を表し、2 行目はメーターが対象とならない日数を表します。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-138">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span> 

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="d1ba8-139">毎日の使用量ファイルの読み方</span><span class="sxs-lookup"><span data-stu-id="d1ba8-139">Read the daily usage file</span></span>

- <span data-ttu-id="d1ba8-140">Azure プランのサブスクリプション メーターは日単位で評価され、蓄積されます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-140">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span> 

- <span data-ttu-id="d1ba8-141">**マネージド サービスのパートナー獲得クレジット**は、日単位で判断および適用されます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-141">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="d1ba8-142">すべてのサブスクリプション メーターには、消費があった月の毎日の行があります。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-142">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="d1ba8-143">次の例があるとします。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-143">In the example below:</span></span>

  - <span data-ttu-id="d1ba8-144">メーターは、7/1 から 7/3 に**マネージド サービスのパートナー獲得クレジット**の対象となりました (実効単価は、小売価格からパートナー獲得クレジットを差し引いた額であることに注意してください)。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-144">Meter qualified for **Partner earned credit for services managed** from 7/1 – 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

   - <span data-ttu-id="d1ba8-145">メーターは、7/4 から 7/7 に**マネージド サービスのパートナー獲得クレジット**の対象となりませんでした (実効単価は小売価格であることに注意してください)。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-145">Meter didn’t qualify for **Partner earned credit for services managed** from 7/4 – 7/7 (note the effective unit price is retail price).</span></span>

    - <span data-ttu-id="d1ba8-146">メーターは、7/8 から 7/31 に**マネージド サービスのパートナー獲得クレジット**の対象となりました (実効単価は、小売価格からパートナー獲得クレジットを差し引いた額であることに注意してください)。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-146">Meter qualified for **Partner earned credit for services managed** from 7/8 – 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

![recon2](images/azure/billing2.png) 

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="d1ba8-148">顧客の通貨での請求書</span><span class="sxs-lookup"><span data-stu-id="d1ba8-148">Invoice in customer currency</span></span> 

<span data-ttu-id="d1ba8-149">Azure プランを介した Azure サービスには、米国ドルで価格が設定され、顧客の国の割り当て通貨で請求されます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-149">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="d1ba8-150">請求通貨が米国ドル以外の場合は、使用された外国為替レートが請求書の最後のページに記載されます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-150">If the billing currency is non-USD, then the FX rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="d1ba8-151">外国為替レートは月ごとに決定され、次の請求書に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-151">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="d1ba8-152">国の通貨の詳細な一覧については、[新しいコマース オファーの国のリリース状況と顧客の通貨一覧](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-152">For a full list of country currencies, please view the [New commerce offers country availability and customer currency matrix](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V).</span></span> 

<span data-ttu-id="d1ba8-153">Microsoft は、請求書の通貨換算に対する価格設定の通貨を決定する際に、[Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) を使用して外国為替レートを決定しています。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-153">Microsoft will use [Thompson Reuters](https://developers.thomsonreuters.com/content/wm-company) to determine the FX rate used to determine pricing currency to invoice currency conversion.</span></span> <span data-ttu-id="d1ba8-154">外国為替レートは、適用される月の最初の日の前に更新され、使用されます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-154">The FX rate will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="d1ba8-155">**例**:8 月 1 日から 8 月 31 日までのサービス期間の使用料金は、8 月 1 日に公開された外国為替レートを使用して請求されます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-155">**Example**:  Usage charges for the service period August 1 – August 31 will be billed using the FX rate published on August 1.</span></span> <span data-ttu-id="d1ba8-156">これらの料金は 9 月の請求書に記載されます。外国為替レートは請求書の最後のページに記載されます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-156">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span> 

<span data-ttu-id="d1ba8-157">パートナー テナント ユーザーには、請求の通貨に関係なく、すべての顧客とすべての注文に関するロール固有の関連情報が引き続き表示されます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-157">Partner tenant users will continue to see role-specific related information regarding all customers and all orders, regardless of the billing currency.</span></span> <span data-ttu-id="d1ba8-158">さらに、ユーザーはすべての通貨のすべての請求書を表示できます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-158">Additionally, the user will be able to see all the invoices in all currencies.</span></span>  
 
## <a name="azure-reservations"></a><span data-ttu-id="d1ba8-159">Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="d1ba8-159">Azure reservations</span></span> 

<span data-ttu-id="d1ba8-160">Azure プランを介して [Azure Reservations](https://docs.microsoft.com/partner-center/azure-reservations) を購入した場合、最初に、パートナー センターで 1 回限りの請求を選択できます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-160">If purchasing [Azure reservations](https://docs.microsoft.com/partner-center/azure-reservations) through an Azure plan, initially,  it will only be possible to choose one-time billing in Partner Center.</span></span> <span data-ttu-id="d1ba8-161">毎月の請求は、Azure portal で確認できます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-161">Monthly billing is available on the Azure portal.</span></span> <span data-ttu-id="d1ba8-162">毎月の請求は、後日、パートナー センターで確認できるようになります。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-162">Monthly billing will be available in Partner Center at a later date.</span></span> 

## <a name="azure-cost-management"></a><span data-ttu-id="d1ba8-163">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="d1ba8-163">Azure cost management</span></span> 

<span data-ttu-id="d1ba8-164">Azure Cost Management ツールを使用すると、組織が Microsoft Azure 全体のコストを視覚化、管理、最適化するために役立ちます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-164">Azure Cost Management tools will help organizations visualize, manage and optimize costs across Microsoft Azure.</span></span> <span data-ttu-id="d1ba8-165">この機能は、Azure portal で使用できます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-165">This feature will be available in the Azure portal.</span></span> <span data-ttu-id="d1ba8-166">パートナーには、次の機能を利用できる常時接続の低待機時間ソリューションがあります。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-166">Partners will have an always-on, low-latency solution with the following features available:</span></span> 

- <span data-ttu-id="d1ba8-167">豊富な分析と予算のアラート</span><span class="sxs-lookup"><span data-stu-id="d1ba8-167">Richer analysis and budget alerting</span></span> 
- <span data-ttu-id="d1ba8-168">API と Power BI コネクタ</span><span class="sxs-lookup"><span data-stu-id="d1ba8-168">APIs and Power BI connectors</span></span> 
- <span data-ttu-id="d1ba8-169">マルチカスタマー ビュー</span><span class="sxs-lookup"><span data-stu-id="d1ba8-169">Multi-customer view</span></span> 
- <span data-ttu-id="d1ba8-170">無料の Azure コスト管理</span><span class="sxs-lookup"><span data-stu-id="d1ba8-170">Free to manage Azure costs</span></span> 
- <span data-ttu-id="d1ba8-171">ロール/ユーザーの拡張</span><span class="sxs-lookup"><span data-stu-id="d1ba8-171">Expansion of roles/users</span></span> 

<span data-ttu-id="d1ba8-172">2019 年 2 月にエンタープライズ契約で利用できるようになったこの機能の詳細については、[Azure Cost Management](https://azure.microsoft.com/services/cost-management) のページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-172">See [Azure cost management](https://azure.microsoft.com/services/cost-management) for more information on this feature, which became available for enterprise agreements in February, 2019.</span></span> <span data-ttu-id="d1ba8-173">これは、CSP の新しい Azure コマース エクスペリエンスの一部として購入された Azure サービスでのみ利用できます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-173">This is available only with Azure services purchased as part of this new Azure commerce experience in CSP.</span></span> 
 
## <a name="azure-spending"></a><span data-ttu-id="d1ba8-174">Azure 利用状況</span><span class="sxs-lookup"><span data-stu-id="d1ba8-174">Azure spending</span></span> 

<span data-ttu-id="d1ba8-175">Azure 利用状況ツールは、CSP の新しいコマース エクスペリエンス向けにパートナー センターで利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-175">An Azure spending tool will be available in Partner Center for the new commerce experience in CSP.</span></span> <span data-ttu-id="d1ba8-176">この機能を適用すると、パートナーは次のことを確認できます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-176">When applied, this capability will enable partners to see:</span></span>  

- <span data-ttu-id="d1ba8-177">顧客の総予算</span><span class="sxs-lookup"><span data-stu-id="d1ba8-177">Total budget on a customer</span></span> 
- <span data-ttu-id="d1ba8-178">既存の Azure プランの推定費用合計</span><span class="sxs-lookup"><span data-stu-id="d1ba8-178">Total estimated spending on an existing Azure plan</span></span> 
- <span data-ttu-id="d1ba8-179">各請求期間における顧客の使用率</span><span class="sxs-lookup"><span data-stu-id="d1ba8-179">Percentage of customers usage in each billing period</span></span> 

<span data-ttu-id="d1ba8-180">Azure プランを介した Azure サービスの請求モデルは後払い式の従量課金制なので、請求額が想定よりも多額にならないように、パートナーは毎月の予算を適用し、使用率を追跡することができます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-180">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated,partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="d1ba8-181">1 社の顧客または複数の顧客に一度に予算を適用できます。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-181">A budget can be applied to one customer or multiple customers at one time.</span></span> 

![Azure 利用状況](images/azure/azurespend.png)

<span data-ttu-id="d1ba8-183">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="d1ba8-183">**For more information**</span></span>

-  <span data-ttu-id="d1ba8-184">パートナー獲得クレジット (PEC) の計算方法は、パートナー センター ダッシュボードから使用できる価格表に記載されています。</span><span class="sxs-lookup"><span data-stu-id="d1ba8-184">How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center dashboard.</span></span> 
   
-  [<span data-ttu-id="d1ba8-185">Azure プランを購入する</span><span class="sxs-lookup"><span data-stu-id="d1ba8-185">Purchase the Azure plan</span></span>](purchase-azure-plan.md)

-  [<span data-ttu-id="d1ba8-186">CSP の新しいコマース エクスペリエンスの価格表</span><span class="sxs-lookup"><span data-stu-id="d1ba8-186">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)
