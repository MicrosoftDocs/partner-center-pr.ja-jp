---
title: Azure プランで Azure サブスクリプションを別の CSP パートナーに譲渡する
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure プランで、クラウド ソリューション プロバイダーの Azure サブスクリプションに関連付けられているプログラム パートナーを変更する方法について説明します。
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 092c76fb874eb7308bdb69503223f722657db957
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277319"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="09636-103">顧客の Azure プラン サブスクリプションの別のパートナーへの譲渡</span><span class="sxs-lookup"><span data-stu-id="09636-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="09636-104">**適切なロール**: アカウント管理者|Sales Agent |課金エージェント</span><span class="sxs-lookup"><span data-stu-id="09636-104">**Appropriate roles**: Account admin | Sales agent | Billing agent</span></span>

<span data-ttu-id="09636-105">この記事では、顧客が Azure プランで Azure サブスクリプションを 1 つのサブスクリプション (CSP) クラウド ソリューション プロバイダー切り替える方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="09636-105">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="09636-106">顧客の Azure サブスクリプションを別のパートナーから切り替えるには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="09636-106">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="09636-107">パートナーと顧客の両方に、完了する手順があります。</span><span class="sxs-lookup"><span data-stu-id="09636-107">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="09636-108">移行ツールにアクセスできるのは、Microsoft との直接請求関係を持つパートナーのみです。</span><span class="sxs-lookup"><span data-stu-id="09636-108">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="09636-109">間接リセラーは、この移行ツールを利用するために間接プロバイダーと一緒に作業する必要があります。</span><span class="sxs-lookup"><span data-stu-id="09636-109">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="09636-110">このツールを利用する前に、顧客は両方のパートナー (現在と将来) と会話している必要があります。</span><span class="sxs-lookup"><span data-stu-id="09636-110">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="09636-111">混乱やチャーンを避けるためには、オフラインの会話を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="09636-111">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="09636-112">さらに、パートナーと顧客は、移行を開始する前に、次の考慮事項と前提条件を理解する必要があります。</span><span class="sxs-lookup"><span data-stu-id="09636-112">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="09636-113">**主な考慮事項:**</span><span class="sxs-lookup"><span data-stu-id="09636-113">**Key considerations:**</span></span>

- <span data-ttu-id="09636-114">Azure の予約は、今後のパートナーにサブスクリプションと一緒に移動しない</span><span class="sxs-lookup"><span data-stu-id="09636-114">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="09636-115">現在のパートナーの Azure サービスの CSP 価格は切り替えされない</span><span class="sxs-lookup"><span data-stu-id="09636-115">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="09636-116">お客様に対するサポート責任は、将来のパートナーに移行します</span><span class="sxs-lookup"><span data-stu-id="09636-116">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="09636-117">請求と請求は、転送時に将来のパートナーに移行されます</span><span class="sxs-lookup"><span data-stu-id="09636-117">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="09636-118">Azure Role-Based Access Control (RBAC) は転送の影響を受けない</span><span class="sxs-lookup"><span data-stu-id="09636-118">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="09636-119">代理管理者 (AOBO) は、既定では将来のパートナーに付与されません</span><span class="sxs-lookup"><span data-stu-id="09636-119">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="09636-120">サード パーティのマーケットプレース製品は、製品が Marketplace の適格性チェックに合格している限り転送されます。</span><span class="sxs-lookup"><span data-stu-id="09636-120">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="09636-121">特別な割引や地域の制限はありません</span><span class="sxs-lookup"><span data-stu-id="09636-121">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="09636-122">製品は非サブスクリプション ベースです</span><span class="sxs-lookup"><span data-stu-id="09636-122">The products are non-subscription based</span></span>
    - <span data-ttu-id="09636-123">将来のパートナーは、発行元と一緒に、製品の展開の許可リストに記載されている必要があります</span><span class="sxs-lookup"><span data-stu-id="09636-123">The future partner should work with the publisher to make sure they are on the allow list for deployment of the product</span></span>
    - <span data-ttu-id="09636-124">Marketplace 製品を譲渡するためにこれらの条件のすべてが満たされない場合は、取り消し、Azure サブスクリプションを譲渡してから、新しいパートナーと Marketplace 製品を再購入する必要があります</span><span class="sxs-lookup"><span data-stu-id="09636-124">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="09636-125">**前提条件:**</span><span class="sxs-lookup"><span data-stu-id="09636-125">**Prerequisites:**</span></span>

- <span data-ttu-id="09636-126">お客様は、移行の意図について現在の CSP パートナーと関わる</span><span class="sxs-lookup"><span data-stu-id="09636-126">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="09636-127">将来の CSP パートナーが顧客と提携し、顧客のニーズを満たすことができます</span><span class="sxs-lookup"><span data-stu-id="09636-127">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="09636-128">将来の CSP パートナーが顧客との関係を確立し、移行を開始する前に Azure プランを購入する</span><span class="sxs-lookup"><span data-stu-id="09636-128">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="09636-129">顧客は、将来の CSP Microsoft 顧客契約してサインインする必要があります</span><span class="sxs-lookup"><span data-stu-id="09636-129">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="09636-130">将来の CSP パートナーは、このツールを使用するためにMicrosoft Partner Agreement署名している必要があります</span><span class="sxs-lookup"><span data-stu-id="09636-130">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="09636-131">完了する顧客のタスク</span><span class="sxs-lookup"><span data-stu-id="09636-131">Customer tasks to be completed</span></span>

