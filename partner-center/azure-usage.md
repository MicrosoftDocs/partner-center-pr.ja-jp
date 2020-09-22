---
title: 最大限の予約使用に備えた Azure VM サイズ
description: Microsoft Azure の予約を購入した場合に、お客様のコンピューティングニーズに合わせて仮想マシン (VM) のサイズを変更する方法について説明します。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: e6c4e3e7a68de720f586754703308a447d7d30c1
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000187"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="7157c-103">最大限の予約使用に備えた Microsoft Azure VM サイズ</span><span class="sxs-lookup"><span data-stu-id="7157c-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="7157c-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="7157c-104">**Applies to**</span></span>

- <span data-ttu-id="7157c-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="7157c-105">Partner Center</span></span>
- <span data-ttu-id="7157c-106">Azure portal</span><span class="sxs-lookup"><span data-stu-id="7157c-106">Azure portal</span></span>
- <span data-ttu-id="7157c-107">CSP プログラムのパートナー</span><span class="sxs-lookup"><span data-stu-id="7157c-107">Partners in the CSP program</span></span>
 
> [!NOTE]
> <span data-ttu-id="7157c-108">この記事は、クラウドソリューションプロバイダー (CSP) プログラムのパートナーにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="7157c-108">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="7157c-109">他の種類のサブスクリプション (従量課金制、個人、Microsoft カスタマーアグリーメント、マイクロソフトエンタープライズ契約サブスクリプションなど) を使用しているお客様は、代わりに [この Azure 予約ドキュメント](/azure/cost-management-billing/reservations)を読む必要があります。</span><span class="sxs-lookup"><span data-stu-id="7157c-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="7157c-110">顧客の Azure 予約の VM サイズを決定する</span><span class="sxs-lookup"><span data-stu-id="7157c-110">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="7157c-111">お客様の代わりに Microsoft Azure 予約を購入する場合は、お客様のコンピューティングニーズに合わせて仮想マシン (VM) のサイズを選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7157c-111">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="7157c-112">この情報は、次のいずれかの方法を使用して確認できます。</span><span class="sxs-lookup"><span data-stu-id="7157c-112">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="7157c-113">Azure Utilization API</span><span class="sxs-lookup"><span data-stu-id="7157c-113">Azure utilization API</span></span>
- <span data-ttu-id="7157c-114">Azure ポータル</span><span class="sxs-lookup"><span data-stu-id="7157c-114">The Azure portal</span></span>
- <span data-ttu-id="7157c-115">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="7157c-115">Azure PowerShell</span></span>
- <span data-ttu-id="7157c-116">Azure Resource Manager (ARM) API</span><span class="sxs-lookup"><span data-stu-id="7157c-116">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="7157c-117">これらの方法を使用するための手順をそれぞれ以下に示します。</span><span class="sxs-lookup"><span data-stu-id="7157c-117">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="7157c-118">予約を購入した後、予約の属性および数量に一致する仮想マシンに予約割引が自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="7157c-118">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="7157c-119">VM に予約を割り当てる必要はありません。</span><span class="sxs-lookup"><span data-stu-id="7157c-119">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="7157c-120">予約割引は、クラシックまたはプロモーションの Vm には適用されません。</span><span class="sxs-lookup"><span data-stu-id="7157c-120">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="7157c-121">顧客に代わって購入する VM の種類とサイズを正しく特定するには、以下で説明するいずれかの方法を使用する必要があります。パートナー センターの調整ファイルには、VM 系列の種類が正しく表示されません。</span><span class="sxs-lookup"><span data-stu-id="7157c-121">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="7157c-122">Azure Utilization API を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="7157c-122">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="7157c-123">API の応答に含まれる additionalInfo の ServiceType 属性の値を使用して、購入する VM サイズ を特定します。</span><span class="sxs-lookup"><span data-stu-id="7157c-123">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="7157c-124">詳細については、[パートナーセンター API](/partner-center/develop/)の「 [Azure の顧客の使用状況レコードを取得する](/partner-center/develop/get-a-customer-s-utilization-record-for-azure)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7157c-124">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="7157c-125">Microsoft Azure portal を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="7157c-125">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="7157c-126">パートナー センターで **[顧客]** ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="7157c-126">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="7157c-127">Azure VM の予約を購入したい顧客を見つけて、下矢印を選択して顧客の情報を展開します。</span><span class="sxs-lookup"><span data-stu-id="7157c-127">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="7157c-128">[ **Microsoft Azure の管理ポータル** ] を選択して、Azure portal で顧客のレコードを開きます。</span><span class="sxs-lookup"><span data-stu-id="7157c-128">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="7157c-129">ポータルのメニューから **[仮想マシン]** を選択し、予約を購入する対象の VM を選択します。</span><span class="sxs-lookup"><span data-stu-id="7157c-129">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="7157c-130">VM の詳細ページで、次に示すように、サイズとリージョンの情報を検索し、この情報を使用してパートナーセンターで予約を購入します。</span><span class="sxs-lookup"><span data-stu-id="7157c-130">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="[詳細] ページのサイズとリージョンの情報":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="7157c-132">Microsoft Azure PowerShell を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="7157c-132">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="7157c-133">下の画像の情報を使用して、予約を購入する対象の VM の場所とサイズを取得します。</span><span class="sxs-lookup"><span data-stu-id="7157c-133">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM の場所とサイズ":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="7157c-135">Azure Resource Manager (ARM) API を使用して VM サイズ情報を取得する</span><span class="sxs-lookup"><span data-stu-id="7157c-135">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="7157c-136">ARMClient または ARM API を使用し、予約を購入する対象の VM に対して ARM クライアントを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="7157c-136">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="7157c-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="7157c-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="7157c-138">この呼び出しでは、**vmSize** と **location** の値が返されます (下図参照)。</span><span class="sxs-lookup"><span data-stu-id="7157c-138">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize 値":::
    :::image type="content" source="images/usage4.png" alt-text="場所の値":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="7157c-141">Azure VM の使用状況と予約割引を確認する</span><span class="sxs-lookup"><span data-stu-id="7157c-141">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="7157c-142">お客様の代わりに Azure 予約 VM インスタンスを購入すると、事前に VM 領域に対する料金の割引が、お客様の予約の属性と数量に一致する仮想マシンに自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="7157c-142">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="7157c-143">次のいずれかの方法を使用して、顧客の予約使用状況を確認し、予約割引が適用されている仮想マシンを確認できます。</span><span class="sxs-lookup"><span data-stu-id="7157c-143">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="7157c-144">Azure ポータル</span><span class="sxs-lookup"><span data-stu-id="7157c-144">The Azure portal</span></span>
