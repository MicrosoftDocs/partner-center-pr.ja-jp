---
title: Azure Marketplace からソフトウェアとソリューションを購入する
description: ソフトウェアの購入と管理を簡素化および合理化するツールについて、Azure Marketplace。
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: 11145280aad1ecd9777ec2fb7540e7d6479acfae
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431542"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace購入

Azure Marketplaceには、購入、請求、および購入ポリシーの管理のプロセスを簡素化および合理化する多数のツールと機能があります。

## <a name="simplified-procurement"></a>簡略化された調達

Azure Marketplace は、さまざまな購入オプションを通じて調達プロセスを簡素化するために役立ちます。 Azure アカウントに関連付けられているクレジット カードを使用して製品を購入した場合、すべての購入は 1 つの請求書に統合され、選択したクレジット カードに請求されます。 大規模な顧客の場合は、大規模な顧客を使用して購入Enterprise Agreement。 EA では、すべてのソフトウェア購入が Azure 請求書に自動的に含まれます。 請求書の項目は、Azure の使用量に応じた請求に、Azure Marketplace の請求が続く形になります。

サービスを通じて購入Azure Marketplace、個々のベンダーの関係と請求書を管理する複雑さを排除できます。 Microsoft から 1 つの統合された月次請求を受け取り、その請求書には、Azure Marketplace購入と Azure の料金の両方が含まれます。

## <a name="permission-to-purchase"></a>購入のアクセス許可

適切なソフトウェア アプリケーションが見つかったら、購入を完了することは簡単です。 ただし、Azure サブスクリプション内で適切なアクセス許可が必要です。 Azure はロール ベースのロール ベース Access Control (RBAC) モデルで動作します。アカウントには、購入を行うサブスクリプション所有者または共同作成者のアクセス許可が必要です。 [](/azure/role-based-access-control/overview)

購入を完了する前に、ユーザーが Azure テナントで正しい構成を持していることを確認します。 これは、購入中のエラーを防ぐのに役立ちます。

アプリのAzure MarketplaceエクスペリエンスでAzure portalするアプリケーションを見つけて、[作成] または [設定とサブスクライブ]**を選択します**。 新しいソリューションを使用する前に、いくつかの情報を入力するように求めるメッセージが表示されます。

> [!CAUTION]
> プライベート マーケットプレースへの承認は、ソリューションの調達を示すのではありません。

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="オファーの [作成] ボタン。":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="[セットアップとサブスクライブ] ボタン。":::

Azure Marketplace オンライン ストアからソリューションをデプロイする場合は、製品の説明ページで [今すぐ取得] を選択し、Azure アカウントの資格情報でサインインします。

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="[Azure Marketplace] ダイアログ ボックス。":::

サインインすると、購入を完了するために、Azure portal製品にリダイレクトされます。

## <a name="purchase-policy-management"></a>購入ポリシー管理

Microsoft では、Azure サブスクリプション管理者として課金プロファイルを使用してユーザーの購入を管理できます。 次の 3 つのオプションから選択できます。

- **無料 + 有料** – ユーザーは、任意のソフトウェア アプリケーションAzure Marketplace取得できます。
- **[無料** ] – ユーザーが無料のソフトウェアのみを展開Azure Marketplace。
- **[いいえ** ] – ユーザーがソフトウェアを展開Azure Marketplace。

これらの設定は、Azure サブスクリプションにアクセスできるすべてのユーザーに適用されます。これにより、Azure サブスクリプションを通じて IT 調達を制御Azure portal。

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="IT 調達を管理するAzure portal。":::

## <a name="cost-management"></a>コスト管理

顧客から製品を購入するAzure Marketplace、コストの管理に役立つ分析情報を得る必要があります。 Azure Cost Managementは、購入した製品に関する情報を表示する無料のツールです。 Cost Managementを使用して、時間の費やしているサービスの詳細と、設定した予算に対してそれらのコストがどのように追跡されるのかを確認できます。 予算の設定に加えて、レポートをスケジュールし、サブスクリプションのコストを分析できます。 コストの分析とAzure Cost Managementの作成に関するMicrosoft Learnモジュールを完了して、コストの詳細を[確認Azure Cost Management。](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)

Azure Marketplace の料金と請求書は、Azure Cost Management の費用分析ツールで確認できます。

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="購入Azure Cost Managementに関する分析情報を取得するには、次のコマンドを使用します。":::

## <a name="purchase-validation-checks"></a>購入の検証チェック

サービスを通じてオファー Azure Marketplace、さまざまな理由で失敗する可能性があります。 購入にコマンド ライン インターフェイス (CLI) を使用すると、Azure Marketplace で使用できないオファーを購入しようとしている可能性が高く、エラーが発生する可能性があります。 購入が失敗する可能性があるチェックを次に示します。

1. サブスクリプションは、サブスクリプション (EA) Enterprise Agreementに属し、EA 管理者は購入をAzure Marketplaceします。
1. EA 管理者は無料オファーに対してだけ購入を有効にし、オファーは有料オファーです。
1. オファーがマーケットプレースに見つかりません。
1. 独立系ソフトウェア ベンダー (ISV) は、少なくともお客様のリージョンでオファーの販売を停止しました。
1. 使用しているサブスクリプションは、オファーが利用できないリージョンの課金アカウントに属しています。
1. サブスクリプション/課金アカウントは、有効な支払い方法 (有効なクレジット カードなど) に関連付けされません。
1. サブスクリプションは CSP (クラウド ソリューション プロバイダーに属し、ISV は CSP を通じた販売を拒否しました。
1. プライベート マーケットプレースはサブスクリプションに対して有効であり、オファーは許可されているオファーの一覧に含め "されません"。
1. オファーは特定の顧客に対してプライベート/プレビューであり、サブスクリプションは許可された顧客の一覧に含めではありません。

## <a name="next-steps"></a>次の手順

- [請求と請求書作成](billing-invoicing.md)