<span data-ttu-id="09636-132">Azure プランで Azure サブスクリプションを譲渡するには、顧客は現在のパートナーに連絡してプロセスを開始する必要があります。</span><span class="sxs-lookup"><span data-stu-id="09636-132">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="09636-133">将来のパートナーが代理で譲渡要求フォームを完了できるよう、現在のパートナーの会社名とドメインを収集する必要があります。</span><span class="sxs-lookup"><span data-stu-id="09636-133">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="09636-134">顧客は、現在のパートナーから譲渡するサブスクリプションも特定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="09636-134">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="09636-135">Office 365、Enterprise Mobility Suite、または Microsoft Dynamics CRM サブスクリプションのパートナーを変更できない。</span><span class="sxs-lookup"><span data-stu-id="09636-135">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="09636-136">譲渡プロセスを開始する譲渡要求フォームを完了する責任は、将来のパートナーの責任です。</span><span class="sxs-lookup"><span data-stu-id="09636-136">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="09636-137">Microsoft は、お客様または現在のパートナーに代わって介入することはできません。</span><span class="sxs-lookup"><span data-stu-id="09636-137">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="09636-138">顧客は、移行を円滑に進め、将来および現在のパートナーと密接に取り組む予定です。</span><span class="sxs-lookup"><span data-stu-id="09636-138">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="09636-139">今後のパートナー タスクの完了</span><span class="sxs-lookup"><span data-stu-id="09636-139">Future partner tasks to be completed</span></span>

<span data-ttu-id="09636-140">サブスクリプションの将来のパートナーは、サブスクリプションの譲渡を要求するために、パートナー センターから譲渡要求フォームを完了する必要があります。</span><span class="sxs-lookup"><span data-stu-id="09636-140">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="09636-141">[顧客] パートナー センター [顧客] を選択し、代理で譲渡要求フォームに入力する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="09636-141">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="09636-142">[顧客] メニューの [サブスクリプション] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="09636-142">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="09636-143">[要求の **転送] セクションを** 選択します。</span><span class="sxs-lookup"><span data-stu-id="09636-143">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="09636-144">[要求の転送 **] セクションで、[新** しい要求の **追加] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="09636-144">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="[転送] セクション。":::

5.  <span data-ttu-id="09636-146">[新しい **転送要求] フォームに入力** します。</span><span class="sxs-lookup"><span data-stu-id="09636-146">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="09636-147">[転送要求 **の送信] を**  >  **選択します**。</span><span class="sxs-lookup"><span data-stu-id="09636-147">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="完全な転送要求フォーム。":::

7.  <span data-ttu-id="09636-149">転送要求の確認の確認</span><span class="sxs-lookup"><span data-stu-id="09636-149">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="保留中の転送を確認します。":::

    >[!Note]
    ><span data-ttu-id="09636-151">今後のパートナーは、転送要求の状態が"保留中" の場合にのみ、右上隅にある [キャンセル要求] を選択して、転送要求を取り消します。</span><span class="sxs-lookup"><span data-stu-id="09636-151">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="09636-152">転送要求の状態が "進行中" または "完了" の場合、取り消しはできません。</span><span class="sxs-lookup"><span data-stu-id="09636-152">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="09636-153">完了する現在のパートナー タスク</span><span class="sxs-lookup"><span data-stu-id="09636-153">Current partner tasks to be completed</span></span>

<span data-ttu-id="09636-154">顧客の現在のパートナーの管理エージェントは、顧客がサブスクリプションの譲渡を要求しているという電子メールを受け取る:</span><span class="sxs-lookup"><span data-stu-id="09636-154">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="レビュー。":::

<span data-ttu-id="09636-156">サブスクリプションの譲渡を完了するには、パートナー センター要求フォームを確認して同意します。</span><span class="sxs-lookup"><span data-stu-id="09636-156">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="09636-157">現在のパートナーが 30 日以内にアクションを実行した場合、要求は期限切れになります。今後のパートナーは、新しい譲渡要求を作成する を持つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="09636-157">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="09636-158">電子メール **から [転送要求の** 確認] を選択するか、</span><span class="sxs-lookup"><span data-stu-id="09636-158">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="09636-159">[顧客] パートナー センター [顧客]を選択し、転送要求が代理で送信された顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="09636-159">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="09636-160">[顧客] メニューの [サブスクリプション] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="09636-160">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="09636-161">[要求の **転送] セクションを** 選択します。</span><span class="sxs-lookup"><span data-stu-id="09636-161">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="09636-162">[受信した要求] で選択した転送要求 ID を **選択して** 、転送 **情報を展開します**</span><span class="sxs-lookup"><span data-stu-id="09636-162">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="ソース レビュー転送要求。":::

