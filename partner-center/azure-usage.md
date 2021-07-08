---
title: 最大限の予約使用に備えた Azure VM サイズ
description: 仮想マシン (VM) を顧客のコンピューティング ニーズに合Microsoft Azureする方法について説明します。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 650618de7460f4667c60ac58cbe6716530db7f16
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510195"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="3b2ea-103">最大限の予約使用に備えた Microsoft Azure VM サイズ</span><span class="sxs-lookup"><span data-stu-id="3b2ea-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="3b2ea-104">**適切なロール**: 管理エージェント |セールス エージェント</span><span class="sxs-lookup"><span data-stu-id="3b2ea-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="3b2ea-105">この記事では、仮想マシン (VM) を顧客のコンピューティングニーズに合Microsoft Azureについて説明します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="3b2ea-106">この記事は、クラウド ソリューション プロバイダー (CSP) プログラムのパートナーにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="3b2ea-107">他の種類のサブスクリプション (例: 使用料、個人、Microsoft 顧客契約、Enterprise Agreement サブスクリプション) を使用しているお客様は、代わりにこの Azure の予約に関するドキュメントをお読[みください](/azure/cost-management-billing/reservations)。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="3b2ea-108">顧客の Azure 予約の VM サイズを決定する</span><span class="sxs-lookup"><span data-stu-id="3b2ea-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="3b2ea-109">顧客に代Microsoft Azure予約を購入する場合は、顧客のコンピューティングニーズを満たしたサイズの仮想マシン (VM) を選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="3b2ea-110">この情報は、次のいずれかの方法を使用して確認できます。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="3b2ea-111">Azure Utilization API</span><span class="sxs-lookup"><span data-stu-id="3b2ea-111">Azure utilization API</span></span>
- <span data-ttu-id="3b2ea-112">Azure ポータル</span><span class="sxs-lookup"><span data-stu-id="3b2ea-112">The Azure portal</span></span>
- <span data-ttu-id="3b2ea-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="3b2ea-113">Azure PowerShell</span></span>
- <span data-ttu-id="3b2ea-114">Azure Resource Manager (ARM) API</span><span class="sxs-lookup"><span data-stu-id="3b2ea-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="3b2ea-115">これらの方法を使用するための手順をそれぞれ以下に示します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="3b2ea-116">予約を購入した後、予約の属性および数量に一致する仮想マシンに予約割引が自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="3b2ea-117">予約を VM に割り当てる必要はない。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="3b2ea-118">予約割引は、クラシック VM またはプロモーション VM には適用されません。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="3b2ea-119">顧客に代わって購入する VM の種類とサイズを正しく特定するには、以下で説明するいずれかの方法を使用する必要があります。パートナー センターの調整ファイルには、VM 系列の種類が正しく表示されません。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="3b2ea-120">Azure Utilization API を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="3b2ea-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="3b2ea-121">API の応答に含まれる additionalInfo の ServiceType 属性の値を使用して、購入する VM サイズ を特定します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="3b2ea-122">詳細については、Azure の [顧客](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) の使用状況レコードの取得に関するページを参照パートナー センター [してください](/partner-center/develop/)。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="3b2ea-123">Microsoft Azure portal を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="3b2ea-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="3b2ea-124">パートナー センターで **[顧客]** ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="3b2ea-125">Azure VM の予約を購入する顧客を探し、下矢印を選択して顧客の情報を展開します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="3b2ea-126">**[Microsoft Azure 管理ポータル]** を選択して、顧客のレコードを Azure portal。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="3b2ea-127">ポータルのメニューから **[仮想マシン]** を選択し、予約を購入する対象の VM を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="3b2ea-128">VM の詳細ページで、次に示すサイズとリージョンの情報を見つけ、この情報を使用して パートナー センター で予約を購入します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="詳細ページのサイズとリージョンの情報。":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="3b2ea-130">Microsoft Azure PowerShell を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="3b2ea-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="3b2ea-131">下の画像の情報を使用して、予約を購入する対象の VM の場所とサイズを取得します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM の場所とサイズ。":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="3b2ea-133">Azure Resource Manager (ARM) API を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="3b2ea-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="3b2ea-134">ARMClient または ARM API を使用し、予約を購入する対象の VM に対して ARM クライアントを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. <span data-ttu-id="3b2ea-135">この呼び出しでは、**vmSize** と **location** の値が返されます (下図参照)。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-135">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize 値。":::
    :::image type="content" source="images/usage4.png" alt-text="location 値。":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="3b2ea-138">Azure VM の使用状況と予約割引を確認する</span><span class="sxs-lookup"><span data-stu-id="3b2ea-138">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="3b2ea-139">顧客に代わって Azure 予約 VM インスタンスを購入した後、事前に VM 領域の支払いを行う割引は、顧客の予約の属性と数量に一致する仮想マシンに自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-139">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="3b2ea-140">次のいずれかの方法を使用して、顧客の予約の使用状況を確認し、予約割引が適用される仮想マシンを確認できます。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-140">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="3b2ea-141">Azure ポータル</span><span class="sxs-lookup"><span data-stu-id="3b2ea-141">The Azure portal</span></span>
