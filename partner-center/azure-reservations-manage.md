---
title: 顧客に代わって Azure Reservations を管理する | パートナー センター
Description: Purchasing and managing Azure reservations on behalf of your customers.
author: v-petand
keywords: Azure, 予約, VM, 管理, 請求, 購入
ms.openlocfilehash: ae27024ba10184b6f704f5ceef9d90af61186321
ms.sourcegitcommit: 034336ae3a697a97a62ad549b8645c836624efaa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2018
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>顧客に代わって Microsoft Azure Reservations を管理する

**適用対象**

-  パートナー ダッシュボード
-  Microsoft Azure portal
-  CSP のパートナー

顧客の Azure Reservations を購入後に管理するには、パートナー ダッシュボードで管理対象の顧客と予約を選択し、Azure portal で予約の変更を行います。 

1. まずダッシュボード メニューから **[顧客]** を選択し、予約を管理する対象の顧客を選択します。 

2. 顧客の詳細ページで **[Azure Reservations]** を選択し、管理する特定の予約を選択します。  

3. **[アクション]** の **[管理]** を選択し、顧客の予約レコード (Azure portal) に移動します。 予約の詳細ページで、次の手順に従ってタスクを完了します。  

|**選択するコントロール**   |**目的**    |
|:-----------------------------|:-----------------|
|**概要**   |有効期限、範囲、使用率データなど、顧客の予約に関する詳細を表示します。 **注意:** 日割り計算の払い戻しを求めるサポート要求を作成するには、**[Refund]** (払い戻し) を選択します。 予約期間のうち未使用の部分を交換するためのサポート要求を作成するには、**[交換]** を選択します。  
|**アクセス制御 (IAM)**   |顧客の予約情報へのアクセスを管理します。|
|**構成**   |予約の範囲や、予約が関連付けられている Azure サブスクリプションを変更します。    |
|**プロパティ**   |予約のプロパティを表示し、予約 ID と予約注文 ID をクリップボードにコピーします。 **注意:** 顧客に代わってサポートを要求する際には、予約 ID と予約注文 ID がサポートから求められることがあります。    |
|**新しいサポート要求**    |Microsoft サポートによるヘルプを要求します。   |
 
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

3. **[アクション]** で **[Refund]** (払い戻し) を選択します。Azure portal で顧客の予約レコードが開き、サポート要求が自動的に開始されます。  

4. **[新しいサポート要求]** ページで、次の手順に従って払い戻しを申請します。 各手順の後には、**[次へ]** を選択します。 

|**手順**   |**選択内容**    |
|:-----------------------------|:-----------------|
|**1. 基本**   |問題の種類: 請求  |
|**2. 問題**   |問題の種類: 予約管理 カテゴリ: 交換と払い戻し |
|**3. 連絡先情報**   |基本設定を選択し、必要な情報を入力します。 完了したら、**[作成]** を選択します。   |

## <a name="azure-reservations-resources"></a>Azure Reservations に関するリソース
|**情報**   |**参照先**    |
|:-----------------------------|:-----------------|
|CSP での Azure Reservations 概要  | [Microsoft Azure Reserved VM Instances の販売](azure-reservations.md) |
|パートナー ダッシュボードで顧客の Azure Reservations を購入する   |[Azure Reservations の購入](azure-reservations-buying.md) |
|Azure Reservations の請求   |[Azure Reservations の請求](azure-reservations-billing.md)   |
|適切な VM サイズの判断と顧客による VM 使用状況の確認   |[最大限の Azure 予約使用に備えた VM サイズ](azure-usage.md)   |
|Azure portal で Azure Reservations を購入する | [Azure Reserved VM Instances による仮想マシン料金の前払い](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) (Azure ヘルプ) |
|Azure portal で Azure Reservations を管理する   |[予約済み VM インスタンスの管理](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) (Azure ヘルプ)  |
|パートナー センター API を使用して Azure Reservations を購入する | [Azure Reserved VM Instances の購入](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) (パートナー センター開発者向けドキュメント)

