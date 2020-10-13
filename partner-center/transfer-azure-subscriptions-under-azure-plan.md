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
ms.openlocfilehash: 4213658fc131d83d6c0640552d862f4de9b5ad86
ms.sourcegitcommit: e10d2a19dea7e317d227d7fbdcf1bbc3dc4f6257
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/13/2020
ms.locfileid: "91980263"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="7b797-103">顧客の Azure プランサブスクリプションを別のパートナーに譲渡する</span><span class="sxs-lookup"><span data-stu-id="7b797-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

## <a name="applies-to"></a><span data-ttu-id="7b797-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="7b797-104">Applies to</span></span>

- <span data-ttu-id="7b797-105">クラウド ソリューション プロバイダー (CSP) プログラムのパートナー</span><span class="sxs-lookup"><span data-stu-id="7b797-105">Partners in the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="7b797-106">この記事では、顧客が azure プランの Azure サブスクリプションを1つのクラウドソリューションプロバイダー (CSP) から別のクラウドソリューションプロバイダー (CSP) に切り替える方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="7b797-106">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="7b797-107">顧客の Azure サブスクリプションを別のパートナーから切り替えるには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="7b797-107">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="7b797-108">パートナーと顧客の両方に対して、手順を完了する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b797-108">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="7b797-109">Microsoft との直接の課金関係を持つパートナーだけが、移行ツールにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="7b797-109">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="7b797-110">間接リセラーは、この移行ツールを活用するために間接プロバイダーと協力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b797-110">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="7b797-111">お客様は、このツールを利用する前に、両方のパートナー (現在と将来) との話し合いを行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b797-111">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="7b797-112">オフラインのメッセージ交換では、混乱とチャーンを避ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b797-112">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="7b797-113">また、移行を開始する前に、パートナーと顧客がこれらの考慮事項と前提条件を理解しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b797-113">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="7b797-114">**主な考慮事項:**</span><span class="sxs-lookup"><span data-stu-id="7b797-114">**Key considerations:**</span></span>

- <span data-ttu-id="7b797-115">Azure Reservations は、今後のパートナーにサブスクリプションと共に移動することはありません</span><span class="sxs-lookup"><span data-stu-id="7b797-115">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="7b797-116">現在のパートナーの Azure サービスの CSP 価格は移行されません</span><span class="sxs-lookup"><span data-stu-id="7b797-116">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="7b797-117">お客様のサポート責任が将来のパートナーに移行されます</span><span class="sxs-lookup"><span data-stu-id="7b797-117">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="7b797-118">課金と請求は、転送時に将来のパートナーに移行されます</span><span class="sxs-lookup"><span data-stu-id="7b797-118">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="7b797-119">Azure Role-Based Access Control (RBAC) は転送の影響を受けません</span><span class="sxs-lookup"><span data-stu-id="7b797-119">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="7b797-120">(AOBO) の代理管理者は、既定では今後のパートナーに付与されません</span><span class="sxs-lookup"><span data-stu-id="7b797-120">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="7b797-121">製品が Marketplace の適格性チェックに合格している限り、サードパーティの marketplace 製品は譲渡されます。</span><span class="sxs-lookup"><span data-stu-id="7b797-121">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="7b797-122">特別な割引や地域の制限はありません</span><span class="sxs-lookup"><span data-stu-id="7b797-122">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="7b797-123">製品は非サブスクリプションベースです</span><span class="sxs-lookup"><span data-stu-id="7b797-123">The products are non-subscription based</span></span>
    - <span data-ttu-id="7b797-124">将来のパートナーは、発行元と協力して、製品の展開の許可リストに含まれていることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b797-124">The future partner should work with the publisher to make sure they are on the allow-list for deployment of the product</span></span>
    - <span data-ttu-id="7b797-125">これらのすべての条件が満たされていない場合は、Marketplace 製品をキャンセルし、Azure サブスクリプションを譲渡した後、新しいパートナーと共に Marketplace 製品を再購入します。</span><span class="sxs-lookup"><span data-stu-id="7b797-125">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="7b797-126">**前提条件:**</span><span class="sxs-lookup"><span data-stu-id="7b797-126">**Prerequisites:**</span></span>

- <span data-ttu-id="7b797-127">お客様が現在の CSP パートナーを移行の目的で利用</span><span class="sxs-lookup"><span data-stu-id="7b797-127">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="7b797-128">将来の CSP パートナーがお客様と連携して顧客のニーズを満たすことができるようにする</span><span class="sxs-lookup"><span data-stu-id="7b797-128">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="7b797-129">将来の CSP パートナーが、移行を開始する前に顧客との関係を確立する</span><span class="sxs-lookup"><span data-stu-id="7b797-129">Future CSP partner establishes a relationship with customer before transition begins</span></span>  
- <span data-ttu-id="7b797-130">お客様は、今後の CSP パートナーと共に Microsoft カスタマー契約に署名する必要があります</span><span class="sxs-lookup"><span data-stu-id="7b797-130">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="7b797-131">このツールを使用するには、今後の CSP パートナーが Microsoft パートナー契約に署名している必要があります</span><span class="sxs-lookup"><span data-stu-id="7b797-131">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="7b797-132">完了する顧客タスク</span><span class="sxs-lookup"><span data-stu-id="7b797-132">Customer tasks to be completed</span></span>

