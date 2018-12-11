---
title: 顧客に代わって Azure Reservations を管理する | パートナー センター
ms.topic: article
ms.date: 10/29/2018
Description: To manage your customers’ Azure reservations post-purchase, you’ll select the customer and reservation you want to manage in Partner Center, and then make changes to the reservation in the Azure portal.
author: v-petand
ms.author: v-petand
keywords: azure reservations を管理, 請求, 購入、キャンセル、exchange, 早期解約手数料が発生
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 7096efb34f8c72d3c8dc724332dd031a180d0636
ms.sourcegitcommit: 777225c8bf16e4a8811a9d88aceb45fcba1cd959
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/11/2018
ms.locfileid: "8917714"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>顧客に代わって Microsoft Azure Reservations を管理する

**適用対象**

-  パートナー センター
-  Microsoft Azure portal
-  CSP のパートナー

顧客の Azure reservations を購入後、管理をするには、顧客とパートナー センターで、管理する対象の予約を選択し、Azure portal で予約を変更します。 

1. 作業の開始、パートナー センター メニューから**顧客**を選択し、予約を管理する対象の顧客を選択します。 

2. 顧客の詳細ページ] メニューのでは、 **Azure reservations**を選択し、管理する特定の予約を選択します。  

3. **[アクション]** の **[管理]** を選択し、顧客の予約レコード (Azure portal) に移動します。 予約の詳細ページで、次の手順に従ってタスクを完了します。  

    | **選択するコントロール**   | **目的**    |
    |:-----------------------------|:-----------------|
    | **概要**   | 有効期限、範囲、使用率データなど、顧客の予約に関する詳細を表示します。 **注意:** 日割り計算の払い戻しを求めるサポート要求を作成するには、**[Refund]** (払い戻し) を選択します。 予約期間のうち未使用の部分を交換するためのサポート要求を作成するには、**[交換]** を選択します。  
    | **アクセス制御 (IAM)**   | 顧客の予約情報へのアクセスを管理します。|
    | **構成**   | 予約の範囲や、予約が関連付けられている Azure サブスクリプションを変更します。    |
    | **プロパティ**   | 予約のプロパティを表示し、予約 ID と予約注文 ID をクリップボードにコピーします。 **注意:** 顧客に代わってサポートを要求する際には、予約 ID と予約注文 ID がサポートから求められることがあります。    |
    | **新しいサポート要求**    | Microsoft サポートによるヘルプを要求します。   |
 
## <a name="cancel-or-exchange-a-reservation"></a>予約の取り消しまたは交換 

任意の時点で、お客様のビジネス ニーズが変化する場合は、予約を取り消すと、払い戻しを取得またはに新しい予約の料金に充当する予約の日割り計算の払い戻し額を交換します。

これらのシナリオの両方で Microsoft は、お客様とし、結果として得られる財務トランザクションを管理できるようにする量を払い戻しします。 Microsoft には、請求、取り消し、払い戻し金額の直接アクセスできません。   
 

**取り消しのしくみ**

お客様は、(1 年に $50,000 に上限の払い戻し額)、いつでも、予約の取り消しを要求できます。 予約をキャンセルするにより、お客様は、Azure 予約の早期解約手数料が発生の残りの月の量を返すです。 顧客のアカウントを払い戻すことができるようにアカウントに、日割り残高から早期の終了手数料を引いたが返金されます。 

取り消しの詳細と料金以下をご覧ください。


|**取り消し日**<br> (日)   |**使用方法**    |**クレジット**  |**早期終了**<br> 料金    |**上限を払い戻し** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 個以下                         | いいえ          | 100%       | いいえ                              | 50,000 米ドル   |
|5 個以下                         | はい         | 日割り  | いいえ                              | 50,000 米ドル   |
|複数の 5                        | いいえ          | 日割り  | 12%                             | 50,000 米ドル   |
|複数の 5                        | はい         | 日割り  | 12%                             | 50,000 米ドル   |


**交換のしくみ** 

顧客を最初に購入したものよりもさまざまな予約を購入する場合は、交換を要求することができます。 予約を交換することにより、お客様は新しい予約の価格に向けた日割り計算の払い戻し額を使用するために、予約をキャンセルする代わりに魅力的なものができます。 

日割り計算の払い戻し額が、アカウントでにかけて、exchange、顧客に提供できるようにします。


## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>顧客に代わって払い戻しまたは交換を申請する 

顧客に代わって払い戻しまたは交換のサポート要求をファイルにをパートナー センターで、顧客と予約を選択し、Azure portal でサポート要求を作成します。 

>[!NOTE]
>Microsoft サポート担当者から、予約 ID と予約注文 ID が求められることがあります。 この情報は、Azure portal で予約の **[プロパティ]** ページを開くと確認できます。 

1. 開始するのには、パートナー センター メニューから**顧客**を選択し、[払い戻し顧客します。 

2. 顧客の詳細ページで **[Azure Reservations]** を選択し、顧客が払い戻しを受ける特定の予約を選択します。  

3. [**操作****払い戻し**の Azure portal で顧客の予約レコードに移動し、サポート要求を開始を選択します。  

4. **[新しいサポート要求]** ページで、次の手順に従って払い戻しを申請します。 各手順の後には、**[次へ]** を選択します。 

    |**手順**                    |**選択内容**    |
    |:---------------------------|:-----------------|
    |**1. 基本**                |問題の種類: 請求  |
    |**2. 問題**               |問題の種類: 予約管理 カテゴリ: 交換と払い戻し |
    |**3. 連絡先情報**   |基本設定を選択し、必要な情報を入力します。 

5.  完了したら、**[作成]** を選択します。

## <a name="azure-reservations-resources"></a>Azure Reservations に関するリソース
|**情報**   |**参照先**    |
|:-----------------------------|:-----------------|
|CSP での Azure Reservations 概要  | [販売 Microsoft Azure 予約インスタンス](azure-reservations.md) |
|パートナー センターで顧客の Azure reservations を購入します。   |[Azure Reservations の購入](azure-reservations-buying.md) |
|適切な VM サイズの判断と顧客による VM 使用状況の確認   |[最大限の Azure 予約使用に備えた VM サイズ](azure-usage.md)   |
|パートナー センター API を使用して Azure Reservations を購入する | [Azure Reserved VM Instances の購入](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) (パートナー センター開発者向けドキュメント)

