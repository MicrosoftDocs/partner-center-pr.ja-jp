---
title: 制限付きの直接請求機能
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP direct 請求パートナーの要件と、制限されている機能を回避するための対処方法について説明します。 機能が制限されているかどうかを確認します。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
keywords: 直接請求、制限
ms.custom: SEOMAY.20
ms.openlocfilehash: a7213708d598e48d1e7e0534908aed99d84b50de
ms.sourcegitcommit: 7abdd277c0eea51237c97cbb163a4943fd740356
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/06/2020
ms.locfileid: "84467232"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a><span data-ttu-id="2e10b-105">制限付きの直接請求機能と、CSP direct bill パートナーに必要な要件</span><span class="sxs-lookup"><span data-stu-id="2e10b-105">Restricted direct bill capabilities and the requirements needed for CSP direct bill partners</span></span>  

## <a name="overview"></a><span data-ttu-id="2e10b-106">概要</span><span class="sxs-lookup"><span data-stu-id="2e10b-106">Overview</span></span>

<span data-ttu-id="2e10b-107">直接請求先のパートナーは、新しい[要件](direct-partner-new-requirements.md)を満たしている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2e10b-107">Direct bill partners must meet the new [requirements](direct-partner-new-requirements.md) to remain in the CSP direct bill partner program.</span></span> <span data-ttu-id="2e10b-108">そうしないと、直接請求機能へのアクセス権が最終的に制限され、特定のタスク (その顧客についての新しい購入の実行など) を実行できなくなります。</span><span class="sxs-lookup"><span data-stu-id="2e10b-108">Otherwise, their access to direct bill capabilities will eventually be restricted and can longer perform specific tasks, such as making new purchases for their customers.</span></span>

> [!Note]
> <span data-ttu-id="2e10b-109">CSP 直接請求パートナープログラムの新しい要件を満たしていない直接請求先のパートナーは、直接請求書の機能が制限されるときに Microsoft によって通知されます。</span><span class="sxs-lookup"><span data-stu-id="2e10b-109">Direct bill partners who do not meet the new requirements for CSP direct bill partner program will be informed by Microsoft when their direct bill capabilities will be restricted.</span></span> <span data-ttu-id="2e10b-110">これは、直接請求[パートナーから間接リセラーへの移行](transition-direct-to-indirect.md)を選択したかどうかに関係なく、すべての直接請求パートナーに適用されます。</span><span class="sxs-lookup"><span data-stu-id="2e10b-110">This applies to all direct bill partners, whether they have opted for [transition from direct bill partner to indirect resellers](transition-direct-to-indirect.md) or not.</span></span>  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a><span data-ttu-id="2e10b-111">直接請求の機能が制限されているかどうかを確認する方法</span><span class="sxs-lookup"><span data-stu-id="2e10b-111">How to tell if your direct bill capabilities has been restricted</span></span>

<span data-ttu-id="2e10b-112">ダイレクト請求パートナーテナントから直接請求機能へのアクセスが制限されているかどうかを確認するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="2e10b-112">To confirm whether access from the direct bill partner tenant to direct bill capabilities has been restricted, follow these steps.</span></span>

