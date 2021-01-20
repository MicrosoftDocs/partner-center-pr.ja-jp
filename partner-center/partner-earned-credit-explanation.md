---
title: マネージド サービスのパートナー獲得クレジット
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: マネージド サービスに対する Microsoft パートナー獲得クレジット (PEC) の計算および支払方法と、お客様が適格であることを確認する方法について説明します。
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f274103feeadfa6fd135f99632f3013c29601972
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182411"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="8784c-103">パートナー獲得クレジットの計算方法と支払方法</span><span class="sxs-lookup"><span data-stu-id="8784c-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="8784c-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="8784c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8784c-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="8784c-105">Global admin</span></span>
- <span data-ttu-id="8784c-106">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="8784c-106">User admin</span></span>
- <span data-ttu-id="8784c-107">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="8784c-107">Admin agent</span></span>
- <span data-ttu-id="8784c-108">課金管理者</span><span class="sxs-lookup"><span data-stu-id="8784c-108">Billing admin</span></span>
- <span data-ttu-id="8784c-109">販売代理店</span><span class="sxs-lookup"><span data-stu-id="8784c-109">Sales agent</span></span>

<span data-ttu-id="8784c-110">マネージド サービスのパートナー獲得クレジット (PEC) では、顧客の Azure 環境の一部または全体の IT の運用と管理を 24 時間 365 日体制で実施しているパートナーを認識してリワードが提供されます。</span><span class="sxs-lookup"><span data-stu-id="8784c-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="8784c-111">既定では、CSP では、顧客のサブスクリプションに対して必要なアクセス権がパートナーに付与されます。これにより、パートナーは、サブスクリプションのリソースに対する運用管理と制御を 24 時間 365 日体制で実行できます。</span><span class="sxs-lookup"><span data-stu-id="8784c-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="8784c-112">次のセクションで、パートナーと取引するために顧客がアクセスをプロビジョニングするその他の方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="8784c-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="8784c-113">月々の請求額は、パートナー獲得クレジットのネット値です。</span><span class="sxs-lookup"><span data-stu-id="8784c-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="8784c-114">パートナーは、毎月の調整ファイルで PEC の詳細を確認できます。</span><span class="sxs-lookup"><span data-stu-id="8784c-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="8784c-115">パートナーと取引するために顧客がアクセスをプロビジョニングするその他の方法については、「[Azure プランのサブスクリプションとリソースを管理する](azure-plan-manage.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8784c-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="8784c-116">また、「[Azure CSP サブスクリプションの管理者特権を復元する](revoke-reinstate-csp.md)」もご覧ください</span><span class="sxs-lookup"><span data-stu-id="8784c-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="eligibility"></a><span data-ttu-id="8784c-117">特典を受ける条件</span><span class="sxs-lookup"><span data-stu-id="8784c-117">Eligibility</span></span>

<span data-ttu-id="8784c-118">パートナー獲得クレジット (PEC) を受け取るには、次の要件が適用されます。</span><span class="sxs-lookup"><span data-stu-id="8784c-118">In order to receive the partner earned credit (PEC), the following requirements apply:</span></span> 

- <span data-ttu-id="8784c-119">自分が管理する Azure 資産に対する獲得クレジットを受け取るには、アクティブな MPN 契約と有効なロールベースのアクセス制御 (RBAC) ロールが必要です。</span><span class="sxs-lookup"><span data-stu-id="8784c-119">You must have an active MPN agreement and valid role-based access control (RBAC) role to receive earned credit for the Azure assets you manage.</span></span>

- <span data-ttu-id="8784c-120">CSP では、顧客の Azure リソースを 24 時間体制で制御し、管理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8784c-120">You must have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span> <span data-ttu-id="8784c-121">つまり、顧客の Azure サブスクリプション、Azure リソース グループ、Azure リソースに対する管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="8784c-121">This means you must have admin privileges on the customer’s Azure subscription, Azure resource group, Azure resource.</span></span> <span data-ttu-id="8784c-122">間接プロバイダーとその間接リセラーの場合、間接プロバイダーは、間接プロバイダーか間接リセラーのどちらか一方またはその両方がこの運用管理を行っているのであれば、PEC を獲得する資格があります。</span><span class="sxs-lookup"><span data-stu-id="8784c-122">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider or the indirect reseller or both have this operational control.</span></span> <span data-ttu-id="8784c-123">詳細については、[Azure CSP サブスクリプションの管理者特権を復元する](./revoke-reinstate-csp.md)ことに関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8784c-123">To learn more about this, see [Reinstate admin privileges for Azure CSP subscriptions](./revoke-reinstate-csp.md).</span></span>

