---
title: インサイト データ定義
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ドキュメントには、さまざまなレポートとそのデータ定義が一覧表示されます。これらは、Insights ダウンロードレポートページからダウンロードできます。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 23ca20fbb2febfd4b1ea92f72fbfda5ac83d7eb6
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565510"
---
# <a name="export--data-definitions"></a>エクスポート–データ定義 

**適切なロール**: レポートビューアー |エグゼクティブレポートビューアー

## <a name="introduction"></a>はじめに 

Insights ダッシュボードの [レポートのダウンロード] ハブを使用すると、生データセットをエクスポートできます。 

次の表は、データ定義と共にダウンロードできるさまざまなレポートを示しています。 

### <a name="partner-profile-report"></a>**パートナープロファイルレポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| MPNId | Microsoft Partner Network (MPN) ID| 
| PartnerName | パートナーの名前 | 
| PGA_MPNId | パートナーグローバルアカウント MPN の識別子 | 
| PGA_PartnerName | パートナーのグローバルアカウント名 | 
| City | パートナーの市区町村の場所 | 
| Country | パートナーの国の場所 | 
| HierarchyLevel | グローバルな MPN ID と location MPN ID のどちらであるかを示します。 | 

### <a name="customer-details-report"></a>**顧客の詳細レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| CustomerName | サブスクリプションを購入した顧客の名前 | 
| CustomerTenantId | 顧客テナントの識別子 | 
| 顧客 Tpid | 上位の親顧客の識別子 | 
| 顧客セグメント | 顧客セグメント | 
| 顧客市場 | 顧客の地理的市場 | 
| 顧客の状態 | 顧客の状態 (アクティブまたは非アクティブ) | 
| Product | MPN によって顧客に販売された製品: Office 365、Dynamics 365、Enterprise Mobility and Security、Power BI、または Microsoft Azure | 
| SKU | 製品 SKU | 
| Month | 使用状況と収益が報告される月 | 
| MPNId | Microsoft Partner Network の識別子 | 
| PartnerName | パートナーの名前 | 
| PartnerLocation | パートナーの地理的な場所 | 
| PartnerAttributionType | パートナーの属性の種類 | 
| SalesChannel | 販売チャネル | 
| 空席の席 | 使用可能なシート数 | 
| RevenueUSD | 米ドルの収益 | 

### <a name="reseller-performance-report"></a>**再販業者のパフォーマンスレポート**

> [!Note]
> 収益と Azure で使用された収益 (ACR) データは、役員のレポートビューアーであるユーザーのみが利用できます。

| 列名 | データの説明 | 
| :--------- | :--------- | 
| ResellerMPNid | リセラー Microsoft Partner Network 識別子 | 
| ResellerName | リセラー名 | 
| ResellerMarket | 市場の再販業者の国 | 
| IndirectProviderMPNId | 間接プロバイダーの識別子 Microsoft Partner Network | 
| IndirectProviderName | 間接プロバイダー名 | 
| Month | 使用状況と収益が報告される月 | 
| Product | 製品名 | 
| SubscriptionID | サブスクリプションの識別子 | 
| 空席の席 | 使用可能な接続クライアント数 | 
| AssignedSeats | 割り当てられた座席数 | 
| BilledRevenueUSD | 米ドルで収益を請求する | 
| CustomerName | サブスクリプションを購入した顧客の名前 | 
| 顧客 Tpid | 上位の親顧客の識別子 | 
| 顧客セグメント | 顧客セグメント | 
| 顧客市場 | 顧客の地理的市場 | 
| ResellerStatus | 再販業者の状態 | 

### <a name="subscription-details-report"></a>**サブスクリプションの詳細レポート**

>[!Note]
>売上および ACR データは、エグゼクティブレポートビューアーのユーザーのみが使用できます。

| 列名 | データの説明 | 
| :--------- | :--------- | 
| SubscriptionId | サブスクリプションの GUID | 
| SubscriptionStartDate | サブスクリプションの開始日 | 
| SubscriptionEndDate | サブスクリプションの終了日 | 
| SubscriptionState | サブスクリプションの状態 (アクティブまたはチャーン) | 
| Month | 使用状況と収益が報告される月 | 
| IsAutoRenew | サブスクリプションが自動削除される ([はい] または [いいえ] ) かどうかを示します。 | 
| CustomerName | サブスクリプションを購入した顧客の名前 | 
| CustomerTenantId | 顧客の GUID | 
| CustomerTpid | 顧客の上位の親識別子 | 
| CustomerSegment | 顧客の市場セグメント | 
| CustomerMarket | 顧客の地理的市場 | 
| Product | パートナーによって顧客に販売された製品 | 
| SKU | 製品の SKU | 
| MPNId | Microsoft Partner Networkの ID | 
| PartnerName | パートナーの名前 | 
| PartnerLocation | パートナーの地理的な場所 | 
| PartnerAttributionType | サブスクリプションの属性の種類 | 
| SalesChannel | 販売チャネル - 直接、クラウド ソリューション プロバイダー (CSP)など | 
| AvailableSeats | 現在利用可能なシート | 
| RevenueUSD | 米国ドルでの収益 | 
| 登録 ID | サブスクリプションの登録 ID | 

### <a name="azure-usage-report"></a>**Azure 使用状況レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| SubscriptionId | サブスクリプションの GUID | 
| SubscriptionStartDate | サブスクリプションの開始日 | 
| SubscriptionEndDate | サブスクリプションの終了日 | 
| SubscriptionState | サブスクリプションの現在の状態 (Open、Closed、Active、または In Grace Period) | 
| Month | 月別に集計された日付 | 
| ServiceName | Azure サービスの名前 | 
| MeterCategory | 測定カテゴリの名前 | 
| UsageUnits | 請求サイクル中に使用されるユニット数 | 
| CustomerName | サブスクリプションを購入した顧客の名前 | 
| CustomerTenantId | 顧客のテナント ID | 
| CustomerTpid | 顧客の上位の親 ID | 
| CustomerSegment | 顧客のセグメント | 
| CustomerMarket | 顧客の地理的市場 | 
| MPNId | Microsoft Partner Networkの ID | 
| PartnerName | パートナーの名前 | 
| PartnerLocation | パートナーの地理的な国の場所 | 
| PartnerAttributionType | パートナーの属性の種類 | 
| SalesChannel | 販売のチャネル (Direct/CSP、Indirect/CSP、Direct など) | 
| ACR_USD | Azure の消費収益 (ACR) (米国ドル) | 
| 登録 ID | Azure サブスクリプションの登録 ID | 

