---
title: CSP パートナー向け Azure プランの価格表
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP プログラム パートナーが、パートナー センターで Azure プランのサブスクリプションの価格表を確認する方法を説明します。
author: brentserbus
ms.author: brserbus
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9c9c19d9df9238e1a53d5196312d7d10515b121f
ms.sourcegitcommit: 6d45415908711cd0e28aeb19756b036274dcd326
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/15/2020
ms.locfileid: "86390339"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Azure 向けの CSP の新しいコマース エクスペリエンスの価格表

**適切なロール**

- 管理エージェント
- 課金管理者
- グローバル管理者
- ヘルプデスク エージェント
- 販売代理店
- ユーザー管理の管理者

CSP の新しい Azure コマース エクスペリエンスの価格表は、パートナー センターに掲載されます。 価格表は、動的に配信されるリアルタイムの正確なファイルであり、価格は米国ドルでのみ表示されます。 ただし、請求については、顧客の所在地の通貨に適用される、サポートされている通貨で行われます。 顧客の所在地での通貨による請求の詳細については、「[Azure プラン - 請求](azure-plan-billing.md)」を参照してください。

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Azure プランのサブスクリプションに対する価格を確認する

1. 左側のパートナー センターのメニューから、 **[販売]** を選択し、 **[マーケットプレース]** を選択します。

2. [Azure プランの価格] で、価格を設定する国を選択します。

3. **[エクスポートの種類]** で、 **[Azure プランの従量課金価格]** 、 **[Azure プランの予約価格]** 、または **[外国為替レート]** を選択します。 

>[!NOTE] 
>**[外国為替レート]** は国に固有ではありません。

4. **[日付での価格]** で、目的の日付を選択します (例: **[現在]** )。

   :::image type="content" source="images/azure/pricingnew.png" alt-text="国固有":::

>[!NOTE] 
>Azure プランの価格と Marketplace のサードパーティ価格の 2 種類の価格表をエクスポートできます。

## <a name="azure-price-list-specifics"></a>Azure 価格表の詳細

- Azure プランの価格は、パートナー センターで、 **[販売]** の下の [マーケットプレース] ページで入手できます。

- Azure プランの従量課金サービス、Azure Reservations、および外国為替レートに対してエクスポートを利用できます。

- エクスポートのオプションには、以下が含まれています。

  - **本日の価格**: これには、当月の 1 日から現在の日付までのすべてのメーターと価格が含まれています。 これには、新しい価格、変更された価格、または削除された価格が含まれます。 すべての価格には、新規であるか削除されたかどうかを説明する有効な開始日と終了日があります。

  - **前月の価格**:各種類のリソースのダウンロードは月単位で行われます。 価格ファイルの場合は、その月に利用可能であったすべてのメーターが含まれます。 月の途中で新しいメーターが出現した場合は、その利用可能性を反映する有効日付きのメーターとして表示されます。 継続されていない価格についても同様であり、利用可能でなくなった日付を示す最後の有効日付きで表示されます。

  - **外国為替レート**:当月 1 日の前日の午後 6 時 (太平洋標準時) に外国為替レートをダウンロードできるようになります。 たとえば、11 月のレートが必要な場合は、10 月 31 日にレートをダウンロードします。 前月の外国為替レートも入手できます。

- 価格表の価格は、直販価格です。 一部のパートナーは、パートナー獲得クレジットの対象になることがあります。 パートナー獲得クレジットの計算方法の詳細については、「[パートナー獲得クレジットの計算方法と支払い方法](partner-earned-credit-explanation.md)」を参照してください。

- **対象となるサービス**:パートナー獲得クレジットは、パートナーが [Azure プランの価格](https://partner.microsoft.com/commerce/sales)ページからエクスポートできる **Azure プランの従量課金価格**に記載されているサービスに適用されます。 ただし、Azure プランの従量課金価格および Azure プランの予約の [Tags]\(タグ\) 列で [Third Party]\(サードパーティ\) として示されているサードパーティ製品には (それ以外についても)、例外があります。

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
|Market|市場価格|
|通貨|価格の通貨|
|UnitPrice|ユニットごとの価格|
|PricingTierRangeMin|階層料金では、最低料金が適用されます|
|PricingTierRangeMax|階層料金では、最高料金が適用されます|
|EffectiveStartDate|価格の開始日|
|EffectiveEndDate|価格の終了日|
|MeterIds|製品 SKU のメーター ID|
|MeterType|メーターの種類|
|タグ|項目のプロパティ。Azure プランの価格では、Azure または Azure と Reservations (特に予約用) になります|

Azure プランの価格表は、[[Azure プランの価格と Marketplace] ページ](https://partner.microsoft.com/commerce/sales?type=Any&category=Any)からエクスポートできます

## <a name="pricing-api-for-azure-plan"></a>Azure プランの価格 API

[価格 API](https://docs.microsoft.com/partner/develop/pricing) を使用して、プログラムにより従量課金と予約に関する Azure プランの価格を取得できます。 また、外国為替レートを取得することもできます。

価格 API は、他のパートナー センター API とは別のエンドポイントにあります。 価格情報には、Azure プランのリソースのメーター価格 (米国ドル) と、Azure プランのサブスクリプションに適用される予約価格が含まれます。

また、Azure プランの価格は米国ドルのみであるため、この API により、パートナーは月ごとの為替レートを取得できます。 API を使用して、当月または以前の月の価格と外国為替レートの両方を取得できます。

>[!NOTE]
> 価格 API は、Azure プランの価格に固有のものです。 Azure 以外のプランのサブスクリプションに採用された Azure リソースまたは予約については、既存の RateCard API とパートナー センターの「料金とプラン」ページに掲載されている価格表を引き続き使用する必要があります。 Azure プランの価格 API では、Microsoft 365 や Dynamics 365 などのソフトウェア、マーケットプレース、シートベースの価格はサポートされません。

Azure プランの価格と外国為替レートの各 API の詳細については、完全な[価格 API のドキュメント](https://docs.microsoft.com/partner/develop/pricing)を参照してください。