1. <span data-ttu-id="2e10b-113">[パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="2e10b-113">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="2e10b-114">**パートナー設定**  ->  **パートナープロファイル**にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="2e10b-114">Go to **Partner settings** -> **Partner Profile**.</span></span>

3. <span data-ttu-id="2e10b-115">[**プログラム情報**] で、 **Microsoft Cloud ソリューションプロバイダーの状態**を探します。</span><span class="sxs-lookup"><span data-stu-id="2e10b-115">Under **Program info**, look for **Microsoft Cloud Solution Provider status**.</span></span>

4. <span data-ttu-id="2e10b-116">プログラムの状態に "値が**制限**されている" ということは、直接請求先のパートナーのテナントによる直接請求の機能へのアクセスが制限されていることを意味します。</span><span class="sxs-lookup"><span data-stu-id="2e10b-116">If the program status has value **restricted**, it means that your direct bill partner tenant's access to direct bill capabilities has been restricted.</span></span>

## <a name="affected-direct-bill-capabilities"></a><span data-ttu-id="2e10b-117">影響を受ける直接請求機能</span><span class="sxs-lookup"><span data-stu-id="2e10b-117">Affected direct bill capabilities</span></span>

<span data-ttu-id="2e10b-118">直接請求書の機能が制限されている場合は、パートナーセンターで顧客の新しい購入を行うことができなくなります。</span><span class="sxs-lookup"><span data-stu-id="2e10b-118">If your direct bill capabilities have been restricted, you can no longer make new purchases for your customers in Partner Center.</span></span> <span data-ttu-id="2e10b-119">この制限は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2e10b-119">This restriction includes:</span></span>

- <span data-ttu-id="2e10b-120">Azure サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="2e10b-120">Azure subscriptions</span></span>

- <span data-ttu-id="2e10b-121">座席ベースのサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="2e10b-121">Seat-based subscriptions</span></span>

- <span data-ttu-id="2e10b-122">既存の座席ベースのサブスクリプションに新しいアドオンを追加します。</span><span class="sxs-lookup"><span data-stu-id="2e10b-122">Add new add-ons to existing seat-based subscriptions.</span></span>

- <span data-ttu-id="2e10b-123">ソフトウェアと予約製品 (ソフトウェアサブスクリプション、永続ソフトウェア、Azure Reserved Virtual Machine instances など) を1回だけ購入してください。</span><span class="sxs-lookup"><span data-stu-id="2e10b-123">Make one-time purchases of software and reservation products (for example, software subscriptions, perpetual software, and Azure Reserved Virtual Machine instances).</span></span>

<span data-ttu-id="2e10b-124">CSP プログラムで[azure パートナー共有サービスプラン](shared-services.md)を使用して、新しい azure サブスクリプションを独自に購入することもできません。</span><span class="sxs-lookup"><span data-stu-id="2e10b-124">You also cannot use the [Azure partner shared services offer](shared-services.md) under the CSP program to purchase new Azure subscriptions for your own use.</span></span>

<span data-ttu-id="2e10b-125">既存の直接請求サブスクリプションは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="2e10b-125">Existing direct bill subscriptions are not affected.</span></span> <span data-ttu-id="2e10b-126">これらは有効なままであり、autorenewed です。</span><span class="sxs-lookup"><span data-stu-id="2e10b-126">They remain valid and are autorenewed.</span></span> <span data-ttu-id="2e10b-127">キャンセルされるまで、Microsoft による直接の課金が継続されます。</span><span class="sxs-lookup"><span data-stu-id="2e10b-127">You will continue to be billed directly by Microsoft until they are canceled.</span></span> <span data-ttu-id="2e10b-128">既存のサブスクリプションは、次の方法で引き続き管理できます。</span><span class="sxs-lookup"><span data-stu-id="2e10b-128">You can still manage existing subscriptions in the following ways:</span></span>

- <span data-ttu-id="2e10b-129">既存のサブスクリプションを中断します</span><span class="sxs-lookup"><span data-stu-id="2e10b-129">Suspend existing subscriptions</span></span>

- <span data-ttu-id="2e10b-130">既存の接続クライアント数に基づくサブスクリプションの接続クライアント数の調整</span><span class="sxs-lookup"><span data-stu-id="2e10b-130">Adjust seat count of existing seat-based subscriptions</span></span>

- <span data-ttu-id="2e10b-131">サブスクリプションに対する既存のアドオンのシート数を調整します。</span><span class="sxs-lookup"><span data-stu-id="2e10b-131">Adjust seat count of existing add-ons to a subscription.</span></span> <span data-ttu-id="2e10b-132">注: 新しいアドオンは新規購入として扱われるため、既存のサブスクリプションに追加することはできません。</span><span class="sxs-lookup"><span data-stu-id="2e10b-132">Note: You cannot add new add-ons to existing subscriptions as it is treated as new purchase.</span></span>

- <span data-ttu-id="2e10b-133">新しい Azure リソースのデプロイと、既存の Azure リソースの管理は、既存の Azure サブスクリプションの下で行います。</span><span class="sxs-lookup"><span data-stu-id="2e10b-133">Deploy new Azure resources and manage existing Azure resources under existing Azure subscriptions.</span></span> <span data-ttu-id="2e10b-134">これには、Azure marketplace と Visual Studio サブスクリプションで利用可能なリソースが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2e10b-134">This includes resources, which are available through Azure marketplace and Visual Studio subscriptions.</span></span>

<span data-ttu-id="2e10b-135">新規購入だけでなく、パートナー センターで次の直接請求機能にアクセスすることもできません。</span><span class="sxs-lookup"><span data-stu-id="2e10b-135">In addition to new purchases, you cannot access the following direct bill capabilities in Partner Center:</span></span>

- <span data-ttu-id="2e10b-136">新しい顧客テナントを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="2e10b-136">You cannot create new customer tenants.</span></span> <span data-ttu-id="2e10b-137">パートナーセンターの [**顧客**] ページにある [**顧客の作成**] オプションは使用できません。</span><span class="sxs-lookup"><span data-stu-id="2e10b-137">The **Create customer** option under **Customers** page in Partner Center will not be available.</span></span>

- <span data-ttu-id="2e10b-138">直接再販業者の関係を要求している顧客への招待を生成することはできません。</span><span class="sxs-lookup"><span data-stu-id="2e10b-138">You cannot generate invitation to customer requesting for direct reseller relationship.</span></span> <span data-ttu-id="2e10b-139">パートナーセンターの [**顧客**] ページにある [**再販業者の関係を要求する**] オプションは使用できません。</span><span class="sxs-lookup"><span data-stu-id="2e10b-139">The **Request a reseller relationship** option under **Customers** page in Partner Center will not be available.</span></span>

    >[!Note]
    ><span data-ttu-id="2e10b-140">直接請求パートナーから間接リセラーへの移行の一環として、直接請求パートナーテナントを間接リセラーとして既に登録している場合は、代わりに間接再販業者の関係を要求する顧客への招待を生成できます。</span><span class="sxs-lookup"><span data-stu-id="2e10b-140">As part of transitioning from direct bill partner to indirect reseller, if you have already enrolled your direct bill partner tenant as indirect reseller, you can generate invitation to customer requesting for indirect reseller relationship instead.</span></span>

- <span data-ttu-id="2e10b-141">新しいサンドボックステナントを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="2e10b-141">You cannot create new sandbox tenant.</span></span> <span data-ttu-id="2e10b-142">各直接請求パートナー テナントでは、直接請求 API の統合のために 1 つのサンドボックス テナントを作成できます。</span><span class="sxs-lookup"><span data-stu-id="2e10b-142">Each direct bill partner tenant can create one sandbox tenant for the purpose of direct bill API integration.</span></span> <span data-ttu-id="2e10b-143">以前に作成したことがない場合は、direct 請求パートナーの機能が制限された後に、この操作を行うことはできません。</span><span class="sxs-lookup"><span data-stu-id="2e10b-143">If you haven't created one previously, you are not allowed to do so after you direct bill partner capability has been restricted.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="2e10b-144">次の手順</span><span class="sxs-lookup"><span data-stu-id="2e10b-144">Next steps</span></span>

- [<span data-ttu-id="2e10b-145">間接リセラーになることについての追加情報</span><span class="sxs-lookup"><span data-stu-id="2e10b-145">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [<span data-ttu-id="2e10b-146">CSP の直接パートナーの新しい要件</span><span class="sxs-lookup"><span data-stu-id="2e10b-146">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)