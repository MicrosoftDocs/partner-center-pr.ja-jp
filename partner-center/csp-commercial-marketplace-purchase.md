---
title: コマーシャル マーケットプレース のオファーを購入する
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP プログラム パートナーが、パートナー センター Marketplace を使用して、独立系ソフトウェア ベンダー (ISV) から SaaS オファーを顧客が購入する方法について説明します。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f5cf4895fa4d66c65215989d808a1dd18ef9064
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147855"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>顧客向けコマーシャル マーケットプレース製品を購入するパートナー センター


**適切なロール**: グローバル管理者|管理エージェント

クラウド ソリューション プロバイダー (CSP) プログラムのパートナーは、コマーシャル マーケットプレースを使用して、独立系ソフトウェア ベンダー (ISV) によって提供される特定のサービスとしてのソフトウェア (SaaS) 製品に対する顧客のサブスクリプションを購入できます。

ISV SaaS サブスクリプションを顧客に提供することで、ビジネスの差別化に役立ちます。 また、特定のビジネス ニーズに対応するソフトウェア バンドルへのアクセス権を顧客に提供することもできます。 これらのマーケットプレース SaaS 製品のライセンスとサブスクリプションは、Microsoft 製品のライセンスとサブスクリプションを管理するのと同じ方法で ISV 発行元から管理します。

ライセンス ベースの SaaS **サブスクリプションまたは** 使用量ベースのサブスクリプション **を購入** できます。 ライセンス ベースと使用量ベースの課金の違いの詳細については、「課金の基本」 [を参照してください](billing-basics.md)。

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>ライセンスベースの SaaS サブスクリプションと測定された SaaS サブスクリプションをパートナー センター

ISV 発行元が提供するライセンスベースまたは測定された SaaS 製品のサブスクリプションは、Microsoft 製品のサブスクリプションの購入に使用するのと同じプロセスを使用して購入します。

パートナー センター でライセンスベースまたは測定された SaaS サブスクリプションを購入するには、「顧客サブスクリプションの作成、中断、または取り消し」 [を参照してください](create-a-new-subscription.md#create-a-new-subscription)。

[パートナー センター API](/partner-center/develop/) を使って、顧客向けの商用マーケットプレース サブスクリプションを作成することもできます。 (API の使用の詳細パートナー センター、コマーシャル マーケットプレース製品のサブスクリプションの作成 [に関するページを参照してください](/partner-center/develop/create-subscription-azure-marketplace-products)。

>[!IMPORTANT]
> CSP プログラムのパートナーは、ライセンスベースまたは測定された **SaaS** サブスクリプションを、パートナー センター 内の ISV パブリッシャーから購入できます。 つまり、ISV 発行元が利用できるライセンスベースまたは測定された **SaaS** オファー (アクセス権を持 [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)つ排他的なオファーを含む) を購入できます。 Isv (Azure アプリケーション、コンテナー、または Vm を含む使用量ベースのプランなど) から、他の商用 marketplace プランを購入または管理するには、 [Azure portal](https://portal.azure.com/)にアクセスする必要があります。

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Azure portal で使用量ベースのサブスクリプションを購入する

サードパーティの ISV 発行元からのライセンスベースの SaaS サブスクリプションとは異なり、使用量ベースのサブスクリプションでは、まず、顧客が Azure サブスクリプションを持っている必要があります。 商用 marketplace の課金、使用量ベースのリソースは、お客様の Azure サブスクリプションの下に分類されます。 顧客が Azure サブスクリプションを持っている場合、CSP プログラムのパートナーは、次の手順に従って、これらのサービスに対して商用の marketplace サブスクリプションを購入できます。

1. パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインし、左側のメニューから [Customers] \ ( **顧客** \) を選択します。

2. 特定の顧客を選択し、[ **サブスクリプション**] を選択します。  

3. [ **使用量ベースのサブスクリプション**] で、[ **すべてのリソース**] を選択します。 これにより、Azure 管理ポータルに移動します。

4. Microsoft Azure 管理ポータルで、左側のメニューから [ **リソースの作成** ] を選択します。

5. Azure Marketplace の一覧の上部にある [ **すべて表示** ] を選択します。

6. リストを絞り込むには、Marketplace の一覧の上部にあるフィルターを使用します。 たとえば、[**発行元**] ドロップダウンリストから **Microsoft** または **Partner** を選択すると、microsoft または ISV 発行元からのオファーのみを表示できます。

7. 特定のプランを選択し、[ **作成**] を選択します。

## <a name="next-steps"></a>次のステップ

- [市販の marketplace プランを管理する](csp-commercial-marketplace-purchase.md)