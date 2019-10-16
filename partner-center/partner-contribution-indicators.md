---
title: パートナー貢献度インジケーター | パートナー センター
ms.topic: article
ms.date: 10/04/2019
description: パートナーの会社が Dynamics 365 Customer Engagement または Dynamics 365 Finance and Operationsでどのような実績を上げているかを示すデータ
ms.assetid: 2F4B9A27-37FF-41E4-8A26-5EAE88DD8A49
keywords: PCI, パフォーマンス, 顧客の成功, 測定, Dynamics 365
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: high
ms.custom: seodec18
ms.openlocfilehash: c0c8f9f721aa0cadfc311ecec5eb6349576fb26a
ms.sourcegitcommit: dcc2a2077ef17255ecf7a2fa5fae6bbeefaa9eb0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/07/2019
ms.locfileid: "71997830"
---
# <a name="partner-contribution-indicators"></a>パートナー貢献度インジケーター

パートナー貢献度インジケーター (PCI) は、Dynamics 365 でのパートナーのパフォーマンス、能力、および顧客の成功を総合的に測定した値のセットです。

## <a name="scoring"></a>スコア付け

PCI では、100 ポイントのスケールを使って、過去 12 か月のパートナーによる Dynamics 365 Customer Engagement または Dynamics 365 Finance and Operations での成功の指標が提供されます。 次に示すのは、PCI の 7 つの各メジャーで獲得できる最大ポイントです。

![スコア付け](images/pci1.png)

### <a name="thresholds"></a>しきい値

各 PCI メトリックには、パートナー企業が最大ポイントを獲得できるしきい値が Microsoft によって設定されてます。 これらのしきい値は、Customer Engagement と Finance & Operations では異なります。 しきい値は、パートナーが先進市場で活動しているか、または新興市場のみで活動するパートナーかによっても異なります。 パートナーに先進市場の顧客が 1 つでもある場合は、先進市場のしきい値が適用されます。 新興市場のしきい値が適用されるためには、パートナーのすべての顧客が新興市場に基づいている必要があります。 (国が先進市場または新興市場のどちらに分類されるかは、Microsoft Partner Network のこちらの定義に基づいています。)

パートナーは、次に示すしきい値を満たしているか超過している場合、特定のメトリックの最大ポイントを獲得できます。 機能コンサルタント増加率 (Functional consultant growth) を除くすべてのメトリックに対して、部分的なポイントを獲得できます。たとえば、新規純利益 (Net New Revenue) が $150,000 である先進市場のパートナーは、最大 10 ポイントの半分 ($150,000/$300,000) を獲得します。

### <a name="customer-engagement-thresholds"></a>Customer Engagement のしきい値

![Engagement のしきい値](images/pci3.png)

### <a name="finance-and-operations-thresholds"></a>Finance and Operations のしきい値

![Finance and Operations](images/pci4.png)

### <a name="developed-and-emerging-markets-functional-consultant-growth"></a>先進市場と新興市場における機能コンサルタントの成長 (Functional consultant growth) 

![先進市場と新興市場](images/pci6.png)
![先進市場と新興市場](images/pci7.png)

## <a name="detailed-definitions-for-each-of-the-pci-metrics"></a>各 PCI メトリックの詳細な定義


