---
title: 顧客に代わって Azure Reservations を管理する | パートナー センター
Description: Purchasing and managing Azure reservations on behalf of your customers.
author: v-petand
keywords: azure reservations を管理, 請求, 購入
ms.localizationpriority: medium
ms.openlocfilehash: 5025c32da86944f65c548a7e3ef6e61f7275522e
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/31/2018
ms.locfileid: "2877402"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>顧客に代わって Microsoft Azure Reservations を管理する

**適用対象**

-  パートナー ダッシュ ボード
-  Microsoft Azure portal
-  CSP のパートナー

顧客の Azure reservations を購入後で管理するには、顧客と予約は、パートナー ダッシュ ボードで管理するを選択し、Azure portal で予約を変更することがします。 

1. まずダッシュボード メニューから **[顧客]** を選択し、予約を管理する対象の顧客を選択します。 

2. 顧客の詳細ページ メニューで、 **Azure 予約**を選択し、[し管理する特定の予約を選択します。  

3. **[アクション]** の **[管理]** を選択し、顧客の予約レコード (Azure portal) に移動します。 予約の詳細ページで、次の手順に従ってタスクを完了します。  

| **選択するコントロール**   | **目的**    |
|:-----------------------------|:-----------------|
| **概要**   | 有効期限、範囲、使用率データなど、顧客の予約に関する詳細を表示します。 **注意:** 日割り計算の払い戻しを求めるサポート要求を作成するには、**[Refund]** (払い戻し) を選択します。 予約期間のうち未使用の部分を交換するためのサポート要求を作成するには、**[交換]** を選択します。  
| **アクセス制御 (IAM)**   | 顧客の予約情報へのアクセスを管理します。|
| **構成**   | 予約の範囲や、予約が関連付けられている Azure サブスクリプションを変更します。    |
| **プロパティ**   | 予約のプロパティを表示し、予約 ID と予約注文 ID をクリップボードにコピーします。 **注意:** 顧客に代わってサポートを要求する際には、予約 ID と予約注文 ID がサポートから求められることがあります。    |
| **新しいサポート要求**    | Microsoft サポートによるヘルプを要求します。   |
 
## <a name="cancel-or-exchange-a-reservation"></a>予約の取り消しまたは交換 
顧客のビジネス ニーズが変化すると、予約の取り消しが必要になることがあります。予約の日割り計算の払い戻し額を新しい予約の料金に充当するという交換が必要になることもあります。 

**取り消しのしくみ**

顧客は、予約をいつでも取り消すことができます (1 年に $50,000 まで)。 予約を取り消すと、Azure 予約の期間のうち、残りの月を Microsoft に返すことができます (早期解約手数料が発生します)。 顧客の元の購入に対して、日割り残高から手数料を差し引いた額が払い戻されます。 

**交換のしくみ** 

交換では、予約で残っている期間の長さに基づいて日割り計算の払い戻し額を顧客が受け取り、その金額を新しい予約に充当できます。   

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>顧客に代わって払い戻しまたは交換を申請する 

顧客に代わって払い戻しまたは交換のサポート要求を登録するには、パートナー ダッシュボードで顧客と予約を選択し、Azure portal でサポート要求を作成します。 

>[!NOTE]
>Microsoft サポート担当者から、予約 ID と予約注文 ID が求められることがあります。 この情報は、Azure portal で予約の **[プロパティ]** ページを開くと確認できます。 

1. まずダッシュボード メニューから **[顧客]** を選択し、払い戻しを受ける顧客を選択します。 

2. 顧客の詳細ページで **[Azure Reservations]** を選択し、顧客が払い戻しを受ける特定の予約を選択します。  

3. [**操作**] には、Azure portal で顧客の予約レコードに移動し、サポート要求を開始する**払い戻し**をを選択します。  

4. **[新しいサポート要求]** ページで、次の手順に従って払い戻しを申請します。 各手順の後には、**[次へ]** を選択します。 

|**手順**   |**選択内容**    |
|:-----------------------------|:-----------------|
|**1. 基本**   |問題の種類: 請求  |
|**2. 問題**   |問題の種類: 予約管理 カテゴリ: 交換と払い戻し |
|**3. 連絡先情報**   |基本設定を選択し、必要な情報を入力します。 完了したら、**[作成]** を選択します。   |

## <a name="azure-reservations-resources"></a>Azure Reservations に関するリソース
|**情報**   |**参照先**    |
|:-----------------------------|:-----------------|
|CSP での Azure Reservations 概要  | [販売 Microsoft Azure 予約インスタンス](azure-reservations.md) |
|パートナー ダッシュボードで顧客の Azure Reservations を購入する   |[Azure Reservations の購入](azure-reservations-buying.md) |
|適切な VM サイズの判断と顧客による VM 使用状況の確認   |[最大限の Azure 予約使用に備えた VM サイズ](azure-usage.md)   |
|パートナー センター API を使用して Azure Reservations を購入する | [Azure Reserved VM Instances の購入](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) (パートナー センター開発者向けドキュメント)