### <a name="office-365-license-usage-report"></a>**Office 365 ライセンス使用状況レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| CustomerTenantId | 顧客のテナント ID | 
| CustomerTpid | 顧客の上位の親 ID | 
| WorkloadName | Skype for Business、Teams、Exchange Online | 
| Month | 使用状況が報告される月 | 
| PaidAvailableUnits | 利用可能な有料ユニットの数 | 
| MonthlyActiveUsers | 月間アクティブ ユーザー数 | 
| CustomerName | サブスクリプションを購入した顧客の名前 | 
| 顧客市場 | 顧客の市場の地理的な国の所在地 | 
| 顧客セグメント | 顧客セグメント | 
| MPNId | Microsoft Partner Network の識別子 | 
| PartnerName | パートナーの名前 | 
| PartnerLocation | パートナーの地理的な場所 | 
| PartnerAttributionType | パートナーの属性の種類 | 

### <a name="enterprise-mobility-license-usage-report"></a>**Enterprise Mobility のライセンス使用状況レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| CustomerTenantId | 顧客のテナント ID | 
| 顧客 Tpid | 顧客の上位の親 ID | 
| WorkloadName | Enterprise Mobility + Security (EMS) ワークロードの名前 | 
| Month | 使用状況が報告される月 | 
| Paidのユニット数 | 使用可能な有料ユニットの数 | 
| 月のアクティブユーザー | 月間アクティブユーザー数 | 
| CustomerName | サブスクリプションを購入した顧客の名前 | 
| 顧客市場 | 顧客の市場の地理的な国の所在地 | 
| 顧客セグメント | 顧客セグメント | 
| MPNId | Microsoft Partner Network の識別子 | 
| PartnerName | パートナーの名前 | 
| PartnerLocation | パートナーの地理的な場所 | 
| PartnerAttributionType | パートナーの属性の種類 | 

### <a name="dynamics-365-license-usage-report"></a>**Dynamics 365 ライセンスの使用状況レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| SubscriptionId | サブスクリプションの GUID | 
| SubscriptionStartDate | サブスクリプションの開始日 | 
| SubscriptionEndDate | サブスクリプションの終了日 | 
| SubscriptionStatus | サブスクリプションの状態 | 
| Month | 使用状況が報告される月 | 
| Revsumの名前 | リビジョン合計除算の名前 | 
| RevSumCategoryName 区分名 | リビジョン合計カテゴリの名前 | 
| SKU | 製品の SKU | 
| SKUId | 製品の SKU ID | 
| FreeVsPaidSKU | 無料または有料の SKU であるかどうかを示します | 
| SalesModel | サブスクリプションの販売に使用される販売チャネル | 
| DetailedSalesModel | サブスクリプションの詳細な販売モデル | 
| CustomerName | サブスクリプションを購入した顧客の名前 | 
| CustomerTenantId | 顧客テナントの GUID | 
| 顧客 Tpid | 顧客の上位の親の識別子 | 
| 顧客セグメント | 顧客の市場セグメント | 
| 顧客市場 | 顧客の地理的市場 | 
| MPNId | Microsoft Partner Network の識別子 | 
| PartnerName | パートナーの名前 | 
| PartnerLocation | パートナーの地理的な国の所在地 | 
| PartnerAttachType | サブスクリプションの属性の種類 | 
| 空席の席 | 現在使用可能な接続クライアント数 | 
| AssignedSeats | 現在割り当てられている接続クライアント数 | 
| アクティブシート数 | 現在のアクティブなシート | 
| Deploymentoppor氏 | 現在の展開の機会 | 
| アクティブの割合 | 現在のアクティブな使用率 (%) | 

### <a name="power-bi-license-usage-report"></a>**Power BI ライセンス使用状況レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| SubscriptionId | サブスクリプションの GUID | 
| SubscriptionStartDate | サブスクリプションの開始日 | 
| SubscriptionEndDate | サブスクリプションの終了日 | 
| SubscriptionStatus | サブスクリプションの状態 (アクティブ、非アクティブ、または猶予期間) | 
| Month | 月別に集計された日付 | 
| SKU | 製品の SKU | 
| SKUId | 製品の SKU ID | 
| FreeVsPaidSKU | 無料または有料の SKU の差別化要因 | 
| SalesModel | サブスクリプションの販売に使用される販売モデル | 
| DetailedSalesModel | サブスクリプションの詳細な販売モデル | 
| CustomerName | サブスクリプションを購入した顧客の名前 | 
| CustomerTenantId | 顧客テナントの GUID | 
| CustomerTpid | 顧客の上位の親の識別子 | 
| CustomerSegment | 顧客の市場セグメント | 
| CustomerMarket | 顧客の地理的市場 | 
| MPNId | id of Microsoft Partner Network | 
| PartnerName | パートナーの名前 | 
| PartnerLocation | パートナーの地理的な国の場所 | 
| PartnerAttachType | サブスクリプションの属性の種類 | 
| AvailableSeats | 現在利用可能なシート | 
| AssignedSeats | 現在割り当てられているシート | 
| ActiveSeats | 現在アクティブなシート | 
| DeploymentOpportunity | 現在のデプロイの機会 | 
| ActiveUsagePercent | 現在のアクティブな使用率 | 

### <a name="teams-meetings-and-calls-report"></a>**Teams の会議と通話レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| CustomerTenantId | 顧客のテナント ID | 
| CustomerTpid | 顧客の上位の親の識別子 | 
| Month | 使用状況が報告される月 | 
| サブワークロード | 使用状況が報告されるサブワークロード (会議、通話、または電話システム) | 
| 会議の数 | 会議の数 | 
| 会議の期間 | 合計会議時間 (時間) | 

