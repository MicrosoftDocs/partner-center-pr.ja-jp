---
title: 制限付きの直接請求機能
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP の直接請求パートナーの要件と、機能が制限されるのを回避するために行う方法について説明します。 機能が制限されていないか確認します。
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b3b1f3e1593f7e35bd3b9ed6c56ea28683bff95a
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855490"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a><span data-ttu-id="51608-104">CSP 直接請求パートナーに必要な制限付き直接請求機能と要件</span><span class="sxs-lookup"><span data-stu-id="51608-104">Restricted direct bill capabilities and the requirements needed for CSP direct bill partners</span></span>

<span data-ttu-id="51608-105">**適切なロール**: グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="51608-105">**Appropriate roles**: Global admin</span></span>

## <a name="overview"></a><span data-ttu-id="51608-106">概要</span><span class="sxs-lookup"><span data-stu-id="51608-106">Overview</span></span>

<span data-ttu-id="51608-107">直接請求パートナーは、CSP [直接請求パートナー](direct-partner-new-requirements.md) プログラムに残す新しい要件を満たす必要があります。</span><span class="sxs-lookup"><span data-stu-id="51608-107">Direct bill partners must meet the new [requirements](direct-partner-new-requirements.md) to remain in the CSP direct bill partner program.</span></span> <span data-ttu-id="51608-108">そうしないと、直接請求機能へのアクセス権が最終的に制限され、特定のタスク (その顧客についての新しい購入の実行など) を実行できなくなります。</span><span class="sxs-lookup"><span data-stu-id="51608-108">Otherwise, their access to direct bill capabilities will eventually be restricted and can longer perform specific tasks, such as making new purchases for their customers.</span></span>

> [!Note]
> <span data-ttu-id="51608-109">CSP 直接請求パートナー プログラムの新しい要件を満たしていない直接請求パートナーは、直接請求機能が制限される場合に Microsoft から通知されます。</span><span class="sxs-lookup"><span data-stu-id="51608-109">Direct bill partners who do not meet the new requirements for CSP direct bill partner program will be informed by Microsoft when their direct bill capabilities will be restricted.</span></span> <span data-ttu-id="51608-110">これは、直接請求パートナーから間接リセラーへの移行を選択した場合でも、すべての直接請求パートナー [に](transition-direct-to-indirect.md) 適用されます。</span><span class="sxs-lookup"><span data-stu-id="51608-110">This applies to all direct bill partners, whether they have opted for [transition from direct bill partner to indirect resellers](transition-direct-to-indirect.md) or not.</span></span>  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a><span data-ttu-id="51608-111">直接請求機能が制限された場合の確認方法</span><span class="sxs-lookup"><span data-stu-id="51608-111">How to tell if your direct bill capabilities has been restricted</span></span>

<span data-ttu-id="51608-112">直接請求パートナー テナントから直接請求機能へのアクセスが制限されているかどうかを確認するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="51608-112">To confirm whether access from the direct bill partner tenant to direct bill capabilities has been restricted, follow these steps.</span></span>

