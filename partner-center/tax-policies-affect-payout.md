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
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>税金ポリシーが支払いに与える影響Azure Marketplace

**適切なロール**

- グローバル管理者
- ユーザー管理の管理者
- 管理エージェント

## <a name="introduction"></a>はじめに

Microsoft コマーシャル マーケットプレースはグローバルに展開されています。 トランザクションは境界を越えて発生し、ISV と顧客がどこにいるかによって、税金への影響が異なる場合があります。 Microsoft AppSourceとAzure Marketplace、パートナー センタープロファイル情報を使用して ISV の国を決定します。 顧客の国を特定するには、顧客の請求情報を使用するか、お客様が EU に入っている場合は、2 つの異なる情報を使用します。

次のシナリオをよりよく理解するには、税の[](tax-details-marketplace.md)詳細の表を参照してください。これは、Microsoft が発行元に代わって税金を収集して支払うのか、その責任が発行元に属するかどうかを示しています。

> [!NOTE]
> このトピックのすべての販売額と税金の割合の例は、正確な数値ではなく、説明のみを目的とします。

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Microsoft が管理する税の国の発行元取引

**シナリオ A** – Microsoft が管理する税の国の発行元と顧客の間で [発生するトランザクション](tax-details-marketplace.md#microsoft-managed-countries)。 これらの取引には、販売時に適用される税金が追加され、Microsoft は該当する国に税金を送信します。 支払いから税金は差し引かされません。支払い計算は税抜きです。

米国 [以外の発行元](#foreign-publisher-transacts-with-us-customer) と米国の顧客の間のトランザクションについては、「シナリオ D」を参照してください。

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="支払いプロセス シナリオ A のワークフローを表示します。":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Marketplace の料金が課税対象サービスである Microsoft が管理する税国の発行元取引

**シナリオ B** – 米国に拠点を置く発行元 (パートナー センター 税プロファイル情報で定義されている) から、国が Marketplace 料金 (課税対象サービス) に税金を課す Microsoft が管理する税の国の顧客との間で発生するトランザクション。 このシナリオでは、ストア サービス料金に対する税金は、発行元の支払いから差し引きます。

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="支払いプロセス シナリオ B のワークフローを示します。":::

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

**シナリオ F** – Microsoft-Managed 国での海外の出版社と EU VAT 登録顧客 (アイルランド以外) のすべてのトランザクション。 お客様は、売上に対して税金を支払うことはありません。

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="支払いプロセスシナリオ F のワークフローを示します。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>国外の出版社は、Microsoft が管理する国 (アイルランド) で、EU に登録されたお客様を販売します。

**シナリオ G** – 米国内の外部発行元と EU の VAT 登録済み顧客 (アイルランド内) 間のすべての取引Microsoft-Managedします。 この税金は、お客様が日本政府に支払いを行い、Microsoft が本税を支払います。

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="支払いプロセス シナリオ G のワークフローを示します。":::

## <a name="next-steps"></a>次のステップ

- [発行元に関する FAQ](/azure/marketplace/marketplace-faq-publisher-guide)
- [支払いプロファイルと税プロファイルを作成する手順](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)