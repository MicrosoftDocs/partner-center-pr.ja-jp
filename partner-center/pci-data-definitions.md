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
ms.openlocfilehash: 21be5b22c453174fcb66e9409d6e26dad8e25c6b
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686349"
---
# <a name="export--data-definitions"></a>エクスポート–データ定義 

**適切なロール** 

- レポート ビューアー
- エグゼクティブ レポート ビューアー

## <a name="introduction"></a>はじめに 

Insights ダッシュボードの [レポートのダウンロード] ハブを使用すると、生データセットをエクスポートできます。 

次の表は、データ定義と共にダウンロードできるさまざまなレポートを示しています。 

### <a name="partner-profile-report"></a>**パートナープロファイルレポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| MPNId | Microsoft Partner Network の識別子 (MPN) | 
| PartnerName | パートナーの名前 | 
| PGA_MPNId | パートナーグローバルアカウント MPN の識別子 | 
| PGA_PartnerName | パートナーのグローバルアカウント名 | 
| City | パートナーの市区町村の場所 | 
| 国 | パートナーの国の場所 | 
| HierarchyLevel | グローバルな MPN ID と location MPN ID のどちらであるかを示します。 | 

### <a name="customer-details-report"></a>**顧客の詳細レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| CustomerName | サブスクリプションを購入した顧客の名前 | 
| CustomerTenantId | 顧客テナントの識別子 | 
| 顧客 Tpid | 上位の親顧客の識別子 | 
| CustomerSegment | 顧客セグメント | 
| CustomerMarket | 顧客の地理的市場 | 
| CustomerStatus | 顧客の状態 (アクティブまたは非アクティブ) | 
| 製品 | MPN によって顧客に販売された製品: O365、DYNAMICS 365、Enterprise Mobility + Security、Power BI、Microsoft Azure | 
| SKU | 製品 SKU | 
| Month | 使用状況と収益が報告される月 | 
| MPNId | id of Microsoft Partner Network | 
| PartnerName | パートナーの名前 | 
| PartnerLocation | パートナーの地理的な場所 | 
| PartnerAttributionType | パートナーの属性の種類 | 
| SalesChannel | 販売チャネル | 
| AvailableSeats | 使用可能なシート | 
| RevenueUSD | 米国ドルでの収益 | 

### <a name="reseller-performance-report"></a>**再販業者のパフォーマンスレポート**

> [!Note]
> 売上および ACR データは、エグゼクティブレポートビューアーのユーザーのみが使用できます。

| 列名 | データの説明 | 
| :--------- | :--------- | 
| ResellerMPNid | リセラー Microsoft Partner Network 識別子 | 
| ResellerName | リセラー名 | 
| ResellerMarket | 市場の再販業者の国 | 
| IndirectProviderMPNId | 間接プロバイダーの識別子 Microsoft Partner Network | 
| IndirectProviderName | 間接プロバイダー名 | 
| Month | 使用状況と収益が報告される月 | 
| 製品 | 製品名 | 
| SubscriptionID | サブスクリプションの識別子 | 
| 空席の席 | 使用可能な接続クライアント数 | 
| AssignedSeats | 割り当てられた座席数 | 
| BilledRevenueUSD | 米ドルで収益を請求する | 
| CustomerName | サブスクリプションを購入した顧客の名前 | 
| 顧客 Tpid | 上位の親顧客の識別子 | 
| CustomerSegment | 顧客セグメント | 
| CustomerMarket | 顧客の地理的市場 | 
| ResellerStatus | リセラーの状態 | 

### <a name="subscription-details-report"></a>**サブスクリプションの詳細レポート**

>[!Note]
>収益と ACR データは、エグゼクティブ レポート閲覧者であるユーザーだけが使用できます。

| 列名 | データの説明 | 
| :--------- | :--------- | 
| SubscriptionId | サブスクリプションの GUID | 
| SubscriptionStartDate | サブスクリプションの開始日 | 
| SubscriptionEndDate | サブスクリプションの終了日 | 
| SubscriptionState | サブスクリプションの状態 (アクティブまたはチャーン) | 
| Month | 使用状況と収益が報告される月 | 
| IsAutoRenew | サブスクリプションが自動削除 (はいまたはいいえ) かどうかを示します | 
| CustomerName | サブスクリプションを購入した顧客の名前 | 
| CustomerTenantId | 顧客の GUID | 
| CustomerTpid | 顧客の上位の親識別子 | 
| CustomerSegment | 顧客の市場セグメント | 
| 顧客市場 | 顧客の地理的市場 | 
| 製品 | パートナーによって顧客に販売された製品 | 
| SKU | 製品の SKU | 
| MPNId | パートナーの Microsoft Partner Network ID | 
| PartnerName | パートナーの名前 | 
| PartnerLocation | パートナーの地理的な場所 | 
| PartnerAttributionType | サブスクリプションの属性の種類 | 
| SalesChannel | 販売ダイレクト、CSP (クラウドソリューションプロバイダー) などのチャネル | 
| 空席の席 | 現在使用可能な接続クライアント数 | 
| RevenueUSD | 米ドルの収益 | 
| 登録 ID | サブスクリプションの登録 ID | 

