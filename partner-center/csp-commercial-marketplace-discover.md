---
title: プランの検出-コマーシャルマーケットプレース
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP パートナーがパートナーセンターを使用して、SaaS プランや独立系ソフトウェアベンダー (Isv) からの価格を表示または検索する方法について説明します。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ab30f8391df58155c8511dc628b1fefd94c8d768
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147974"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a><span data-ttu-id="087fb-103">パートナーセンターコマーシャルマーケットプレースでのプランと価格の検出</span><span class="sxs-lookup"><span data-stu-id="087fb-103">Discover offers and pricing in Partner Center commercial marketplace</span></span>

<span data-ttu-id="087fb-104">**適切なロール**: 全体管理者 |管理エージェント</span><span class="sxs-lookup"><span data-stu-id="087fb-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="087fb-105">独立系ソフトウェアベンダー (Isv) は、商用マーケットプレースでプランを公開することを選択した場合、そのプランを CSP プログラムで利用できるようにするかどうかを決定することもできます。</span><span class="sxs-lookup"><span data-stu-id="087fb-105">When Independent Software Vendors (ISVs) choose to publish an offer in the commercial marketplace, they can also decide if they want the offer to be made available in the CSP program.</span></span> <span data-ttu-id="087fb-106">CSP プログラムを通じてプランを販売することを選択した場合、CSP パートナーはパートナーセンターの Marketplace でプランを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="087fb-106">If they choose to sell the offer through the CSP program, CSP partners should see the offer in Partner Center Marketplace area.</span></span>

<span data-ttu-id="087fb-107">パートナーセンターで期待どおりに ISV プランが表示されない場合は、次の原因が考えられます。</span><span class="sxs-lookup"><span data-stu-id="087fb-107">If an ISV offer does not appear as you expect in Partner Center, it may be because:</span></span>

