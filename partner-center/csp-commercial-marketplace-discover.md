---
title: プランの検出-コマーシャルマーケットプレース
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP パートナーがパートナーセンターを使用して、SaaS プランや独立系ソフトウェアベンダー (Isv) からの価格を表示または検索する方法について説明します。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cb7b4ffdb4edf75e3e121e4ddea6b9de191ddbbf
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000416"
---
# <a name="discover-offers-and-pricing-in-the-partner-center-commercial-marketplace"></a><span data-ttu-id="4d4cc-103">パートナーセンターコマーシャルマーケットプレースでのプランと価格の検出</span><span class="sxs-lookup"><span data-stu-id="4d4cc-103">Discover offers and pricing in the Partner Center commercial marketplace</span></span>

<span data-ttu-id="4d4cc-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="4d4cc-104">**Applies to**</span></span>

- <span data-ttu-id="4d4cc-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="4d4cc-105">Partner Center</span></span>
- <span data-ttu-id="4d4cc-106">CSP プログラムのパートナー</span><span class="sxs-lookup"><span data-stu-id="4d4cc-106">Partners in the CSP program</span></span>

<span data-ttu-id="4d4cc-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="4d4cc-107">**Appropriate roles**</span></span>

- <span data-ttu-id="4d4cc-108">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="4d4cc-108">Global admin</span></span>
- <span data-ttu-id="4d4cc-109">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="4d4cc-109">Admin agent</span></span>

<span data-ttu-id="4d4cc-110">独立系ソフトウェアベンダー (Isv) は、商用マーケットプレースでプランを公開することを選択した場合、そのプランを CSP プログラムで利用できるようにするかどうかを決定することもできます。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-110">When Independent Software Vendors (ISVs) choose to publish an offer in the commercial marketplace, they can also decide if they want the offer to be made available in the CSP program.</span></span> <span data-ttu-id="4d4cc-111">CSP プログラムを通じてプランを販売することを選択した場合、CSP パートナーは、パートナーセンターの Marketplace 領域にプランを表示する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-111">If they choose to sell the offer through the CSP program, CSP partners should see the offer in the Partner Center Marketplace area.</span></span>

<span data-ttu-id="4d4cc-112">パートナーセンターで ISV プランが期待どおりに表示されない場合は、次の原因が考えられます。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-112">If an ISV offer does not appear as you expect in the Partner Center, it may be because:</span></span>

