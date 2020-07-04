---
title: パートナー獲得クレジットの計算方法
ms.topic: article
ms.date: 06/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure プランのパートナー獲得クレジット (PEC) の側面を計算する方法について説明します。 これには、パートナーと間接プロバイダーの資格要件が含まれます。
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOJUNE.20
ms.openlocfilehash: 065cf0c8f95667b470081edcb1b66398235604b3
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948132"
---
# <a name="how-partner-earned-credit-pec-is-calculated-for-partners-in-the-cloud-solution-provider-program"></a><span data-ttu-id="c7bbb-104">クラウドソリューションプロバイダープログラムのパートナーに対してパートナーの獲得クレジット (PEC) を計算する方法</span><span class="sxs-lookup"><span data-stu-id="c7bbb-104">How partner earned credit (PEC) is calculated for partners in the Cloud Solution Provider program</span></span>

<span data-ttu-id="c7bbb-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="c7bbb-105">**Appropriate roles**</span></span>

- <span data-ttu-id="c7bbb-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="c7bbb-106">Global admin</span></span>
- <span data-ttu-id="c7bbb-107">課金管理者</span><span class="sxs-lookup"><span data-stu-id="c7bbb-107">Billing admin</span></span>

<span data-ttu-id="c7bbb-108">Microsoft 365 年中無休の IT 運用管理、または CSP における顧客の Azure 環境全体を所有するパートナーは、PEC を利用できます。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-108">Partners who own the 24x7 IT operations management of parts or the entire Azure environment of their customers in CSP are rewarded with PEC.</span></span> <span data-ttu-id="c7bbb-109">PEC は、Microsoft との直接の課金関係を持つパートナーに請求書の一部として提供されます。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-109">The PEC is provided as part of the invoice to the partner who has a direct billing relationship with Microsoft.</span></span> <span data-ttu-id="c7bbb-110">クレジットは日単位で計算され、月次請求書に反映されます。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-110">The credit is calculated daily and reflected in the monthly invoice.</span></span> <span data-ttu-id="c7bbb-111">CSP の既定では、顧客のサブスクリプションに対する必要なアクセス権がパートナーに付与されます。これにより、サブスクリプションのリソースを24時間365日体制で管理し、制御することができます。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription that allows them to have 24X7 operations management and control of the resources on the subscription.</span></span> <span data-ttu-id="c7bbb-112">次のセクションでは、お客様が取引先へのアクセスをプロビジョニングするためのその他の方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-112">Additional ways in which customer can provision access for transacting partner are described in the following section.</span></span>


## <a name="important-eligibility-and-calculation-requirements"></a><span data-ttu-id="c7bbb-113">重要な資格と計算の要件:</span><span class="sxs-lookup"><span data-stu-id="c7bbb-113">Important eligibility and calculation requirements:</span></span>

- <span data-ttu-id="c7bbb-114">パートナーには、active MPN agreement と有効なルールベースのアカウント制御 (RBAC) の役割があります。これにより、管理対象の azure 資産の獲得クレジットを受け取ることができます。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-114">A partner should have an active MPN agreement and a valid Rules Based Account Control (RBAC) role to receive earned credit for the azure assets they manage.</span></span> <span data-ttu-id="c7bbb-115">[有効な RBAC ロール] の詳細情報</span><span class="sxs-lookup"><span data-stu-id="c7bbb-115">Learn more about [valid RBAC roles]</span></span>

- <span data-ttu-id="c7bbb-116">間接プロバイダーは、お客様または間接リセラーか、またはその両方が、CSP 内の顧客の Azure リソースを24時間365日体制で管理および管理している場合に、PEC の対象となります。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-116">The indirect provider will be eligible for PEC if either they or their indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="c7bbb-117">PEC は、パートナーによって管理される CSP 内の顧客の Azure 資産に対して課金される (請求可能な) 消費量に関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-117">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> 

- <span data-ttu-id="c7bbb-118">PEC は、Microsoft によって請求される CSP のパートナー (間接プロバイダーおよびダイレクト請求パートナー) にのみご利用いただけます。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-118">PEC is available only to partners in CSP who are billed by Microsoft (indirect provider and direct bill partner).</span></span>

- <span data-ttu-id="c7bbb-119">対象サービス: パートナーの獲得クレジットは、価格表に記載されているすべての Azure 1PP Azure の使用量に適用されます。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-119">Eligible Services: Partner earned credit is applicable to all Azure 1PP Azure consumption given on the price list.</span></span> <span data-ttu-id="c7bbb-120">3PP や Azure Reservations に限定されない例外もあります。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-120">There are exceptions including, but not limited to, 3PP and Azure Reservations.</span></span>

- <span data-ttu-id="c7bbb-121">PEC は毎日計算され、毎日偵察ファイルで表示できます。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-121">PEC is calculated daily and can be viewed in the daily recon file.</span></span> <span data-ttu-id="c7bbb-122">パートナー (プロバイダーを通じて) は、PEC を確実に取得するために、一日中 (24 時間365日) のアクセス権を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-122">A partner (provider or reseller (through their provider) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>

- <span data-ttu-id="c7bbb-123">PEC は、Azure リソース レベルで獲得されます。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-123">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="c7bbb-124">パートナーがサブスクリプションまたはリソースグループレベルで有効なアクセス権を持っている場合は、上位のエンティティにロールがある各リソースが PEC を獲得します。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-124">If the partner has valid access at the subscription, or resource group level, each resource that role up to the higher entity will earn PEC.</span></span> 

- <span data-ttu-id="c7bbb-125">PEC は、パートナーの月次請求書に記載されます。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-125">PEC will be included on the partner's monthly invoice.</span></span> <span data-ttu-id="c7bbb-126">請求書の料金は正味です。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-126">The invoice is net of charges.</span></span> <span data-ttu-id="c7bbb-127">詳細は、請求書の偵察ファイルに表示されます。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-127">The details are shown in the invoice recon file.</span></span>

<span data-ttu-id="c7bbb-128">Azure サブスクリプションを管理するためのアクセス権を取得する方法と、MPN ID を RBAC ロールにリンクする方法については、「 [azure プランでのサブスクリプションとリソースの管理」](azure-plan-manage.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7bbb-128">For information on gaining access to manage Azure subscriptions and on how to link your MPN ID to RBAC roles, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="c7bbb-129">詳細情報</span><span class="sxs-lookup"><span data-stu-id="c7bbb-129">For more information</span></span>

- [<span data-ttu-id="c7bbb-130">Azure プラン-課金</span><span class="sxs-lookup"><span data-stu-id="c7bbb-130">Azure plan - billing</span></span>](azure-plan-billing.md)

- [<span data-ttu-id="c7bbb-131">CSP の新しいコマース エクスペリエンスの価格表</span><span class="sxs-lookup"><span data-stu-id="c7bbb-131">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)