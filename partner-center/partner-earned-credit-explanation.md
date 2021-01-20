---
title: マネージド サービスのパートナー獲得クレジット
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: マネージド サービスに対する Microsoft パートナー獲得クレジット (PEC) の計算および支払方法と、お客様が適格であることを確認する方法について説明します。
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f274103feeadfa6fd135f99632f3013c29601972
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182411"
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

## <a name="eligibility"></a>特典を受ける条件

パートナー獲得クレジット (PEC) を受け取るには、次の要件が適用されます。 

- 自分が管理する Azure 資産に対する獲得クレジットを受け取るには、アクティブな MPN 契約と有効なロールベースのアクセス制御 (RBAC) ロールが必要です。

- CSP では、顧客の Azure リソースを 24 時間体制で制御し、管理する必要があります。 つまり、顧客の Azure サブスクリプション、Azure リソース グループ、Azure リソースに対する管理者特権が必要です。 間接プロバイダーとその間接リセラーの場合、間接プロバイダーは、間接プロバイダーか間接リセラーのどちらか一方またはその両方がこの運用管理を行っているのであれば、PEC を獲得する資格があります。 詳細については、[Azure CSP サブスクリプションの管理者特権を復元する](./revoke-reinstate-csp.md)ことに関するページをご覧ください。

- 上記の要件に加えて、PEC は Azure プランの従量課金価格に記載されているサービスにのみ適用されます。これは [Azure プランの価格](https://partner.microsoft.com/commerce/sales)ページからエクスポートできます。

- PEC は、以下のサービスには適用 **されません**。
    - Azure プランの予約
    - Azure プラン従量課金価格の [タグ] 列に "サード パーティ" と表示されているサード パーティ製品
    - Marketplace 価格表の製品
    - [Azure スポット仮想マシン](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- PEC は、Azure リソース レベルで獲得されます。 サブスクリプションまたはリソース グループ レベルのいずれかで有効なアクセス権をお持ちの場合は、上位のエンティティにまとめられるリソースごとに PEC が獲得されます。

- PEC の詳細については、[Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners) に関するページもご覧ください。

### <a name="calculation"></a>計算

PEC は日単位で計算され、毎日の使用状況ファイルと毎月の請求調整ファイルで確認できます。 パートナー (間接プロバイダーまたは間接リセラー) が PEC を確実に取得するには、終日 (24 時間 365 日) のアクセス権を持っている必要があります。 PEC は、マネージド Azure 資産を対象として 1 日単位で計算されます。 特定の請求期間 (月) に対する最大 PEC は 15% です。 パートナーは、永続的な特権アクセスを月中ずっと保持し (アクセスの期間)、かつそれがすべての対象リソースに及ぶなら (アクセスの範囲)、15% の全 PEC を獲得します。 範囲と期間が減ると、その月の PEC レートは低くなります。 毎日評価される使用量ファイルには、特定の Azure 資産について PEC が適用されているかどうかが 1 日単位で示されます。 パートナーは、永続的な特権アクセスに対する変更を監視するためのアラートに登録することもできます。

## <a name="azure-cost-management"></a>Azure Cost Management

コスト分析を使用する Azure Cost Management (ACM) を使用すると、パートナーは、PEC の特典を受けたコストを表示できます。  

1. [Azure portal](https://portal.azure.com) で、パートナー テナントにサインインし、 **[コストの管理と請求]** を選択します。

2. **[コスト管理]** を選択します

3. **[コスト分析]** を選択します

   [コスト分析] ビューには、Microsoft に支払った料金で購入および使用したすべてのサービスについて、課金アカウントのコストが表示されます。

4. PEC が適用されているコストを表示するには、ピボット グラフのドロップダウンで **PartnerEarnedCreditApplied** を選択します。 **PartnerEarnedCreditApplied** プロパティが True の場合、関連付けられているコストには、パートナー獲得クレジットの特典が適用されています。 

   PartnerEarnedCreditApplied プロパティが False の場合、関連付けられているコストはクレジットに必要な資格を満たしていないか、購入したサービスがパートナー獲得クレジットの対象になっていません。

   >[!NOTE] 
   >通常、使用したサービスが **[コスト管理]** に表示されるまでには 8 から 24 時間かかり、PEC クレジットは Azure Cost Management にアクセスしてから 48 時間以内に表示されます。

5. また、 **[Group by and Add]\(グループ化と追加\)** フィルター機能を使用して **PartnerEarnedCreditApplied** プロパティでグループ化およびフィルター処理を行い、PEC が適用されたコストおよび PEC が適用されていないコストを詳しく調べることもできます。

## <a name="next-steps"></a>次の手順

- [パートナー獲得クレジット - 概要](partner-earned-credit.md)

- パートナー獲得クレジットの計算の詳細な例については、パートナー センター ダッシュボードで確認できる価格表をご覧ください (サインインする必要があります)。

- [Azure プランに移行する - はじめに](azure-plan-get-started.md)

- [Azure プランのサブスクリプションとリソースを管理する](azure-plan-manage.md)

- [Azure CSP サブスクリプションの管理者特権の取り消しまたは復元](revoke-reinstate-csp.md)