### <a name="azure-usage-report"></a>**Azure の使用状況レポート**

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
| SalesChannel | 販売のチャネル (直接/CSP、間接/CSP、ダイレクトなど) | 
| ACR_USD | Azure で使用された収益 (ACR) (米ドル) | 
| 登録 ID | Azure サブスクリプションの登録 ID | 

### <a name="office-365-license-usage-report"></a>**Office 365 のライセンス使用状況レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| CustomerTenantId | 顧客のテナント ID | 
| 顧客 Tpid | 顧客の上位の親 ID | 
| WorkloadName | Skype for Business、Teams、Exchange Online | 
| Month | 使用状況が報告される月 | 
| Paidのユニット数 | 使用可能な有料ユニットの数 | 
| 月のアクティブユーザー | 月間アクティブユーザー数 | 
| CustomerName | サブスクリプションを購入した顧客の名前 | 
| 顧客市場 | 顧客の市場の地理的な国の所在地 | 
| 顧客セグメント | 顧客セグメント | 
| MPNId | id of Microsoft Partner Network | 
| PartnerName | パートナーの名前 | 
| PartnerLocation | パートナーの地理的な場所 | 
| PartnerAttributionType | パートナーの属性の種類 | 

### <a name="enterprise-mobility-license-usage-report"></a>**Enterprise Mobility ライセンス使用状況レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| CustomerTenantId | 顧客のテナント ID | 
| CustomerTpid | 顧客の上位の親 ID | 
| WorkloadName | EMS (Enterprise Mobility + Security) ワークロードの名前 | 
| Month | 使用状況が報告される月 | 
| PaidAvailableUnits | 利用可能な有料ユニットの数 | 
| MonthlyActiveUsers | 月間アクティブ ユーザー数 | 
| CustomerName | サブスクリプションを購入した顧客の名前 | 
| CustomerMarket | 顧客の市場の地理的な国の場所 | 
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
| FreeVsPaidSKU | 無料の SKU か有料 SKU かを示します | 
| SalesModel | サブスクリプションの販売に使用される販売チャネル | 
| DetailedSalesModel | サブスクリプションの詳細な販売モデル | 
| CustomerName | サブスクリプションを購入した顧客の名前 | 
| CustomerTenantId | 顧客テナントの GUID | 
| CustomerTpid | 顧客の上位の親識別子 | 
| CustomerSegment | 顧客の市場セグメント | 
| CustomerMarket | 顧客の地理的市場 | 
| MPNId | id of Microsoft Partner Network | 
| PartnerName | パートナーの名前 | 
| PartnerLocation | パートナーの地理的な国の場所 | 
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
| 空席の席 | 現在使用可能なシート数 | 
| AssignedSeats | 現在割り当てられている座席 | 
| アクティブシート数 | 現在のアクティブなシート | 
| Deploymentoppor氏 | 現在の展開の機会 | 
| アクティブの割合 | 現在のアクティブな使用率 (%) | 

### <a name="teams-meetings-and-calls-report"></a>**チームの会議と通話レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| CustomerTenantId | 顧客のテナント ID | 
| 顧客 Tpid | 上位の親顧客の識別子 | 
| Month | 使用状況が報告される月 | 
| サブワークロード | 使用状況が報告されるサブワークロード (会議、通話、または電話システム) | 
| 会議数 | 会議の数 | 
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
| 3P アプリケーション名 | Teams アプリの名前 | 
| ユーザー数 | アプリのユーザー数 | 


### <a name="training-details-report"></a>**トレーニングの詳細レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| TrainingActivityId | トレーニングの識別子 | 
| TrainingTitle | トレーニングのタイトル | 
| TrainingType | トレーニングの種類 (認定または試験) | 
| 個別 Alfirstname | 顧客の名 | 
| 個性 Allastname | 顧客の姓 | 
| 電子メール | お客様の個人の電子メール ID | 
| CorpEmail | 顧客の会社の電子メール ID | 
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
| 補完日 | トレーニングの完了日 | 
| MPNId | Microsoft Partner Network の識別子 | 
| PartnerName | パートナーの名前 | 
| 国 | パートナーの地理的な国の所在地 | 

### <a name="competency-summary-and-history-report"></a>**コンピテンシーの概要と履歴レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| CompetencyName | コンピテンシーの名前 | 
| CompetencyLevel | コンピテンシーのレベル (Gold またはシルバー) | 
| CompetencyStatus | コンピテンシーの現在の状態 (アクティブ、非アクティブ、または猶予期間) | 
| CompetencyStartDate | コンピテンシーの開始日 | 
| CompetencyEndDate | コンピテンシーの終了日 | 

