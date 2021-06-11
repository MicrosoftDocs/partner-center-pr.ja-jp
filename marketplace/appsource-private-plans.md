---
title: プライベート プラン (Microsoft AppSource
description: プライベート プランを Microsoft AppSource (Azure Marketplace) で設定します。
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: a576c9606ade59cef7d0b2d5e1584016740d08eb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2021
ms.locfileid: "112008552"
---
# <a name="private-plans-in-microsoft-appsource"></a>プライベート プラン (Microsoft AppSource

プライベート プランは、発行元が特定の顧客にカスタム プランを提供する方法です。 このオプションは、次のMicrosoft AppSource。 プライベート プランは、AppSource でサービスとしてのソフトウェア (SaaS) オファーに対して販売できます。このプランは、今すぐ使用する行動を呼び出します。

## <a name="ask-your-isv-for-a-private-plan"></a>ISV にプライベート プランを求める

AppSource でプライベート プランを利用するには、ISV に直接問い合わせ、カスタム価格と技術仕様をネゴシエートする必要があります。 プライベート プランの条項に同意すると、ISV によって自動的にプランが作成され、組織のテナント ID に割り当てる必要があります。

### <a name="finding-your-tenant-id"></a>テナント ID の検索

1. AppSource の右上隅にあるアカウント プロファイル アイコンを選択し、[テナントの表示] **を選択します**。
2. テナント ID をコピーし、ISV に指定します。

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="テナント ID を検索する方法を示します。":::

## <a name="find-a-private-plan-in-appsource"></a>AppSource でプライベート プランを検索する

ISV が新しいプライベート プランを発行してから AppSource に表示するには、最大で 48 時間かかる場合があります。 テナント ID に関連付けられているプライベート プランを見つけるには、AppSource の右上にある [プライベート プラン] **(ロック** アイコン) を選択します。

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="上部のツール バーにロック アイコン (ロックロック) が表示されます。":::

サインインしていない場合は、メッセージが表示されます。 その後、[プランと価格] タブで、テナント ID に関連付 **けられているプライベート プランを購入** できます。

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="[プランと価格] タブにプライベート オファーが表示されます。":::

テナントでプライベート プランを使用できない場合は、プライベート プランやオファーを持たなかったというメッセージが表示されます。

## <a name="purchase-a-private-plan"></a>プライベート プランを購入する

ISV には、オファー内に 1 つ以上のプライベート プランを含めできます。 各オファーはパブリックプランとプライベート プランの両方を持つ場合がありますが、プライベート プランは、ページの右上にあるプライベート オファー アイコン (ロック) からアクセスされる個別のオファー登録情報ページの下に表示されます。

[プランと価格] タブに、使用可能 **なプライベート プランが表示** されます。プライベート プランには、独特の青いバッジが付きます。

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="プライベート オファーの横に青いプライベート オファー バッジが表示されます。":::

選択したプランを購入するには、[今すぐ取得] **を選択** し、提供されている手順に従います。

## <a name="next-steps"></a>次のステップ

- [Microsoft AppSource とは](appsource-overview.md)