- <span data-ttu-id="3b2ea-142">Azure Utilization API</span><span class="sxs-lookup"><span data-stu-id="3b2ea-142">Azure utilization API</span></span>

<span data-ttu-id="3b2ea-143">これらの方法を使用するための手順をそれぞれ以下に示します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-143">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="3b2ea-144">どの仮想マシンに割引が適用されるかを確認できるのは Azure Utilization API のみです。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-144">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="3b2ea-145">ポータルで顧客の予約の使用状況をMicrosoft Azureする</span><span class="sxs-lookup"><span data-stu-id="3b2ea-145">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="3b2ea-146">パートナー センターで **[顧客]** ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-146">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="3b2ea-147">予約割引と使用状況を確認する顧客を探し、下矢印を選択して顧客の情報を展開します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-147">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="3b2ea-148">**[Microsoft Azure 管理ポータル]** を選択して、顧客のレコードを Azure portal。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-148">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="3b2ea-149">ポータルのメニューから **[予約]** を選択し、使用状況を確認する対象の予約を選択します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-149">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="3b2ea-150">[概要 **] ページ** で、予約の使用率グラフを確認します。これは、仮想マシンに適用された予約の量を示します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-150">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="3b2ea-151">使用率データには、最大で 8 時間の遅延が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-151">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="3b2ea-152">a.</span><span class="sxs-lookup"><span data-stu-id="3b2ea-152">a.</span></span> <span data-ttu-id="3b2ea-153">予約の使用率が 100% の場合、顧客は予約購入で提供できるすべての節約を受け取っています。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-153">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="3b2ea-154">b.</span><span class="sxs-lookup"><span data-stu-id="3b2ea-154">b.</span></span> <span data-ttu-id="3b2ea-155">予約の使用量が 0% の場合、割引は仮想マシンに適用されません。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-155">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="3b2ea-156">c.</span><span class="sxs-lookup"><span data-stu-id="3b2ea-156">c.</span></span> <span data-ttu-id="3b2ea-157">予約の使用量が 1% から 99% の場合、未使用の特典があります。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-157">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="3b2ea-158">この状況を回避するには、購入を行う前に、顧客のコンピューティングニーズをサポートする適切なサイズの VM を決定します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-158">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="3b2ea-159">Azure 使用率 API を使用して顧客の予約の使用状況を確認する</span><span class="sxs-lookup"><span data-stu-id="3b2ea-159">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="3b2ea-160">どの仮想マシンに割引が適用されるかを確認できるのは Azure Utilization API のみです。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-160">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="3b2ea-161">Azure Utilization API を使用すると、予約の使用状況データを取得できます。これにより、顧客が予約割引を獲得できるかどうかと、どの VM (仮想マシン) に割引が適用されるかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-161">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="3b2ea-162">例 A と例 B を比較して、顧客の予約の使用状況を確認する方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-162">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="予約の使用例。":::

