---
title: Microsoft の商用マーケットプレースに関する支払いに関してよく寄せられる質問
description: 商用マーケットプレースでの支払いに関してよく寄せられる質問への回答を得ます。
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/11/2020
ms.openlocfilehash: eea01f5c3c7f6e249a00e8b95df93274b87fb43d
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/25/2020
ms.locfileid: "91335700"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>コマーシャルマーケットプレース支払いに関してよく寄せられる質問

この記事では、商用マーケットプレースの支払いに関してよく寄せられる質問に回答します。

## <a name="earnings-incorrect-or-missing"></a>収益が間違っているか見つかりません

#### <a name="why-are-my-earnings-missing"></a>収益が欠けているのはなぜですか。

- 顧客の注文は、まだ支払いに適合していない可能性があります。 企業以外の顧客の注文については、発行元が資格を取得する前に、Microsoft がお客様の支払いを受ける必要があります。 企業の顧客の注文については、販売注文日から1-2 日後に収益が使用できるようになります。 注文 [レポート](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order)で注文の状態を確認します。
- 2019年7月より前のトランザクションの収益は、トランザクション履歴レポートに表示されない場合があります。 支払額の [ダウンロード](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport)の履歴ステートメントを確認します。
- 支払い [サイクルの時間枠](payment-thresholds-methods-timeframes.md) を確認し、支払い明細書に収益がどのように表示されるかを理解します。

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>予想とは異なる収入があるのはなぜですか。

- お客様によって注文が部分的に支払われた場合、料金と適切な税金を差し引いた額が部分的に支払われます。
- 国別の税金の責任を確認します。 税金がマイクロソフトによって責任を負う国の場合、Microsoft は発行元の利益から税金を徴収し、deducts します。 明細書に示されているトランザクションの金額は、課税額の後です。 「 [税金の詳細](tax-details-marketplace.md)」を参照してください。
- SaaS と IaaS のプランでは、standard 20% ではなく10% の割引機関の料金が発生し、収益率は90% になります。 このプロモーションは、2021年6月30日まで有効です。

