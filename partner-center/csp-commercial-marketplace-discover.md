---
title: プランの検出-コマーシャルマーケットプレース
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP パートナーがパートナーセンターを使用して、SaaS プランや独立系ソフトウェアベンダー (Isv) からの価格を表示または検索する方法について説明します。
author: LauraBrenner
ms.author: labrenne
keywords: サブスクリプション、marketplace、商業市場、サードパーティ、ISV、SaaS プラン、クラウドソリューションプロバイダープログラム、CSP プログラム、CSP パートナー
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 10653e41adee052b43ed092f4fd9bb48b79a1355
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908115"
---
# <a name="discover-offers-and-pricing-in-the-partner-center-commercial-marketplace"></a>パートナーセンターコマーシャルマーケットプレースでのプランと価格の検出

**適用対象**

- パートナー センター
- CSP プログラムのパートナー

**適切なロール**

- グローバル管理者
- 管理エージェント

独立系ソフトウェアベンダー (Isv) は、商用マーケットプレースでプランを公開することを選択した場合、そのプランを CSP プログラムで利用できるようにするかどうかを決定することもできます。 CSP プログラムを通じてプランを販売することを選択した場合、CSP パートナーは、パートナーセンターの Marketplace 領域にプランを表示する必要があります。

パートナーセンターで ISV プランが期待どおりに表示されない場合は、次の原因が考えられます。

- ISV は、CSP プログラムを通じてプランを販売しないと判断しました。 たとえば、一部の ISV 製品は、商用マーケットプレースの他の領域 ( [Microsoft AppSource](https://appsource.microsoft.com/)や[Azure marketplace](https://azuremarketplace.microsoft.com/)など) で利用できるようになっていますが、パートナーセンターマーケットプレースの csp には記載されていない場合があります。

- ISV は、選択された数の CSP パートナーのみにプランを限定することに決めました。 限定プランの詳細については、このヘルプトピックの「」を参照してください。

- プランの種類は、パートナーセンターまたは Azure portal (たとえば、コンテナーや一部の使用量ベースのプラン) では不可能ない可能性があります。

- この ISV プランでは、関連付けられている顧客の請求先の国がサポートされていない可能性があります。

## <a name="view-marketplace-offers-in-partner-center"></a>パートナーセンターで Marketplace のプランを表示する

CSP プログラムで利用可能な商用 marketplace プランを表示するには、次のようにします。 

1. パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard)にサインインし、左側のナビゲーションメニューから [ **CSP** ] を選択します。

2. [**販売**]、[ **Marketplace**] の順に選択します。 既定では、すべての種類とカテゴリの製品が表示されます。

3. 種類またはカテゴリでフィルターを選択します。 また、**検索**機能を使用して、特定のキーワード、プラン名、ISV 発行元の名前を検索することもできます。

4. 一覧から特定の製品プランを選択します。 [製品の概要] タブが表示され、プランの詳細を確認できます。 このタブには次の情報が含まれます。 

    - 製品またはプランの説明

    - ISV 発行者に関する詳細情報

    - ISV 発行元によってアップロードされたドキュメントまたはマーケティング資料へのリンク

    - CSP プログラムのカスタマーサポート、エンジニアリング、または連絡先に関する他の ISV 連絡先

5. プランの利用可能なプラン、Sku、または価格に関する詳細情報を表示するには、[**プランと価格設定**] タブを選択します。このタブには、次の項目が表示されます。

    - このプランが利用可能な市場

    - プランで利用可能な Sku またはプランの一覧

    - 各 SKU または使用可能なプランの価格

## <a name="view-marketplace-offers-via-partner-center-apis"></a>パートナーセンター Api を使用して Marketplace のプランを表示する

CSP プログラムパートナーは Api を使用して、対象となるプランの一覧を返すこともできます。 パートナーがパートナーセンター marketplace を通じて販売することができるのは、資格のあるオファーのみです。 Api を使用してカタログ内のプランを特定するパートナー向けに、[市場向けのプランの一覧を取得](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)するためのガイダンスを参照してください。

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>パートナーセンターで最新の Marketplace プランの価格を確認する

プランに関連付けられている最新の価格の詳細については、次の手順に従ってください。

1. パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard)にサインインし、左側のナビゲーションメニューから [ **CSP** ] を選択します。

2. [**販売**] を選択し、その後に [**料金とプラン**] を選択します。

3. [ **Marketplace** ] セクションまで下にスクロールし、場所を選択して**marketplace の価格**をダウンロードします。 これにより、SaaS の最新の価格データを含むスプレッドシートが生成され、ISV 発行元から提供されるライセンスベースのプランが生成されます。 一部の Azure アプリケーションの料金は、ここにも表示される場合があります。 この情報は毎日更新されるため、選択した頻度で現在の価格を確認することができます。

4. ISV 製品に無料試用期間が含まれている場合、スプレッドシートにその製品の2つの行が表示されます。

    - 1行目は無料試用版の価格を示しています。 つまり、無料試用期間を利用できます。

    - もう1つの行には、無料試用期間が終了した後に適用される価格と使用条件が示されています。

CSP プログラムパートナーとして、特定の商用 marketplace プランに関連する他のインセンティブの対象となる場合があります。 その他のインセンティブの詳細については、 [csp インセンティブガイド](https://aka.ms/partnerincentives)(csp ログインが必要) を参照してください。

## <a name="learn-about-marketplace-exclusive-offers"></a>Marketplace 限定プランの詳細

Isv は、CSP プログラムの特定のパートナーだけがオファーを利用できるようにするオプションを備えています。 これは、排他的なオファーとして知られています。 CSP プログラム内のすべてのパートナーは、パートナーセンターの商用マーケットプレースにあるすべての ISV プランを表示できます (ただし、排他とマークされているプランを含む)。

プランが排他とマークされ**ていない**場合は、すべてのパートナーがそのプランを購入できます (選択した顧客の請求先の国が ISV のオファーの使用可能な国に一致していることを前提とします)。

ただし、排他とマークされているプランでは、ISV によって選択されたパートナーだけがそのプランを購入できます。

> [!NOTE]
> お客様に販売するものとして提供されているプランが [排他] として表示される場合は、ISV に直接連絡して、排他プランを販売するためのアクセス許可を要求します。 排他プランの詳細を表示すると、選択できる [ **CONTACT ISV** ] リンクが表示される場合があります。

商用マーケットプレースの ISV エクスペリエンスの詳細については、[クラウドソリューションプロバイダー](https://docs.microsoft.com/azure/marketplace/cloud-solution-providers)に関するページを参照してください。

Marketplace での CSP エクスペリエンスの詳細については、「[コマーシャルマーケットプレースの概要」](csp-commercial-marketplace-overview.md)を参照してください。

## <a name="next-steps"></a>次のステップ

- [商用 marketplace プランの購入](csp-commercial-marketplace-purchase.md)
