---
title: 顧客を現在の Azure プランから Azure プランに移行する
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP パートナーが、パートナー センターを使用して顧客を既存の CSP Azure プランから、Azure プランで管理される Azure サービスに移行する方法について説明します。
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: bcc6534995a7550f0f09d1da2d52cbf676b66c40
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527508"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a><span data-ttu-id="c080a-103">顧客を既存の CSP Azure プランから Azure プランに移行する</span><span class="sxs-lookup"><span data-stu-id="c080a-103">Transition customers to Azure plan from existing CSP Azure offers</span></span>

<span data-ttu-id="c080a-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="c080a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c080a-105">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="c080a-105">Admin agent</span></span>
- <span data-ttu-id="c080a-106">課金管理者</span><span class="sxs-lookup"><span data-stu-id="c080a-106">Billing admin</span></span>
- <span data-ttu-id="c080a-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="c080a-107">Global admin</span></span>
- <span data-ttu-id="c080a-108">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="c080a-108">Helpdesk agent</span></span>
- <span data-ttu-id="c080a-109">販売代理店</span><span class="sxs-lookup"><span data-stu-id="c080a-109">Sales agent</span></span>
- <span data-ttu-id="c080a-110">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="c080a-110">User management admin</span></span>

<span data-ttu-id="c080a-111">間接プロバイダーおよび直接請求パートナーは、Azure 向け Microsoft クラウド サービス プロバイダー (CSP) プログラムで利用可能な新しいコマース エクスペリエンスに移行できます。</span><span class="sxs-lookup"><span data-stu-id="c080a-111">Indirect providers and direct bill partners can transition to the new commerce experience available in the Microsoft Cloud Service Provider Program (CSP) for Azure.</span></span> <span data-ttu-id="c080a-112">(間接リセラーは、間接プロバイダーを通じて行う必要があります)。パートナーからの購入、マイクロソフト販売者からの購入、または Web 上での直接購入にかかわらず、クラウド サービスを簡単に購入するための最新の方法が顧客に提供されます。</span><span class="sxs-lookup"><span data-stu-id="c080a-112">(Indirect resellers will need to work through their indirect providers.) Customers will have a streamlined way to buy cloud services, whether purchasing from partners, from Microsoft sellers, or directly on the web.</span></span>

<span data-ttu-id="c080a-113">移行機能は、新しい Azure 向けコマース エクスペリエンスに移行する顧客で、Microsoft 顧客契約に署名している顧客のみを対象としています。Office 365 や Dynamics 365 などの CSP の他のプランは対象外です。</span><span class="sxs-lookup"><span data-stu-id="c080a-113">The transition capability is only for customers transitioning to the new commerce experience for Azure and who have signed the Microsoft Customer Agreement and not for other offers in CSP such as Office 365 or Dynamics 365.</span></span>

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a><span data-ttu-id="c080a-114">既存の CSP プランの Azure プランへの移行</span><span class="sxs-lookup"><span data-stu-id="c080a-114">Transition existing CSP offers to an Azure plan</span></span>

<span data-ttu-id="c080a-115">パートナー センターで、既存の CSP Azure プランから CSP プログラムの新しいコマース エクスペリエンスである Azure プランで管理される Azure サービスに顧客を移行させることができます。</span><span class="sxs-lookup"><span data-stu-id="c080a-115">You can transition a customer from their existing CSP Azure offers to Azure services under the Azure plan in the new commerce experience in the CSP program from within Partner Center.</span></span> <span data-ttu-id="c080a-116">これを行うには、パートナーと顧客の間にパートナー センターを通じて再販業者関係が確立されている必要があり、顧客が Microsoft 顧客契約に署名している必要があります。</span><span class="sxs-lookup"><span data-stu-id="c080a-116">To do this, the partner and customer must have an established reseller relationship through Partner Center, and the customer must have signed the Microsoft Customer Agreement.</span></span>

### <a name="select-transition-to-azure-plan"></a><span data-ttu-id="c080a-117">Azure プランへの移行を選択する</span><span class="sxs-lookup"><span data-stu-id="c080a-117">Select transition to Azure plan</span></span>

