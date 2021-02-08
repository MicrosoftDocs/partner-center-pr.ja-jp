---
title: Azure プランの請求 - 請求書と調整ファイル
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure プランの請求に関連する請求書と調整ファイルの構造にアクセスして理解する方法について説明します。
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 819f90ca9a8467de4a8001a1b10f8409d3fb1b81
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/28/2021
ms.locfileid: "98924991"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="8b0cb-103">CSP の新しいコマース エクスペリエンス - Azure の請求</span><span class="sxs-lookup"><span data-stu-id="8b0cb-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="8b0cb-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="8b0cb-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8b0cb-105">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="8b0cb-105">Admin agent</span></span>
- <span data-ttu-id="8b0cb-106">課金管理者</span><span class="sxs-lookup"><span data-stu-id="8b0cb-106">Billing admin</span></span>
- <span data-ttu-id="8b0cb-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="8b0cb-107">Global admin</span></span>

<span data-ttu-id="8b0cb-108">この記事では、Azure プランの請求に関連する請求書と調整ファイルの構造にアクセスして理解する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-108">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="8b0cb-109">Azure プランの請求は、調整された 1 つの請求日とカレンダーの月単位の請求期間を使用することで、請求エクスペリエンスが簡単になりました。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-109">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="8b0cb-110">請求の要点の概要</span><span class="sxs-lookup"><span data-stu-id="8b0cb-110">Summary of billing essentials</span></span>

- <span data-ttu-id="8b0cb-111">**請求日**:請求書と調整ファイルは、パートナー センター ダッシュボード/API で 8 日 (UTC 時間の午前 0 時) までに取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="8b0cb-112">**請求書の請求期間**:請求書の請求期間は、10/1 から 10/31、11/1 から 11/30 のように、カレンダーの月に合わせて調整されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="8b0cb-113">**料金サービス期間**:料金はカレンダーの月に合わせて調整されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="8b0cb-114">たとえば、請求先パートナーが 10/15 に Azure プランを介して Azure サービスを追加し、顧客が 10/15 に Azure サービスの使用を開始した場合、請求先パートナーは、サービス期間 10/15 から 10/31 の顧客の使用量に対して、11/8 に請求書/調整を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="8b0cb-115">12/8 に生成される翌月の請求書には、サービス期間 11/1 から 11/31 のすべての料金が含まれます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-115">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="8b0cb-116">**請求書の支払い条件**:請求日から 60 日以内。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="8b0cb-117">**請求書の通貨**:2021 年 1 月 28 日以降、EU と EFTA および英国のリージョンのパートナーは、新規の顧客および 2020 年 5 月 11 日より前にテナントを作成した既存の CSP の顧客が初めて新しいコマース オファーを購入した場合、それらの購入についてはパートナーの場所の通貨で課金されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-117">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="8b0cb-118">EU と EFTA および英国リージョン以外のパートナーは、引き続きパートナーの場所の通貨で課金されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-118">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="8b0cb-119">**パートナー インセンティブ**:請求月の末日から 45 日以内に支払われます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="8b0cb-120">請求書および調整ファイルにアクセスする</span><span class="sxs-lookup"><span data-stu-id="8b0cb-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="8b0cb-121">請求書を表示できる状態になると、会社の全体管理者または請求管理者にはメールが送信されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="8b0cb-122">請求書および調整ファイルにアクセスするには:</span><span class="sxs-lookup"><span data-stu-id="8b0cb-122">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="8b0cb-123">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="8b0cb-124">パートナー センター メニューで **[請求]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="8b0cb-125">**定期的** および **1 回限り** と目的の通貨を示すタブを選択します。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="請求":::

4. <span data-ttu-id="8b0cb-127">**請求書** または **調整ファイル** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-127">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="8b0cb-128">過去の請求書および調整ファイルを表示するには、下の [請求履歴] 行を展開します。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-128">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="8b0cb-129">使用状況データについて</span><span class="sxs-lookup"><span data-stu-id="8b0cb-129">Understanding usage data</span></span> 

