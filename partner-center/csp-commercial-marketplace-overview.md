---
title: 概要-CSP marketplace
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Marketplace の独立系ソフトウェアベンダー (Isv) のサービスとしてのソフトウェア (SaaS) プランに対する顧客のサブスクリプションを販売する方法について説明します。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6b914d6dbd69f374976584d1261382ef8fe9ded9
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979449"
---
# <a name="overview-of-the-commercial-marketplace-in-partner-center"></a>パートナー センターのコマーシャル マーケットプレースの概要

**適切なロール**

- グローバル管理者

クラウドソリューションプロバイダー (CSP) プログラムのパートナーになると、サードパーティの独立系ソフトウェアベンダー (Isv) によって発行されたソリューションと共に、Microsoft 製品をバンドルして販売することができます。 この方法でソリューションをバンドルできるため、エンドカスタマーにサービスを提供し、CSP サービスビジネスを拡大することができます。

CSP プログラムのパートナーとして、パートナーセンターを使用して、Microsoft の商用マーケットプレースから多数の ISV ソリューションを購入することができます。 これにより、ユーザーと顧客はいくつかの重要な利点を得ることができます。

- Microsoft のテクノロジと環境に合わせて最適化されたソフトウェアソリューションのカタログへのアクセス。
- シンプルなコントラクトと短縮された調達サイクル。
- パートナーセンター Api との単一の統合。 (この統合により、ISV ソリューションのカタログへのアクセスが可能になり、運用とエンジニアリングのコストが削減され、1つのプロバイダーを通じて複数のベンダーサブスクリプションと請求の管理が効率化されます)。
- お客様の Azure テナントでのデプロイとプロビジョニングの合理化 (仮想マシンベースのソリューションの場合)。
- 直接 ISV の購入や契約、Microsoft ソリューションの構成と統合、複数のベンダーからの定期的な請求書の管理または統合に関する潜在的な課題を軽減します。

## <a name="overview-of-csp-offers-in-the-commercial-marketplace"></a>商用マーケットプレースにおける CSP の提供の概要

CSP プログラムのパートナーである場合は、ISV のオファーに関して、多くの市販の marketplace アクティビティを実行する必要があります。 各アクティビティの詳細については、次の表を参照してください。

|**必要に応じて**  |**読み取り**   |
|:------------------------------------|:------------------|
|利用可能なプラン、価格、製品の詳細、または発行者の連絡先情報を表示または検索する方法について説明します | [オファーの検出](csp-commercial-marketplace-discover.md) | 
|プランを購入して展開する方法について説明します   | [購入プラン](csp-commercial-marketplace-purchase.md)   | 
|サブスクリプションをキャンセルまたは更新する方法、またはライセンスを追加または削除する方法について説明します。  | [オファーの管理](csp-commercial-marketplace-manage.md) |
|商用 marketplace での購入に対する課金のしくみについて説明します | [課金について](csp-commercial-marketplace-billing.md) |
|ISV が購入できるサポートの種類について説明します。 | [サポートについて](csp-commercial-marketplace-support.md) |
|商用マーケットプレースにおける CSP パートナーと Isv の契約および責任について説明します。 | [コントラクトについて](csp-commercial-marketplace-contracting.md) |

> [!NOTE]
> この概要では、CSP プログラムのパートナーがパートナーセンターで特定の商用 marketplace 機能を使用する方法について説明します。 CSP プログラムのパートナーとは異なり、ISV 発行者には異なる marketplace ロールがあります。 また、パートナーセンター内で使用できるさまざまな商用 Marketplace 機能もあります。 ISV 発行元の役割の詳細については、「 [Azure の商用 Marketplace の概要](/azure/marketplace/partner-center-portal/commercial-marketplace-overview)」を参照してください。

## <a name="where-to-complete-commercial-marketplace-activities"></a>コマーシャルマーケットプレースアクティビティを完了する場所

CSP プログラムのパートナーとして、パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard) から、または [パートナーセンター api](/partner-center/develop/)を使用して、ISV SaaS プランの多くの商用マーケットプレースアクティビティを直接完了できます。 ただし、他の marketplace アクティビティを完了するには、次の手順に進む必要があります。

- [Microsoft Azure 管理ポータル](https://portal.azure.com/)

    または

- サードパーティの ISV 発行元のシステムまたは web サイト

活動を完了する多くの部分は、選択したオファーの種類から始まります。 CSP プログラムのパートナーは、現在、サードパーティの ISV 発行元との2種類のプランを利用できます。

1. ライセンスベースの SaaS プラン  
2. 使用量ベースのプラン (仮想マシン、コンテナー、または Azure アプリケーションに基づくオファーを含む)

ライセンスベースのプランと使用量ベースのプランとの課金の違いについては、 [課金の基本](billing-basics.md) に関するページを参照してください。  

ライセンスベースまたは使用量ベースの ISV プランで特定の marketplace アクティビティを完了する場所については、次の表を参照してください。

|**Isv からのライセンスベースまたは従量制の SaaS プランの場合**  |**用途**  |
|:------------------------------------|:------------------|
|利用可能なプランを検出または検索するには  | パートナーセンターのダッシュボードまたはパートナーセンターの Api  |
|プランを購入するには  | パートナーセンターのダッシュボードまたはパートナーセンターの Api  |
|購入したプラン (アカウントのセットアップ、ソフトウェアの管理、または顧客の AAD テナントへのデプロイ) をデプロイするには  | ISV 発行元のシステムまたは web サイト  |
|プランのサブスクリプションの取り消し/更新、またはライセンスの追加/削除を行うには | パートナーセンターのダッシュボードまたはパートナーセンターの Api  |
|ユーザーを作成したり、アクセス許可を管理したりするには  | ISV 発行元のシステムまたは web サイト  |

|**Isv からの使用量ベースのオファー**  |**用途**  |
|:------------------------------------|:------------------|
|利用可能なプランを検出または検索するには  | パートナーセンターのダッシュボード、パートナーセンターの Api、または Azure portal  |
|プランを購入するには  | Azure portal  |
|購入したプラン (アカウントのセットアップ、ソフトウェアの管理、または顧客の AAD テナントへのデプロイ) をデプロイするには  | Azure portal  |
|プランのサブスクリプションの取り消し/更新、またはライセンスの追加/削除を行うには | Azure portal  |
|ユーザーを作成したり、アクセス許可を管理したりするには  | Azure portal  |

## <a name="next-steps"></a>次のステップ

- [市販の marketplace プランを検出または表示する](csp-commercial-marketplace-discover.md)
- [商用 marketplace プランの購入](csp-commercial-marketplace-purchase.md)
