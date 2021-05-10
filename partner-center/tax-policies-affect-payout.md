---
title: 税金ポリシーが支払いに与える影響Azure Marketplace
description: 税ポリシーが支払いに与える影響についてAzure Marketplace。
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 343db43633245030a5eba213cb5c8b79d09a7dee
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686315"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="5d9d3-103">税金ポリシーが支払いに与える影響Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="5d9d3-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="5d9d3-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="5d9d3-104">**Appropriate roles**</span></span>

- <span data-ttu-id="5d9d3-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="5d9d3-105">Global admin</span></span>
- <span data-ttu-id="5d9d3-106">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="5d9d3-106">User management admin</span></span>
- <span data-ttu-id="5d9d3-107">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="5d9d3-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="5d9d3-108">はじめに</span><span class="sxs-lookup"><span data-stu-id="5d9d3-108">Introduction</span></span>

<span data-ttu-id="5d9d3-109">Microsoft コマーシャル マーケットプレースはグローバルに展開されています。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="5d9d3-110">トランザクションは境界を越えて発生し、ISV と顧客がどこにいるかによって、税金への影響が異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="5d9d3-111">Microsoft AppSourceとAzure Marketplace、パートナー センタープロファイル情報を使用して ISV の国を決定します。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="5d9d3-112">顧客の国を特定するには、顧客の請求情報を使用するか、お客様が EU に入っている場合は、2 つの異なる情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="5d9d3-113">次のシナリオをよりよく理解するには、税の[](tax-details-marketplace.md)詳細の表を参照してください。これは、Microsoft が発行元に代わって税金を収集して支払うのか、その責任が発行元に属するかどうかを示しています。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="5d9d3-114">このトピックのすべての販売額と税金の割合の例は、正確な数値ではなく、説明のみを目的とします。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="5d9d3-115">Microsoft が管理する税の国の発行元取引</span><span class="sxs-lookup"><span data-stu-id="5d9d3-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="5d9d3-116">**シナリオ A** – Microsoft が管理する税の国の発行元と顧客の間で [発生するトランザクション](tax-details-marketplace.md#microsoft-managed-countries)。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="5d9d3-117">これらの取引には、販売時に適用される税金が追加され、Microsoft は該当する国に税金を送信します。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="5d9d3-118">支払いから税金は差し引かされません。支払い計算は税抜きです。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="5d9d3-119">米国 [以外の発行元](#foreign-publisher-transacts-with-us-customer) と米国の顧客の間のトランザクションについては、「シナリオ D」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="支払いプロセス シナリオ A のワークフローを表示します。":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="5d9d3-121">Marketplace の料金が課税対象サービスである Microsoft が管理する税国の発行元取引</span><span class="sxs-lookup"><span data-stu-id="5d9d3-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="5d9d3-122">**シナリオ B** – 米国に拠点を置く発行元 (パートナー センター 税プロファイル情報で定義されている) から、国が Marketplace 料金 (課税対象サービス) に税金を課す Microsoft が管理する税の国の顧客との間で発生するトランザクション。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="5d9d3-123">このシナリオでは、ストア サービス料金に対する税金は、発行元の支払いから差し引きます。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="支払いプロセス シナリオ B のワークフローを示します。":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="5d9d3-125">パブリッシャーによるトランザクションの処理は、発行元管理税の国で行う</span><span class="sxs-lookup"><span data-stu-id="5d9d3-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="5d9d3-126">**シナリオ C** –お客様に対して源泉徴収税が適用されていない、発行元管理の税金の国で、発行元と顧客の間で行われるトランザクション。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="5d9d3-127">お客様は、販売時点で税金を支払うことなく、適用されるすべての税金を支払うことになります。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="5d9d3-128">国固有の価格の詳細については (たとえば、今後の課税を相殺する場合)、「 [商業市場向けプランと価格](/azure/marketplace/plans-pricing#custom-prices)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="支払いプロセスシナリオ C のワークフローを示します。":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="5d9d3-130">外部パブリッシャーのトランザクションは、米国の顧客とやり取りします</span><span class="sxs-lookup"><span data-stu-id="5d9d3-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="5d9d3-131">**シナリオ D** –米国の条約を使用しない国では、パートナーセンターの税プロファイル情報によって定義されているように、米国のお客様への販売を行う ( [シナリオ E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)を参照してください) すべての外部出版社。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="5d9d3-132">米国政府機関は、発行元に代わって Microsoft の源泉徴収税を要求します。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="5d9d3-133">支払い額からパブリッシャーへの税金の源泉徴収は、プランの価格に基づいて計算されます。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="支払いプロセスシナリオ D のワークフローを示します。":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="5d9d3-135">米国のお客様との条約による海外パブリッシャー</span><span class="sxs-lookup"><span data-stu-id="5d9d3-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="5d9d3-136">**シナリオ E** –米国のお客様への販売を行っている国では、(パートナーセンターの税プロファイル情報によって定義されているように) すべての国外発行元 (顧客のアカウント住所で定義されているとおり)。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="5d9d3-137">米国政府機関では、Microsoft が発行元に代わって税金を源泉徴収する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="支払いプロセスシナリオ E のワークフローを示します。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="5d9d3-139">国外の出版社は、Microsoft が管理する国 (アイルランド以外) で、EU に登録されたお客様を販売します。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="5d9d3-140">**シナリオ F** – Microsoft-Managed 国での海外の出版社と EU VAT 登録顧客 (アイルランド以外) のすべてのトランザクション。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="5d9d3-141">お客様は、売上に対して税金を支払うことはありません。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="支払いプロセスシナリオ F のワークフローを示します。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="5d9d3-143">国外の出版社は、Microsoft が管理する国 (アイルランド) で、EU に登録されたお客様を販売します。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="5d9d3-144">**シナリオ G** – 米国内の外部発行元と EU の VAT 登録済み顧客 (アイルランド内) 間のすべての取引Microsoft-Managedします。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="5d9d3-145">この税金は、お客様が日本政府に支払いを行い、Microsoft が本税を支払います。</span><span class="sxs-lookup"><span data-stu-id="5d9d3-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="支払いプロセス シナリオ G のワークフローを示します。":::

## <a name="next-steps"></a><span data-ttu-id="5d9d3-147">次のステップ</span><span class="sxs-lookup"><span data-stu-id="5d9d3-147">Next steps</span></span>

- [<span data-ttu-id="5d9d3-148">発行元に関する FAQ</span><span class="sxs-lookup"><span data-stu-id="5d9d3-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="5d9d3-149">支払いプロファイルと税プロファイルを作成する手順</span><span class="sxs-lookup"><span data-stu-id="5d9d3-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)