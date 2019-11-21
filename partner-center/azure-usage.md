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
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="a71d8-104">最大限の予約使用に備えた Microsoft Azure VM サイズ</span><span class="sxs-lookup"><span data-stu-id="a71d8-104">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="a71d8-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="a71d8-105">**Applies to**</span></span>

- <span data-ttu-id="a71d8-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="a71d8-106">Partner Center</span></span>
- <span data-ttu-id="a71d8-107">Azure portal</span><span class="sxs-lookup"><span data-stu-id="a71d8-107">Azure portal</span></span>
- <span data-ttu-id="a71d8-108">CSP のパートナー</span><span class="sxs-lookup"><span data-stu-id="a71d8-108">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="a71d8-109">顧客の Azure 予約の VM サイズを決定する</span><span class="sxs-lookup"><span data-stu-id="a71d8-109">Determine the VM size for a customer's Azure reservation</span></span> 

<span data-ttu-id="a71d8-110">お客様の代わりに Microsoft Azure 予約を購入する場合は、お客様のコンピューティングニーズに合わせて仮想マシン (VM) のサイズを選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a71d8-110">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="a71d8-111">この情報は、次のいずれかの方法を使用して確認できます。</span><span class="sxs-lookup"><span data-stu-id="a71d8-111">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="a71d8-112">Azure Utilization API</span><span class="sxs-lookup"><span data-stu-id="a71d8-112">Azure utilization API</span></span>
- <span data-ttu-id="a71d8-113">Azure portal</span><span class="sxs-lookup"><span data-stu-id="a71d8-113">The Azure portal</span></span>
- <span data-ttu-id="a71d8-114">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a71d8-114">Azure PowerShell</span></span>
- <span data-ttu-id="a71d8-115">Azure Resource Manager (ARM) API</span><span class="sxs-lookup"><span data-stu-id="a71d8-115">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="a71d8-116">これらの方法を使用するための手順をそれぞれ以下に示します。</span><span class="sxs-lookup"><span data-stu-id="a71d8-116">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="a71d8-117">予約を購入した後、予約の属性および数量に一致する仮想マシンに予約割引が自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="a71d8-117">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="a71d8-118">VM に予約を割り当てる必要はありません。</span><span class="sxs-lookup"><span data-stu-id="a71d8-118">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="a71d8-119">予約割引は、クラシックまたはプロモーションの Vm には適用されません。</span><span class="sxs-lookup"><span data-stu-id="a71d8-119">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="a71d8-120">顧客に代わって購入する VM の種類とサイズを正しく特定するには、以下で説明するいずれかの方法を使用する必要があります。パートナー センターの調整ファイルには、VM 系列の種類が正しく表示されません。</span><span class="sxs-lookup"><span data-stu-id="a71d8-120">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

<span data-ttu-id="a71d8-121">**Azure Utilization API を使用して VM サイズ情報を取得する**</span><span class="sxs-lookup"><span data-stu-id="a71d8-121">**Get VM sizing information using the Azure utilization API**</span></span>

