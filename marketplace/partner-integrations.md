---
title: Azure Marketplace パートナーの統合
description: Azure 環境に統合された Azure Marketplace ソリューションについて説明し、Microsoft パートナーのデプロイガイドへのリンクを提供します。
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: b31486000e59f3d85ee30019ecea000252b297a8
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/21/2020
ms.locfileid: "95006907"
---
# <a name="azure-marketplace-partner-integrations"></a>Azure Marketplace パートナーの統合

パートナーソリューションを Azure 環境に統合する方法について説明します。 この記事では、各ソリューションの概要と、詳細なデプロイガイドへのリンクを示します。 ソリューションはアルファベット順に一覧表示されます。 

## <a name="apache-kafka-on-confluent-cloud"></a>Confluent Cloud での Apache Kafka

![Confluent Cloud](./media/partners/confluent-cloud.png)

Azure では、クラウドアプリケーションに加えて Confluent Cloud と統合できます。 Confluent のお客様は、多くの場合、Azure portal と Confluent Cloud の間を移動します。 たとえば、ユーザーが Azure Marketplace で Confluent Cloud プランを購入すると、Confluent Cloud を使用してアカウントを設定することが求められます。 このプロセスでは複雑さと時間が増加するため、ユーザーは2つのポータル間で構成とリソースを管理する必要があります。 Microsoft が Confluent Cloud と提携しているプラットフォームでの管理の負担を軽減するために、Azure から Confluent Cloud に統合されたプロビジョニングレイヤーを構築しています。 このソリューションは Azure Marketplace で利用可能であり、Azure で Confluent Cloud オファリングを使用するためのシームレスなエクスペリエンスを提供します

このソリューションでは、Azure で有効になっているリソースプロバイダーを使用して、Confluent クラウドリソースをプロビジョニングします。 これにより、ユーザーは Azure portal、Azure CLI、Azure Sdk を使用してリアルタイムのイベントストリーミングにアクセスできます。 Confluent Cloud は、環境、クラスター、トピック、API キー、およびマネージコネクタを含む SaaS アプリケーションを所有して実行します。

Confluent Cloud との緊密な統合により、次の機能が有効になります。

- 完全に管理されたインフラストラクチャを使用して、Azure portal から新しい Confluent Cloud 組織のリソースをプロビジョニングします。
- Azure Active Directory を使用した Azure から Confluent Cloud へのシングルサインオンを効率化します。Confluent Cloud ポータルでは、別個の認証は必要ありません。
- Azure サブスクリプションの請求書を通じて、Confluent クラウドの消費料金の統合課金を取得します。
- Azure portal から Confluent Cloud リソースを管理し、Azure リソースと共に [ **すべてのリソース** ] ページで追跡します。

[Confluent クラウドデプロイガイド](https://docs.confluent.io/current/cloud/marketplace/index.html)

Azure での Confluent に関する問題については、「」を参照 [https://support.confluent.io](https://support.confluent.io) してください。 初めてのユーザーの場合は、Confluent サポートポータルにサインインする前にパスワードをリセットしてください。 Confluent のアカウントをお持ちでない場合は、に電子メールをお送りください [cloud-support@confluent.io](mailto:cloud-support@confluent.io) 。

## <a name="datadog"></a>Datadog

![DataDog のロゴ](./media/partners/datadog.png)

Datadog は、ハイブリッド環境とマルチクラウド環境でのアプリケーションの正常性とパフォーマンスを理解するために、Azure ユーザー向けの可観測性およびセキュリティツールを提供します。 ただし、必要な統合を構成するには、Azure portal と Datadog 間を頻繁に移動する必要があります。 ポータルでの構成とリソースの管理を簡略化するために、Microsoft は Datadog と連携して Azure で統合 Datadog ソリューションを作成しました。 Azure Marketplace を通じて提供されているこのソリューションでは、Azure のお客様が Datadog のクラウド監視ソリューションを使用するためのシームレスなエクスペリエンスを提供します。

このソリューションの詳細については、 [Azure Monitor のドキュメント](/azure/azure-monitor/platform/partners#datadog) を参照して、パブリックプレビューにサインアップしてください。

## <a name="next-steps"></a>次の手順

- [Azure Marketplace オンラインストア](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn: Azure アカウントを作成する](/learn/modules/create-an-azure-account/)
