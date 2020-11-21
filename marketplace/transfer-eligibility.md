---
title: 譲渡資格–請求先アカウント間でのサブスクリプションの譲渡に関するガイドライン (Azure Marketplace)
description: Azure portal 内の請求先アカウント間でサブスクリプションを転送する前の商用小切手のガイドライン。
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007220"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>課金アカウント間のサブスクリプションの資格を譲渡する

[サブスクリプションは](/azure/cost-management-billing/understand/subscription-transfer)、Azure portal の [課金] セクションで、1つの請求アカウントから別のアカウントに転送できます。 転送前に、サードパーティ製品のサブスクリプションがスキャンされます。 転送は *すべて* の製品に対してクリアされている場合にのみ許可されます (以下の [条件](#criteria-for-transfer-approval-or-denial) を参照)。 システムは、次の手順を決定するのに役立つように、クリアされなかったアプリに関連するエラーメッセージを生成します。

> [!NOTE]
> Saas リソースはサブスクリプションではなくテナントに関連付けられているため、この記事は SaaS プランには適用されません。 SaaS リソースは課金アカウント間で転送されますが、これはリソースごとに、Azure サポートによってサポート要求として行われます。

## <a name="criteria-for-transfer-approval-or-denial"></a>転送の承認または拒否の条件

いずれかのサードパーティ製アプリが次のいずれかの条件を満たしている場合は、サブスクリプションを転送できません。

- ターゲットアカウントは商用で、アプリはパートナーによって販売されることがオプトアウトされます。
- 選択したパートナーのアプリがオプトインされていますが、対象のアカウントが許可リストに含まれていません。
- プランは、選択したサブスクリプションについて過去に提供されていたプレビュー版であったか、またはプライベートプランだったので、許可リストに登録されていません。
- 新しい請求先アカウントは、プランが販売されているリージョンとは異なるリージョンにあり、そのリージョンでプランを販売することはできません。

ブロックされた転送は、サブスクリプションからリソースを削除するまで有効です。その後、転送を再試行することができます。

## <a name="next-steps"></a>次の手順

[Microsoft AppSource と Azure Marketplace のサポートを受ける](get-support.md)

