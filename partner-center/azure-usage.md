---
title: 最大限の予約使用に備えた Microsoft Azure VM サイズ | パートナー センター
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Microsoft Azure の予約を購入した場合に、お客様のコンピューティングニーズに合わせて仮想マシン (VM) のサイズを変更する方法について説明します。
author: LauraBrenner
ms.author: labrenne
keywords: Azure, 予約, VM, 管理, 請求, 使用, サイズ
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 2b8148d66be8a439056efa41eccb60cbc3e4274b
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253246"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>最大限の予約使用に備えた Microsoft Azure VM サイズ

**適用対象**

- パートナー センター
- Azure portal
- CSP のパートナー

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>顧客の Azure 予約の VM サイズを決定する 

お客様の代わりに Microsoft Azure 予約を購入する場合は、お客様のコンピューティングニーズに合わせて仮想マシン (VM) のサイズを選択する必要があります。 この情報は、次のいずれかの方法を使用して確認できます。

- Azure Utilization API
- Azure portal
- Azure PowerShell
- Azure Resource Manager (ARM) API

これらの方法を使用するための手順をそれぞれ以下に示します。 予約を購入した後、予約の属性および数量に一致する仮想マシンに予約割引が自動的に適用されます。 VM に予約を割り当てる必要はありません。

>[!NOTE]
>予約割引は、クラシックまたはプロモーションの Vm には適用されません。

>[!IMPORTANT]
>顧客に代わって購入する VM の種類とサイズを正しく特定するには、以下で説明するいずれかの方法を使用する必要があります。パートナー センターの調整ファイルには、VM 系列の種類が正しく表示されません。

**Azure Utilization API を使用して VM サイズ情報を取得する**

1. API の応答に含まれる additionalInfo の ServiceType 属性の値を使用して、購入する VM サイズ を特定します。
2. 詳細については、[パートナーセンター API](https://docs.microsoft.com/partner-center/develop/)の「 [Azure の顧客の使用状況レコードを取得する](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)」を参照してください。

**Microsoft Azure portal を使用して VM サイズ情報を取得する**

1. パートナー センターで **[顧客]** ページに移動します。
2. Azure VM の予約を購入したい顧客を見つけて、下矢印を選択して顧客の情報を展開します。 **[Microsoft Azure の管理ポータル]** を選択して、Azure portal で顧客のレコードを開きます。
3. ポータルのメニューから **[仮想マシン]** を選択し、予約を購入する対象の VM を選択します。
4. VM の詳細ページで、次に示すように、サイズとリージョンの情報を検索し、この情報を使用してパートナーセンターで予約を購入します。  

    ![[詳細] ページのサイズとリージョンの情報](images/usage1.png)

**Microsoft Azure PowerShell を使用して VM サイズ情報を取得する**

下の画像の情報を使用して、予約を購入する対象の VM の場所とサイズを取得します。 

![VM の場所とサイズ](images/usage2.png)

**Azure Resource Manager (ARM) API を使用して VM サイズ情報を取得する**

1. ARMClient または ARM API を使用し、予約を購入する対象の VM に対して ARM クライアントを呼び出します。

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. この呼び出しでは、**vmSize** と **location** の値が返されます (下図参照)。

    ![vmSize 値](images/usage3.png) ![location 値](images/usage4.png)

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Azure VM の使用状況と予約割引を確認する

お客様の代わりに Azure 予約 VM インスタンスを購入すると、事前に VM 領域に対する料金の割引が、お客様の予約の属性と数量に一致する仮想マシンに自動的に適用されます。

次のいずれかの方法を使用して、顧客の予約使用状況を確認し、予約割引が適用されている仮想マシンを確認できます。

- Azure portal
- Azure Utilization API

これらの方法を使用するための手順をそれぞれ以下に示します。

>[!NOTE]
>どの仮想マシンに割引が適用されるかを確認できるのは Azure Utilization API のみです。  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Microsoft Azure portal で顧客の予約使用状況を確認する

1. パートナー センターで **[顧客]** ページに移動します。

2. 予約割引と使用量を確認し、下矢印を選択して顧客の情報を展開します。 **[Microsoft Azure の管理ポータル]** を選択して、Azure portal で顧客のレコードを開きます。
3. ポータルのメニューから **[予約]** を選択し、使用状況を確認する対象の予約を選択します。
4. **[概要]** ページで、予約の使用状況グラフを確認します。これには、仮想マシンに適用された予約の量が表示されます。

    >[!NOTE]
    >使用率データには、最大で 8 時間の遅延が発生することがあります。

    a. 予約の使用率が100% の場合、お客様は予約購入によって得られる節約額をすべて取得することになります。
    b. 予約の使用率が0% の場合、割引は仮想マシンに適用されません。
    c. 予約の使用量が 1 ~ 99% の場合、未使用の特典があります。

5. この状況を回避するには、購入を行う前に、顧客のコンピューティングニーズをサポートする正しいサイズの VM を決定します。

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Azure 使用率 API を使用して顧客の予約使用状況を確認する

>[!NOTE]
>どの仮想マシンに割引が適用されるかを確認できるのは Azure Utilization API のみです。  

Azure Utilization API を使用すると、予約の使用状況データを取得できます。これにより、顧客が予約割引を獲得できるかどうかと、どの VM (仮想マシン) に割引が適用されるかを確認できます。 例 A と例 B を比較して、顧客の予約使用状況を確認する方法を確認してください。

![予約の使用例](images/usage5.png)

- reservationId は、VM に割引を適用するために使用された Azure 予約を識別します。
- consumptionMeter は、予約割引が適用されている VM の MeterId です。
- 予約割引が適用されるため、ReservationMeter には料金として $0 が示されます。

詳細については、[パートナーセンター API](https://docs.microsoft.com/partner-center/develop/)の「 [Azure の顧客の使用状況レコードを取得する](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)」を参照してください。

>[!IMPORTANT]
>現時点では、Microsoft Windows Server などのソフトウェアの料金は VM 予約の価格に含まれず、注文レコードと請求書に個別の明細項目として表示されます。 ただし、顧客が Azure ハイブリッド特典を利用できる場合、ソフトウェア料金は適用されません。 詳しくは、「[Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)」 (予約インスタンスに含まれない Windows ソフトウェアの料金) をご覧ください。  

## <a name="azure-reservations-resources"></a>Azure Reservations に関するリソース

|**情報**   |**参照先**    |
|:-----------------------------|:-----------------|
|CSP での Azure Reservations 概要  | [Microsoft Azure Reserved VM Instances の販売](azure-reservations.md)
|パートナー センターで顧客の Azure Reservations を購入する   |[Azure Reservations を購入する](azure-reservations-buying.md)
|パートナー センターでの Azure Reservations の管理 | [パートナー センターで Azure Reservations を管理する](azure-reservations-manage.md)
|Azure portal で Azure Reservations を購入する | [Azure Reserved VM Instances による仮想マシン料金の前払い](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) (Azure ヘルプ) |
|Azure portal で Azure Reservations を管理する   |[予約済み VM インスタンスの管理](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) (Azure ヘルプ)  |
|パートナー センター API を使用して Azure Reservations を購入する | [Azure Reserved VM Instances の購入](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) (パートナー センター開発者向けドキュメント)