- <span data-ttu-id="087fb-108">ISV は、CSP プログラムを通じてプランを販売しないと判断しました。</span><span class="sxs-lookup"><span data-stu-id="087fb-108">The ISV decided not to sell the offer through the CSP program.</span></span> <span data-ttu-id="087fb-109">たとえば、一部の ISV 製品は、商用マーケットプレースの他の領域 ( [Microsoft AppSource](https://appsource.microsoft.com/) や [Azure marketplace](https://azuremarketplace.microsoft.com/)など) で利用できるようになっていますが、パートナーセンターマーケットプレースの CSP プログラムのパートナーには記載されていない場合があります。</span><span class="sxs-lookup"><span data-stu-id="087fb-109">For example, some ISV products may have been made available in other areas of the commercial marketplace (such as in [Microsoft AppSource](https://appsource.microsoft.com/) and [Azure Marketplace](https://azuremarketplace.microsoft.com/)), but may not appear for partners in the CSP program in Partner Center marketplace.</span></span>

- <span data-ttu-id="087fb-110">ISV は、選択された数の CSP パートナーのみにプランを限定することに決めました。</span><span class="sxs-lookup"><span data-stu-id="087fb-110">The ISV decided to make the offer exclusive to only a select number of CSP partners.</span></span> <span data-ttu-id="087fb-111">限定プランの詳細については、このヘルプトピックの「」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="087fb-111">For more information about exclusive offers, see later in this help topic.</span></span>

- <span data-ttu-id="087fb-112">プランの種類は、パートナーセンターまたは Azure portal (たとえば、コンテナーや一部の使用量ベースのプラン) では不可能ない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="087fb-112">The offer type may not be transactable through Partner Center or Azure portal (e.g. Containers or some usage-based offers).</span></span>

- <span data-ttu-id="087fb-113">この ISV プランでは、関連付けられている顧客の請求先の国がサポートされていない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="087fb-113">The billing country of your associated customer(s) may not be supported for this ISV offer.</span></span>

## <a name="view-marketplace-offers-in-partner-center"></a><span data-ttu-id="087fb-114">パートナーセンターで Marketplace のプランを表示する</span><span class="sxs-lookup"><span data-stu-id="087fb-114">View Marketplace offers in Partner Center</span></span>

<span data-ttu-id="087fb-115">CSP プログラムで利用可能な商用 marketplace プランを表示するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="087fb-115">To view available commercial marketplace offers in the CSP program:</span></span>

1. <span data-ttu-id="087fb-116">パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインし、左側のナビゲーションメニューから [ **CSP** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="087fb-116">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="087fb-117">[ **販売**]、[ **Marketplace**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="087fb-117">Select **Sell**, followed by **Marketplace**.</span></span> <span data-ttu-id="087fb-118">既定では、すべての種類とカテゴリの製品が表示されます。</span><span class="sxs-lookup"><span data-stu-id="087fb-118">By default, you will see products of all types and categories.</span></span>

3. <span data-ttu-id="087fb-119">種類またはカテゴリでフィルターを選択します。</span><span class="sxs-lookup"><span data-stu-id="087fb-119">Select a filter by type or category.</span></span> <span data-ttu-id="087fb-120">また、 **検索** 機能を使用して、特定のキーワード、プラン名、ISV 発行元の名前を検索することもできます。</span><span class="sxs-lookup"><span data-stu-id="087fb-120">You can also use **Search** to find specific keywords, offer names or the names of ISV publishers.</span></span>

4. <span data-ttu-id="087fb-121">一覧から特定の製品オファーを選択します。</span><span class="sxs-lookup"><span data-stu-id="087fb-121">Select a specific product offer from the list.</span></span> <span data-ttu-id="087fb-122">これにより、オファーの詳細を確認できる製品の [概要] タブが表示されます。</span><span class="sxs-lookup"><span data-stu-id="087fb-122">This will take you to a product Overview tab where you can learn more about the offer.</span></span> <span data-ttu-id="087fb-123">このタブの情報には、次のものが含まれる場合があります。</span><span class="sxs-lookup"><span data-stu-id="087fb-123">Information on this tab might include:</span></span> 

    - <span data-ttu-id="087fb-124">製品またはオファーの説明</span><span class="sxs-lookup"><span data-stu-id="087fb-124">A description of the product or offer</span></span>

    - <span data-ttu-id="087fb-125">ISV パブリッシャーの詳細</span><span class="sxs-lookup"><span data-stu-id="087fb-125">More information about the ISV publisher</span></span>

    - <span data-ttu-id="087fb-126">ISV 発行元によってアップロードされたドキュメントまたはマーケティング資料へのリンク</span><span class="sxs-lookup"><span data-stu-id="087fb-126">Links to documentation or marketing materials uploaded by the ISV publisher</span></span>

    - <span data-ttu-id="087fb-127">カスタマー サポート、エンジニアリング、または CSP プログラムの連絡先に関して、その他の可能な ISV 連絡先</span><span class="sxs-lookup"><span data-stu-id="087fb-127">Other possible ISV contacts for customer support, engineering, or a contact for the CSP program</span></span>

5. <span data-ttu-id="087fb-128">オファーの使用可能なプラン、SKU、または価格の詳細を表示するには、[プラン + 価格] タブ **を選択** します。このタブには次の情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="087fb-128">To see more information about an offer's available plans, SKUs, or pricing, select the **Plans + Pricing** tab. This tab will show you:</span></span>

    - <span data-ttu-id="087fb-129">このオファーを利用できる市場</span><span class="sxs-lookup"><span data-stu-id="087fb-129">The markets where this offer is available to you</span></span>

    - <span data-ttu-id="087fb-130">オファーで使用できる SKU またはプランの一覧</span><span class="sxs-lookup"><span data-stu-id="087fb-130">A list of SKUs or plans available for the offer</span></span>

    - <span data-ttu-id="087fb-131">使用可能な各 SKU またはプランの価格</span><span class="sxs-lookup"><span data-stu-id="087fb-131">Pricing for each SKU or Plan available</span></span>

## <a name="view-marketplace-offers-via-partner-center-apis"></a><span data-ttu-id="087fb-132">Api を使用して Marketplace オファーパートナー センター表示する</span><span class="sxs-lookup"><span data-stu-id="087fb-132">View Marketplace offers via Partner Center APIs</span></span>

<span data-ttu-id="087fb-133">CSP プログラム パートナーは、API を使用して、対象となるオファーの一覧を返す場合にも使用できます。</span><span class="sxs-lookup"><span data-stu-id="087fb-133">CSP program partners can also use APIs to return a list of eligible offers.</span></span> <span data-ttu-id="087fb-134">対象となるオファーは、パートナーがマーケットプレース経由で販売できる SaaS ISV オファーパートナー センターされます。</span><span class="sxs-lookup"><span data-stu-id="087fb-134">Eligible offers will be only those SaaS ISV offers available for the partner to sell via Partner Center marketplace.</span></span> <span data-ttu-id="087fb-135">API を使用してカタログ内のオファーを識別するパートナーについては、市場向けオファーの一覧を取得するためのガイダンス [を参照してください](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)。</span><span class="sxs-lookup"><span data-stu-id="087fb-135">For partners using APIs to identify offers in the catalog, refer to the guidance to [obtain a list of offers for a market](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).</span></span>

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a><span data-ttu-id="087fb-136">最新の Marketplace オファーの価格については、以下を参照パートナー センター</span><span class="sxs-lookup"><span data-stu-id="087fb-136">View the latest Marketplace offer pricing in Partner Center</span></span>

<span data-ttu-id="087fb-137">オファーに関連付けられている最新の価格の詳細については、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="087fb-137">Follow these steps for the latest pricing details associated with an offer:</span></span>

1. <span data-ttu-id="087fb-138">ダッシュボードにパートナー センター [し、](https://partner.microsoft.com/dashboard)左側のナビゲーション **メニューから [CSP]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="087fb-138">Sign into Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **CSP** from the left navigation menu.</span></span>

2. <span data-ttu-id="087fb-139">[販売 **] を** 選択し、続いて [価格と **プラン] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="087fb-139">Select **Sell**, followed by **Pricing and offers**.</span></span>

3. <span data-ttu-id="087fb-140">[Marketplace] セクションまで **下にスクロール** し、場所を選択して Marketplace の価格 **をダウンロードします**。</span><span class="sxs-lookup"><span data-stu-id="087fb-140">Scroll down to the **Marketplace** section, select a location and download **Marketplace pricing**.</span></span> <span data-ttu-id="087fb-141">これにより、SaaS、ライセンスベースのプラン、および ISV 発行元から提供されている従量制課金プランの最新の価格データを含むスプレッドシートが生成されます。</span><span class="sxs-lookup"><span data-stu-id="087fb-141">This generates a spreadsheet with the latest pricing data for SaaS, license-based offers and metered offers available from ISV publishers.</span></span> <span data-ttu-id="087fb-142">一部の Azure アプリケーションの料金は、ここにも表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="087fb-142">Some Azure application pricing may also appear here.</span></span> <span data-ttu-id="087fb-143">この情報は毎日更新されるため、選択した頻度で現在の価格を確認することができます。</span><span class="sxs-lookup"><span data-stu-id="087fb-143">This information is updated daily, so you can check it for current prices as often as you choose.</span></span>

4. <span data-ttu-id="087fb-144">ISV 製品に無料試用期間が含まれている場合、スプレッドシートにその製品の2つの行が表示されます。</span><span class="sxs-lookup"><span data-stu-id="087fb-144">If an ISV product includes a free trial period, the spreadsheet will display two rows for that product:</span></span>

    - <span data-ttu-id="087fb-145">1行目は無料試用版の価格を示しています。</span><span class="sxs-lookup"><span data-stu-id="087fb-145">One row shows the free trial price of zero.</span></span> <span data-ttu-id="087fb-146">つまり、無料試用期間を利用できます。</span><span class="sxs-lookup"><span data-stu-id="087fb-146">This means a free trial period is available.</span></span>

    - <span data-ttu-id="087fb-147">もう1つの行には、無料試用期間が終了した後に適用される価格と使用条件が示されています。</span><span class="sxs-lookup"><span data-stu-id="087fb-147">The other row shows the price and terms that will apply after the free trial period is over.</span></span>

<span data-ttu-id="087fb-148">CSP プログラムパートナーとして、特定の商用 marketplace プランに関連する他のインセンティブの対象となる場合があります。</span><span class="sxs-lookup"><span data-stu-id="087fb-148">As a CSP program partner, you may be eligible for other incentives associated with certain commercial marketplace offers.</span></span> <span data-ttu-id="087fb-149">その他のインセンティブの詳細については、 [csp インセンティブガイド](https://aka.ms/partnerincentives) (csp ログインが必要) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="087fb-149">For more information about other incentives, see the [CSP incentive guide](https://aka.ms/partnerincentives) (requires CSP login).</span></span>

## <a name="learn-about-marketplace-exclusive-offers"></a><span data-ttu-id="087fb-150">Marketplace 限定プランの詳細</span><span class="sxs-lookup"><span data-stu-id="087fb-150">Learn about marketplace exclusive offers</span></span>

<span data-ttu-id="087fb-151">Isv は、CSP プログラムの特定のパートナーだけがオファーを利用できるようにするオプションを備えています。</span><span class="sxs-lookup"><span data-stu-id="087fb-151">ISVs have the option to make their offers available only to specific partners in the CSP program.</span></span> <span data-ttu-id="087fb-152">これは、排他的なオファーとして知られています。</span><span class="sxs-lookup"><span data-stu-id="087fb-152">This is known as an Exclusive offer.</span></span> <span data-ttu-id="087fb-153">CSP プログラム内のすべてのパートナーは、パートナーセンターの商用 marketplace にあるすべての ISV プランを表示できます。ただし、排他とマークされているプランも含まれます。</span><span class="sxs-lookup"><span data-stu-id="087fb-153">All partners in the CSP program can still view all ISV offers in Partner Center commercial marketplace, including those offers marked Exclusive.</span></span>

<span data-ttu-id="087fb-154">プランが排他とマークされ **ていない** 場合は、すべてのパートナーがそのプランを購入できます (選択した顧客の請求先の国が ISV のオファーの使用可能な国に一致していることを前提とします)。</span><span class="sxs-lookup"><span data-stu-id="087fb-154">If an offer is **not** marked Exclusive, all partners can purchase that offer (assuming the selected customer’s billing country matches the country availability of the ISV's offer).</span></span>

<span data-ttu-id="087fb-155">ただし、排他とマークされているプランでは、ISV によって選択されたパートナーだけがそのプランを購入できます。</span><span class="sxs-lookup"><span data-stu-id="087fb-155">For any offer marked Exclusive, however, only those partners selected by the ISV will be able to purchase that offer.</span></span>

> [!NOTE]
> <span data-ttu-id="087fb-156">お客様に販売するものとして提供されているプランが [排他] として表示される場合は、ISV に直接連絡して、排他プランを販売するためのアクセス許可を要求します。</span><span class="sxs-lookup"><span data-stu-id="087fb-156">If you see an offer marked Exclusive that you would like to sell to your customers, reach out to the ISV directly and ask for permission to sell the Exclusive offer.</span></span> <span data-ttu-id="087fb-157">排他プランの詳細を表示すると、選択できる [ **CONTACT ISV** ] リンクが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="087fb-157">When you view the details of an Exclusive offer, you may see a **Contact ISV** link that you can select.</span></span>

<span data-ttu-id="087fb-158">商用マーケットプレースの ISV エクスペリエンスの詳細については、 [クラウドソリューションプロバイダー](/azure/marketplace/cloud-solution-providers)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="087fb-158">To learn more about the ISV experience in the commercial marketplace, read [Cloud Solution Providers](/azure/marketplace/cloud-solution-providers).</span></span>

<span data-ttu-id="087fb-159">Marketplace での CSP エクスペリエンスの詳細については、「 [コマーシャルマーケットプレースの概要」](csp-commercial-marketplace-overview.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="087fb-159">For more information on the CSP experience in the marketplace, read [Commercial marketplace overview](csp-commercial-marketplace-overview.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="087fb-160">次のステップ</span><span class="sxs-lookup"><span data-stu-id="087fb-160">Next steps</span></span>

- [<span data-ttu-id="087fb-161">商用 marketplace プランの購入</span><span class="sxs-lookup"><span data-stu-id="087fb-161">Purchase commercial marketplace offers</span></span>](csp-commercial-marketplace-purchase.md)