- <span data-ttu-id="3b2ea-164">reservationId は、VM に割引を適用するために使用された Azure 予約を識別します。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-164">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="3b2ea-165">consumptionMeter は、予約割引が適用されている VM の MeterId です。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-165">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="3b2ea-166">予約割引が適用されるため、ReservationMeter には料金として $0 が示されます。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-166">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="3b2ea-167">詳細については、Azure の [顧客](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) の使用状況レコードの取得に関するページを参照パートナー センター [してください](/partner-center/develop/)。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-167">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="3b2ea-168">現時点では、Microsoft Windows Server などのソフトウェアの料金は VM 予約の価格に含まれず、注文レコードと請求書に個別の明細項目として表示されます。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-168">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="3b2ea-169">ただし、顧客が Azure ハイブリッド特典を利用できる場合、ソフトウェア料金は適用されません。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-169">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="3b2ea-170">詳しくは、「[Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs)」 (予約インスタンスに含まれない Windows ソフトウェアの料金) をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-170">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="3b2ea-171">次のステップ</span><span class="sxs-lookup"><span data-stu-id="3b2ea-171">Next steps</span></span>

|<span data-ttu-id="3b2ea-172">**対象**</span><span class="sxs-lookup"><span data-stu-id="3b2ea-172">**For information about**</span></span>   |<span data-ttu-id="3b2ea-173">**参照先**</span><span class="sxs-lookup"><span data-stu-id="3b2ea-173">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="3b2ea-174">CSP での Azure Reservations 概要</span><span class="sxs-lookup"><span data-stu-id="3b2ea-174">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="3b2ea-175">Microsoft Azure Reserved VM Instances の販売</span><span class="sxs-lookup"><span data-stu-id="3b2ea-175">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="3b2ea-176">パートナー センターで顧客の Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="3b2ea-176">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="3b2ea-177">Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="3b2ea-177">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="3b2ea-178">パートナー センターでの Azure Reservations の管理</span><span class="sxs-lookup"><span data-stu-id="3b2ea-178">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="3b2ea-179">パートナー センターでの Azure Reservations の管理</span><span class="sxs-lookup"><span data-stu-id="3b2ea-179">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="3b2ea-180">Azure portal で Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="3b2ea-180">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="3b2ea-181">[Azure Reserved VM Instances による仮想マシン料金の前払い](/azure/virtual-machines/windows/prepay-reserved-vm-instances) (Azure ヘルプ)</span><span class="sxs-lookup"><span data-stu-id="3b2ea-181">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="3b2ea-182">Azure portal で Azure Reservations を管理する</span><span class="sxs-lookup"><span data-stu-id="3b2ea-182">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="3b2ea-183">[予約済み VM インスタンスの管理](/azure/billing/billing-manage-reserved-vm-instance) (Azure ヘルプ)</span><span class="sxs-lookup"><span data-stu-id="3b2ea-183">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="3b2ea-184">パートナー センター API を使用して Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="3b2ea-184">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="3b2ea-185">[Azure Reserved VM Instances の購入](/partner-center/develop/purchase-azure-reservations) (パートナー センター開発者向けドキュメント)</span><span class="sxs-lookup"><span data-stu-id="3b2ea-185">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="3b2ea-186">購入したサブスクリプションから独自の Azure 予約を購入するアクセス許可を顧客に付与する。</span><span class="sxs-lookup"><span data-stu-id="3b2ea-186">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="3b2ea-187">顧客に自分の Azure 予約を購入するアクセス許可を付与する</span><span class="sxs-lookup"><span data-stu-id="3b2ea-187">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |