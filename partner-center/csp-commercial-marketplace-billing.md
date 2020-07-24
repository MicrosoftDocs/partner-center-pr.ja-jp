---
title: 商用 marketplace 製品の課金
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンター内の商用マーケットプレースから購入した ISV SaaS 製品またはサブスクリプションの課金のしくみについて説明します。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f5c506e1f3dd5e1ffcac1d7017687b1b36718745
ms.sourcegitcommit: 37562b0e29ab921b6b454bb9801376f1feedb715
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/22/2020
ms.locfileid: "86943476"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a><span data-ttu-id="5de47-103">パートナーセンターでの商用 marketplace 製品とサブスクリプションの課金</span><span class="sxs-lookup"><span data-stu-id="5de47-103">Billing for commercial marketplace products and subscriptions in Partner Center</span></span>

<span data-ttu-id="5de47-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="5de47-104">**Applies to**</span></span>

- <span data-ttu-id="5de47-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="5de47-105">Partner Center</span></span>
- <span data-ttu-id="5de47-106">CSP プログラムのパートナー</span><span class="sxs-lookup"><span data-stu-id="5de47-106">Partners in the CSP program</span></span>

<span data-ttu-id="5de47-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="5de47-107">**Appropriate roles**</span></span>

- <span data-ttu-id="5de47-108">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="5de47-108">Global admin</span></span>
- <span data-ttu-id="5de47-109">課金管理者</span><span class="sxs-lookup"><span data-stu-id="5de47-109">Billing admin</span></span>

<span data-ttu-id="5de47-110">CSP プログラムのパートナーとして、パートナーセンターを使用して、商用マーケットプレースの ISV 発行元からライセンスベースの SaaS 製品を購入できます。</span><span class="sxs-lookup"><span data-stu-id="5de47-110">As a partner in the CSP program, you can use Partner Center to purchase license-based SaaS products from ISV publishers in the commercial marketplace.</span></span> <span data-ttu-id="5de47-111">その後、これらの種類の購入に関する請求書にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="5de47-111">After you do so, you can access a bill for these types of purchases.</span></span> <span data-ttu-id="5de47-112">請求期間はカレンダー月の最初の日から開始され、カレンダー月の最後の日に終了します。</span><span class="sxs-lookup"><span data-stu-id="5de47-112">The billing period starts on the first day of the calendar month and ends on the last day of the calendar month.</span></span> <span data-ttu-id="5de47-113">請求書は、次の月の8日に利用可能になります。</span><span class="sxs-lookup"><span data-stu-id="5de47-113">Invoices are made available on the 8th day of the following month.</span></span>

