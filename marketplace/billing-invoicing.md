---
title: 顧客に対する請求Azure Marketplace請求
description: この記事では、顧客に対する請求と請求に関する一般的Azure Marketplace説明します。
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: d45d301abfea03e06a8fc67e759012d4275d7dec
ms.sourcegitcommit: 8511fec63961d8c77a4d1eea3e3f1d37cdea46c6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/19/2021
ms.locfileid: "112373458"
---
# <a name="azure-marketplace-billing-and-invoicing"></a>Azure Marketplace請求と請求

この記事では、顧客に対する課金と請求Azure Marketplace説明します。

## <a name="microsoft-supports-multiple-currencies"></a>Microsoft では、複数の通貨がサポートされています

Azure Marketplaceは、次の 17 の通貨で価格が設定され、請求されます。

- オーストラリアドル (AUD)
- ブラジルの実 (政府)
- 英国ポンド (GBP)
- カナダ ドル (CAD)
- 中国語 (CNY)
- デンマーククローネ (DKK)
- Euro (EUR)
- インドルピー (INR)
- 日本の日本円 (JPY)
- 韓国語の勝利 (KRW)
- ニュージーランド ドル (NZD)
- ノルウェークローネ (NOK)
- ロシア語のくすき (RUSSIAN)
- スウェーデンクローナ (SEK)
- スイス語 (CHF)
- 台湾ドル (TWD)
- 米国ドル (USD)

## <a name="billing"></a>課金

購入した期間に、定期的な購入に対して課金されます。 これらの料金は、それぞれのカレンダー月の請求書に表示されます。 元の購入の同じ日に、次の期間に自動復元が続行されます。

[![月次および毎年の定期的な購入の請求方法のタイムラインの例。](media/billing/billing-charges-recurring.png)](media/billing/billing-charges-recurring.png#lightbox)

>[!NOTE]
> サービス期間は、サービスを使用するために支払った期間です。 事前にキャンセルしない限り、サービス期間の と で自動更新されます。

> [!NOTE]
> 更新月の日付が購入月の日付と等しくない場合は、請求月の最終日に調整されます。 つまり、1/31 にサブスクライブする場合、2 月の請求終了日は 2/27 になります。新しい請求期間は 2/28 (2/28、閏年から始まる場合は 2/29) から始まる予定です。

## <a name="invoices"></a>Invoices

各カレンダー月の初めに、請求書がカレンダーの月の初めに電子メールでAzure portal。 請求書には、カレンダー月中に購入または使用した無料プランと有料プランすべてが表示されます。 無料オファーのみがある場合は、0 ドルの明細項目しか表示され、支払いアクションを実行する必要はありません。 **Enterprise Agreement顧客は** 、Azure と Azure Marketplace の両方の料金 (オーストラリア、日本、シンガポールの顧客を除く) を示す合計請求書を受け取ります。 **サービスから直接購入Azure Marketplace、** 購入した場合にのみAzure Marketplace受け取ります。 詳細については [、「MOSP アカウントの請求書」を参照してください](/azure/cost-management-billing/understand/download-azure-invoice#invoices-for-mosp-billing-accounts)。

請求書を受け取る場合は、次の内容が異なります。

- 支払い方法がクレジット カードの場合は、予約の購入直後に請求されます。 この請求書は、毎月の請求書とは別の金額です。
- 支払い方法が check/wire の場合、この購入は毎月の Marketplace 請求書に含まれます。

Microsoft Online Services Program (MOSP)、Microsoft 顧客契約 (MCA)、Microsoft Partner Agreement (MPA) の各課金アカウントの請求書が作成されます。 請求書は、課金アカウントの種類に基づいて生成されます。 Azure Marketplace期間が終了した数日後に課金されます。 1 か月Azure Marketplace、スポット VM の請求書は、月の [9 日目頃に生成されます](/azure/cost-management-billing/understand/download-azure-invoice#invoices-for-mosp-billing-accounts)。 前月のそれぞれの料金が表示されます。 たとえば、ユーザーが 3 月 1 日に予約を購入し、3 月 30 日に別の予約を購入した場合、4 月の 1 つの請求書に両方の予約が含まれます。

請求書の詳細については、「Azure 外部サービスの [料金について」を参照してください](/azure/cost-management-billing/understand/understand-azure-marketplace-charges)。

## <a name="next-steps"></a>次の手順

- [Azure Marketplace とは何ですか?](azure-marketplace-overview.md)
- [Azure Marketplace購入](azure-purchasing-invoicing.md)
