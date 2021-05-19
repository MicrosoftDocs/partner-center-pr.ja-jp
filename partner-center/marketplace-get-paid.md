---
title: パートナーセンターでの有料
description: 商用 marketplace プラン、インセンティブプログラム、クラウドソリューションプロバイダープログラムなどを通じて、Microsoft パートナーとして収益の支払いを受ける方法について説明します。 支払いポリシー、支払い保留の状態、および支払い明細が含まれます。
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 11/25/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: 3dc8b728ef20da77b9a6d2a925ebb0388ea53837
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146495"
---
# <a name="getting-paid-in-partner-center"></a>パートナーセンターでの有料

**適切なロール**: Account admin |全体管理者

この記事には、プラン、アドオン、広告収益の支払いに関する重要な情報が記載されています。 支払いポリシー、支払い前に必要な手順、および支払い明細書の概要がまとめられています。

## <a name="payout-policies-and-agreements"></a>支払いポリシーと契約

支払いを受けるには、契約および支払いポリシーに従う必要があります。

- [Microsoft Azure Marketplace Publisher agreement](/legal/marketplace/msft-publisher-agreement): 支払いを受ける前に、この発行元契約に同意する必要があります。 本ライセンス条項は、Microsoft と Microsoft との間の関係について説明しています。これには、購入したすべての販売に関してマイクロソフトが請求する店舗料金も含まれます。
- 支払い[ポリシー](payout-policy-details.md)には、支払いスケジュールや支払い方法などの支払いポリシーが表示されます。 また、顧客の非支払いのプロセスについても説明します。
- 「[税金の詳細](tax-details-marketplace.md)」では、Microsoft [Publisher Agreement](/legal/marketplace/msft-publisher-agreement)の価格選択と税金の責任に関する税金の考慮事項について説明しています。
- **店舗料金** は、公式に発行元アグリーメントで定義されています。 店舗料金は、アドオンを含む、商用マーケットプレースによって収集されたすべてのプラン売上に適用されます。
- **支払いは月** 単位で行われます (支払いのしきい値が満たされている場合)。 通常、毎月15日までに、特定の月に支払いが送信されます。 支払いには一般に 3 ~ 10 営業日かかります。 詳細については、「[支払いのしきい値、方法、期間](payment-thresholds-methods-timeframes.md)」を参照してください。

## <a name="prerequisite-steps-before-getting-paid"></a>購入前の前提条件となる手順

初めて支払いを受け取る前に、支払いアカウントを設定し、必要な銀行および税フォームに記入する必要があります。 銀行および税のフォームでは、お好みの支払い方法と、源泉徴収税の税フォームを提供します。 支払いを行う前に、銀行と税のフォームが必要です。 詳細については、「支払い [アカウントと税フォームを設定する」を参照してください](set-up-your-payout-account.md)。

### <a name="payout-hold-status"></a>支払い保留状態

既定では、前述のように月単位で支払いを送信します。 ただし、プログラムの支払いを保留にできます。Microsoft は、お客様のアカウントに支払いをリリースすることはできません。 支払いを保留にした場合、引き続き [支払い] ページに収益 **が記録** されます。 ただしパートナー様によって保留状態が解除されるまでは、Microsoft からの支払いは口座に送金されません。

支払いを保留するには、右上にある [設定] 歯車アイコン、[アカウント設定] の順 **に選択します**。 左側 **のメニューで**[支払いと税金]を選択し、[支払いプロファイルと税金プロファイルの割り当て] セクションで、支払いを保持するプログラムを探します。 [支払 **いを保留する]** チェック ボックスをオンにして、このプログラムの支払いを保留します。 支払い保留状態はいつでも変更できますが、決定は次の毎月の支払いに影響します。 たとえば、4 月の支払いを保留したい場合、3 月が終わる前に支払い保留状態を **[オン]** に設定します。

支払い保留状態を **[オン**] に設定すると、このプログラムのすべての支払いは、チェック ボックスをオフにするまで保留 **になります**。 これを行う場合は、次の毎月の支払いサイクルに含まれます (支払いのしきい値が満たされている場合)。 支払いが保留されているが、6 月に支払いを生成する場合は、5 月末までに [オフ]チェック ボックスをオフにします。

>[!Note]
> 支払い保留状態は、各プログラムに個別に適用されます (Microsoft Store、広告、Azure Marketplaceなど)。 すべてのプログラムの支払いを保持する場合は、各プログラムの支払いを個別に保持します。

## <a name="payout-statements"></a>支払い明細

支払い明細書には、トランザクション履歴のオファーとアドオンからの売上からの収益が表示されます。 支払いの詳細を表示し、tsv または csv 形式でレポートをダウンロードすることもできます。 支払い明細書にアクセスする方法と、トランザクション履歴および支払いレポートの詳細については、「 [支払明細書](payout-statement.md) 」を参照してください。 さらに、 [Partner 支払い API](https://apidocs.microsoft.com/services/partnerpayouts) を使用して、支払いレポートを体系的にプルすることもできます。

## <a name="next-steps"></a>次のステップ

- [Partner 支払い API](https://apidocs.microsoft.com/services/partnerpayouts)
- [支払いに関する FAQ](payout-faq.md)