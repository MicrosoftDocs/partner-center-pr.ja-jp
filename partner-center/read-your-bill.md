---
title: 請求書 & 偵察ファイルを読み取る方法
ms.topic: article
ms.date: 06/05/2020
description: 請求書 & 調整ファイルについて説明します。 請求書には、その月の期間におけるプログラム、製品、および顧客に対するパートナーセンターの料金が表示されます。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4b91b2f9580d9c369e7a267c2b413db8a4a6300d
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436631"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a><span data-ttu-id="2ab16-104">請求書と調整ファイルを理解する-パートナーセンターでそれらを検索する方法について説明します</span><span class="sxs-lookup"><span data-stu-id="2ab16-104">Understand your bill and reconciliation file - learn how to find them in Partner Center</span></span>

<span data-ttu-id="2ab16-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="2ab16-105">**Applies to**</span></span>

- <span data-ttu-id="2ab16-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="2ab16-106">Partner Center</span></span>
- <span data-ttu-id="2ab16-107">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="2ab16-107">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="2ab16-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="2ab16-108">**Appropriate roles**</span></span>

- <span data-ttu-id="2ab16-109">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="2ab16-109">Global admin</span></span>
- <span data-ttu-id="2ab16-110">課金管理者</span><span class="sxs-lookup"><span data-stu-id="2ab16-110">Billing admin</span></span>
- <span data-ttu-id="2ab16-111">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="2ab16-111">Admin agent</span></span>


<span data-ttu-id="2ab16-112">**請求書**は、**すべてのパートナーセンターの請求**(プログラム全体、すべての製品、およびすべての顧客) の概要です。</span><span class="sxs-lookup"><span data-stu-id="2ab16-112">Your **invoice** is a **summary of all your Partner Center charges** (across the program, all products, and all customers).</span></span> 

## <a name="invoice-types"></a><span data-ttu-id="2ab16-113">請求書の種類</span><span class="sxs-lookup"><span data-stu-id="2ab16-113">Invoice types</span></span>

<span data-ttu-id="2ab16-114">Microsoft は、ライセンスベースの料金 (Office 365 など) と使用量ベースの料金 (Azure など) に対して1つの請求書を発行し、1回限りの料金 (Azure RI、Marketplace、Azure plan など) に対して別の請求書を発行します。</span><span class="sxs-lookup"><span data-stu-id="2ab16-114">Microsoft will issue one invoice for any license-based charges (such as Office 365) and usage-based charges (such as Azure) and a separate invoice for one-time charges (such as Azure RI, Marketplace, or Azure plan).</span></span>

<span data-ttu-id="2ab16-115">たとえば、次のように入力します。</span><span class="sxs-lookup"><span data-stu-id="2ab16-115">For example,</span></span>  

<span data-ttu-id="2ab16-116">**シナリオ 1 [Single Currency]**: パートナーは145P プランと O365 ライセンスを購入しています。</span><span class="sxs-lookup"><span data-stu-id="2ab16-116">**Scenario 1 [Single Currency]**: Partner has purchases for 145P offer and O365 licenses,</span></span>  

- <span data-ttu-id="2ab16-117">パートナーは、O365 と Azure (145p) の両方の料金をカバーする1つの請求書 PDF と2つの調整ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="2ab16-117">Partner will get one invoice PDF and 2 reconciliation files covering the charges for both O365 and Azure (145p).</span></span>  

<span data-ttu-id="2ab16-118">**シナリオ 2 [Single Currency]**: パートナーは、145p 購入と共に、azure RI、Marketplace、または azure プランを購入しています。</span><span class="sxs-lookup"><span data-stu-id="2ab16-118">**Scenario 2 [Single Currency]**: Partner has purchases for Azure RI, Marketplace and/or Azure plan along with 145p purchases.</span></span>

- <span data-ttu-id="2ab16-119">パートナーは、1つの請求書 PDF と、Azure の料金 (145p) をカバーする調整ファイルを取得します。</span><span class="sxs-lookup"><span data-stu-id="2ab16-119">Partner will get one invoice PDF and a reconciliation file covering the charges for Azure (145p).</span></span> 

- <span data-ttu-id="2ab16-120">パートナーは、Azure RI、Marketplace、Azure プランの料金をカバーする別の請求書 PDF と調整ファイルを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="2ab16-120">Partner will receive another invoice PDF and a reconciliation file covering their charges for Azure RI, Marketplace, Azure plan.</span></span> 

