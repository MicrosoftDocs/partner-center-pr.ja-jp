---
title: Azure Partner Shared Services の追加
description: Azure Partner Shared Services を使用して、自分で使用する Azure サブスクリプションを購入し、Azure の購入、追跡、および管理のための統一された方法を利用できます。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 40ba485cecce394dc81632d01f8774859690c522
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551607"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a><span data-ttu-id="47cb1-103">パートナーが自分で使用するために Azure サブスクリプションを購入できるように Azure パートナー共有サービスを追加する</span><span class="sxs-lookup"><span data-stu-id="47cb1-103">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>

<span data-ttu-id="47cb1-104">**適切なロール**: 全体管理者 |管理エージェント |営業担当者</span><span class="sxs-lookup"><span data-stu-id="47cb1-104">**Appropriate roles**: Global admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="47cb1-105">Azure Partner Shared Services (APSS) は、クラウドソリューションプロバイダー (CSP) プログラムのパートナー向けの新しいオファーの種類であり、パートナーが自分で使用する Azure サブスクリプションを購入できるようにします。</span><span class="sxs-lookup"><span data-stu-id="47cb1-105">Azure Partner Shared Services (APSS) is a new offer type for partners in the Cloud Solution Provider (CSP) program, enabling partners to purchase Azure subscriptions for their own use.</span></span><span data-ttu-id="47cb1-106">パートナーにとっては、Microsoft との Azure ライセンス契約および再販契約を集約できるだけでなく、統一された方法で Azure を購入、追跡、管理できるようになります。</span><span class="sxs-lookup"><span data-stu-id="47cb1-106">  It creates the opportunity for partners to use a uniform method for purchasing, tracking, and managing Azure in addition to the ability to consolidate their Azure licensing and reselling agreements with Microsoft.</span></span> <span data-ttu-id="47cb1-107">APSS を使用すると、パートナーは、Microsoft Enterprise Agreement および Web ダイレクトプログラムの場合と同じように、CSP で Azure サブスクリプションを使用する場合と同じ柔軟性を持つようになりました。たとえば、開発とテスト環境の構築、内部ワークロードのデプロイ、共有サービスやマルチテナントアプリケーションのホストなどのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="47cb1-107">With APSS, partners now have the same flexibility to use Azure subscriptions in CSP as they do in the Microsoft Enterprise Agreement and Web Direct programs, opening up scenarios such as:  build development and test environments, deploy internal workloads, and host shared services or multi-tenant applications.</span></span>  

## <a name="create-the-shared-services-tenant"></a><span data-ttu-id="47cb1-108">共有サービス テナントを作成する</span><span class="sxs-lookup"><span data-stu-id="47cb1-108">Create the shared services tenant</span></span>

1. <span data-ttu-id="47cb1-109">[**設定**] [  >  **アカウント設定**] [  >  **共有サービス**] にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="47cb1-109">Go to **Settings** > **Account settings** > **Shared services**.</span></span>

   :::image type="content" source="images/sharedservices2.png" alt-text="共有サービスのアカウント設定 >":::