### <a name="competency-performance-report"></a>**コンピテンシーのパフォーマンスレポート**

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
| State | 組織の地理的な状態の場所 | 
| 郵便番号 | 組織の郵便番号 | 
| 国 | 組織の地理的な国の所在地 | 
| Segment | 市場セグメント | 
| サブセグメント | 市場の小区分 | 
| SMC の種類の概要 | SMC の種類 | 
| 上位のアンマネージ-コンピューティングベース | 上位の非管理対象ユーザー– compute | 
| 上位のアンマネージ-ユーザーベース | 管理されていない上位の顧客 - ユーザー | 
| IsNonProfit | 組織が非営利団体であるかどうかを示します (はいまたはいいえ) | 
| リモート作業を有効にする - Exchange Online をターゲットにする | アクティブな Exchange Online サブスクリプションをお持ちのお客様は、サブスクリプションにアップMicrosoft 365 | 
| リモート作業を有効にする - Cloud Ascent の傾向を使用したオンプレミスの取得 (現在のバージョン) - +10 ライセンス | 現在オンプレミスの Office または Windows クライアントを持っているお客様。 つまり、クライアント のバージョンは、End of Life (EOL) バージョンより後です。 お客様は 10 以上のライセンスを持つ。 傾向スコアを持つ顧客。 パートナーは、パートナーからパートナーへの変換をMicrosoft 365。 | 
| リモート作業を有効にする - Cloud Ascent の傾向を使用したオンプレミスの取得 (現在のバージョン) - <10 ライセンス | 現在のオンプレミスの Office または Windows クライアント (つまり、EOL より新しいバージョン) を持っているお客様。 お客様のライセンス数は 10 未満です。 傾向スコアを持つ顧客。 パートナーは、パートナーからパートナーへの変換をMicrosoft 365。 | 
| リモート作業を有効にする - クラウドアセントの傾向がないオンプレミスの取得 (現在のバージョン) - +10 ライセンス | 現在のオンプレミスの Office または Windows クライアント (つまり、EOL より新しいバージョン) を持っているお客様。 お客様は 10 以上のライセンスを持つ。 顧客には傾向スコアが含め "ない"。 パートナーは Microsoft 365 への変換を対象にする必要があります。 | 
| クラウドのアセント傾向を使用せずに、リモートでの作業オンプレミスの取得 (現在のバージョン) を有効にする-<10 ライセンス | 現在のオンプレミスの Office または Windows クライアント (EOL より後のバージョン) を持つ顧客。 お客様のライセンスは10個未満です。 お客様には傾向スコアがありません。 パートナーは Microsoft 365 への変換を対象にする必要があります。 | 
| クラウドアセント傾向-+ 10 ライセンスを使用したリモート作業オンプレミスの取得 (EOL バージョン) の有効化 | 旧バージョンのオンプレミスの Office または Windows クライアント (つまり、EOL バージョン以前) を所有しているお客様。 お客様には10個以上のライセンスがあります。 お客様には傾向スコアがあります。 パートナーは Microsoft 365 への変換を対象にする必要があります。 | 
| クラウドアセント傾向を使用したリモート作業オンプレミスの取得 (EOL バージョン) の有効化-<10 ライセンス | 旧バージョンのオンプレミスの Office または Windows クライアント (つまり、EOL バージョン以前) を所有しているお客様。 お客様のライセンスは10個未満です。 お客様には傾向スコアがあります。 パートナーは Microsoft 365 への変換を対象にする必要があります。 | 
| クラウドアセント傾向-+ 10 ライセンスを使用せずに、リモートでの作業中のオンプレミスの取得 (EOL バージョン) を有効にする | 現在のオンプレミスの Office または Windows クライアント (つまり、EOL バージョン以前) を所有しているお客様。 お客様には10個以上のライセンスがあります。 お客様には傾向スコアがありません。 パートナーは、パートナーからパートナーへの変換をMicrosoft 365。 | 
| リモート作業を有効にする - クラウドアセントの傾向がないオンプレミスの取得 (EOL バージョン) - <10 ライセンス | 現在のオンプレミスの Office または Windows クライアント (つまり、EOL バージョン以前) を持っているお客様。 お客様のライセンス数は 10 未満です。 顧客には傾向スコアが含め "ない"。 パートナーは、パートナーからパートナーへの変換をMicrosoft 365。 | 
| リモート作業を有効にする - アプリケーションの高い傾向のMicrosoft 365 (Act NowithEvaluate) | 顧客に対する傾向が高い見込み顧客Microsoft 365 | 
| リモート作業を有効にする - アプリと競合する (ズーム) Microsoft 365 | Zoom と Microsoft 365、Teams への変換をターゲットとする顧客 | 
| リモート作業を有効にする - 競合 (ズーム) をMicrosoft 365 | Zoom を使用しているお客様(Teams への変換のターゲット) | 
| コストの削減と管理 - E3 Microsoft 365 E5 の対象Microsoft 365 E3 | E3 を使用している既存Microsoft 365、E5 のターゲットMicrosoft 365。 | 
| コストの削減と管理 - Microsoft 365 Business Premium を対象とする Business Basic および Business Standard Microsoft 365顧客 | 既存の Microsoft 365 Business Basic および Business Standard のお客様、Microsoft 365 Business Premium のターゲット | 
| 組織の生産性の変革 - 表面的傾向 | 顧客が Surface の傾向を示す | 
| M365Cluster | 顧客が顧客の購入傾向を識別Microsoft 365。 今すぐターゲットを作成し、クラスターを評価します。 育成をターゲットにして、現在の行動後に容量が残っていて、顧客を評価する場合にのみ、お客様を教育します。 | 
| M365Fit | ファイヤグラフィックを定義する内部および外部のデータポイント。 スコアリングでは、お客様を比較し、Microsoft のクラウド製品に適しているかどうかを確認するために、最適な小規模または中規模の企業 (Smb) に近いモデルを使用します。 Fit スコアリングは四半期ごとに更新されます。 | 
| M365Intent | ソーシャルメディアに関連するシグナルと、顧客のオンライン動作によってインテントが定義されます。 インテントスコアリングは、クラスターを定義するために適合します。 インテントスコアリングは毎月更新されます。 | 
| SurfaceCluster | 適合性とインテントの推奨事項をクラスターに統合することにより、顧客の傾向の購入を示します。 今すぐターゲットを作成し、クラスターを評価します。 育成をターゲットにして、現在の行動後に容量が残っていて、顧客を評価する場合にのみ、お客様を教育します。 | 
| SurfaceFit | ファイヤグラフィックを定義する内部および外部のデータポイント。 スコアリングでは、最適な Smb を使用して顧客を比較し、Microsoft のクラウド製品に適合しているかどうかを確認します。 Fit スコアリングは四半期ごとに更新されます。 | 
| SurfaceIntent | ソーシャルメディアに関連するシグナルと、顧客のオンライン動作によってインテントが定義されます。 意図スコアリングは、クラスターを定義するために Fit にオーバーレイされます。 意図のスコアリングは毎月更新されます。 | 
| O365Cluster | Office 365 を購入する顧客の傾向を識別します。 [今すぐ実行する] と [クラスターの評価] を選択すると、より高い収益が得られるためです。 [今すぐ行動] と [顧客を評価する] が対象の後に容量がまだ存在する場合にのみ、顧客を対象にし、顧客を教育します。 | 
| O365Fit | 企業図を定義する内部および外部のデータ ポイント。 適合スコアリングでは、類似モデルを最適な SMB に使用して、顧客を比較し、Microsoft クラウド製品に適合する可能性が高いかどうかを確認します。 Fit スコアリングは四半期ごとに更新されます。 | 
| O365Intent | ソーシャル メディアと顧客のオンライン動作に関連するシグナルは、意図を定義します。 意図スコアリングは、クラスターを定義するために Fit にオーバーレイされます。 意図のスコアリングは毎月更新されます。 | 
| M365UpsellCustomer | 顧客が顧客に対するアップセルの傾向を示Microsoft 365 | 
| Google を持つ | 顧客が Google 製品を所有する競合シグナルを表示するかどうかを識別します | 
| AWS を持つ | 顧客が顧客 (AWS) 製品を所有アマゾン ウェブ サービスシグナルを表示するかどうかを識別します | 
| EA あり | 更新が enterprise agreement (EA) と EA サブスクリプションのどちらであるかを識別します | 
| 開いている | 更新がオープンまたはオープン値アグリーメントであるかどうかを識別します | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**クラウドのアセント-Dynamics 365 傾向レポート**