1. <span data-ttu-id="8b0cb-130">Azure プランは、使用状況に関するルートまたは最上位のコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="8b0cb-131">すべての使用状況は、1 つの Azure プランに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-131">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="8b0cb-132">プラン内には、1 つ以上の Azure サブスクリプションがあります。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="8b0cb-133">これらは、リソースの管理とデプロイに使用されるコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="8b0cb-134">サブスクリプション内では、リソース グループはグループ リソースに追加されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="8b0cb-135">すべてのリソースは 1 つのリソース グループにデプロイされます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="8b0cb-136">リソースの例としては、仮想マシンやストレージ アカウントなどがあります。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="8b0cb-137">リソース出力メーター: メーターはリソースの消費量の測定であり、1 つのリソースが複数のメーターの使用量を出力する場合があります。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="8b0cb-138">メーターは、ProductId、SKUId、および AvailabilityId によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="8b0cb-139">サブスクリプション リソース グループと使用状況測定の階層</span><span class="sxs-lookup"><span data-stu-id="8b0cb-139">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="8b0cb-140">**Azure アカウント (テナント)**</span><span class="sxs-lookup"><span data-stu-id="8b0cb-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="8b0cb-141">サブスクリプション A</span><span class="sxs-lookup"><span data-stu-id="8b0cb-141">Subscription A</span></span>
    - <span data-ttu-id="8b0cb-142">リソース グループ 1</span><span class="sxs-lookup"><span data-stu-id="8b0cb-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="8b0cb-143">仮想マシン (リソース)</span><span class="sxs-lookup"><span data-stu-id="8b0cb-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="8b0cb-144">コンピューティング メーター</span><span class="sxs-lookup"><span data-stu-id="8b0cb-144">Compute meter</span></span>
        - <span data-ttu-id="8b0cb-145">仮想ネットワーク (リソース)</span><span class="sxs-lookup"><span data-stu-id="8b0cb-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="8b0cb-146">課金メーターなし</span><span class="sxs-lookup"><span data-stu-id="8b0cb-146">No billing meter</span></span>

    - <span data-ttu-id="8b0cb-147">リソース グループ 2</span><span class="sxs-lookup"><span data-stu-id="8b0cb-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="8b0cb-148">仮想マシン (リソース)</span><span class="sxs-lookup"><span data-stu-id="8b0cb-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="8b0cb-149">コンピューター メーター</span><span class="sxs-lookup"><span data-stu-id="8b0cb-149">Computer meter</span></span>
        - <span data-ttu-id="8b0cb-150">Premium SSD マネージド ディスク (リソース)</span><span class="sxs-lookup"><span data-stu-id="8b0cb-150">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="8b0cb-151">ストレージ容量メーター</span><span class="sxs-lookup"><span data-stu-id="8b0cb-151">Storage capacity meter</span></span>
            - <span data-ttu-id="8b0cb-152">ストレージ操作メーター</span><span class="sxs-lookup"><span data-stu-id="8b0cb-152">Storage operations meter</span></span>

- <span data-ttu-id="8b0cb-153">サブスクリプション B   -リソース グループ 1       - Azure SQL (リソース)           - DTU メーター       - VPN ゲートウェイ (リソース)           - VPN ゲートウェイ メーター</span><span class="sxs-lookup"><span data-stu-id="8b0cb-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="8b0cb-154">リソース グループ 2</span><span class="sxs-lookup"><span data-stu-id="8b0cb-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="8b0cb-155">仮想ネットワーク インターフェイス (リソース)</span><span class="sxs-lookup"><span data-stu-id="8b0cb-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="8b0cb-156">課金メーターなし</span><span class="sxs-lookup"><span data-stu-id="8b0cb-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="8b0cb-157">請求書の読み方</span><span class="sxs-lookup"><span data-stu-id="8b0cb-157">Read the invoice</span></span>

1. <span data-ttu-id="8b0cb-158">請求書は、毎月 8 日までに取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-158">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="8b0cb-159">パートナーには、60 日後に支払われます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="8b0cb-160">請求期間は、10/1 から 10/31 など、カレンダーの 1 か月間が対象になります。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="8b0cb-161">料金に調整額は含まれていません (金額に "管理対象のサービスのパートナー獲得クレジット" は含まれていません)。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="8b0cb-162">請求の詳細については、請求書および調整ファイルと毎日評価される使用量ファイルを確認します。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="請求書":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="8b0cb-164">請求書と調整ファイルを読む</span><span class="sxs-lookup"><span data-stu-id="8b0cb-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="8b0cb-165">Azure プランとメーターの各組み合わせに対し、調整ファイルには最大で 2 行の請求明細が記載される場合があります。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="8b0cb-166">メーターが、カレンダーの 1 か月間を通して何らかの種類の割引またはクレジット (階層 1 の割引や管理対象サービスのパートナー獲得クレジットなど) の対象となる場合、調整ファイルには 1 行の請求明細のみが記載されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="8b0cb-167">**PriceAdjusmentDescription** 列では、割引または獲得クレジットが参照されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="8b0cb-168">特定のメーターに対して割引またはパートナー獲得クレジットの対象となるリソースがない場合、調整ファイルに記載される請求明細は 1 行のみであり、実効単価は小売価格 (つまり単価) になります。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="8b0cb-169">メーターまたはそのメーターを出力している任意のリソースが、1 か月間の一部について **マネージド サービスのパートナー獲得クレジット** の対象となる場合、調整ファイルには 2 行の請求明細が記載されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-169">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="8b0cb-170">1 行目はメーターが対象となる日数を表し、2 行目はメーターが対象とならない日数を表します。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="8b0cb-171">毎日の使用量ファイルの読み方</span><span class="sxs-lookup"><span data-stu-id="8b0cb-171">Read the daily usage file</span></span>