- <span data-ttu-id="8784c-124">上記の要件に加えて、PEC は Azure プランの従量課金価格に記載されているサービスにのみ適用されます。これは [Azure プランの価格](https://partner.microsoft.com/commerce/sales)ページからエクスポートできます。</span><span class="sxs-lookup"><span data-stu-id="8784c-124">In addition to the requirements above, PEC is only applicable to services listed in the Azure plan consumption pricing, which you can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span>

- <span data-ttu-id="8784c-125">PEC は、以下のサービスには適用 **されません**。</span><span class="sxs-lookup"><span data-stu-id="8784c-125">PEC is **not** applicable to the following services:</span></span>
    - <span data-ttu-id="8784c-126">Azure プランの予約</span><span class="sxs-lookup"><span data-stu-id="8784c-126">Azure Plan reservations</span></span>
    - <span data-ttu-id="8784c-127">Azure プラン従量課金価格の [タグ] 列に "サード パーティ" と表示されているサード パーティ製品</span><span class="sxs-lookup"><span data-stu-id="8784c-127">Third-party products identified as Third Party in the Tags column of the Azure plan consumption price</span></span>
    - <span data-ttu-id="8784c-128">Marketplace 価格表の製品</span><span class="sxs-lookup"><span data-stu-id="8784c-128">Products in the Marketplace price list</span></span>
    - [<span data-ttu-id="8784c-129">Azure スポット仮想マシン</span><span class="sxs-lookup"><span data-stu-id="8784c-129">Azure Spot Virtual Machines</span></span>](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- <span data-ttu-id="8784c-130">PEC は、Azure リソース レベルで獲得されます。</span><span class="sxs-lookup"><span data-stu-id="8784c-130">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="8784c-131">サブスクリプションまたはリソース グループ レベルのいずれかで有効なアクセス権をお持ちの場合は、上位のエンティティにまとめられるリソースごとに PEC が獲得されます。</span><span class="sxs-lookup"><span data-stu-id="8784c-131">If you have valid access at either the subscription or resource group level, each resource that rolls up to the higher entity will earn PEC.</span></span>

- <span data-ttu-id="8784c-132">PEC の詳細については、[Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners) に関するページもご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8784c-132">Details on PEC are also available on the [Azure Cost management](/azure/cost-management-billing/costs/get-started-partners) page.</span></span>

### <a name="calculation"></a><span data-ttu-id="8784c-133">計算</span><span class="sxs-lookup"><span data-stu-id="8784c-133">Calculation</span></span>

<span data-ttu-id="8784c-134">PEC は日単位で計算され、毎日の使用状況ファイルと毎月の請求調整ファイルで確認できます。</span><span class="sxs-lookup"><span data-stu-id="8784c-134">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="8784c-135">パートナー (間接プロバイダーまたは間接リセラー) が PEC を確実に取得するには、終日 (24 時間 365 日) のアクセス権を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8784c-135">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="8784c-136">PEC は、マネージド Azure 資産を対象として 1 日単位で計算されます。</span><span class="sxs-lookup"><span data-stu-id="8784c-136">PEC is calculated on a daily basis on the managed Azure assets.</span></span> <span data-ttu-id="8784c-137">特定の請求期間 (月) に対する最大 PEC は 15% です。</span><span class="sxs-lookup"><span data-stu-id="8784c-137">The maximum PEC for a given billing period (Month) is 15%.</span></span> <span data-ttu-id="8784c-138">パートナーは、永続的な特権アクセスを月中ずっと保持し (アクセスの期間)、かつそれがすべての対象リソースに及ぶなら (アクセスの範囲)、15% の全 PEC を獲得します。</span><span class="sxs-lookup"><span data-stu-id="8784c-138">Partners retaining persistent privileged access through the month (span of access) and for all the eligible resources (scope of access) will earn full PEC of 15%.</span></span> <span data-ttu-id="8784c-139">範囲と期間が減ると、その月の PEC レートは低くなります。</span><span class="sxs-lookup"><span data-stu-id="8784c-139">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="8784c-140">毎日評価される使用量ファイルには、特定の Azure 資産について PEC が適用されているかどうかが 1 日単位で示されます。</span><span class="sxs-lookup"><span data-stu-id="8784c-140">Daily rated usage file shows on a daily basis on an Azure asset, whether PEC is applied or not.</span></span> <span data-ttu-id="8784c-141">パートナーは、永続的な特権アクセスに対する変更を監視するためのアラートに登録することもできます。</span><span class="sxs-lookup"><span data-stu-id="8784c-141">Partners can also enroll in alerts to monitor changes to persistent privileged access.</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="8784c-142">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="8784c-142">Azure Cost Management</span></span>

<span data-ttu-id="8784c-143">コスト分析を使用する Azure Cost Management (ACM) を使用すると、パートナーは、PEC の特典を受けたコストを表示できます。</span><span class="sxs-lookup"><span data-stu-id="8784c-143">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="8784c-144">[Azure portal](https://portal.azure.com) で、パートナー テナントにサインインし、 **[コストの管理と請求]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8784c-144">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="8784c-145">**[コスト管理]** を選択します</span><span class="sxs-lookup"><span data-stu-id="8784c-145">Select **Cost management**</span></span>

3. <span data-ttu-id="8784c-146">**[コスト分析]** を選択します</span><span class="sxs-lookup"><span data-stu-id="8784c-146">Select **Cost Analysis**</span></span>

   <span data-ttu-id="8784c-147">[コスト分析] ビューには、Microsoft に支払った料金で購入および使用したすべてのサービスについて、課金アカウントのコストが表示されます。</span><span class="sxs-lookup"><span data-stu-id="8784c-147">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="8784c-148">PEC が適用されているコストを表示するには、ピボット グラフのドロップダウンで **PartnerEarnedCreditApplied** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8784c-148">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="8784c-149">**PartnerEarnedCreditApplied** プロパティが True の場合、関連付けられているコストには、パートナー獲得クレジットの特典が適用されています。</span><span class="sxs-lookup"><span data-stu-id="8784c-149">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

   <span data-ttu-id="8784c-150">PartnerEarnedCreditApplied プロパティが False の場合、関連付けられているコストはクレジットに必要な資格を満たしていないか、購入したサービスがパートナー獲得クレジットの対象になっていません。</span><span class="sxs-lookup"><span data-stu-id="8784c-150">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

   >[!NOTE] 
   ><span data-ttu-id="8784c-151">通常、使用したサービスが **[コスト管理]** に表示されるまでには 8 から 24 時間かかり、PEC クレジットは Azure Cost Management にアクセスしてから 48 時間以内に表示されます。</span><span class="sxs-lookup"><span data-stu-id="8784c-151">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="8784c-152">また、 **[Group by and Add]\(グループ化と追加\)** フィルター機能を使用して **PartnerEarnedCreditApplied** プロパティでグループ化およびフィルター処理を行い、PEC が適用されたコストおよび PEC が適用されていないコストを詳しく調べることもできます。</span><span class="sxs-lookup"><span data-stu-id="8784c-152">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8784c-153">次の手順</span><span class="sxs-lookup"><span data-stu-id="8784c-153">Next steps</span></span>

- [<span data-ttu-id="8784c-154">パートナー獲得クレジット - 概要</span><span class="sxs-lookup"><span data-stu-id="8784c-154">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="8784c-155">パートナー獲得クレジットの計算の詳細な例については、パートナー センター ダッシュボードで確認できる価格表をご覧ください (サインインする必要があります)。</span><span class="sxs-lookup"><span data-stu-id="8784c-155">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="8784c-156">Azure プランに移行する - はじめに</span><span class="sxs-lookup"><span data-stu-id="8784c-156">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="8784c-157">Azure プランのサブスクリプションとリソースを管理する</span><span class="sxs-lookup"><span data-stu-id="8784c-157">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="8784c-158">Azure CSP サブスクリプションの管理者特権の取り消しまたは復元</span><span class="sxs-lookup"><span data-stu-id="8784c-158">Revoke or re-instate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)