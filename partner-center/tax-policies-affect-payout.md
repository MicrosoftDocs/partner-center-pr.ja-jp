---
title: 税金ポリシーが支払いに与える影響Azure Marketplace
description: 税ポリシーが支払いに与える影響についてAzure Marketplace。
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: a93e94912f840e4cb69c3cc834f03af1b34f19aa
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856017"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="6ea1a-103">税金ポリシーが支払いに与える影響Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="6ea1a-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="6ea1a-104">**適切なロール**: グローバル管理者|ユーザー管理管理者|管理エージェント</span><span class="sxs-lookup"><span data-stu-id="6ea1a-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="6ea1a-105">はじめに</span><span class="sxs-lookup"><span data-stu-id="6ea1a-105">Introduction</span></span>

<span data-ttu-id="6ea1a-106">Microsoft コマーシャル マーケットプレースはグローバルに展開されています。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-106">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="6ea1a-107">トランザクションは境界を越えて発生し、ISV と顧客がどこにいるかによって、税金への影響が異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-107">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="6ea1a-108">Microsoft AppSourceとAzure Marketplace、パートナー センタープロファイル情報を使用して ISV の国を決定します。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-108">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="6ea1a-109">顧客の国を特定するには、顧客の請求情報を使用するか、お客様が EU に入っている場合は、2 つの異なる情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-109">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="6ea1a-110">次のシナリオをよりよく理解するには、税の[](tax-details-marketplace.md)詳細の表を参照してください。これは、Microsoft が発行元に代わって税金を収集して支払うのか、その責任が発行元に属するかどうかを示しています。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-110">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="6ea1a-111">このトピックのすべての販売額と税金の割合の例は、正確な数値ではなく、説明のみを目的とします。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-111">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="6ea1a-112">Microsoft が管理する税の国の発行元取引</span><span class="sxs-lookup"><span data-stu-id="6ea1a-112">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="6ea1a-113">**シナリオ A** – Microsoft が管理する税の国の発行元と顧客の間で [発生するトランザクション](tax-details-marketplace.md#microsoft-managed-countries)。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-113">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="6ea1a-114">これらの取引には、販売時に適用される税金が追加され、Microsoft は該当する国に税金を送信します。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-114">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="6ea1a-115">支払いから税金は差し引かされません。支払い計算は税抜きです。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-115">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="6ea1a-116">米国 [以外の発行元](#foreign-publisher-transacts-with-us-customer) と米国の顧客の間のトランザクションについては、「シナリオ D」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-116">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="支払いプロセス シナリオ A のワークフローを表示します。":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="6ea1a-118">Marketplace の料金が課税対象サービスである Microsoft が管理する税国の発行元取引</span><span class="sxs-lookup"><span data-stu-id="6ea1a-118">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="6ea1a-119">**シナリオ B** – 米国に拠点を置く発行元 (パートナー センター 税プロファイル情報で定義されている) から、国が Marketplace 料金 (課税対象サービス) に税金を課す Microsoft が管理する税の国の顧客との間で発生するトランザクション。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-119">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="6ea1a-120">このシナリオでは、ストア サービス料金に対する税金は、発行元の支払いから差し引きます。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-120">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="支払いプロセス シナリオ B のワークフローを示します。":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="6ea1a-122">発行元が管理する税の国の発行元取引</span><span class="sxs-lookup"><span data-stu-id="6ea1a-122">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="6ea1a-123">**シナリオ C** – 発行元と、顧客に対して差し引き税を課していない発行元が管理する税の国の顧客との間で発生するトランザクション。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-123">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="6ea1a-124">お客様は販売時点で税金を支払わないので、適用される税金を支払うのは発行元の義務です。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-124">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="6ea1a-125">国固有の価格 (今後の課税を相殺する場合など) の詳細については、「コマーシャル マーケットプレース オファーのプランと価格 [」を参照してください](/azure/marketplace/plans-pricing#custom-prices)。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-125">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="支払いプロセス シナリオ C のワークフローを示します。":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="6ea1a-127">米国顧客との外部発行元取引</span><span class="sxs-lookup"><span data-stu-id="6ea1a-127">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="6ea1a-128">**シナリオ D** – 米国の国の (パートナー センター 税プロファイル情報で定義されている) すべての外部発行元 (シナリオ [E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)を参照) が米国ベースの顧客に対して販売を行う (顧客アカウントの住所によって定義されます)。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-128">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="6ea1a-129">米国政府は、Microsoft が発行元に代わって税金を差し引く必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-129">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="6ea1a-130">支払いから発行元に差し引いた税金は、オファーの価格に基づいて計算されます。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-130">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="支払いプロセス シナリオ D のワークフローを示します。":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="6ea1a-132">米国のお客様との取引に関する協定を持つ外部発行元</span><span class="sxs-lookup"><span data-stu-id="6ea1a-132">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="6ea1a-133">**シナリオ E** – 米国の顧客に対して販売を行う米国の国 (パートナー センター 税プロファイル情報で定義されている) すべての外部発行元 (顧客アカウントの住所によって定義されます)。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-133">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="6ea1a-134">米国政府は、Microsoft が発行元に代わって税金を差し引く必要はない。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-134">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="支払いプロセス シナリオ E のワークフローを示します。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="6ea1a-136">外の発行元は、Microsoft が管理する国 (アイルランド以外) の EU VAT 登録済み顧客に販売します</span><span class="sxs-lookup"><span data-stu-id="6ea1a-136">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="6ea1a-137">**シナリオ F** – 米国内の外部発行元と EU の VAT に登録された顧客 (アイルランド以外) 間のすべての取引Microsoft-Managedします。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-137">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="6ea1a-138">顧客は、販売に対して税金を支払うのではありません。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-138">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="支払いプロセス シナリオ F のワークフローを示します。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="6ea1a-140">国外の出版社は、Microsoft が管理する国 (アイルランド) で、EU に登録されたお客様を販売します。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-140">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="6ea1a-141">**シナリオ G** – Microsoft-Managed 国での海外の出版社と EU VAT 登録のお客様 (アイルランド内) のすべての取引。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-141">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="6ea1a-142">お客様は、アイルランドの VAT を支払い、マイクロソフトはこの税金をアイルランド政府に支払います。</span><span class="sxs-lookup"><span data-stu-id="6ea1a-142">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="支払いプロセスシナリオ G のワークフローを示します。":::

## <a name="next-steps"></a><span data-ttu-id="6ea1a-144">次の手順</span><span class="sxs-lookup"><span data-stu-id="6ea1a-144">Next steps</span></span>

- [<span data-ttu-id="6ea1a-145">発行元の FAQ</span><span class="sxs-lookup"><span data-stu-id="6ea1a-145">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="6ea1a-146">支払いと税金のプロファイルを作成する手順</span><span class="sxs-lookup"><span data-stu-id="6ea1a-146">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)