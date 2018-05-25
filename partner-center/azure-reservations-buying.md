---
title: 顧客に代わって Microsoft Azure Reservations を購入する | パートナー センター
Description: Buy Azure reservations on behalf of customers in your Partner Dashboard.
author: v-petand
keywords: Azure, 予約, VM, 管理, 請求, 購入
ms.openlocfilehash: 9a937c0422f54a52b33a57086b75e02557b5ee3b
ms.sourcegitcommit: 034336ae3a697a97a62ad549b8645c836624efaa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2018
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-the-partner-dashboard"></a>パートナー ダッシュボードで顧客に代わって Microsoft Azure Reservations を購入する 

**適用対象**

-  パートナー ダッシュボード
-  Microsoft Azure portal
-  CSP のパートナー

>[!IMPORTANT]
>顧客に代わって Azure Reservations の購入を行う前に、顧客のニーズに適した仮想マシン サイズの決定方法について、必ず「[最大限の予約使用に備えた Microsoft Azure VM サイズ](azure-usage.md)」をご確認ください。 

パートナー ダッシュボードで顧客に代わって Microsoft Azure Reservations を購入するには、次の手順に従います。

Azure Reservations は Azure portal で購入することもできます。 その方法については、「[Azure Reserved VM Instances による仮想マシン料金の前払い](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)」をご覧ください。

1. [ダッシュボード] メニューで **[顧客]** を選択します。  

2. **[顧客]** ページで、Azure Reservations を購入する顧客を見つけ、下矢印を選択して顧客行を展開します。  

3. **[製品の追加]** を選択し、製品の一覧で **[Azure Reserved VM Instances]** を選択します。 

    または、顧客名を選択してアカウントの詳細ページを開き、**[Azure Reservations] > [製品の追加]** を選択します。 製品の一覧から **[Azure Reserved VM Instances]** を選択します。 

4. Azure Reservations をアクティブな Azure サブスクリプションに関連付ける必要があります。 Azure Reservations を追加する先の顧客サブスクリプションを選択します。 使用可能な Azure Reserved VM Instances の一覧が表示されます。 

    >[!IMPORTANT] 
    >顧客がまだ Azure サブスクリプションを持っていない場合は、メニューから **[サブスクリプション]** を選択して、ここで追加します。 

5. ダッシュボード ウィンドウの右側で、予約期間 (1 年間または 3 年間) を選択し、フィルターを使用して、顧客の要件を満たす予約インスタンスを検索します。  

6. 購入する予約済み VM インスタンスを見つけたら、顧客が VM で使用する予約インスタンスの数を **[数量]** に入力し、**[カートに追加]** を選択します。  

7. 必要な項目をすべて注文に追加できるまで、手順 5 と 6 を繰り返します。 **[確認]** を選択して、注文内容を確認します。  

8. **[Review your orders]** (ご注文の確認) ページで、予約インスタンスの数を確認 (必要に応じて変更) し、予約の範囲を選択します。 **[購入]** を選択して注文内容を購入します。 

    >[!NOTE]
    >予約の範囲には、1 つのサブスクリプションまたは複数のサブスクリプション (共有範囲) を指定できます。 1 つのサブスクリプションを指定した場合、予約割引は、そのサブスクリプションの VM のみに適用されます。 共有を選択した場合は、顧客の請求コンテキストに含まれるすべてのサブスクリプションで実行されている VM に予約割引が適用されます。 

9. 注文番号を含む注文の詳細は、次のページに表示されます。 **[完了]** を選択して **[注文履歴]** ページに移動します。 

>[!IMPORTANT]
>まだであれば、[顧客] ページで顧客を見つけ、下矢印を選択して顧客行を展開します。 **[Microsoft Azure の管理ポータル]** を選択すると、Azure portal に顧客レコードが表示されます。

## <a name="azure-reservations-resources"></a>Azure Reservations に関するリソース
|**情報**   |**参照先**    |
|:-----------------------------|:-----------------|
|CSP での Azure Reservations 概要  | [Microsoft Azure Reserved VM Instances の販売](azure-reservations.md) |
|Azure Reservations の請求   |[Azure Reservations の請求](azure-reservations-billing.md)   |
|パートナー ダッシュボードで Azure Reservations を管理する | [パートナー ダッシュボードで Azure Reservations を管理する](azure-reservations-manage.md)
|適切な VM サイズの判断と顧客による VM 使用状況の確認   |[最大限の Azure 予約使用に備えた VM サイズ](azure-usage.md)   |
|Azure portal で Azure Reservations を購入する | [Azure Reserved VM Instances による仮想マシン料金の前払い](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) (Azure ヘルプ) |
|Azure portal で Azure Reservations を管理する   |[予約済み VM インスタンスの管理](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) (Azure ヘルプ)  |
|パートナー センター API を使用して Azure Reservations を購入する | [Azure Reserved VM Instances の購入](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) (パートナー センター開発者向けドキュメント)

 


 
