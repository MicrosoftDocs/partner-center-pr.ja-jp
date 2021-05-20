---
title: 最大限の予約使用に備えた Azure VM サイズ
description: 仮想マシン (VM) を顧客のコンピューティングニーズに合Microsoft Azureする方法について説明します。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 14d488091227e30909b3d41af0684494a8b55de7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149453"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>最大限の予約使用に備えた Microsoft Azure VM サイズ

**適切なロール**: 管理エージェント |セールス エージェント

この記事では、仮想マシン (VM) を顧客のコンピューティングニーズに合Microsoft Azureについて説明します。
 
> [!NOTE]
> この記事は、クラウド ソリューション プロバイダー (CSP) プログラムのパートナーにのみ適用されます。 他の種類のサブスクリプション (例: 使用料、個人、Microsoft 顧客契約、Enterprise Agreement サブスクリプション) を使用しているお客様は、代わりに、この Azure の予約に関するドキュメントをお読 [みください](/azure/cost-management-billing/reservations)。

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>顧客の Azure 予約の VM サイズを決定する

顧客に代Microsoft Azure予約を購入する場合は、顧客のコンピューティング ニーズに合わせてサイズが設定された仮想マシン (VM) を選択する必要があります。 この情報は、次のいずれかの方法を使用して確認できます。

- Azure Utilization API
- Azure ポータル
- Azure PowerShell
- Azure Resource Manager (ARM) API

これらの方法を使用するための手順をそれぞれ以下に示します。 予約を購入した後、予約の属性および数量に一致する仮想マシンに予約割引が自動的に適用されます。 予約を VM に割り当てる必要はない。

>[!NOTE]
>予約割引は、クラシック VM またはプロモーション VM には適用されません。

>[!IMPORTANT]
>顧客に代わって購入する VM の種類とサイズを正しく特定するには、以下で説明するいずれかの方法を使用する必要があります。パートナー センターの調整ファイルには、VM 系列の種類が正しく表示されません。

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Azure Utilization API を使用して VM サイズ情報を取得する

1. API の応答に含まれる additionalInfo の ServiceType 属性の値を使用して、購入する VM サイズ を特定します。

2. 詳細については、Azure の [顧客](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) の使用状況レコードの取得に関するページを参照パートナー センター [してください](/partner-center/develop/)。

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Microsoft Azure portal を使用して VM サイズ情報を取得する

1. パートナー センターで **[顧客]** ページに移動します。

2. Azure VM の予約を購入する顧客を探し、下矢印を選択して顧客の情報を展開します。 **[Microsoft Azure の管理ポータル]** を選択して、顧客のレコードを Azure portal。

3. ポータルのメニューから **[仮想マシン]** を選択し、予約を購入する対象の VM を選択します。

4. VM の詳細ページで、次に示すサイズとリージョンの情報を見つけ、この情報を使用して パートナー センター で予約を購入します。  

   :::image type="content" source="images/usage1.png" alt-text="[詳細] ページのサイズとリージョンの情報":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Microsoft Azure PowerShell を使用して VM サイズ情報を取得する

下の画像の情報を使用して、予約を購入する対象の VM の場所とサイズを取得します。 

:::image type="content" source="images/usage2.png" alt-text="VM の場所とサイズ":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Azure Resource Manager (ARM) API を使用して VM サイズ情報を取得する

1. ARMClient または ARM API を使用し、予約を購入する対象の VM に対して ARM クライアントを呼び出します。

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. この呼び出しでは、**vmSize** と **location** の値が返されます (下図参照)。

    :::image type="content" source="images/usage3.png" alt-text="vmSize 値":::
    :::image type="content" source="images/usage4.png" alt-text="location 値":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Azure VM の使用状況と予約割引を確認する

顧客に代わって Azure 予約 VM インスタンスを購入した後、事前に VM 領域の支払いを行う割引は、顧客の予約の属性と数量に一致する仮想マシンに自動的に適用されます。

次のいずれかの方法を使用して、顧客の予約の使用状況を確認し、予約割引が適用される仮想マシンを確認できます。

- Azure ポータル
- Azure Utilization API

これらの方法を使用するための手順をそれぞれ以下に示します。

>[!NOTE]
>どの仮想マシンに割引が適用されるかを確認できるのは Azure Utilization API のみです。  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>次の手順で顧客の予約の使用状況を確認Microsoft Azure portal

1. パートナー センターで **[顧客]** ページに移動します。

2. 予約割引と使用量を確認し、下矢印を選択して顧客の情報を展開します。 [ **Microsoft Azure の管理ポータル** ] を選択して、Azure portal で顧客のレコードを開きます。
3. ポータルのメニューから **[予約]** を選択し、使用状況を確認する対象の予約を選択します。
4. [ **概要** ] ページで、予約の使用状況グラフを確認します。これには、仮想マシンに適用された予約の量が表示されます。

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

:::image type="content" source="images/usage5.png" alt-text="予約の使用例":::

- reservationId は、VM に割引を適用するために使用された Azure 予約を識別します。
- consumptionMeter は、予約割引が適用されている VM の MeterId です。
- 予約割引が適用されるため、ReservationMeter には料金として $0 が示されます。

詳細については、[パートナーセンター API](/partner-center/develop/)の「 [Azure の顧客の使用状況レコードを取得する](/partner-center/develop/get-a-customer-s-utilization-record-for-azure)」を参照してください。

>[!IMPORTANT]
>現時点では、Microsoft Windows Server などのソフトウェアの料金は VM 予約の価格に含まれず、注文レコードと請求書に個別の明細項目として表示されます。 ただし、顧客が Azure ハイブリッド特典を利用できる場合、ソフトウェア料金は適用されません。 詳しくは、「[Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs)」 (予約インスタンスに含まれない Windows ソフトウェアの料金) をご覧ください。  

## <a name="next-steps"></a>次のステップ

|**対象**   |**参照先**    |
|:-----------------------------|:-----------------|
|CSP での Azure Reservations 概要  | [Microsoft Azure Reserved VM Instances の販売](azure-reservations.md)
|パートナー センターで顧客の Azure Reservations を購入する   | [Azure Reservations を購入する](azure-reservations-buying.md)
|パートナー センターでの Azure Reservations の管理 | [パートナー センターでの Azure Reservations の管理](azure-reservations-manage.md)
|Azure portal で Azure Reservations を購入する | [Azure Reserved VM Instances による仮想マシン料金の前払い](/azure/virtual-machines/windows/prepay-reserved-vm-instances) (Azure ヘルプ) |
|Azure portal で Azure Reservations を管理する   | [予約済み VM インスタンスの管理](/azure/billing/billing-manage-reserved-vm-instance) (Azure ヘルプ)  |
|パートナー センター API を使用して Azure Reservations を購入する | [Azure Reserved VM Instances の購入](/partner-center/develop/purchase-azure-reservations) (パートナー センター開発者向けドキュメント)   |
|購入したサブスクリプションから独自の Azure 予約を購入するためのアクセス許可を顧客に付与します。 | [独自の Azure 予約を購入するためのアクセス許可を顧客に付与する](give-customers-permission.md)   |