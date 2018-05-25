---
title: 最大限の予約使用に備えた Microsoft Azure VM サイズ | パートナー ダッシュ ボード
Description: Information on purchasing and managing Azure reservations
author: v-petand
keywords: Azure, 予約, VM, 管理, 請求, 使用, サイズ
ms.openlocfilehash: 4050780f9d3dc3ad7d3c4ece0d363845ec1efe9c
ms.sourcegitcommit: 034336ae3a697a97a62ad549b8645c836624efaa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2018
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="3f738-103">最大限の予約使用に備えた Microsoft Azure VM サイズ</span><span class="sxs-lookup"><span data-stu-id="3f738-103">Microsoft Azure VM sizing for maximum reservation usage</span></span> 

**<span data-ttu-id="3f738-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="3f738-104">Applies to</span></span>**

-  <span data-ttu-id="3f738-105">パートナー ダッシュボード</span><span class="sxs-lookup"><span data-stu-id="3f738-105">Partner Dashboard</span></span>
-  <span data-ttu-id="3f738-106">Azure portal</span><span class="sxs-lookup"><span data-stu-id="3f738-106">Azure portal</span></span>
-  <span data-ttu-id="3f738-107">CSP のパートナー</span><span class="sxs-lookup"><span data-stu-id="3f738-107">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="3f738-108">顧客の Azure 予約の VM サイズを決定する</span><span class="sxs-lookup"><span data-stu-id="3f738-108">Determine the VM size for a customer’s Azure reservation</span></span> 

<span data-ttu-id="3f738-109">顧客に代わって Microsoft Azure Reservations を購入するときは、顧客のコンピューティング ニーズに合わせて仮想マシン (VM) のサイズを選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3f738-109">When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.</span></span> <span data-ttu-id="3f738-110">この情報は、次のいずれかの方法を使用して確認できます。</span><span class="sxs-lookup"><span data-stu-id="3f738-110">You can find this information using one of these methods:</span></span>

-   <span data-ttu-id="3f738-111">Azure Utilization API</span><span class="sxs-lookup"><span data-stu-id="3f738-111">Azure utilization API</span></span>
-   <span data-ttu-id="3f738-112">Azure portal</span><span class="sxs-lookup"><span data-stu-id="3f738-112">The Azure portal</span></span>
-   <span data-ttu-id="3f738-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="3f738-113">Azure PowerShell</span></span>
-   <span data-ttu-id="3f738-114">Azure Resource Manager (ARM) API</span><span class="sxs-lookup"><span data-stu-id="3f738-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="3f738-115">これらの方法を使用するための手順をそれぞれ以下に示します。</span><span class="sxs-lookup"><span data-stu-id="3f738-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="3f738-116">予約を購入した後、予約の属性および数量に一致する仮想マシンに予約割引が自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3f738-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="3f738-117">予約を VM に割り当てる必要はありません。</span><span class="sxs-lookup"><span data-stu-id="3f738-117">You don’t need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="3f738-118">予約割引は、従来型またはプロモーション用の VM には適用されません。</span><span class="sxs-lookup"><span data-stu-id="3f738-118">Reservation discounts don’t apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="3f738-119">顧客に代わって購入する VM の種類とサイズを正しく特定するには、以下で説明するいずれかの方法を使用する必要があります。パートナー センターの調整ファイルには、VM 系列の種類が正しく表示されません。</span><span class="sxs-lookup"><span data-stu-id="3f738-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>


**<span data-ttu-id="3f738-120">Azure Utilization API を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="3f738-120">Get VM sizing information using the Azure utilization API</span></span>**

1.  <span data-ttu-id="3f738-121">API の応答に含まれる additionalInfo の ServiceType 属性の値を使用して、購入する VM サイズ を特定します。</span><span class="sxs-lookup"><span data-stu-id="3f738-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span> 

