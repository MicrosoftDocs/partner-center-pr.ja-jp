---
title: Azure Partner Shared Services の追加 | パートナー センター
ms.topic: article
ms.date: 03/15/2019
description: Azure Partner Shared Services は、CSP プログラムのパートナー様向けの新しいプランの種類です。このプランでは、パートナー様自身が使用する Azure サブスクリプションを購入できます。
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, Shared Services, テナント
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: bfdb82d0698f2e0aba3f5284a53fe22010efc0da
ms.sourcegitcommit: f916aa2884239b205398c24d04d1f1dc41b63c2b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/28/2019
ms.locfileid: "64666896"
---
# <a name="add-azure-partner-shared-services"></a>Azure Partner Shared Services の追加

**適用対象**

-  パートナー センター

Azure Partner Shared Services は、CSP プログラムのパートナー様向けの新しいプランの種類です。このプランでは、パートナー様自身が使用する Azure サブスクリプションを購入できます。  パートナーにとっては、Microsoft との Azure ライセンス契約および再販契約を集約できるだけでなく、統一された方法で Azure を購入、追跡、管理できるようになります。 Azure Partner Shared Services の提供開始により、パートナー様は、Microsoft Enterprise Agreement および Web ダイレクト プログラムと同じように、CSP で柔軟に Azure サブスクリプションを利用できるようになりました。開発環境やテスト環境の構築、内部負荷の展開、共有サービスやマルチテナント アプリケーションのホスティングなどのシナリオにも対応できます。  

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

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>マーケットプレースのプランと Azure Partner Shared Services

2019 年 3 月 1 日時点で、Azure Partner Shared Services (APSS) ではマーケットプレースのプランがサポートされなくなります。   

|**マーケットプレースのサポート**   |**2019 年 3 月 1 日より前にサポートされる APSS**|**2019 年 3 月 1 日以降**|
|---------------------------|:----------------------------|:-------------------|
|ライセンス持ち込み (BYOL) と無料サービス   | 〇   | X|
|その他のサードパーティのマーケットプレースのプラン   | X   |X|


APSS を使用して展開された BYOL または無料サービスを備えたパートナーには影響がありませんが、2019 年 3 月 1 日以降、新しい BYOL や無料サービスを購入することはできません。 

(BYOL や無料サービスだけでなく) 利用可能なすべてのマーケットプレースのプランを掲載するカタログを活用するには、CSP パートナーは Web ダイレクトの Azure サブスクリプションを使用して共有サービスを展開することをお勧めします。  以前よりマーケットプレースからサードパーティの BYOL と無料サービスのリソースを展開し、それらを引き続き使用してサードパーティのプランをさらに展開することを希望する CSP パートナーは、Web ダイレクト「[既存の Azure サブスクリプションを移行する](https://docs.microsoft.com/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)」に APSS サブスクリプションを移行することをお勧めします。

2019 年 3 月 1 日以降、APSS サブスクリプションを継続して使用し、新しいサードパーティの [BYOL サービス](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)または無料サービスを展開することを計画しているパートナーは、これらを APSS サブスクリプションに展開するために ISV からの指示に従います。

