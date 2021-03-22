---
title: Azure Marketplace の支払いポリシーが支払いに与える影響
description: 税金ポリシーが Azure Marketplace の支払いにどのように影響するかを説明します。
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 817cdb895efab553b6f0131cdcdcf9b24bc6db3e
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768824"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="1bbf3-103">Azure Marketplace の支払いポリシーが支払いに与える影響</span><span class="sxs-lookup"><span data-stu-id="1bbf3-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="1bbf3-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="1bbf3-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="1bbf3-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="1bbf3-105">Global admin</span></span>
-    <span data-ttu-id="1bbf3-106">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="1bbf3-106">User management admin</span></span>
-    <span data-ttu-id="1bbf3-107">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="1bbf3-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="1bbf3-108">はじめに</span><span class="sxs-lookup"><span data-stu-id="1bbf3-108">Introduction</span></span>

<span data-ttu-id="1bbf3-109">Microsoft の商用マーケットプレースにはグローバルなリーチがあります。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="1bbf3-110">トランザクションは、境界を越えて発生します。 ISV と顧客が配置されている場所によっては、税金の影響が異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="1bbf3-111">Microsoft AppSource と Azure Marketplace では、パートナーセンターの税プロファイル情報を使用して ISV の国を決定します。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="1bbf3-112">顧客の国を特定するには、顧客の請求情報を使用するか、顧客が EU 内にある場合は2つの異なる情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="1bbf3-113">次のシナリオについて理解を深めるには、「 [税金の詳細](tax-details-marketplace.md) 」の表を参照してください。これは、Microsoft が発行元に代わって税金を徴収または支払うか、またはその責任が発行元に属しているかを示しています。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="1bbf3-114">このトピックの売上値と税金の割合の例はすべて、わかりやすいように、正確な数値ではありません。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="1bbf3-115">Microsoft が管理する税国でのパブリッシャーのトランザクションの処理</span><span class="sxs-lookup"><span data-stu-id="1bbf3-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="1bbf3-116">**シナリオ A** – [Microsoft が管理する税の国](tax-details-marketplace.md#microsoft-managed-countries)で、発行元と顧客の間で行われるトランザクション。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="1bbf3-117">これらのトランザクションには、販売時点で適用される税金が適用され、マイクロソフトは該当する国にその税金を送信します。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="1bbf3-118">支払い額から源泉徴収される税金はなく、支払いの計算は限定されています。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="1bbf3-119">米国以外のパブリッシャーと米国のお客様の間のトランザクションについては、 [シナリオ D](#foreign-publisher-transacts-with-us-customer) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="支払いプロセスシナリオ A のワークフローを示します。":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="1bbf3-121">発行元のトランザクションは、Marketplace の料金が課税対象サービスである Microsoft 管理税の国で動作します</span><span class="sxs-lookup"><span data-stu-id="1bbf3-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="1bbf3-122">**シナリオ B** –米国ベースの発行元 (パートナーセンターの税プロファイル情報によって定義されている) 間で、Microsoft が管理している税の国において、お客様に対して、Marketplace の料金 (課税対象サービス) に対して税金が課せられた顧客に対して行われるトランザクション。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="1bbf3-123">このシナリオでは、ストアサービスの料金の税は、発行元の支払いから差し引かれます。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="支払いプロセスシナリオ B のワークフローを示します。":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="1bbf3-125">パブリッシャーによるトランザクションの処理は、発行元管理税の国で行う</span><span class="sxs-lookup"><span data-stu-id="1bbf3-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="1bbf3-126">**シナリオ C** –お客様に対して源泉徴収税が適用されていない、発行元管理の税金の国で、発行元と顧客の間で行われるトランザクション。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="1bbf3-127">お客様は、販売時点で税金を支払うことなく、適用されるすべての税金を支払うことになります。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="1bbf3-128">国固有の価格の詳細については (たとえば、今後の課税を相殺する場合)、「 [商業市場向けプランと価格](/azure/marketplace/plans-pricing#custom-prices)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="支払いプロセスシナリオ C のワークフローを示します。":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="1bbf3-130">外部パブリッシャーのトランザクションは、米国の顧客とやり取りします</span><span class="sxs-lookup"><span data-stu-id="1bbf3-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="1bbf3-131">**シナリオ D** –米国の条約を使用しない国では、パートナーセンターの税プロファイル情報によって定義されているように、米国のお客様への販売を行う ( [シナリオ E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)を参照してください) すべての外部出版社。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="1bbf3-132">米国政府機関は、発行元に代わって Microsoft の源泉徴収税を要求します。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="1bbf3-133">支払い額からパブリッシャーへの税金の源泉徴収は、プランの価格に基づいて計算されます。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="支払いプロセスシナリオ D のワークフローを示します。":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="1bbf3-135">米国のお客様との条約による海外パブリッシャー</span><span class="sxs-lookup"><span data-stu-id="1bbf3-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="1bbf3-136">**シナリオ E** –米国のお客様への販売を行っている国では、(パートナーセンターの税プロファイル情報によって定義されているように) すべての国外発行元 (顧客のアカウント住所で定義されているとおり)。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="1bbf3-137">米国政府機関では、Microsoft が発行元に代わって税金を源泉徴収する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="支払いプロセスシナリオ E のワークフローを示します。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="1bbf3-139">国外の出版社は、Microsoft が管理する国 (アイルランド以外) で、EU に登録されたお客様を販売します。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="1bbf3-140">**シナリオ F** – Microsoft-Managed 国での海外の出版社と EU VAT 登録顧客 (アイルランド以外) のすべてのトランザクション。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="1bbf3-141">お客様は、売上に対して税金を支払うことはありません。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="支払いプロセスシナリオ F のワークフローを示します。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="1bbf3-143">国外の出版社は、Microsoft が管理する国 (アイルランド) で、EU に登録されたお客様を販売します。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="1bbf3-144">**シナリオ G** – Microsoft-Managed 国での海外の出版社と EU VAT 登録のお客様 (アイルランド内) のすべての取引。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="1bbf3-145">お客様は、アイルランドの VAT を支払い、マイクロソフトはこの税金をアイルランド政府に支払います。</span><span class="sxs-lookup"><span data-stu-id="1bbf3-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="支払いプロセスシナリオ G のワークフローを示します。":::

## <a name="next-steps"></a><span data-ttu-id="1bbf3-147">次の手順</span><span class="sxs-lookup"><span data-stu-id="1bbf3-147">Next steps</span></span>

- [<span data-ttu-id="1bbf3-148">発行元の FAQ</span><span class="sxs-lookup"><span data-stu-id="1bbf3-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="1bbf3-149">支払いと税金のプロファイルを作成する手順</span><span class="sxs-lookup"><span data-stu-id="1bbf3-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)