2.  <span data-ttu-id="3f738-122">詳しくは、[パートナー ダッシュボード API](https://docs.microsoft.com/partner-center/develop/) の「[Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)」 (顧客の Azure 使用率レコードを取得する) をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3f738-122">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Dashboard API](https://docs.microsoft.com/partner-center/develop/).</span></span> 

**<span data-ttu-id="3f738-123">Microsoft Azure portal を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="3f738-123">Get VM sizing information using the Microsoft Azure portal</span></span>**

1.  <span data-ttu-id="3f738-124">パートナー ダッシュ ボードで、**[顧客]** ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="3f738-124">In your Partner Dashboard, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="3f738-125">Azure VM 予約を購入する顧客を見つけ、下矢印を選択して顧客情報を展開します。</span><span class="sxs-lookup"><span data-stu-id="3f738-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="3f738-126">**[Microsoft Azure の管理ポータル]** を選択すると、Azure portal に顧客レコードが表示されます。</span><span class="sxs-lookup"><span data-stu-id="3f738-126">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="3f738-127">ポータルのメニューから **[仮想マシン]** を選択し、予約を購入する対象の VM を選択します。</span><span class="sxs-lookup"><span data-stu-id="3f738-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span> 

4.  <span data-ttu-id="3f738-128">VM の詳細ページで、サイズと地域の情報を見つけます (下図参照)。パートナー センターで予約を購入する際には、この情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="3f738-128">On the VM’s detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![](images/usage1.png)

**<span data-ttu-id="3f738-129">Microsoft Azure PowerShell を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="3f738-129">Get VM sizing information using Microsoft Azure PowerShell</span></span>**

<span data-ttu-id="3f738-130">下の画像の情報を使用して、予約を購入する対象の VM の場所とサイズを取得します。</span><span class="sxs-lookup"><span data-stu-id="3f738-130">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![](images/usage2.png)

**<span data-ttu-id="3f738-131">Azure Resource Manager (ARM) API を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="3f738-131">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>**

1.  <span data-ttu-id="3f738-132">ARMClient または ARM API を使用し、予約を購入する対象の VM に対して ARM クライアントを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="3f738-132">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2.  <span data-ttu-id="3f738-133">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="3f738-133">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3.  <span data-ttu-id="3f738-134">この呼び出しでは、**vmSize** と **location** の値が返されます (下図参照)。</span><span class="sxs-lookup"><span data-stu-id="3f738-134">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    ![](images/usage3.png)
    ![](images/usage4.png)
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="3f738-135">Azure VM の使用状況と予約割引を確認する</span><span class="sxs-lookup"><span data-stu-id="3f738-135">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="3f738-136">顧客の代わりに Azure Reserved VM Instances を購入した場合は、VM 領域の前払いに対する割引が、顧客の予約の属性および数量に一致する仮想マシンに自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3f738-136">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer’s reservation.</span></span> 

<span data-ttu-id="3f738-137">次のいずれかの方法を使用し、顧客の予約の使用状況を調べて、どの仮想マシンに予約割引が適用されるかを確認します。</span><span class="sxs-lookup"><span data-stu-id="3f738-137">You can verify the customer’s reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>   

-   <span data-ttu-id="3f738-138">Azure portal</span><span class="sxs-lookup"><span data-stu-id="3f738-138">The Azure portal</span></span>
-   <span data-ttu-id="3f738-139">Azure Utilization API</span><span class="sxs-lookup"><span data-stu-id="3f738-139">Azure utilization API</span></span>

<span data-ttu-id="3f738-140">これらの方法を使用するための手順をそれぞれ以下に示します。</span><span class="sxs-lookup"><span data-stu-id="3f738-140">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="3f738-141">どの仮想マシンに割引が適用されるかを確認できるのは Azure Utilization API のみです。</span><span class="sxs-lookup"><span data-stu-id="3f738-141">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="3f738-142">Microsoft Azure portal で顧客の予約の使用状況を確認する</span><span class="sxs-lookup"><span data-stu-id="3f738-142">Verify the customer’s reservation usage in the Microsoft Azure portal</span></span>

1.  <span data-ttu-id="3f738-143">パートナー ダッシュ ボードで、**[顧客]** ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="3f738-143">In your Partner Dashboard, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="3f738-144">予約割引と使用状況を確認する対象の顧客を見つけ、下矢印を選択して顧客情報を展開します。</span><span class="sxs-lookup"><span data-stu-id="3f738-144">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="3f738-145">**[Microsoft Azure の管理ポータル]** を選択すると、Azure portal に顧客レコードが表示されます。</span><span class="sxs-lookup"><span data-stu-id="3f738-145">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="3f738-146">ポータルのメニューから **[予約]** を選択し、使用状況を確認する対象の予約を選択します。</span><span class="sxs-lookup"><span data-stu-id="3f738-146">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span> 

4.  <span data-ttu-id="3f738-147">**[概要]** ページで、予約の使用率グラフを確認します。このグラフには、仮想マシンに適用されている予約の割合が示されています。</span><span class="sxs-lookup"><span data-stu-id="3f738-147">On the **Overview** page check the reservation’s utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span> 

    >[!NOTE]
    ><span data-ttu-id="3f738-148">使用率データには、最大で 8 時間の遅延が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="3f738-148">Utilization data may be delayed by up to 8 hours.</span></span>
    
    <span data-ttu-id="3f738-149">a. </span><span class="sxs-lookup"><span data-stu-id="3f738-149">a.</span></span>  <span data-ttu-id="3f738-150">予約の使用率が 100% の場合は、顧客は予約購入によって可能な節約をすべて適用できます。</span><span class="sxs-lookup"><span data-stu-id="3f738-150">If the reservation’s utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span> 
    
    <span data-ttu-id="3f738-151">b. </span><span class="sxs-lookup"><span data-stu-id="3f738-151">b.</span></span>  <span data-ttu-id="3f738-152">予約の使用率が 0% の場合は、どの仮想マシンにも割引が適用されません。</span><span class="sxs-lookup"><span data-stu-id="3f738-152">If the reservation’s usage is 0%, the discount is not being applied to any virtual machine.</span></span> 
    
    <span data-ttu-id="3f738-153">c. </span><span class="sxs-lookup"><span data-stu-id="3f738-153">c.</span></span>  <span data-ttu-id="3f738-154">予約の使用率が 1% ～ 99% の場合は、特典が一部使用されません。</span><span class="sxs-lookup"><span data-stu-id="3f738-154">If the reservation’s usage is between 1% and 99%, there are unused benefits.</span></span> 

5.  <span data-ttu-id="3f738-155">このような状況を避けるには、購入を行う前に、顧客のコンピューティング ニーズをサポートするために適した VM のサイズを決定します。</span><span class="sxs-lookup"><span data-stu-id="3f738-155">To avoid this situation, determine the correct size VM to support the customer’s computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="3f738-156">Azure Utilization API で顧客の予約の使用状況を確認する</span><span class="sxs-lookup"><span data-stu-id="3f738-156">Verify the customer’s reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="3f738-157">どの仮想マシンに割引が適用されるかを確認できるのは Azure Utilization API のみです。</span><span class="sxs-lookup"><span data-stu-id="3f738-157">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="3f738-158">Azure Utilization API を使用すると、予約の使用状況データを取得できます。これにより、顧客が予約割引を獲得できるかどうかと、どの VM (仮想マシン) に割引が適用されるかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="3f738-158">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="3f738-159">顧客の予約の使用状況を確認する方法については、下の Example A と Example B を比較してください。</span><span class="sxs-lookup"><span data-stu-id="3f738-159">Compare Example A to Example B to see how to verify a customer’s reservation usage.</span></span> 

![](images\usage5.png)

-   <span data-ttu-id="3f738-160">reservationId は、VM に割引を適用するために使用された Azure 予約を識別します。</span><span class="sxs-lookup"><span data-stu-id="3f738-160">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
-   <span data-ttu-id="3f738-161">consumptionMeter は、予約割引が適用されている VM の MeterId です。</span><span class="sxs-lookup"><span data-stu-id="3f738-161">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
-   <span data-ttu-id="3f738-162">予約割引が適用されるため、ReservationMeter には料金として $0 が示されます。</span><span class="sxs-lookup"><span data-stu-id="3f738-162">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span> 

<span data-ttu-id="3f738-163">詳しくは、[パートナー ダッシュボード API](https://docs.microsoft.com/partner-center/develop/) の「[Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)」 (顧客の Azure 使用率レコードを取得する) をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3f738-163">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Dashboard API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="3f738-164">現時点では、Microsoft Windows Server などのソフトウェアの料金は VM 予約の価格に含まれず、注文レコードと請求書に個別の明細項目として表示されます。</span><span class="sxs-lookup"><span data-stu-id="3f738-164">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="3f738-165">ただし、顧客が Azure ハイブリッド特典を利用できる場合、ソフトウェア料金は適用されません。</span><span class="sxs-lookup"><span data-stu-id="3f738-165">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="3f738-166">詳しくは、「[Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)」 (予約インスタンスに含まれない Windows ソフトウェアの料金) をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3f738-166">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="3f738-167">Azure Reservations に関するリソース</span><span class="sxs-lookup"><span data-stu-id="3f738-167">Azure reservations resources</span></span>
|**<span data-ttu-id="3f738-168">情報</span><span class="sxs-lookup"><span data-stu-id="3f738-168">For information about</span></span>**   |**<span data-ttu-id="3f738-169">参照先</span><span class="sxs-lookup"><span data-stu-id="3f738-169">Read this</span></span>**    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="3f738-170">CSP での Azure Reservations 概要</span><span class="sxs-lookup"><span data-stu-id="3f738-170">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="3f738-171">Microsoft Azure Reserved VM Instances の販売</span><span class="sxs-lookup"><span data-stu-id="3f738-171">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="3f738-172">パートナー ダッシュボードで顧客の Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="3f738-172">Purchasing Azure reservations for your customers in your Partner Dashboard</span></span>   |[<span data-ttu-id="3f738-173">Azure Reservations の購入</span><span class="sxs-lookup"><span data-stu-id="3f738-173">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="3f738-174">Azure Reservations の請求</span><span class="sxs-lookup"><span data-stu-id="3f738-174">Billing for Azure reservations</span></span>   |[<span data-ttu-id="3f738-175">Azure Reservations の請求</span><span class="sxs-lookup"><span data-stu-id="3f738-175">Billing for Azure reservations</span></span>](azure-reservations-billing.md)   |
| <span data-ttu-id="3f738-176">パートナー ダッシュボードで Azure Reservations を管理する</span><span class="sxs-lookup"><span data-stu-id="3f738-176">Managing Azure reservations in your Partner Dashboard</span></span> | [<span data-ttu-id="3f738-177">パートナー ダッシュボードで Azure Reservations を管理する</span><span class="sxs-lookup"><span data-stu-id="3f738-177">Managing Azure reservations in your Partner Dashboard</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="3f738-178">Azure portal で Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="3f738-178">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="3f738-179">[Azure Reserved VM Instances による仮想マシン料金の前払い](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) (Azure ヘルプ)</span><span class="sxs-lookup"><span data-stu-id="3f738-179">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="3f738-180">Azure portal で Azure Reservations を管理する</span><span class="sxs-lookup"><span data-stu-id="3f738-180">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="3f738-181">[予約済み VM インスタンスの管理](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) (Azure ヘルプ)</span><span class="sxs-lookup"><span data-stu-id="3f738-181">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="3f738-182">パートナー センター API を使用して Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="3f738-182">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="3f738-183">[Azure Reserved VM Instances の購入](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) (パートナー センター開発者向けドキュメント)</span><span class="sxs-lookup"><span data-stu-id="3f738-183">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) in the Partner Center developer documentation</span></span>



