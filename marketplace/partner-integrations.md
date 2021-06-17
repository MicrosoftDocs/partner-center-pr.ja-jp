---
title: Azure Marketplace パートナー統合
description: Azure 環境Azure Marketplaceするソリューションについて説明し、Microsoft パートナーからのデプロイ ガイドへのリンクを取得します。
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: 56e72af367cdcb264cc444446c5fcbedcd880451
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276486"
---
# <a name="azure-marketplace-partner-integrations"></a>Azure Marketplace パートナー統合

パートナー ソリューションを Azure 環境に統合する方法について説明します。 この記事では、各ソリューションの概要と、詳細なデプロイ ガイドへのリンクを示します。 ソリューションはアルファベット順に一覧表示されます。 

## <a name="apache-kafka-on-confluent-cloud"></a>Confluent Cloud での Apache Kafka

![Confluent Cloud。](./media/partners/confluent-cloud.png)

Azure では、クラウド アプリケーションに加えて Confluent Cloud と統合できます。 Confluent のお客様は、多くの場合、Azure portal Confluent Cloud 間を移動します。 たとえば、ユーザーが Azure Marketplace で Confluent Cloud オファーを購入すると、Confluent Cloud でアカウントを設定する必要があります。 このプロセスにより複雑性と時間が追加され、ユーザーは 2 つのポータル間で構成とリソースを管理する必要があります。 プラットフォーム間での管理の負担を軽減するために、Microsoft は Confluent Cloud と連携して、Azure から Confluent Cloud への統合プロビジョニング レイヤーを構築しました。 このソリューションは、Azure Azure Marketplaceで Confluent Cloud オファリングを使用するシームレスなエクスペリエンスを提供します

このソリューションでは、Azure で有効になっているリソース プロバイダーを使用して Confluent Cloud リソースをプロビジョニングします。 これにより、ユーザーは、Azure portal、Azure CLI、および Azure SDK を介してリアルタイム のイベント ストリーミングにアクセスできます。 Confluent Cloud は、環境、クラスター、トピック、API キー、マネージド コネクタを含む SaaS アプリケーションを所有して実行します。

Confluent Cloud との深い統合により、次の機能が可能です。

- フル マネージド インフラストラクチャにより、Azure portal から新しい Confluent Cloud の組織リソースをプロビジョニング。
- Azure から Confluent Cloud へのシングル サインオンを Azure Active Directory。Confluent Cloud ポータルから個別の認証を行う必要はありません。
- Azure サブスクリプションの請求を通じて、Confluent Cloud の消費料金の統合請求を取得します。
- サーバーから Confluent Cloud リソースを管理Azure portal、Azure リソースと共に [すべてのリソース] ページでそれらを追跡します。

[Confluent クラウドデプロイ ガイド](https://docs.confluent.io/current/cloud/marketplace/index.html)

Azure 上の Confluent に関連する問題については、 にアクセスしてください [https://support.confluent.io](https://support.confluent.io) 。 初めて使用する場合は、Confluent サポート ポータルにサインインする前にパスワードをリセットしてください。 Confluent のアカウントをお持ちではない場合は、 にメールをお送りください [cloud-support@confluent.io](mailto:cloud-support@confluent.io) 。

## <a name="datadog"></a>Datadog

![DataDog ロゴ。](./media/partners/datadog.png)

Datadog は、Azure ユーザーがハイブリッドおよびマルチクラウド環境全体のアプリケーションの正常性とパフォーマンスを把握するための監視およびセキュリティ ツールを提供します。 ただし、必要な統合を構成するには、Azure portal と Datadog 間を頻繁に移動する必要があります。 ポータル間の構成とリソース管理を簡素化するために、Microsoft は Datadog と一緒に Azure に統合 Datadog ソリューションを作成しました。 このソリューションAzure Marketplace、Azure のお客様が Datadog のクラウド監視ソリューションを使用するシームレスなエクスペリエンスを提供します。

このソリューション [Azure Monitor詳細](/azure/azure-monitor/platform/partners#datadog) を確認し、パブリック プレビューにサインアップするには、次のドキュメントを参照してください。

## <a name="next-steps"></a>次のステップ

- [Azure Marketplace オンライン ストア](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn: Azure アカウントを作成する](/learn/modules/create-an-azure-account/)