### <a name="teams-monthly-usage-report"></a>**Teams の月間使用状況レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| CustomerTenantId | 顧客のテナント ID | 
| CustomerTpid | 顧客の上位の親の識別子 | 
| Month | 使用状況が報告される月 | 
| サブワークロード | 使用状況が報告されるサブワークロード (会議、通話、または電話システム) | 
| デスクトップ ユーザー | デスクトップで Teams を使用するユーザーの数 | 
| モバイル ユーザー | モバイルで Teams を使用するユーザーの数 | 
| Web ユーザー | Web 上で Teams を使用するユーザーの数 | 
| AllUpParticipants | 1 か月間の Teams の一意のユーザー数 | 

### <a name="teams-usage-3p-apps-report"></a>**Teams の使用状況 3P アプリ レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| CustomerTenantId | 顧客のテナント ID | 
| CustomerTpid | 顧客の上位の親 ID | 
| Month | 使用状況が報告される月 | 
| 3P アプリ名 | Teams アプリの名前 | 
| ユーザー数 | アプリのユーザー数 | 


### <a name="training-details-report"></a>**トレーニングの詳細レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| TrainingActivityId | トレーニングの識別子 | 
| TrainingTitle | トレーニングのタイトル | 
| TrainingType | トレーニングの種類 (認定または試験) | 
| IndividualFirstName | 顧客の名 | 
| IndividualLastName | 顧客の名 | 
| 電子メール | 顧客の個人用電子メール ID | 
| CorpEmail | 顧客の Office 電子メール ID | 
| TrainingCompletionDate | トレーニングの完了日 | 
| Month | データが報告される月 | 
| IcMCP | ユーザーが Microsoft Certified Professional (MCP) かどうかを示します | 
| MCPID | ユーザーの MCP ID | 
| MPNId | id of Microsoft Partner Network | 
| PartnerName | パートナーの名前 | 
| PartnerCityLocation | パートナーの地理的な都市の場所 | 
| PartnerCountryLocation | パートナーの地理的な国の場所 | 

### <a name="microsoft-learn-report"></a>**Microsoft Learnレポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| UserName | ユーザーの名前 | 
| UserId | ユーザーの GUID | 
| TrainingName | トレーニングの名前 | 
| TrainingType | トレーニングの種類 (モジュールまたはラーニング パス) | 
| 製品 | 学習モジュールが適用される製品 | 
| ロール | トレーニングの該当するロール | 
| CompletionDate | トレーニングの完了日 | 
| MPNId | id of Microsoft Partner Network | 
| PartnerName | パートナーの名前 | 
| Country | パートナーの地理的な国の場所 | 

### <a name="competency-summary-and-history-report"></a>**コンピテンシーの概要と履歴レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| CompetencyName | コンピテンシーの名前 | 
| CompetencyLevel | コンピテンシーのレベル (Gold または Silver) | 
| CompetencyStatus | コンピテンシーの現在の状態 (アクティブ、非アクティブ、または猶予期間) | 
| CompetencyStartDate | コンピテンシーの開始日 | 
| CompetencyEndDate | コンピテンシーの終了日 | 

