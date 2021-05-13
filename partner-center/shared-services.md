---
title: Azure Partner Shared Services の追加
description: 独自Azure Partner Shared Services Azure サブスクリプションを購入し、Azure を購入、追跡、管理するための統一された方法を使用します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 929907c7c6f238fb84a13622227534797f0ac949
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855337"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>パートナー Azure Partner Shared Services使用するために Azure サブスクリプションを購入できるよう、サブスクリプションを追加する

**適切なロール**: グローバル管理者|管理エージェント |セールス エージェント

Azure Partner Shared Services は、CSP プログラムのパートナー様向けの新しいプランの種類です。このプランでは、パートナー様自身が使用する Azure サブスクリプションを購入できます。パートナーにとっては、Microsoft との Azure ライセンス契約および再販契約を集約できるだけでなく、統一された方法で Azure を購入、追跡、管理できるようになります。 Azure Partner Shared Services では、パートナーは、Microsoft Enterprise Agreement および Web Direct プログラムと同じように CSP で Azure サブスクリプションを使用する柔軟性を備え、開発環境とテスト環境の構築、内部ワークロードのデプロイ、共有サービスまたはマルチテナント アプリケーションのホストなどのシナリオを開く機能を備えています。  

## <a name="create-the-shared-services-tenant"></a>共有サービス テナントを作成する

1. [設定] [**アカウント**  >  **設定] [共有サービス**  >  **] に移動します**。

   :::image type="content" source="images/sharedservices2.png" alt-text="共有サービス>アカウント設定":::

2. 共有サービス テナントをお持ちでない場合は、**[Create shared services]** (共有サービスの作成) をクリックします。

   :::image type="content" source="images/sharedservices3.png" alt-text="共有サービスの作成":::

3. これにより、共有サービス テナントが作成され、共有リソースや内部ワークロードで使用する Azure CSP Shared Services サブスクリプションの購入が行われます。

   :::image type="content" source="images/sharedservices5.png" alt-text="テナントの作成とサブスクリプションの購入":::

## <a name="about-the-azure--internalshared-services-offer"></a>Azure - Internal/Shared Services プランについて

- サブスクリプションAzure - Internal/Shared Servicesは、パートナーが Azure を独自に使用するために取得パートナー センター CSP でアクセスする新しい Azure オファーの種類です。

- Azure Partner Shared Servicesサブスクリプションは対象であり、RIs の購入に使用できます。

- Azure - Internal/Shared Services プランは、共有サービス テナントにのみ適用できます。

- サブスクリプションを使用するAzure - Internal/Shared Servicesは、独自の開発目的で Azure を使用できる方法です。 このオファーのプロビジョニングに使用する共有テナントは、Office 365 や Dynamics ライセンスなどの他のサービスには使用できません。

- サブスクリプションのキャンセルは、他のサブスクリプションと同様の方法で行うことができます。 [すべての設定を表示 **] [**  >  **共有サービス] の設定**  >  **に移動します**。 Azure - Internal/Shared Services を選択して取り消します。

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Azure Partner Shared Services の利用状況の詳細にアクセスする

Azure の利用状況は、CSP 請求書と調整ファイルに記載されます。 請求書では、Microsoft Azure の明細項目の一部として含まれます。 利用状況の詳細は、このプラン用に作成されたテナントに対して記録された調整ファイルで参照できます。

## <a name="azure-partner-shared-services-pricing"></a>Azure Partner Shared Services の価格

Azure Partner Shared Servicesの新しい価格ファイルを表示するには、[価格とオファーの販売] に移動し、当月の価格  >  表を選択します。 今後数週間のうちには、特定の価格カードの API もリリースされる予定です。

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>マーケットプレースのプランと Azure Partner Shared Services

2019 年 3 月 1 日の現在、Azure Partner Shared Services (APSS) は Marketplace オファーをサポートしなくなりました。

|**マーケットプレースのサポート**   |**2019 年 3 月 1 日より前にサポートされる APSS**|**2019 年 3 月 1 日以降**|
|---------------------------|:----------------------------|:-------------------|
|ライセンス持ち込み (BYOL) と無料サービス   | はい   | いいえ|
|その他のサードパーティのマーケットプレースのプラン   | いいえ   |いいえ|

APSS を使用してデプロイされた BYOL または無料サービスを持つパートナーには影響はありません。ただし、2019 年 3 月 1 日より後は、新しい BYOL または無料サービスを購入する予定ではありません。

利用可能な Marketplace オファー (BYOL や無料サービス) の完全なカタログを利用するには、CSP パートナーが Web ダイレクト Azure サブスクリプションを使用して共有サービスをデプロイすることをお勧めします。  以前にサードパーティの BYOL と無料のサービスリソースをデプロイしたことがあり、それを引き続き使用してサードパーティ製品をデプロイする場合は、 [既存の Azure サブスクリプション](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)の Web direct 移行に APSS サブスクリプションを移行することをお勧めします。

2019年3月1日より後に APSS サブスクリプションの使用を予定しており、新しいサードパーティの [Byol サービス](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) または無料サービスをデプロイすることを計画しているパートナーは、isv の指示に従ってこれらを APSS サブスクリプションにデプロイできます。

## <a name="next-steps"></a>次の手順

- [CSP によるソフトウェア サブスクリプションの販売](csp-software-subscriptions.md)