<span data-ttu-id="2ab16-121">**シナリオ 3 [マルチ通貨]**: パートナーが、eur での DKK および azure プランの azure RI と、eur で145p の購入を購入したとします。</span><span class="sxs-lookup"><span data-stu-id="2ab16-121">**Scenario 3 [Multi-Currency]**: Partner has purchases for Azure RI in DKK and Azure plan in EUR along with 145p purchases in EUR.</span></span>

- <span data-ttu-id="2ab16-122">パートナーは、1つの請求書 PDF と、DKK における Azure RI の料金をカバーする調整ファイルを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="2ab16-122">Partner will receive one invoice PDF and a reconciliation file covering the charges for Azure RI in DKK.</span></span> 

- <span data-ttu-id="2ab16-123">パートナーは、1つの請求書 PDF と、EUR での Azure プランの料金をカバーする調整ファイルを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="2ab16-123">Partner will receive one invoice PDF and a reconciliation file covering the charges for Azure plan in EUR.</span></span> 

- <span data-ttu-id="2ab16-124">パートナーは、EUR (またはパートナー請求通貨) で145p プランの料金をカバーする別の請求書 PDF と調整ファイルを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="2ab16-124">Partner will receive another invoice PDF and a reconciliation file covering their charges for 145p offer in EUR (or partner billing currency).</span></span> 

## <a name="find-your-bill"></a><span data-ttu-id="2ab16-125">請求書の検索</span><span class="sxs-lookup"><span data-stu-id="2ab16-125">Find your bill</span></span> 

<span data-ttu-id="2ab16-126">請求書は、パートナーセンターのダッシュボードの [課金] ページで確認できます。</span><span class="sxs-lookup"><span data-stu-id="2ab16-126">You can find your invoice on the Billing page of the dashboard in Partner Center.</span></span> <span data-ttu-id="2ab16-127">このページでは、請求履歴、支出傾向、および調整ファイルを見つけることもできます。</span><span class="sxs-lookup"><span data-stu-id="2ab16-127">You can also find your billing history, spending trends, and reconciliation files on this page.</span></span> 

1. <span data-ttu-id="2ab16-128">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="2ab16-128">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span> 

