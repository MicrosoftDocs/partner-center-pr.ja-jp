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
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Azure Marketplace の支払いポリシーが支払いに与える影響

**適切なロール**: 全体管理者 |ユーザー管理の管理者 |管理エージェント

## <a name="introduction"></a>はじめに

Microsoft の商用マーケットプレースにはグローバルなリーチがあります。 トランザクションは、境界を越えて発生します。独立系ソフトウェアベンダー (ISV) と顧客が配置されている場所によっては、税金の影響が異なる場合があります。 Microsoft AppSource と Azure Marketplace では、パートナーセンターの税プロファイル情報を使用して ISV の国を決定します。 顧客の国を特定するには、顧客の請求情報を使用するか、顧客が EU 内にある場合は2つの異なる情報を使用します。

次のシナリオについて理解を深めるには、「 [税金の詳細](tax-details-marketplace.md) 」の表を参照してください。これは、Microsoft が発行元に代わって税金を徴収または支払うか、またはその責任が発行元に属しているかを示しています。

> [!NOTE]
> このトピックの売上値と税金の割合の例はすべて、わかりやすいように、正確な数値ではありません。

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Microsoft が管理する税国でのパブリッシャーのトランザクションの処理

**シナリオ A** – [Microsoft が管理する税の国](tax-details-marketplace.md#microsoft-managed-countries)で、発行元と顧客の間で行われるトランザクション。 これらのトランザクションには、販売時点で適用される税金が適用され、マイクロソフトは該当する国にその税金を送信します。 支払い額から源泉徴収される税金はなく、支払いの計算は限定されています。

米国以外のパブリッシャーと米国のお客様の間のトランザクションについては、 [シナリオ D](#foreign-publisher-transacts-with-us-customer) を参照してください。

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="支払いプロセスシナリオ A のワークフローを示します。":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>発行元のトランザクションは、Marketplace の料金が課税対象サービスである Microsoft 管理税の国で動作します

**シナリオ B** –米国ベースの発行元 (パートナーセンターの税プロファイル情報によって定義されている) 間で、Microsoft が管理している税の国において、お客様に対して、Marketplace の料金 (課税対象サービス) に対して税金が課せられた顧客に対して行われるトランザクション。 このシナリオでは、ストアサービスの料金の税は、発行元の支払いから差し引かれます。

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="支払いプロセスシナリオ B のワークフローを示します。":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>パブリッシャーによるトランザクションの処理は、発行元管理税の国で行う

**シナリオ C** –お客様に対して源泉徴収税が適用されていない、発行元管理の税金の国で、発行元と顧客の間で行われるトランザクション。 お客様は、販売時点で税金を支払うことなく、適用されるすべての税金を支払うことになります。

国固有の価格の詳細については (たとえば、今後の課税を相殺する場合)、「 [商業市場向けプランと価格](/azure/marketplace/plans-pricing#custom-prices)」を参照してください。

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="支払いプロセスシナリオ C のワークフローを示します。":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>外部パブリッシャーのトランザクションは、米国の顧客とやり取りします

**シナリオ D** –米国の条約を使用しない国では、パートナーセンターの税プロファイル情報によって定義されているように、米国のお客様への販売を行う ( [シナリオ E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)を参照してください) すべての外部出版社。 米国政府機関は、発行元に代わって Microsoft の源泉徴収税を要求します。 支払い額からパブリッシャーへの税金の源泉徴収は、プランの価格に基づいて計算されます。

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="支払いプロセスシナリオ D のワークフローを示します。":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>米国のお客様との条約による海外パブリッシャー

**シナリオ E** –米国のお客様への販売を行っている国では、(パートナーセンターの税プロファイル情報によって定義されているように) すべての国外発行元 (顧客のアカウント住所で定義されているとおり)。 米国政府機関では、Microsoft が発行元に代わって税金を源泉徴収する必要はありません。

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="支払いプロセスシナリオ E のワークフローを示します。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>国外の出版社は、Microsoft が管理する国 (アイルランド以外) で、EU に登録されたお客様を販売します。

**シナリオ F** – Microsoft-Managed の国で、海外の出版社と EU 値 (VAT) に登録されている顧客 (アイルランド以外) のすべてのトランザクション。 お客様は、売上に対して税金を支払うことはありません。

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="支払いプロセスシナリオ F のワークフローを示します。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>国外の出版社は、Microsoft が管理する国 (アイルランド) で、EU に登録されたお客様を販売します。

**シナリオ G** – Microsoft-Managed 国での海外の出版社と EU VAT 登録のお客様 (アイルランド内) のすべての取引。 お客様は、アイルランドの VAT を支払い、マイクロソフトはこの税金をアイルランド政府に支払います。

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="支払いプロセスシナリオ G のワークフローを示します。":::

## <a name="next-steps"></a>次の手順

- [発行元の FAQ](/azure/marketplace/marketplace-faq-publisher-guide)
- [支払いと税金のプロファイルを作成する手順](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)