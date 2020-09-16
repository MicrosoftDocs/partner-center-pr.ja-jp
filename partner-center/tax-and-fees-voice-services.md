---
title: リージョン PSTN サービスの税と料金
description: 音声製品 Microsoft 365 行動する Office 365 パートナーとして、PSTN サービスの地域の税金、料金、または規制要件が適用される場合があります。
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5817e5bb010cee0ab280c83408167f28915a6237
ms.sourcegitcommit: 9b36128fdbd24e4bfe4597b1e6104bd560583c5c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "90594460"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>地域の税、公衆電話回線ネットワーク (PTSN) サービスの規制

**適用対象**

- パートナー センター
- Microsoft 365 音声製品を操作する Office 365 パートナー

**適切なロール**
-    グローバル管理者
-    ユーザー管理者
-    管理エージェント

一部の管轄区の公衆交換電話網 (PSTN) サービスには、パートナーの注文と請求に影響する可能性がある特別な税金および規制の要件が適用される場合があります。 米国には、オーディオ会議、通話プラン、および通信クレジットを含む PSTN サービスが含まれており、特別な税金と規制の要件が適用されます。 米国とプエルトリコでは、Microsoft は PSTN サービスを税金包括として価格を付けます。  独自の PSTN の税金と規制は、Microsoft 365 音声製品を操作する Office 365 パートナーに影響します。  パートナーが Microsoft PSTN サービスの価格を引き上げると、PSTN に関する税金と手数料を計算し支払う義務が生じる場合があります。

## <a name="partner-recommendations"></a>パートナーの推奨事項

お客様の組織の PSTN、税金、料金、およびその他の潜在的な負債に関する責任を理解するために、お客様の税金および法律顧問にご協力ください。

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>請求書プレゼンテーションとパートナー調整ファイル

米国の CSP 請求書および CSP 調整ファイル (Skype for Business PSTN と Microsoft 365 Voice サービスを含むカナダ) では、PSTN および PSTN 以外のコンポーネント用に個別の行項目が提供されます。

さらに、CSP の請求書には次の脚注が表示されます。

* 表示される料金は、オーディオ会議およびプランサービスの呼び出しに対して課金されます。  適用可能なトランザクションの税金については、米国内で行われた売上を除いて、示されている量だけが請求されます。  米国では、表示される料金は、通話プランとオーディオ会議サービスの料金が含まれているため、税金と料金が請求されます。  オーディオ会議と通話プランサービスは、Microsoft 関連によって提供されることが認められています。  詳細については、[Microsoft ボリューム ライセンス](https://go.microsoft.com/fwlink/?LinkId=690247)をご覧ください。

## <a name="reconciliation-file-example"></a>調整ファイルの例

Office 365 Enterprise E5 は、調整ファイルに同一の名前と同じ Id を持つ2つの行項目として表示されますが、各品目には一意の単価 (例: $28.40 と $2.00) があります。 これにより、Office 365 プランの Skype for Business PSTN 会議コンポーネントが区別され、税金を正しく適用することができます。

**パートナーの調整の例 #1 (列の選択):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Cycle fee   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Cycle fee   |2.00   |

**パートナーの調整の例 #2**

カナダで利用可能な Microsoft 365 Business 音声には、CSP 請求書に統合されている追加の PSTN 非課税コンポーネントがあります (Office 365 E5 と同様、2つの行項目が表示されます。1つは PSTN コンポーネント用、もう1つは pstn 以外のコンポーネント用) です。  Microsoft 365 Business 音声の CSP 調整ファイルには、すべての PSTN の非課税コンポーネントが個別に表示されます (個々の PSTN コンポーネントはに統合されません)。CSV または API ツール)。  調整ファイルで見つかった顧客の注文明細と請求金額の合計が CSP 請求書と一致します。

## <a name="additional-resources"></a>その他のリソース
詳細については、 [パートナーサイトの Microsoft 365](https://www.microsoft.com/microsoft-365/partners/) を参照してください。

