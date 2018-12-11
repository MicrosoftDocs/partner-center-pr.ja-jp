---
title: 最大限の予約使用に Microsoft Azure VM サイズ |パートナー センター
ms.topic: article
ms.date: 10/29/2018
Description: When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.
author: v-petand
ms.author: v-petand
keywords: Azure, 予約, VM, 管理, 請求, 使用, サイズ
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 04a027bf50739434f9a6d155eb8a31f4074185a7
ms.sourcegitcommit: 777225c8bf16e4a8811a9d88aceb45fcba1cd959
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/11/2018
ms.locfileid: "8917544"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="0b537-103">最大限の予約使用に備えた Microsoft Azure VM サイズ</span><span class="sxs-lookup"><span data-stu-id="0b537-103">Microsoft Azure VM sizing for maximum reservation usage</span></span> 

**<span data-ttu-id="0b537-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="0b537-104">Applies to</span></span>**

-  <span data-ttu-id="0b537-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="0b537-105">Partner Center</span></span>
-  <span data-ttu-id="0b537-106">Azure portal</span><span class="sxs-lookup"><span data-stu-id="0b537-106">Azure portal</span></span>
-  <span data-ttu-id="0b537-107">CSP のパートナー</span><span class="sxs-lookup"><span data-stu-id="0b537-107">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="0b537-108">顧客の Azure 予約の VM サイズを決定する</span><span class="sxs-lookup"><span data-stu-id="0b537-108">Determine the VM size for a customer’s Azure reservation</span></span> 

<span data-ttu-id="0b537-109">顧客に代わって Microsoft Azure Reservations を購入するときは、顧客のコンピューティング ニーズに合わせて仮想マシン (VM) のサイズを選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0b537-109">When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.</span></span> <span data-ttu-id="0b537-110">この情報は、次のいずれかの方法を使用して確認できます。</span><span class="sxs-lookup"><span data-stu-id="0b537-110">You can find this information using one of these methods:</span></span>

-   <span data-ttu-id="0b537-111">Azure Utilization API</span><span class="sxs-lookup"><span data-stu-id="0b537-111">Azure utilization API</span></span>
-   <span data-ttu-id="0b537-112">Azure portal</span><span class="sxs-lookup"><span data-stu-id="0b537-112">The Azure portal</span></span>
-   <span data-ttu-id="0b537-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="0b537-113">Azure PowerShell</span></span>
-   <span data-ttu-id="0b537-114">Azure Resource Manager (ARM) API</span><span class="sxs-lookup"><span data-stu-id="0b537-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="0b537-115">これらの方法を使用するための手順をそれぞれ以下に示します。</span><span class="sxs-lookup"><span data-stu-id="0b537-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="0b537-116">予約を購入した後、予約の属性および数量に一致する仮想マシンに予約割引が自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0b537-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="0b537-117">予約を VM に割り当てる必要はありません。</span><span class="sxs-lookup"><span data-stu-id="0b537-117">You don’t need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="0b537-118">予約割引は、従来型またはプロモーション用の VM には適用されません。</span><span class="sxs-lookup"><span data-stu-id="0b537-118">Reservation discounts don’t apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="0b537-119">顧客に代わって購入する VM の種類とサイズを正しく特定するには、以下で説明するいずれかの方法を使用する必要があります。パートナー センターの調整ファイルには、VM 系列の種類が正しく表示されません。</span><span class="sxs-lookup"><span data-stu-id="0b537-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>


**<span data-ttu-id="0b537-120">Azure Utilization API を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="0b537-120">Get VM sizing information using the Azure utilization API</span></span>**

1.  <span data-ttu-id="0b537-121">API の応答に含まれる additionalInfo の ServiceType 属性の値を使用して、購入する VM サイズ を特定します。</span><span class="sxs-lookup"><span data-stu-id="0b537-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span> 