2. <span data-ttu-id="2ab16-129">左側のメニューで、[ **課金**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="2ab16-129">In the left-hand menu, select **Billing**.</span></span> 

3. <span data-ttu-id="2ab16-130">[課金] ページで、ダウンロードする請求書を選択します。</span><span class="sxs-lookup"><span data-stu-id="2ab16-130">On the Billing page, select the invoice you want to download.</span></span> 

<span data-ttu-id="2ab16-131">最新の請求書へのリンクについては、最後の請求日の時点で、[アカウントの残高] の下に表示されます。</span><span class="sxs-lookup"><span data-stu-id="2ab16-131">You can find a link to your latest invoice at the top of the page under Account balance as of last invoice date.</span></span> 

<span data-ttu-id="2ab16-132">以前の請求書は、[請求履歴] セクションで確認できます。</span><span class="sxs-lookup"><span data-stu-id="2ab16-132">You can find previous invoices in the Billing history section.</span></span> <span data-ttu-id="2ab16-133">適切な年を選択し、適切な請求期間の横にあるドロップダウン矢印を選択します。</span><span class="sxs-lookup"><span data-stu-id="2ab16-133">Choose the appropriate year, then select the drop-down arrow next to the appropriate Billing period.</span></span> <span data-ttu-id="2ab16-134">請求書 (.pdf) の横にあるリンクを選択して、その期間の請求書をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="2ab16-134">Select the link next to Invoices (.pdf) to download that period's invoice.</span></span> 

## <a name="understanding-invoice-pdf"></a><span data-ttu-id="2ab16-135">請求書の PDF について</span><span class="sxs-lookup"><span data-stu-id="2ab16-135">Understanding invoice PDF</span></span> 

<span data-ttu-id="2ab16-136">**使用量とライセンスに基づく請求書**: Office 365 や Azure などのサービスに対する請求書は、選択した請求日の2日以内に利用可能になります [UTC]。</span><span class="sxs-lookup"><span data-stu-id="2ab16-136">**Invoices for Usage and license-based charges**: Invoices for charges for services such as Office 365 and Azure will be available within two (2) days of your selected billing date [UTC].</span></span>  

<span data-ttu-id="2ab16-137">**Onetime の請求書と定期的な料金**: azure RI、azure Plan、Marketplace などのサービスの請求書は、毎月8日以降にご利用いただけます。</span><span class="sxs-lookup"><span data-stu-id="2ab16-137">**Invoices for onetime and recurring charges**: Invoices for charges for services such as Azure RI, Azure plan, Marketplace will be available not later than 8th of every month.</span></span>  

<span data-ttu-id="2ab16-138">Invoice PDF ドキュメントの主なフィールドの一部を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2ab16-138">Below are some of the key fields on the Invoice PDF document –</span></span>

<span data-ttu-id="2ab16-139">**請求書番号**: それぞれの請求期間に対して生成された請求書ドキュメントの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="2ab16-139">**Invoice number**: Unique identifier for the invoice document generated for the respective billing period.</span></span> 

<span data-ttu-id="2ab16-140">**請求期間**: 使用状況とライセンスベースのサービスがある期間です。</span><span class="sxs-lookup"><span data-stu-id="2ab16-140">**Billing period**: This is the period during which you have usages and license-based services.</span></span> 

<span data-ttu-id="2ab16-141">**請求日**: 請求書が毎月生成される請求日または記念日。</span><span class="sxs-lookup"><span data-stu-id="2ab16-141">**Invoice date**: The billing date or anniversary date on which your invoice is generated each month.</span></span> 

<span data-ttu-id="2ab16-142">**支払い期日**: 支払いを受け取る必要がある日付。</span><span class="sxs-lookup"><span data-stu-id="2ab16-142">**Payment due date**: The date by which your payment must be received.</span></span> 

<span data-ttu-id="2ab16-143">**料金**: それぞれの請求期間における請求通貨の金額。</span><span class="sxs-lookup"><span data-stu-id="2ab16-143">**Charges**: The amount due in your billing currency for the respective billing period.</span></span> 

<span data-ttu-id="2ab16-144">**クレジット**: クレジット (SLA など) またはサブスクリプションに対して行われた変更の調整 (接続クライアント数の増加や減少など)。</span><span class="sxs-lookup"><span data-stu-id="2ab16-144">**Credits**: Credits (such as SLA) or adjustments for changes made to subscriptions (for example, seat increases or decreases).</span></span> 

<span data-ttu-id="2ab16-145">**お支払い**方法: お客様の地域に基づいて請求書を支払う方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="2ab16-145">**Payment instructions**: Description of how to pay your invoice, based on your region.</span></span> <span data-ttu-id="2ab16-146">支払いを行う場合は、常に請求書番号を含めてください。</span><span class="sxs-lookup"><span data-stu-id="2ab16-146">Always be sure to include your invoice number when making a payment.</span></span> 

<span data-ttu-id="2ab16-147">請求書ファイル内のすべてのフィールド (1 回限りの料金のフィールドを含む) の詳細については、「 [請求書ファイルのフィールド](invoice-file.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ab16-147">For a detailed description of all the fields in your invoice file (including fields for one-time charges), see [Invoice file fields](invoice-file.md).</span></span> 

## <a name="understand-reconciliation-files"></a><span data-ttu-id="2ab16-148">調整ファイルについて</span><span class="sxs-lookup"><span data-stu-id="2ab16-148">Understand reconciliation files</span></span>

 <span data-ttu-id="2ab16-149">調整ファイルは、料金のドリルダウン/明細項目の詳細を提供し、請求書 PDF と共にダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="2ab16-149">Reconciliation files, which provides a drill down/itemized details of your charges, are available to download along with the Invoice PDF.</span></span> <span data-ttu-id="2ab16-150">調整ファイルには、顧客の請求書の作成に使用できる顧客 id とサブスクリプション id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2ab16-150">The reconciliation files include customer identifiers and subscription identifiers that you can use to create customer invoices.</span></span> <span data-ttu-id="2ab16-151">偵察ファイルの詳細については [、「調整ファイルの使用方法](use-the-reconciliation-files.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ab16-151">Please refer to  [How to use the reconciliation files](use-the-reconciliation-files.md) to get more details on the recon files.</span></span> 