- <span data-ttu-id="8b0cb-172">Azure プランのサブスクリプション メーターは日単位で評価され、蓄積されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="8b0cb-173">**マネージド サービスのパートナー獲得クレジット** は、日単位で判断および適用されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="8b0cb-174">すべてのサブスクリプション メーターには、消費があった月の毎日の行があります。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="8b0cb-175">次の例があるとします。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-175">In the example below:</span></span>

  - <span data-ttu-id="8b0cb-176">メーターは、7/1 から 7/3 に **マネージド サービスのパートナー獲得クレジット** の対象となりました (実効単価は、小売価格からパートナー獲得クレジットを差し引いた額であることに注意してください)。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-176">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="8b0cb-177">メーターは、7/4 から 7/7 に **マネージド サービスのパートナー獲得クレジット** の対象となりませんでした (実効単価は小売価格であることに注意してください)。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-177">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="8b0cb-178">メーターは、7/8 から 7/31 に **マネージド サービスのパートナー獲得クレジット** の対象となりました (実効単価は、小売価格からパートナー獲得クレジットを差し引いた額であることに注意してください)。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-178">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="8b0cb-180">顧客の通貨での請求書</span><span class="sxs-lookup"><span data-stu-id="8b0cb-180">Invoice in customer currency</span></span>

<span data-ttu-id="8b0cb-181">Azure プランを介した Azure サービスには、米国ドルで価格が設定され、顧客の国の割り当て通貨で請求されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="8b0cb-182">請求通貨が米国ドル以外の場合は、使用された外国為替 (FX) レートが請求書の最後のページに記載されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="8b0cb-183">外国為替レートは月ごとに決定され、次の請求書に適用されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="8b0cb-184">国の通貨の詳細な一覧については、[新しいコマース オファーの提供国と顧客の通貨の対応表](https://go.microsoft.com/fwlink/?linkid=2112354)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-184">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="8b0cb-185">Microsoft はロンドン証券取引所に従って換算を行います。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-185">Microsoft follows the London Stock Exchange for conversion.</span></span> <span data-ttu-id="8b0cb-186">使用される為替レートは、ロンドン証券取引所でその月の最終営業日の最後の 1 秒間に取得された為替レートに相当します。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-186">We use the exchange rate, which is equal to the exchange rate captured on the last second of the last business day of the month on the London Stock Exchange.</span></span> <span data-ttu-id="8b0cb-187">外国為替レートは、適用される月の最初の日の前に更新され、使用されます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-187">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="8b0cb-188">Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="8b0cb-188">Azure reservations</span></span>


<span data-ttu-id="8b0cb-189">Azure プランを通じて [Azure の予約](azure-reservations.md)を購入する場合は、1 回限りまたは毎月の請求を選択できます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-189">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="8b0cb-190">Azure 利用状況</span><span class="sxs-lookup"><span data-stu-id="8b0cb-190">Azure spending</span></span>

<span data-ttu-id="8b0cb-191">Azure の既存の利用状況エクスペリエンスは、パートナー センターでの新しい Azure プラン課金をサポートするように更新されています。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-191">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="8b0cb-192">これにより、パートナーは次のことができます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-192">This enables partners to:</span></span>

- <span data-ttu-id="8b0cb-193">顧客レベルで設定された予算のアラートを表示し、管理し、受け取る</span><span class="sxs-lookup"><span data-stu-id="8b0cb-193">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="8b0cb-194">Azure プランの推定支出の合計を表示する (リソースおよびメーターのレベルで分類)</span><span class="sxs-lookup"><span data-stu-id="8b0cb-194">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="8b0cb-195">Azure プランを介した Azure サービスの請求モデルは後払い式の従量課金制なので、請求額が想定よりも多額にならないように、パートナーは毎月の予算を適用し、使用率を追跡することができます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-195">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="8b0cb-196">1 社の顧客または複数の顧客に一度に予算を適用できます。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-196">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure 利用状況":::

## <a name="next-steps"></a><span data-ttu-id="8b0cb-198">次のステップ</span><span class="sxs-lookup"><span data-stu-id="8b0cb-198">Next steps</span></span>

- <span data-ttu-id="8b0cb-199">パートナー獲得クレジット (PEC) の計算方法を参照する。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-199">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="8b0cb-200">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard/)にサインインし、利用可能な価格表を見つける。</span><span class="sxs-lookup"><span data-stu-id="8b0cb-200">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="8b0cb-201">[Azure プランの購入方法](purchase-azure-plan.md)を参照する</span><span class="sxs-lookup"><span data-stu-id="8b0cb-201">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="8b0cb-202">[CSP の新しいコマース エクスペリエンスの価格表](azure-plan-price-list.md)を参照する</span><span class="sxs-lookup"><span data-stu-id="8b0cb-202">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
