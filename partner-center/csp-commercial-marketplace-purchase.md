---
title: 顧客向けの市販の marketplace 製品またはプランを購入する |パートナーセンター
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP プログラムパートナーがパートナーセンターマーケットプレースを使用して、独立系ソフトウェアベンダー (Isv) から SaaS プランを購入できるようにする方法について説明します。
author: MicheleHope
ms.author: v-mihope
keywords: サブスクリプション、marketplace、商業市場、サードパーティ、ISV、SaaS プラン、クラウドソリューションプロバイダープログラム、プランの購入、サブスクリプションの購入
ms.localizationpriority: medium
ms.openlocfilehash: 3dd3facf79e0e33a6dfc35a162c444a13a19b256
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253800"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>パートナーセンターで顧客向けの商用 marketplace 製品を購入する

**適用対象**

- パートナー センター
- CSP プログラムのパートナー

**適切なロール**

- 全体管理者
- 管理エージェント

クラウドソリューションプロバイダー (CSP) プログラムのパートナーとして、商用マーケットプレースを使用して、独立系ソフトウェアベンダー (Isv) によって提供される特定のサービスとしてのソフトウェア (SaaS) 製品に対して顧客のサブスクリプションを購入することができます。 

顧客に対して ISV SaaS サブスクリプションを提供することにより、ビジネスを差別化することができます。 また、特定のビジネスニーズに対応するソフトウェアバンドルへのアクセス権を顧客に与えることもできます。 これらの marketplace SaaS 製品のライセンスとサブスクリプションは、Microsoft 製品のライセンスとサブスクリプションを管理するのと同じように、ISV 発行元から管理します。

**ライセンスベース**の SaaS サブスクリプションまたは**使用状況ベースの**サブスクリプションのいずれかを購入できます。 ライセンスベースと使用量ベースの課金の違いの詳細については、[課金の基本](billing-basics.md)に関するページを参照してください。

## <a name="purchase-license-based-saas-subscriptions-in-partner-center"></a>パートナーセンターでライセンスベースの SaaS サブスクリプションを購入する

Microsoft 製品のサブスクリプションを購入する場合と同じプロセスを使用して、ISV 発行元によって提供されるライセンスベースの SaaS 製品のサブスクリプションを購入します。

パートナーセンターでライセンスベースの SaaS サブスクリプションを購入するには、「[顧客サブスクリプションの作成、中断、キャンセル](create-a-new-subscription.md#create-a-new-subscription)」を参照してください。

[パートナー センター API](https://docs.microsoft.com/partner-center/develop/) を使って、顧客向けの商用マーケットプレース サブスクリプションを作成することもできます。 (パートナーセンター Api の使用方法の詳細については、「[商用 marketplace 製品のサブスクリプションを作成する](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)」を参照してください)。

>[!IMPORTANT]
> CSP プログラムのパートナーは、パートナーセンター内の ISV 発行元から**ライセンスベース**の SaaS サブスクリプションのみを購入できます。 つまり、ISV 発行者が利用可能にした**ライセンスベース**の SaaS プランを購入できます。これには、アクセス権を持つ[限定プラン](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)も含まれます。 Isv (Azure アプリケーション、コンテナー、または Vm を含む**使用量ベース**、従量制課金、消費量ベースのプランなど) から、他の商用 marketplace プランを購入または管理するには、 [azure 管理ポータル](https://portal.azure.com/)にアクセスする必要があります。 詳細については、次のトピックを参照してください。

## <a name="purchase-usage-based-subscriptions-in-the-azure-management-portal"></a>Azure 管理ポータルで使用量ベースのサブスクリプションを購入する

サードパーティの ISV 発行元からのライセンスベースの SaaS サブスクリプションとは異なり、使用量ベースのサブスクリプションでは、まず、顧客が Azure サブスクリプションを持っている必要があります。 商用 marketplace の課金、使用量ベースのリソースは、お客様の Azure サブスクリプションの下に分類されます。 顧客が Azure サブスクリプションを持っている場合、CSP プログラムのパートナーは、次の手順に従って、これらのサービスに対して商用の marketplace サブスクリプションを購入できます。

1. パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard)にサインインし、左側のメニューから [Customers] \ (**顧客**\) を選択します。

2. 特定の顧客を選択し、 **[サブスクリプション]** を選択します。  

3. **[使用量ベースのサブスクリプション]** で、 **[すべてのリソース]** を選択します。 これにより、Azure 管理ポータルに移動します。

4. Microsoft Azure 管理ポータルで、左側のメニューから **[リソースの作成]** を選択します。

5. Azure Marketplace の一覧の上部にある **[すべて表示]** を選択します。

6. リストを絞り込むには、Marketplace の一覧の上部にあるフィルターを使用します。 たとえば、 **[発行元]** ドロップダウンリストから**Microsoft**または**Partner**を選択すると、microsoft または ISV 発行元からのオファーのみを表示できます。

7. 特定のプランを選択し、 **[作成]** を選択します。

## <a name="next-steps"></a>次の手順

- [市販の marketplace プランを管理する](csp-commercial-marketplace-purchase.md)