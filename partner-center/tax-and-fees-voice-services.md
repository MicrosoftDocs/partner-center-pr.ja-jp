---
title: 地域の PSTN サービスの税金と料金
description: Microsoft 365 Voice 製品を取引する Office 365 パートナーは、PSTN サービスに関する地域の税金、料金、または規制要件の対象となる場合があります。
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 80cb5503323f483c13c983375559baf70f9d0b6f
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854725"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>地域税、公衆交換電話網 (PTSN) サービスの規制

**適切なロール**: グローバル管理者|ユーザー管理者|管理エージェント

一部の地域の公衆交換電話網 (PSTN) サービスは、パートナーの注文や請求に影響を与える可能性がある特別な税金および規制要件の対象となる場合があります。 この米国、電話会議、通話プラン、通信クレジットを含む PSTN サービスは、特別な税金および規制要件の対象となります。 米国および米国では、Microsoft は PSTN サービスに税金を含む価格を設定しています。  一意の PSTN 税と規制は、音声製品の取引を行う Office 365 Microsoft 365影響します。  パートナーが Microsoft PSTN サービスの価格を引き上げると、PSTN に関する税金と手数料を計算し支払う義務が生じる場合があります。

## <a name="partner-recommendations"></a>パートナーの推奨事項

PSTN サービスの規制、税金と料金、その他の潜在的な責任に関する組織の責任を理解するために、税金と法的措置を取る。

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>請求書プレゼンテーションとパートナー調整ファイル

skype for Business PSTN および Microsoft 365 Voice サービスを含む 米国、メキシコ、カナダの CSP 請求書と CSP 調整ファイルは、PSTN コンポーネントと PSTN 以外のコンポーネントに個別の品目を提供します。

さらに、CSP の請求書には、次の脚注が表示されます。

* 表示される価格は、電話会議および通話プラン サービスの料金です。  該当するトランザクション税は、表示される金額に対して課金されます。ただし、該当するトランザクション税は、米国。  米国では、表示される価格は、通話プランとオーディオ会議サービスの料金と、課金に必要な税金と料金が含まれるので、税金が含まれます。  オーディオ会議および通話プラン サービスは、それらを提供する権限を持つ Microsoft の系列会社によって提供されます。  詳細については、[Microsoft ボリューム ライセンス](https://go.microsoft.com/fwlink/?LinkId=690247)をご覧ください。

## <a name="reconciliation-file-example"></a>調整ファイルの例

Office 365 Enterprise E5 は、調整ファイルに同一の名前と同じ Id を持つ2つの行項目として表示されますが、各品目には一意の単価 (例: $28.40 と $2.00) があります。 これにより、Office 365 プランの Skype for Business PSTN 会議コンポーネントが区別され、税金を正しく適用することができます。

**パートナーの調整の例 #1 (列の選択):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Cycle fee   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Cycle fee   |2.00   |

**パートナーの調整の例 #2**

カナダで利用可能な Microsoft 365 Business 音声には、CSP 請求書に統合されている追加の PSTN 非課税コンポーネントがあります (Office 365 E5 と同様、2つの行項目が表示されます。1つは PSTN コンポーネント用、もう1つは pstn 以外のコンポーネント用) です。  Microsoft 365 Business 音声の CSP 調整ファイルには、すべての PSTN の非課税コンポーネントが個別に表示されます (個々の PSTN コンポーネントはに統合されません)。CSV または API ツール)。  調整ファイルで見つかった顧客の注文の詳細と請求金額の合計は、CSP 請求書と一致します。

## <a name="additional-resources"></a>その他の情報
詳細については、パートナー向けMicrosoft 365 [サイトを参照](https://www.microsoft.com/microsoft-365/partners/) してください。