- <span data-ttu-id="4d4cc-113">ISV は、CSP プログラムを通じてプランを販売しないと判断しました。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-113">The ISV decided not to sell the offer through the CSP program.</span></span> <span data-ttu-id="4d4cc-114">たとえば、一部の ISV 製品は、商用マーケットプレースの他の領域 ( [Microsoft AppSource](https://appsource.microsoft.com/) や [Azure marketplace](https://azuremarketplace.microsoft.com/)など) で利用できるようになっていますが、パートナーセンターマーケットプレースの csp には記載されていない場合があります。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-114">For example, some ISV products may have been made available in other areas of the commercial marketplace (such as in [Microsoft AppSource](https://appsource.microsoft.com/) and [Azure Marketplace](https://azuremarketplace.microsoft.com/)), but may not appear for CSPs in the Partner Center marketplace.</span></span>

- <span data-ttu-id="4d4cc-115">ISV は、選択された数の CSP パートナーのみにプランを限定することに決めました。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-115">The ISV decided to make the offer exclusive to only a select number of CSP partners.</span></span> <span data-ttu-id="4d4cc-116">限定プランの詳細については、このヘルプトピックの「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-116">For more information about exclusive offers, see later in this help topic.</span></span>

- <span data-ttu-id="4d4cc-117">プランの種類は、パートナーセンターまたは Azure portal (たとえば、コンテナーや一部の使用量ベースのプラン) では不可能ない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-117">The offer type may not be transactable through the Partner Center or Azure portal (e.g. Containers or some usage-based offers).</span></span>

- <span data-ttu-id="4d4cc-118">この ISV プランでは、関連付けられている顧客の請求先の国がサポートされていない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-118">The billing country of your associated customer(s) may not be supported for this ISV offer.</span></span>

## <a name="view-marketplace-offers-in-partner-center"></a><span data-ttu-id="4d4cc-119">パートナーセンターで Marketplace のプランを表示する</span><span class="sxs-lookup"><span data-stu-id="4d4cc-119">View Marketplace offers in Partner Center</span></span>

<span data-ttu-id="4d4cc-120">CSP プログラムで利用可能な商用 marketplace プランを表示するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-120">To view available commercial marketplace offers in the CSP program:</span></span> 

1. <span data-ttu-id="4d4cc-121">パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインし、左側のナビゲーションメニューから [ **CSP** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-121">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="4d4cc-122">[ **販売**]、[ **Marketplace**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-122">Select **Sell**, followed by **Marketplace**.</span></span> <span data-ttu-id="4d4cc-123">既定では、すべての種類とカテゴリの製品が表示されます。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-123">By default, you will see products of all types and categories.</span></span>

3. <span data-ttu-id="4d4cc-124">種類またはカテゴリでフィルターを選択します。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-124">Select a filter by type or category.</span></span> <span data-ttu-id="4d4cc-125">また、 **検索** 機能を使用して、特定のキーワード、プラン名、ISV 発行元の名前を検索することもできます。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-125">You can also use **Search** to find specific keywords, offer names or the names of ISV publishers.</span></span>

4. <span data-ttu-id="4d4cc-126">一覧から特定の製品プランを選択します。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-126">Select a specific product offer from the list.</span></span> <span data-ttu-id="4d4cc-127">[製品の概要] タブが表示され、プランの詳細を確認できます。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-127">This will take you to a product Overview tab where you can learn more about the offer.</span></span> <span data-ttu-id="4d4cc-128">このタブには次の情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-128">Information on this tab might include:</span></span> 

    - <span data-ttu-id="4d4cc-129">製品またはプランの説明</span><span class="sxs-lookup"><span data-stu-id="4d4cc-129">A description of the product or offer</span></span>

    - <span data-ttu-id="4d4cc-130">ISV 発行者に関する詳細情報</span><span class="sxs-lookup"><span data-stu-id="4d4cc-130">More information about the ISV publisher</span></span>

    - <span data-ttu-id="4d4cc-131">ISV 発行元によってアップロードされたドキュメントまたはマーケティング資料へのリンク</span><span class="sxs-lookup"><span data-stu-id="4d4cc-131">Links to documentation or marketing materials uploaded by the ISV publisher</span></span>

    - <span data-ttu-id="4d4cc-132">CSP プログラムのカスタマーサポート、エンジニアリング、または連絡先に関する他の ISV 連絡先</span><span class="sxs-lookup"><span data-stu-id="4d4cc-132">Other possible ISV contacts for customer support, engineering, or a contact for the CSP Program</span></span>

5. <span data-ttu-id="4d4cc-133">プランの利用可能なプラン、Sku、または価格に関する詳細情報を表示するには、[ **プランと価格設定** ] タブを選択します。このタブには、次の項目が表示されます。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-133">To see more information about an offer's available plans, SKUs, or pricing, select the **Plans + Pricing** tab. This tab will show you:</span></span>

    - <span data-ttu-id="4d4cc-134">このプランが利用可能な市場</span><span class="sxs-lookup"><span data-stu-id="4d4cc-134">The markets where this offer is available to you</span></span>

    - <span data-ttu-id="4d4cc-135">プランで利用可能な Sku またはプランの一覧</span><span class="sxs-lookup"><span data-stu-id="4d4cc-135">A list of SKUs or plans available for the offer</span></span>

    - <span data-ttu-id="4d4cc-136">各 SKU または使用可能なプランの価格</span><span class="sxs-lookup"><span data-stu-id="4d4cc-136">Pricing for each SKU or Plan available</span></span>

## <a name="view-marketplace-offers-via-partner-center-apis"></a><span data-ttu-id="4d4cc-137">パートナーセンター Api を使用して Marketplace のプランを表示する</span><span class="sxs-lookup"><span data-stu-id="4d4cc-137">View Marketplace offers via Partner Center APIs</span></span>

<span data-ttu-id="4d4cc-138">CSP プログラムパートナーは Api を使用して、対象となるプランの一覧を返すこともできます。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-138">CSP program partners can also use APIs to return a list of eligible offers.</span></span> <span data-ttu-id="4d4cc-139">パートナーがパートナーセンター marketplace を通じて販売することができるのは、資格のあるオファーのみです。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-139">Eligible offers will be only those SaaS ISV offers available for the partner to sell via the Partner Center marketplace.</span></span> <span data-ttu-id="4d4cc-140">Api を使用してカタログ内のプランを特定するパートナー向けに、 [市場向けのプランの一覧を取得](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)するためのガイダンスを参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-140">For partners using APIs to identify offers in the catalog, refer to the guidance to [obtain a list of offers for a market](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).</span></span>

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a><span data-ttu-id="4d4cc-141">パートナーセンターで最新の Marketplace プランの価格を確認する</span><span class="sxs-lookup"><span data-stu-id="4d4cc-141">View the latest Marketplace offer pricing in Partner Center</span></span>

<span data-ttu-id="4d4cc-142">プランに関連付けられている最新の価格の詳細については、次の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-142">Follow these steps for the latest pricing details associated with an offer:</span></span>

1. <span data-ttu-id="4d4cc-143">パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインし、左側のナビゲーションメニューから [ **CSP** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-143">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="4d4cc-144">[ **販売**] を選択し、その後に [ **料金とプラン**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-144">Select **Sell**, followed by **Pricing and offers**.</span></span>

3. <span data-ttu-id="4d4cc-145">[ **Marketplace** ] セクションまで下にスクロールし、場所を選択して **marketplace の価格**をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-145">Scroll down to the **Marketplace** section, select a location and download **Marketplace pricing**.</span></span> <span data-ttu-id="4d4cc-146">これにより、SaaS の最新の価格データを含むスプレッドシートが生成され、ISV 発行元から提供されるライセンスベースのプランが生成されます。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-146">This generates a spreadsheet with the latest pricing data for SaaS, license-based offers available from ISV publishers.</span></span> <span data-ttu-id="4d4cc-147">一部の Azure アプリケーションの料金は、ここにも表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-147">Some Azure application pricing may also appear here.</span></span> <span data-ttu-id="4d4cc-148">この情報は毎日更新されるため、選択した頻度で現在の価格を確認することができます。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-148">This information is updated daily, so you can check it for current prices as often as you choose.</span></span>

4. <span data-ttu-id="4d4cc-149">ISV 製品に無料試用期間が含まれている場合、スプレッドシートにその製品の2つの行が表示されます。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-149">If an ISV product includes a free trial period, the spreadsheet will display two rows for that product:</span></span>

    - <span data-ttu-id="4d4cc-150">1行目は無料試用版の価格を示しています。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-150">One row shows the free trial price of zero.</span></span> <span data-ttu-id="4d4cc-151">つまり、無料試用期間を利用できます。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-151">This means a free trial period is available.</span></span>

    - <span data-ttu-id="4d4cc-152">もう1つの行には、無料試用期間が終了した後に適用される価格と使用条件が示されています。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-152">The other row shows the price and terms that will apply after the free trial period is over.</span></span>

<span data-ttu-id="4d4cc-153">CSP プログラムパートナーとして、特定の商用 marketplace プランに関連する他のインセンティブの対象となる場合があります。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-153">As a CSP program partner, you may be eligible for other incentives associated with certain commercial marketplace offers.</span></span> <span data-ttu-id="4d4cc-154">その他のインセンティブの詳細については、 [csp インセンティブガイド](https://aka.ms/partnerincentives) (csp ログインが必要) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-154">For more information about other incentives, see the [CSP incentive guide](https://aka.ms/partnerincentives) (requires CSP login).</span></span>

## <a name="learn-about-marketplace-exclusive-offers"></a><span data-ttu-id="4d4cc-155">Marketplace 限定プランの詳細</span><span class="sxs-lookup"><span data-stu-id="4d4cc-155">Learn about marketplace exclusive offers</span></span>

<span data-ttu-id="4d4cc-156">Isv は、CSP プログラムの特定のパートナーだけがオファーを利用できるようにするオプションを備えています。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-156">ISVs have the option to make their offers available only to specific partners in the CSP program.</span></span> <span data-ttu-id="4d4cc-157">これは、排他的なオファーとして知られています。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-157">This is known as an Exclusive offer.</span></span> <span data-ttu-id="4d4cc-158">CSP プログラム内のすべてのパートナーは、パートナーセンターの商用マーケットプレースにあるすべての ISV プランを表示できます (ただし、排他とマークされているプランを含む)。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-158">All partners in the CSP program can still view all ISV offers in the Partner Center commercial marketplace, including those offers marked Exclusive.</span></span>

<span data-ttu-id="4d4cc-159">プランが排他とマークされ **ていない** 場合は、すべてのパートナーがそのプランを購入できます (選択した顧客の請求先の国が ISV のオファーの使用可能な国に一致していることを前提とします)。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-159">If an offer is **not** marked Exclusive, all partners can purchase that offer (assuming the selected customer’s billing country matches the country availability of the ISV's offer).</span></span>

<span data-ttu-id="4d4cc-160">ただし、排他とマークされているプランでは、ISV によって選択されたパートナーだけがそのプランを購入できます。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-160">For any offer marked Exclusive, however, only those partners selected by the ISV will be able to purchase that offer.</span></span>

> [!NOTE]
> <span data-ttu-id="4d4cc-161">お客様に販売するものとして提供されているプランが [排他] として表示される場合は、ISV に直接連絡して、排他プランを販売するためのアクセス許可を要求します。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-161">If you see an offer marked Exclusive that you would like to sell to your customers, reach out to the ISV directly and ask for permission to sell the Exclusive offer.</span></span> <span data-ttu-id="4d4cc-162">排他プランの詳細を表示すると、選択できる [ **CONTACT ISV** ] リンクが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-162">When you view the details of an Exclusive offer, you may see a **Contact ISV** link that you can select.</span></span>

<span data-ttu-id="4d4cc-163">商用マーケットプレースの ISV エクスペリエンスの詳細については、 [クラウドソリューションプロバイダー](/azure/marketplace/cloud-solution-providers)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-163">To learn more about the ISV experience in the commercial marketplace, read [Cloud Solution Providers](/azure/marketplace/cloud-solution-providers).</span></span>

<span data-ttu-id="4d4cc-164">Marketplace での CSP エクスペリエンスの詳細については、「 [コマーシャルマーケットプレースの概要」](csp-commercial-marketplace-overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d4cc-164">For more information on the CSP experience in the marketplace, read [Commercial marketplace overview](csp-commercial-marketplace-overview.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="4d4cc-165">次のステップ</span><span class="sxs-lookup"><span data-stu-id="4d4cc-165">Next steps</span></span>

- [<span data-ttu-id="4d4cc-166">商用 marketplace プランの購入</span><span class="sxs-lookup"><span data-stu-id="4d4cc-166">Purchase commercial marketplace offers</span></span>](csp-commercial-marketplace-purchase.md)