**参考資料**: コマーシャルマーケット [プレース発行者契約](https://go.microsoft.com/fwlink/p/?LinkID=699560)、支払い [ポリシーの詳細](payout-policy-details.md)、 [支払いのしきい値、方法、時間帯](payment-thresholds-methods-timeframes.md)、商用マーケットプレース [での支払い](marketplace-get-paid.md)、税金の [詳細](tax-details-marketplace.md)、 [支払い明細書](payout-statement.md)、 [商業市場分析の注文ダッシュボード](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>収益の調整
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>分析で支払いステートメントを注文または使用状況レポートに調整操作方法
支払いトランザクション履歴レポートに表示される AssetID、orderID、および行項目 ID を使用して、分析注文と使用状況レポートを表示します。 次のマッピングを使用します。

- 支払いトランザクション履歴。 AssetID = order。OrderID
- 支払いトランザクション履歴。 OrderID & LineItem = Usage. UsageReferenceID [OrderID: LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>顧客の注文に対して支払いを予測する時期を操作方法
- まず、assetID を使用して、 [注文レポート](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order)で顧客の注文を確認します。
- 顧客のサブスクリプションについては、顧客 [レポート](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer)でカスタマーチャネルを確認してください。
- 企業のお客様については、発注日から1-2 日後に、出版社の収益が明細書に記載されています。
- 非企業のお客様については、お客様の支払いが受領されてから1-2 日後に発行元の収益が示されます。

**参考資料**: [支払い明細書](payout-statement.md)、 [商業市場分析における注文ダッシュボード](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>支払いポリシー

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>現在の機関の料金と支払い率を確認操作方法には、

- 市販の marketplace 発行者契約を確認します。 標準機関の料金は20% です。 SaaS 共同販売の対象となるトランザクションには、10% の割引料金が適用されます。 プロモーション機関の料金のお知らせを確認します。
- 支払い明細では、指定されたトランザクションの実際の支払い率を指定します。

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>Microsoft からの支払いは、ステートメントに1回表示されると予想されますか?
- 実績が未処理の状態になったら、収益を処理する月の成熟日を確認できます。 支払いの準備が完了すると、獲得状態が "処理済み" に変わります。  Microsoft は、成熟度月の15日で支払いをリリースします。
- クレジットカードによる注文の場合、Microsoft は、収益が成熟するまで30日間支払いを行います。

 **参考資料**: [市販の Marketplace 発行者契約](https://go.microsoft.com/fwlink/p/?LinkID=699560)、 [支払いポリシーの詳細](payout-policy-details.md)、 [税金の詳細](tax-details-marketplace.md)、 [支払いのしきい値、方法、時間枠](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>支払いと調整

#### <a name="why-is-my-payment-missing"></a>支払いが見つからないのはなぜですか。

- [[概要] ページ](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)で、支払いの状態と税金のプロファイルの状態が*有効*として表示されていることを確認します。
- 支払いの最小しきい値を満たしていない可能性があります。 支払いを受けるには、収益が $50 米ドル以上である必要があります。


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>アカウントで支払いを受けないように設定操作方法ますか?
支払いは、支払い [プロファイル](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)に保持できます。単に **ホールド**をチェックします。 マイクロソフトは、保留を解除するまでお支払いをお待ちしています。

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>購入通貨とは異なる通貨で受信するのはなぜですか。

支払い通貨は、支払いプロファイルで選択した通貨に基づいて算出されます。 購入通貨は、顧客が支払った通貨に基づいています。

#### <a name="how-do-i-reconcile-adjustments"></a>調整の調整を操作方法しますか?

支払いの調整は、システムの問題などの補正調整に対応するための支払いの修正です。 支払いステートメントでは、理由コードによって調整の理由が指定されます。 これらは、個々のトランザクションに直接調整するためのものではありません。

**参考資料**: [市販の Marketplace 発行者契約](https://go.microsoft.com/fwlink/p/?LinkID=699560)、 [支払いポリシーの詳細](payout-policy-details.md)、 [税金の詳細](tax-details-marketplace.md)、 [支払いのしきい値、方法、時間枠](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>税

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>支払い明細書に含まれる Microsoft または発行元の税送金責任はどのようにして特定できますか?

[トランザクション履歴のダウンロード] で、[税モデル] 列を見つけます。 これは、MS 管理または ISV によって管理されることを示します。 [税の詳細](tax-details-marketplace.md)については、「国固有の税ルールと支払いによる影響」を参照してください。

#### <a name="how-do-i-download-service-fee-tax-forms"></a>操作方法サービス料金税のフォームをダウンロードしますか?

支払い **支払い** ページにアクセスし、[支払い] セクション **の一覧を表示** します。 サービス手数料税を持つ支払いについては、サービス料金税のフォームへのリンクが表示されます。

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>PDF で源泉徴収税フォームをダウンロード操作方法には、

支払い *支払い* ページにアクセスし、[支払い] セクション **の一覧を表示** します。 支払の横に、源泉徴収税フォームへのリンクが表示されます。

#### <a name="where-do-i-find-year-end-tax-forms"></a>年度末の税金のフォームはどこで確認できますか?

[ [プロファイル] ページ](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) にアクセスして、年度末の税フォームを表示します。

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>トランザクションの源泉徴収税を検索操作方法には
源泉徴収税は、米国太平洋標準時の出版社に適用されます。 源泉徴収税は、毎月の支払いで計算されます。

**参考資料**: [商業市場発行者契約](https://go.microsoft.com/fwlink/p/?LinkID=699560)、 [支払いポリシーの詳細](payout-policy-details.md)

## <a name="payout-statement-access"></a>支払明細書へのアクセス

#### <a name="how-do-i-access-a-payout-statement"></a>支払明細書にアクセス操作方法

1. ロールを確認します。 支払い明細書にアクセスするには、 *財務共同作成* 者または *アカウント所有者* ロールが必要です。
2. 右上のナビゲーションで、[ **支払** ] アイコンを選択して、支払明細書を表示します。 **トランザクション履歴**、**支払い**、**ダウンロード**のいずれかを選択します。

**参考資料**: [支払いロールと権限](payout-statement.md#roles-and-permissions)、 [支払いステートメント](payout-statement.md) 

## <a name="payout-statement-report"></a>支払明細書レポート

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>トランザクションのダウンロードの各フィールドにはどのような意味がありますか。

属性とその意味の詳細な一覧については、「 [支払いステートメント](payout-statement.md) 」を参照してください。

#### <a name="what-is-earning-status"></a>獲得ステータスとは

これは、未処理、処理、または送信された収益を示しています。

- **未処理** -収益は、成熟日までのエスクロー期間になります。
- **処理** –収益は成熟しており、毎月の支払いで準備されています。 支払いは、毎月15日にリリースされます。
- **送信** -支払いプロファイルに基づいて銀行に支払いが正常にリリースされました。

#### <a name="how-do-i-download-service-fee-tax-forms"></a>操作方法サービス料金税のフォームをダウンロードしますか?

支払い **支払い** ページにアクセスし、[支払い] セクション **の一覧を表示** します。 サービス手数料税を持つ支払いについては、サービス料金税のフォームへのリンクが表示されます。

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>PDF で源泉徴収税フォームをダウンロード操作方法には、

支払い **支払い** ページにアクセスし、[支払い] セクション **の一覧を表示** します。 支払の横に、源泉徴収税フォームへのリンクが表示されます。

#### <a name="where-do-i-find-year-end-tax-forms"></a>年度末の税金のフォームはどこで確認できますか?

[ [プロファイル] ページ](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) にアクセスして、年度末の税フォームを表示します。

**参考資料**: [支払いステートメント](payout-statement.md)、 [トランザクション履歴のダウンロード](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>履歴明細書

#### <a name="how-do-i-view-historical-information"></a>履歴情報を表示操作方法には

履歴ステートメントでは、2019年10月時点での支払いデータのスナップショットが表示されます。 残念ながら、ここに示す支払い情報は更新されません。 最新の情報を入手するには、最新のデータのサポートチケットを送信します。

**参考資料**: [支払いステートメント](payout-statement.md)、 [トランザクション履歴のダウンロード](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>支払いのエクスポート API

#### <a name="how-do-i-download-payout-data"></a>支払いデータをダウンロード操作方法には

[パートナー支払い API](https://apidocs.microsoft.com/services/partnerpayouts)を使用します。

## <a name="next-steps"></a>次のステップ

- [コマーシャル マーケットプレースでの支払いの受け取り](marketplace-get-paid.md)