### <a name="competency-performance-report"></a>**コンピテンシーパフォーマンス レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| CompetencyName | コンピテンシーの名前 | 
| CompetencyAttainmentOptionName | コンピテンシー取得オプションの名前 | 
| Month | メトリックが報告される月 | 
| MetricName | コンピテンシーに関連するメトリックの名前 | 
| MetricMonthlyContribution | メトリックの月単位の貢献 | 
| TTMAggregate | 後続の 12 か月間の集計メトリック | 
| AnniversaryYearAggregate | 現在の記念日の年の集計メトリック | 
| GoldThreshold | Gold コンピテンシーを満たすパフォーマンス要件 | 
| SilverThreshold | Silver コンピテンシーを満たすパフォーマンス要件 | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Cloud Ascent - Microsoft 365の傾向レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| MPN ID | Microsoft Partner Network ID | 
| パートナー名 | パートナーの名前 | 
| Customer ID | 顧客の識別子番号 | 
| DUNS 番号 | 傾向&スコア付けされている顧客の Dun & Bradstreet (D&B) 番号 | 
| アカウント名 | アカウントの名前 | 
| Domain | アカウントのドメイン | 
| 組織の規模 | 組織の規模 | 
| 業種 | 組織が属している業界 | 
| Vertical | Microsoft、D&B、およびその他の業界標準によって識別される、傾向のスコアを付けている顧客の垂直 | 
| 領域 | 場所の地理的領域 | 
| 子会社 | 傾向のスコアが付けられている顧客の子会社 | 
| Sales Territory | 傾向のスコアが付けられている顧客の販売区域 | 
| City | 組織の地理的都市の場所 | 
| 州 | 組織の地理的な状態の場所 | 
| 郵便番号 | 組織の郵便番号 | 
| Country | 組織の地理的な国の所在地 | 
| Segment | 市場セグメント | 
| サブセグメント | 市場の小区分 | 
| SMC の種類の概要 | SMC の種類 | 
| 上位のアンマネージ-コンピューティングベース | 上位の非管理対象ユーザー– compute | 
| 上位のアンマネージ-ユーザーベース | 上位の非管理対象顧客–ユーザー | 
| IsNonProfit 営利 | 組織が非営利であるかどうかを示します (Yes または No) | 
| リモート作業-ターゲットの Exchange Online を有効にする | アクティブな Exchange Online サブスクリプションを所有しているお客様は、Microsoft 365 にアップセル | 
| クラウドアセント傾向-+ 10 ライセンスを使用して、リモートでの作業中のオンプレミスの取得 (現在のバージョン) を有効にします | 現在オンプレミスの Office または Windows クライアントを所有しているお客様。 つまり、クライアントのバージョンは、有効期限 (EOL) のバージョンよりも後になります。 お客様には10個以上のライセンスがあります。 傾向スコアを持つ顧客。 パートナーは Microsoft 365 への変換を対象にする必要があります。 | 
| クラウドアセント傾向を使用したリモート作業オンプレミスの取得 (現在のバージョン) の有効化-<10 ライセンス | 現在のオンプレミスの Office または Windows クライアント (EOL より後のバージョン) を持つ顧客。 お客様のライセンスは10個未満です。 傾向スコアを持つ顧客。 パートナーは Microsoft 365 への変換を対象にする必要があります。 | 
| クラウドアセント傾向-+ 10 ライセンスを使用せずに、リモートでの作業中のオンプレミスの取得 (現在のバージョン) を有効にする | 現在のオンプレミスの Office または Windows クライアント (EOL より後のバージョン) を持つ顧客。 お客様には10個以上のライセンスがあります。 お客様には傾向スコアがありません。 パートナーは Microsoft 365 への変換を対象にする必要があります。 | 
| クラウドのアセント傾向を使用せずに、リモートでの作業オンプレミスの取得 (現在のバージョン) を有効にする-<10 ライセンス | 現在のオンプレミスの Office または Windows クライアント (EOL より後のバージョン) を持つ顧客。 お客様のライセンスは10個未満です。 お客様には傾向スコアがありません。 パートナーは Microsoft 365 への変換を対象にする必要があります。 | 
| クラウドアセント傾向-+ 10 ライセンスを使用したリモート作業オンプレミスの取得 (EOL バージョン) の有効化 | 旧バージョンのオンプレミスの Office または Windows クライアント (つまり、EOL バージョン以前) を所有しているお客様。 お客様には10個以上のライセンスがあります。 お客様には傾向スコアがあります。 パートナーは Microsoft 365 への変換を対象にする必要があります。 | 
| クラウドアセント傾向を使用したリモート作業オンプレミスの取得 (EOL バージョン) の有効化-<10 ライセンス | 旧バージョンのオンプレミスの Office または Windows クライアント (つまり、EOL バージョン以前) を所有しているお客様。 お客様のライセンスは10個未満です。 お客様には傾向スコアがあります。 パートナーは Microsoft 365 への変換を対象にする必要があります。 | 
| クラウドアセント傾向-+ 10 ライセンスを使用せずに、リモートでの作業中のオンプレミスの取得 (EOL バージョン) を有効にする | 現在のオンプレミスの Office または Windows クライアント (つまり、EOL バージョン以前) を所有しているお客様。 お客様には10個以上のライセンスがあります。 お客様には傾向スコアがありません。 パートナーは Microsoft 365 への変換を対象にする必要があります。 | 
| クラウドアセント傾向を使用せずに、リモートでの作業中のオンプレミスの取得 (EOL バージョン) を有効にする-<10 ライセンス | 現在のオンプレミスの Office または Windows クライアント (つまり、EOL バージョン以前) を所有しているお客様。 お客様のライセンスは10個未満です。 お客様には傾向スコアがありません。 パートナーは Microsoft 365 への変換を対象にする必要があります。 | 
| Microsoft 365 でのリモート作業-高傾向見込顧客の有効化 (Act NowithEvaluate) | Microsoft 365 の高い傾向を持つ見込み客 | 
| Microsoft 365 を使用したリモート作業の競合 (ズーム) を有効にする | ズームと Microsoft 365 があり、チームへの変換の対象となるお客様 | 
| Microsoft 365 を使用せずに、リモート作業の競合 (ズーム) を有効にする | ズームを使用した顧客、チームへの変換のターゲット | 
| Microsoft 365 E5 を対象としたコストを削減し、Microsoft 365 E3 を管理する | Microsoft 365 E3 を使用する既存の顧客、Microsoft 365 E5 のターゲット | 
| Microsoft 365 Business Premium を対象とする Microsoft 365 Business Basic および Business Standard のお客様のコストを削減し、管理します | 既存の Microsoft 365 Business Basic および Business Standard のお客様、Microsoft 365 Business Premium のターゲット | 
| 組織の生産性の変革-Surface 傾向 | 顧客が Surface の傾向を表示する | 
| M365Cluster | Microsoft 365 購入する顧客の傾向を識別します。 今すぐターゲットを作成し、クラスターを評価します。 育成をターゲットにして、現在の行動後に容量が残っていて、顧客を評価する場合にのみ、お客様を教育します。 | 
| M365Fit | ファイヤグラフィックを定義する内部および外部のデータポイント。 スコアリングでは、お客様を比較し、Microsoft のクラウド製品に適しているかどうかを確認するために、最適な小規模または中規模の企業 (Smb) に近いモデルを使用します。 Fit スコアリングは四半期ごとに更新されます。 | 
| M365Intent | ソーシャルメディアに関連するシグナルと、顧客のオンライン動作によってインテントが定義されます。 インテントスコアリングは、クラスターを定義するために適合します。 インテントスコアリングは毎月更新されます。 | 
| SurfaceCluster | 適合性とインテントの推奨事項をクラスターに統合することにより、顧客の傾向の購入を示します。 今すぐターゲットを作成し、クラスターを評価します。 育成をターゲットにして、現在の行動後に容量が残っていて、顧客を評価する場合にのみ、お客様を教育します。 | 
| SurfaceFit | ファイヤグラフィックを定義する内部および外部のデータポイント。 スコアリングでは、最適な Smb を使用して顧客を比較し、Microsoft のクラウド製品に適合しているかどうかを確認します。 Fit スコアリングは四半期ごとに更新されます。 | 
| SurfaceIntent | ソーシャルメディアに関連するシグナルと、顧客のオンライン動作によってインテントが定義されます。 インテントスコアリングは、クラスターを定義するために適合します。 インテントスコアリングは毎月更新されます。 | 
| O365Cluster | Office 365 を購入する顧客の傾向を識別します。 今すぐターゲットを作成し、クラスターを評価します。 育成をターゲットにして、現在の行動後に容量が残っていて、顧客を評価する場合にのみ、お客様を教育します。 | 
| O365Fit | ファイヤグラフィックを定義する内部および外部のデータポイント。 スコアリングでは、最適な Smb を使用して顧客を比較し、Microsoft のクラウド製品に適合しているかどうかを確認します。 Fit スコアリングは四半期ごとに更新されます。 | 
| O365Intent | ソーシャルメディアに関連するシグナルと、顧客のオンライン動作によってインテントが定義されます。 インテントスコアリングは、クラスターを定義するために適合します。 インテントスコアリングは毎月更新されます。 | 
| M365UpsellCustomer | 顧客が Microsoft 365 のアップセル傾向を表示するかどうかを識別します | 
| Google あり | 顧客が Google 製品を所有するための競争力のある信号を表示するかどうかを識別します | 
| AWS | 顧客が所有するアマゾンウェブサービス (AWS) 製品の競争力のある信号を表示するかどうかを識別します | 
| EA あり | 更新が enterprise agreement (EA) と EA サブスクリプションのどちらであるかを識別します | 
| 開いている | 更新がオープンまたはオープン値アグリーメントであるかどうかを識別します | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**クラウドのアセント-Dynamics 365 傾向レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| MPN ID | Microsoft Partner Network (MPN) ID | 
| パートナー名 | パートナーの名前 | 
| Customer ID | 顧客の id 番号 | 
| DUNS 番号 | 傾向に対してスコアを付けている顧客の Dun & Bradstreet 番号 | 
| アカウント名 | アカウントの名前 | 
| Domain | アカウントのドメイン | 
| 組織の規模 | 組織の規模 | 
| 業種 | 組織が属している業界 | 
| Vertical | Microsoft、D&B、およびその他の業界標準によって識別される、傾向のスコアを付けている顧客の垂直
| 領域 | 場所の地理的領域 | 
| 子会社 | 傾向のスコアが付けられている顧客の子会社 | 
| Sales Territory | 傾向のスコアが付けられている顧客の販売区域 | 
| City | 地理的な都市の所在地 | 
| 州 | 地理的な州の場所 | 
| 郵便番号 | 組織の郵便番号 | 
| Country | 地理的な国の所在地 | 
| Segment | 市場セグメント | 
| サブセグメント | 市場の小区分 | 
| SMC の種類の概要 | 顧客の分類: 上位の管理されていないユーザーのベースは、300人以上の従業員を対象としています。 USD10、Azure では、管理されていないコンピューティングベースの最上位は25人の従業員であり、中小企業は25人を超える従業員です。 | 
| 上位のアンマネージ-コンピューティングベース | 上位の非管理対象ユーザー– compute | 
| 上位のアンマネージ-ユーザーベース | 上位の非管理対象顧客–ユーザー | 
| IsNonProfit 営利 | 組織が非営利であるかどうかを示します (Yes または No) | 
| デジタル販売 Microsoft 365 シートサイズ >= 25 台の座席 (SalesPro 傾向 model) をアクティブ化する | Dynamics 365 を使用しないお客様。 座席サイズ:25 +。 パートナーは Dynamics 365 SalesPro のクロスセルを対象にする必要があります。 | 
| デジタル販売の有効化-Dynamics 365 SalesPro 傾向 (今すぐ動作または評価) | Dynamics 365 を使用しない傾向のお客様。 パートナーは Dynamics 365 SalesPro のターゲットにする必要があります。 | 
| 財務リスク & 不正アクセスの管理-Dynamics オンプレミスインストール Navision (Business Central 傾向 model) | オンプレミスの Navision を使用する既存の顧客。 パートナーは Dynamics 365 Business Central のターゲットにする必要があります。 | 
| 財務リスク & 不正アクセスの管理-Dynamics オンプレミスインストールベース-Dynamics AX (Dynamics 365 Finance + Operations 傾向 model) | オンプレミスの AX を使用する既存の顧客。 パートナーは Dynamics 365 Finance + 操作を対象にする必要があります。 | 
| 財務リスク & 不正アクセスの管理-Dynamics オンプレミスインストールベース-優れた Plains (Business Central 傾向 model) | オンプレミスの優れた Plains を持つ既存のお客様。 パートナーは Dynamics 365 Business Central のターゲットにする必要があります。 | 
| 財務リスク & 不正アクセスの管理-Dynamics オンプレミスインストールベース-ソロモン (Business Central 傾向 model) | オンプレミスのソロモンを使用する既存の顧客。 パートナーは Dynamics 365 Business Central のターゲットにする必要があります。 | 
| 不正アクセスのリスク & 管理-Dynamics オンプレミスインストールベース-その他 (Business Central 傾向モデル) | 既存のお客様は、以前に一覧表示されていない他のオンプレミスソリューションを使用します。 パートナーは Dynamics 365 Business Central のターゲットにする必要があります。 | 
| アジャイルビジネスプロセスの構築-Dynamics オンプレミスインストールベース-AX/GP/SL/NAV/その他 (Dynamics 365 傾向モデル) | アジャイルビジネスプロセスの構築-Dynamics オンプレミスインストールベース-AX/GP/SL/NAV/その他 (Dynamics 365 傾向モデル) | 
| アジャイルビジネスプロセスの構築-Dynamics 競合 Mendix/OutSystems/Salesforce (Dynamics 365 傾向 model) | アジャイルビジネスプロセスの構築-Dynamics 競合 Mendix/OutSystems/Salesforce (Dynamics 365 傾向 model) | 
| アジャイルビジネスプロセスの構築-Dynamics 365 Finance + Operations インストールベース | 既存の Dynamics 365 Finance + Operations のお客様。 パワーアプリを対象とするパートナー。 | 
| アジャイルビジネスプロセスの構築-Dynamics 365 Business Central インストールベース | 既存の Dynamics 365 Business Central のお客様。 パワーアプリを対象とするパートナー。 | 
| アジャイルビジネスプロセスの構築-Dynamics 365 Customer Engagement インストールベース | 既存の Dynamics 365 Customer Engagement のお客様。 パワーアプリを対象とするパートナー。 | 
| 回復力のあるサプライチェーンを構築し、Oracle または SAP ERP (エンタープライズリソースプランニング) のお客様による Dynamics 365 サプライチェーン管理として最初の Dynamics 365 ワークロードをアクティブ化する | Dynamics 365 サプライチェーン管理の対象となるお客様 | 
| 回復力のあるサプライチェーンを構築する-Dynamics 365 サプライチェーンの管理と小売、またはその両方を既存の Dynamics 365 Customer Engagement のお客様に提供する | 既存の Dynamics 365 Customer Engagement のお客様は、Dynamics 365 サプライチェーン管理をクロス販売することを目標としています。 | 
| 回復力のあるサプライチェーンの構築-Dynamics 365 サプライチェーンの管理、小売、またはコマースから Dynamics 365 のお客様への提携、Oracle または SAP への販売 | Dynamics 365 サプライチェーン管理の対象となる Oracle または SAP を持つ既存の Dynamics 365 Customer Engagement のお客様 | 
| D365BCCluster | Dynamics 365 Business Central を購入する顧客の傾向を識別します。 傾向 for Business Central をご利用のお客様は、中および小規模のカテゴリに分類されます。 今すぐターゲットを作成し、クラスターを評価します。これにより、より高い yield が生成されます。 育成をターゲットにして、現在の機能を対象としていて、顧客を評価した後でも容量が残っている場合にのみ、お客様に教育 | 
| D365BCFit | ファイヤグラフィックを定義する内部および外部のデータポイント。 スコアリングでは、最適な SMB を使用して顧客を比較し、Microsoft のクラウド製品に適しているかどうかを確認します。 Fit スコアリングは四半期ごとに更新されます。 | 
| D365BCIntent | ソーシャルメディアに関連するシグナルと、顧客のオンライン動作によってインテントが定義されます。 インテントスコアリングは、クラスターを定義するために適合します。 インテントスコアリングは毎月更新されます。 | 
| D365FOCluster | Dynamics 365 Finance および操作を購入する顧客の傾向を識別します。 財務 + 操作の傾向を表示しているお客様は、上位の管理されていないカテゴリになります。 今すぐターゲットを作成し、クラスターを評価します。これにより、より高い yield が生成されます。 育成をターゲットにして、現在の機能を対象としていて、顧客を評価した後でも容量が残っている場合にのみ、お客様に教育 | 
| D365FOFit | ファイヤグラフィックを定義する内部および外部のデータポイント。 スコアリングでは、最適な SMB を使用して顧客を比較し、Microsoft のクラウド製品に適しているかどうかを確認します。 Fit スコアリングは四半期ごとに更新されます。 | 
| D365FOIntent | ソーシャルメディアに関連するシグナルと、顧客のオンライン動作によってインテントが定義されます。 インテントスコアリングは、クラスターを定義するために適合します。 インテントスコアリングは毎月更新されます。 | 
| D365CECluster | Dynamics 365 Customer Engagement を購入する顧客の傾向を識別します。 顧客エンゲージメントのために傾向をお持ちのお客様は、中および小規模のカテゴリに分類されます。 今すぐターゲットを作成し、クラスターを評価します。これにより、より高い yield が生成されます。 育成をターゲットにして、現在の機能を対象としていて、顧客を評価した後でも容量が残っている場合にのみ、お客様に教育 | 
| D365CEFit | Dynamics 365 Customer Engagement に適していることを示します。 | 
| D365CEIntent | Dynamics 365 Customer Engagement の意図を示します | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Dynamics オンプレミス AX または CRM のお客様がオープン更新を行っているかどうかを識別します | 
| M365UpsellCustomer | 顧客が Microsoft 365 のアップセル傾向を表示するかどうかを識別します | 
| Google あり | 顧客が Google 製品を所有するための競争力のある信号を表示するかどうかを識別します | 
| AWS | 顧客が所有する AWS 製品の競争力のある信号を表示するかどうかを識別します | 
| EA あり | 更新が EA または EA サブスクリプションであるかどうかを識別します | 
| 開いている | 更新がオープンまたはオープン値アグリーメントであるかどうかを識別します | 

