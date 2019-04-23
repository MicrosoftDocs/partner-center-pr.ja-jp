---
title: Azure Marketplace の製品にサブスクリプションを販売 |パートナー センター
ms.topic: article
ms.date: 04/04/2019
description: パートナー センターを使用するには (SaaS) サービスとしてソフトウェアへのサブスクリプションを顧客に販売する製品は独立系ソフトウェア ベンダー (Isv) によって、Azure Marketplace に公開します。
author: JnHs
ms.author: jenhayes
keywords: サブスクリプションの場合、Marketplace でサード パーティの ISV
ms.localizationpriority: medium
ms.openlocfilehash: a086ab3a58e926d33c118690e7b171ba4f0fd18b
ms.sourcegitcommit: 41b6e677db10ef8e5d12f9240d3450f085ee6d91
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2019
ms.locfileid: "60124273"
---
# <a name="sell-subscriptions-to-azure-marketplace-products"></a>Azure Marketplace 製品にサブスクリプションを販売する

**適用対象**

- パートナー センター

パートナー センターを使用するにはサービス (SaaS) 製品に公開と、お客様は、サブスクリプション ソフトウェアを販売する[Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace)独立系ソフトウェア ベンダー (Isv) によって。 こうと、ビジネスを区別して、特定のビジネス ニーズに対応するソフトウェア バンドルをお客様に提供します。 Microsoft 製品と同様のライセンスとこれらの Azure Marketplace の SaaS 製品のサブスクリプションを管理します。

Azure Marketplace の詳細については、次を参照してください。 [Azure Marketplace Faq](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide)します。

## <a name="view-marketplace-offers-and-pricing"></a>ビューの Marketplace プランと価格

すべての可能なプランを表示する選択**Marketplace**左側のナビゲーション メニューから。 既定では、すべての種類とカテゴリの製品を確認します。 型や、カテゴリによるフィルター処理したり、特定のキーワードを検索する検索ボックスを使用できます。 パブリッシャーと利用可能な Sku に関する情報を確認する製品を選択します。

> [!NOTE]
> Azure Marketplace で利用できる一部の製品がここに表示されません。 Isv は、パートナー センターでクラウド ソリューション プロバイダー (CSP) パートナーに自社製品を提供するかどうかを決定できます。 たいパートナー センターを介して顧客に提供する Azure Marketplace で製品を表示する場合は、Azure Marketplace で発行元の連絡先情報を見つけるし、関心があることを伝えてください。

Azure Marketplace の製品の価格は、頻繁に変更できます。 Marketplace のすべての製品の現在の価格情報を取得する次のように選択します。**エクスポート価格表**の右上隅にある、 **Marketplace**ページ。 これにより、すべての価格データを含むスプレッドシートが生成されます。 価格情報を現在の価格を取得するには、何度でもチェックできるように、1 日が更新されます。

## <a name="purchase-marketplace-products-for-your-customers"></a>Marketplace の製品をお客様を購入します。

Azure Marketplace の SaaS 製品のサブスクリプションを購入、サブスクリプションの Microsoft 製品の購入方法と同じプロセスに従います。 顧客のサブスクリプションを追加するときにのみ Marketplace が提供する Isv から選択して表示することができます**パートナー**で、**パブリッシャー**フィルター。 詳細については、次を参照してください。[サブスクリプションの新規作成](create-a-new-subscription.md)です。

> [!IMPORTANT]
> パートナー センターでサービス (SaaS) 製品のサブスクリプションとしてソフトウェアを購入することのみできます。 (Azure アプリケーション、コンテナー、または Vm) などの他のオファーの種類は、Azure portal を使用して管理し、使用量に応じて課金されます。 Azure portal での従量課金制のソリューションを有効にするために既存の Azure サブスクリプションが必要です。

表示を提供するいくつかに注意してください、 **Marketplace**ページは、特定の顧客に利用できない可能性があります。 可用性は、さまざまな ISV が顧客の請求先の国/地域をサポートしているかどうかなどの要因によって受ける可能性があります。

> [!TIP]
> 使用することも[パートナー センター Api](https://docs.microsoft.com/partner-center/develop/)お客様の Azure Marketplace のサブスクリプションを作成します。 詳細については、次を参照してください。 [Azure Marketplace の製品のサブスクリプションを作成](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)です。

Azure Marketplace の製品にサブスクリプションを使用するためのオプションがある[、サブスクリプションを取り消す](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription)キャンセル期間 (月単位のサブスクリプションまたは年間サブスクリプションは 14 日間は 24 時間) 内で。 できます[、サブスクリプションを自動的に更新するかどうかを選択](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription)します。

## <a name="access-billing-info-for-marketplace-products"></a>Marketplace の製品の課金情報にアクセスします。

、Marketplace の製品は、請求期間は、カレンダー月の最初の日を開始し、カレンダー月の最終日に終了します。 しましょう、請求書利用可能な次の月の第 8 日にします。 パートナー センターで、またはパートナー センター Api を使用してこれらの請求書にアクセスできます。

詳細については、次を参照してください。[パートナー センターでの課金の種類について](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges)します。

## <a name="provide-support-for-customers-using-marketplace-products"></a>Marketplace の製品を使用して顧客のサポートを提供します。

Microsoft の製品と同様に、請求とサブスクリプションの管理に関する質問について、お客様の連絡先の最初のポイントがあります。 テクニカル サポートでは、発行元に問い合わせる必要があります。 Microsoft では、Marketplace の製品のサポートは提供されませんを発行元のサポートの連絡先情報を提供します。

詳細については、次を参照してください。 [Azure Marketplace の製品サポート](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-azure-marketplace-products)と[サポートを顧客に提供する](https://docs.microsoft.com/partner-center/customer-support)します。

## <a name="manage-subscriptions-using-partner-center-apis"></a>パートナー センター Api を使用してサブスクリプションを管理します。

Azure Marketplace の製品の市場のプランの一覧を取得、作成、Azure Marketplace サブスクリプションの場合、注文を送信し、ライセンス認証リンクを取得するパートナー センター Api を使用してサブスクリプションを作成することができます。 ライフ サイクル管理を行って、これらのサブスクリプションの請求書を管理するパートナー センター Api を使用することもできます。

詳細については、次を参照してください。 [Azure Marketplace の製品のサブスクリプションを作成](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)です。