1. <span data-ttu-id="c080a-118">顧客向けの Azure プランを選択します。</span><span class="sxs-lookup"><span data-stu-id="c080a-118">Select Azure plan for your customer.</span></span>

2. <span data-ttu-id="c080a-119">**[請求を Azure プランに移行する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c080a-119">Select **Transition billing to Azure plan**.</span></span>

   :::image type="content" source="images/azure/transition1.png" alt-text="使用状況に基づいたサブスクリプションのレポート情報を示すスクリーンショット。選択可能な次のオプションが表示されています:[Azure サブスクリプション請求を Azure プランに移行する]。":::

3. <span data-ttu-id="c080a-121">**[続行]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c080a-121">Select **Continue**</span></span>

   :::image type="content" source="images/azure/transition2.png" alt-text="[Transition to Azure plan]\(Azure プランへの移行\) というタイトルのダイアログ ボックス。移行についての説明と、[続行] および [キャンセル] という選択可能な 2 つのオプションが表示されています。":::

   <span data-ttu-id="c080a-123">顧客は、Azure プランに移行されます。</span><span class="sxs-lookup"><span data-stu-id="c080a-123">Your customer will be transitioned to the Azure plan.</span></span>

   <span data-ttu-id="c080a-124">**移行ワークフローによって、前提条件となる手順が自動化されます**。</span><span class="sxs-lookup"><span data-stu-id="c080a-124">**The transition workflow automates the pre-requisite steps**:</span></span>

   - <span data-ttu-id="c080a-125">Azure プランの購入</span><span class="sxs-lookup"><span data-stu-id="c080a-125">Purchase of Azure plan(s)</span></span>
   - <span data-ttu-id="c080a-126">ダイレクト CSP での顧客ごとに 1 つのプラン シナリオ</span><span class="sxs-lookup"><span data-stu-id="c080a-126">One plan per customer in Direct CSP scenarios</span></span>  
   - <span data-ttu-id="c080a-127">リセラーごとに 1 つのプラン</span><span class="sxs-lookup"><span data-stu-id="c080a-127">One plan per reseller</span></span>  

   <span data-ttu-id="c080a-128">例として、パートナーが 2 つの Microsoft Azure プランを購入し、その購入の中に 2 つの異なる POR が含まれているとします。</span><span class="sxs-lookup"><span data-stu-id="c080a-128">For an example, a partner has purchased two Microsoft Azure offers and has    included two distinct POR in the purchase.</span></span> <span data-ttu-id="c080a-129">この場合、移行ワークフローでは、2 つの Azure プラン (リセラーごとに 1 つ) が購入され、各 Azure サブスクリプションが Azure プランに自動的にマップされます。</span><span class="sxs-lookup"><span data-stu-id="c080a-129">In this case, the transition    workflow will purchase two Azure plans (one per reseller) and map the    respective Azure subscriptions under the Azure plans automatically.</span></span>  

   <span data-ttu-id="c080a-130">**Azure サブスクリプションの Azure プランへのマッピング**</span><span class="sxs-lookup"><span data-stu-id="c080a-130">**Mapping Azure subscription to Azure plan**</span></span>

   <span data-ttu-id="c080a-131">Azure プランを購入すると、システムによって既存の Azure サブスクリプションが Azure プランにマップされます。</span><span class="sxs-lookup"><span data-stu-id="c080a-131">After your purchase of Azure plan(s), our system will map the existing Azure    subscriptions to the Azure plans.</span></span> <span data-ttu-id="c080a-132">進行状況は、パートナー センターだけでなく Azure portal でも確認できます。</span><span class="sxs-lookup"><span data-stu-id="c080a-132">The progress can be viewed in Azure portal as    well as in Partner center.</span></span>

4. <span data-ttu-id="c080a-133">顧客のパートナー センターの **[サブスクリプション]** ページに戻り、顧客の現地通貨を使用して予算制限を更新します。</span><span class="sxs-lookup"><span data-stu-id="c080a-133">Return to your customer's Partner Center **Subscriptions** page to update their budget limit using their local currency.</span></span>

   :::image type="content" source="images/azure/transition3.png" alt-text="パートナー センターの [サブスクリプション] ページの一部分。請求期間の予算制限が現地の通貨で設定されています。":::

   >[!NOTE]
   ><span data-ttu-id="c080a-135">パートナー センターで設定した予算は、Azure portal には引き継がれません。</span><span class="sxs-lookup"><span data-stu-id="c080a-135">The budget you set in Partner Center doesn't carry over to the Azure portal.</span></span> <span data-ttu-id="c080a-136">Azure portal で、予算とアラートも設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c080a-136">You should also set the budget and alert in Azure portal.</span></span>

   <span data-ttu-id="c080a-137">Azure プランに移行すると、この顧客用の Azure サブスクリプションを購入することはできなくなります。</span><span class="sxs-lookup"><span data-stu-id="c080a-137">When you move to the Azure plan, you can no longer purchase Azure subscriptions for this customer.</span></span> <span data-ttu-id="c080a-138">サブスクリプションは、Azure portal で Azure プランの中に作成します。</span><span class="sxs-lookup"><span data-stu-id="c080a-138">You create the subscriptions under the Azure plan in the Azure portal.</span></span>

   >[!NOTE]
   > <span data-ttu-id="c080a-139">Azure プランで RBAC を通して購入されたすべての Azure サブスクリプションに対し、現地通貨で請求および課金されます。</span><span class="sxs-lookup"><span data-stu-id="c080a-139">All Azure subscriptions purchased through RBAC under the Azure plan will be    priced and billed in local currency.</span></span> <span data-ttu-id="c080a-140">為替レートは使用されません。</span><span class="sxs-lookup"><span data-stu-id="c080a-140">FX rates will not be used.</span></span>

### <a name="track-your-transition-details"></a><span data-ttu-id="c080a-141">移行の詳細を追跡する</span><span class="sxs-lookup"><span data-stu-id="c080a-141">Track your transition details</span></span>

<span data-ttu-id="c080a-142">パートナー センターだけでなく、Azure portal でも移行の進行状況を確認してください。</span><span class="sxs-lookup"><span data-stu-id="c080a-142">Follow the transition progress in Azure portal as well as in Partner Center.</span></span>

:::image type="content" source="images/azure/details1.png" alt-text="サブスクリプションごとに移行の詳細リストが表示されている表のスクリーンショット。サブスクリプション ID、移行日、移行の状態が含まれています。":::

### <a name="billing-impact-to-partners"></a><span data-ttu-id="c080a-144">パートナーに対する請求の影響</span><span class="sxs-lookup"><span data-stu-id="c080a-144">Billing impact to partners</span></span>

<span data-ttu-id="c080a-145">既存の CSP Azure プランから顧客を移行する場合、次のような請求の影響が発生します。</span><span class="sxs-lookup"><span data-stu-id="c080a-145">If you transition a customer from an existing CSP Azure offer, you will have the following billing impacts:</span></span>

- <span data-ttu-id="c080a-146">元の CSP Azure サブスクリプションの終了時点までのすべての使用量については、既存の CSP 請求書で請求されます。</span><span class="sxs-lookup"><span data-stu-id="c080a-146">You will be billed on your existing CSP invoice for all usage up to the point of exiting the original CSP Azure subscription.</span></span>

- <span data-ttu-id="c080a-147">既存の CSP サブスクリプションに対する管理者アクセス権を持っている場合は、そのサブスクリプションが移行されたときに引き続きアクセス権を所有します。</span><span class="sxs-lookup"><span data-stu-id="c080a-147">If you had admin access rights to the existing CSP subscription, you will continue to have access when that subscription is migrated.</span></span>

<span data-ttu-id="c080a-148">ダイレクト エンタープライズ契約を CSP に移行し、サーバーとクラウドの登録を Azure サービスに移行するには、[Microsoft パートナー契約での Azure サブスクリプションの課金所有権の取得](https://docs.microsoft.com/azure/billing/mpa-request-ownership)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c080a-148">To transition direct Enterprise Agreements to CSP and Server and Cloud enrollments to Azure services, read [Get billing ownership of Azure subscriptions for Microsoft Partner Agreement](https://docs.microsoft.com/azure/billing/mpa-request-ownership)</span></span>

### <a name="audit-log"></a><span data-ttu-id="c080a-149">監査ログ</span><span class="sxs-lookup"><span data-stu-id="c080a-149">Audit log</span></span>

<span data-ttu-id="c080a-150">請求を調整するには、 **[サブスクリプション]** ページで "Microsoft Azure" (0145P) サブスクリプションの履歴を表示します。</span><span class="sxs-lookup"><span data-stu-id="c080a-150">To reconcile billing, view your history of "Microsoft Azure" (0145P) subscriptions on the **Subscriptions** page.</span></span>

<span data-ttu-id="c080a-151">"Microsoft Azure" (0145P) サブスクリプションは、次の 2 つの部分で構成されます。</span><span class="sxs-lookup"><span data-stu-id="c080a-151">"Microsoft Azure" (0145P) subscription is comprised of two parts:</span></span>

1. <span data-ttu-id="c080a-152">コマース サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="c080a-152">Commerce subscription</span></span>
2. <span data-ttu-id="c080a-153">Azure サブスクリプション (権利)</span><span class="sxs-lookup"><span data-stu-id="c080a-153">Azure subscription (entitlement)</span></span>

<span data-ttu-id="c080a-154">移行が完了すると、Azure サブスクリプションは新しい Azure プランの下に移動され、コマース サブスクリプションはこれ以上の使用が報告されないように停止されます。</span><span class="sxs-lookup"><span data-stu-id="c080a-154">When the transition is complete, the Azure subscription is moved under new Azure plan and the commerce subscription is suspended so that no further usage is reported.</span></span>  

>[!NOTE]
><span data-ttu-id="c080a-155">CSP で Microsoft Azure (0145P) サブスクリプションを 購入した場合、コマース サブスクリプションと Azure サブスクリプション (権利) の価格は同じになります。</span><span class="sxs-lookup"><span data-stu-id="c080a-155">When Microsoft Azure (0145P) subscription is purchased in CSP, both the commerce subscription and the Azure subscription (entitlement) have the same value.</span></span> <span data-ttu-id="c080a-156">これは、課金所有権の変更または譲渡で価格が異なる場合にのみ発生します。</span><span class="sxs-lookup"><span data-stu-id="c080a-156">It is only in the case of billing ownership changes or transfers do the values differ.</span></span>

### <a name="transition-issues"></a><span data-ttu-id="c080a-157">移行に関する問題</span><span class="sxs-lookup"><span data-stu-id="c080a-157">Transition issues</span></span>

<span data-ttu-id="c080a-158">移行中に問題が発生することは想定されていません。</span><span class="sxs-lookup"><span data-stu-id="c080a-158">We don't anticipate any issues during transitions.</span></span> <span data-ttu-id="c080a-159">発生した場合は、移行ワークフロー自体の中で更新が実行されます。</span><span class="sxs-lookup"><span data-stu-id="c080a-159">If one occurs, we will update you in the transition workflow itself.</span></span> <span data-ttu-id="c080a-160">Azure の使用に障害が発生することはありません。</span><span class="sxs-lookup"><span data-stu-id="c080a-160">There won't be disturbances to Azure usage.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="c080a-161">次の手順</span><span class="sxs-lookup"><span data-stu-id="c080a-161">Next steps</span></span>

- [<span data-ttu-id="c080a-162">Azure プランのサブスクリプションとリソースを管理する</span><span class="sxs-lookup"><span data-stu-id="c080a-162">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="c080a-163">パートナー獲得クレジット - 概要</span><span class="sxs-lookup"><span data-stu-id="c080a-163">Partner earned credit - overview</span></span>](partner-earned-credit.md)