<span data-ttu-id="5de47-114">請求書には、パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard/)から、または[パートナーセンター api](https://docs.microsoft.com/partner-center/develop/)を使用してアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="5de47-114">You can access invoices from either the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) or by using [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/).</span></span>

<span data-ttu-id="5de47-115">CSP プログラムのパートナーは、パートナーセンターまたは Azure portal (お客様が以前に購入した CSP に購入した Azure テナントを使用) から製品を購入した場合に、お客様が購入した ISV 商用 marketplace ソリューションに対して課金されます。</span><span class="sxs-lookup"><span data-stu-id="5de47-115">Partners in the CSP program are billed for ISV commercial marketplace solutions purchased for a customer when they purchase those products from either Partner Center or from the Azure portal (using the customer's prior, CSP-purchased Azure tenant).</span></span>

>[!NOTE]
><span data-ttu-id="5de47-116">お客様が独自の Azure AD テナント (CSP プログラムのパートナーから購入したものではない) を使用している場合、お客様は独自の ISV SaaS ソリューションを ([Microsoft AppSource](https://appsource.microsoft.com/)または[Azure Marketplace](https://azuremarketplace.microsoft.com/)) から直接購入することもできます。</span><span class="sxs-lookup"><span data-stu-id="5de47-116">If customers use their own Azure AD tenant (not one purchased from a partner in the CSP program), customers can also choose to purchase their own ISV SaaS solution directly from ([Microsoft AppSource](https://appsource.microsoft.com/) or [Azure Marketplace](https://azuremarketplace.microsoft.com/)).</span></span> <span data-ttu-id="5de47-117">その場合は、Microsoft から直接請求書を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="5de47-117">If they do so, they will receive their own bill directly from Microsoft.</span></span> <span data-ttu-id="5de47-118">同様に、CSP プログラムのパートナーが Azure サブスクリプションまたは新しい Azure プランを顧客に販売し、そのテナントへの[ロールベースのアクセス権](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles)を顧客 (または間接**リセラー) に**付与した場合、その顧客 (または間接リセラー) は、事前の承認または CSP パートナーへの通知を行わずに、商用の marketplace プランを購入できます。</span><span class="sxs-lookup"><span data-stu-id="5de47-118">Likewise, if a partner in the CSP program sells an Azure subscription or the new Azure plan to the customer and grants the customer (or indirect reseller) [role-based access](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles) to that tenant (assigning any role to the customer besides **Reader**), that customer (or indirect reseller) can also purchase commercial marketplace offers without prior approval or notification to the CSP partner.</span></span> <span data-ttu-id="5de47-119">このような場合、マイクロソフトは、顧客が行った購入について、CSP プログラムに直接パートナーに通知しません。</span><span class="sxs-lookup"><span data-stu-id="5de47-119">In these cases, Microsoft will not directly notify partners in the CSP program about purchases made by their customers.</span></span> <span data-ttu-id="5de47-120">ただし、Microsoft では、Azure サブスクリプションでのアクティビティに関するアラートまたは通知を設定するために使用できるオプションの[Azure Monitor](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log)メカニズムを提供しています。</span><span class="sxs-lookup"><span data-stu-id="5de47-120">However, Microsoft does offer an optional [Azure Monitor](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) mechanism that you can use to set alerts or notifications about activity on an Azure subscription.</span></span>

## <a name="access-billing-information-for-commercial-marketplace-products"></a><span data-ttu-id="5de47-121">商用 marketplace 製品の課金情報へのアクセス</span><span class="sxs-lookup"><span data-stu-id="5de47-121">Access billing information for commercial marketplace products</span></span>

<span data-ttu-id="5de47-122">請求書を表示できる状態になると、会社の全体管理者または請求管理者にはメールが送信されます。</span><span class="sxs-lookup"><span data-stu-id="5de47-122">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> <span data-ttu-id="5de47-123">市販の marketplace 製品を購入するための最新の請求書と調整ファイルにアクセスするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="5de47-123">To access the latest invoice and reconciliation file for commercial marketplace product purchases:</span></span>

1. <span data-ttu-id="5de47-124">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="5de47-124">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="5de47-125">パートナー センター メニューで **[請求]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="5de47-125">From the Partner Center menu, select **Billing**.</span></span> 

    <span data-ttu-id="5de47-126">課金ページの上部に2つのタブが表示されます。**定期的**および**定期的な購入と1回限りの購入**です。</span><span class="sxs-lookup"><span data-stu-id="5de47-126">You will see two tabs at the top of the Billing page: **Recurring** and **Recurring and one-time purchases**.</span></span> <span data-ttu-id="5de47-127">各タブでは、さまざまな marketplace 製品の請求書と調整 (recon) ファイルにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="5de47-127">Each tab lets you access invoice and reconciliation (recon) files for different marketplace products:</span></span>

    - <span data-ttu-id="5de47-128">[**定期的**なタブ]: Office 365、Microsoft 365、Dynamics 365、Azure Active Directory、Power BI Pro、および Microsoft Azure に関連するサブスクリプションの請求書と調整ファイルを表示します。</span><span class="sxs-lookup"><span data-stu-id="5de47-128">**Recurring** tab: Shows invoice and reconciliation files for subscriptions related to Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro, and Microsoft Azure.</span></span>

    - <span data-ttu-id="5de47-129">[**定期的および1回限りの購入**] タブ: azure プラン、azure 予約、ソフトウェア、および商用 marketplace 製品の請求書と調整ファイルが表示されます。</span><span class="sxs-lookup"><span data-stu-id="5de47-129">**Recurring and one-time purchases** tab: Shows invoice and reconciliation files for Azure plan, Azure reservations, software and commercial marketplace products.</span></span>
  
3. <span data-ttu-id="5de47-130">[**定期的な購入と1回限りの購入**] タブを選択します。異なる通貨で顧客のサブスクリプションを購入した場合は、通貨ごとにタブが表示されます。</span><span class="sxs-lookup"><span data-stu-id="5de47-130">Select the **Recurring and one-time purchases** tab. If you purchased subscriptions for a customer in a different currency, you will see a tab for each currency.</span></span> <span data-ttu-id="5de47-131">このページでは、次のような操作を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="5de47-131">You can do a few things fr:om this page:</span></span>

    - <span data-ttu-id="5de47-132">最新の請求書と調整ファイルを表示するには、[**請求書**] または [**調整ファイル**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="5de47-132">To see the latest invoice and reconciliation file, select **Invoice** or **Reconciliation file**.</span></span> <span data-ttu-id="5de47-133">(必要に応じて、[パートナーセンター api](https://docs.microsoft.com/partner-center/develop/)を使用して、最新の請求書にアクセスし、ファイルデータにアクセスすることもできます。</span><span class="sxs-lookup"><span data-stu-id="5de47-133">(If you wanted to, you can also access the latest invoice and recon file data using [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/).</span></span>

    - <span data-ttu-id="5de47-134">以前の請求書とファイルを表示するには、下の [**請求履歴**] 行を展開します。</span><span class="sxs-lookup"><span data-stu-id="5de47-134">To see earlier invoices and recon files, expand the **Billing history** row below.</span></span>

    - <span data-ttu-id="5de47-135">最新のアカウント活動に基づいて、いつでもアカウントの残高や請求金額を確認するには、[**推定**] 見出しの下のリンクを選択します。</span><span class="sxs-lookup"><span data-stu-id="5de47-135">To check your estimated account balance or bill at any time based on the latest account activity, select a link under the **Estimates** heading.</span></span>  

    >[!NOTE]
    > <span data-ttu-id="5de47-136">月の8日目に請求書を投稿すると、税金とその他の適用可能な料金およびクレジットが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5de47-136">When we post your bill on the 8th day of the month, it will include taxes and any other applicable charges and credits.</span></span> <span data-ttu-id="5de47-137">これは、請求期間中に発生した最終的な金額と異なる場合があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="5de47-137">This means the final amount due might differ from what you see during the billing period.</span></span>

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a><span data-ttu-id="5de47-138">請求書と、商用 marketplace 製品のファイルに関する詳細</span><span class="sxs-lookup"><span data-stu-id="5de47-138">More about invoices and recon files for commercial marketplace products</span></span>

<span data-ttu-id="5de47-139">このセクションでは、サードパーティの ISV 発行元の顧客向けに購入した商用 marketplace SaaS サブスクリプションの請求書と調整ファイルの詳細について説明します。</span><span class="sxs-lookup"><span data-stu-id="5de47-139">This section offers more information about invoice and reconciliation files for commercial marketplace SaaS subscriptions purchased for customers from third-party ISV publishers.</span></span>

<span data-ttu-id="5de47-140">[パートナーセンター] メニューの [**課金**] オプションから [**定期的かつ1回限りの購入**] を選択すると、Microsoft (ファーストパーティ) と ISV (サードパーティ) の購入に関連する請求書と調整ファイルにアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="5de47-140">When you select **Recurring and one-time purchases** from the **Billing** option in the Partner Center menu, you gain access to invoices and reconciliation files for charges related to both Microsoft (first-party) and ISV (third-party) purchases.</span></span> <span data-ttu-id="5de47-141">これらの購入には、次のものが関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="5de47-141">These purchases may be associated with:</span></span>

- <span data-ttu-id="5de47-142">SaaS サブスクリプション (Microsoft または ISV 発行元のいずれか)</span><span class="sxs-lookup"><span data-stu-id="5de47-142">SaaS subscriptions (from either Microsoft or ISV publishers)</span></span>

- <span data-ttu-id="5de47-143">Azure プラン</span><span class="sxs-lookup"><span data-stu-id="5de47-143">Azure plan</span></span>

- <span data-ttu-id="5de47-144">Azure の予約</span><span class="sxs-lookup"><span data-stu-id="5de47-144">Azure reservations</span></span>

- <span data-ttu-id="5de47-145">その他のサブスクリプションベースのソフトウェア (Microsoft または ISV 発行元のいずれか)</span><span class="sxs-lookup"><span data-stu-id="5de47-145">Other subscription-based software (from either Microsoft or ISV publishers)</span></span>

<span data-ttu-id="5de47-146">これらの購入の例には、SUSE Linux ソフトウェア (ソフトウェアサブスクリプション) や Azure ISV SaaS 製品サブスクリプションなどがあります。</span><span class="sxs-lookup"><span data-stu-id="5de47-146">Examples of these purchases might include SUSE Linux software (a software subscription) or an Azure ISV SaaS product subscription.</span></span>

>[!NOTE]
> <span data-ttu-id="5de47-147">請求書とファイルへの登録方法の詳細については、「[課金の概要](billing.md)」も参照してください。</span><span class="sxs-lookup"><span data-stu-id="5de47-147">For more information about how to read invoice and recon files, see also [Billing overview](billing.md).</span></span>

### <a name="tips-on-reading-your-invoice"></a><span data-ttu-id="5de47-148">請求書の読み取りに関するヒント</span><span class="sxs-lookup"><span data-stu-id="5de47-148">Tips on reading your invoice</span></span>

<span data-ttu-id="5de47-149">サードパーティの ISV 発行元からライセンスベースの SaaS 製品を購入した場合は、請求書の料金のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="5de47-149">When you purchase a license-based SaaS product from a third-party ISV publisher, you will only see charges for the license fee on your invoice.</span></span> <span data-ttu-id="5de47-150">これは、ISV の SaaS 製品が基になる Azure インフラストラクチャリソースを使用 (または消費) する場合にも当てはまります。</span><span class="sxs-lookup"><span data-stu-id="5de47-150">This is true even when the ISV's SaaS product uses (or consumes) underlying Azure infrastructure resources.</span></span> <span data-ttu-id="5de47-151">これは、ISV の SaaS 製品に対するお客様の Azure インフラストラクチャの使用料金は、ISV に直接請求されるためです。</span><span class="sxs-lookup"><span data-stu-id="5de47-151">That is because your customer's Azure infrastructure usage charges for an ISV's SaaS product are billed directly to the ISV.</span></span> <span data-ttu-id="5de47-152">(Isv には、関連付けられている Azure 従量課金料金が、Azure の使用量に関する毎日評価される請求書調整ファイルとして表示されます)。</span><span class="sxs-lookup"><span data-stu-id="5de47-152">(ISVs will see associated Azure consumption charges in their own Azure usage daily-rated invoice reconciliation file.)</span></span>

<span data-ttu-id="5de47-153">請求書にはいくつかのページが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5de47-153">Your invoice will contain several pages:</span></span>

- <span data-ttu-id="5de47-154">**請求書のページ 1:** CSP プログラムパートナーの請求の詳細について概要を説明します。</span><span class="sxs-lookup"><span data-stu-id="5de47-154">**Page 1 of the invoice:** Contains a summary overview of the CSP program partner's billing details.</span></span> <span data-ttu-id="5de47-155">これには、請求期間、請求書番号、支払い条件 (Net 60 日)、請求書による支払い方法 (ネットワークまたはチェックによる支払い) の料金の概要が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5de47-155">This includes a summary of charges for the billing period, an invoice number, payment terms (Net 60 days), and billing payment methods to pay by wire or by check.</span></span>

- <span data-ttu-id="5de47-156">**請求書のページ 2 (およびそれ以降のページ):** ファーストパーティの Microsoft 購入とサードパーティの ISV (ライセンスベース) の購入の両方について、商用 marketplace からの料金を詳細に説明します。</span><span class="sxs-lookup"><span data-stu-id="5de47-156">**Page 2 (and any subsequent pages) of the invoice:** Details charges for both first-party Microsoft purchases and third-party ISV (license-based) purchases from the commercial marketplace.</span></span> <span data-ttu-id="5de47-157">ISV ライセンスベースの購入は、各製品名の下の**発行元**の行で特定できます。</span><span class="sxs-lookup"><span data-stu-id="5de47-157">You can identify ISV license-based purchases by the **Publisher** line beneath each product name.</span></span> <span data-ttu-id="5de47-158">関連する調整ファイルは、特定の請求書の請求についての詳細な課金を提供します。</span><span class="sxs-lookup"><span data-stu-id="5de47-158">The associated reconciliation file offers more billing details for specific invoice charges.</span></span>

- <span data-ttu-id="5de47-159">**請求書の最終ページ:** ISV からライセンスベースの marketplace 製品に対して課金された場合、この最終ページには、ISV 発行元の名前とアドレスに関する詳細が表示されます。</span><span class="sxs-lookup"><span data-stu-id="5de47-159">**Final page of the invoice:** If you were charged for license-based marketplace products from an ISV, this final page will display more details about the ISV publisher's name and address.</span></span>

### <a name="tips-on-reading-your-reconciliation-file"></a><span data-ttu-id="5de47-160">調整ファイルの読み取りに関するヒント</span><span class="sxs-lookup"><span data-stu-id="5de47-160">Tips on reading your reconciliation file</span></span>

<span data-ttu-id="5de47-161">**定期的および1回限りの購入**調整ファイルには、請求書の料金に対応する追加の詳細を含むいくつかの列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5de47-161">The **Recurring and one-time purchases** reconciliation file contains several columns with additional details that map to the charges in your invoice.</span></span> <span data-ttu-id="5de47-162">**Publishername**列には、Microsoft またはサードパーティの ISV 発行元からの購入であるかどうかが表示されます。</span><span class="sxs-lookup"><span data-stu-id="5de47-162">The **PublisherName** column shows whether the purchase is from Microsoft or a third-party ISV publisher.</span></span>

<span data-ttu-id="5de47-163">調整ファイルの料金には、$0 という料金が表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="5de47-163">Some charges in your reconciliation file may appear with a cost of $0.</span></span> <span data-ttu-id="5de47-164">これは、ISV の "無料試用版" プラン (通常は30日または60日) または「ライセンスの持ち込み」プランが原因である可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5de47-164">This may be due to an ISV "free trial" offer (usually 30 or 60 days) or a Bring Your Own License offer.</span></span>

<span data-ttu-id="5de47-165">無料試用版 ISV の場合は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="5de47-165">In the case of free trial ISV offers:</span></span>

- <span data-ttu-id="5de47-166">無料試用期間は、その期間における ISV のライセンスベースの SaaS 製品のコストを対象としています。</span><span class="sxs-lookup"><span data-stu-id="5de47-166">The free trial period covers the cost of the ISV's license-based SaaS product during that time.</span></span> <span data-ttu-id="5de47-167">また、関連付けられている Azure インフラストラクチャによるその SaaS 製品の使用に対して課金されることもありません。</span><span class="sxs-lookup"><span data-stu-id="5de47-167">You will also not be charged for associated Azure infrastructure use of that SaaS product.</span></span>  <span data-ttu-id="5de47-168">ただし、使用量ベースの ISV プランを使用している場合、無料試用版には、基になる Azure インフラストラクチャの使用コストは含まれません。</span><span class="sxs-lookup"><span data-stu-id="5de47-168">If you are using a usage-based ISV offer, however, the free trial does not include the cost of underlying Azure infrastructure usage.</span></span> <span data-ttu-id="5de47-169">この場合、Azure インフラストラクチャの使用量の料金は、別の Azure 調整ファイルに表示されます。</span><span class="sxs-lookup"><span data-stu-id="5de47-169">In this case, Azure infrastructure usage charges will appear in a separate Azure reconciliation file.</span></span>

- <span data-ttu-id="5de47-170">お客様に対して ISV の無料試用対象製品を購入して展開すると、お客様は ISV 発行元によって無料試用版に自動的に登録されます。</span><span class="sxs-lookup"><span data-stu-id="5de47-170">When you purchase and deploy an ISV's free trial-eligible product for your customer, the customer is automatically enrolled in the free trial by the ISV publisher.</span></span> <span data-ttu-id="5de47-171">無料試用期間は、ISV 発行者によって定義された期間が過ぎると自動的に終了します。</span><span class="sxs-lookup"><span data-stu-id="5de47-171">The free trial period ends automatically after the period defined by the ISV publisher.</span></span> <span data-ttu-id="5de47-172">期間が終了すると、顧客には課金されます。</span><span class="sxs-lookup"><span data-stu-id="5de47-172">After the period ends, the customer will be charged.</span></span> <span data-ttu-id="5de47-173">つまり、調整ファイルには試用対象製品の2つの行が表示されることがあります。1つは試用期間を追跡するもの、もう1つは有料プランを追跡するもの (試用期間が終了するまでに $0 のコストが表示されます) です。</span><span class="sxs-lookup"><span data-stu-id="5de47-173">This means the reconciliation file may show two rows for a trial-eligible product: One that tracks the trial period and one that tracks the paid offer (which will display a cost of $0 until after the trial period ends).</span></span> <span data-ttu-id="5de47-174">試用期間が終了すると、有料プランを示す行には料金が表示されます。</span><span class="sxs-lookup"><span data-stu-id="5de47-174">Once the trial ends, the row showing the paid offer will start to show charges.</span></span> 

<span data-ttu-id="5de47-175">各列が表す内容の詳細については、「[調整ファイルの使用](use-the-reconciliation-files.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5de47-175">For more information about what each column represents, see [Use your reconciliation files](use-the-reconciliation-files.md).</span></span> <span data-ttu-id="5de47-176">「[パートナーセンターでの課金の種類](billing-different-types.md)」も参照してください。</span><span class="sxs-lookup"><span data-stu-id="5de47-176">See also [Types of billing in Partner Center](billing-different-types.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="5de47-177">次のステップ</span><span class="sxs-lookup"><span data-stu-id="5de47-177">Next steps</span></span>

- [<span data-ttu-id="5de47-178">顧客向けの商用 marketplace 製品を管理する</span><span class="sxs-lookup"><span data-stu-id="5de47-178">Manage commercial marketplace products for customers</span></span>](csp-commercial-marketplace-manage.md)
- [<span data-ttu-id="5de47-179">商用 marketplace 製品のサポートについて説明します</span><span class="sxs-lookup"><span data-stu-id="5de47-179">Learn about support for commercial marketplace products</span></span>](csp-commercial-marketplace-support.md)
