---
title: サーバー サブスクリプション& Azure の予約
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客向クラウド ソリューション プロバイダー Azure の予約とサーバー サブスクリプションを取得、プロビジョニング、管理する機会について説明します。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 79175fc7e67fdcdc3195b33859f3609c4caf942f
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149419"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a>Azure 予約 VM インスタンス (RI) &顧客向けサーバー サブスクリプションを取得、プロビジョニング、管理する


**適切なロール**: 管理エージェント |グローバル管理者|ヘルプデスク エージェント |Sales Agent |ユーザー管理管理者


## <a name="what-are-azure-reservations"></a>Azure の予約とは

Azure Reservations では、1 年分または 3 年分の料金を前払いすることにより、仮想マシン、SQL Database の処理能力、Azure Cosmos DB スループット、その他の Azure リソースを割引価格で利用することができます。 前払いすると、使用するリソースの割り引きを受けることができます。 予約では、従量課金制の価格と比較して、仮想マシン、SQL Database の処理能力、Azure Cosmos DB、その他のリソースのコストを最大 72% も削減することができます。 予約は課金割引を提供するもので、リソースの実行時の状態には影響しません。 詳細については [、「Azure の予約とは」を参照してください。](/azure/billing/billing-save-compute-costs-reservations)

## <a name="why-should-customers-buy-a-reservation"></a>顧客が予約を購入する必要がある理由

顧客が長期間実行する仮想マシン、Azure Cosmos DB、または SQL データベースを使用している場合、予約の購入は最もコスト効率に優れたオプションです。 たとえば、予約を使用しないでサービスの 4 つのインスタンスを連続的に実行している場合、従量課金制料金で課金されます。 これらのリソースについて予約を購入した場合は、すぐに予約割引が適用されます。 リソースには従量課金制の料金が適用されなくなります。

### <a name="compelling-new-azure-offer-in-csp"></a>CSP での魅力的な新しい Azure プラン

今日、予測が十分可能で永続的なクラウド ワークロードはコスト効率の高いソリューションでサポートしたいという需要が急速に高まっています。Azure Reservations とサーバー サブスクリプションが CSP プログラムに含まれることで、Microsoft のパートナーはこのような顧客の需要に対応できます。 CSP プログラムを使用すると、パートナーは、Microsoft パートナー センター および Azure portal を介して、商用顧客に代わって Azure の予約とサーバー サブスクリプションを取得、プロビジョニング、管理できます。
Azure の予約を購入する方法について、CSP プログラムのパートナーに選択肢を提供しています。 CSP パートナーは、顧客に代わって Azure の予約を購入[](give-customers-permission.md)できます。または、パートナーが購入した以前の[Azure](azure-reservations-buying.md)サブスクリプションから顧客が独自の予約を購入できる場合もあります。

Azure Reservations を利用すると、開発、テスト、アプリケーションの実行、データセンターの拡張を含む幅広いコンピューティング ソリューションに対して柔軟な仮想化を実現できます。

[たとえば、Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/)では、商用のお客様は、仮想マシンを 1 年間または 3 年間購入 (または "予約" する) だけで、Azure VM の料金に対して最大 72% を節約できます。 ソフトウェア アシュアランスに含まれている Azure ハイブリッド特典を利用できる Windows Server 顧客は、従量課金制の価格と比較して最大 80% を節約できます。

説得力のある価格と優れたデプロイの柔軟性の組み合わせが一致しない場合、お客様は Azure の予約を選択するときに最適な全体的な価値を得る可能性があります。

- Azure Portal [で予約を購入](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) する方法に関するページを参照してください。

- ソフトウェア サブスクリプションと Linux ISV 年間サブスクリプションについては、パートナー センター の [価格と [](https://partner.microsoft.com/dashboard/sell/pricingandoffers)プラン] ページの **[Microsoft Azure 予約** インスタンス] カテゴリの下にある **Azure RI CSP** の商用価格表を参照してください。


 
**Linux ISV 年間サブスクリプション**

- SUSE Linux
- Red Hat Enterprise Linux
- Azure Red Hat OpenShift

**ISV 年間サブスクリプション**

- Azure VMware Solution by CloudSimple

## <a name="getting-started"></a>作業の開始

Azure Reservations を顧客と一緒に配置し、可能な限り迅速に運用を開始する方法を理解するには、準備に関する資料を確認するための次のアプローチをお勧めします。

1. 新しいコマース運用ガイド [パートナー センターを確認して理解します](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)。

2. [パートナーセンター api (api/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)での Azure Reservations とサーバーサブスクリプションの更新について説明します。


### <a name="sales-readiness"></a>販売の準備

- [リモートデスクトップサービス (RDS) クライアントアクセスライセンス (CAL) (アナウンス)](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [Azure Reserved VM Instances (Azure portal)](/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [サーバー サブスクリプション](./csp-software-subscriptions.md)

- [SQL DB の予約 (Azure portal)](/azure/sql-database/sql-database-reserved-capacity)

- [Azure Cosmos DB (Azure portal)](/azure/cosmos-db/cosmos-db-reserved-capacity)

- [SQL Managed Instance (Azure portal)](/azure/sql-database/sql-database-managed-instance)

- [SUSE および Red Hat Enterprise Linux (Azure portal)](/azure/virtual-machines/linux/prepay-suse-software-charges)

- [Azure 上の Red Hat Linux](https://azure.com/redhat)

- [Azure 上の SUSE Linux](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [Linux on Azure](https://azure.microsoft.com/overview/linux-on-azure/)

- [Azure の料金概要](https://azure.microsoft.com/pricing/)

- [Azure 料金計算ツール](https://azure.microsoft.com/pricing/calculator)

- [Azure Databricks ユニットの予約](/azure/billing/billing-prepay-databricks-reserved-capacity)


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

## <a name="next-steps"></a>次のステップ

- [Azure ハイブリッド特典のよくあるご質問](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

* 割引による実際の効果は、リージョン、インスタンスの種類、使用率によって異なります。