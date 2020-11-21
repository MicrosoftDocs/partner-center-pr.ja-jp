---
title: Azure Marketplace でのプライベートプラン
description: Azure Marketplace でのプライベートプランについて説明します。
ms.prod: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 055151f0420d642d591554a829dc21b69df84ebd
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007265"
---
# <a name="private-offers-in-azure-marketplace"></a>Azure Marketplace でのプライベートプラン

プライベートプランは、パブリッシャーが特定の顧客にカスタムプランを提供する方法です。 このオプションは現在、Azure portal の Azure Marketplace エクスペリエンスでのみサポートされています。 プライベートプランは、Azure portal から購入して直接インストールできる有料プランでのみ利用できます。 発行元は、ポータルからインストールできるかどうかに関係なく、コンサルティングサービス、アクション呼び出しとしての **連絡** を持つサービス、または無料サービスに対してプライベートプランを作成することはできません。

## <a name="find-private-offers-in-the-azure-portal"></a>Azure portal でのプライベートプランの検索

パートナーは、プライベートオファーを発行するときに、Azure portal の **Marketplace** セクションの対象ユーザーのみに表示されます。 これらのユーザーは、オファーの種類に応じて、サブスクリプション ID またはテナント ID によって定義されます。 プライベートプランの資格がある場合、ポータルでそれらを検索する方法は2つあります。

> [!NOTE]
> 現在、プライベートプランは、Azure portal で検索またはフィルターできません (カテゴリ別)。

Azure portal で、[ **+ リソースの作成** ] を選択するか、[marketplace] を検索して **marketplace** のページにアクセスします。 プライベートプランの資格をお持ちの場合は、ページの上部に **プライベートプランの利用可能なバナーが** 表示されます。 [プライベート **プランの表示** ] を選択して、プライベートプランページにアクセスします。

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="使用可能なプライベートプランがあるときに表示されるバナー。":::

または、[プライベートプラン] バナーが表示されている場合は、製品ギャラリーページの下部までスクロールしても、プライベートプランのサブセットが表示されます。 リンクを選択すると、プライベートプランページにアクセスするための **詳細が表示** されます。

:::image type="content" source="media/private-offers/see-more-link.png" alt-text="画面の下部にプライベートプランが表示され、[詳細を表示] リンクが表示されます。":::

## <a name="review-private-plans"></a>プライベートプランの確認

プライベートプランは、実際にはオファー内のプライベートプランです。 各プランには、パブリックとプライベートの両方の複数のプランを含めることができますが、プライベートプランはパブリックプランとは別のリストに記載されています。

使用可能なプライベートプランは、特徴的な **プライベート** バッジでマークされた [**プラン**] タブで確認できます。

:::image type="content" source="media/private-offers/private-badge.png" alt-text="プライベートとマークされたプランのページ。":::

複数のサブスクリプションがある場合は、すべてのサブスクリプションで利用可能なすべてのプライベートプランが表示されます。 [ **作成**] を選択すると、リソースの作成ページにルーティングされ、リソースの構成が開始されます。

[ **作成** ] を選択し、複数のサブスクリプションを持っていても、それらのすべてがプライベートプランに追加されていない場合は、既定のサブスクリプションがこのプライベートプランの対象となるサブスクリプションではない可能性があります。 この場合は、適切なサブスクリプションを選択します。

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="使用可能なプライベートプランが他にもあることを示すリンクが表示されます。":::

## <a name="next-steps"></a>次の手順

- [Azure Marketplace とは何ですか?](azure-marketplace-overview.md)
