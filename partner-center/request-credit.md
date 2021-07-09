---
title: Microsoft から SLA クレジットを要求する
ms.topic: article
ms.date: 03/31/2021
description: 顧客がサービスの停止を経験している場合に Microsoft からサービスレベルアグリーメント (SLA) のクレジットを要求するための特典、制限、および手順について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 3a0bb85143efe3d4135b56985b9a04e2dbe5e4cc
ms.sourcegitcommit: 57442bbbef15a70bd9a042642140cbf2c8608b09
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/09/2021
ms.locfileid: "113519435"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Microsoft からサービスレベルアグリーメント (SLA) のクレジットを要求する方法とタイミング

**適切なロール**: 管理エージェント |全体管理者

お客様に提供しているサービスが停止している場合は、Microsoft からの **サービスレベルアグリーメント (SLA) クレジット** を要求できます。

## <a name="sla-credit-calculation"></a>SLA クレジットの計算

Microsoft からの SLA クレジットは、影響を受けたサービスに基づいて決定されます。 たとえば、顧客が Office 365 スイートを使用していても、SharePoint の停止のみが発生した場合、SLA クレジットは SharePoint に対してのみ承認され、お客様のプラン全体では承認されません。

*クレジットは、影響を受けるサービスと停止の期間に基づいて、日割りで評価されます。* SLA クレジットに適合するシナリオの種類を確認するには、 [オンラインサービスの統合](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)された sla に関するドキュメントを参照してください。 この情報は、クラウドソリューションプロバイダー (CSP) プログラムを通じて販売されたサービスにも適用されます。


## <a name="request-an-sla-credit"></a>SLA のクレジットを要求する

*CSP パートナーは、インシデントが発生した月の後のカレンダー月の終わりまでに要求と必要なすべての情報を送信する必要があります。* たとえば、インシデントが2月15日に発生した場合、マイクロソフトは、3月31日までに要求と必要なすべての情報を受け取る必要があります。 エンドカスタマーと間接リセラーは、SLA クレジット要求を送信できません。間接プロバイダーまたはダイレクト請求パートナーは、その代わりに要求を送信する必要があります。

> [!NOTE]
> アドバイザリインシデントは、通常、SLA クレジットの対象にはなりません。 Service Health ダッシュボードに送信されたインシデントは、テナントが影響を受けている *可能性が* あることを示し、発行時に Microsoft が持っている最適な情報を表します。 正常性ページデータは、サービスの一般提供を表します。 個々のサービスの影響、軽減策、解決策は異なる場合があります。 詳細については、インシデントの最終投稿とインシデントレビューの投稿を確認してください。 詳細については、「 [How to check Microsoft 365 service health](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) 」を参照してください。

### <a name="required-information"></a>必要な情報

顧客名、テナント識別子、パートナーチケット番号、チケットが作成された日付/時刻スタンプは、要求を処理するのに十分ではありません。

マイクロソフトに [SLA クレジット要求を送信](#submit-sla-credit-request) する前に、サポートチケットに含まれる次の情報を **すべて** 収集する必要があります。

- 顧客テナントの GUID
- [停止インシデント識別子](#outage-incident-identifier)
- 顧客が停止によって影響を受け、SLA クレジットを要求したことを示す証拠。
- 影響を受けたサブスクリプションは CSP を通じて購入されましたか? (*yes* または *no*)

#### <a name="evidence-that-proves-customer-impact"></a>顧客への影響を証明する証拠

- ダウンタイムの時間と期間に関する情報
- 影響を受けるユーザーの数と場所 (該当する場合)
- 発生時のインシデントの解決試行の説明
- 影響を受ける顧客からのサポートを要求する電子メール
- サービスへの影響の解決に関するサポートチケット番号と顧客連絡先の詳細


#### <a name="outage-incident-identifier"></a>停止インシデント識別子

停止インシデントの識別子は、Microsoft 365 管理センターの [ **Service Health** ] ページで確認できます。 **停止インシデント ID** は、影響を受けるサービスを示す2文字の省略形で始まる番号です (たとえば、Exchange Online の停止の場合は *EX25194* )。 次の表では、一般的なサービスの省略形について説明します。

| 2文字の省略形 | Microsoft サービス |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online Protection |
| SB | Skype for Businessオンライン (以前の Lync Online) |
| OS | Office サブスクリプション |
|  PB | Office 365 用 BI 機能 |
| SP | SharePoint Online |
| YA | Yammer Enterprise |
| MO | ポータルエラー |

### <a name="submit-sla-credit-request"></a>SLA クレジット要求の送信

パートナーセンターのダッシュボードを使用して SLA クレジット要求を Microsoft に送信するには、次の手順を実行します。

1. パートナー センター ダッシュボードにサインインします。
2. 左側のメニューで、[ **サービス要求**] を選択し、[ **パートナーサポート要求**] を選択します。
3. [ **パートナーの要求** ] ページで、[ **新しい要求**] を選択します。
4. [ **要求の開始** ] ページで、 **CSP-customers、orders、およびサブスクリプション** を検索します。 このセクションで、[ **問題の種類を選択**] を選択し、[ **カスタマーサービスのクレジット要求**] を選択します。
5. [ **推奨されるソリューション** ] ページで、[ **追加のヘルプが必要ですか?**] の [ **はい]** を選択します。
6. [ **詳細** ] ページで、[ **問題の詳細** ] セクションに入力します。 [ **詳細** ] テキストボックスに、前に収集した [必要な情報](#required-information) を入力します。
7. [ **送信** ] を選択して、SLA クレジット要求を送信します。

## <a name="next-steps"></a>次のステップ

- [顧客に代わって問題を報告する](report-problems-on-behalf-of-a-customer.md)
