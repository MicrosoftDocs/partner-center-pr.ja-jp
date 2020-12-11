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
ms.openlocfilehash: 4e22386dc8bddd9662a0d80020a5c90c464e9d39
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534813"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a><span data-ttu-id="8983d-103">顧客を既存の CSP Azure プランから Azure プランに移行する</span><span class="sxs-lookup"><span data-stu-id="8983d-103">Transition customers to Azure plan from existing CSP Azure offers</span></span>

<span data-ttu-id="8983d-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="8983d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8983d-105">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="8983d-105">Admin agent</span></span>
- <span data-ttu-id="8983d-106">課金管理者</span><span class="sxs-lookup"><span data-stu-id="8983d-106">Billing admin</span></span>
- <span data-ttu-id="8983d-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="8983d-107">Global admin</span></span>
- <span data-ttu-id="8983d-108">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="8983d-108">Helpdesk agent</span></span>
- <span data-ttu-id="8983d-109">販売代理店</span><span class="sxs-lookup"><span data-stu-id="8983d-109">Sales agent</span></span>
- <span data-ttu-id="8983d-110">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="8983d-110">User management admin</span></span>

<span data-ttu-id="8983d-111">この記事では、CSP パートナーが、パートナー センターを使用して顧客を既存の CSP Azure オファーから、Azure プランで管理される Azure サービスに移行する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="8983d-111">This article explains how CSP partners can use Partner Center to move customers from existing CSP Azure offers to Azure services under the Azure plan.</span></span> <span data-ttu-id="8983d-112">間接プロバイダーおよび直接請求パートナーは、Azure 向け Microsoft クラウド サービス プロバイダー (CSP) プログラムで利用可能な新しいコマース エクスペリエンスに移行できます。</span><span class="sxs-lookup"><span data-stu-id="8983d-112">Indirect providers and direct bill partners can transition to the new commerce experience available in the Microsoft Cloud Service Provider Program (CSP) for Azure.</span></span> <span data-ttu-id="8983d-113">(間接リセラーは、間接プロバイダーを通じて行う必要があります)。パートナーからの購入、マイクロソフト販売者からの購入、または Web 上での直接購入にかかわらず、クラウド サービスを簡単に購入するための最新の方法が顧客に提供されます。</span><span class="sxs-lookup"><span data-stu-id="8983d-113">(Indirect resellers will need to work through their indirect providers.) Customers will have a streamlined way to buy cloud services, whether purchasing from partners, from Microsoft sellers, or directly on the web.</span></span>

<span data-ttu-id="8983d-114">移行機能は、Azure の新しいコマース エクスペリエンスに移行し、Microsoft 顧客契約に署名したお客様のみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="8983d-114">The transition capability is only for customers transitioning to the new commerce experience for Azure and who have signed the Microsoft Customer Agreement.</span></span> <span data-ttu-id="8983d-115">Office 365 や Dynamics 365 など、CSP の他のオファーは対象ではありません。</span><span class="sxs-lookup"><span data-stu-id="8983d-115">It is not for other offers in CSP such as Office 365 or Dynamics 365.</span></span>

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a><span data-ttu-id="8983d-116">既存の CSP プランの Azure プランへの移行</span><span class="sxs-lookup"><span data-stu-id="8983d-116">Transition existing CSP offers to an Azure plan</span></span>

<span data-ttu-id="8983d-117">パートナー センターで、既存の CSP Azure プランから CSP プログラムの新しいコマース エクスペリエンスである Azure プランで管理される Azure サービスに顧客を移行させることができます。</span><span class="sxs-lookup"><span data-stu-id="8983d-117">You can transition a customer from their existing CSP Azure offers to Azure services under the Azure plan in the new commerce experience in the CSP program from within Partner Center.</span></span> <span data-ttu-id="8983d-118">これを行うには、パートナーと顧客の間にパートナー センターを通じて再販業者関係が確立されている必要があり、顧客が Microsoft 顧客契約に署名している必要があります。</span><span class="sxs-lookup"><span data-stu-id="8983d-118">To do this, the partner and customer must have an established reseller relationship through Partner Center, and the customer must have signed the Microsoft Customer Agreement.</span></span>