| 列名 | データの説明 | 
| :--------- | :--------- | 
| MPN ID | Microsoft Partner Network ID | 
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
| State | 地理的な州の場所 | 
| 郵便番号 | 組織の郵便番号 | 
| 国 | 地理的な国の場所 | 
| Segment | 市場セグメント | 
| サブ セグメント | 市場サブセグメント | 
| SMC の種類の概要 | 顧客の分類: 上位のアンマネージド ユーザー ベースは 300 以上の従業員を持つ顧客、上位のアンマネージド コンピューティング ベースは Azure 3 年間で 10,000 米ドルの潜在顧客、中規模の企業は従業員が 25 人以上の顧客、小規模企業は従業員が 25 人未満の顧客です。 | 
| 上位アンマネージド - コンピューティング ベース | 上位のアンマネージド顧客 – コンピューティング | 
| 管理されていない上位 - ユーザー ベース | 管理されていない上位の顧客 - ユーザー | 
| IsNonProfit | 組織が非営利団体であるかどうかを示します (はいまたはいいえ) | 
| デジタル販売のアクティブ化 - Microsoft 365 - シート サイズ >= 25 シート (SalesPro 傾向モデル) | Dynamics 365 を使用しないお客様。 シートサイズ: 25 以上。 パートナーは Dynamics 365 SalesPro のクロス販売を対象とする必要があります。 | 
| デジタル販売のアクティブ化 - Dynamics 365 SalesPro の傾向 (今すぐ実行または評価) | Dynamics 365 を使用しない高い傾向の顧客。 パートナーは Dynamics 365 SalesPro を対象とする必要があります。 | 
| 財務リスク & 不正アクセスの管理-Dynamics オンプレミスインストール Navision (Business Central 傾向 model) | オンプレミスの Navision を使用する既存の顧客。 パートナーは Dynamics 365 Business Central のターゲットにする必要があります。 | 
| 財務リスク & 不正アクセスの管理-Dynamics オンプレミスインストールベース-Dynamics AX (Dynamics 365 Finance + Operations 傾向 model) | オンプレミスの AX を使用する既存の顧客。 パートナーは Dynamics 365 Finance + 操作を対象にする必要があります。 | 
| 財務リスク & 不正アクセスの管理-Dynamics オンプレミスインストールベース-優れた Plains (Business Central 傾向 model) | オンプレミスの優れた Plains を持つ既存のお客様。 パートナーは Dynamics 365 Business Central のターゲットにする必要があります。 | 
| 財務リスク & 不正アクセスの管理-Dynamics オンプレミスインストールベース-ソロモン (Business Central 傾向 model) | オンプレミスのソロモンを使用する既存の顧客。 パートナーは Dynamics 365 Business Central のターゲットにする必要があります。 | 
| 不正アクセスのリスク & 管理-Dynamics オンプレミスインストールベース-その他 (Business Central 傾向モデル) | 既存のお客様は、以前に一覧表示されていない他のオンプレミスソリューションを使用します。 パートナーは Dynamics 365 Business Central のターゲットにする必要があります。 | 
| アジャイルビジネスプロセスの構築-Dynamics オンプレミスインストールベース-AX/GP/SL/NAV/その他 (Dynamics 365 傾向モデル) | アジャイルビジネスプロセスの構築-Dynamics オンプレミスインストールベース-AX/GP/SL/NAV/その他 (Dynamics 365 傾向モデル) | 
| アジャイルビジネスプロセスの構築-Dynamics 競合 Mendix/OutSystems/Salesforce (Dynamics 365 傾向 model) | アジャイルビジネスプロセスの構築-Dynamics 競合 Mendix/OutSystems/Salesforce (Dynamics 365 傾向 model) | 
| アジャイルビジネスプロセスの構築-Dynamics 365 Finance + Operations インストールベース | 既存の Dynamics 365 Finance + Operations のお客様。 パートナーとターゲット Power Apps。 | 
| アジャイル ビジネス プロセスの構築 - Dynamics 365 Business Central のインストール ベース | Dynamics 365 Business Central の既存のお客様。 パートナーとターゲット Power Apps。 | 
| アジャイル ビジネス プロセスの構築 - Dynamics 365 Customer Engagement インストール ベース | 既存の Dynamics 365 Customer Engagement のお客様。 パートナーとターゲット Power Apps。 | 
| 回復力のあるサプライ チェーンを構築する - Windows と Dynamics 365 の最初のワークロードを、Oracle 以外または SAP ERP (エンタープライズ リソースプランニング) のお客様と Dynamics 365 Supply Chain Management としてアクティブ化する | Dynamics 365 Supply Chain Management の対象顧客 | 
| 回復力のあるサプライ チェーンの構築 - Dynamics 365 Supply Chain Management または Retail または Commerce を既存の Dynamics 365 Customer Engagement のお客様にクロス販売します | 既存の Dynamics 365 Customer Engagement のお客様は、Dynamics 365 サプライ チェーン管理のクロス販売をターゲットにしています。 | 
| 回復力のあるサプライ チェーンの構築 - Dynamics 365 Supply Chain Management または Retail または Commerce を Dynamics 365 Customer Engagement および Oracle または SAP にクロス販売する | Dynamics 365 Supply Chain Management を対象とする Oracle または SAP を使用する既存の Dynamics 365 Customer Engagement のお客様 | 
| D365BCCluster | Dynamics 365 Business Central を購入する顧客の傾向を識別します。 Business Central の傾向を示すお客様は、中と小のカテゴリに分類されます。 Target Act Now および Evaluate クラスターは、より高い収益を生成します。 [今すぐ行動] と [顧客の評価] をターゲットにした後に容量がまだある場合にのみ、顧客を対象にし、顧客を教育します。 | 
| D365BCFit | ファイヤグラフィックを定義する内部および外部のデータポイント。 スコアリングでは、最適な SMB を使用して顧客を比較し、Microsoft のクラウド製品に適しているかどうかを確認します。 Fit スコアリングは四半期ごとに更新されます。 | 
| D365BCIntent | ソーシャルメディアに関連するシグナルと、顧客のオンライン動作によってインテントが定義されます。 インテントスコアリングは、クラスターを定義するために適合します。 インテントスコアリングは毎月更新されます。 | 
| D365FOCluster | Dynamics 365 Finance および操作を購入する顧客の傾向を識別します。 財務 + 操作の傾向を表示しているお客様は、上位の管理されていないカテゴリになります。 今すぐターゲットを作成し、クラスターを評価します。これにより、より高い yield が生成されます。 育成をターゲットにして、現在の機能を対象としていて、顧客を評価した後でも容量が残っている場合にのみ、お客様に教育 | 
| D365FOFit | ファイヤグラフィックを定義する内部および外部のデータポイント。 スコアリングでは、最適な SMB を使用して顧客を比較し、Microsoft のクラウド製品に適しているかどうかを確認します。 Fit スコアリングは四半期ごとに更新されます。 | 
| D365FOIntent | ソーシャルメディアに関連するシグナルと、顧客のオンライン動作によってインテントが定義されます。 インテントスコアリングは、クラスターを定義するために適合します。 インテントスコアリングは毎月更新されます。 | 
| D365CECluster | Dynamics 365 Customer Engagement を購入する顧客の傾向を識別します。 Customer Engagement の傾向を示す顧客は、中と小のカテゴリに分類されます。 Target Act Now および Evaluate クラスターは、より高い収益を生成します。 [今すぐ行動] と [顧客の評価] をターゲットにした後に容量がまだある場合にのみ、顧客を対象にし、顧客を教育します。 | 
| D365CEFit | Dynamics 365 Customer Engagement に適合を示します | 
| D365CEIntent | Dynamics 365 Customer Engagement の意図を示します | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | 顧客が Dynamics オンプレミス AX または CRM のオープン更新を行ったかどうかを識別します | 
| M365UpsellCustomer | 顧客が顧客に対するアップセルの傾向を示Microsoft 365 | 
| Google を持つ | 顧客が Google 製品を所有する競合シグナルを表示するかどうかを識別します | 
| AWS を持つ | 顧客が AWS 製品を所有する競合シグナルを表示するかどうかを識別します | 
| EA を持つ | 更新が EA サブスクリプションか EA サブスクリプションかを識別します | 
| 開いている | 更新がオープンまたはオープン値アグリーメントであるかどうかを識別します | 

