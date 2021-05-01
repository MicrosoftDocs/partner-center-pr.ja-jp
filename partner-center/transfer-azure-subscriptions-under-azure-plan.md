---
title: Azure プランで Azure サブスクリプションを別の CSP パートナーに転送する
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure プランで顧客の Azure サブスクリプションに関連付けられているクラウドソリューションプロバイダープログラムパートナーを変更する方法について説明します。
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 12afa751d2e7cb6b6ef0cd7308f09746a8a43b52
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284504"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="afe15-103">顧客の Azure プランサブスクリプションを別のパートナーに譲渡する</span><span class="sxs-lookup"><span data-stu-id="afe15-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="afe15-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="afe15-104">**Appropriate roles**</span></span>

- <span data-ttu-id="afe15-105">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="afe15-105">Account admin</span></span>
- <span data-ttu-id="afe15-106">販売代理店</span><span class="sxs-lookup"><span data-stu-id="afe15-106">Sales agent</span></span>
- <span data-ttu-id="afe15-107">課金エージェント</span><span class="sxs-lookup"><span data-stu-id="afe15-107">Billing agent</span></span>

<span data-ttu-id="afe15-108">この記事では、顧客が azure プランの Azure サブスクリプションを1つのクラウドソリューションプロバイダー (CSP) から別のクラウドソリューションプロバイダー (CSP) に切り替える方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="afe15-108">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="afe15-109">顧客の Azure サブスクリプションを別のパートナーから切り替えるには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="afe15-109">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="afe15-110">パートナーと顧客の両方に対して、手順を完了する必要があります。</span><span class="sxs-lookup"><span data-stu-id="afe15-110">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="afe15-111">Microsoft との直接の課金関係を持つパートナーだけが、移行ツールにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="afe15-111">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="afe15-112">間接リセラーは、この移行ツールを活用するために間接プロバイダーと協力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="afe15-112">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="afe15-113">お客様は、このツールを利用する前に、両方のパートナー (現在と将来) との話し合いを行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="afe15-113">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="afe15-114">オフラインのメッセージ交換では、混乱とチャーンを避ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="afe15-114">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="afe15-115">また、移行を開始する前に、パートナーと顧客がこれらの考慮事項と前提条件を理解しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="afe15-115">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="afe15-116">**主な考慮事項:**</span><span class="sxs-lookup"><span data-stu-id="afe15-116">**Key considerations:**</span></span>

- <span data-ttu-id="afe15-117">Azure Reservations は、今後のパートナーにサブスクリプションと共に移動することはありません</span><span class="sxs-lookup"><span data-stu-id="afe15-117">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="afe15-118">現在のパートナーの Azure サービスの CSP 価格は移行されません</span><span class="sxs-lookup"><span data-stu-id="afe15-118">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="afe15-119">お客様のサポート責任が将来のパートナーに移行されます</span><span class="sxs-lookup"><span data-stu-id="afe15-119">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="afe15-120">課金と請求は、転送時に将来のパートナーに移行されます</span><span class="sxs-lookup"><span data-stu-id="afe15-120">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="afe15-121">Azure Role-Based Access Control (RBAC) は転送の影響を受けません</span><span class="sxs-lookup"><span data-stu-id="afe15-121">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="afe15-122">(AOBO) の代理管理者は、既定では今後のパートナーに付与されません</span><span class="sxs-lookup"><span data-stu-id="afe15-122">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="afe15-123">製品が Marketplace の適格性チェックに合格している限り、サードパーティの marketplace 製品は譲渡されます。</span><span class="sxs-lookup"><span data-stu-id="afe15-123">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="afe15-124">特別な割引や地域の制限はありません</span><span class="sxs-lookup"><span data-stu-id="afe15-124">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="afe15-125">製品は非サブスクリプションベースです</span><span class="sxs-lookup"><span data-stu-id="afe15-125">The products are non-subscription based</span></span>
    - <span data-ttu-id="afe15-126">将来のパートナーは、発行元と協力して、製品の展開のために許可リストにいることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="afe15-126">The future partner should work with the publisher to make sure they are on the allowlist for deployment of the product</span></span>
    - <span data-ttu-id="afe15-127">これらのすべての条件が満たされていない場合は、Marketplace 製品をキャンセルし、Azure サブスクリプションを譲渡した後、新しいパートナーと共に Marketplace 製品を再購入します。</span><span class="sxs-lookup"><span data-stu-id="afe15-127">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="afe15-128">**前提条件:**</span><span class="sxs-lookup"><span data-stu-id="afe15-128">**Prerequisites:**</span></span>

