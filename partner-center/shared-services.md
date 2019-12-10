---
title: Azure Partner Shared Services の追加 | パートナー センター
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure Partner Shared Services を使用して、自分で使用する Azure サブスクリプションを購入したり、Azure の購入、追跡、管理のための統一された方法を利用したりすることができます。
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, Shared Services, テナント
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 2d6c51ceb9151298f21bb0ebfd696e57bd8d13fb
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943455"
---
# <a name="add-azure-partner-shared-services"></a>Azure Partner Shared Services の追加

**適用対象**

-  パートナー センター

Azure Partner Shared Services は、CSP プログラムのパートナー様向けの新しいプランの種類です。このプランでは、パートナー様自身が使用する Azure サブスクリプションを購入できます。  パートナーは、Azure のライセンスと再販契約を Microsoft と統合する機能に加えて、Azure の購入、追跡、および管理に対して統一された方法を使用する機会を提供します。 Azure Partner Shared Services の提供開始により、パートナー様は、Microsoft Enterprise Agreement および Web ダイレクト プログラムと同じように、CSP で柔軟に Azure サブスクリプションを利用できるようになりました。開発環境やテスト環境の構築、内部負荷の展開、共有サービスやマルチテナント アプリケーションのホスティングなどのシナリオにも対応できます。  

## <a name="create-the-shared-services-tenant"></a>共有サービス テナントを作成する

1. **[設定]**  >  **[View all settings]** (すべての設定を表示) >  **[共有サービス]** の順に移動します。

    ![**[アカウント設定]** の **[共有サービス]**](images/sharedservices2.png)

2. 共有サービス テナントをお持ちでない場合は、 **[Create shared services]** (共有サービスの作成) をクリックします。

    ![共有サービスの作成](images/sharedservices3.png)

3. これにより、共有サービス テナントが作成され、共有リソースや内部ワークロードで使用する Azure CSP Shared Services サブスクリプションの購入が行われます。

    ![テナントの作成とサブスクリプションの購入](images/sharedservices5.png)

## <a name="about-the-azure--internalshared-services-offer"></a>Azure - Internal/Shared Services プランについて

- Azure-Internal/Shared Services サブスクリプションは、パートナーセンターを通じてアクセスされる CSP の新しい Azure プランの種類であり、パートナーは Azure を独自に使用することができます。 

- Azure-Internal/Shared Services プランは割引およびインセンティブの対象ではありません。

- Azure - Internal/Shared Services プランは、共有サービス テナントにのみ適用できます。

- Azure-Internal/Shared Services サブスクリプションの主な用途は、独自の開発目的で Azure を使用できるようにすることです。 このプランのプロビジョニングに使用する共有テナントは、Office 365 や Dynamics のシートなどの他のサービスに使うことはできません。 

- サブスクリプションのキャンセルは、他のサブスクリプションと同様の方法で行うことができます。 **[設定]**  >  **[View all settings]** (すべての設定を表示) >  **[共有サービス]** の順に移動します。 Azure - Internal/Shared Services を選択して取り消します。

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Azure Partner Shared Services の利用状況の詳細にアクセスする

Azure の利用状況は、CSP 請求書と調整ファイルに記載されます。 請求書では、Microsoft Azure の明細項目の一部として含まれます。 利用状況の詳細は、このプラン用に作成されたテナントに対して記録された調整ファイルで参照できます。 

## <a name="azure-partner-shared-services-pricing"></a>Azure Partner Shared Services の価格

Azure Partner Shared Services の新しい価格ファイルを確認するには、 **[販売]**  >  **[料金とプラン]** の順に移動し、現在の月の価格表を選択します。 今後数週間のうちには、特定の価格カードの API もリリースされる予定です。

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>マーケットプレースのプランと Azure Partner Shared Services

2019 年 3 月 1 日時点で、Azure Partner Shared Services (APSS) ではマーケットプレースのプランがサポートされなくなります。   

|**マーケットプレースのサポート**   |**2019 年 3 月 1 日より前にサポートされる APSS**|**2019 年 3 月 1 日以降**|
|---------------------------|:----------------------------|:-------------------|
|ライセンス持ち込み (BYOL) と無料サービス   | [はい]   | 必須ではない|
|その他のサードパーティのマーケットプレースのプラン   | 必須ではない   |必須ではない|


APSS を使用して展開された BYOL または無料サービスを備えたパートナーには影響がありませんが、2019 年 3 月 1 日以降、新しい BYOL や無料サービスを購入することはできません。 

(BYOL や無料サービスだけでなく) 利用可能なすべてのマーケットプレースのプランを掲載するカタログを活用するには、CSP パートナーは Web ダイレクトの Azure サブスクリプションを使用して共有サービスを展開することをお勧めします。  以前よりマーケットプレースからサードパーティの BYOL と無料サービスのリソースを展開し、それらを引き続き使用してサードパーティのプランをさらに展開することを希望する CSP パートナーは、Web ダイレクト「[既存の Azure サブスクリプションを移行する](https://docs.microsoft.com/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)」に APSS サブスクリプションを移行することをお勧めします。

2019 年 3 月 1 日以降、APSS サブスクリプションを継続して使用し、新しいサードパーティの [BYOL サービス](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)または無料サービスを展開することを計画しているパートナーは、これらを APSS サブスクリプションに展開するために ISV からの指示に従います。