<span data-ttu-id="7b797-133">Azure プランで Azure サブスクリプションを譲渡するには、お客様は現在のパートナーに連絡してプロセスを開始する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b797-133">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="7b797-134">パートナーは、現在のパートナーの会社名とドメインを収集する必要があります。これにより、将来のパートナーが代理で転送要求フォームを完了できるようになります。</span><span class="sxs-lookup"><span data-stu-id="7b797-134">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="7b797-135">また、お客様は、現在のパートナーから譲渡するサブスクリプションを特定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b797-135">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="7b797-136">Office 365、Enterprise Mobility Suite、または Microsoft Dynamics CRM サブスクリプションのパートナーを変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="7b797-136">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="7b797-137">譲渡プロセスを開始する転送要求フォームを完了するのは、今後のパートナーの責任です。</span><span class="sxs-lookup"><span data-stu-id="7b797-137">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="7b797-138">Microsoft は、お客様または現在のパートナーに代わって介入することはできません。</span><span class="sxs-lookup"><span data-stu-id="7b797-138">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="7b797-139">お客様は、将来と現在のパートナーと密接に連携して、移行を円滑に進めることを計画する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b797-139">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="7b797-140">今後のパートナータスクの完了</span><span class="sxs-lookup"><span data-stu-id="7b797-140">Future partner tasks to be completed</span></span>

