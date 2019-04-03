---
title: Azure Partner Shared Services の追加 | パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: Azure Partner Shared Services は、CSP プログラムのパートナー様向けの新しいプランの種類です。このプランでは、パートナー様自身が使用する Azure サブスクリプションを購入できます。
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, Shared Services, テナント
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: ff1e169f54c71e634d07ade9981ecb11009fa9de
ms.sourcegitcommit: 9a2bda49446030e60251c9c913259472ff2eed9a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "57682470"
---
# <a name="add-azure-partner-shared-services"></a>Azure Partner Shared Services の追加

**適用対象**

-  パートナー センター

Azure Partner Shared Services は、CSP プログラムのパートナー様向けの新しいプランの種類です。このプランでは、パートナー様自身が使用する Azure サブスクリプションを購入できます。  Azure のライセンスおよび再販契約をマイクロソフトとの統合に購入、追跡、および機能に加えて Azure を管理するための統一的な方法を使用するパートナーにとっての機会を作成します。 Azure Partner Shared Services の提供開始により、パートナー様は、Microsoft Enterprise Agreement および Web ダイレクト プログラムと同じように、CSP で柔軟に Azure サブスクリプションを利用できるようになりました。開発環境やテスト環境の構築、内部負荷の展開、共有サービスやマルチテナント アプリケーションのホスティングなどのシナリオにも対応できます。  

## <a name="create-the-shared-services-tenant"></a>共有サービス テナントを作成する

1. **[設定]** > **[View all settings]** (すべての設定を表示) > **[共有サービス]** の順に移動します。

    ![**[アカウント設定]** の **[共有サービス]**](images/sharedservices2.png)

2. 共有サービス テナントをお持ちでない場合は、**[Create shared services]** (共有サービスの作成) をクリックします。

    ![共有サービスの作成](images/sharedservices3.png)

3. これにより、共有サービス テナントが作成され、共有リソースや内部ワークロードで使用する Azure CSP Shared Services サブスクリプションの購入が行われます。

    ![テナントの作成とサブスクリプションの購入](images/sharedservices5.png)

## <a name="about-the-azure--internalshared-services-offer"></a>Azure - Internal/Shared Services プランについて

- Azure - Internal/Shared Services サブスクリプションは、パートナー センターからアクセスできる、CSP プログラムの新しい Azure プランの種類です。このプランでは、パートナー様が独自の用途に Azure を利用できます。 

- Azure - Internal/Shared Services プランは、割引やインセンティブの対象にはなりません。

- Azure - Internal/Shared Services プランは、共有サービス テナントにのみ適用できます。

- Azure - Internal/Shared Services サブスクリプションの主な用途は、Azure を独自の開発目的に利用することです。 このプランのプロビジョニングに使用する共有テナントは、Office 365 や Dynamics のシートなどの他のサービスに使うことはできません。 

- サブスクリプションのキャンセルは、他のサブスクリプションと同様の方法で行うことができます。 **[設定]** > **[View all settings]** (すべての設定を表示) > **[共有サービス]** の順に移動します。 Azure - Internal/Shared Services を選択して取り消します。

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Azure Partner Shared Services の利用状況の詳細にアクセスする

Azure の利用状況は、CSP 請求書と調整ファイルに記載されます。 請求書では、Microsoft Azure の明細項目の一部として含まれます。 利用状況の詳細は、このプラン用に作成されたテナントに対して記録された調整ファイルで参照できます。 

## <a name="azure-partner-shared-services-pricing"></a>Azure Partner Shared Services の価格

Azure Partner Shared Services の新しい価格ファイルを確認するには、**[販売]** > **[料金とプラン]** の順に移動し、現在の月の価格表を選択します。 今後数週間のうちには、特定の価格カードの API もリリースされる予定です。

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Marketplace のオファリングは、Azure Partner Shared Services

Azure Partner Shared Services (APSS) には、2019 年 3 月 1 日の時点での Marketplace サービスがサポートされていません。   

|**Marketplace のサポート**   |**APSS、2019 年 3 月 1 日より前に、でサポート**|**、2019 年 3 月 1 日後**|
|---------------------------|:----------------------------|:-------------------|
|ライセンス (BYOL) と無料サービス   | はい   | いいえ|
|その他のサード パーティの marketplace プラン   | いいえ   |いいえ|


BYOL または解放したパートナー APSS を使用してデプロイされたサービスに影響はありません。ただし、2019 年 3 月 1 日後にないされる新しい BYOL または無料のサービスを購入できるようにします。 

利用可能な Marketplace プランの完全なカタログ (BYOL、無料のサービスだけでなく) 利用するために、CSP パートナーは、web ダイレクト Azure サブスクリプションを使用する共有サービスをデプロイをお勧めします。  サード パーティの BYOL を展開し、無料の CSP パートナー以前、Marketplace からリソースをサービスを引き続きそれらを使用してよりサード パーティの web ダイレクト APSS サブスクリプションに移行することが推奨されますオファリングをデプロイ[への移行既存の Azure サブスクリプション](https://docs.microsoft.com/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)します。

後は、2019 年 3 月 1 日、APSS サブスクリプションを使用してを続行し、新しいサード パーティを展開する予定のパートナー、 [BYOL サービス](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)または無料のサービス、ことができます、APSS サブスクリプションにこれらを展開する Isv の指示に従います。

