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
ms.openlocfilehash: 100a3d2988c19d57f7426c7212b7464d8e96dc94
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152955"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Microsoft からサービスレベルアグリーメント (SLA) のクレジットを要求する方法とタイミング

**適切なロール**: 管理エージェント |全体管理者

お客様に提供しているサービスが停止している場合は、Microsoft からの **サービスレベルアグリーメント (SLA) クレジット** を要求できます。

## <a name="sla-credit-calculation"></a>SLA クレジットの計算

Microsoft からの SLA クレジットは、影響を受けたサービスに基づいて決定されます。 たとえば、顧客が Office 365 スイートを使用していても、SharePoint の停止しか経験していない場合は、顧客の計画全体ではなく、SharePoint に対してのみ SLA クレジットが承認されます。

*クレジットは、影響を受けるサービスと停止の期間に基づいて、日割りで評価されます。* SLA クレジットに適合するシナリオの種類を確認するには、 [オンラインサービスの統合](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)された sla に関するドキュメントを参照してください。 この情報は、クラウドソリューションプロバイダープログラムを通じて販売されたサービスにも適用されます。


## <a name="request-an-sla-credit"></a>SLA のクレジットを要求する

*クラウドソリューションプロバイダー (CSP) パートナーは、請求書および必要なすべての情報を、インシデントが発生した月の後のカレンダー月の終わりまでに提出する必要があります。* たとえば、インシデントが2月15日に発生した場合、マイクロソフトは、3月31日までに要求と必要なすべての情報を受け取る必要があります。 エンドカスタマーと間接リセラーは、SLA クレジット要求を送信できません。間接プロバイダーまたはダイレクト請求パートナーは、その代わりに要求を送信する必要があります。

>[!NOTE]
>アドバイザリインシデント ([Microsoft 365 service health を確認する方法](/microsoft-365/enterprise/view-service-health#incidents-and-advisories)) は、SLA クレジットの対象ではありません。

### <a name="required-information"></a>必要な情報

顧客名、テナント識別子、パートナーチケット番号、チケットが作成された日付/時刻スタンプは、要求を処理するのに十分ではありません。

マイクロソフトに [SLA クレジット要求を送信](#submit-sla-credit-request) する前に、サポートチケットに含まれる次の情報を **すべて** 収集する必要があります。

- 顧客テナントの GUID
- [停止インシデント識別子](#outage-incident-identifier)
- 顧客が停止の影響を受け、SLA クレジットを要求した証拠。
- 影響を受け取ったサブスクリプションは CSP を通じて購入されましたか? (*はい**またはいいえ*)

#### <a name="evidence-that-proves-customer-impact"></a>顧客への影響を証明する証拠

- ダウンタイムの時間と期間に関する情報
- 影響を受けるユーザーの数と場所 (該当する場合)
- 発生時にインシデントを解決しようとする試みについて説明します
- 影響を受け、サポートを要求している顧客からの電子メールと、その後のクレジット
- サービスへの影響の解決に関するサポート チケット番号と顧客の連絡先の詳細


#### <a name="outage-incident-identifier"></a>停止インシデント識別子

停止インシデントの識別子は、次のページのService Healthで確認Microsoft 365 管理センター。 停止 **インシデント ID は**、影響を受けるサービスを示す 2 文字の省略形が付いた数値です (たとえば、Exchange Online の停止の場合は *EX25194)。* 次の表では、一般的なサービスの省略形について説明します。

| 2 文字の省略形 | Microsoft サービス |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online Protection |
| SB | Skype for Business Online (旧 Lync Online) |
| OS | Office サブスクリプション |
|  PB | Office 365 用 BI 機能 |
| SP | SharePoint Online |
| 屋 | Yammer Enterprise |
| MO | ポータル エラー |

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
