---
title: Azure プランの価格表 | パートナー センター
ms.topic: article
ms.date: 10/15/2019
description: Azure プランのサブスクリプションに対する価格表を確認する方法
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: 64f7b6930f31afc63397ae3ed0e0dba2357b0f1e
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171283"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Azure 向けの CSP の新しいコマース エクスペリエンスの価格表 

CSP の新しい Azure コマース エクスペリエンスの価格表は、パートナー センターに掲載されます。 価格表は、動的に配信されるリアルタイムの正確なファイルであり、価格は米国ドルでのみ表示されます。 ただし、請求については、顧客の所在地の通貨に適用される、サポートされている通貨で行われます。 顧客の所在地での通貨による請求の詳細については、「[Azure プラン - 請求](azure-plan-billing.md)」を参照してください。

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Azure プランのサブスクリプションに対する価格を確認する

1. 左側のパートナー センターのメニューから、 **[販売]** を選択し、 **[マーケットプレース]** を選択します。

2. **[エクスポートの種類]** で、 **[Azure プランの従量課金価格]** を選択します。

3. **[日付での価格]** で、目的の日付を選択します (例: **[現在]** )。 注: **[外国為替レート]** を選択して、現在の外国為替レートをエクスポートすることもできます。

![Azure の価格 2](images/azure/pricelist2.jpg)

4. **[マーケットプレース]** で、製品の **[種類]** と **[カテゴリ]** を選択するか、製品を検索します。 検索条件に基づいて利用可能な製品が表示されます。

![pricing](images/azure/Azurepricelist1.jpg)

5. 次に、 **[Azure プランの価格表のエクスポート]**  を選択して、選択した製品用の Azure プランの価格をダウンロードします。


![価格表のエクスポート](images/azure/pricelist1.png)



## <a name="azure-price-list-specifics"></a>Azure 価格表の詳細

- Azure プランの価格は、パートナー センターで、 **[販売]** の下の [マーケットプレース] ページで入手できます。

- Azure プランの従量課金サービス、Azure Reservations、および外国為替レートに対してエクスポートを利用できます。

- エクスポートのオプションには、以下が含まれています。

    - **本日の価格**:これには、当月の 1 日から現在の日付までのすべてのメーターと価格が含まれています。 これには、新しい価格、変更された価格、または削除された価格が含まれます。 すべての価格には、新規であるか削除されたかどうかを説明する有効な開始日と終了日があります。

    - **前月の価格**:各種類のリソースのダウンロードは月単位で行われます。 価格ファイルの場合は、その月に利用可能であったすべてのメーターが含まれます。 月の途中で新しいメーターが出現した場合は、その利用可能性を反映する有効日付きのメーターとして表示されます。 継続されていない価格についても同様であり、利用可能でなくなった日付を示す最後の有効日付きで表示されます。

    - **外国為替レート**:当月 1 日の前日の午後 6 時 (太平洋標準時) に外国為替レートをダウンロードできるようになります。 たとえば、11 月のレートが必要な場合は、10 月 31 日にレートをダウンロードします。 前月の外国為替レートも入手できます。

    - **対象となるサービス**:パートナー獲得クレジットは、パートナーが Azure プランの価格ページからエクスポートできる **[Azure プランの従量課金価格]** に記載されているサービスに適用されます。 サードパーティ サービスやAzure Reservations など (これらに限定はされません)、例外があることに注意してください。

- 価格表の価格は、直販価格です。 一部のパートナーは、パートナー獲得クレジットの対象になることがあります。 パートナー獲得クレジットの計算方法の詳細については、「[パートナー獲得クレジットの計算方法と支払い方法](partner-earned-credit-explanation.md)」を参照してください。


## <a name="price-list-data"></a>価格表のデータ

|**フィールド**   |**説明**   |
|--------------------------|:---------------------------|
|ProductTitle  |製品のタイトルまたは名前|
|ProductID   |製品の ID|
|SKuId|SKU の ID|
|SkuTitle|SKU のタイトルまたは名前|
|発行元|ファーストパーティは常に Microsoft になります|
|SkuDescription|SKU の説明|
|UnitOfMeasure|課金または請求される単位|
|TermDuration|期間ベースの製品の場合は、予約に適用される期間の長さ|
|市場|市場価格|
|通貨|価格の通貨|
|UnitPrice|ユニットごとの価格|
|PricingTierRangeMin|階層料金では、最低料金が適用されます|
|PricingTierRangeMax|階層料金では、最高料金が適用されます|
|EffectiveStartDate|価格の開始日|
|EffectiveEndDate|価格の終了日|
|MeterIds|製品 SKU のメーター ID|
|MeterType|メーターの種類|
|タグ|項目のプロパティ。Azure プランの価格では、Azure または Azure と Reservations (特に予約用) になります|

詳細な[価格表の情報](https://partner.microsoft.com/commerce/sales?type=Any&category=Any)  