### <a name="cloud-ascent---azure-propensity-report"></a>**クラウドの発展-Azure 傾向レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| MPN ID | Microsoft Partner Network (MPN) ID | 
| パートナー名 | パートナーの名前 | 
| Customer ID | 顧客の id 番号 | 
| DUNS 番号 | 傾向に対してスコアを付けている顧客の Dun & Bradstreet 番号 | 
| アカウント名 | アカウントの名前 | 
| Domain | アカウントのドメイン | 
| 組織の規模 | 組織の規模 | 
| 業種 | 業種 | 
| Vertical | Microsoft、D&B、およびその他の業界標準によって識別される、傾向のスコアを付けている顧客の垂直 | 
| 領域 | 場所の地理的領域 | 
| 子会社 | 傾向のスコアが付けられている顧客の子会社 | 
| Sales Territory | 傾向のスコアが付けられている顧客の販売区域 | 
| City | 地理的な都市の所在地 | 
| 州 | 地理的な州の場所 | 
| 郵便番号 | 組織の郵便番号 | 
| Country | 地理的な国の場所 | 
| Segment | 市場セグメント | 
| サブ セグメント | 市場サブセグメント | 
| SMC の種類の概要 | SMC の種類 | 
| 上位アンマネージド - コンピューティング ベース | 上位のアンマネージド顧客 – コンピューティング | 
| 管理されていない上位 - ユーザー ベース | 管理されていない上位の顧客 - ユーザー | 
| IsNonProfit | 組織が非営利団体であるかどうかを示します (はいまたはいいえ) | 
| 移行 - EOL Windows Server - EOL Windows Server IB with Cloud Ascent propensity - 5 つ以上のライセンス | オンプレミスの Windows Server (EOL バージョン以前) の EOL を持っているお客様。 お客様は 5 つ以上のライセンスを持つ。 傾向スコアを持つ顧客。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - EOL Windows Server - EOL Windows Server IB with Cloud Ascent propensity - <5 ライセンス | オンプレミスの Windows Server (EOL バージョン以前) の EOL を持っているお客様。 顧客のライセンス数は 5 未満です。 傾向スコアを持つ顧客。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - EOL Windows Server - EOL Windows Server IB without Cloud Ascent propensity - 5 以上のライセンス | オンプレミスの Windows Server (EOL バージョン以前) の EOL を持っているお客様。 お客様には 5 つ以上のライセンスがあります。 顧客には傾向スコアが含め "ない"。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - EOL Windows Server - EOL Windows Server IB without Cloud Ascent propensity - <5 ライセンス | オンプレミスの Windows Server (EOL バージョン以前) の EOL を持っているお客様。 ライセンスが 5 つ未満です。 顧客には傾向スコアが含め "ない"。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - EOL SQL - EOL SQL Server IB と Cloud Ascent の傾向 - 5 つ以上のライセンス | オンプレミスの EOL を持つSQL Server (つまり、EOL バージョン以前) です。 お客様には 5 つ以上のライセンスがあります。 顧客は傾向スコアを持っています。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - EOL SQL - EOL SQL Server IB と Cloud Ascent の傾向 - <5 ライセンス | オンプレミスの EOL を持つSQL Server (つまり、EOL バージョン以前) です。 ライセンスが 5 つ未満です。 傾向スコアを持つ顧客。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - EOL SQL - EOL SQL Server Ib without Cloud Ascent propensity - 5 以上のライセンス | オンプレミスの EOL を持つSQL Server (つまり、EOL バージョン以前) です。 お客様は 5 つ以上のライセンスを持つ。 顧客には傾向スコアが含め "ない"。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - EOL SQL - EOL SQL Server IB (Cloud Ascent の傾向なし) - <5 ライセンス | オンプレミスの EOL を持つSQL Server (つまり、EOL バージョン以前) です。 お客様のライセンス数は 5 未満です。 顧客には傾向スコアが含め "ない"。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - オンプレミスの Windows Server - Cloud Ascent の傾向を備える現在の Windows Server IB を移行する - 5 以上のライセンス | 現在のオンプレミスの Windows Server (つまり、EOL より新しいバージョン) を持っているお客様。 お客様には 5 つ以上のライセンスがあります。 顧客は傾向スコアを持っています。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - オンプレミスの Windows Server を移行する - 現在の Windows Server IB と Cloud Ascent の傾向 - <5 ライセンス | 現在のオンプレミスの Windows Server (つまり、EOL より新しいバージョン) を持っているお客様。 お客様のライセンス数は 5 未満です。 お客様は Azure の傾向スコアを持っています。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - オンプレミスの Windows Server を移行する - Cloud Ascent の傾向のない現在の Windows Server IB - 5 以上のライセンス | 現在のオンプレミスの Windows Server (つまり、EOL より新しいバージョン) を持っているお客様。 お客様には 5 つ以上のライセンスがあります。 顧客には傾向スコアが含め "ない"。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - オンプレミスの Windows Server - Cloud Ascent の傾向のない現在の Windows Server IB の移行 - <5 ライセンス | 現在のオンプレミスの Windows Server (つまり、EOL より新しいバージョン) を持っているお客様。 お客様のライセンス数は 5 未満です。 顧客には傾向スコアが含め "ない"。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - Azure SQL または SQL 仮想マシン (VM) に移行する - Cloud Ascent の傾向を持つ現在の SQL Server IB - 5 以上のライセンス | 現在オンプレミスのサービスを利用しているSQL Server (つまり、EOL より後のバージョン) です。 お客様には 5 つ以上のライセンスがあります。 顧客は傾向スコアを持っています。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - Azure SQL または SQL VM に移行する - Cloud Ascent の傾向SQL Server IB の現在の <5 ライセンス | 現在オンプレミスのサービスを利用しているSQL Server (つまり、EOL より後のバージョン) です。 お客様のライセンス数は 5 未満です。 顧客は傾向スコアを持っています。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - Azure SQL または SQL VM に移行する - Cloud Ascent の傾向を持SQL Server IB の現在のバージョン - 5 つ以上のライセンス | 現在オンプレミスのサービスを利用しているSQL Server (つまり、EOL より後のバージョン) です。 お客様には 5 つ以上のライセンスがあります。 顧客には傾向スコアが含め "ない"。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - Azure SQL または SQL VM に移行する - Cloud Ascent の傾向のない現在SQL Server IB - <5 ライセンス | 現在オンプレミスのサービスを利用しているSQL Server (つまり、EOL より後のバージョン) です。 お客様のライセンス数は 5 未満です。 顧客には傾向スコアが含め "ない"。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - OSS - オープン ソースシェイクスピア (OSS) DB への移行 | 次のいずれかの競合製品を持つ既存の顧客: PostgreSQL、MySQL、MariaDB。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - OSS - Azure 上の Linux | Linux を使用している既存の顧客。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| 移行-SAP-SAP on Azure | SAP を使用する既存の顧客。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| 移行-Windows 仮想デスクトップ-リモートデスクトップサービス IB | アクティブな Windows リモートデスクトップサービスを持つ顧客を識別します。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| 移行-Windows 仮想デスクトップ-最新の作業を Azure/WVD にクロス販売 | Microsoft 365 を持つ顧客を識別します。 Azure は使用できません。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| 移行-VMware IB | 製品を使用した既存のお客様: VMware。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| 移行-Citrix IB | 製品を使用した既存のお客様: Citrix Systems。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| イノベーション-分析-高 Azure 傾向の Power BI IB | と Active Power BI サブスクリプションをお持ちのお客様: Power BI スタンドアロン Pro、Power BI-Azure スイート、Power BI Office スイート、Power BI スイート-Microsoft 365 | 
| GitHub での DevOps の有効化-Visual Studio/MSDN IB | アクティブな Visual Studio のバージョンを持つ顧客を識別します | 
| Windows Server Standard バージョン | お客様による Windows Server Standard 購入のバージョンを表示します | 
| Windows Server Standard ライセンス | お客様による Windows Server Standard の購入のライセンスの種類を表示します | 
| Windows Server データセンターのバージョン | 顧客によって購入された Windows データセンターのバージョンを表示します | 
| Windows Server データセンターライセンス | お客様が購入した Windows データセンターのライセンスの種類を表示します | 
| AzureFit | ファイヤグラフィックを定義する内部および外部のデータポイント。 スコアリングでは、最適な SMB を使用して顧客を比較し、Microsoft のクラウド製品に適しているかどうかを確認します。 Fit スコアリングは四半期ごとに更新されます。 | 
| AzureIntent | ソーシャルメディアに関連するシグナルと、顧客のオンライン動作によってインテントが定義されます。 インテントスコアリングは、クラスターを定義するために適合します。 インテントスコアリングは毎月更新されます。 | 
| AzureCluster | 適合性とインテントの推奨事項をクラスターに統合することで、Azure を購入する顧客の傾向を識別します。 今すぐターゲットを作成し、クラスターを評価します。これにより、より高い yield が生成されます。 育成をターゲットにして、現在の機能を対象としていて、顧客を評価した後でも容量が残っている場合にのみ、お客様に教育 | 
| WindowsServerDataCenter_HasOpenRenewal | お客様が Windows Server Datacenter の更新を開いているかどうかを識別します | 
| WindowsServerStandard_HasOpenRenewal | お客様が Windows Server Standard の更新を開いているかどうかを識別します | 
| AzureUpsellCustomer | 顧客が Azure のアップセル傾向を表示するかどうかを識別します | 
| Google あり | 顧客が Google 製品を所有するための競争力のある信号を表示するかどうかを識別します | 
| AWS | 顧客が所有する AWS 製品の競争力のある信号を表示するかどうかを識別します | 
| EA あり | 更新が EA または EA サブスクリプションであるかどうかを識別します | 
| 開いている | 更新がオープンまたはオープン値アグリーメントであるかどうかを識別します | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**クラウドのアセント-契約の更新傾向レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| MPN ID | Microsoft Partner Network ID | 
| パートナー名 | パートナーの名前 | 
| Customer ID | 顧客の id 番号 | 
| DUNS 番号 | 傾向に対してスコアを付けている顧客の Dun & Bradstreet 番号 | 
| アカウント名 | アカウントの名前 | 
| Domain | アカウントのドメイン | 
| 組織の規模 | 組織の規模 | 
| 業種 | 業種 | 
| Vertical | Microsoft、D&B、およびその他の業界標準によって識別される、傾向のスコアを付けている顧客の垂直 | 
| 領域 | 場所の地理的領域 | 
| 子会社 | 傾向のスコアが付けられている顧客の子会社 | 
| Sales Territory | 傾向のスコアが付けられている顧客の販売区域 | 
| City | 地理的な都市の所在地 | 
| 州 | 地理的な州の場所 | 
| 郵便番号 | 組織の郵便番号 | 
| Country | 地理的な国の所在地 | 
| Segment | 市場セグメント | 
| サブセグメント | 市場の小区分 | 
| SMC の種類の概要 | SMC の種類 | 
| 上位のアンマネージ-コンピューティングベース | 上位の非管理対象ユーザー– compute | 
| 上位のアンマネージ-ユーザーベース | 上位の非管理対象顧客–ユーザー | 
| IsNonProfit 営利 | 組織が非営利であるかどうかを示します (Yes または No) | 
| Google あり | 顧客が所有する AWS 製品の競争力のある信号を表示するかどうかを識別します | 
| AWS | 顧客が所有する AWS 製品の競争力のある信号を表示するかどうかを識別します | 
| Azure クラスター | Azure を購入する顧客の傾向を識別します。 今すぐターゲットを作成し、クラスターを評価します。これにより、より高い yield が生成されます。 育成をターゲットにして、現在の機能を対象としていて、顧客を評価した後でも容量が残っている場合にのみ、お客様に教育 | 
| D365 Finance + Operations クラスター | Dynamics 365 Finance および操作を購入する顧客の傾向を識別します。 財務 + 操作の傾向を表示しているお客様は、上位の管理されていないカテゴリになります。 今すぐターゲットを作成し、クラスターを評価します。これにより、より高い yield が生成されます。 育成をターゲットにして、現在の機能を対象としていて、顧客を評価した後でも容量が残っている場合にのみ、お客様に教育 | 
| D365 CE クラスター | Dynamics 365 Customer Engagement を購入する顧客の傾向を識別します。 顧客エンゲージメントのために傾向をお持ちのお客様は、中および小規模のカテゴリに分類されます。 今すぐターゲットを作成し、クラスターを評価します。これにより、より高い yield が生成されます。 育成をターゲットにして、現在の機能を対象としていて、顧客を評価した後でも容量が残っている場合にのみ、お客様に教育 | 
| D365 BC クラスター | Dynamics 365 Business Central を購入する顧客の傾向を識別します。 傾向 for Business Central をご利用のお客様は、中および小規模のカテゴリに分類されます。 今すぐターゲットを作成し、クラスターを評価します。これにより、より高い yield が生成されます。 育成をターゲットにして、現在の機能を対象としていて、顧客を評価した後でも容量が残っている場合にのみ、お客様に教育 | 
| Microsoft 365 クラスター | Microsoft 365 を購入する顧客の傾向を識別します。 今すぐターゲットを作成し、クラスターを評価します。これにより、より高い yield が生成されます。 育成をターゲットにして、現在の機能を対象としていて、顧客を評価した後でも容量が残っている場合にのみ、お客様に教育 | 
| ライセンスプログラム | 更新するライセンスプログラムの種類を識別します | 
| 契約 ID | アグリーメントの識別子 | 
| 契約終了日 | 契約の終了日 | 
| 有効期限の種類 | 有効期限の種類 | 
| 期限切れの収益 | 有効期限が切れたサブスクリプションに関連付けられている収益 | 
| EA あり | 更新が EA または EA サブスクリプションであるかどうかを識別します | 
| 開いている | 更新がオープンまたはオープン値アグリーメントであるかどうかを識別します | 
| Azure のアップセル顧客 | 顧客が Azure のアップセル傾向を表示するかどうかを識別します | 
| Microsoft 365 アップセルの顧客 | 顧客が Microsoft 365 のアップセル傾向を表示するかどうかを識別します | 
| Revsumの名前 | 更新の対象となる製品を識別します | 

## <a name="next-steps"></a>次の手順

詳細については、「 [レポートのダウンロード](pci-download-reports.md)」を参照してください。
