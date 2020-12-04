---
title: マネージド サービスのパートナー獲得クレジット
ms.topic: article
ms.date: 11/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: マネージド サービスに対する Microsoft パートナー獲得クレジット (PEC) の計算および支払方法と、お客様が適格であることを確認する方法について説明します。
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 97af446c4021e9785833374131eee2f08431b5fe
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474310"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="22d04-103">パートナー獲得クレジットの計算方法と支払方法</span><span class="sxs-lookup"><span data-stu-id="22d04-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="22d04-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="22d04-104">**Appropriate roles**</span></span>

- <span data-ttu-id="22d04-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="22d04-105">Global admin</span></span>
- <span data-ttu-id="22d04-106">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="22d04-106">User admin</span></span>
- <span data-ttu-id="22d04-107">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="22d04-107">Admin agent</span></span>
- <span data-ttu-id="22d04-108">課金管理者</span><span class="sxs-lookup"><span data-stu-id="22d04-108">Billing admin</span></span>
- <span data-ttu-id="22d04-109">販売代理店</span><span class="sxs-lookup"><span data-stu-id="22d04-109">Sales agent</span></span>

<span data-ttu-id="22d04-110">マネージド サービスのパートナー獲得クレジット (PEC) では、顧客の Azure 環境の一部または全体の IT の運用と管理を 24 時間 365 日体制で実施しているパートナーを認識してリワードが提供されます。</span><span class="sxs-lookup"><span data-stu-id="22d04-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="22d04-111">既定では、CSP では、顧客のサブスクリプションに対して必要なアクセス権がパートナーに付与されます。これにより、パートナーは、サブスクリプションのリソースに対する運用管理と制御を 24 時間 365 日体制で実行できます。</span><span class="sxs-lookup"><span data-stu-id="22d04-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="22d04-112">次のセクションで、パートナーと取引するために顧客がアクセスをプロビジョニングするその他の方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="22d04-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="22d04-113">月々の請求額は、パートナー獲得クレジットのネット値です。</span><span class="sxs-lookup"><span data-stu-id="22d04-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="22d04-114">パートナーは、毎月の調整ファイルで PEC の詳細を確認できます。</span><span class="sxs-lookup"><span data-stu-id="22d04-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="22d04-115">パートナーと取引するために顧客がアクセスをプロビジョニングするその他の方法については、「[Azure プランのサブスクリプションとリソースを管理する](azure-plan-manage.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22d04-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="22d04-116">また、「[Azure CSP サブスクリプションの管理者特権を復元する](revoke-reinstate-csp.md)」もご覧ください</span><span class="sxs-lookup"><span data-stu-id="22d04-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="important-eligibility-and-calculation-information"></a><span data-ttu-id="22d04-117">参加資格と計算に関する重要な情報</span><span class="sxs-lookup"><span data-stu-id="22d04-117">Important eligibility and calculation information</span></span>

- <span data-ttu-id="22d04-118">パートナーは、管理する Azure 資産に対して獲得したクレジットを受け取るには、アクティブな MPN 契約と有効な RBAC ロールが必要です。</span><span class="sxs-lookup"><span data-stu-id="22d04-118">Partner should have an active MPN agreement and valid RBAC role to receive earned credit for the Azure assets they manage.</span></span> 

- <span data-ttu-id="22d04-119">間接プロバイダーと間接リセラーの場合、間接プロバイダーは、間接プロバイダーか間接リセラーのどちらか一方またはその両方が 24 時間 365 日体制で顧客の CSP 内の Azure リソースを運用管理しているのであれば、PEC を獲得する資格があります。</span><span class="sxs-lookup"><span data-stu-id="22d04-119">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider, or the indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="22d04-120">PEC は、パートナーによって管理される CSP 内の顧客の Azure 資産に対して課金される (請求可能な) 消費量に関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="22d04-120">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> <span data-ttu-id="22d04-121">PEC は、Microsoft (間接プロバイダーと直接請求パートナー) によって課金される CSP のパートナーに対してのみ利用可能にすることができます。</span><span class="sxs-lookup"><span data-stu-id="22d04-121">PEC is made available only to partners in CSP billed by Microsoft (indirect provider and direct bill partner).</span></span> 

