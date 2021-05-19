---
title: プランの検出-コマーシャルマーケットプレース
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP パートナーがパートナーセンターを使用して、SaaS プランや独立系ソフトウェアベンダー (Isv) からの価格を表示または検索する方法について説明します。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ab30f8391df58155c8511dc628b1fefd94c8d768
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147974"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>パートナーセンターコマーシャルマーケットプレースでのプランと価格の検出

**適切なロール**: 全体管理者 |管理エージェント

独立系ソフトウェアベンダー (Isv) は、商用マーケットプレースでプランを公開することを選択した場合、そのプランを CSP プログラムで利用できるようにするかどうかを決定することもできます。 CSP プログラムを通じてプランを販売することを選択した場合、CSP パートナーはパートナーセンターの Marketplace でプランを確認する必要があります。

パートナーセンターで期待どおりに ISV プランが表示されない場合は、次の原因が考えられます。

- ISV は、CSP プログラムを通じてプランを販売しないと判断しました。 たとえば、一部の ISV 製品は、商用マーケットプレースの他の領域 ( [Microsoft AppSource](https://appsource.microsoft.com/) や [Azure marketplace](https://azuremarketplace.microsoft.com/)など) で利用できるようになっていますが、パートナーセンターマーケットプレースの CSP プログラムのパートナーには記載されていない場合があります。

- ISV は、選択された数の CSP パートナーのみにプランを限定することに決めました。 限定プランの詳細については、このヘルプトピックの「」を参照してください。

- プランの種類は、パートナーセンターまたは Azure portal (たとえば、コンテナーや一部の使用量ベースのプラン) では不可能ない可能性があります。

- この ISV プランでは、関連付けられている顧客の請求先の国がサポートされていない可能性があります。

## <a name="view-marketplace-offers-in-partner-center"></a>パートナーセンターで Marketplace のプランを表示する

CSP プログラムで利用可能な商用 marketplace プランを表示するには、次のようにします。

1. パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインし、左側のナビゲーションメニューから [ **CSP** ] を選択します。

2. [ **販売**]、[ **Marketplace**] の順に選択します。 既定では、すべての種類とカテゴリの製品が表示されます。

3. 種類またはカテゴリでフィルターを選択します。 また、 **検索** 機能を使用して、特定のキーワード、プラン名、ISV 発行元の名前を検索することもできます。

4. 一覧から特定の製品オファーを選択します。 これにより、オファーの詳細を確認できる製品の [概要] タブが表示されます。 このタブの情報には、次のものが含まれる場合があります。 

    - 製品またはオファーの説明

    - ISV パブリッシャーの詳細

    - ISV 発行元によってアップロードされたドキュメントまたはマーケティング資料へのリンク

    - カスタマー サポート、エンジニアリング、または CSP プログラムの連絡先に関して、その他の可能な ISV 連絡先

5. オファーの使用可能なプラン、SKU、または価格の詳細を表示するには、[プラン + 価格] タブ **を選択** します。このタブには次の情報が表示されます。

    - このオファーを利用できる市場

    - オファーで使用できる SKU またはプランの一覧

    - 使用可能な各 SKU またはプランの価格

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Api を使用して Marketplace オファーパートナー センター表示する

CSP プログラム パートナーは、API を使用して、対象となるオファーの一覧を返す場合にも使用できます。 対象となるオファーは、パートナーがマーケットプレース経由で販売できる SaaS ISV オファーパートナー センターされます。 API を使用してカタログ内のオファーを識別するパートナーについては、市場向けオファーの一覧を取得するためのガイダンス [を参照してください](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)。

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>最新の Marketplace オファーの価格については、以下を参照パートナー センター

オファーに関連付けられている最新の価格の詳細については、次の手順に従います。

1. ダッシュボードにパートナー センター [し、](https://partner.microsoft.com/dashboard)左側のナビゲーション **メニューから [CSP]** を選択します。

2. [販売 **] を** 選択し、続いて [価格と **プラン] を選択します**。

3. [Marketplace] セクションまで **下にスクロール** し、場所を選択して Marketplace の価格 **をダウンロードします**。 これにより、SaaS、ライセンスベースのプラン、および ISV 発行元から提供されている従量制課金プランの最新の価格データを含むスプレッドシートが生成されます。 一部の Azure アプリケーションの料金は、ここにも表示される場合があります。 この情報は毎日更新されるため、選択した頻度で現在の価格を確認することができます。

4. ISV 製品に無料試用期間が含まれている場合、スプレッドシートにその製品の2つの行が表示されます。

    - 1行目は無料試用版の価格を示しています。 つまり、無料試用期間を利用できます。

    - もう1つの行には、無料試用期間が終了した後に適用される価格と使用条件が示されています。

CSP プログラムパートナーとして、特定の商用 marketplace プランに関連する他のインセンティブの対象となる場合があります。 その他のインセンティブの詳細については、 [csp インセンティブガイド](https://aka.ms/partnerincentives) (csp ログインが必要) を参照してください。

## <a name="learn-about-marketplace-exclusive-offers"></a>Marketplace 限定プランの詳細

Isv は、CSP プログラムの特定のパートナーだけがオファーを利用できるようにするオプションを備えています。 これは、排他的なオファーとして知られています。 CSP プログラム内のすべてのパートナーは、パートナーセンターの商用 marketplace にあるすべての ISV プランを表示できます。ただし、排他とマークされているプランも含まれます。

プランが排他とマークされ **ていない** 場合は、すべてのパートナーがそのプランを購入できます (選択した顧客の請求先の国が ISV のオファーの使用可能な国に一致していることを前提とします)。

ただし、排他とマークされているプランでは、ISV によって選択されたパートナーだけがそのプランを購入できます。

> [!NOTE]
> お客様に販売するものとして提供されているプランが [排他] として表示される場合は、ISV に直接連絡して、排他プランを販売するためのアクセス許可を要求します。 排他プランの詳細を表示すると、選択できる [ **CONTACT ISV** ] リンクが表示される場合があります。

商用マーケットプレースの ISV エクスペリエンスの詳細については、 [クラウドソリューションプロバイダー](/azure/marketplace/cloud-solution-providers)に関するページを参照してください。

Marketplace での CSP エクスペリエンスの詳細については、「 [コマーシャルマーケットプレースの概要」](csp-commercial-marketplace-overview.md)を参照してください。

## <a name="next-steps"></a>次のステップ

- [商用 marketplace プランの購入](csp-commercial-marketplace-purchase.md)