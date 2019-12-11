---
title: マネージド サービスのパートナー獲得クレジット (プレビュー) | パートナー センター
ms.topic: article
ms.date: 10/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: マネージド サービスに対する Microsoft パートナー獲得クレジットの計算および支払方法と、お客様が適格であることを確認する方法について説明します。
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: f22aebcfe9269b15a5916564a5cd1f4707302331
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943075"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="4023b-103">パートナー獲得クレジットの計算方法と支払方法</span><span class="sxs-lookup"><span data-stu-id="4023b-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="4023b-104">マネージド サービスのパートナー獲得クレジット (PEC) では、顧客の Azure 環境の一部または全体の IT の運用と管理を 24 時間 365 日体制で実施しているパートナーを認識してリワードが提供されます。</span><span class="sxs-lookup"><span data-stu-id="4023b-104">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="4023b-105">既定では、CSP では、顧客のサブスクリプションに対して必要なアクセス権がパートナーに付与されます。これにより、パートナーは、サブスクリプションのリソースに対する運用管理と制御を 24 時間 365 日体制で実行できます。</span><span class="sxs-lookup"><span data-stu-id="4023b-105">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="4023b-106">次のセクションで、パートナーと取引するために顧客がアクセスをプロビジョニングするその他の方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="4023b-106">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="4023b-107">月々の請求額は、パートナー獲得クレジットのネット値です。</span><span class="sxs-lookup"><span data-stu-id="4023b-107">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="4023b-108">パートナーは、毎月の調整ファイルで PEC の詳細を確認できます。</span><span class="sxs-lookup"><span data-stu-id="4023b-108">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="4023b-109">パートナーと取引するために顧客がアクセスをプロビジョニングするその他の方法については、「[Azure プランのサブスクリプションとリソースを管理する](azure-plan-manage.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4023b-109">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="4023b-110">また、「[Azure CSP サブスクリプションの管理者特権を復元する](revoke-reinstate-csp.md)」もご覧ください</span><span class="sxs-lookup"><span data-stu-id="4023b-110">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="important-eligibility-and-calculation-information"></a><span data-ttu-id="4023b-111">参加資格と計算に関する重要な情報</span><span class="sxs-lookup"><span data-stu-id="4023b-111">Important eligibility and calculation information</span></span>

- <span data-ttu-id="4023b-112">パートナーは、管理する Azure 資産に対して獲得したクレジットを受け取るには、アクティブな MPN 契約と有効な RBAC ロールが必要です。</span><span class="sxs-lookup"><span data-stu-id="4023b-112">Partner should have an active MPN agreement and valid RBAC role to receive earned credit for the Azure assets they manage.</span></span> 

- <span data-ttu-id="4023b-113">間接プロバイダーと間接リセラーの場合、間接プロバイダーは、間接プロバイダーか間接リセラーのどちらか一方またはその両方が 24 時間 365 日体制で顧客の CSP 内の Azure リソースを運用管理しているのであれば、PEC を獲得する資格があります。</span><span class="sxs-lookup"><span data-stu-id="4023b-113">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider, or the indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="4023b-114">PEC は、パートナーによって管理される CSP 内の顧客の Azure 資産に対して課金される (請求可能な) 消費量に関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="4023b-114">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> <span data-ttu-id="4023b-115">PEC は、Microsoft (間接プロバイダーと直接請求パートナー) によって課金される CSP のパートナーに対してのみ利用可能にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4023b-115">PEC is made available only to partners in CSP billed by Microsoft (indirect provider and direct bill partner).</span></span> 

- <span data-ttu-id="4023b-116">対象となるサービス:パートナー獲得クレジットは、パートナーが [Azure プランの価格](https://partner.microsoft.com/commerce/sales)ページからエクスポートできる **Azure プランの従量課金価格**に記載されているサービスに適用されます。</span><span class="sxs-lookup"><span data-stu-id="4023b-116">Eligible services: Partner earned credit is applicable to services listed in the **Azure plan consumption pricing** which partners can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span> <span data-ttu-id="4023b-117">ただし、Azure プランの従量課金価格および Azure プランの予約の **[Tags]\(タグ\)** 列で **[Third Party]\(サードパーティ\)** として示されているサードパーティ製品や、Marketplace の価格表の製品には (それ以外についても)、例外があります。</span><span class="sxs-lookup"><span data-stu-id="4023b-117">Note, there are exceptions including, but not limited to, third-party products identified as **Third Party** in  the **Tags** column of the Azure plan consumption price list and Azure Plan reservations, and products in the Marketplace price list.</span></span>

- <span data-ttu-id="4023b-118">PEC は日単位で計算され、毎日の使用状況ファイルと毎月の請求調整ファイルで確認できます。</span><span class="sxs-lookup"><span data-stu-id="4023b-118">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="4023b-119">パートナー (間接プロバイダーまたは間接リセラー) が PEC を確実に取得するには、終日 (24 時間 365 日) のアクセス権を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4023b-119">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>  

- <span data-ttu-id="4023b-120">PEC は、Azure リソース レベルで獲得されます。</span><span class="sxs-lookup"><span data-stu-id="4023b-120">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="4023b-121">パートナーがサブスクリプションまたはリソース グループ レベルで有効なアクセス権を持っている場合は、上位のエンティティにまとめられるリソースごとに PEC が獲得されます。</span><span class="sxs-lookup"><span data-stu-id="4023b-121">If the partner has valid access at the subscription, or resource group level, each resource that roles up to the higher entity will earn PEC.</span></span>  

- <span data-ttu-id="4023b-122">PEC の詳細は、[Azure Cost Management](https://go.microsoft.com/fwlink/?linkid=2106482) でも確認できます。</span><span class="sxs-lookup"><span data-stu-id="4023b-122">PEC details will also be available on [Azure Cost management](https://go.microsoft.com/fwlink/?linkid=2106482)</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="4023b-123">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="4023b-123">Azure Cost Management</span></span>

 <span data-ttu-id="4023b-124">コスト分析を使用する Azure Cost Management (ACM) を使用すると、パートナーは、PEC の特典を受けたコストを表示できます。</span><span class="sxs-lookup"><span data-stu-id="4023b-124">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="4023b-125">Azure Portal で、パートナー テナントにサインインし、 **[コストの管理と請求]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="4023b-125">In the Azure Portal, sign into your partner tenant and select **Cost Management + Billing**.</span></span>
2.  <span data-ttu-id="4023b-126">**[コスト管理]** を選択します</span><span class="sxs-lookup"><span data-stu-id="4023b-126">Select **Cost management**</span></span>
3.  <span data-ttu-id="4023b-127">**[コスト分析]** を選択します</span><span class="sxs-lookup"><span data-stu-id="4023b-127">Select **Cost Analysis**</span></span>

<span data-ttu-id="4023b-128">[コスト分析] ビューには、Microsoft に支払った料金で購入および使用したすべてのサービスについて、課金アカウントのコストが表示されます。</span><span class="sxs-lookup"><span data-stu-id="4023b-128">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4.  <span data-ttu-id="4023b-129">PEC が適用されているコストを表示するには、ピボット グラフのドロップダウンで **PartnerEarnedCreditApplied** を選択します。</span><span class="sxs-lookup"><span data-stu-id="4023b-129">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="4023b-130">**PartnerEarnedCreditApplied** プロパティが True の場合、関連付けられているコストには、パートナー獲得クレジットの特典が適用されています。</span><span class="sxs-lookup"><span data-stu-id="4023b-130">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

<span data-ttu-id="4023b-131">PartnerEarnedCreditApplied プロパティが False の場合、関連付けられているコストはクレジットに必要な資格を満たしていないか、購入したサービスがパートナー獲得クレジットの対象になっていません。</span><span class="sxs-lookup"><span data-stu-id="4023b-131">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

<span data-ttu-id="4023b-132">注: 通常、使用したサービスが **[コスト管理]** に表示されるまでには 8 から 24 時間かかり、PEC クレジットは Azure Cost Management にアクセスしてから 48 時間以内に表示されます。</span><span class="sxs-lookup"><span data-stu-id="4023b-132">Note:Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="4023b-133">また、 **[Group by and Add]\(グループ化と追加\)** フィルター機能を使用して **PartnerEarnedCreditApplied** プロパティでグループ化およびフィルター処理を行い、PEC が適用されたコストおよび PEC が適用されていないコストを詳しく調べることもできます。</span><span class="sxs-lookup"><span data-stu-id="4023b-133">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

 <span data-ttu-id="4023b-134">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="4023b-134">**For more information**</span></span>

- [<span data-ttu-id="4023b-135">パートナー獲得クレジット - 概要</span><span class="sxs-lookup"><span data-stu-id="4023b-135">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="4023b-136">パートナー獲得クレジットの計算の詳細な例については、パートナー センター ダッシュボードで確認できる価格表をご覧ください (サインインする必要があります)。</span><span class="sxs-lookup"><span data-stu-id="4023b-136">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="4023b-137">Azure プランに移行する - はじめに</span><span class="sxs-lookup"><span data-stu-id="4023b-137">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="4023b-138">Azure プランのサブスクリプションとリソースを管理する</span><span class="sxs-lookup"><span data-stu-id="4023b-138">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="4023b-139">Azure CSP サブスクリプションの管理者特権を取り消したり元に戻したりする</span><span class="sxs-lookup"><span data-stu-id="4023b-139">Revoke or re-instate admin privileges for Azure CSP subscriptions  </span></span>](revoke-reinstate-csp.md)

