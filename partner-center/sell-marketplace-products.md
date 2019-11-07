---
title: 商用マーケットプレース製品にサブスクリプションを販売する | パートナー センター
ms.topic: article
ms.date: 08/16/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナー センターを使用して、貴社の顧客に、独立系ソフトウェア ベンダー (ISV) によって商用マーケットプレースに発行されたサービスとしてのソフトウェア (SaaS) 製品に対するサブスクリプションを販売できます。
author: JnHs
ms.author: jenhayes
keywords: サブスクリプション, Marketplace, サード パーティ, ISV
ms.localizationpriority: medium
ms.openlocfilehash: bf3ad75f4bac84163efb4a67009a5d4d7f2261d5
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/06/2019
ms.locfileid: "73651635"
---
# <a name="sell-subscriptions-to-commercial-marketplace-products"></a>商用マーケットプレース製品にサブスクリプションを販売する

**適用対象**

- パートナー センター

パートナー センターを使用して、貴社の顧客に、独立系ソフトウェア ベンダー (ISV) によって商用マーケットプレース ([Microsoft AppSource](https://appsource.microsoft.com/) および [Azure Marketplace](https://azuremarketplace.microsoft.com/)) に発行されたサービスとしてのソフトウェア (SaaS) 製品に対するサブスクリプションを販売できます。 これは、貴社のビジネスを差別化し、特定のビジネス ニーズに対応するソフトウェア バンドルを顧客に提供するのに役立ちます。 Microsoft 製品の場合と同じように、これらのマーケットプレース SaaS 製品に対するライセンスとサブスクリプションを管理します。

商用マーケットプレースの詳細については、「[Marketplace に関する FAQ](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide)」を参照してください。

> [!IMPORTANT]
> パートナーセンターで購入できるのは、サービスとしてのソフトウェア (SaaS) の商用マーケットプレース サブスクリプションのみです。 他の商用マーケットプレース オファーの種類 (Azure アプリケーション、コンテナー、VM など) は、Azure portal を通して管理され、使用量に応じて課金されます。 Azure portal で従量課金制ソリューションを有効にするには、既存の Azure サブスクリプションが必要です。

## <a name="view-marketplace-offers-and-pricing"></a>Marketplace のオファーと価格を表示する

購入可能なすべての商用マーケットプレース オファーを表示するには、左側のナビゲーション メニューから **[Marketplace]** を選択します。 既定では、すべての種類とカテゴリの製品が表示されます。 種類やカテゴリでフィルター処理したり、検索ボックスを使って特定のキーワードを検索したりできます。 製品を選択すると、無料試用期間が提供されているかどうかなど、発行元と利用可能な SKU に関する情報が表示されます。

> [!NOTE]
> 商用マーケットプレースで購入可能な製品の一部が、ここに表示されない場合があります。 ISV は、自社製品をパートナー センターでクラウド ソリューション プロバイダー (CSP) パートナーに提供するかどうかを決定できます。 パートナーセンターを通じて顧客に提供する製品がコマーシャルマーケットプレースに表示される場合は、製品一覧から発行者の連絡先情報を検索し、関心のあるものを通知してください。

商用マーケットプレースの製品の価格は、頻繁に変わることがあります。 商用マーケットプレースのすべての製品の現在の価格情報を取得するには、 **[Marketplace]** ページの右上隅にある **[価格表のエクスポート]** を選択します。 これにより、すべての価格データが含まれるスプレッドシートが生成されます。 この価格情報は毎日更新されるため、できる限り頻繁にチェックして、最新の価格を入手してください。

> [!TIP]
> この一覧では、無料試用版がある製品については、スプレッドシートに 2 つの行が追加され、 一方の行には価格として 0 が表示されます。これは無料試用版が使用できることを示します。 もう一方の行には、試用期間の終了後に適用される価格と条件が示されます。
>
> この一覧の[従量制課金](https://docs.microsoft.com/azure/marketplace/partner-center-portal/saas-metered-billing)が使用されている製品は、条件フィールドが空白になります。

## <a name="purchase-commercial-marketplace-products-for-your-customers"></a>顧客のために商用マーケットプレースの製品を購入する

商用マーケットプレースの SaaS 製品に対するサブスクリプションの購入は、Microsoft 製品のサブスクリプションの購入と同じプロセスで行います。 サブスクリプションを購入する前に、顧客を選択するか、新しい顧客を追加する必要があります。

顧客に対するサブスクリプションを追加するときは、 **[発行元]** フィルターで **[パートナー]** を選択することにより、ISV からの Marketplace オファーだけを表示することができます。 詳しくは、「[新しいサブスクリプションの作成](create-a-new-subscription.md)」をご覧ください。

**Marketplace** のページに表示されているオファーの一部は、特定の顧客が利用できない場合があることに注意してください。 ISV が顧客の請求先の国/地域をサポートするかどうかなど、さまざまな要因によって可用性が影響を受ける可能性があります。

> [!TIP]
> [パートナー センター API](https://docs.microsoft.com/partner-center/develop/) を使って、顧客向けの商用マーケットプレース サブスクリプションを作成することもできます。 詳しくは、「[商用マーケットプレース製品のサブスクリプションを作成する](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)」をご覧ください。

商用マーケットプレース製品に対するサブスクリプションの場合、貴社は、キャンセル期間内であれば[サブスクリプションを取り消す](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription)ことができます (月単位のサブスクリプションの場合は 24 時間、年単位のサブスクリプションの場合は 14 日)。 また、貴社は、[サブスクリプションを自動的に更新するかどうかを選択する](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription)こともできます。

## <a name="license-activation-for-commercial-marketplace-products"></a>商用マーケットプレース製品のライセンス認証

プランの種類が "サービスとしてのソフトウェア (SaaS)" の場合、ライセンスの割り当てとライセンス認証は、製品を発行した独立系ソフトウェアベンダー (ISV) によって管理されます。 このプロセスを完了するには、発行元が特定の購入を特定できるようにする認証コードを使用して、発行元のサイトにアクセスする必要があります。 このリンクは、SaaS プランを購入した後に表示される確認ページと、(そのプランの行の) **[サブスクリプション]** ページにあります。 [パートナー センター API を使用して、このリンクを取得](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item)することもできます。

このリンクを使用して発行元のサイトにアクセスすると、ライセンスのプロビジョニングと割り当てを行うために必要な追加情報またはアクションが表示されます。または、セットアッププロセスを完了する必要があります。 必要な手順は、発行元とプランによって異なることがあります。 必要な情報は、ご自身の責任において送信する必要があります (または、必要な情報を直接提供できる URL を顧客に送信します)。 必要な情報が提供されると、発行元は適切なライセンスをプロビジョニングして割り当てます。 サブスクリプションの請求は、ライセンスが正常に割り当てられた後に開始されます。

## <a name="access-billing-info-for-commercial-marketplace-products"></a>商用マーケットプレース製品の課金情報にアクセスする

商用マーケットプレース製品の場合、請求期間はカレンダー月の最初の日に開始し、カレンダー月の最後の日に終了します。 請求書は、次の月の8日目に使用できるようにします。 これらの請求書には、パートナー センターまたはパートナー センター API を使用してアクセスできます。

詳しくは、「[パートナー センターでの課金の種類について](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges)」をご覧ください。

## <a name="provide-support-for-customers-using-commercial-marketplace-products"></a>商用マーケットプレース製品を使用している顧客にサポートを提供する

Microsoft 製品の場合と同じように、請求とサブスクリプションの管理に関する質問については、貴社が顧客に対する最初の窓口になる必要があります。 テクニカル サポートについては、貴社が発行元に問い合わせる必要があります。 Microsoft では、市販の marketplace 製品はサポートしていませんが、発行元のサポート連絡先情報は提供されます。

詳細については、「[商用マーケットプレース製品のサポート](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-commercial-marketplace-products)」および「[顧客へのサポートの提供](https://docs.microsoft.com/partner-center/customer-support)」をご覧ください。

## <a name="manage-subscriptions-using-partner-center-apis"></a>パートナー センター API を使用してサブスクリプションを管理する

パートナーセンター API を使用して、商用マーケットプレース製品のサブスクリプションを作成できます。 そのためには、まずマーケットプレースのオファーの一覧を取得し、次に特定の商用マーケットプレース サブスクリプションの注文を作成して送信します。 最後に、サブスクリプションのライセンス認証リンクを取得します。

パートナー センター API を使用すると、これらのサブスクリプションのライフサイクル管理を行ったり、請求書を管理したりすることもできます。

詳しくは、「[商用マーケットプレース製品のサブスクリプションを作成する](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)」をご覧ください。