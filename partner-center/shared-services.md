---
title: Azure Partner Shared Services の追加
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure Partner Shared Services を使用して、自分で使用する Azure サブスクリプションを購入し、Azure の購入、追跡、および管理のための統一された方法を利用できます。
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, Shared Services, テナント
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 62989c58284de46834f02abc01041c454e725a81
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/04/2020
ms.locfileid: "84425951"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>パートナーが自分で使用するために Azure サブスクリプションを購入できるように Azure パートナー共有サービスを追加する

**適用対象**

- パートナー センター

Azure Partner Shared Services は、CSP プログラムのパートナー様向けの新しいプランの種類です。このプランでは、パートナー様自身が使用する Azure サブスクリプションを購入できます。パートナーにとっては、Microsoft との Azure ライセンス契約および再販契約を集約できるだけでなく、統一された方法で Azure を購入、追跡、管理できるようになります。 Azure Partner Shared Services を使用すると、パートナーは、Microsoft マイクロソフトエンタープライズ契約および Web ダイレクトプログラムの場合と同じように、CSP で Azure サブスクリプションを柔軟に使用できるようになり、開発とテスト環境の構築、内部ワークロードのデプロイ、共有サービスやマルチテナントアプリケーションのホストなどのシナリオを開くことができます。  

## <a name="create-the-shared-services-tenant"></a>共有サービス テナントを作成する

1. [**設定**] [すべての設定] [  >  **View all settings**  >  **共有サービス**] にアクセスします。

   ![**[アカウント設定]** の **[共有サービス]**](images/sharedservices2.png)

2. 共有サービス テナントをお持ちでない場合は、**[Create shared services]** (共有サービスの作成) をクリックします。

   ![共有サービスの作成](images/sharedservices3.png)

3. これにより、共有サービス テナントが作成され、共有リソースや内部ワークロードで使用する Azure CSP Shared Services サブスクリプションの購入が行われます。

   ![テナントの作成とサブスクリプションの購入](images/sharedservices5.png)

## <a name="about-the-azure--internalshared-services-offer"></a>Azure - Internal/Shared Services プランについて

- Azure-Internal/Shared Services サブスクリプションは、パートナーセンターを通じてアクセスされる CSP の新しい Azure プランの種類であり、パートナーは Azure を独自に使用することができます。 

- Azure-Internal/Shared Services プランは割引およびインセンティブの対象ではありません。

- Azure - Internal/Shared Services プランは、共有サービス テナントにのみ適用できます。

- Azure-Internal/Shared Services サブスクリプションの主な用途は、独自の開発目的で Azure を使用できるようにすることです。 このプランのプロビジョニングに使用する共有テナントは、Office 365 や Dynamics のシートなどの他のサービスに使うことはできません。 

- サブスクリプションのキャンセルは、他のサブスクリプションと同様の方法で行うことができます。 [**設定**] ビューの [すべての設定] [  >  **View all settings**  >  **共有サービス**] にアクセスします。 Azure - Internal/Shared Services を選択して取り消します。

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Azure Partner Shared Services の利用状況の詳細にアクセスする

Azure の利用状況は、CSP 請求書と調整ファイルに記載されます。 請求書では、Microsoft Azure の明細項目の一部として含まれます。 利用状況の詳細は、このプラン用に作成されたテナントに対して記録された調整ファイルで参照できます。 

## <a name="azure-partner-shared-services-pricing"></a>Azure Partner Shared Services の価格

Azure パートナーの共有サービスの新しい価格ファイルを確認するに**Sell**は、  >  **価格とプラン**の販売に関するページにアクセスし、当月の価格表を選択してください。 今後数週間のうちには、特定の価格カードの API もリリースされる予定です。

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>マーケットプレースのプランと Azure Partner Shared Services

2019年3月1日の時点で、Azure Partner Shared Services (APSS) では Marketplace プランはサポートされなくなりました。

|**マーケットプレースのサポート**   |**2019 年 3 月 1 日より前にサポートされる APSS**|**2019 年 3 月 1 日以降**|
|---------------------------|:----------------------------|:-------------------|
|ライセンス持ち込み (BYOL) と無料サービス   | はい   | いいえ|
|その他のサードパーティのマーケットプレースのプラン   | いいえ   |いいえ|

APSS を使用してデプロイされた BYOL または無料のサービスを利用しているパートナーは影響を受けません。ただし、2019年3月1日以降、新しい BYOL または無料サービスを購入することはできません。

(BYOL と無料サービスだけでなく) 利用可能な Marketplace プランの完全なカタログを利用するには、CSP パートナーが web ダイレクト Azure サブスクリプションを使用して共有サービスをデプロイすることをお勧めします。  以前にサードパーティの BYOL と無料のサービスリソースをデプロイしたことがあり、それを引き続き使用してサードパーティ製品をデプロイする場合は、[既存の Azure サブスクリプション](https://docs.microsoft.com/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)の Web direct 移行に APSS サブスクリプションを移行することをお勧めします。

2019年3月1日より後に APSS サブスクリプションの使用を予定しており、新しいサードパーティの[Byol サービス](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)または無料サービスをデプロイすることを計画しているパートナーは、isv の指示に従ってこれらを APSS サブスクリプションにデプロイできます。