5.  <span data-ttu-id="09636-164">転送要求を確認します。</span><span class="sxs-lookup"><span data-stu-id="09636-164">Review transfer request.</span></span> <span data-ttu-id="09636-165">転送する要求された Azure サブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="09636-165">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="09636-166">次に進む前に注意してください。選択したサブスクリプションにアクセスできなくなりました。</span><span class="sxs-lookup"><span data-stu-id="09636-166">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="09636-167">それ以上の使用量については請求されません。</span><span class="sxs-lookup"><span data-stu-id="09636-167">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="09636-168">Azure の予約は、サブスクリプションと一緒に譲渡されるのではありません。</span><span class="sxs-lookup"><span data-stu-id="09636-168">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="09636-169">次に、[ **同意して転送] を選択** して転送プロセスを完了します。</span><span class="sxs-lookup"><span data-stu-id="09636-169">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Azure プランで譲渡するサブスクリプションを選択します。":::

7.  <span data-ttu-id="09636-171">譲渡同意の確認を表示します。</span><span class="sxs-lookup"><span data-stu-id="09636-171">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="09636-172">この時点で、将来のパートナー、顧客、および現在のパートナーには、受け入れされた譲渡要求が電子メールで通知されます。</span><span class="sxs-lookup"><span data-stu-id="09636-172">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="09636-173">移行が受け入れられると、システムが更新されている間、転送状態は最大 15 分間保留中のままになる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="09636-173">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="09636-174">時間がかかる場合、システムは 3 日間試し続ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="09636-174">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="09636-175">転送の状態が [保留中] のままである場合、パートナーはサービス要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="09636-175">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="09636-176">譲渡が完了すると、要求に含まれるサブスクリプションが将来のパートナーの Azure プランに表示され、一覧に表示されなくなりました。</span><span class="sxs-lookup"><span data-stu-id="09636-176">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="09636-177">間接プロバイダーの場合: 譲渡要求が受け入れられると間接リセラーに通知してください。</span><span class="sxs-lookup"><span data-stu-id="09636-177">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="09636-178">譲渡された顧客サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="09636-178">Managing your transferred customer subscriptions</span></span>

- <span data-ttu-id="09636-179">移転中、Azure ロールベースのアクセス制御 (RBAC) を使用して割り当てられた既存のユーザー、グループ、またはサービス プリンシパルへのアクセスは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="09636-179">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="09636-180">Azure ロールベースのアクセス制御 [(Azure RBAC)](/azure/role-based-access-control/overview) は、Azure リソースにアクセスできるユーザー、それらのリソースで実行できる操作、およびユーザーがアクセスできる領域を顧客が管理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="09636-180">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="09636-181">新しいパートナーとして、サブスクリプションの譲渡後に顧客のリソースへの RBAC アクセス権は付与されない。</span><span class="sxs-lookup"><span data-stu-id="09636-181">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="09636-182">顧客の前のパートナーは、RBAC アクセス権を保持します。</span><span class="sxs-lookup"><span data-stu-id="09636-182">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="09636-183">顧客と一緒に、サブスクリプションに関する分析情報を持つユーザーと、必要な変更を行う方法を理解します。</span><span class="sxs-lookup"><span data-stu-id="09636-183">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="09636-184">そのため、顧客が前のパートナーの Azure RBAC アクセスを削除し、新しいパートナーのアクセス権を追加することが重要です。</span><span class="sxs-lookup"><span data-stu-id="09636-184">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="09636-185">新しいアクセス権を付与する顧客の詳細については、「Azure ロールベースのアクセス制御 [(Azure RBAC) とは」を参照してください。](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="09636-185">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="09636-186">顧客が以前のパートナーの RBAC アクセスを削除する方法の詳細については、「ロールの割り当てを削除 [する」を参照してください](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)。</span><span class="sxs-lookup"><span data-stu-id="09636-186">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="09636-187">さらに、サブスクリプションへの代理管理者 [(AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) アクセス権は自動的に取得されません。</span><span class="sxs-lookup"><span data-stu-id="09636-187">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="09636-188">パートナーが顧客に代わって顧客の Azure サブスクリプションを管理するには、AOBO が必要です。</span><span class="sxs-lookup"><span data-stu-id="09636-188">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="09636-189">Azure の特権の詳細については、「顧客のサービスまたはサブスクリプションを管理するためのアクセス許可を [取得する」を参照してください。](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="09636-189">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="09636-190">次のステップ:</span><span class="sxs-lookup"><span data-stu-id="09636-190">Next steps:</span></span>

- [<span data-ttu-id="09636-191">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="09636-191">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="09636-192">顧客のサービスまたはサブスクリプションを管理するためのアクセス許可を取得します。</span><span class="sxs-lookup"><span data-stu-id="09636-192">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