### <a name="cloud-ascent---azure-propensity-report"></a>**クラウドの発展-Azure 傾向レポート**

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
| State | 地理的な州の場所 | 
| 郵便番号 | 組織の郵便番号 | 
| 国 | 地理的な国の所在地 | 
| Segment | 市場セグメント | 
| サブセグメント | 市場サブセグメント | 
| SMC の種類の概要 | SMC の種類 | 
| 上位アンマネージド - コンピューティング ベース | 上位のアンマネージド顧客 – コンピューティング | 
| 管理されていない上位 - ユーザー ベース | 管理されていない上位の顧客 - ユーザー | 
| IsNonProfit | 組織が非営利団体であるかどうかを示します (はいまたはいいえ) | 
| 移行 - EOL Windows Server - EOL Windows Server IB with Cloud Ascent propensity - 5 つ以上のライセンス | オンプレミスの Windows Server (EOL バージョン以前) の EOL を持っているお客様。 お客様は 5 つ以上のライセンスを持つ。 傾向スコアを持つ顧客。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - EOL Windows Server - EOL Windows Server IB with Cloud Ascent propensity - <5 ライセンス | オンプレミスの Windows Server (EOL バージョン以前) の EOL を持っているお客様。 顧客のライセンス数は 5 未満です。 傾向スコアを持つ顧客。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - EOL Windows Server - EOL Windows Server IB without Cloud Ascent propensity - 5 以上のライセンス | プレミスの Windows Server (eol バージョンまたはそれ以前のバージョン) を持つ顧客。 お客様は5ライセンスを超えています。 お客様には傾向スコアがありません。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| 移行-EOL Windows Server-EOL Windows Server IB (クラウドアセント傾向なし)-<5 ライセンス | プレミスの Windows Server (eol バージョンまたはそれ以前のバージョン) を持つ顧客。 のライセンス数は5未満です。 お客様には傾向スコアがありません。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| クラウドアセント傾向-5 + ライセンスを使用して、EOL SQL Server IB を移行する | プレミスの SQL Server (EOL バージョン以前) を所有しているお客様。 お客様には5つ以上のライセンスがあります。 お客様には傾向スコアがあります。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| クラウドアセント傾向を使用した EOL SQL Server IB の移行-<5 ライセンス | プレミスの SQL Server (EOL バージョン以前) を所有しているお客様。 のライセンス数は5未満です。 傾向スコアを持つ顧客。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| クラウドアセント傾向を使用せずに、EOL SQL Server IB を移行する-5 + ライセンス | オンプレミスの EOL を持つSQL Server (つまり、EOL バージョン以前) です。 お客様は 5 つ以上のライセンスを持つ。 顧客には傾向スコアが含め "ない"。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - EOL SQL - EOL SQL Server IB (Cloud Ascent の傾向なし) - <5 ライセンス | オンプレミスの EOL を持つSQL Server (つまり、EOL バージョン以前) です。 お客様のライセンス数は 5 未満です。 顧客には傾向スコアが含め "ない"。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - オンプレミスの Windows Server - Cloud Ascent の傾向を備える現在の Windows Server IB を移行する - 5 以上のライセンス | 現在のオンプレミスの Windows Server (つまり、EOL より新しいバージョン) を持っているお客様。 お客様には 5 つ以上のライセンスがあります。 顧客は傾向スコアを持っています。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - オンプレミスの Windows Server を移行する - 現在の Windows Server IB と Cloud Ascent の傾向 - <5 ライセンス | 現在のオンプレミスの Windows Server (つまり、EOL より新しいバージョン) を持っているお客様。 お客様のライセンス数は 5 未満です。 お客様は Azure の傾向スコアを持っています。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - オンプレミスの Windows Server を移行する - Cloud Ascent の傾向のない現在の Windows Server IB - 5 以上のライセンス | 現在オンプレミスの Windows Server (EOL よりも後のバージョン) を所有しているお客様。 お客様には5つ以上のライセンスがあります。 お客様には傾向スコアがありません。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| 移行-オンプレミスの Windows Server-クラウドのアセントを使用しない最新の Windows Server IB 傾向-<5 ライセンス | 現在オンプレミスの Windows Server (EOL よりも後のバージョン) を所有しているお客様。 お客様のライセンス数は5未満です。 お客様には傾向スコアがありません。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| 移行-Azure SQL または SQL 仮想マシン (Vm) への移行-現在の SQL Server IB と Cloud アセント傾向-5 + ライセンス | 現在のオンプレミス SQL Server (EOL より後のバージョン) を持つ顧客。 お客様には5つ以上のライセンスがあります。 お客様には傾向スコアがあります。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| 移行-Azure SQL または SQL Vm への移行-現在 SQL Server IB とクラウドアセント傾向-<5 ライセンス | 現在のオンプレミス SQL Server (EOL より後のバージョン) を持つ顧客。 お客様のライセンス数は5未満です。 お客様には傾向スコアがあります。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| 移行-Azure SQL または SQL Vm への移行-クラウドアセント傾向を使用しない現在 SQL Server IB-5 + ライセンス | 現在オンプレミスのサービスを利用しているSQL Server (つまり、EOL より後のバージョン) です。 お客様には 5 つ以上のライセンスがあります。 顧客には傾向スコアが含め "ない"。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - Azure SQL または SQL VM に移行する - Cloud Ascent の傾向のない現在SQL Server IB - <5 ライセンス | 現在オンプレミスのサービスを利用しているSQL Server (つまり、EOL より後のバージョン) です。 お客様のライセンス数は 5 未満です。 顧客には傾向スコアが含め "ない"。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - OSS - オープン ソースシェイクスピア (OSS) DB への移行 | 次のいずれかの競合製品を持つ既存の顧客: PostgreSQL、MySQL、MariaDB。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - OSS - Azure 上の Linux | Linux を使用している既存の顧客。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - SAP - SAP on Azure | SAP を使用している既存の顧客。 パートナーは、この顧客を Azure への移行対象とする必要があります。 | 
| 移行 - Windows Virtual Desktop - IB リモート デスクトップ サービス IB | アクティブな Windows デバイスを持つリモート デスクトップ サービス。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| 移行-Windows 仮想デスクトップ-最新の作業を Azure/WVD にクロス販売 | Microsoft 365 を持つ顧客を識別します。 Azure は使用できません。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| 移行-VMware IB | 製品を使用した既存のお客様: VMware。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| 移行-Citrix IB | 製品を使用した既存のお客様: Citrix Systems。 パートナーは、Azure への移行のためにこの顧客をターゲットとする必要があります。 | 
| イノベーション-分析-高 Azure 傾向の Power BI IB | と Active Power BI サブスクリプションをお持ちのお客様: Power BI スタンドアロン Pro、Power BI-Azure スイート、Power BI Office スイート、Power BI スイート-Microsoft 365 | 
| GitHub での DevOps の有効化-Visual Studio/MSDN IB | アクティブな Visual Studio のバージョンを持つ顧客を識別します | 
| Windows Server Standard バージョン | お客様による Windows Server Standard 購入のバージョンを表示します | 
| Windows Server Standard ライセンス | お客様による Windows Server Standard の購入のライセンスの種類を表示します | 
| Windows Server データセンターのバージョン | 顧客によって購入された Windows データセンターのバージョンを表示します | 
| Windows Server データ センター ライセンス | 顧客による Windows データ センターの購入のライセンスの種類を表示します | 
| AzureFit | 企業図を定義する内部および外部のデータ ポイント。 適合スコアリングでは、類似モデルを最適な SMB と使用して、顧客を比較し、Microsoft クラウド製品に適合する可能性が高いかどうかを確認します。 Fit スコアリングは四半期ごとに更新されます。 | 
| AzureIntent | ソーシャル メディアと顧客のオンライン動作に関連するシグナルは、意図を定義します。 意図スコアリングは、クラスターを定義するために Fit にオーバーレイされます。 意図のスコアリングは毎月更新されます。 | 
| AzureCluster | Fit と Intent の推奨事項をクラスターに統合することで、Azure を購入する顧客の傾向を識別します。 Target Act Now および Evaluate クラスターは、より高い収益を生成します。 [今すぐ行動] と [顧客の評価] をターゲットにした後に容量がまだある場合にのみ、顧客を対象にし、顧客を教育します。 | 
| WindowsServerDataCenter_HasOpenRenewal | 顧客が Windows Server データセンターのオープン更新を行ったかどうかを識別します | 
| WindowsServerStandard_HasOpenRenewal | 顧客が Windows Server Standard のオープン更新を行ったかどうかを識別します | 
| AzureUpsellCustomer | 顧客が Azure のアップセルの傾向を示すかどうかを識別します | 
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
| Sales Territory | 傾向についてスコア付けされている顧客の販売地域 | 
| City | 地理的な都市の場所 | 
| State | 地理的な状態の場所 | 
| 郵便番号 | 組織の郵便番号 | 
| 国 | 地理的な国の場所 | 
| Segment | 市場セグメント | 
| サブ セグメント | 市場サブセグメント | 
| SMC の種類の概要 | SMC の種類 | 
| 上位アンマネージド - コンピューティング ベース | 上位のアンマネージド顧客 – コンピューティング | 
| 管理されていない上位 - ユーザー ベース | 管理されていない上位の顧客 - ユーザー | 
| IsNonProfit | 組織が非営利団体であるかどうかを示します (はいまたはいいえ) | 
| Google を持つ | 顧客が AWS 製品を所有する競合シグナルを表示するかどうかを識別します | 
| AWS を持つ | 顧客が AWS 製品を所有する競合シグナルを表示するかどうかを識別します | 
| Azure クラスター | Azure を購入する顧客の傾向を識別します。 今すぐターゲットを作成し、クラスターを評価します。これにより、より高い yield が生成されます。 育成をターゲットにして、現在の機能を対象としていて、顧客を評価した後でも容量が残っている場合にのみ、お客様に教育 | 
| D365 Finance + Operations クラスター | Dynamics 365 Finance および操作を購入する顧客の傾向を識別します。 財務 + 操作の傾向を表示しているお客様は、上位の管理されていないカテゴリになります。 今すぐターゲットを作成し、クラスターを評価します。これにより、より高い yield が生成されます。 育成をターゲットにして、現在の機能を対象としていて、顧客を評価した後でも容量が残っている場合にのみ、お客様に教育 | 
| D365 CE クラスター | Dynamics 365 Customer Engagement を購入する顧客の傾向を識別します。 顧客エンゲージメントのために傾向をお持ちのお客様は、中および小規模のカテゴリに分類されます。 今すぐターゲットを作成し、クラスターを評価します。これにより、より高い yield が生成されます。 育成をターゲットにして、現在の機能を対象としていて、顧客を評価した後でも容量が残っている場合にのみ、お客様に教育 | 
| D365 BC クラスター | Dynamics 365 Business Central を購入する顧客の傾向を識別します。 傾向 for Business Central をご利用のお客様は、中および小規模のカテゴリに分類されます。 今すぐターゲットを作成し、クラスターを評価します。これにより、より高い yield が生成されます。 育成をターゲットにして、現在の機能を対象としていて、顧客を評価した後でも容量が残っている場合にのみ、お客様に教育 | 
| Microsoft 365 クラスター | 顧客が顧客の購入傾向を識別Microsoft 365。 Target Act Now および Evaluate クラスターは、より高い収益を生成します。 [今すぐ行動] と [顧客の評価] をターゲットにした後に容量がまだある場合にのみ、顧客を対象にし、顧客を教育します。 | 
| ライセンス プログラム | 更新のライセンス プログラムの種類を識別します | 
| 契約 ID | 契約の識別子 | 
| 契約終了日 | 契約の終了日 | 
| 有効期限の種類 | 有効期限の種類 | 
| 期限切れの収益 | 期限切れのサブスクリプションに関連する収益 | 
| EA を持つ | 更新が EA サブスクリプションか EA サブスクリプションかを識別します | 
| 開いている | 更新がオープンまたはオープン値の契約かどうかを識別します | 
| Azure Upsell のお客様 | 顧客が Azure のアップセルの傾向を示すかどうかを識別します | 
| Microsoft 365 Upsell のお客様 | 顧客が顧客に対するアップセルの傾向を示Microsoft 365 | 
| RevSumDivisionName | 更新を行う製品を識別します | 

## <a name="next-steps"></a>次のステップ

詳細については、「 [レポートのダウンロード](pci-download-reports.md)」を参照してください。
