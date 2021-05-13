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
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>税金ポリシーが支払いに与える影響Azure Marketplace

**適切なロール**: グローバル管理者|ユーザー管理管理者|管理エージェント

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

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>発行元が管理する税の国の発行元取引

**シナリオ C** – 発行元と、顧客に対して差し引き税を課していない発行元が管理する税の国の顧客との間で発生するトランザクション。 お客様は販売時点で税金を支払わないので、適用される税金を支払うのは発行元の義務です。

国固有の価格 (今後の課税を相殺する場合など) の詳細については、「コマーシャル マーケットプレース オファーのプランと価格 [」を参照してください](/azure/marketplace/plans-pricing#custom-prices)。

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="支払いプロセス シナリオ C のワークフローを示します。":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>米国顧客との外部発行元取引

**シナリオ D** – 米国の国の (パートナー センター 税プロファイル情報で定義されている) すべての外部発行元 (シナリオ [E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)を参照) が米国ベースの顧客に対して販売を行う (顧客アカウントの住所によって定義されます)。 米国政府は、Microsoft が発行元に代わって税金を差し引く必要があります。 支払いから発行元に差し引いた税金は、オファーの価格に基づいて計算されます。

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="支払いプロセス シナリオ D のワークフローを示します。":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>米国のお客様との取引に関する協定を持つ外部発行元

**シナリオ E** – 米国の顧客に対して販売を行う米国の国 (パートナー センター 税プロファイル情報で定義されている) すべての外部発行元 (顧客アカウントの住所によって定義されます)。 米国政府は、Microsoft が発行元に代わって税金を差し引く必要はない。

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="支払いプロセス シナリオ E のワークフローを示します。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>外の発行元は、Microsoft が管理する国 (アイルランド以外) の EU VAT 登録済み顧客に販売します

**シナリオ F** – 米国内の外部発行元と EU の VAT に登録された顧客 (アイルランド以外) 間のすべての取引Microsoft-Managedします。 顧客は、販売に対して税金を支払うのではありません。

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="支払いプロセス シナリオ F のワークフローを示します。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>国外の出版社は、Microsoft が管理する国 (アイルランド) で、EU に登録されたお客様を販売します。

**シナリオ G** – Microsoft-Managed 国での海外の出版社と EU VAT 登録のお客様 (アイルランド内) のすべての取引。 お客様は、アイルランドの VAT を支払い、マイクロソフトはこの税金をアイルランド政府に支払います。

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="支払いプロセスシナリオ G のワークフローを示します。":::

## <a name="next-steps"></a>次の手順

- [発行元の FAQ](/azure/marketplace/marketplace-faq-publisher-guide)
- [支払いと税金のプロファイルを作成する手順](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)