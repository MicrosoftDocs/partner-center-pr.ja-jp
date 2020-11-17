---
title: Azure 予約 & サーバーサブスクリプション
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure の予約とサーバーサブスクリプションを取得、プロビジョニング、および管理するためのクラウドソリューションプロバイダーの機会について説明します。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0434ad2e6494f5efc1b1e5e2aa003dc6587d7b4e
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691352"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a>Azure reserved VM instances (RI) と顧客向けのサーバーサブスクリプションの取得、プロビジョニング、& 管理


**適切なロール**

- 管理エージェント
- グローバル管理者
- ヘルプデスク エージェント
- 販売代理店
- ユーザー管理の管理者


## <a name="what-are-azure-reservations"></a>Azure の予約とは

Azure Reservations では、1 年分または 3 年分の料金を前払いすることにより、仮想マシン、SQL Database の処理能力、Azure Cosmos DB スループット、その他の Azure リソースを割引価格で利用することができます。 前払いすると、使用するリソースの割り引きを受けることができます。 予約では、従量課金制の価格と比較して、仮想マシン、SQL Database の処理能力、Azure Cosmos DB、その他のリソースのコストを最大 72% も削減することができます。 予約は課金割引を提供するもので、リソースの実行時の状態には影響しません。 詳細について[は、「Azure Reservations とは](/azure/billing/billing-save-compute-costs-reservations)」を参照してください。

## <a name="why-should-customers-buy-a-reservation"></a>顧客が予約を購入する必要がある理由

顧客が長期間実行する仮想マシン、Azure Cosmos DB、または SQL データベースを使用している場合、予約の購入は最もコスト効率に優れたオプションです。 たとえば、予約を使用しないでサービスの 4 つのインスタンスを連続的に実行している場合、従量課金制料金で課金されます。 これらのリソースについて予約を購入した場合は、すぐに予約割引が適用されます。 リソースには従量課金制の料金が適用されなくなります。

### <a name="compelling-new-azure-offer-in-csp"></a>CSP での魅力的な新しい Azure プラン

今日、予測が十分可能で永続的なクラウド ワークロードはコスト効率の高いソリューションでサポートしたいという需要が急速に高まっています。Azure Reservations とサーバー サブスクリプションが CSP プログラムに含まれることで、Microsoft のパートナーはこのような顧客の需要に対応できます。 CSP プログラムを使用すると、パートナーは、Microsoft パートナーセンターと Azure portal を通じて、商用の顧客に代わって Azure Reservations とサーバーのサブスクリプションを取得、プロビジョニング、および管理できます。
また、Azure の予約を購入する方法について、CSP プログラムの選択肢をパートナーに提供しています。 CSP パートナーは [、お客様の代わりに azure の予約を購入](azure-reservations-buying.md) できます。また、お客様は、パートナーが購入した以前の azure サブスクリプションから [独自の予約を購入する](give-customers-permission.md) こともできます。

Azure Reservations を利用すると、開発、テスト、アプリケーションの実行、データセンターの拡張を含む幅広いコンピューティング ソリューションに対して柔軟な仮想化を実現できます。

たとえば [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) では、商用のお客様は、1年間または3年間の仮想マシンを購入または "予約" するだけで、最大72% と従量課金制の Azure VM 料金を節約できるようになりました。 ソフトウェア アシュアランスに含まれている Azure ハイブリッド特典を利用できる Windows Server 顧客は、従量課金制の価格と比較して最大 80% を節約できます。

説得力のある価格と比類のない展開の柔軟性の組み合わせにより、お客様は Azure Reservations を選択すると、全体的な価値が最も高くなります。

- Azure Portal での [購入予約](https://docs.microsoft.com/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) をご覧ください。

- ソフトウェアサブスクリプションと Linux ISV の年間サブスクリプションについては、パートナーセンターの [価格とプラン](https://partner.microsoft.com/dashboard/sell/pricingandoffers)に関するページの **Microsoft Azure 予約済みインスタンス**] カテゴリの下にある **Azure RI CSP の商用価格表** を参照してください。


 
**Linux ISV 年間サブスクリプション**

- SUSE Linux
- Red Hat Enterprise Linux
- Azure Red Hat OpenShift

**ISV 年間サブスクリプション**

- Azure VMware Solution by CloudSimple

## <a name="getting-started"></a>作業の開始

Azure Reservations を顧客と共に配置し、可能な限り迅速に運用を開始する方法を理解するために、次の方法で準備資料を確認することをお勧めします。

1. [パートナーセンターの新しいコマース運用ガイド](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)を確認し、理解します。

2. [パートナーセンター api (api/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)での Azure Reservations とサーバーサブスクリプションの更新について説明します。


### <a name="sales-readiness"></a>販売の準備

- [リモートデスクトップサービス (RDS) クライアントアクセスライセンス (CAL) (アナウンス)](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [Azure Reserved VM Instances (Azure portal)](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [サーバー サブスクリプション](https://docs.microsoft.com/partner-center/csp-software-subscriptions)

- [SQL DB の予約 (Azure portal)](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)

- [Azure Cosmos DB (Azure portal)](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)

- [SQL Managed Instance (Azure portal)](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)

- [SUSE および Red Hat Enterprise Linux (Azure portal)](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)

- [Azure 上の Red Hat Linux](https://azure.com/redhat)

- [Azure 上の SUSE Linux](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [Azure 上の Linux](https://azure.microsoft.com/overview/linux-on-azure/)

- [Azure の料金概要](https://azure.microsoft.com/pricing/)

- [Azure 料金計算ツール](https://azure.microsoft.com/pricing/calculator)

- [Azure Databricks ユニットの予約](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a>トレーニング

登録して、 [商用ライセンス準備ウェビナー](https://commercial-licensing.eventbuilder.com/FY2019_ALL) およびオンデマンドイベントを表示します。
以前に記録されたライセンス準備オンデマンドイベントには、次のようなトピックが含まれます。

- CSP オンラインサービス、CSP Azure、一般的なライセンス更新 (Azure を含む) (2018 年11月)

- SQL DB の予約容量 & インスタンスサイズの柔軟性 (8 月2018日)

- CSP のサーバーサブスクリプション (2018 年7月)

- CSP での Azure Reservations の概要 (2018 年5月)

## <a name="operations"></a>Operations

[パートナーセンターの新しいコマース運用ガイド](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf): 主要なポリシーと運用面 (契約、パートナーセンターからの注文、請求書、価格表の詳細、インセンティブ、調整ファイル、API/SDK、サンドボックス、Azure Partner Shared Services など) に関する包括的なガイドです。

## <a name="azure-hybrid-benefit"></a>Azure ハイブリッド特典

[Azure ハイブリッド特典](https://azure.microsoft.com/pricing/hybrid-benefit)は、ソフトウェアアシュアランス付きのライセンスを所有しているお客様にとっての価格特典です。これにより、既存のオンプレミスの Windows Server の価値を最大化したり、Azure への移行時にライセンスへの SQL Server を適用したりすることができます。 対象と80なるお客様は、Azure Virtual Machines (infrastructure as a service (IaaS)) で最大 40% * を節約し、Azure SQL Database (プラットフォームとしてのプラットフォーム、または PaaS) に対して最大55% の節約を可能にし、Azure ハイブリッド特典を使用して Azure Virtual Machines (IaaS) に SQL Server します

## <a name="next-steps"></a>次の手順

- [Azure ハイブリッド特典のよくあるご質問](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

* 割引による実際の効果は、リージョン、インスタンスの種類、使用率によって異なります。
