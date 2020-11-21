---
title: Azure Marketplace からのソフトウェアとソリューションの購入
description: Azure Marketplace でソフトウェアの購入と管理を簡略化し、合理化するツールについて説明します。
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: b93ce1394326887b4265114c58527c36379101d9
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007243"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace での購入

Azure Marketplace には多数のツールと機能があり、購入ポリシーの購入、請求、管理のプロセスを簡略化し、合理化することができます。

## <a name="simplified-procurement"></a>簡素化された調達

Azure Marketplace は、さまざまな購入オプションを通じて調達プロセスを簡素化するために役立ちます。 Azure アカウントに関連付けられているクレジットカードを使用して製品を購入した場合、すべての購入は1つの請求書にまとめられ、選択したクレジットカードに請求されます。 大規模なお客様の場合は、マイクロソフトエンタープライズ契約を使用して購入できます。 EA を使用すると、すべてのソフトウェアの購入が Azure の請求書に自動的に含まれます。 請求書の項目は、Azure の使用量に応じた請求に、Azure Marketplace の請求が続く形になります。

Azure Marketplace を通じて購入すると、個々のベンダーと請求書の管理の複雑さが解消されます。 Azure Marketplace での購入と Azure の料金の両方を含む、Microsoft からの1つの統合月単位請求書を取得できます。

## <a name="permission-to-purchase"></a>購入するためのアクセス許可

適切なソフトウェアアプリケーションが見つかったら、購入を完了するのは簡単です。 ただし、Azure サブスクリプション内で適切なアクセス許可が必要になります。 Azure は [ロールベースの Access Control](https://docs.microsoft.com/azure/role-based-access-control/overview) (RBAC) モデルで動作するため、アカウントには購入を行うための **サブスクリプションの所有者** または **共同作成者** のアクセス許可が必要です。

購入を完了する前に、ユーザーが Azure テナントで正しい構成を持っていることを確認してください。 これは、購入時のエラーを防ぐのに役立ちます。

Azure portal の Azure Marketplace エクスペリエンスで、購入するアプリケーションを見つけ、[ **作成** ] または [セットアップ **+ サブスクライブ**] を選択します。 新しいソリューションを使用する前に、いくつかの情報を入力するように求められます。

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="オファーの [作成] ボタン。":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="[セットアップ + サブスクライブ] ボタン。":::

Azure Marketplace オンラインストアからソリューションをデプロイする場合は、[製品の説明] ページで [ **今すぐ入手** する] を選択し、azure アカウントの資格情報でサインインします。

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Azure Marketplace のサインインダイアログボックス。":::

サインインすると、Azure portal の製品にリダイレクトされ、購入が完了します。

## <a name="purchase-policy-management"></a>ポリシー管理の購入

Microsoft では、Azure サブスクリプション管理者として課金プロファイルを使用してユーザーの購入を管理できます。 次の 3 つのオプションから選択できます。

- **無料 + 有料** – Azure Marketplace ソフトウェアアプリケーションを取得することをユーザーに許可します。
- **Free** – Azure Marketplace から無料のソフトウェアのみをデプロイできます。
- [いいえ] –ユーザー **が** Azure Marketplace からソフトウェアをデプロイできないようにします。

これらの設定は、Azure サブスクリプションへのアクセス権を持つすべてのユーザーに適用されます。これにより、Azure portal を通じて IT 調達を制御できるようになります。

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Azure portal による IT 調達の制御":::

## <a name="cost-management"></a>コスト管理

Azure Marketplace から製品を購入すると、コストの管理に役立つ洞察を得ることができます。 Azure Cost Management は、購入した製品に関する情報を表示するための無料ツールです。 Cost Management を使用すると、時間の経過と共に使用しているサービスの詳細と、設定した予算に対してそれらのコストがどのように追跡されるかを確認できます。 予算を設定するだけでなく、レポートのスケジュールを設定したり、サブスクリプションのコストを分析したりすることもできます。 Azure Cost Management の詳細については、「 [コストの分析」と「Azure Cost Management を使用した予算の作成](https://docs.microsoft.com/learn/modules/analyze-costs-create-budgets-azure-cost-management/)」の「Microsoft Learn」モジュールを参照してください。

Azure Marketplace の料金と請求書は、Azure Cost Management の費用分析ツールで確認できます。

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Azure Cost Management を使用すると、購入した製品に関する洞察を得ることができます。":::

## <a name="next-steps"></a>次の手順

- [請求と請求](billing-invoicing.md)
