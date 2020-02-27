---
title: Azure プランへの顧客の移行 | パートナー センター
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客を Azure プランに簡単に移動する方法について説明します。
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: d9a283242fb911537004719fd62a58478c511565
ms.sourcegitcommit: c3de2c04d761314116b876ffdd4b2c79641007c1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/24/2020
ms.locfileid: "77567238"
---
# <a name="transition-your-customers-to-azure-plan"></a>顧客の Azure プランへの移行

**適切なロール**

- 管理エージェント
- 課金管理者
- グローバル管理者
- ヘルプデスク エージェント
- 販売代理店
- ユーザー管理の管理者

間接プロバイダーおよび直接請求パートナーは、Azure 向け Microsoft クラウド サービス プロバイダー (CSP) プログラムで利用可能な新しいコマース エクスペリエンスに移行できます。 (間接リセラーは、間接プロバイダーを通じて行う必要があります)。パートナーからの購入、マイクロソフト販売者からの購入、または Web 上での直接購入にかかわらず、クラウド サービスを簡単に購入するための最新の方法が顧客に提供されます。

移行機能は、新しい Azure 向けコマース エクスペリエンスに移行する顧客で、Microsoft 顧客契約に署名している顧客のみを対象としています。Office 365 や Dynamics 365 などの CSP の他のプランは対象外です。

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

- [Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/)  顧客のテナントのユーザーのみが、その Time Series Insights 環境内のデータにアクセスできます。 パートナーは既定で、顧客の Time Series Insights 環境を管理できますが、そこにあるデータへのアクセスが必要な場合、それらは顧客のテナントに追加される必要があります。 

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

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>既存の CSP プランの Azure プランへの移行

パートナー センターで、既存の CSP Azure プランから CSP プログラムの新しいコマース エクスペリエンスである Azure プランで管理される Azure サービスに顧客を移行させることができます。 これを行うには、パートナーと顧客の間にパートナー センターを通じて再販業者関係が確立されている必要があり、顧客が Microsoft 顧客契約に署名している必要があります。

### <a name="select-transition-to-azure-plan"></a>Azure プランへの移行を選択する

1. 顧客向けの Azure プランを選択します。

2. **[請求を Azure プランに移行する]** を選択します。

![移行](images/azure/transition1.png)

3. **[続行]** を選択します。

![移行](images/azure/transition2.png)

顧客は、Azure プランに移行されます。

**移行ワークフローによって、前提条件となる手順が自動化されます**。

- Azure プランの購入
- ダイレクト CSP での顧客ごとに 1 つのプラン シナリオ  
- リセラーごとに 1 つのプラン  

例として、パートナーが 2つの Microsoft Azure プランを購入し、その購入の中に 2 つの異なる POR が含まれているとします。 この場合、移行ワークフローでは、2 つの Azure プラン (リセラーごとに 1 つ) が購入され、各 Azure サブスクリプションが Azure プランに自動的にマップされます。  

**Azure サブスクリプションの Azure プランへのマッピング**

Azure プランを購入すると、システムによって既存の Azure サブスクリプションが Azure プランにマップされます。 進行状況は、パートナー センターだけでなく Azure portal でも確認できます。 

4. 顧客のパートナー センターの **[サブスクリプション]** ページに戻り、顧客の現地通貨を使用して予算制限を更新します。 

![移行](images/azure/transition3.png)

>[!NOTE]
>パートナー センターで設定した予算は、Azure portal には引き継がれません。 Azure portal で、予算とアラートも設定する必要があります。

Azure プランに移行すると、この顧客用の Azure サブスクリプションを購入することはできなくなります。 サブスクリプションは、Azure portal で Azure プランの中に作成します。

>[!NOTE]
> Azure プランで RBAC を通して購入されたすべての Azure サブスクリプションに対し、現地通貨で請求および課金されます。 為替レートは使用されません。

### <a name="track-your-transition-details"></a>移行の詳細を追跡する

パートナー センターだけでなく、Azure portal でも移行の進行状況を確認してください。

![詳細の表示](images/azure/details1.png)

**パートナーに対する請求の影響**

既存の CSP Azure プランから顧客を移行する場合、次のような請求の影響が発生します。

- 元の CSP Azure サブスクリプションの終了時点までのすべての使用量については、既存の CSP 請求書で請求されます。

- 既存の CSP サブスクリプションに対する管理者アクセス権を持っている場合は、そのサブスクリプションが移行されたときに引き続きアクセス権を所有します。

ダイレクト エンタープライズ契約を CSP に移行し、サーバーとクラウドの登録を Azure サービスに移行するには、[Microsoft パートナー契約での Azure サブスクリプションの課金所有権の取得](https://docs.microsoft.com/azure/billing/mpa-request-ownership)に関する記事を参照してください。

**監査ログ**:

請求を調整するには、 **[サブスクリプション]** ページで "Microsoft Azure" (0145P) サブスクリプションの履歴を確認します。 

"Microsoft Azure" (0145P) サブスクリプションは、次の 2 つの部分で構成されます。
1. コマース サブスクリプション 
2. Azure サブスクリプション (権利)

移行が完了すると、Azure サブスクリプションは新しい Azure プランの下に移動され、コマース サブスクリプションはこれ以上の使用が報告されないように停止されます。  

>[注]\:CSP で Microsoft Azure (0145P) サブスクリプションを 購入した場合、コマース サブスクリプションと Azure サブスクリプション (権利) の価格は同じになります。 これは、課金所有権の変更または譲渡で価格が異なる場合にのみ発生します。 

**移行に関する問題**

移行中に問題が発生することは想定されていません。 発生した場合は、移行ワークフロー自体の中で更新が実行されます。 Azure の使用に障害が発生することはありません。  

## <a name="next-steps"></a>次の手順

- [Azure プランのサブスクリプションとリソースを管理する](azure-plan-manage.md)

- [パートナー獲得クレジット - 概要](partner-earned-credit.md)