### <a name="select-transition-to-azure-plan"></a><span data-ttu-id="8983d-119">Azure プランへの移行を選択する</span><span class="sxs-lookup"><span data-stu-id="8983d-119">Select transition to Azure plan</span></span>

1. <span data-ttu-id="8983d-120">顧客向けの Azure プランを選択します。</span><span class="sxs-lookup"><span data-stu-id="8983d-120">Select Azure plan for your customer.</span></span>

2. <span data-ttu-id="8983d-121">**[請求を Azure プランに移行する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8983d-121">Select **Transition billing to Azure plan**.</span></span>

   :::image type="content" source="images/azure/transition1.png" alt-text="使用状況に基づいたサブスクリプションのレポート情報を示すスクリーンショット。選択可能な次のオプションが表示されています:[Azure サブスクリプション請求を Azure プランに移行する]。":::

3. <span data-ttu-id="8983d-123">**[続行]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8983d-123">Select **Continue**</span></span>

   :::image type="content" source="images/azure/transition2.png" alt-text="[Transition to Azure plan]\(Azure プランへの移行\) というタイトルのダイアログ ボックス。移行についての説明と、[続行] および [キャンセル] という選択可能な 2 つのオプションが表示されています。":::

   <span data-ttu-id="8983d-125">顧客は、Azure プランに移行されます。</span><span class="sxs-lookup"><span data-stu-id="8983d-125">Your customer will be transitioned to the Azure plan.</span></span>

   <span data-ttu-id="8983d-126">**移行ワークフローによって、前提条件となる手順が自動化されます**。</span><span class="sxs-lookup"><span data-stu-id="8983d-126">**The transition workflow automates the pre-requisite steps**:</span></span>

   - <span data-ttu-id="8983d-127">Azure プランの購入</span><span class="sxs-lookup"><span data-stu-id="8983d-127">Purchase of Azure plan(s)</span></span>
   - <span data-ttu-id="8983d-128">ダイレクト CSP での顧客ごとに 1 つのプラン シナリオ</span><span class="sxs-lookup"><span data-stu-id="8983d-128">One plan per customer in Direct CSP scenarios</span></span>  
   - <span data-ttu-id="8983d-129">リセラーごとに 1 つのプラン</span><span class="sxs-lookup"><span data-stu-id="8983d-129">One plan per reseller</span></span>  

   <span data-ttu-id="8983d-130">例として、パートナーが 2つの Microsoft Azure プランを購入し、その購入の中に 2 つの異なる POR が含まれているとします。</span><span class="sxs-lookup"><span data-stu-id="8983d-130">For an example, a partner has purchased two Microsoft Azure offers and has included two distinct POR in the purchase.</span></span> <span data-ttu-id="8983d-131">この場合、移行ワークフローでは、2 つの Azure プラン (リセラーごとに 1 つ) が購入され、各 Azure サブスクリプションが Azure プランに自動的にマップされます。</span><span class="sxs-lookup"><span data-stu-id="8983d-131">In this case, the transition    workflow will purchase two Azure plans (one per reseller) and map the respective Azure subscriptions under the Azure plans automatically.</span></span>  

   <span data-ttu-id="8983d-132">**Azure サブスクリプションの Azure プランへのマッピング**</span><span class="sxs-lookup"><span data-stu-id="8983d-132">**Mapping Azure subscription to Azure plan**</span></span>

   <span data-ttu-id="8983d-133">Azure プランを購入すると、システムによって既存の Azure サブスクリプションが Azure プランにマップされます。</span><span class="sxs-lookup"><span data-stu-id="8983d-133">After your purchase of Azure plan(s), our system will map the existing Azure subscriptions to the Azure plans.</span></span> <span data-ttu-id="8983d-134">進行状況は、パートナー センターだけでなく Azure portal でも確認できます。</span><span class="sxs-lookup"><span data-stu-id="8983d-134">The progress can be viewed in Azure portal as well as in Partner center.</span></span>

4. <span data-ttu-id="8983d-135">顧客のパートナー センターの **[サブスクリプション]** ページに戻り、顧客の現地通貨を使用して予算制限を更新します。</span><span class="sxs-lookup"><span data-stu-id="8983d-135">Return to your customer's Partner Center **Subscriptions** page to update their budget limit using their local currency.</span></span>

   :::image type="content" source="images/azure/transition3.png" alt-text="パートナー センターの [サブスクリプション] ページの一部分。請求期間の予算制限が現地の通貨で設定されています。":::

   >[!NOTE]
   ><span data-ttu-id="8983d-137">パートナー センターで設定した予算は、Azure portal には引き継がれません。</span><span class="sxs-lookup"><span data-stu-id="8983d-137">The budget you set in Partner Center doesn't carry over to the Azure portal.</span></span> <span data-ttu-id="8983d-138">Azure portal で、予算とアラートも設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8983d-138">You should also set the budget and alert in Azure portal.</span></span>

   <span data-ttu-id="8983d-139">Azure プランに移行すると、この顧客用の Azure サブスクリプションを購入することはできなくなります。</span><span class="sxs-lookup"><span data-stu-id="8983d-139">When you move to the Azure plan, you can no longer purchase Azure subscriptions for this customer.</span></span> <span data-ttu-id="8983d-140">サブスクリプションは、Azure portal で Azure プランの中に作成します。</span><span class="sxs-lookup"><span data-stu-id="8983d-140">You create the subscriptions under the Azure plan in the Azure portal.</span></span>

   >[!NOTE]
   > <span data-ttu-id="8983d-141">Azure プランで RBAC を通して購入されたすべての Azure サブスクリプションに対し、現地通貨で請求および課金されます。</span><span class="sxs-lookup"><span data-stu-id="8983d-141">All Azure subscriptions purchased through RBAC under the Azure plan will be    priced and billed in local currency.</span></span> <span data-ttu-id="8983d-142">為替レートは使用されません。</span><span class="sxs-lookup"><span data-stu-id="8983d-142">FX rates will not be used.</span></span>

### <a name="track-your-transition-details"></a><span data-ttu-id="8983d-143">移行の詳細を追跡する</span><span class="sxs-lookup"><span data-stu-id="8983d-143">Track your transition details</span></span>

<span data-ttu-id="8983d-144">パートナー センターだけでなく、Azure portal でも移行の進行状況を確認してください。</span><span class="sxs-lookup"><span data-stu-id="8983d-144">Follow the transition progress in Azure portal as well as in Partner Center.</span></span>

:::image type="content" source="images/azure/details1.png" alt-text="サブスクリプションごとに移行の詳細リストが表示されている表のスクリーンショット。サブスクリプション ID、移行日、移行の状態が含まれています。":::

### <a name="billing-impact-to-partners"></a><span data-ttu-id="8983d-146">パートナーに対する請求の影響</span><span class="sxs-lookup"><span data-stu-id="8983d-146">Billing impact to partners</span></span>

<span data-ttu-id="8983d-147">既存の CSP Azure プランから顧客を移行する場合、次のような請求の影響が発生します。</span><span class="sxs-lookup"><span data-stu-id="8983d-147">If you transition a customer from an existing CSP Azure offer, you will have the following billing impacts:</span></span>

- <span data-ttu-id="8983d-148">元の CSP Azure サブスクリプションの終了時点までのすべての使用量については、既存の CSP 請求書で請求されます。</span><span class="sxs-lookup"><span data-stu-id="8983d-148">You will be billed on your existing CSP invoice for all usage up to the point of exiting the original CSP Azure subscription.</span></span>

- <span data-ttu-id="8983d-149">既存の CSP サブスクリプションに対する管理者アクセス権を持っている場合は、そのサブスクリプションが移行されたときに引き続きアクセス権を所有します。</span><span class="sxs-lookup"><span data-stu-id="8983d-149">If you had admin access rights to the existing CSP subscription, you will continue to have access when that subscription is migrated.</span></span>

<span data-ttu-id="8983d-150">ダイレクト エンタープライズ契約を CSP に移行し、サーバーとクラウドの登録を Azure サービスに移行するには、[Microsoft パートナー契約での Azure サブスクリプションの課金所有権の取得](/azure/billing/mpa-request-ownership)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8983d-150">To transition direct Enterprise Agreements to CSP and Server and Cloud enrollments to Azure services, read [Get billing ownership of Azure subscriptions for Microsoft Partner Agreement](/azure/billing/mpa-request-ownership)</span></span>

### <a name="audit-log"></a><span data-ttu-id="8983d-151">監査ログ</span><span class="sxs-lookup"><span data-stu-id="8983d-151">Audit log</span></span>

<span data-ttu-id="8983d-152">請求を調整するには、 **[サブスクリプション]** ページで "Microsoft Azure" (0145P) サブスクリプションの履歴を表示します。</span><span class="sxs-lookup"><span data-stu-id="8983d-152">To reconcile billing, view your history of "Microsoft Azure" (0145P) subscriptions on the **Subscriptions** page.</span></span>

<span data-ttu-id="8983d-153">"Microsoft Azure" (0145P) サブスクリプションは、次の 2 つの部分で構成されます。</span><span class="sxs-lookup"><span data-stu-id="8983d-153">"Microsoft Azure" (0145P) subscription is comprised of two parts:</span></span>

1. <span data-ttu-id="8983d-154">コマース サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="8983d-154">Commerce subscription</span></span>
2. <span data-ttu-id="8983d-155">Azure サブスクリプション (権利)</span><span class="sxs-lookup"><span data-stu-id="8983d-155">Azure subscription (entitlement)</span></span>

<span data-ttu-id="8983d-156">移行が完了すると、Azure サブスクリプションは新しい Azure プランの下に移動され、コマース サブスクリプションはこれ以上の使用が報告されないように停止されます。</span><span class="sxs-lookup"><span data-stu-id="8983d-156">When the transition is complete, the Azure subscription is moved under new Azure plan and the commerce subscription is suspended so that no further usage is reported.</span></span>  

>[!NOTE]
><span data-ttu-id="8983d-157">CSP で Microsoft Azure (0145P) サブスクリプションを 購入した場合、コマース サブスクリプションと Azure サブスクリプション (権利) の価格は同じになります。</span><span class="sxs-lookup"><span data-stu-id="8983d-157">When Microsoft Azure (0145P) subscription is purchased in CSP, both the commerce subscription and the Azure subscription (entitlement) have the same value.</span></span> <span data-ttu-id="8983d-158">これは、課金所有権の変更または譲渡で価格が異なる場合にのみ発生します。</span><span class="sxs-lookup"><span data-stu-id="8983d-158">It is only in the case of billing ownership changes or transfers do the values differ.</span></span>

### <a name="transition-issues"></a><span data-ttu-id="8983d-159">移行に関する問題</span><span class="sxs-lookup"><span data-stu-id="8983d-159">Transition issues</span></span>

<span data-ttu-id="8983d-160">移行中に問題が発生することは想定されていません。</span><span class="sxs-lookup"><span data-stu-id="8983d-160">We don't anticipate any issues during transitions.</span></span> <span data-ttu-id="8983d-161">発生した場合は、移行ワークフロー自体の中で更新が実行されます。</span><span class="sxs-lookup"><span data-stu-id="8983d-161">If one occurs, we will update you in the transition workflow itself.</span></span> <span data-ttu-id="8983d-162">Azure の使用に障害が発生することはありません。</span><span class="sxs-lookup"><span data-stu-id="8983d-162">There won't be disturbances to Azure usage.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="8983d-163">次の手順</span><span class="sxs-lookup"><span data-stu-id="8983d-163">Next steps</span></span>

- [<span data-ttu-id="8983d-164">Azure プランのサブスクリプションとリソースを管理する</span><span class="sxs-lookup"><span data-stu-id="8983d-164">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="8983d-165">パートナー獲得クレジット - 概要</span><span class="sxs-lookup"><span data-stu-id="8983d-165">Partner earned credit - overview</span></span>](partner-earned-credit.md)