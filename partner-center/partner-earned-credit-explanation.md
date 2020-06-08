---
title: マネージド サービスのパートナー獲得クレジット
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: マネージド サービスに対する Microsoft パートナー獲得クレジット (PEC) の計算および支払方法と、お客様が適格であることを確認する方法について説明します。
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 653b75c0ec9cafdc39506eb8da82eefe6d8709e7
ms.sourcegitcommit: 3a1c0934ff337fc164bee690e7b9d69d113fdb99
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "84328213"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>パートナー獲得クレジットの計算方法と支払方法

**適切なロール**

- グローバル管理者
- ユーザー管理者
- 管理エージェント
- 課金管理者
- 販売代理店

マネージド サービスのパートナー獲得クレジット (PEC) では、顧客の Azure 環境の一部または全体の IT の運用と管理を 24 時間 365 日体制で実施しているパートナーを認識してリワードが提供されます。 既定では、CSP では、顧客のサブスクリプションに対して必要なアクセス権がパートナーに付与されます。これにより、パートナーは、サブスクリプションのリソースに対する運用管理と制御を 24 時間 365 日体制で実行できます。 次のセクションで、パートナーと取引するために顧客がアクセスをプロビジョニングするその他の方法について説明します。 月々の請求額は、パートナー獲得クレジットのネット値です。 パートナーは、毎月の調整ファイルで PEC の詳細を確認できます。 パートナーと取引するために顧客がアクセスをプロビジョニングするその他の方法については、「[Azure プランのサブスクリプションとリソースを管理する](azure-plan-manage.md)」を参照してください。

また、「[Azure CSP サブスクリプションの管理者特権を復元する](revoke-reinstate-csp.md)」もご覧ください

## <a name="important-eligibility-and-calculation-information"></a>参加資格と計算に関する重要な情報

- パートナーは、管理する Azure 資産に対して獲得したクレジットを受け取るには、アクティブな MPN 契約と有効な RBAC ロールが必要です。 

- 間接プロバイダーと間接リセラーの場合、間接プロバイダーは、間接プロバイダーか間接リセラーのどちらか一方またはその両方が 24 時間 365 日体制で顧客の CSP 内の Azure リソースを運用管理しているのであれば、PEC を獲得する資格があります。

- PEC は、パートナーによって管理される CSP 内の顧客の Azure 資産に対して課金される (請求可能な) 消費量に関連付けられます。 PEC は、Microsoft (間接プロバイダーと直接請求パートナー) によって課金される CSP のパートナーに対してのみ利用可能にすることができます。 

- 対象となるサービス:パートナー獲得クレジットは、パートナーが [Azure プランの価格](https://partner.microsoft.com/commerce/sales)ページからエクスポートできる **Azure プランの従量課金価格**に記載されているサービスに適用されます。 ただし、Azure プランの従量課金価格および Azure プランの予約の **[Tags]\(タグ\)** 列で **[Third Party]\(サードパーティ\)** として示されているサードパーティ製品や、Marketplace の価格表の製品には (それ以外についても)、例外があります。

- PEC は日単位で計算され、毎日の使用状況ファイルと毎月の請求調整ファイルで確認できます。 パートナー (間接プロバイダーまたは間接リセラー) が PEC を確実に取得するには、終日 (24 時間 365 日) のアクセス権を持っている必要があります。  

- PEC は、Azure リソース レベルで獲得されます。 パートナーがサブスクリプションまたはリソース グループ レベルで有効なアクセス権を持っている場合は、上位のエンティティにまとめられるリソースごとに PEC が獲得されます。  

- PEC の詳細は、[Azure Cost Management](https://go.microsoft.com/fwlink/?linkid=2106482) でも確認できます。

## <a name="azure-cost-management"></a>Azure Cost Management

 コスト分析を使用する Azure Cost Management (ACM) を使用すると、パートナーは、PEC の特典を受けたコストを表示できます。  

1. Azure Portal で、パートナー テナントにサインインし、 **[コストの管理と請求]** を選択します。
2.  **[コスト管理]** を選択します
3.  **[コスト分析]** を選択します

[コスト分析] ビューには、Microsoft に支払った料金で購入および使用したすべてのサービスについて、課金アカウントのコストが表示されます。

4.  PEC が適用されているコストを表示するには、ピボット グラフのドロップダウンで **PartnerEarnedCreditApplied** を選択します。 **PartnerEarnedCreditApplied** プロパティが True の場合、関連付けられているコストには、パートナー獲得クレジットの特典が適用されています。 

PartnerEarnedCreditApplied プロパティが False の場合、関連付けられているコストはクレジットに必要な資格を満たしていないか、購入したサービスがパートナー獲得クレジットの対象になっていません。

注: 通常、使用したサービスが **[コスト管理]** に表示されるまでには 8 から 24 時間かかり、PEC クレジットは Azure Cost Management にアクセスしてから 48 時間以内に表示されます。

5. また、 **[Group by and Add]\(グループ化と追加\)** フィルター機能を使用して **PartnerEarnedCreditApplied** プロパティでグループ化およびフィルター処理を行い、PEC が適用されたコストおよび PEC が適用されていないコストを詳しく調べることもできます。

 **詳細情報**

- [パートナー獲得クレジット - 概要](partner-earned-credit.md)

- パートナー獲得クレジットの計算の詳細な例については、パートナー センター ダッシュボードで確認できる価格表をご覧ください (サインインする必要があります)。

- [Azure プランに移行する - はじめに](azure-plan-get-started.md)

- [Azure プランのサブスクリプションとリソースを管理する](azure-plan-manage.md)

- [Azure CSP サブスクリプションの管理者特権を取り消したり元に戻したりする](revoke-reinstate-csp.md)

