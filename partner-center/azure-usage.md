---
title: 最大予約の使用状況の Microsoft Azure VM のサイズ |パートナー センター
ms.topic: article
ms.date: 03/15/2019
Description: 顧客に代わって Microsoft Azure Reservations を購入するときは、顧客のコンピューティング ニーズに合わせて仮想マシン (VM) のサイズを選択する必要があります。
author: LauraBrenner
ms.author: v-petand
keywords: Azure, 予約, VM, 管理, 請求, 使用, サイズ
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 9a398b73cf00bd71130d25f0ec94a33b457e216b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135544"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>最大限の予約使用に備えた Microsoft Azure VM サイズ 

**適用対象**

-  パートナー センター
-  Azure portal
-  CSP のパートナー

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>顧客の Azure 予約の VM サイズを決定する 

顧客に代わって Microsoft Azure Reservations を購入するときは、顧客のコンピューティング ニーズに合わせて仮想マシン (VM) のサイズを選択する必要があります。 この情報は、次のいずれかの方法を使用して確認できます。

-   Azure Utilization API
-   Azure portal
-   Azure PowerShell
-   Azure Resource Manager (ARM) API

これらの方法を使用するための手順をそれぞれ以下に示します。 予約を購入した後、予約の属性および数量に一致する仮想マシンに予約割引が自動的に適用されます。 予約を VM に割り当てる必要はありません。

>[!NOTE]
>予約割引は、従来型またはプロモーション用の VM には適用されません。

>[!IMPORTANT]
>顧客に代わって購入する VM の種類とサイズを正しく特定するには、以下で説明するいずれかの方法を使用する必要があります。パートナー センターの調整ファイルには、VM 系列の種類が正しく表示されません。


**VM の Azure 使用率の API を使用して情報をサイズ変更の取得します。**

1.  API の応答に含まれる additionalInfo の ServiceType 属性の値を使用して、購入する VM サイズ を特定します。 

2.  詳しくは、[パートナー センター API](https://docs.microsoft.com/partner-center/develop/) の「[Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)」 (顧客の Azure 使用率レコードを取得する) をご覧ください。 

**VM サイズ、Microsoft Azure ポータルを使用して情報の取得します。**

1.  パートナー センターに移動、**顧客**ページ。

2.  Azure VM 予約を購入する顧客を見つけ、下矢印を選択して顧客情報を展開します。 **[Microsoft Azure の管理ポータル]** を選択すると、Azure portal に顧客レコードが表示されます。 

3.  ポータルのメニューから **[仮想マシン]** を選択し、予約を購入する対象の VM を選択します。 

4.  VM の詳細ページで、サイズと地域の情報を見つけます (下図参照)。パートナー センターで予約を購入する際には、この情報を使用します。  

    ![[詳細] ページのサイズとリージョンの情報](images/usage1.png)

**サイズ情報を Microsoft Azure PowerShell を使用して VM を取得します。**

下の画像の情報を使用して、予約を購入する対象の VM の場所とサイズを取得します。 

![VM の場所とサイズ](images/usage2.png)

**VM の Azure リソース マネージャー (ARM) API を使用して情報をサイズ変更の取得します。**

1.  ARMClient または ARM API を使用し、予約を購入する対象の VM に対して ARM クライアントを呼び出します。

2.  /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3.  この呼び出しでは、**vmSize** と **location** の値が返されます (下図参照)。

    ![vmSize 値](images/usage3.png)
    ![場所の値](images/usage4.png)
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Azure VM の使用状況と予約割引を確認する

顧客の代わりに Azure Reserved VM Instances を購入した場合は、VM 領域の前払いに対する割引が、顧客の予約の属性および数量に一致する仮想マシンに自動的に適用されます。 

次のいずれかの方法を使用し、顧客の予約の使用状況を調べて、どの仮想マシンに予約割引が適用されるかを確認します。   

-   Azure portal
-   Azure Utilization API

これらの方法を使用するための手順をそれぞれ以下に示します。

>[!NOTE]
>どの仮想マシンに割引が適用されるかを確認できるのは Azure Utilization API のみです。  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Microsoft Azure portal で顧客の予約の使用状況を確認する

1.  パートナー センターに移動、**顧客**ページ。

2.  予約割引と使用状況を確認する対象の顧客を見つけ、下矢印を選択して顧客情報を展開します。 **[Microsoft Azure の管理ポータル]** を選択すると、Azure portal に顧客レコードが表示されます。 

3.  ポータルのメニューから **[予約]** を選択し、使用状況を確認する対象の予約を選択します。 

4.  **[概要]** ページで、予約の使用率グラフを確認します。このグラフには、仮想マシンに適用されている予約の割合が示されています。 

    >[!NOTE]
    >使用率データには、最大で 8 時間の遅延が発生することがあります。
    
    a.   予約の使用率が 100% の場合は、顧客は予約購入によって可能な節約をすべて適用できます。 
    
    b.   予約の使用率が 0% の場合は、どの仮想マシンにも割引が適用されません。 
    
    c.  予約の使用率が 1% ～ 99% の場合は、特典が一部使用されません。 

5.  このような状況を避けるには、購入を行う前に、顧客のコンピューティング ニーズをサポートするために適した VM のサイズを決定します。

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Azure Utilization API で顧客の予約の使用状況を確認する

>[!NOTE]
>どの仮想マシンに割引が適用されるかを確認できるのは Azure Utilization API のみです。  

Azure Utilization API を使用すると、予約の使用状況データを取得できます。これにより、顧客が予約割引を獲得できるかどうかと、どの VM (仮想マシン) に割引が適用されるかを確認できます。 顧客の予約の使用状況を確認する方法については、下の Example A と Example B を比較してください。 

![予約の使用例](images/usage5.png)

-   reservationId は、VM に割引を適用するために使用された Azure 予約を識別します。
-   consumptionMeter は、予約割引が適用されている VM の MeterId です。
-   予約割引が適用されるため、ReservationMeter には料金として $0 が示されます。 

詳しくは、[パートナー センター API](https://docs.microsoft.com/partner-center/develop/) の「[Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)」 (顧客の Azure 使用率レコードを取得する) をご覧ください。

>[!IMPORTANT]
>現時点では、Microsoft Windows Server などのソフトウェアの料金は VM 予約の価格に含まれず、注文レコードと請求書に個別の明細項目として表示されます。 ただし、顧客が Azure ハイブリッド特典を利用できる場合、ソフトウェア料金は適用されません。 詳しくは、「[Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)」 (予約インスタンスに含まれない Windows ソフトウェアの料金) をご覧ください。  

## <a name="azure-reservations-resources"></a>Azure Reservations に関するリソース
|**について**   |**この記事を読む**    |
|:-----------------------------|:-----------------|
|CSP での Azure Reservations 概要  | [Microsoft Azure 予約 VM インスタンスを販売します。](azure-reservations.md)
|パートナー センターで顧客向けの Azure 予約を購入   |[Azure 予約を購入します。](azure-reservations-buying.md)
|パートナー センターでの Azure 予約を管理します。 | [パートナー センターでの Azure 予約を管理します。](azure-reservations-manage.md)
|Azure portal で Azure Reservations を購入する | [Azure Reserved VM Instances による仮想マシン料金の前払い](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) (Azure ヘルプ) |
|Azure portal で Azure Reservations を管理する   |[予約済み VM インスタンスの管理](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) (Azure ヘルプ)  |
|パートナー センター API を使用して Azure Reservations を購入する | [Azure Reserved VM Instances の購入](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) (パートナー センター開発者向けドキュメント)