- <span data-ttu-id="afe15-129">お客様が現在の CSP パートナーを移行の目的で利用</span><span class="sxs-lookup"><span data-stu-id="afe15-129">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="afe15-130">将来の CSP パートナーがお客様と連携して顧客のニーズを満たすことができるようにする</span><span class="sxs-lookup"><span data-stu-id="afe15-130">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="afe15-131">今後の CSP パートナーが顧客との関係を確立し、移行が開始される前に Azure プランを購入する</span><span class="sxs-lookup"><span data-stu-id="afe15-131">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="afe15-132">お客様は、今後の CSP パートナーと共に Microsoft カスタマー契約に署名する必要があります</span><span class="sxs-lookup"><span data-stu-id="afe15-132">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="afe15-133">このツールを使用するには、今後の CSP パートナーが Microsoft パートナー契約に署名している必要があります</span><span class="sxs-lookup"><span data-stu-id="afe15-133">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="afe15-134">完了する顧客タスク</span><span class="sxs-lookup"><span data-stu-id="afe15-134">Customer tasks to be completed</span></span>

<span data-ttu-id="afe15-135">Azure プランで Azure サブスクリプションを譲渡するには、お客様は現在のパートナーに連絡してプロセスを開始する必要があります。</span><span class="sxs-lookup"><span data-stu-id="afe15-135">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="afe15-136">パートナーは、現在のパートナーの会社名とドメインを収集する必要があります。これにより、将来のパートナーが代理で転送要求フォームを完了できるようになります。</span><span class="sxs-lookup"><span data-stu-id="afe15-136">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="afe15-137">また、お客様は、現在のパートナーから譲渡するサブスクリプションを特定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="afe15-137">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="afe15-138">Office 365、Enterprise Mobility Suite、または Microsoft Dynamics CRM サブスクリプションのパートナーを変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="afe15-138">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="afe15-139">譲渡プロセスを開始する転送要求フォームを完了するのは、今後のパートナーの責任です。</span><span class="sxs-lookup"><span data-stu-id="afe15-139">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="afe15-140">Microsoft は、お客様または現在のパートナーに代わって介入することはできません。</span><span class="sxs-lookup"><span data-stu-id="afe15-140">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="afe15-141">お客様は、将来と現在のパートナーと密接に連携して、移行を円滑に進めることを計画する必要があります。</span><span class="sxs-lookup"><span data-stu-id="afe15-141">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="afe15-142">今後のパートナータスクの完了</span><span class="sxs-lookup"><span data-stu-id="afe15-142">Future partner tasks to be completed</span></span>