1. <span data-ttu-id="51608-113">[パートナー センター ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="51608-113">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="51608-114">[アカウント設定 **] [法的プロファイル**  ->  **] に移動します**。</span><span class="sxs-lookup"><span data-stu-id="51608-114">Go to **Account settings** -> **Legal Profile**.</span></span>

3. <span data-ttu-id="51608-115">[ **プログラム情報] で**、状態 **Microsoft クラウド ソリューション プロバイダー探します**。</span><span class="sxs-lookup"><span data-stu-id="51608-115">Under **Program info**, look for **Microsoft Cloud Solution Provider status**.</span></span>

4. <span data-ttu-id="51608-116">プログラムの状態に **値が制限** されている場合は、直接請求パートナー テナントの直接請求機能へのアクセスが制限されています。</span><span class="sxs-lookup"><span data-stu-id="51608-116">If the program status has value **restricted**, it means that your direct bill partner tenant's access to direct bill capabilities has been restricted.</span></span>

## <a name="affected-direct-bill-capabilities"></a><span data-ttu-id="51608-117">影響を受ける直接請求機能</span><span class="sxs-lookup"><span data-stu-id="51608-117">Affected direct bill capabilities</span></span>

<span data-ttu-id="51608-118">直接請求機能が制限されている場合は、顧客に対して新しい購入を行パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="51608-118">If your direct bill capabilities have been restricted, you can no longer make new purchases for your customers in Partner Center.</span></span> <span data-ttu-id="51608-119">この制限には次が含まれます。</span><span class="sxs-lookup"><span data-stu-id="51608-119">This restriction includes:</span></span>

- <span data-ttu-id="51608-120">Azure サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="51608-120">Azure subscriptions</span></span>

- <span data-ttu-id="51608-121">ライセンスベースのサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="51608-121">License-based subscriptions</span></span>

- <span data-ttu-id="51608-122">既存のライセンス ベースのサブスクリプションに新しいアドオンを追加します。</span><span class="sxs-lookup"><span data-stu-id="51608-122">Add new add-ons to existing license-based subscriptions.</span></span>

- <span data-ttu-id="51608-123">ソフトウェアおよび予約製品 (ソフトウェア サブスクリプション、永続的ソフトウェア、Azure 予約仮想マシン インスタンスなど) を 1 回購入します。</span><span class="sxs-lookup"><span data-stu-id="51608-123">Make one-time purchases of software and reservation products (for example, software subscriptions, perpetual software, and Azure Reserved Virtual Machine instances).</span></span>

<span data-ttu-id="51608-124">また、CSP プログラムで [Azure パートナー共有](shared-services.md) サービス オファーを使用して、独自に使用するために新しい Azure サブスクリプションを購入することはできません。</span><span class="sxs-lookup"><span data-stu-id="51608-124">You also cannot use the [Azure partner shared services offer](shared-services.md) under the CSP program to purchase new Azure subscriptions for your own use.</span></span>

<span data-ttu-id="51608-125">既存の直接請求サブスクリプションは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="51608-125">Existing direct bill subscriptions are not affected.</span></span> <span data-ttu-id="51608-126">それらは有効なまま残り、自動的に更新されます。</span><span class="sxs-lookup"><span data-stu-id="51608-126">They remain valid and are auto-renewed.</span></span> <span data-ttu-id="51608-127">取り消されるまで、引き続き Microsoft から直接請求されます。</span><span class="sxs-lookup"><span data-stu-id="51608-127">You will continue to be billed directly by Microsoft until they are canceled.</span></span> <span data-ttu-id="51608-128">既存のサブスクリプションは、引き続き次の方法で管理できます。</span><span class="sxs-lookup"><span data-stu-id="51608-128">You can still manage existing subscriptions in the following ways:</span></span>

- <span data-ttu-id="51608-129">既存のサブスクリプションを中断します</span><span class="sxs-lookup"><span data-stu-id="51608-129">Suspend existing subscriptions</span></span>

- <span data-ttu-id="51608-130">既存のライセンス ベースのサブスクリプションのライセンス数を調整する</span><span class="sxs-lookup"><span data-stu-id="51608-130">Adjust license count of existing license-based subscriptions</span></span>

- <span data-ttu-id="51608-131">サブスクリプションに対する既存のアドオンのライセンス数を調整します。</span><span class="sxs-lookup"><span data-stu-id="51608-131">Adjust license count of existing add-ons to a subscription.</span></span> 

    >[!Note]
    ><span data-ttu-id="51608-132">新しいアドオンは新規購入として扱われるため、既存のサブスクリプションに追加することはできません。</span><span class="sxs-lookup"><span data-stu-id="51608-132">You cannot add new add-ons to existing subscriptions as it is treated as new purchase.</span></span>

- <span data-ttu-id="51608-133">新しい Azure リソースのデプロイと、既存の Azure リソースの管理は、既存の Azure サブスクリプションの下で行います。</span><span class="sxs-lookup"><span data-stu-id="51608-133">Deploy new Azure resources and manage existing Azure resources under existing Azure subscriptions.</span></span> <span data-ttu-id="51608-134">これには、Azure Marketplace と Visual Studio サブスクリプションで利用可能なリソースが含まれます。</span><span class="sxs-lookup"><span data-stu-id="51608-134">This includes resources, which are available through Azure Marketplace and Visual Studio subscriptions.</span></span>

<span data-ttu-id="51608-135">新規購入だけでなく、パートナー センターで次の直接請求機能にアクセスすることもできません。</span><span class="sxs-lookup"><span data-stu-id="51608-135">In addition to new purchases, you cannot access the following direct bill capabilities in Partner Center:</span></span>

- <span data-ttu-id="51608-136">新しい顧客テナントを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="51608-136">You cannot create new customer tenants.</span></span> <span data-ttu-id="51608-137">パートナーセンターの [**顧客**] ページにある [**顧客の作成**] オプションは使用できません。</span><span class="sxs-lookup"><span data-stu-id="51608-137">The **Create customer** option under **Customers** page in Partner Center will not be available.</span></span>

- <span data-ttu-id="51608-138">直接再販業者の関係を要求している顧客への招待を生成することはできません。</span><span class="sxs-lookup"><span data-stu-id="51608-138">You cannot generate invitation to customer requesting for direct reseller relationship.</span></span> <span data-ttu-id="51608-139">パートナーセンターの [**顧客**] ページにある [**再販業者の関係を要求する**] オプションは使用できません。</span><span class="sxs-lookup"><span data-stu-id="51608-139">The **Request a reseller relationship** option under **Customers** page in Partner Center will not be available.</span></span>

    >[!NOTE]
    ><span data-ttu-id="51608-140">直接請求パートナーから間接リセラーへの移行の一環として、直接請求パートナーテナントを間接リセラーとして既に登録している場合は、代わりに間接再販業者の関係を要求する顧客への招待を生成できます。</span><span class="sxs-lookup"><span data-stu-id="51608-140">As part of transitioning from direct bill partner to indirect reseller, if you have already enrolled your direct bill partner tenant as indirect reseller, you can generate invitation to customer requesting for indirect reseller relationship instead.</span></span>

- <span data-ttu-id="51608-141">新しいサンドボックステナントを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="51608-141">You cannot create new sandbox tenant.</span></span> <span data-ttu-id="51608-142">各ダイレクト請求パートナーテナントは、直接請求 API 統合用に1つのサンドボックステナントを作成できます。</span><span class="sxs-lookup"><span data-stu-id="51608-142">Each direct bill partner tenant can create one sandbox tenant for direct bill API integration.</span></span> <span data-ttu-id="51608-143">以前に作成したことがない場合は、直接請求先パートナーの機能が制限された後でその操作を行うことはできません。</span><span class="sxs-lookup"><span data-stu-id="51608-143">If you haven't created one previously, you are not allowed to do so after your direct bill partner capability has been restricted.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="51608-144">次の手順</span><span class="sxs-lookup"><span data-stu-id="51608-144">Next steps</span></span>

- [<span data-ttu-id="51608-145">間接リセラーになることについての追加情報</span><span class="sxs-lookup"><span data-stu-id="51608-145">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [<span data-ttu-id="51608-146">CSP の直接パートナーの新しい要件</span><span class="sxs-lookup"><span data-stu-id="51608-146">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