2. <span data-ttu-id="47cb1-111">共有サービステナントをまだ持っていない場合は、[ **共有サービスの作成**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="47cb1-111">If you don't already have a shared services tenant, select **Create shared services**.</span></span>

   :::image type="content" source="images/sharedservices3.png" alt-text="共有サービスを作成します。":::

3. <span data-ttu-id="47cb1-113">これにより、共有サービス テナントが作成され、共有リソースや内部ワークロードで使用する Azure CSP Shared Services サブスクリプションの購入が行われます。</span><span class="sxs-lookup"><span data-stu-id="47cb1-113">This creates a shared services tenant and purchases the Azure CSP Shared Services subscription, to be used for shared resources and internal workload.</span></span>

   :::image type="content" source="images/sharedservices5.png" alt-text="テナントを作成し、サブスクリプションを購入します。":::

## <a name="about-the-azure--internalshared-services-offer"></a><span data-ttu-id="47cb1-115">Azure - Internal/Shared Services プランについて</span><span class="sxs-lookup"><span data-stu-id="47cb1-115">About the Azure- Internal/Shared Services offer</span></span>

- <span data-ttu-id="47cb1-116">Azure-Internal/Shared Services サブスクリプションは、パートナーセンターを通じてアクセスされる CSP の新しい Azure プランの種類であり、パートナーは Azure を独自に使用することができます。</span><span class="sxs-lookup"><span data-stu-id="47cb1-116">The Azure - Internal/Shared Services subscription is a new Azure offer type in CSP accessed through Partner Center that partners get for their own use of Azure.</span></span>

- <span data-ttu-id="47cb1-117">Azure Partner Shared Services サブスクリプションは対象となり、RIs の購入に使用できます。</span><span class="sxs-lookup"><span data-stu-id="47cb1-117">Azure Partner Shared Services subscriptions are eligible and can be used to purchase RIs.</span></span>

- <span data-ttu-id="47cb1-118">Azure - Internal/Shared Services プランは、共有サービス テナントにのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="47cb1-118">The Azure - Internal/Shared Services offer can only be applied to the shared services tenant.</span></span>

- <span data-ttu-id="47cb1-119">Azure-Internal/Shared Services サブスクリプションの主な用途は、独自の開発目的で Azure を使用できるようにすることです。</span><span class="sxs-lookup"><span data-stu-id="47cb1-119">The primary use for the Azure - Internal/Shared Services subscription is so that you can use Azure for your own development purposes.</span></span> <span data-ttu-id="47cb1-120">このプランのプロビジョニングに使用する共有テナントは、Office 365 や Dynamics のライセンスなどの他のサービスには使用できません。</span><span class="sxs-lookup"><span data-stu-id="47cb1-120">The shared tenant you use to provision this offer cannot be used for other services such as Office 365 or Dynamics licenses.</span></span>

- <span data-ttu-id="47cb1-121">サブスクリプションのキャンセルは、他のサブスクリプションと同様の方法で行うことができます。</span><span class="sxs-lookup"><span data-stu-id="47cb1-121">You can cancel the subscription like any other subscription.</span></span> <span data-ttu-id="47cb1-122">[**設定**] ビューの [すべての設定] [  >    >  **共有サービス**] にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="47cb1-122">Go to the **settings** > **View all settings** > **Shared services**.</span></span> <span data-ttu-id="47cb1-123">Azure - Internal/Shared Services を選択して取り消します。</span><span class="sxs-lookup"><span data-stu-id="47cb1-123">Select the Azure - Internal/Shared Services subscription and cancel it.</span></span>

## <a name="accessing-azure-partner-shared-services-consumption-details"></a><span data-ttu-id="47cb1-124">Azure Partner Shared Services の利用状況の詳細にアクセスする</span><span class="sxs-lookup"><span data-stu-id="47cb1-124">Accessing Azure Partner Shared Services consumption details</span></span>

<span data-ttu-id="47cb1-125">Azure の利用状況は、CSP 請求書と調整ファイルに記載されます。</span><span class="sxs-lookup"><span data-stu-id="47cb1-125">You will find the Azure consumption on your CSP invoice and the reconciliation file.</span></span> <span data-ttu-id="47cb1-126">請求書では、Microsoft Azure の明細項目の一部として含まれます。</span><span class="sxs-lookup"><span data-stu-id="47cb1-126">It will be included as part of Microsoft Azure line item in the invoice.</span></span> <span data-ttu-id="47cb1-127">利用状況の詳細は、このプラン用に作成されたテナントに対して記録された調整ファイルで参照できます。</span><span class="sxs-lookup"><span data-stu-id="47cb1-127">The detailed consumption information will be available in the reconciliation file logged against the tenant that was created for this offer.</span></span>

## <a name="azure-partner-shared-services-pricing"></a><span data-ttu-id="47cb1-128">Azure Partner Shared Services の価格</span><span class="sxs-lookup"><span data-stu-id="47cb1-128">Azure Partner Shared Services pricing</span></span>

<span data-ttu-id="47cb1-129">APSS の新しい価格ファイルを確認するには、**販売**  >  **価格とプラン** に関するページにアクセスし、当月の価格表を選択してください。</span><span class="sxs-lookup"><span data-stu-id="47cb1-129">To see the new pricing file for APSS, go to **Sell** > **Pricing and offers** and select the current month's price list.</span></span> <span data-ttu-id="47cb1-130">今後数週間のうちには、特定の価格カードの API もリリースされる予定です。</span><span class="sxs-lookup"><span data-stu-id="47cb1-130">In the coming weeks, a specific rate card api will also be released.</span></span>

## <a name="marketplace-offers-and-azure-partner-shared-services"></a><span data-ttu-id="47cb1-131">マーケットプレースのプランと Azure Partner Shared Services</span><span class="sxs-lookup"><span data-stu-id="47cb1-131">Marketplace offers and Azure Partner Shared Services</span></span>

<span data-ttu-id="47cb1-132">2019年3月1日の時点で、APSS は Marketplace プランをサポートしなくなりました。</span><span class="sxs-lookup"><span data-stu-id="47cb1-132">As of March 1, 2019, APSS no longer supports Marketplace offers.</span></span>

|<span data-ttu-id="47cb1-133">**マーケットプレースのサポート**</span><span class="sxs-lookup"><span data-stu-id="47cb1-133">**Marketplace support**</span></span>   |<span data-ttu-id="47cb1-134">**2019 年 3 月 1 日より前にサポートされる APSS**</span><span class="sxs-lookup"><span data-stu-id="47cb1-134">**APSS supported before March 1, 2019**</span></span>|<span data-ttu-id="47cb1-135">**2019 年 3 月 1 日以降**</span><span class="sxs-lookup"><span data-stu-id="47cb1-135">**After March 1, 2019**</span></span>|
|---------------------------|:----------------------------|:-------------------|
|<span data-ttu-id="47cb1-136">ライセンス持ち込み (BYOL) と無料サービス</span><span class="sxs-lookup"><span data-stu-id="47cb1-136">Bring your own license (BYOL) and free services</span></span>   | <span data-ttu-id="47cb1-137">はい</span><span class="sxs-lookup"><span data-stu-id="47cb1-137">Yes</span></span>   | <span data-ttu-id="47cb1-138">いいえ</span><span class="sxs-lookup"><span data-stu-id="47cb1-138">No</span></span>|
|<span data-ttu-id="47cb1-139">その他のサードパーティのマーケットプレースのプラン</span><span class="sxs-lookup"><span data-stu-id="47cb1-139">Other third-party marketplace offers</span></span>   | <span data-ttu-id="47cb1-140">いいえ</span><span class="sxs-lookup"><span data-stu-id="47cb1-140">No</span></span>   |<span data-ttu-id="47cb1-141">いいえ</span><span class="sxs-lookup"><span data-stu-id="47cb1-141">No</span></span>|

<span data-ttu-id="47cb1-142">APSS を使用してデプロイされた BYOL または無料のサービスを利用しているパートナーは影響を受けません。ただし、2019年3月1日以降、新しい BYOL または無料サービスを購入することはできません。</span><span class="sxs-lookup"><span data-stu-id="47cb1-142">Partners who have BYOL or free services deployed using APSS will not be impacted; however after March 1, 2019 they will not be able to purchase new BYOL or free services.</span></span>

<span data-ttu-id="47cb1-143">(BYOL と無料サービスだけでなく) 利用可能な Marketplace プランの完全なカタログを利用するには、CSP パートナーが web ダイレクト Azure サブスクリプションを使用して共有サービスをデプロイすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="47cb1-143">To take advantage of the full catalog of Marketplace offers available (not just BYOL and free services), we recommend CSP partners deploy shared services using web direct Azure subscriptions.</span></span>  <span data-ttu-id="47cb1-144">以前にサードパーティの BYOL と無料のサービスリソースをデプロイしたことがあり、それを引き続き使用してサードパーティ製品をデプロイする場合は、 [既存の Azure サブスクリプション](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)の Web direct 移行に APSS サブスクリプションを移行することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="47cb1-144">CSP partners who have deployed third-party BYOL and free service resources from the Marketplace previously and wish to continue using them and deploy more third-party offerings are encouraged to migrate the APSS subscription to web direct [Migrating Existing Azure Subscriptions](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span></span>

<span data-ttu-id="47cb1-145">2019年3月1日より後に APSS サブスクリプションの使用を予定しており、新しいサードパーティの [Byol サービス](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) または無料サービスをデプロイすることを計画しているパートナーは、isv の指示に従ってこれらを APSS サブスクリプションにデプロイできます。</span><span class="sxs-lookup"><span data-stu-id="47cb1-145">Partners, who plan to continue using APSS subscription after the March 1, 2019 and wish to deploy new third-party [BYOL services](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) or free services, can follow the instructions from ISVs to deploy these to their APSS subscriptions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="47cb1-146">次の手順</span><span class="sxs-lookup"><span data-stu-id="47cb1-146">Next steps</span></span>

- [<span data-ttu-id="47cb1-147">CSP によるソフトウェア サブスクリプションの販売</span><span class="sxs-lookup"><span data-stu-id="47cb1-147">Sell software subscriptions through CSP</span></span>](csp-software-subscriptions.md)