<span data-ttu-id="afe15-143">サブスクリプションの今後のパートナーは、パートナーセンターから譲渡要求フォームを完了して、サブスクリプションの譲渡を要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="afe15-143">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="afe15-144">パートナーセンターメニューから、[ **顧客**] を選択し、代理で転送要求フォームを完了する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="afe15-144">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="afe15-145">カスタマーメニューから [ **サブスクリプション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="afe15-145">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="afe15-146">[ **転送要求** ] セクションを選択します。</span><span class="sxs-lookup"><span data-stu-id="afe15-146">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="afe15-147">[ **転送要求] セクション** で、[ **新しい要求の追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="afe15-147">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="転送セクション":::

5.  <span data-ttu-id="afe15-149">**新しい転送要求** フォームに入力します。</span><span class="sxs-lookup"><span data-stu-id="afe15-149">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="afe15-150">[**転送要求** の送信] を選択し  >  ます。</span><span class="sxs-lookup"><span data-stu-id="afe15-150">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="転送要求の完了フォーム":::

7.  <span data-ttu-id="afe15-152">転送要求の確認の確認</span><span class="sxs-lookup"><span data-stu-id="afe15-152">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="保留中の転送の確認":::

    >[!Note]
    ><span data-ttu-id="afe15-154">将来のパートナーは、転送要求の状態が [保留中] の場合にのみ、右上隅にある **[要求のキャンセル]** を選択して、譲渡要求を取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="afe15-154">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="afe15-155">転送要求の状態が "進行中" または "完了" になると、取り消しはできなくなります。</span><span class="sxs-lookup"><span data-stu-id="afe15-155">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="afe15-156">完了する現在のパートナータスク</span><span class="sxs-lookup"><span data-stu-id="afe15-156">Current partner tasks to be completed</span></span>

<span data-ttu-id="afe15-157">お客様の現在のパートナーの管理者エージェントは、お客様がサブスクリプションの譲渡を要求しているという電子メールを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="afe15-157">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="確認":::

<span data-ttu-id="afe15-159">パートナーセンターから譲渡要求フォームを確認して同意し、サブスクリプションの譲渡を完了します。</span><span class="sxs-lookup"><span data-stu-id="afe15-159">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="afe15-160">現在のパートナーが30日以内にアクションを実行しなかった場合は、要求の有効期限が切れ、今後のパートナーは新しい転送要求を作成するためにを使用します。</span><span class="sxs-lookup"><span data-stu-id="afe15-160">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="afe15-161">[電子メールからの **転送要求のレビュー** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="afe15-161">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="afe15-162">パートナーセンターメニューから [ **顧客**] を選択し、譲渡要求が送信された顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="afe15-162">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="afe15-163">カスタマーメニューから [ **サブスクリプション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="afe15-163">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="afe15-164">[ **転送要求** ] セクションを選択します。</span><span class="sxs-lookup"><span data-stu-id="afe15-164">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="afe15-165">[**受信した要求**] で選択した **転送要求 ID** を選択して、[転送情報] を展開します。</span><span class="sxs-lookup"><span data-stu-id="afe15-165">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="ソースレビューの譲渡要求":::

5.  <span data-ttu-id="afe15-167">譲渡要求を確認します。</span><span class="sxs-lookup"><span data-stu-id="afe15-167">Review transfer request.</span></span> <span data-ttu-id="afe15-168">転送する要求された Azure サブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="afe15-168">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="afe15-169">続行する前に、選択したサブスクリプションにアクセスできなくなります。</span><span class="sxs-lookup"><span data-stu-id="afe15-169">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="afe15-170">今後の使用のために請求されることはありません。</span><span class="sxs-lookup"><span data-stu-id="afe15-170">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="afe15-171">Azure の予約は、サブスクリプションと共には転送されません。</span><span class="sxs-lookup"><span data-stu-id="afe15-171">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="afe15-172">次に、[ **受け入れて転送** ] を選択して、転送プロセスを完了します。</span><span class="sxs-lookup"><span data-stu-id="afe15-172">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Azure プランで転送するサブスクリプションを選択します":::

7.  <span data-ttu-id="afe15-174">転送の受け入れ確認を表示します。</span><span class="sxs-lookup"><span data-stu-id="afe15-174">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="afe15-175">この時点で、今後のパートナー、顧客、および現在のパートナーには、電子メールで受け入れられた譲渡要求が通知されます。</span><span class="sxs-lookup"><span data-stu-id="afe15-175">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="afe15-176">その後、移行が受け入れられると、システムが更新されている間、転送状態が最大15分間保留状態のままになることがあります。</span><span class="sxs-lookup"><span data-stu-id="afe15-176">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="afe15-177">時間がかかると、システムは3日間試行し続けます。</span><span class="sxs-lookup"><span data-stu-id="afe15-177">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="afe15-178">転送の状態が保留中のままである場合、パートナーはサービス要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="afe15-178">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="afe15-179">転送が完了すると、要求内に含まれているサブスクリプションが、今後のパートナーの Azure プランに表示され、お客様と共に表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="afe15-179">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="afe15-180">間接プロバイダーの場合: 譲渡要求が受け入れられたことを間接リセラーに知らせてください。</span><span class="sxs-lookup"><span data-stu-id="afe15-180">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="afe15-181">転送された顧客サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="afe15-181">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="afe15-182">移転中、Azure ロールベースのアクセス制御 (RBAC) を使用して割り当てられた既存のユーザー、グループ、またはサービス プリンシパルへのアクセスは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="afe15-182">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="afe15-183">Azure のロールベースのアクセス制御 [(AZURE RBAC)](/azure/role-based-access-control/overview) を使用すると、顧客は、azure リソースにアクセスできるユーザー、それらのリソースを使用して実行できること、およびアクセス権を持つ領域を管理できます。</span><span class="sxs-lookup"><span data-stu-id="afe15-183">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="afe15-184">新しいパートナーとして、サブスクリプションの譲渡後に、お客様のリソースに対する RBAC アクセス権は付与されません。</span><span class="sxs-lookup"><span data-stu-id="afe15-184">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="afe15-185">お客様の以前のパートナーは、RBAC アクセスを維持しています。</span><span class="sxs-lookup"><span data-stu-id="afe15-185">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="afe15-186">お客様と協力して、サブスクリプションについての洞察を持つユーザーと、必要な変更を行う方法を理解します。</span><span class="sxs-lookup"><span data-stu-id="afe15-186">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="afe15-187">そのため、お客様は前のパートナー向けの Azure RBAC アクセスを削除し、新しいパートナーのアクセス権を追加することが重要です。</span><span class="sxs-lookup"><span data-stu-id="afe15-187">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="afe15-188">顧客が新しいアクセス権を付与する方法の詳細については、「 [azure のロールベースのアクセス制御 (AZURE RBAC) とは](/azure/role-based-access-control/overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="afe15-188">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="afe15-189">以前のパートナーの RBAC アクセスを削除する顧客の詳細については、「 [ロールの割り当てを削除する](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="afe15-189">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="afe15-190">さらに、サブスクリプションへ [の (AOBO) アクセスの代理](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) として自動的に管理者を取得することはありません。</span><span class="sxs-lookup"><span data-stu-id="afe15-190">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="afe15-191">AOBO は、パートナーが顧客の Azure サブスクリプションを代理として管理するために必要です。</span><span class="sxs-lookup"><span data-stu-id="afe15-191">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="afe15-192">Azure の特権の詳細について[は、「顧客のサービスまたはサブスクリプションを管理するためのアクセス許可を取得する](./customers-revoke-admin-privileges.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="afe15-192">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="afe15-193">次のステップ:</span><span class="sxs-lookup"><span data-stu-id="afe15-193">Next steps:</span></span>

- [<span data-ttu-id="afe15-194">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="afe15-194">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="afe15-195">顧客のサービスまたはサブスクリプションを管理するためのアクセス許可を取得します。</span><span class="sxs-lookup"><span data-stu-id="afe15-195">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
