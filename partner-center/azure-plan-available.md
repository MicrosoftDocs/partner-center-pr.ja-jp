---
title: Azure CSP で使用可能な Azure サービス | パートナー センター
ms.topic: article
ms.date: 03/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: このセクションでは、Azure クラウド ソリューション プロバイダー (CSP) プログラムで使用できない Azure サービスについて説明します。
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: a86d66c3f7a799145d1f5a9bb3561a459e699f97
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2020
ms.locfileid: "79024096"
---
# <a name="available-azure-services-in-azure-csp"></a>Azure CSP で利用可能な Azure サービス

**適切なロール**

- 管理エージェント
- 課金管理者
- グローバル管理者
- ヘルプデスク エージェント
- 販売代理店
- ユーザー管理の管理者

## <a name="available-azure-services-in-azure-csp"></a>Azure CSP で利用可能な Azure サービス

このセクションでは、Azure クラウド ソリューション プロバイダー (CSP) プログラムで使用できない Azure サービスについて説明します。 また、ナショナル クラウド [Microsoft Azure Germany](https://azure.microsoft.com/overview/clouds/germany/) および [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/) のサービスの可用性についても説明します。

>[!Note]
>[Azure China]( https://www.azure.cn/) は、Azure CSP プログラムでは使用できません。

### <a name="global-cloud"></a>グローバル クラウド 

Azure Resource Manager モデルに基づくすべてのサービスは、CSP プログラムで利用できます。  Azure Resource Manager 以外のサービスは、CSP プログラムでは利用できません。  

### <a name="csp-specific-service-configurations"></a>CSP 固有のサービス構成

次のサービスでは、CSP に特別な構成が必要です。

- [StorSimple](https://docs.microsoft.com/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-csp)

- [Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx) 

- [Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/)  顧客のテナントのユーザーのみが、その Time Series Insights 環境内のデータにアクセスできます。 パートナーは、既定で顧客の Time Series Insights 環境を管理できますが、そこにあるデータへのアクセスを必要とする場合は顧客テナントに追加される必要があります。 

### <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

Visual Studio Marketplace から以下に記載された項目を購入できるようになりました (サードパーティの拡張機能以外)。

- [Azure DevOps](https://www.visualstudio.com/team-services/) 

- [Visual Studio サブスクリプション](https://www.visualstudio.com/subscriptions/)

- [Xamarin University トレーニング](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

円滑に使用を開始できるように、CSP での [Azure DevOps のセットアップ、購入、管理](https://docs.microsoft.com/vsts/billing/csp/set-up-csp-customer)に関するビデオとドキュメントをご用意しました。

### <a name="azure-marketplace-items-in-azure-csp"></a>Azure CSP での Azure Marketplace 項目

現在、Azure CSP サブスクリプションでは、すべての Azure Marketplace 項目を利用できるわけではありません。

- Microsoft ベースの Azure サービス:これらのサービスは利用可能です。 前の表とコメントを確認してください。

- ライセンス持ち込み (BYOL) 項目:これらの項目は利用可能です。 BYOL 対応 Azure Marketplace 項目の完全な一覧については、[Azure Marketplace BYOL に関するページ](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)をご覧ください。

- 従量課金制のサードパーティ製 Azure Marketplace 項目:これらの項目は、プロバイダーが CSP チャネルに公開している場合、利用できます。 詳細については、「[Azure Marketplace 製品にサブスクリプションを販売する](https://aka.ms/marketplaceincsp)」を参照してください。   

- Citrix XenApp Essentials:パートナーは、CSP での顧客向け XenApp Essentials を購入できます。 詳しくは、次の Citrix ブログ「[XenApp Essentials の配布を Microsoft クラウド ソリューション プロバイダー チャネルから利用可能](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/)」をご覧ください。

### <a name="national-clouds"></a>ナショナル クラウド 
次の表に、ナショナル クラウドの CSP 向けファーストパーティ製 Azure 製品、サービス、および機能の定期的に更新される一覧を示します。 

| Azure 製品、サービス、機能 | 米国政府 | ドイツ |
| ------ | :-----------: | :-----------: |
|  **Compute**  |    |    |
|  仮想マシン  |  X  |  X  |
|  クラウド サービス  |    |    |
|  仮想マシン スケール セット  |  X  |  X  |
|  関数  |    |    |
|  Azure Container Service  |    |    |
|  **ネットワーク**  |    |    |
|  Azure DNS  |    |    |
|  コンテンツ配信ネットワーク  |    |    |
|  Traffic Manager  |    |    |
|  ExpressRoute  |  X  |  X  |
|  仮想ネットワーク  |  X  |  X  |
|  ロード バランサー  |  X  |  X  |
|  VPN Gateway  |  X  |  X  |
|  Application Gateway  |  X  |  X  |
|  Network Watcher  |  X  |  X  |
|  **ストレージ**  |    |    |
|  記憶域  |  X  |  X  |
|  バックアップ  |  X  |  X  |
|  StorSimple  |    |  X  |
|  Site Recovery  |  X  |  X  |
|  Data Lake Store  |    |    |
|  マネージド ディスク  |  X  |  X  |
|  **Web + モバイル**  |    |    |
|  アプリ サービス  |  X  |  X  |
|  App Service on Linux  |    |  X  |
|  API 管理  |  X  |    |
|  コンテンツ配信ネットワーク  |    |    |
|  メディア サービス  |  X  |  X  |
|  通知ハブ  |  X  |  X  |
|  Azure Search  |    |    |
|  Azure App Service の Logic Apps 機能  |    |    |
|  **コンテナー**  |    |    |
|  アプリ サービス  |  X  |  X  |
|  App Service on Linux  |    |  X  |
|  Batch (バッチ)  |  X  |  X  |
|  コンテナー レジストリ  |    |    |
|  コンテナー インスタンス  |    |    |
|  Service Fabric  |  X  |  X  |
|  コンテナー サービス  |    |    |
|  **データベース**  |    |    |
|  SQL データベース  |  X  |  X  |
|  Azure Cosmos DB  |  X  |  X  |
|  SQL Data Warehouse  |  X  |  X  |
|  Redis Cache  |  X  |  X  |
|  SQL Server Stretch Database  |  X  |  X  |
|  Azure Database for MySQL  |    |    |
|  Azure Database for PostgreSQL  |    |    |
|  **データ + 分析**  |    |    |
|  Databricks  |    |    |
|  HDInsight  |  X  |  X  |
|  Stream Analytics  |    |  X  |
|  Data Factory  |    |    |
|  Log Analytics  |  X  |    |
|  Data Catalog  |    |    |
|  Data Lake Store  |    |    |
|  Data Lake Analytics  |    |    |
|  Azure Analysis Services  |    |    |
|  Power BI Embedded  |    |    |
|  **AI + Cognitive Services**  |    |    |
|  Machine Learning  |    |  X  |
|  Azure Bot Service  |    |    |
|  Cognitive Services  |    |    |
|  Azure Batch AI  |    |    |
|  **モノのインターネット**  |    |    |
|  IoT Hub  |  X  |  X  |
|  IoT Central  |    |    |
|  Machine Learning  |    |  X  |
|  Stream Analytics  |    |  X  |
|  Event Hubs  |  X  |  X  |
|  所在ベースのサービス  |    |    |
|  通知ハブ  |  X  |  X  |
|  Time Series Insights  |    |    |
|  **Enterprise Integration**  |    |    |
|  StorSimple  |  X  |    |
|  API 管理  |    |    |
|  イベント グリッド  |    |    |
|  Data Factory  |    |    |
|  Service Bus  |  X  |  X  |
|  Data Catalog  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Azure App Service の Logic Apps 機能  |    |    |
|  **セキュリティ + ID**  |    |    |
|  Azure Active Directory  |  X  |  X  |
|  Azure Active Directory B2C  |    |    |
|  多要素認証  |    |    |
|  Azure Active Directory Domain Services  |    |    |
|  Key Vault  |  X  |  X  |
|  セキュリティ センター  |  X  |  X  |
|  **開発者ツール**  |    |    |
|  Visual Studio Team Services  |    |    |
|  Application Insights  |    |    |
|  DevTest Labs  |    |    |
|  Visual Studio App Center  |    |    |
|  Xamarin University  |    |    |
|  **監視 + 管理**  |    |    |
|  Advisor  |    |    |
|  バックアップ  |  X  |  X  |
|  Site Recovery  |  X  |  X  |
|  スケジューラ  |  X  |  X  |
|  自動化  |  X  |  X  |
|  Log Analytics  |  X  |    |
|  Azure Monitor  |    |    |
|  Azure マネージド アプリケーション  |    |    |
|  Azure Migrate  |    |    |
|  管理グループ  |    |  

### <a name="next-steps"></a>次の手順

- パートナー センターで利用可能な Azure 向け機能については、[こちら](https://docs.microsoft.com/azure/cloud-solution-provider/overview/partner-center-overview)をご覧ください。

- Azure CSP で最初の顧客を[作成](https://docs.microsoft.com/azure/cloud-solution-provider/customer-management/create-new-customer)し、Azure サービスをデプロイしましょう。