<span data-ttu-id="7b797-141">サブスクリプションの今後のパートナーは、パートナーセンターから譲渡要求フォームを完了して、サブスクリプションの譲渡を要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b797-141">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="7b797-142">パートナーセンターメニューから、[ **顧客**] を選択し、代理で転送要求フォームを完了する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b797-142">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="7b797-143">カスタマーメニューから [ **サブスクリプション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b797-143">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="7b797-144">[ **転送要求** ] セクションを選択します。</span><span class="sxs-lookup"><span data-stu-id="7b797-144">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="7b797-145">[ **転送要求] セクション**で、[ **新しい要求の追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b797-145">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="転送セクション":::

5.  <span data-ttu-id="7b797-147">**新しい転送要求**フォームに入力します。</span><span class="sxs-lookup"><span data-stu-id="7b797-147">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="7b797-148">[**転送要求**の送信] を選択し  >  **Send**ます。</span><span class="sxs-lookup"><span data-stu-id="7b797-148">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="転送セクション":::

7.  <span data-ttu-id="7b797-150">転送要求の確認の確認</span><span class="sxs-lookup"><span data-stu-id="7b797-150">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="転送セクション":::

    >[!Note]
    ><span data-ttu-id="7b797-152">将来のパートナーは、転送要求の状態が [保留中] の場合にのみ、右上隅にある **[要求のキャンセル]** を選択して、譲渡要求を取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="7b797-152">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="7b797-153">転送要求の状態が "進行中" または "完了" になると、取り消しはできなくなります。</span><span class="sxs-lookup"><span data-stu-id="7b797-153">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="7b797-154">完了する現在のパートナータスク</span><span class="sxs-lookup"><span data-stu-id="7b797-154">Current partner tasks to be completed</span></span>

<span data-ttu-id="7b797-155">お客様の現在のパートナーの管理者エージェントは、お客様がサブスクリプションの譲渡を要求しているという電子メールを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="7b797-155">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="転送セクション":::

<span data-ttu-id="7b797-157">パートナーセンターから譲渡要求フォームを確認して同意し、サブスクリプションの譲渡を完了します。</span><span class="sxs-lookup"><span data-stu-id="7b797-157">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="7b797-158">現在のパートナーが30日以内にアクションを実行しなかった場合は、要求の有効期限が切れ、今後のパートナーは新しい転送要求を作成するためにを使用します。</span><span class="sxs-lookup"><span data-stu-id="7b797-158">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="7b797-159">[電子メールからの **転送要求のレビュー** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b797-159">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="7b797-160">パートナーセンターメニューから [ **顧客**] を選択し、譲渡要求が送信された顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b797-160">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="7b797-161">カスタマーメニューから [ **サブスクリプション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b797-161">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="7b797-162">[ **転送要求** ] セクションを選択します。</span><span class="sxs-lookup"><span data-stu-id="7b797-162">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="7b797-163">[**受信した要求**] で選択した**転送要求 ID**を選択して、[転送情報] を展開します。</span><span class="sxs-lookup"><span data-stu-id="7b797-163">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="転送セクション":::

5.  <span data-ttu-id="7b797-165">譲渡要求を確認します。</span><span class="sxs-lookup"><span data-stu-id="7b797-165">Review transfer request.</span></span> <span data-ttu-id="7b797-166">転送する要求された Azure サブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="7b797-166">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="7b797-167">続行する前に、選択したサブスクリプションにアクセスできなくなります。</span><span class="sxs-lookup"><span data-stu-id="7b797-167">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="7b797-168">今後の使用のために請求されることはありません。</span><span class="sxs-lookup"><span data-stu-id="7b797-168">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="7b797-169">Azure の予約は、サブスクリプションと共には転送されません。</span><span class="sxs-lookup"><span data-stu-id="7b797-169">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="7b797-170">次に、[ **受け入れて転送** ] を選択して、転送プロセスを完了します。</span><span class="sxs-lookup"><span data-stu-id="7b797-170">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="転送セクション":::

7.  <span data-ttu-id="7b797-172">転送の受け入れ確認を表示します。</span><span class="sxs-lookup"><span data-stu-id="7b797-172">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="7b797-173">この時点で、今後のパートナー、顧客、および現在のパートナーには、電子メールで受け入れられた譲渡要求が通知されます。</span><span class="sxs-lookup"><span data-stu-id="7b797-173">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="7b797-174">その後、移行が受け入れられると、システムが更新されている間、転送状態が最大15分間保留状態のままになることがあります。</span><span class="sxs-lookup"><span data-stu-id="7b797-174">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="7b797-175">時間がかかると、システムは3日間試行し続けます。</span><span class="sxs-lookup"><span data-stu-id="7b797-175">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="7b797-176">転送の状態が保留中のままである場合、パートナーはサービス要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b797-176">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="7b797-177">転送が完了すると、要求内に含まれているサブスクリプションが、今後のパートナーの Azure プランに表示され、お客様と共に表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="7b797-177">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="7b797-178">間接プロバイダーの場合: 譲渡要求が受け入れられたことを間接リセラーに知らせてください。</span><span class="sxs-lookup"><span data-stu-id="7b797-178">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="7b797-179">転送された顧客サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="7b797-179">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="7b797-180">移転中、Azure ロールベースのアクセス制御 (RBAC) を使用して割り当てられた既存のユーザー、グループ、またはサービス プリンシパルへのアクセスは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="7b797-180">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="7b797-181">Azure のロールベースのアクセス制御 [(AZURE RBAC)](/azure/role-based-access-control/overview) を使用すると、顧客は、azure リソースにアクセスできるユーザー、それらのリソースを使用して実行できること、およびアクセス権を持つ領域を管理できます。</span><span class="sxs-lookup"><span data-stu-id="7b797-181">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="7b797-182">新しいパートナーとして、サブスクリプションの譲渡後に、お客様のリソースに対する RBAC アクセス権は付与されません。</span><span class="sxs-lookup"><span data-stu-id="7b797-182">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="7b797-183">お客様の以前のパートナーは、RBAC アクセスを維持しています。</span><span class="sxs-lookup"><span data-stu-id="7b797-183">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="7b797-184">お客様と協力して、サブスクリプションについての洞察を持つユーザーと、必要な変更を行う方法を理解します。</span><span class="sxs-lookup"><span data-stu-id="7b797-184">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="7b797-185">そのため、お客様は前のパートナー向けの Azure RBAC アクセスを削除し、新しいパートナーのアクセス権を追加することが重要です。</span><span class="sxs-lookup"><span data-stu-id="7b797-185">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="7b797-186">顧客が新しいアクセス権を付与する方法の詳細については、「 [azure のロールベースのアクセス制御 (AZURE RBAC) とは](/azure/role-based-access-control/overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b797-186">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="7b797-187">以前のパートナーの RBAC アクセスを削除する顧客の詳細については、「 [ロールの割り当てを削除する](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b797-187">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="7b797-188">さらに、サブスクリプションへ [の (AOBO) アクセスの代理](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) として自動的に管理者を取得することはありません。</span><span class="sxs-lookup"><span data-stu-id="7b797-188">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="7b797-189">AOBO は、パートナーが顧客の Azure サブスクリプションを代理として管理するために必要です。</span><span class="sxs-lookup"><span data-stu-id="7b797-189">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="7b797-190">Azure の特権の詳細について[は、「顧客のサービスまたはサブスクリプションを管理するためのアクセス許可を取得する](./customers-revoke-admin-privileges.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b797-190">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="7b797-191">次のステップ:</span><span class="sxs-lookup"><span data-stu-id="7b797-191">Next steps:</span></span>

- [<span data-ttu-id="7b797-192">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="7b797-192">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="7b797-193">顧客のサービスまたはサブスクリプションを管理するためのアクセス許可を取得します。</span><span class="sxs-lookup"><span data-stu-id="7b797-193">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)