1. <span data-ttu-id="a71d8-122">API の応答に含まれる additionalInfo の ServiceType 属性の値を使用して、購入する VM サイズ を特定します。</span><span class="sxs-lookup"><span data-stu-id="a71d8-122">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>
2. <span data-ttu-id="a71d8-123">詳細については、[パートナーセンター API](https://docs.microsoft.com/partner-center/develop/)の「 [Azure の顧客の使用状況レコードを取得する](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a71d8-123">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

<span data-ttu-id="a71d8-124">**Microsoft Azure portal を使用して VM サイズ情報を取得する**</span><span class="sxs-lookup"><span data-stu-id="a71d8-124">**Get VM sizing information using the Microsoft Azure portal**</span></span>

1. <span data-ttu-id="a71d8-125">パートナー センターで **[顧客]** ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="a71d8-125">In Partner Center, go to your **Customers** page.</span></span>
2. <span data-ttu-id="a71d8-126">Azure VM の予約を購入したい顧客を見つけて、下矢印を選択して顧客の情報を展開します。</span><span class="sxs-lookup"><span data-stu-id="a71d8-126">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="a71d8-127">**[Microsoft Azure の管理ポータル]** を選択して、Azure portal で顧客のレコードを開きます。</span><span class="sxs-lookup"><span data-stu-id="a71d8-127">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="a71d8-128">ポータルのメニューから **[仮想マシン]** を選択し、予約を購入する対象の VM を選択します。</span><span class="sxs-lookup"><span data-stu-id="a71d8-128">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>
4. <span data-ttu-id="a71d8-129">VM の詳細ページで、次に示すように、サイズとリージョンの情報を検索し、この情報を使用してパートナーセンターで予約を購入します。</span><span class="sxs-lookup"><span data-stu-id="a71d8-129">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![[詳細] ページのサイズとリージョンの情報](images/usage1.png)

<span data-ttu-id="a71d8-131">**Microsoft Azure PowerShell を使用して VM サイズ情報を取得する**</span><span class="sxs-lookup"><span data-stu-id="a71d8-131">**Get VM sizing information using Microsoft Azure PowerShell**</span></span>

<span data-ttu-id="a71d8-132">下の画像の情報を使用して、予約を購入する対象の VM の場所とサイズを取得します。</span><span class="sxs-lookup"><span data-stu-id="a71d8-132">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![VM の場所とサイズ](images/usage2.png)

<span data-ttu-id="a71d8-134">**Azure Resource Manager (ARM) API を使用して VM サイズ情報を取得する**</span><span class="sxs-lookup"><span data-stu-id="a71d8-134">**Get VM sizing information using the Azure Resource Manager (ARM) API**</span></span>

1. <span data-ttu-id="a71d8-135">ARMClient または ARM API を使用し、予約を購入する対象の VM に対して ARM クライアントを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="a71d8-135">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="a71d8-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="a71d8-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="a71d8-137">この呼び出しでは、**vmSize** と **location** の値が返されます (下図参照)。</span><span class="sxs-lookup"><span data-stu-id="a71d8-137">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    <span data-ttu-id="a71d8-138">![vmSize 値](images/usage3.png) ![location 値](images/usage4.png)</span><span class="sxs-lookup"><span data-stu-id="a71d8-138">![vmSize value](images/usage3.png) ![location value](images/usage4.png)</span></span>

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="a71d8-139">Azure VM の使用状況と予約割引を確認する</span><span class="sxs-lookup"><span data-stu-id="a71d8-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="a71d8-140">お客様の代わりに Azure 予約 VM インスタンスを購入すると、事前に VM 領域に対する料金の割引が、お客様の予約の属性と数量に一致する仮想マシンに自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="a71d8-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="a71d8-141">次のいずれかの方法を使用して、顧客の予約使用状況を確認し、予約割引が適用されている仮想マシンを確認できます。</span><span class="sxs-lookup"><span data-stu-id="a71d8-141">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="a71d8-142">Azure portal</span><span class="sxs-lookup"><span data-stu-id="a71d8-142">The Azure portal</span></span>
- <span data-ttu-id="a71d8-143">Azure Utilization API</span><span class="sxs-lookup"><span data-stu-id="a71d8-143">Azure utilization API</span></span>

<span data-ttu-id="a71d8-144">これらの方法を使用するための手順をそれぞれ以下に示します。</span><span class="sxs-lookup"><span data-stu-id="a71d8-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="a71d8-145">どの仮想マシンに割引が適用されるかを確認できるのは Azure Utilization API のみです。</span><span class="sxs-lookup"><span data-stu-id="a71d8-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="a71d8-146">Microsoft Azure portal で顧客の予約使用状況を確認する</span><span class="sxs-lookup"><span data-stu-id="a71d8-146">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="a71d8-147">パートナー センターで **[顧客]** ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="a71d8-147">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="a71d8-148">予約割引と使用量を確認し、下矢印を選択して顧客の情報を展開します。</span><span class="sxs-lookup"><span data-stu-id="a71d8-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="a71d8-149">**[Microsoft Azure の管理ポータル]** を選択して、Azure portal で顧客のレコードを開きます。</span><span class="sxs-lookup"><span data-stu-id="a71d8-149">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="a71d8-150">ポータルのメニューから **[予約]** を選択し、使用状況を確認する対象の予約を選択します。</span><span class="sxs-lookup"><span data-stu-id="a71d8-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="a71d8-151">**[概要]** ページで、予約の使用状況グラフを確認します。これには、仮想マシンに適用された予約の量が表示されます。</span><span class="sxs-lookup"><span data-stu-id="a71d8-151">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="a71d8-152">使用率データには、最大で 8 時間の遅延が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="a71d8-152">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="a71d8-153">a.</span><span class="sxs-lookup"><span data-stu-id="a71d8-153">a.</span></span> <span data-ttu-id="a71d8-154">予約の使用率が100% の場合、お客様は予約購入によって得られる節約額をすべて取得することになります。</span><span class="sxs-lookup"><span data-stu-id="a71d8-154">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="a71d8-155">b.</span><span class="sxs-lookup"><span data-stu-id="a71d8-155">b.</span></span> <span data-ttu-id="a71d8-156">予約の使用率が0% の場合、割引は仮想マシンに適用されません。</span><span class="sxs-lookup"><span data-stu-id="a71d8-156">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="a71d8-157">c.</span><span class="sxs-lookup"><span data-stu-id="a71d8-157">c.</span></span> <span data-ttu-id="a71d8-158">予約の使用量が 1 ~ 99% の場合、未使用の特典があります。</span><span class="sxs-lookup"><span data-stu-id="a71d8-158">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="a71d8-159">この状況を回避するには、購入を行う前に、顧客のコンピューティングニーズをサポートする正しいサイズの VM を決定します。</span><span class="sxs-lookup"><span data-stu-id="a71d8-159">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="a71d8-160">Azure 使用率 API を使用して顧客の予約使用状況を確認する</span><span class="sxs-lookup"><span data-stu-id="a71d8-160">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="a71d8-161">どの仮想マシンに割引が適用されるかを確認できるのは Azure Utilization API のみです。</span><span class="sxs-lookup"><span data-stu-id="a71d8-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="a71d8-162">Azure Utilization API を使用すると、予約の使用状況データを取得できます。これにより、顧客が予約割引を獲得できるかどうかと、どの VM (仮想マシン) に割引が適用されるかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="a71d8-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="a71d8-163">例 A と例 B を比較して、顧客の予約使用状況を確認する方法を確認してください。</span><span class="sxs-lookup"><span data-stu-id="a71d8-163">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

![予約の使用例](images/usage5.png)

- <span data-ttu-id="a71d8-165">reservationId は、VM に割引を適用するために使用された Azure 予約を識別します。</span><span class="sxs-lookup"><span data-stu-id="a71d8-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="a71d8-166">consumptionMeter は、予約割引が適用されている VM の MeterId です。</span><span class="sxs-lookup"><span data-stu-id="a71d8-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="a71d8-167">予約割引が適用されるため、ReservationMeter には料金として $0 が示されます。</span><span class="sxs-lookup"><span data-stu-id="a71d8-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="a71d8-168">詳細については、[パートナーセンター API](https://docs.microsoft.com/partner-center/develop/)の「 [Azure の顧客の使用状況レコードを取得する](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a71d8-168">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="a71d8-169">現時点では、Microsoft Windows Server などのソフトウェアの料金は VM 予約の価格に含まれず、注文レコードと請求書に個別の明細項目として表示されます。</span><span class="sxs-lookup"><span data-stu-id="a71d8-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="a71d8-170">ただし、顧客が Azure ハイブリッド特典を利用できる場合、ソフトウェア料金は適用されません。</span><span class="sxs-lookup"><span data-stu-id="a71d8-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="a71d8-171">詳しくは、「[Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)」 (予約インスタンスに含まれない Windows ソフトウェアの料金) をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a71d8-171">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="a71d8-172">Azure Reservations に関するリソース</span><span class="sxs-lookup"><span data-stu-id="a71d8-172">Azure reservations resources</span></span>

|<span data-ttu-id="a71d8-173">**情報**</span><span class="sxs-lookup"><span data-stu-id="a71d8-173">**For information about**</span></span>   |<span data-ttu-id="a71d8-174">**参照先**</span><span class="sxs-lookup"><span data-stu-id="a71d8-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="a71d8-175">CSP での Azure Reservations 概要</span><span class="sxs-lookup"><span data-stu-id="a71d8-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="a71d8-176">Microsoft Azure Reserved VM Instances の販売</span><span class="sxs-lookup"><span data-stu-id="a71d8-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="a71d8-177">パートナー センターで顧客の Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="a71d8-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="a71d8-178">Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="a71d8-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="a71d8-179">パートナー センターでの Azure Reservations の管理</span><span class="sxs-lookup"><span data-stu-id="a71d8-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="a71d8-180">パートナー センターで Azure Reservations を管理する</span><span class="sxs-lookup"><span data-stu-id="a71d8-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="a71d8-181">Azure portal で Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="a71d8-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="a71d8-182">[Azure Reserved VM Instances による仮想マシン料金の前払い](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) (Azure ヘルプ)</span><span class="sxs-lookup"><span data-stu-id="a71d8-182">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="a71d8-183">Azure portal で Azure Reservations を管理する</span><span class="sxs-lookup"><span data-stu-id="a71d8-183">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="a71d8-184">[予約済み VM インスタンスの管理](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) (Azure ヘルプ)</span><span class="sxs-lookup"><span data-stu-id="a71d8-184">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="a71d8-185">パートナー センター API を使用して Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="a71d8-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="a71d8-186">[Azure Reserved VM Instances の購入](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) (パートナー センター開発者向けドキュメント)</span><span class="sxs-lookup"><span data-stu-id="a71d8-186">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>
