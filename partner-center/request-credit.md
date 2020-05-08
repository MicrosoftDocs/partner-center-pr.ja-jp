---
title: Microsoft から SLA クレジットを要求する
ms.topic: article
ms.date: 04/28/2020
description: 顧客がサービスの停止を経験している場合に Microsoft からサービスレベルアグリーメント (SLA) のクレジットを要求するための特典、制限、および手順について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: E7F1F68D-25E5-46C5-9C98-1D0A9FAB7993
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 328051d69f2dfd869cca8c80de595b2e27c9a1af
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/07/2020
ms.locfileid: "82907876"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Microsoft からサービスレベルアグリーメント (SLA) のクレジットを要求する方法とタイミング

お客様に提供しているサービスで障害が発生した場合に、Microsoft から**サービスレベルアグリーメント (SLA) のクレジット**を要求することができます。

## <a name="sla-credit-calculation"></a>SLA クレジットの計算

Microsoft からの SLA クレジットは、影響を受けたサービスに基づいて決定されます。 たとえば、顧客が Office 365 スイートを使用していても、SharePoint の停止しか経験していない場合は、顧客の計画全体ではなく、SharePoint に対してのみ SLA クレジットが承認されます。

*クレジットは、影響を受けるサービスと停止の期間に基づいて、日割りで評価されます。* SLA クレジットに適合するシナリオの種類を確認するには、[オンラインサービスの統合](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)された sla に関するドキュメントを参照してください。 この情報は、クラウドソリューションプロバイダープログラムを通じて販売されたサービスにも適用されます。

## <a name="request-an-sla-credit"></a>SLA のクレジットを要求する

*クラウドソリューションプロバイダー (CSP) パートナーは、請求書および必要なすべての情報を、インシデントが発生した月の後のカレンダー月の終わりまでに提出する必要があります。* たとえば、インシデントが2月15日に発生した場合、マイクロソフトは、3月31日までに要求と必要なすべての情報を受け取る必要があります。 エンドカスタマーと間接リセラーは、SLA クレジット要求を送信できません。間接プロバイダーまたはダイレクト請求パートナーは、その代わりに要求を送信する必要があります。

### <a name="required-information"></a>必要な情報

マイクロソフトに[SLA クレジット要求を送信](#submit-sla-credit-request)する前に、次の情報を収集してサポートチケットに含める必要があります。

- 顧客テナントの GUID
- [停止インシデント識別子](#outage-incident-identifier)
- 影響を受けたサブスクリプションは CSP を通じて購入されましたか? (*yes*または*no*)

#### <a name="outage-incident-identifier"></a>停止インシデント識別子

停止インシデントの識別子は、Microsoft 365 管理センターの [ **Service Health** ] ページで確認できます。 **停止インシデント ID**は、影響を受けるサービスを示す2文字の省略形 (Exchange Online が停止した場合の*EX25194*など) を表す数字です。 次の表では、一般的なサービスの省略形について説明します。

| 2文字の省略形 | Microsoft サービス |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online の保護 |
| SB | Skype for Business Online (以前の Lync Online) |
| OS | Office サブスクリプション |
|  PB | Office 365 用 BI 機能 |
| SP | SharePoint Online |
| YA | Yammer Enterprise |
| MO | ポータルエラー |

### <a name="submit-sla-credit-request"></a>SLA クレジット要求の送信

パートナーセンターのダッシュボードを使用して SLA クレジット要求を Microsoft に送信するには、次の手順を実行します。

1. パートナー センター ダッシュボードにサインインします。
2. 左側のメニューで、[**サービス要求**] を選択し、[**パートナーサポート要求**] を選択します。
3. [**パートナーの要求**] ページで、[**新しい要求**] を選択します。
4. [**要求の開始**] ページで、 **CSP-customers、orders、およびサブスクリプション**を検索します。 このセクションで、[**問題の種類を選択**] を選択し、[**カスタマーサービスのクレジット要求**] を選択します。
5. [**推奨されるソリューション**] ページで、[**追加のヘルプが必要ですか?**] の [**はい]** を選択します。
6. [**詳細**] ページで、[**問題の詳細**] セクションに入力します。 [**詳細**] テキストボックスに、前に収集した[必要な情報](#required-information)を入力します。
7. [**送信**] を選択して、SLA クレジット要求を送信します。
