---
title: パートナーの獲得クレジットの計算方法 |パートナーセンター
ms.topic: article
ms.date: 09/17/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure プランのパートナー獲得クレジットの比率を計算する方法
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 402ee0e2084191c7d4f592dd91480be8e1bd0341
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653717"
---
# <a name="how-the-partner-earned-credit-pec-is-calculated"></a><span data-ttu-id="5698e-103">パートナーの獲得クレジット (PEC) の計算方法</span><span class="sxs-lookup"><span data-stu-id="5698e-103">How the partner earned credit (PEC) is calculated</span></span>


<span data-ttu-id="5698e-104">Microsoft 365 年中無休の IT 運用管理、または CSP における顧客の Azure 環境全体を所有するパートナーは、PEC を利用できます。</span><span class="sxs-lookup"><span data-stu-id="5698e-104">Partners who own the 24x7 IT operations management of parts or the entire Azure environment of their customers in CSP are rewarded with PEC.</span></span> <span data-ttu-id="5698e-105">PEC は、Microsoft との直接の課金関係を持つパートナーに請求書の一部として提供されます。</span><span class="sxs-lookup"><span data-stu-id="5698e-105">The PEC is provided as part of the invoice to the partner who has a direct billing relationship with Microsoft.</span></span> <span data-ttu-id="5698e-106">クレジットは日単位で計算され、月次請求書に反映されます。</span><span class="sxs-lookup"><span data-stu-id="5698e-106">The credit is calculated daily and reflected in the monthly invoice.</span></span> <span data-ttu-id="5698e-107">CSP の既定では、顧客のサブスクリプションに対する必要なアクセス権がパートナーに付与されます。これにより、サブスクリプションのリソースを24時間365日体制で管理し、制御することができます。</span><span class="sxs-lookup"><span data-stu-id="5698e-107">By default, in CSP, partners are granted the necessary access rights to the customer's subscription that allows them to have 24X7 operations management and control of the resources on the subscription.</span></span> <span data-ttu-id="5698e-108">次のセクションでは、お客様が取引先へのアクセスをプロビジョニングするためのその他の方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="5698e-108">Additional ways in which customer can provision access for transacting partner are described in the following section.</span></span>   


## <a name="important-eligibility-and-calculation-requirements"></a><span data-ttu-id="5698e-109">重要な資格と計算の要件:</span><span class="sxs-lookup"><span data-stu-id="5698e-109">Important eligibility and calculation requirements:</span></span>

- <span data-ttu-id="5698e-110">パートナーは、管理対象の azure 資産の獲得クレジットを受け取るために、active MPN agreement と有効なルールベースのアカウント C (RBAC) の役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5698e-110">A partner should have an active MPN agreement and a valid Rules Based Account C (RBAC) role to receive earned credit for the azure assets they manage.</span></span> <span data-ttu-id="5698e-111">[有効な RBAC ロール] の詳細情報</span><span class="sxs-lookup"><span data-stu-id="5698e-111">Learn more about [valid RBAC roles]</span></span>

- <span data-ttu-id="5698e-112">間接プロバイダーは、お客様または間接リセラーか、またはその両方が、CSP 内の顧客の Azure リソースを24時間365日体制で管理および管理している場合に、PEC の対象となります。</span><span class="sxs-lookup"><span data-stu-id="5698e-112">The indirect provider will be eligible for PEC if either they or their indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="5698e-113">PEC は、パートナーによって管理される CSP におけるお客様の Azure 資産の請求 (課金) に関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="5698e-113">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> 

- <span data-ttu-id="5698e-114">PEC は、Microsoft によって請求される CSP のパートナー (間接プロバイダーおよびダイレクト請求パートナー) にのみご利用いただけます。</span><span class="sxs-lookup"><span data-stu-id="5698e-114">PEC is available only to partners in CSP who are billed by Microsoft (indirect provider and direct bill partner).</span></span>

- <span data-ttu-id="5698e-115">対象サービス: パートナーの獲得クレジットは、価格表に記載されているすべての Azure 1PP Azure の使用量に適用されます。</span><span class="sxs-lookup"><span data-stu-id="5698e-115">Eligible Services: Partner earned credit is applicable to all Azure 1PP Azure consumption given on the price list.</span></span> <span data-ttu-id="5698e-116">3PP や Azure Reservations に限定されない例外もあります。</span><span class="sxs-lookup"><span data-stu-id="5698e-116">There are exceptions including, but not limited to, 3PP and Azure Reservations.</span></span>

- <span data-ttu-id="5698e-117">PEC は毎日計算され、毎日偵察ファイルで表示できます。</span><span class="sxs-lookup"><span data-stu-id="5698e-117">PEC is calculated daily and can be viewed in the daily recon file.</span></span> <span data-ttu-id="5698e-118">パートナー (プロバイダーを通じて) は、PEC を確実に取得するために、一日中 (24 時間365日) のアクセス権を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5698e-118">A partner (provider or reseller (through their provider) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>

- <span data-ttu-id="5698e-119">Azure リソースレベルまで、PEC が獲得されます。</span><span class="sxs-lookup"><span data-stu-id="5698e-119">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="5698e-120">パートナーがサブスクリプションまたはリソースグループレベルで有効なアクセス権を持っている場合は、上位のエンティティにロールがある各リソースが PEC を獲得します。</span><span class="sxs-lookup"><span data-stu-id="5698e-120">If the partner has valid access at the subscription, or resource group level, each resource that role up to the higher entity will earn PEC.</span></span> 

- <span data-ttu-id="5698e-121">PEC は、パートナーの月次請求書に記載されます。</span><span class="sxs-lookup"><span data-stu-id="5698e-121">PEC will be included on the partner's monthly invoice.</span></span> <span data-ttu-id="5698e-122">請求書の料金は正味です。</span><span class="sxs-lookup"><span data-stu-id="5698e-122">The invoice is net of charges.</span></span> <span data-ttu-id="5698e-123">詳細は、請求書の偵察ファイルに表示されます。</span><span class="sxs-lookup"><span data-stu-id="5698e-123">The details are shown in the invoice recon file.</span></span>

<span data-ttu-id="5698e-124">Azure サブスクリプションを管理するためのアクセス権を取得する方法と、MPN ID を RBAC ロールにリンクする方法については、「 [azure プランでのサブスクリプションとリソースの管理」](azure-plan-manage.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5698e-124">For information on gaining access to manage Azure subscriptions and on how to link your MPN ID to RBAC roles, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="5698e-125">詳細情報</span><span class="sxs-lookup"><span data-stu-id="5698e-125">For more information</span></span>

- [<span data-ttu-id="5698e-126">Azure プラン-課金</span><span class="sxs-lookup"><span data-stu-id="5698e-126">Azure plan - billing</span></span>](azure-plan-billing.md)

- [<span data-ttu-id="5698e-127">CSP の新しいコマース エクスペリエンスの価格表</span><span class="sxs-lookup"><span data-stu-id="5698e-127">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)