- <span data-ttu-id="7157c-145">Azure Utilization API</span><span class="sxs-lookup"><span data-stu-id="7157c-145">Azure utilization API</span></span>

<span data-ttu-id="7157c-146">これらの方法を使用するための手順をそれぞれ以下に示します。</span><span class="sxs-lookup"><span data-stu-id="7157c-146">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="7157c-147">どの仮想マシンに割引が適用されるかを確認できるのは Azure Utilization API のみです。</span><span class="sxs-lookup"><span data-stu-id="7157c-147">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="7157c-148">Microsoft Azure portal で顧客の予約使用状況を確認する</span><span class="sxs-lookup"><span data-stu-id="7157c-148">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="7157c-149">パートナー センターで **[顧客]** ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="7157c-149">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="7157c-150">予約割引と使用量を確認し、下矢印を選択して顧客の情報を展開します。</span><span class="sxs-lookup"><span data-stu-id="7157c-150">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="7157c-151">[ **Microsoft Azure の管理ポータル** ] を選択して、Azure portal で顧客のレコードを開きます。</span><span class="sxs-lookup"><span data-stu-id="7157c-151">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="7157c-152">ポータルのメニューから **[予約]** を選択し、使用状況を確認する対象の予約を選択します。</span><span class="sxs-lookup"><span data-stu-id="7157c-152">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="7157c-153">[ **概要** ] ページで、予約の使用状況グラフを確認します。これには、仮想マシンに適用された予約の量が表示されます。</span><span class="sxs-lookup"><span data-stu-id="7157c-153">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="7157c-154">使用率データには、最大で 8 時間の遅延が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="7157c-154">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="7157c-155">a.</span><span class="sxs-lookup"><span data-stu-id="7157c-155">a.</span></span> <span data-ttu-id="7157c-156">予約の使用率が100% の場合、お客様は予約購入によって得られる節約額をすべて取得することになります。</span><span class="sxs-lookup"><span data-stu-id="7157c-156">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="7157c-157">b.</span><span class="sxs-lookup"><span data-stu-id="7157c-157">b.</span></span> <span data-ttu-id="7157c-158">予約の使用率が0% の場合、割引は仮想マシンに適用されません。</span><span class="sxs-lookup"><span data-stu-id="7157c-158">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="7157c-159">c.</span><span class="sxs-lookup"><span data-stu-id="7157c-159">c.</span></span> <span data-ttu-id="7157c-160">予約の使用量が 1 ~ 99% の場合、未使用の特典があります。</span><span class="sxs-lookup"><span data-stu-id="7157c-160">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="7157c-161">この状況を回避するには、購入を行う前に、顧客のコンピューティングニーズをサポートする正しいサイズの VM を決定します。</span><span class="sxs-lookup"><span data-stu-id="7157c-161">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="7157c-162">Azure 使用率 API を使用して顧客の予約使用状況を確認する</span><span class="sxs-lookup"><span data-stu-id="7157c-162">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="7157c-163">どの仮想マシンに割引が適用されるかを確認できるのは Azure Utilization API のみです。</span><span class="sxs-lookup"><span data-stu-id="7157c-163">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="7157c-164">Azure Utilization API を使用すると、予約の使用状況データを取得できます。これにより、顧客が予約割引を獲得できるかどうかと、どの VM (仮想マシン) に割引が適用されるかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="7157c-164">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="7157c-165">例 A と例 B を比較して、顧客の予約使用状況を確認する方法を確認してください。</span><span class="sxs-lookup"><span data-stu-id="7157c-165">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="予約の使用例":::