2.  <span data-ttu-id="0b537-122">詳しくは、[パートナー センター API](https://docs.microsoft.com/partner-center/develop/) の「[Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)」 (顧客の Azure 使用率レコードを取得する) をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0b537-122">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span> 

**<span data-ttu-id="0b537-123">Microsoft Azure portal を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="0b537-123">Get VM sizing information using the Microsoft Azure portal</span></span>**

1.  <span data-ttu-id="0b537-124">パートナー センターで、[**顧客**] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="0b537-124">In Partner Center, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="0b537-125">Azure VM 予約を購入する顧客を見つけ、下矢印を選択して顧客情報を展開します。</span><span class="sxs-lookup"><span data-stu-id="0b537-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="0b537-126">**[Microsoft Azure の管理ポータル]** を選択すると、Azure portal に顧客レコードが表示されます。</span><span class="sxs-lookup"><span data-stu-id="0b537-126">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="0b537-127">ポータルのメニューから **[仮想マシン]** を選択し、予約を購入する対象の VM を選択します。</span><span class="sxs-lookup"><span data-stu-id="0b537-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span> 

4.  <span data-ttu-id="0b537-128">VM の詳細ページで、サイズと地域の情報を見つけます (下図参照)。パートナー センターで予約を購入する際には、この情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="0b537-128">On the VM’s detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![詳細ページのサイズと地域の情報](images/usage1.png)

**<span data-ttu-id="0b537-130">Microsoft Azure PowerShell を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="0b537-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>**

<span data-ttu-id="0b537-131">下の画像の情報を使用して、予約を購入する対象の VM の場所とサイズを取得します。</span><span class="sxs-lookup"><span data-stu-id="0b537-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![VM の場所とサイズ](images/usage2.png)

**<span data-ttu-id="0b537-133">Azure Resource Manager (ARM) API を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="0b537-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>**

1.  <span data-ttu-id="0b537-134">ARMClient または ARM API を使用し、予約を購入する対象の VM に対して ARM クライアントを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="0b537-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2.  <span data-ttu-id="0b537-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="0b537-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3.  <span data-ttu-id="0b537-136">この呼び出しでは、**vmSize** と **location** の値が返されます (下図参照)。</span><span class="sxs-lookup"><span data-stu-id="0b537-136">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    <span data-ttu-id="0b537-137">![vmSize 値](images/usage3.png)
    ![場所の値](images/usage4.png)</span><span class="sxs-lookup"><span data-stu-id="0b537-137">![vmSize value](images/usage3.png)
![location value](images/usage4.png)</span></span>
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="0b537-138">Azure VM の使用状況と予約割引を確認する</span><span class="sxs-lookup"><span data-stu-id="0b537-138">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="0b537-139">顧客の代わりに Azure Reserved VM Instances を購入した場合は、VM 領域の前払いに対する割引が、顧客の予約の属性および数量に一致する仮想マシンに自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0b537-139">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer’s reservation.</span></span> 

<span data-ttu-id="0b537-140">次のいずれかの方法を使用し、顧客の予約の使用状況を調べて、どの仮想マシンに予約割引が適用されるかを確認します。</span><span class="sxs-lookup"><span data-stu-id="0b537-140">You can verify the customer’s reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>   

-   <span data-ttu-id="0b537-141">Azure portal</span><span class="sxs-lookup"><span data-stu-id="0b537-141">The Azure portal</span></span>
-   <span data-ttu-id="0b537-142">Azure Utilization API</span><span class="sxs-lookup"><span data-stu-id="0b537-142">Azure utilization API</span></span>

<span data-ttu-id="0b537-143">これらの方法を使用するための手順をそれぞれ以下に示します。</span><span class="sxs-lookup"><span data-stu-id="0b537-143">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="0b537-144">どの仮想マシンに割引が適用されるかを確認できるのは Azure Utilization API のみです。</span><span class="sxs-lookup"><span data-stu-id="0b537-144">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="0b537-145">Microsoft Azure portal で顧客の予約の使用状況を確認する</span><span class="sxs-lookup"><span data-stu-id="0b537-145">Verify the customer’s reservation usage in the Microsoft Azure portal</span></span>

1.  <span data-ttu-id="0b537-146">パートナー センターで、[**顧客**] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="0b537-146">In Partner Center, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="0b537-147">予約割引と使用状況を確認する対象の顧客を見つけ、下矢印を選択して顧客情報を展開します。</span><span class="sxs-lookup"><span data-stu-id="0b537-147">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="0b537-148">**[Microsoft Azure の管理ポータル]** を選択すると、Azure portal に顧客レコードが表示されます。</span><span class="sxs-lookup"><span data-stu-id="0b537-148">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="0b537-149">ポータルのメニューから **[予約]** を選択し、使用状況を確認する対象の予約を選択します。</span><span class="sxs-lookup"><span data-stu-id="0b537-149">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span> 

4.  <span data-ttu-id="0b537-150">**[概要]** ページで、予約の使用率グラフを確認します。このグラフには、仮想マシンに適用されている予約の割合が示されています。</span><span class="sxs-lookup"><span data-stu-id="0b537-150">On the **Overview** page check the reservation’s utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span> 

    >[!NOTE]
    ><span data-ttu-id="0b537-151">使用率データには、最大で 8 時間の遅延が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="0b537-151">Utilization data may be delayed by up to 8 hours.</span></span>
    
    <span data-ttu-id="0b537-152">a. </span><span class="sxs-lookup"><span data-stu-id="0b537-152">a.</span></span>  <span data-ttu-id="0b537-153">予約の使用率が 100% の場合は、顧客は予約購入によって可能な節約をすべて適用できます。</span><span class="sxs-lookup"><span data-stu-id="0b537-153">If the reservation’s utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span> 
    
    <span data-ttu-id="0b537-154">b. </span><span class="sxs-lookup"><span data-stu-id="0b537-154">b.</span></span>  <span data-ttu-id="0b537-155">予約の使用率が 0% の場合は、どの仮想マシンにも割引が適用されません。</span><span class="sxs-lookup"><span data-stu-id="0b537-155">If the reservation’s usage is 0%, the discount is not being applied to any virtual machine.</span></span> 
    
    <span data-ttu-id="0b537-156">c. </span><span class="sxs-lookup"><span data-stu-id="0b537-156">c.</span></span>  <span data-ttu-id="0b537-157">予約の使用率が 1% ～ 99% の場合は、特典が一部使用されません。</span><span class="sxs-lookup"><span data-stu-id="0b537-157">If the reservation’s usage is between 1% and 99%, there are unused benefits.</span></span> 

5.  <span data-ttu-id="0b537-158">このような状況を避けるには、購入を行う前に、顧客のコンピューティング ニーズをサポートするために適した VM のサイズを決定します。</span><span class="sxs-lookup"><span data-stu-id="0b537-158">To avoid this situation, determine the correct size VM to support the customer’s computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="0b537-159">Azure Utilization API で顧客の予約の使用状況を確認する</span><span class="sxs-lookup"><span data-stu-id="0b537-159">Verify the customer’s reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="0b537-160">どの仮想マシンに割引が適用されるかを確認できるのは Azure Utilization API のみです。</span><span class="sxs-lookup"><span data-stu-id="0b537-160">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="0b537-161">Azure Utilization API を使用すると、予約の使用状況データを取得できます。これにより、顧客が予約割引を獲得できるかどうかと、どの VM (仮想マシン) に割引が適用されるかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="0b537-161">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="0b537-162">顧客の予約の使用状況を確認する方法については、下の Example A と Example B を比較してください。</span><span class="sxs-lookup"><span data-stu-id="0b537-162">Compare Example A to Example B to see how to verify a customer’s reservation usage.</span></span> 

![予約の使用例](images\usage5.png)

-   <span data-ttu-id="0b537-164">reservationId は、VM に割引を適用するために使用された Azure 予約を識別します。</span><span class="sxs-lookup"><span data-stu-id="0b537-164">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
-   <span data-ttu-id="0b537-165">consumptionMeter は、予約割引が適用されている VM の MeterId です。</span><span class="sxs-lookup"><span data-stu-id="0b537-165">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
-   <span data-ttu-id="0b537-166">予約割引が適用されるため、ReservationMeter には料金として $0 が示されます。</span><span class="sxs-lookup"><span data-stu-id="0b537-166">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span> 

<span data-ttu-id="0b537-167">詳しくは、[パートナー センター API](https://docs.microsoft.com/partner-center/develop/) の「[Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)」 (顧客の Azure 使用率レコードを取得する) をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0b537-167">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="0b537-168">現時点では、Microsoft Windows Server などのソフトウェアの料金は VM 予約の価格に含まれず、注文レコードと請求書に個別の明細項目として表示されます。</span><span class="sxs-lookup"><span data-stu-id="0b537-168">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="0b537-169">ただし、顧客が Azure ハイブリッド特典を利用できる場合、ソフトウェア料金は適用されません。</span><span class="sxs-lookup"><span data-stu-id="0b537-169">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="0b537-170">詳しくは、「[Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)」 (予約インスタンスに含まれない Windows ソフトウェアの料金) をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0b537-170">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="0b537-171">Azure Reservations に関するリソース</span><span class="sxs-lookup"><span data-stu-id="0b537-171">Azure reservations resources</span></span>
|**<span data-ttu-id="0b537-172">情報</span><span class="sxs-lookup"><span data-stu-id="0b537-172">For information about</span></span>**   |**<span data-ttu-id="0b537-173">参照先</span><span class="sxs-lookup"><span data-stu-id="0b537-173">Read this</span></span>**    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="0b537-174">CSP での Azure Reservations 概要</span><span class="sxs-lookup"><span data-stu-id="0b537-174">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="0b537-175">Microsoft Azure Reserved VM Instances の販売</span><span class="sxs-lookup"><span data-stu-id="0b537-175">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="0b537-176">パートナー センターで顧客の Azure reservations を購入します。</span><span class="sxs-lookup"><span data-stu-id="0b537-176">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="0b537-177">Azure Reservations の購入</span><span class="sxs-lookup"><span data-stu-id="0b537-177">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="0b537-178">パートナー センターで Azure reservations を管理します。</span><span class="sxs-lookup"><span data-stu-id="0b537-178">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="0b537-179">パートナー センターで Azure reservations を管理します。</span><span class="sxs-lookup"><span data-stu-id="0b537-179">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="0b537-180">Azure portal で Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="0b537-180">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="0b537-181">[Azure Reserved VM Instances による仮想マシン料金の前払い](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) (Azure ヘルプ)</span><span class="sxs-lookup"><span data-stu-id="0b537-181">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="0b537-182">Azure portal で Azure Reservations を管理する</span><span class="sxs-lookup"><span data-stu-id="0b537-182">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="0b537-183">[予約済み VM インスタンスの管理](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) (Azure ヘルプ)</span><span class="sxs-lookup"><span data-stu-id="0b537-183">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="0b537-184">パートナー センター API を使用して Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="0b537-184">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="0b537-185">[Azure Reserved VM Instances の購入](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) (パートナー センター開発者向けドキュメント)</span><span class="sxs-lookup"><span data-stu-id="0b537-185">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>