- <span data-ttu-id="22d04-122">対象となるサービス:パートナー獲得クレジットは、パートナーが [Azure プランの価格](https://partner.microsoft.com/commerce/sales)ページからエクスポートできる **Azure プランの従量課金価格** に記載されているサービスに適用されます。</span><span class="sxs-lookup"><span data-stu-id="22d04-122">Eligible services: Partner earned credit is applicable to services listed in the **Azure plan consumption pricing** which partners can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span> 

- <span data-ttu-id="22d04-123">対象とならないサービス: パートナー獲得クレジットは、以下のものには適用 "\**_されません_* _"</span><span class="sxs-lookup"><span data-stu-id="22d04-123">Ineligible services: Partner earned credit is \**_not_* _ applicable to the following:</span></span>
    - <span data-ttu-id="22d04-124">Azure プランの予約</span><span class="sxs-lookup"><span data-stu-id="22d04-124">Azure Plan reservations</span></span>
    - <span data-ttu-id="22d04-125">Azure プラン従量課金価格の **[タグ] 列** に "*サード パーティ*" と表示されているサード パーティ製品</span><span class="sxs-lookup"><span data-stu-id="22d04-125">Third-party products identified as _ *Third Party*\* in the **Tags column** of the Azure plan consumption price</span></span>    
    - <span data-ttu-id="22d04-126">Marketplace 価格表の製品</span><span class="sxs-lookup"><span data-stu-id="22d04-126">Products in the Marketplace price list</span></span>
   - [<span data-ttu-id="22d04-127">Azure スポット仮想マシン</span><span class="sxs-lookup"><span data-stu-id="22d04-127">Azure Spot Virtual Machines</span></span>](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- <span data-ttu-id="22d04-128">PEC は日単位で計算され、毎日の使用状況ファイルと毎月の請求調整ファイルで確認できます。</span><span class="sxs-lookup"><span data-stu-id="22d04-128">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="22d04-129">パートナー (間接プロバイダーまたは間接リセラー) が PEC を確実に取得するには、終日 (24 時間 365 日) のアクセス権を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="22d04-129">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="22d04-130">PEC は、マネージド Azure 資産を対象として 1 日単位で計算されます。</span><span class="sxs-lookup"><span data-stu-id="22d04-130">PEC is calculated on daily basis on the managed Azure assets.</span></span> <span data-ttu-id="22d04-131">特定の請求期間 (月) に対する最大 PEC は 15% です。</span><span class="sxs-lookup"><span data-stu-id="22d04-131">The maximum PEC for a given billing period (Month) is 15%.</span></span> <span data-ttu-id="22d04-132">パートナーは、永続的な特権アクセスを月中ずっと保持し (アクセスの期間)、かつそれがすべての対象リソースに及ぶなら (アクセスの範囲)、15% の全 PEC を獲得します。</span><span class="sxs-lookup"><span data-stu-id="22d04-132">Partners retaining persistent privileged access through the month(span of access) and for all the eligible resources (scope of access) will earn full PEC of 15%.</span></span> <span data-ttu-id="22d04-133">範囲と期間が減ると、その月の PEC レートは低くなります。</span><span class="sxs-lookup"><span data-stu-id="22d04-133">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="22d04-134">毎日評価される使用量ファイルには、特定の Azure 資産について PEC が適用されているかどうかが 1 日単位で示されます。</span><span class="sxs-lookup"><span data-stu-id="22d04-134">Daily rated usage file shows on daily basis on an Azure asset whether PEC is applied or not.</span></span> <span data-ttu-id="22d04-135">パートナーは、永続的な特権アクセスに対する変更があるかどうかを検出するアラートに登録することもできます。</span><span class="sxs-lookup"><span data-stu-id="22d04-135">Partners can also enroll in alerts to detect if there are changes to persistent privileged access.</span></span>

- <span data-ttu-id="22d04-136">PEC は、Azure リソース レベルで獲得されます。</span><span class="sxs-lookup"><span data-stu-id="22d04-136">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="22d04-137">パートナーがサブスクリプションまたはリソース グループ レベルで有効なアクセス権を持っている場合は、上位のエンティティにまとめられるリソースごとに PEC が獲得されます。</span><span class="sxs-lookup"><span data-stu-id="22d04-137">If the partner has valid access at the subscription, or resource group level, each resource that roles up to the higher entity will earn PEC.</span></span>  

- <span data-ttu-id="22d04-138">PEC の詳細は、[Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners) でも確認できます。</span><span class="sxs-lookup"><span data-stu-id="22d04-138">PEC details will also be available on [Azure Cost management](/azure/cost-management-billing/costs/get-started-partners)</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="22d04-139">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="22d04-139">Azure Cost Management</span></span>

<span data-ttu-id="22d04-140">コスト分析を使用する Azure Cost Management (ACM) を使用すると、パートナーは、PEC の特典を受けたコストを表示できます。</span><span class="sxs-lookup"><span data-stu-id="22d04-140">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="22d04-141">[Azure portal](https://portal.azure.com) で、パートナー テナントにサインインし、 **[コストの管理と請求]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="22d04-141">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="22d04-142">**[コスト管理]** を選択します</span><span class="sxs-lookup"><span data-stu-id="22d04-142">Select **Cost management**</span></span>

3. <span data-ttu-id="22d04-143">**[コスト分析]** を選択します</span><span class="sxs-lookup"><span data-stu-id="22d04-143">Select **Cost Analysis**</span></span>

   <span data-ttu-id="22d04-144">[コスト分析] ビューには、Microsoft に支払った料金で購入および使用したすべてのサービスについて、課金アカウントのコストが表示されます。</span><span class="sxs-lookup"><span data-stu-id="22d04-144">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="22d04-145">PEC が適用されているコストを表示するには、ピボット グラフのドロップダウンで **PartnerEarnedCreditApplied** を選択します。</span><span class="sxs-lookup"><span data-stu-id="22d04-145">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="22d04-146">**PartnerEarnedCreditApplied** プロパティが True の場合、関連付けられているコストには、パートナー獲得クレジットの特典が適用されています。</span><span class="sxs-lookup"><span data-stu-id="22d04-146">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

<span data-ttu-id="22d04-147">PartnerEarnedCreditApplied プロパティが False の場合、関連付けられているコストはクレジットに必要な資格を満たしていないか、購入したサービスがパートナー獲得クレジットの対象になっていません。</span><span class="sxs-lookup"><span data-stu-id="22d04-147">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

>[!NOTE] 
><span data-ttu-id="22d04-148">通常、使用したサービスが **[コスト管理]** に表示されるまでには 8 から 24 時間かかり、PEC クレジットは Azure Cost Management にアクセスしてから 48 時間以内に表示されます。</span><span class="sxs-lookup"><span data-stu-id="22d04-148">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="22d04-149">また、 **[Group by and Add]\(グループ化と追加\)** フィルター機能を使用して **PartnerEarnedCreditApplied** プロパティでグループ化およびフィルター処理を行い、PEC が適用されたコストおよび PEC が適用されていないコストを詳しく調べることもできます。</span><span class="sxs-lookup"><span data-stu-id="22d04-149">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="22d04-150">次の手順</span><span class="sxs-lookup"><span data-stu-id="22d04-150">Next steps</span></span>

- [<span data-ttu-id="22d04-151">パートナー獲得クレジット - 概要</span><span class="sxs-lookup"><span data-stu-id="22d04-151">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="22d04-152">パートナー獲得クレジットの計算の詳細な例については、パートナー センター ダッシュボードで確認できる価格表をご覧ください (サインインする必要があります)。</span><span class="sxs-lookup"><span data-stu-id="22d04-152">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="22d04-153">Azure プランに移行する - はじめに</span><span class="sxs-lookup"><span data-stu-id="22d04-153">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="22d04-154">Azure プランのサブスクリプションとリソースを管理する</span><span class="sxs-lookup"><span data-stu-id="22d04-154">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="22d04-155">Azure CSP サブスクリプションの管理者特権の取り消しまたは復元</span><span class="sxs-lookup"><span data-stu-id="22d04-155">Revoke or re-instate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)
