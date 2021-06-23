---
title: Azure Marketplace の支払いポリシーが支払いに与える影響
description: 税金ポリシーが Azure Marketplace の支払いにどのように影響するかを説明します。
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 32c5cda9558aaaeddaf194eb8258ba732e2ac698
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/23/2021
ms.locfileid: "112489970"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="793e6-103">Azure Marketplace の支払いポリシーが支払いに与える影響</span><span class="sxs-lookup"><span data-stu-id="793e6-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="793e6-104">**適切なロール**: 全体管理者 |ユーザー管理の管理者 |管理エージェント</span><span class="sxs-lookup"><span data-stu-id="793e6-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="793e6-105">はじめに</span><span class="sxs-lookup"><span data-stu-id="793e6-105">Introduction</span></span>

<span data-ttu-id="793e6-106">Microsoft の商用マーケットプレースにはグローバルなリーチがあります。</span><span class="sxs-lookup"><span data-stu-id="793e6-106">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="793e6-107">トランザクションは、境界を越えて発生します。独立系ソフトウェアベンダー (ISV) と顧客が配置されている場所によっては、税金の影響が異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="793e6-107">Transactions occur across borders and depending on where the independent software vendor (ISV) and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="793e6-108">Microsoft AppSource と Azure Marketplace では、パートナーセンターの税プロファイル情報を使用して ISV の国を決定します。</span><span class="sxs-lookup"><span data-stu-id="793e6-108">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="793e6-109">顧客の国を特定するには、顧客の請求情報を使用するか、顧客が EU 内にある場合は2つの異なる情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="793e6-109">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="793e6-110">次のシナリオについて理解を深めるには、「 [税金の詳細](tax-details-marketplace.md) 」の表を参照してください。これは、Microsoft が発行元に代わって税金を徴収または支払うか、またはその責任が発行元に属しているかを示しています。</span><span class="sxs-lookup"><span data-stu-id="793e6-110">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="793e6-111">このトピックの売上値と税金の割合の例はすべて、わかりやすいように、正確な数値ではありません。</span><span class="sxs-lookup"><span data-stu-id="793e6-111">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="793e6-112">Microsoft が管理する税国でのパブリッシャーのトランザクションの処理</span><span class="sxs-lookup"><span data-stu-id="793e6-112">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="793e6-113">**シナリオ A** – [Microsoft が管理する税の国](tax-details-marketplace.md#microsoft-managed-countries)で、発行元と顧客の間で行われるトランザクション。</span><span class="sxs-lookup"><span data-stu-id="793e6-113">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="793e6-114">これらのトランザクションには、販売時点で適用される税金が適用され、マイクロソフトは該当する国にその税金を送信します。</span><span class="sxs-lookup"><span data-stu-id="793e6-114">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="793e6-115">支払い額から源泉徴収される税金はなく、支払いの計算は限定されています。</span><span class="sxs-lookup"><span data-stu-id="793e6-115">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="793e6-116">米国以外のパブリッシャーと米国のお客様の間のトランザクションについては、 [シナリオ D](#foreign-publisher-transacts-with-us-customer) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="793e6-116">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="支払いプロセスシナリオ A のワークフローを示します。":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="793e6-118">発行元のトランザクションは、Marketplace の料金が課税対象サービスである Microsoft 管理税の国で動作します</span><span class="sxs-lookup"><span data-stu-id="793e6-118">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="793e6-119">**シナリオ B** –米国ベースの発行元 (パートナーセンターの税プロファイル情報によって定義されている) 間で、Microsoft が管理している税の国において、お客様に対して、Marketplace の料金 (課税対象サービス) に対して税金が課せられた顧客に対して行われるトランザクション。</span><span class="sxs-lookup"><span data-stu-id="793e6-119">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="793e6-120">このシナリオでは、ストアサービスの料金の税は、発行元の支払いから差し引かれます。</span><span class="sxs-lookup"><span data-stu-id="793e6-120">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="支払いプロセスシナリオ B のワークフローを示します。":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="793e6-122">パブリッシャーによるトランザクションの処理は、発行元管理税の国で行う</span><span class="sxs-lookup"><span data-stu-id="793e6-122">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="793e6-123">**シナリオ C** –お客様に対して源泉徴収税が適用されていない、発行元管理の税金の国で、発行元と顧客の間で行われるトランザクション。</span><span class="sxs-lookup"><span data-stu-id="793e6-123">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="793e6-124">お客様は、販売時点で税金を支払うことなく、適用されるすべての税金を支払うことになります。</span><span class="sxs-lookup"><span data-stu-id="793e6-124">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="793e6-125">国固有の価格の詳細については (たとえば、今後の課税を相殺する場合)、「 [商業市場向けプランと価格](/azure/marketplace/plans-pricing#custom-prices)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="793e6-125">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="支払いプロセスシナリオ C のワークフローを示します。":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="793e6-127">外部パブリッシャーのトランザクションは、米国の顧客とやり取りします</span><span class="sxs-lookup"><span data-stu-id="793e6-127">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="793e6-128">**シナリオ D** –米国の条約を使用しない国では、パートナーセンターの税プロファイル情報によって定義されているように、米国のお客様への販売を行う ( [シナリオ E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)を参照してください) すべての外部出版社。</span><span class="sxs-lookup"><span data-stu-id="793e6-128">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="793e6-129">米国政府機関は、発行元に代わって Microsoft の源泉徴収税を要求します。</span><span class="sxs-lookup"><span data-stu-id="793e6-129">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="793e6-130">支払い額からパブリッシャーへの税金の源泉徴収は、プランの価格に基づいて計算されます。</span><span class="sxs-lookup"><span data-stu-id="793e6-130">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="支払いプロセスシナリオ D のワークフローを示します。":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="793e6-132">米国のお客様との条約による海外パブリッシャー</span><span class="sxs-lookup"><span data-stu-id="793e6-132">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="793e6-133">**シナリオ E** –米国のお客様への販売を行っている国では、(パートナーセンターの税プロファイル情報によって定義されているように) すべての国外発行元 (顧客のアカウント住所で定義されているとおり)。</span><span class="sxs-lookup"><span data-stu-id="793e6-133">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="793e6-134">米国政府機関では、Microsoft が発行元に代わって税金を源泉徴収する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="793e6-134">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="支払いプロセスシナリオ E のワークフローを示します。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="793e6-136">国外の出版社は、Microsoft が管理する国 (アイルランド以外) で、EU に登録されたお客様を販売します。</span><span class="sxs-lookup"><span data-stu-id="793e6-136">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="793e6-137">**シナリオ F** – Microsoft-Managed の国で、海外の出版社と EU 値 (VAT) に登録されている顧客 (アイルランド以外) のすべてのトランザクション。</span><span class="sxs-lookup"><span data-stu-id="793e6-137">**Scenario F** – All transactions between foreign publishers and EU value-added tax (VAT)-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="793e6-138">お客様は、売上に対して税金を支払うことはありません。</span><span class="sxs-lookup"><span data-stu-id="793e6-138">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="支払いプロセスシナリオ F のワークフローを示します。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="793e6-140">国外の出版社は、Microsoft が管理する国 (アイルランド) で、EU に登録されたお客様を販売します。</span><span class="sxs-lookup"><span data-stu-id="793e6-140">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="793e6-141">**シナリオ G** – Microsoft-Managed 国での海外の出版社と EU VAT 登録のお客様 (アイルランド内) のすべての取引。</span><span class="sxs-lookup"><span data-stu-id="793e6-141">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="793e6-142">お客様は、アイルランドの VAT を支払い、マイクロソフトはこの税金をアイルランド政府に支払います。</span><span class="sxs-lookup"><span data-stu-id="793e6-142">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="支払いプロセスシナリオ G のワークフローを示します。":::

## <a name="next-steps"></a><span data-ttu-id="793e6-144">次の手順</span><span class="sxs-lookup"><span data-stu-id="793e6-144">Next steps</span></span>

- [<span data-ttu-id="793e6-145">発行元の FAQ</span><span class="sxs-lookup"><span data-stu-id="793e6-145">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="793e6-146">支払いと税金のプロファイルを作成する手順</span><span class="sxs-lookup"><span data-stu-id="793e6-146">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)