- <span data-ttu-id="7157c-167">reservationId は、VM に割引を適用するために使用された Azure 予約を識別します。</span><span class="sxs-lookup"><span data-stu-id="7157c-167">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="7157c-168">consumptionMeter は、予約割引が適用されている VM の MeterId です。</span><span class="sxs-lookup"><span data-stu-id="7157c-168">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="7157c-169">予約割引が適用されるため、ReservationMeter には料金として $0 が示されます。</span><span class="sxs-lookup"><span data-stu-id="7157c-169">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="7157c-170">詳細については、[パートナーセンター API](/partner-center/develop/)の「 [Azure の顧客の使用状況レコードを取得する](/partner-center/develop/get-a-customer-s-utilization-record-for-azure)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7157c-170">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="7157c-171">現時点では、Microsoft Windows Server などのソフトウェアの料金は VM 予約の価格に含まれず、注文レコードと請求書に個別の明細項目として表示されます。</span><span class="sxs-lookup"><span data-stu-id="7157c-171">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="7157c-172">ただし、顧客が Azure ハイブリッド特典を利用できる場合、ソフトウェア料金は適用されません。</span><span class="sxs-lookup"><span data-stu-id="7157c-172">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="7157c-173">詳しくは、「[Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs)」 (予約インスタンスに含まれない Windows ソフトウェアの料金) をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7157c-173">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="7157c-174">Azure Reservations に関するリソース</span><span class="sxs-lookup"><span data-stu-id="7157c-174">Azure reservations resources</span></span>

|<span data-ttu-id="7157c-175">**対象**</span><span class="sxs-lookup"><span data-stu-id="7157c-175">**For information about**</span></span>   |<span data-ttu-id="7157c-176">**参照先**</span><span class="sxs-lookup"><span data-stu-id="7157c-176">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="7157c-177">CSP での Azure Reservations 概要</span><span class="sxs-lookup"><span data-stu-id="7157c-177">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="7157c-178">Microsoft Azure Reserved VM Instances の販売</span><span class="sxs-lookup"><span data-stu-id="7157c-178">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="7157c-179">パートナー センターで顧客の Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="7157c-179">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="7157c-180">Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="7157c-180">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="7157c-181">パートナー センターでの Azure Reservations の管理</span><span class="sxs-lookup"><span data-stu-id="7157c-181">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="7157c-182">パートナー センターでの Azure Reservations の管理</span><span class="sxs-lookup"><span data-stu-id="7157c-182">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="7157c-183">Azure portal で Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="7157c-183">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="7157c-184">[Azure Reserved VM Instances による仮想マシン料金の前払い](/azure/virtual-machines/windows/prepay-reserved-vm-instances) (Azure ヘルプ)</span><span class="sxs-lookup"><span data-stu-id="7157c-184">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="7157c-185">Azure portal で Azure Reservations を管理する</span><span class="sxs-lookup"><span data-stu-id="7157c-185">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="7157c-186">[予約済み VM インスタンスの管理](/azure/billing/billing-manage-reserved-vm-instance) (Azure ヘルプ)</span><span class="sxs-lookup"><span data-stu-id="7157c-186">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="7157c-187">パートナー センター API を使用して Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="7157c-187">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="7157c-188">[Azure Reserved VM Instances の購入](/partner-center/develop/purchase-azure-reservations) (パートナー センター開発者向けドキュメント)</span><span class="sxs-lookup"><span data-stu-id="7157c-188">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="7157c-189">購入したサブスクリプションから独自の Azure 予約を購入するためのアクセス許可を顧客に付与します。</span><span class="sxs-lookup"><span data-stu-id="7157c-189">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="7157c-190">独自の Azure 予約を購入するためのアクセス許可を顧客に付与する</span><span class="sxs-lookup"><span data-stu-id="7157c-190">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |