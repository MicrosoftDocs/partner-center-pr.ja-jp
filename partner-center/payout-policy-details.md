---
title: 支払いスケジュールとプロセス
description: 支払いおよびトランザクション (支払いスケジュールや、支払いや他のトランザクションの再Azure Marketplaceについて学習します。
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 05/25/2021
ms.openlocfilehash: bcecd4c31d80a4130331c652491e7951af180c67
ms.sourcegitcommit: f1255fb65eac6ee2e0ff0cb95cc16a02dc57fc1a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/27/2021
ms.locfileid: "110582425"
---
# <a name="payout-schedules-and-processes"></a>支払いスケジュールとプロセス

**適切なロール**: アカウント管理者|グローバル管理者

この記事では、Microsoft の支払いスケジュール、支払いの状態を確認する場所、および顧客の支払い以外のプロセスについて説明します。

## <a name="payment-schedules"></a>支払いスケジュール

以下のセクションでは、トランザクションまたは CSP トランザクションの **Enterprise Agreement支払** Microsoft 顧客契約 **について** 説明します。

### <a name="transactions-when-customer-has-an-enterprise-agreement"></a>顧客が顧客を持つ場合のEnterprise Agreement

顧客がトランザクションに対して既存の Microsoft Enterprise Agreement を使用して Microsoft AppSource または Azure Marketplace から製品を購入した場合、顧客請求書の後の次の支払いサイクルで支払いを発行します。 顧客がクレジット カードを使用するトランザクションには、支払いの前に 30 日間の保有期間があります。

支払いは、多くの場合、Microsoft が顧客から支払いを収集する前に発生します。 お [客様が Microsoft への支払いに](#process-for-customer-non-payment) 失敗したが、既に支払いを発行している場合に実行するアクションについては、以下の「顧客の支払い以外の処理」を参照してください。

| Event | 説明 | レポートの可視性 | タイミング* |
| --- | --- | --- | --- |
| 使用状況またはトランザクションの月 | 顧客はサービスを使用または購入します。 | [使用状況](/azure/marketplace/partner-center-portal/usage-dashboard)または[注文ダッシュボード](/azure/marketplace/partner-center-portal/orders-dashboard) | **月 1** |
| Microsoft が請求金額を計算する | 合計使用量、合計トランザクション数を決定する | [使用状況](/azure/marketplace/partner-center-portal/usage-dashboard)または[注文ダッシュボード](/azure/marketplace/partner-center-portal/orders-dashboard) | **月 2** |
| 投稿された支払い | 機関の費用と支払いの利益を確認する | [支払いステートメント](payout-statement.md)のトランザクション履歴で未処理としてマークされている | **Month 3 (第1週)** |
| 支払いを準備する | 毎月の支払いのために収益が準備されています | [支払明細書](payout-statement.md)のトランザクション履歴で、次のようにマークされています。 | **Month 3 (第1週)** |
| **送信された支払い** | **支払いはパブリッシャーに送信されます** | **トランザクション履歴と、支払い [明細書](payout-statement.md)の支払いセクションで送信済みとしてマークされます。** | **月 3 (15 日以降)** |
| 顧客によって支払われる請求書 | Microsoft がお客様から支払いを収集します | 変更なし | **月 4 ~ 12** |
|

\* 支払い日は太平洋標準時 (PST) です。

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="エンタープライズ契約のお客様の支払いのタイムライン。":::

### <a name="transactions-when-customer-has-a-microsoft-customer-agreement-or-csp"></a>顧客が Microsoft の顧客契約または CSP を持っている場合のトランザクション

クレジットカードまたは月次請求書によるすべての購入には、顧客から資金が収集されることを保証するために、30日間の保持期間があります。

| Event | 説明 | レポートの可視性 | 調節 |
| --- | --- | --- | --- |
| 使用状況またはトランザクションの月 | 顧客はサービスを使用または購入します。 | [使用状況](/azure/marketplace/partner-center-portal/usage-dashboard)または[注文ダッシュボード](/azure/marketplace/partner-center-portal/orders-dashboard) | **月 1** |
| 顧客による請求書の支払い | 合計使用量、合計トランザクション値、および顧客の支払い請求書を決定する | [使用状況](/azure/marketplace/partner-center-portal/usage-dashboard)または[注文ダッシュボード](/azure/marketplace/partner-center-portal/orders-dashboard) | **月 2** |
| 投稿された支払い | 機関の料金と支払い収益を決定する | 支払い明細書のトランザクション履歴で未処理として [マークされます](payout-statement.md) | **月 2** |
| 30 日間の保有期間 | 資金、可能なチャージバック、および返金要求の収集を確認する | 支払い明細書のトランザクション履歴で未処理として [マークされます](payout-statement.md) | **月 3** |
| 支払いを準備する | 収益は毎月の支払いのために準備されます | 支払い明細書のトランザクション履歴で [近日予定] [としてマークされます](payout-statement.md) | **月 4 (第 1 週)** |
| **送信された支払い** | **支払いはパブリッシャーに送信されます** | **トランザクション履歴と、支払い [明細書](payout-statement.md)の支払いセクションで送信済みとしてマークされます。** | **Month 4 (15 日以降)** |
|

\* 支払い日は太平洋標準時 (PST) です。

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="クレジットカードおよび請求書の顧客に対する支払いのタイムライン。":::

## <a name="process-for-customer-non-payment"></a>顧客が未払いの場合のプロセス

まれに、コマーシャル マーケットプレースでの購入の代金を Microsoft が顧客から集められないことがあります。 顧客が請求スケジュールに従って Microsoft に支払いを行わない場合は、集金プロセスが開始されます。 このプロセスには 4 か月ほどかかり、Microsoft からの通知が永続的に送られます。 このプロセスの最後までに支払いを受けていない場合、Microsoft は資金を回収不可として書き込みます。

ここで説明する支払いプロセスにより、Microsoft では、最終的に回収不能となった資金をパブリッシャー (お客様) に既に支払っている可能性があります。 そのため、こうした金額を調整するプロセスが用意されています。

Microsoft では、次のいずれかの方法を使用して、支払い済みの代金を回収します。(1) Microsoft では、将来の支払いから未払い額を差し引く可能性があります。たとえば、支払いのうち 1,000 ドルが回収不能と判断されて損金処理された場合、1,000 ドルが回収されるまで将来の支払いが保留されます。または、(2) Microsoft では、未回収金額についてパブリッシャーに返済を要求するか、請求書を送る可能性があります。

次のスケジュールを例に示します。

| Event | 概算の日付 * | パートナーへの表示対象 |
| --- | --- | --- |
| 支払日の例 | 2020 年 10 月 15 日 | 支払いダッシュボードのトランザクション履歴と [支払い] セクションで **送信済み** とマークされます |
| <font color="red">顧客が Microsoft に支払いを行わない場合</font> | 2020 年 12 月 2 日 – 2020 年 12 月 5 日 | 変更なし、同上 |
| 顧客が最初の支払い遅延メールを受け取る | 2020 年 12 月 6 日 | なし |
| 顧客が、緊急度が高まっていることを知らせる定期的なメールを受け取る | 2020 年 12 月 7 日 – 2021 年 1 月 31 日 | なし |
| 損金処理の可能性があることがパブリッシャーに通知される | 2021 年 1 月 7 日 | - |
| 顧客が終了通知を受け取る | 2021 年 2 月 1 日 | なし |
| 集金プロセスの終了/資金の損金処理 | 2021 年 2 月 15 日 | 資金が損金処理されたことを示す電子メール通知がパブリッシャーに送信されます。 |
| 支払い額が差し引かれる | 2021 年 3 月 1 日 | パートナーセンターの支払い明細書に、パブリッシャによって負のトランザクションが表示される |
| 支払いが保留される | 2021 年 3 月 15 日 | 今後の支払いは、パートナーセンターの支払い明細書に表示されます。 パブリッシャーは、残高が負でなくなるまで支払いを受け取れなくなります。  |
|||

\* 支払い日は太平洋標準時 (PST) です。

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>支払いが支払い受取口座に着金するまでの日数

通常、毎月15日の特定の月に支払いが送信されますが、支払いがアカウントに到着するまでに別の時間がかかります。 日数は、以下で説明するように、アカウントに使用する支払い方法によって異なります。

> [!NOTE]
> 次に示す曜日は概数です。支払いによっては、お客様のアカウントにより多くの時間がかかる場合があります。

| 支払い方法     | 支払い受取口座に着金するまでの日数     |
|--------------------|--------------------------------------------|
| PayPal             | 1 営業日                             |
| ACH または SEPA           | 2 から 3 営業日                          |
| 電信送金      | 7 から 10 営業日                         |
|

## <a name="next-steps"></a>次のステップ

- [税の詳細](tax-details-marketplace.md)