|**Metric**   |**ポイント**   |**定義**   |**評価期間**|
|---------------|:--------------------------|:-------------------|:----------|
|新規純利益 (Net new revenue)|10|指定された製品のすべての販売チャネルでの新規請求済み純利益。 請求金額からクレジットを差し引いた値が計算され、12 か月間について集計されます。
||| - **Customer Engagement** の製品には、Sales、Customer Service、Field Service、Project Service Automation、Marketing、Microsoft Relationship Sales、Talent、Enterprise Team Member が含まれます。 -
||| **Finance and Operations** の製品には、Finance and Operations、Retail、Talent、Enterprise Team Member が含まれます。販売チャネルには、エンタープライズ契約 (EA)、クラウド ソリューション プロバイダー (CSP)、Web ダイレクトが含まれます。 エンタープライズ契約の利益には、契約の最初の年からの利益のみが含まれます。 2 年目および 3 年目から繰り返し発生する利益は含まれません。|過去 12 か月|
|純顧客追加数 (Net customer adds)|10|すべての販売チャネルでの顧客の純追加数。 月ごとの顧客追加数から顧客喪失数を差し引いた値が計算され、12 か月間について集計されます。 顧客の追加とは、前月には支払い開始ユニットを持っていなかった顧客が、今月は持つようになった場合です。 顧客の喪失とは、前月には支払い開始ユニットを持っていた顧客が、今月は持たなくなった場合です。 販売チャネルには、エンタープライズ契約 (EA)、クラウド ソリューション プロバイダー (CSP)、Web ダイレクトが含まれます。 失った顧客を再度獲得したときに異なるパートナーが関連付けられた場合は、最新のパートナーがクレジットを受け取ります。|過去 12 か月|
|機能コンサルタント数 (Functional consultants)|15 |現在アクティブな機能コンサルタント認定を保有しているユーザーの数。**Customer Engagement**: 機能コンサルタント認定には、ユーザーが MB200 と、MB210、MB220、MB230、MB240、MB6-898 のいずれかを渡す必要があります。 **Finance and Operations**: 機能コンサルタント認定をには、ユーザーが MB300 と、MB310、MB320、MB330、MB6897、MB6-898 のいずれかを渡す必要があります。|現在のスナップショット|
|機能コンサルタント増加率 (Functional consultant growth)|15|現時点でアクティブな機能コンサルタント認定を保有しているユーザーの数と、**2019 年 12 月 31 日**の時点でアクティブな機能コンサルタント認定を保有しているユーザーの数の比較。 **部分ポイントは付与されません**。 増加率が、先進市場パートナーの場合は表 3 で示されているしきい値を、新興市場パートナーの場合は表 4 で示されているしきい値を、満たすか超えている必要があります。|現在のスナップショットと 2019 年 12 月 31 日のスナップショット|
|開発者向け|5|**Customer Engagement** の場合、これは MB2-716 の現在アクティブな認定を保持しているユーザーの数です。 **Finance and Operations** の場合、これは MB6-894 の現在アクティブな認定を保持しているユーザーの数です。|現在のスナップショット|
|新規大規模展開数 (New large deployments)|20|**Customer Engagement** の場合、過去 12 か月間に、有料サブスクリプションが月間 250 アクティブ ユーザーのしきい値を超えた場合、関連付けられているパートナーは、そのテナント下のすべての Customer Engagement 運用インスタンス数 (組織数) に対するクレジットを獲得します。 **Finance and Operations** の場合、過去 12 か月間に、有料サブスクリプションが月間 100 アクティブ ユーザーのしきい値を超えた場合、関連付けられているパートナーは、そのテナント下のすべての Finance and Operations 運用インスタンス数 (CS プロジェクト数) に対するクレジットを獲得します。 月間アクティブ ユーザー数はサブスクリプション レベルでカウントされ、有料サブスクリプションのみが対象となります。 月間アクティブ ユーザー数は、毎月の終了時に計算されます。 指定された月間アクティブ ユーザー数しきい値を 13 か月前の時点で下回っていて、過去 12 か月間に 1 回でもそのしきい値を超えた場合、サブスクリプションは月間アクティブ ユーザー数しきい値を超えたものと見なされます。 テナントに複数のサブスクリプションがあり、それぞれが異なるパートナーに関連付けられている場合、関連付けられている有料サブスクリプションが必要な月間アクティブ ユーザー数しきい値を超えた場合、すべてのパートナーが、該当する製品カテゴリでテナント下にあるすべての運用インスタンスに対するクレジットを獲得します。|過去 12 か月|
|月間アクティブ ユーザー数増加率 (Monthly active user growth)|25|現在の月間アクティブ ユーザー数と、13 か月前の月間アクティブ ユーザー数の比較。 月間アクティブ ユーザー数はサブスクリプション レベルでカウントされ、有料サブスクリプションのみが対象となります。 月間アクティブ ユーザー数は、毎月の終了時に計算されます。 **Customer Engagement** の場合、運用環境に必要な月間アクティブ ユーザー数のベースラインは、先進市場のパートナーでは 250 人以上、新興市場のパートナーでは 150 人以上であり、13 か月前の顧客ベース全体がポイントの対象になります。 **Finance and Operations** の場合、運用環境に必要な月間アクティブ ユーザー数のベースラインは、先進市場のパートナーでは 100 人以上、新興市場のパートナーでは 50 人以上であり、13 か月前の顧客ベース全体がポイントの対象になります。|過去 12 か月|

## <a name="customer-to-partner-association"></a>顧客とパートナーの関連付け

パートナーが顧客のテナントに属する有料サブスクリプションのクラウド ソリューション プロバイダー (CSP)、要求取引指名パートナー (CPOR)、またはデジタル指名パートナー (DPOR) の場合にのみ、パートナーは、メトリック定義の範囲内で、特定の顧客に対する新規純利益、純顧客追加数、新規大規模展開数、および月間アクティブ ユーザー数増加率のクレジットを受け取ります。

パートナーは、Dynamics 365 Online Solution Advisor (OSA) インセンティブを通じてサブスクリプション レベルで顧客との関連付けが確立されている場合、CPOR になります。

パートナーは、製品内のサブスクリプション レベルで顧客との関連付けが確立されている場合、DPOR になります。

特定のサブスクリプションに対して CPOR と DPOR の両方が存在する場合は、CPOR がサブスクリプションに関連付けられている PCI メトリックのすべてのクレジットを受け取ります。

## <a name="how-to-read-the-charts"></a>グラフを読む方法

![グラフを読む方法](images/pci2.png)








