---
title: お客様が独自のサービスを CSP で購入できるようにする
description: CSP プログラムパートナーが、パートナーセンターで購入したサブスクリプションに対して、Azure の予約などの独自のサービスを購入できるようにする方法について説明します。
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9fabd6bd188c9d596128672d9fce3321db9b5432
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150762"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a><span data-ttu-id="a3578-103">パートナーセンターで自分の製品またはサービスを購入するためのアクセス許可を顧客に付与する</span><span class="sxs-lookup"><span data-stu-id="a3578-103">Give customers permission in Partner Center to buy their own products or services</span></span>

<span data-ttu-id="a3578-104">**適切なロール**: 管理エージェント |営業担当者</span><span class="sxs-lookup"><span data-stu-id="a3578-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="a3578-105">この記事では、クラウドソリューションプロバイダー (CSP) プログラムのパートナーが、独自のサービスまたはリソースの一部を購入するためのアクセス許可を付与する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="a3578-105">This article shows how a partner in the Cloud Solution Provider (CSP) program can give a customer permission to buy some of their own services or resources.</span></span>

<span data-ttu-id="a3578-106">CSP プログラムのパートナーは、多くの場合、パートナーセンターとその商用マーケットプレースを使用して、顧客向けのソリューションとサービスを購入します。</span><span class="sxs-lookup"><span data-stu-id="a3578-106">Partners in the CSP program often use Partner Center and its commercial marketplace to buy solutions and services for their customers.</span></span> <span data-ttu-id="a3578-107">パートナーは、一部のお客様に対して、これらのサービスを Azure portal から直接プロビジョニングすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="a3578-107">Partners then allow some customers to provision these services themselves directly from the Azure portal.</span></span>

<span data-ttu-id="a3578-108">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="a3578-108">Here's an example.</span></span> <span data-ttu-id="a3578-109">たとえば、パートナーセンターで顧客の Azure プランサブスクリプションを購入したとします。</span><span class="sxs-lookup"><span data-stu-id="a3578-109">Let's say you buy an Azure Plan subscription for a customer in Partner Center.</span></span> <span data-ttu-id="a3578-110">その後、顧客の代理として、そのサブスクリプションに他のリソースまたはサービスを追加することを決定します。</span><span class="sxs-lookup"><span data-stu-id="a3578-110">You then decide to add other resources or services to that subscription on the customer's behalf.</span></span> <span data-ttu-id="a3578-111">この場合、顧客のサブスクリプションに Azure の予約を追加することができます (予約済みの仮想マシンインスタンスの追加など)。</span><span class="sxs-lookup"><span data-stu-id="a3578-111">In this case, you might add Azure reservations to the customer's subscription (such as, adding reserved, virtual machine instances).</span></span> <span data-ttu-id="a3578-112">その後、顧客が Azure portal で Azure 予約リソースをさらにプロビジョニングできるようにすることができます。</span><span class="sxs-lookup"><span data-stu-id="a3578-112">You might then allow the customer to further provision the Azure reservation resources themselves in the Azure portal.</span></span>

<span data-ttu-id="a3578-113">これで、 **顧客のアクセス許可** 機能を使用して、Azure リソースでより多くのセルフサービスオプションをお客様に提供できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="a3578-113">Now, with the **Customer permissions** feature, you give customers more self-service options with Azure resources.</span></span> <span data-ttu-id="a3578-114">顧客に対してアクセス許可を有効にすると、顧客は独自のリソース (Azure の予約の購入など) を購入できるようになります。</span><span class="sxs-lookup"><span data-stu-id="a3578-114">By turning on permissions for the customer, you allow customers to buy their own resources (such as, buying their own Azure reservations).</span></span>  

## <a name="overview-of-customer-permissions-in-partner-center"></a><span data-ttu-id="a3578-115">パートナーセンターにおける顧客のアクセス許可の概要</span><span class="sxs-lookup"><span data-stu-id="a3578-115">Overview of customer permissions in Partner Center</span></span>

<span data-ttu-id="a3578-116">[顧客 **アカウント** ] ページを使用して、顧客のアクセス許可をオンまたはオフにします。</span><span class="sxs-lookup"><span data-stu-id="a3578-116">Use the Customer **Account** page to turn on (or turn off) customer permissions.</span></span> <span data-ttu-id="a3578-117">現在、この機能は以下をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="a3578-117">Currently, this feature supports:</span></span>

- <span data-ttu-id="a3578-118">**Azure の予約:** このアクセス許可を有効にすると、顧客は、購入した特定の Azure サブスクリプションに対して独自の Azure 予約を購入できます。</span><span class="sxs-lookup"><span data-stu-id="a3578-118">**Azure reservations:** Turning on this permission allows the customer to purchase their own Azure reservations for a specific Azure subscription you've purchased for them.</span></span>

<span data-ttu-id="a3578-119">カスタマーアクセス許可を有効にする前に、次の重要な点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="a3578-119">Before you turn on customer permissions, note these important points:</span></span>

- <span data-ttu-id="a3578-120">既定では、顧客のアクセス許可は、パートナーセンターで自動的に無効 (オフ) になります。</span><span class="sxs-lookup"><span data-stu-id="a3578-120">By default, customer permissions are automatically disabled (turned off) in Partner Center.</span></span>

- <span data-ttu-id="a3578-121">顧客に対するアクセス許可を有効 (またはオフにする) 前に、顧客の管理エージェントのロールを割り当パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="a3578-121">Before you can turn on (or turn off) permissions for a customer, you must be assigned the role of Admin Agent in Partner Center.</span></span>

  <span data-ttu-id="a3578-122">Sales Agent またはヘルプ デスク エージェントのロールを割り当てられたパートナーは、読み取り専用アクセス権を持ち、顧客のアクセス許可をオンまたはオフにすることはできません。</span><span class="sxs-lookup"><span data-stu-id="a3578-122">Partners assigned the role of Sales Agent or Help Desk Agent have read-only access and can't turn customer permissions on or off.</span></span>

- <span data-ttu-id="a3578-123">選択した顧客に対してアクセス許可を有効 (有効) できます。</span><span class="sxs-lookup"><span data-stu-id="a3578-123">You can turn on (enable) permissions for any customer you choose.</span></span>

- <span data-ttu-id="a3578-124">ダッシュボードまたは API を使用して、顧客のアクセス許可パートナー センター (または [パートナー センターできます](/partner-center/develop/manage-customers)。</span><span class="sxs-lookup"><span data-stu-id="a3578-124">You can turn on (or turn off) customer permissions using either the Partner Center dashboard or [Partner Center APIs](/partner-center/develop/manage-customers).</span></span>

- <span data-ttu-id="a3578-125">特定の顧客に対してアクセス許可を有効 (有効) にした後、その顧客が行った後続の購入に対して支払う責任があります。</span><span class="sxs-lookup"><span data-stu-id="a3578-125">After you turn on (enable) permissions for a specific customer, you will be responsible to pay for any subsequent purchases made by that customer.</span></span> <span data-ttu-id="a3578-126">顧客が行った購入を交換、キャンセル、または更新する (または予約の初期スコープを変更する) 場合、顧客は自身で行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3578-126">If customers want to exchange, cancel or renew a purchase they've made (or they want to change the initial scope of a reservation), they will not be able to do so themselves.</span></span> <span data-ttu-id="a3578-127">パートナーは、購入の交換、キャンセル、更新を支援したり、後で予約のスコープを変更したりするために、パートナーから質問する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3578-127">They need to ask you, as the partner, to help them exchange, cancel, and renew purchases, or make later changes to a reservation's scope.</span></span>  

- <span data-ttu-id="a3578-128">特定の顧客に対するアクセス許可を有効にした後、顧客が行った後の購入は通知されません。</span><span class="sxs-lookup"><span data-stu-id="a3578-128">After you turn on permissions for a specific customer, you will **not be** notified of any later purchases made by the customer.</span></span>

- <span data-ttu-id="a3578-129">顧客が行った後の購入は、パートナー センターによって行われたすべての購入と共に表示されます。</span><span class="sxs-lookup"><span data-stu-id="a3578-129">Later purchases made by the customer will appear in Partner Center along with any purchases made by you.</span></span> <span data-ttu-id="a3578-130">これらの購入は、顧客の注文履歴ページ、予約ページ、またはアクティビティログ で [**確認できます**](activity-logs.md)。</span><span class="sxs-lookup"><span data-stu-id="a3578-130">You can find these purchases on the customer's **Order history** page, their **Reservations** page, or in the [**Activity Log**](activity-logs.md).</span></span>

>[!NOTE]
> <span data-ttu-id="a3578-131">顧客が支払う価格と、顧客が購入を管理する方法については、「顧客が購入した予約を管理する」 [を参照してください](give-customers-permission.md#help-customers-manage-reservations-they-purchase)。</span><span class="sxs-lookup"><span data-stu-id="a3578-131">For information about prices the customer will pay and how to help customers manage their purchases, see [Help customers manage reservations they purchase](give-customers-permission.md#help-customers-manage-reservations-they-purchase).</span></span>

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a><span data-ttu-id="a3578-132">顧客に自分の Azure 予約を購入するアクセス許可を付与する</span><span class="sxs-lookup"><span data-stu-id="a3578-132">Give customers permission to buy their own Azure reservations</span></span>

<span data-ttu-id="a3578-133">Azure Reservations は、Azure サービスを割引料金で購入できる優れた方法です。</span><span class="sxs-lookup"><span data-stu-id="a3578-133">Azure reservations are a great way to buy Azure services at a discounted rate.</span></span> <span data-ttu-id="a3578-134">Azure 予約の利点の詳細については、「Azure の予約 [とは」を参照してください。](/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="a3578-134">To learn more about the benefits of Azure reservations, see [What are Azure Reservations?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span></span>

<span data-ttu-id="a3578-135">これで、既に行っている場合と同様に、顧客に代わって Azure の予約を購入できます。</span><span class="sxs-lookup"><span data-stu-id="a3578-135">Now you have the choice to buy Azure reservations on behalf of your customers, as you may have already been doing.</span></span> <span data-ttu-id="a3578-136">または、独自の Azure 予約を購入するアクセス許可を顧客に付与できます。</span><span class="sxs-lookup"><span data-stu-id="a3578-136">Or, you can give customers permission to buy their own Azure reservations.</span></span>

>[!NOTE]
> <span data-ttu-id="a3578-137">顧客に独自の Azure 予約を購入するアクセス許可を付与した後は、購入した予約を管理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="a3578-137">After you give customers permission to buy their own Azure reservations, help them manage any reservations they purchase.</span></span> <span data-ttu-id="a3578-138">詳細については、「購入した [予約を顧客が管理できるよう](give-customers-permission.md#help-customers-manage-reservations-they-purchase)にする」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3578-138">For more information, see [Help customers manage reservations they purchase](give-customers-permission.md#help-customers-manage-reservations-they-purchase).</span></span>

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a><span data-ttu-id="a3578-139">顧客が独自の Azure 予約を購入できるようにするには</span><span class="sxs-lookup"><span data-stu-id="a3578-139">To enable customers to buy their own Azure reservations</span></span>

1. <span data-ttu-id="a3578-140">顧客に代わって購入した既存の Azure プランまたは Azure グローバルサブスクリプションがあることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a3578-140">Verify the customer has an existing Azure Plan or Azure Global subscription you purchased on their behalf.</span></span>

2. <span data-ttu-id="a3578-141">お客様にこのサブスクリプションの **所有者** ロールが割り当てられていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a3578-141">Verify the customer has been assigned the **Owner** role for this subscription.</span></span>

3. <span data-ttu-id="a3578-142">自分の Azure 予約を購入するには、顧客のアクセス許可を有効にします (こ **の機能を** 有効にします)。</span><span class="sxs-lookup"><span data-stu-id="a3578-142">Enable customer permissions (turn this feature **On**) to purchase their own Azure reservations.</span></span>

<span data-ttu-id="a3578-143">各手順は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="a3578-143">Each step appears below.</span></span>

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a><span data-ttu-id="a3578-144">顧客が既存の Azure サブスクリプションを持っていることを確認する</span><span class="sxs-lookup"><span data-stu-id="a3578-144">Verify the customer has an existing Azure subscription</span></span>

<span data-ttu-id="a3578-145">顧客に独自の Azure 予約を購入するアクセス許可を付与する前に、顧客が既存の Azure プランまたは Azure グローバルサブスクリプションを持っていることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3578-145">Before you give customers permission to buy their own Azure reservations, you must verify the customer has an existing Azure Plan or Azure Global subscription.</span></span> <span data-ttu-id="a3578-146">顧客がパートナーセンターで現在の Azure サブスクリプションを表示していない場合は、顧客のアクセス許可を有効にする前にサブスクリプションを購入する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3578-146">If the customer shows no current Azure subscription in Partner Center, you must buy a subscription for them before you turn on their customer permissions.</span></span>

- <span data-ttu-id="a3578-147">顧客が既に Azure サブスクリプションを持っているかどうかを確認するには、パートナーセンターのダッシュボードにサインインし、[ **CSP** ]、[ **顧客**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="a3578-147">To see if a customer already has an Azure subscription, sign into the Partner Center dashboard, then select **CSP** followed by **Customers**.</span></span> <span data-ttu-id="a3578-148">一覧から特定の顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="a3578-148">Select the specific customer from the list.</span></span> <span data-ttu-id="a3578-149">次に、[ **サブスクリプション** ] を選択し、azure プランまたは azure グローバルのいずれかの使用量ベースのサブスクリプションを検索します。</span><span class="sxs-lookup"><span data-stu-id="a3578-149">Then select **Subscriptions** and look for any usage-based subscriptions for either Azure Plan or Azure Global.</span></span>

- <span data-ttu-id="a3578-150">顧客が既存の Azure サブスクリプションを持っていない場合は、サブスクリプションを購入することができます。</span><span class="sxs-lookup"><span data-stu-id="a3578-150">If a customer doesn't have an existing Azure subscription, you can buy a subscription for them.</span></span> <span data-ttu-id="a3578-151">「 [Azure プランの購入」を](purchase-azure-plan.md)参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3578-151">See [Purchase the Azure Plan](purchase-azure-plan.md).</span></span>

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a><span data-ttu-id="a3578-152">お客様に Azure の正しいロールが割り当てられていることを確認する</span><span class="sxs-lookup"><span data-stu-id="a3578-152">Verify the customer has been assigned the correct role in Azure</span></span>

<span data-ttu-id="a3578-153">顧客が既存の Azure サブスクリプションを持っていることを確認した後、顧客に関連付けられているキーユーザーに、その Azure サブスクリプションの正しい **所有者** ロールが割り当てられていることを確認する必要もあります。</span><span class="sxs-lookup"><span data-stu-id="a3578-153">After you verify the customer has an existing Azure subscription, you also need to verify the key users associated with your customer have been assigned the correct **Owner** role for that Azure subscription.</span></span> <span data-ttu-id="a3578-154">これは、お客様が購入した Azure サブスクリプションの Azure 予約を購入する必要がある、ロールベースのアクセス (RBAC) です。</span><span class="sxs-lookup"><span data-stu-id="a3578-154">This is the role-based access (RBAC) the customer needs to buy Azure reservations for an Azure subscription you purchased.</span></span>

<span data-ttu-id="a3578-155">パートナーによっては、自分の Azure リソースを積極的に管理およびプロビジョニングすることを希望するお客様に、既に **所有者** ロールが割り当てられている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a3578-155">Some partners may have already assigned the **Owner** role to customers wanting to actively manage and provision their own Azure resources.</span></span> <span data-ttu-id="a3578-156">以前に購入したサブスクリプションを管理するために、既に **所有者** の状態を顧客に割り当てている場合は、この手順を省略できます。</span><span class="sxs-lookup"><span data-stu-id="a3578-156">If you have already assigned **Owner** status to a customer to manage prior subscriptions you've purchased for them, you can skip this step.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="a3578-157">**所有者** ロールが割り当てられていない場合、ユーザーは Azure の予約を購入できないように Azure portal にエラーを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="a3578-157">If a customer has not been assigned the **Owner** role, they will receive an error in the Azure portal preventing them from buying Azure reservations.</span></span>

<span data-ttu-id="a3578-158">顧客に Azure サブスクリプションの **所有者** ロールが割り当てられていることを確認するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="a3578-158">To verify the customer has been assigned the **Owner** role for an Azure subscription:</span></span>

1. <span data-ttu-id="a3578-159">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="a3578-159">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a3578-160">[ **CSP**]、[ **顧客** ] の順に選択し、特定の顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="a3578-160">Select **CSP**, then **Customers** and select the specific customer.</span></span>

3. <span data-ttu-id="a3578-161">その顧客の **サブスクリプション** を選択し、特定の Azure サブスクリプションを見つけます。</span><span class="sxs-lookup"><span data-stu-id="a3578-161">Select **Subscriptions** for that customer and locate the specific Azure subscription.</span></span>

4. <span data-ttu-id="a3578-162">その顧客のサブスクリプションの横にある [ **管理** ] ボタンを選択します。</span><span class="sxs-lookup"><span data-stu-id="a3578-162">Select the **Manage** button next to that customer's subscription.</span></span> <span data-ttu-id="a3578-163">これにより、 [Azure portal](https://portal.azure.com/)が開きます。</span><span class="sxs-lookup"><span data-stu-id="a3578-163">Doing so opens the [Azure portal](https://portal.azure.com/).</span></span>

5. <span data-ttu-id="a3578-164">特定のユーザーに **所有者** ロールを割り当てるには、次の手順に従っ [て、管理者としてユーザーを割り当て](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)ます。</span><span class="sxs-lookup"><span data-stu-id="a3578-164">To assign the **Owner** role to a specific user, follow these steps [To assign a user as an administrator](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).</span></span>

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a><span data-ttu-id="a3578-165">独自の Azure 予約を購入するには、顧客のアクセス許可をオンまたはオフにします</span><span class="sxs-lookup"><span data-stu-id="a3578-165">Turn on or turn off customer permissions to purchase their own Azure reservations</span></span>

<span data-ttu-id="a3578-166">顧客に既存の Azure サブスクリプションがあることを確認し、ユーザーにそのサブスクリプションの **所有者** ロールが割り当てられていることを確認したら、顧客のアクセス許可を有効にする (有効にする) ことができます。</span><span class="sxs-lookup"><span data-stu-id="a3578-166">After you verify the customer has an existing Azure subscription and users are assigned the **Owner** role for that subscription, you're ready to turn on (enable) customer permissions.</span></span> <span data-ttu-id="a3578-167">また、これらの手順を使用して、顧客のアクセス許可をオフ (無効) にすることもできます。</span><span class="sxs-lookup"><span data-stu-id="a3578-167">You can also use these steps to turn off (disable) customer permissions.</span></span> <span data-ttu-id="a3578-168">パートナーセンターのダッシュボードまたは [パートナーセンター api](/partner-center/develop/manage-customers)を使用して、顧客のアクセス許可を有効または無効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a3578-168">You can enable or disable customer permissions using either the Partner Center dashboard or [Partner Center APIs](/partner-center/develop/manage-customers).</span></span>

<span data-ttu-id="a3578-169">パートナーセンターで顧客のアクセス許可をオンまたはオフにするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="a3578-169">To turn on (or turn off) customer permissions in Partner Center:</span></span>

1. <span data-ttu-id="a3578-170">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="a3578-170">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a3578-171">左側のナビゲーションメニューで、[ **CSP**]、[ **Customers**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="a3578-171">From the left navigation menu, select **CSP**, then **Customers**.</span></span> <span data-ttu-id="a3578-172">顧客リストが表示されます。</span><span class="sxs-lookup"><span data-stu-id="a3578-172">A customer list appears.</span></span>

3. <span data-ttu-id="a3578-173">特定の顧客名を選択します。</span><span class="sxs-lookup"><span data-stu-id="a3578-173">Select a specific customer name.</span></span>

4. <span data-ttu-id="a3578-174">[Customer] メニューから [ **Account** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a3578-174">Select **Account** from the customer menu.</span></span> <span data-ttu-id="a3578-175">[顧客 **アカウント** ] ページが表示されます。</span><span class="sxs-lookup"><span data-stu-id="a3578-175">The customer **Account** page appears.</span></span>

5. <span data-ttu-id="a3578-176">ページの下部にある [ **顧客のアクセス許可** ] 領域を探します。</span><span class="sxs-lookup"><span data-stu-id="a3578-176">Locate the **Customer permissions** area at the bottom of the page.</span></span>

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="アカウントページに対する顧客のアクセス許可。" border="true":::

6. <span data-ttu-id="a3578-178">[ **Azure の予約**] で、[ **顧客の購入を許可する** ] オプションを見つけます。</span><span class="sxs-lookup"><span data-stu-id="a3578-178">Under **Azure reservations**, locate the **Allow customer to purchase** option.</span></span>

7. <span data-ttu-id="a3578-179">顧客のアクセス許可を有効にする場合は、このオプションの横にあるスイッチを [オン] の位置 **に移動** します。</span><span class="sxs-lookup"><span data-stu-id="a3578-179">To turn on customer permissions, move the switch next to this option to the **On** position.</span></span> <span data-ttu-id="a3578-180">顧客のアクセス許可をオフにする場合は、スイッチを [オフ] の位置 **に移動** します。</span><span class="sxs-lookup"><span data-stu-id="a3578-180">To turn off customer permissions, move the switch to the **Off** position.</span></span>

>[!NOTE]
> <span data-ttu-id="a3578-181">独自の Azure 予約を購入するための顧客のアクセス許可をオンにした場合のその他の問題については、「パートナー センター での顧客のアクセス許可の [概要」を参照してください](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)。</span><span class="sxs-lookup"><span data-stu-id="a3578-181">To learn what else happens when you turn on a customer's permissions to purchase their own Azure reservations, see [Overview of customer permissions in Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).</span></span>
>
><span data-ttu-id="a3578-182">顧客のアクセス許可を有効 (またはオフ) すると、アクティビティ ログに各アクションが記録されます。</span><span class="sxs-lookup"><span data-stu-id="a3578-182">When you turn on (or turn off) customer permissions, the Activity log records each action.</span></span> <span data-ttu-id="a3578-183">(このログには、ダッシュボードの上部にある [歯車] アイコンを選択パートナー センターできます)。</span><span class="sxs-lookup"><span data-stu-id="a3578-183">(This log is accessible when you select the Gear icon from the top of the Partner Center dashboard).</span></span> <span data-ttu-id="a3578-184">顧客のアクセス許可をオンまたはオフにした場合、アクションはアクティビティログに [顧客購入アクセス許可の作成] または [顧客購入アクセス許可の **削除]** として表示されます。</span><span class="sxs-lookup"><span data-stu-id="a3578-184">When you turn customer permissions on or off, the action will appear as either **Create Customer Purchase Permissions** or **Delete Customer Purchase Permissions** in the Activity log.</span></span>

## <a name="help-customers-manage-reservations-they-purchase"></a><span data-ttu-id="a3578-185">顧客が購入した予約の管理を支援する</span><span class="sxs-lookup"><span data-stu-id="a3578-185">Help customers manage reservations they purchase</span></span>

<span data-ttu-id="a3578-186">顧客に独自の Azure 予約を購入するアクセス許可を付与すると、購入したリソースの管理を向上できます。</span><span class="sxs-lookup"><span data-stu-id="a3578-186">Once you give customers permission to purchase their own Azure reservations, you can help them better manage any resources they purchase.</span></span> <span data-ttu-id="a3578-187">お客様は、Azure の予約の多くの側面を、 から直接管理[Azure portal。](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="a3578-187">Customers can manage many aspects of Azure reservations themselves directly from the [Azure portal](https://portal.azure.com/).</span></span> <span data-ttu-id="a3578-188">CSP サブスクリプション内で購入した Azure 予約の他のいくつかの側面を管理する際に、支援が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3578-188">They will need your help managing a few, other aspects of Azure reservations they purchase within your CSP subscription.</span></span>  

<span data-ttu-id="a3578-189">Azure の予約のこれらの側面の管理について、お客様が理解を得る助けとなります。</span><span class="sxs-lookup"><span data-stu-id="a3578-189">Help customers understand more about managing these aspects of Azure reservations:</span></span>

- <span data-ttu-id="a3578-190">顧客が Azure の予約に対して支払う価格</span><span class="sxs-lookup"><span data-stu-id="a3578-190">Prices customers will pay for Azure reservations</span></span>
- <span data-ttu-id="a3578-191">お客様が Azure 予約の使用を最適化する方法</span><span class="sxs-lookup"><span data-stu-id="a3578-191">How customers can optimize use of Azure reservations</span></span>
- <span data-ttu-id="a3578-192">顧客が共有スコープで予約を購入するとどうなるか。</span><span class="sxs-lookup"><span data-stu-id="a3578-192">What happens when customers purchase reservations with a shared scope?</span></span>
- <span data-ttu-id="a3578-193">顧客が予約を変更、キャンセル、更新する場合、またはスコープを変更する場合は、どうなるでしょうか。</span><span class="sxs-lookup"><span data-stu-id="a3578-193">What happens if customers want to change, cancel, and renew a reservation, or change its scope?</span></span>

<span data-ttu-id="a3578-194">**顧客が予約の料金を支払う価格。**</span><span class="sxs-lookup"><span data-stu-id="a3578-194">**Prices customers will pay for their reservations.**</span></span> <span data-ttu-id="a3578-195">顧客は、CSP パートナーの請求先アカウントで以前に購入したサブスクリプションに基づいて Azure の予約を購入します。</span><span class="sxs-lookup"><span data-stu-id="a3578-195">Your customer will be purchasing Azure reservations based on a subscription you previously bought for them in your CSP partner billing account.</span></span> <span data-ttu-id="a3578-196">このサブスクリプションに基づいて購入した Azure 予約に対する顧客の価格もユーザーによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="a3578-196">The customer's price for any Azure reservations they purchase based on this subscription is also set by you.</span></span> <span data-ttu-id="a3578-197">この価格は、顧客が顧客に表示される Web Direct の価格とは異なる場合Azure portal。</span><span class="sxs-lookup"><span data-stu-id="a3578-197">This price may be different from the Web Direct price the customer sees in the Azure portal.</span></span>

<span data-ttu-id="a3578-198">**顧客が予約の使用を最適化する方法。**</span><span class="sxs-lookup"><span data-stu-id="a3578-198">**How customers can optimize their use of a reservation.**</span></span> <span data-ttu-id="a3578-199">お客様によっては、予約の使用を最適化する方法、または購入時に予約の初期スコープを割り当てる方法について、さらに学習することができます。</span><span class="sxs-lookup"><span data-stu-id="a3578-199">Some customers might benefit from learning more about how to optimize their use of a reservation or how to assign a reservation’s initial scope during their purchase.</span></span> <span data-ttu-id="a3578-200">詳細については、「 [Azure リソースの予約を管理](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)する」をお読みください。</span><span class="sxs-lookup"><span data-stu-id="a3578-200">For more information, ask customers to read [Manage reservations for Azure resources](/azure/cost-management-billing/reservations/manage-reserved-vm-instance).</span></span>

<span data-ttu-id="a3578-201">**顧客が共有スコープで予約を購入するとどうなりますか。**</span><span class="sxs-lookup"><span data-stu-id="a3578-201">**What happens when a customer purchases a reservation with a shared scope?**</span></span> <span data-ttu-id="a3578-202">顧客が以前の CSP サブスクリプションに基づいて予約を購入し、その予約に共有スコープを割り当てると、CSP によって顧客に与えられた割引は、CSP パートナーがその顧客に対して購入したすべてのサブスクリプションの照合の使用に適用されます。</span><span class="sxs-lookup"><span data-stu-id="a3578-202">When customers purchase a reservation based on a prior CSP subscription and assign a shared scope to that reservation, any discounts the customer has been given by the CSP will apply to matching usage for all subscriptions the CSP partner has purchased for that customer.</span></span>

<span data-ttu-id="a3578-203">**顧客が購入を交換、キャンセル、または更新する場合や、予約の初期スコープを変更する場合は、どうすればよいでしょうか。**</span><span class="sxs-lookup"><span data-stu-id="a3578-203">**What should customers do if they want to exchange, cancel, or renew a purchase they have made, or change the initial scope of a reservation?**</span></span> <span data-ttu-id="a3578-204">お客様は、予約の初期スコープを変更するためにパートナーに依頼する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3578-204">Customers need to ask their partner to help them change a reservation's initial scope.</span></span> <span data-ttu-id="a3578-205">また、予約を交換、取り消し、または更新するためのパートナーの支援も必要です。</span><span class="sxs-lookup"><span data-stu-id="a3578-205">They also need a partner's help to exchange, cancel, or renew a reservation.</span></span> <span data-ttu-id="a3578-206">これらのタスクは、CSP パートナーによって購入されたサブスクリプションに基づいて、予約を使用して実行することはできません。</span><span class="sxs-lookup"><span data-stu-id="a3578-206">They cannot perform these tasks themselves with reservations based on subscriptions purchased for them by a CSP partner.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a3578-207">次のステップ</span><span class="sxs-lookup"><span data-stu-id="a3578-207">Next steps</span></span>

- [<span data-ttu-id="a3578-208">顧客に代わって Azure の予約を購入する</span><span class="sxs-lookup"><span data-stu-id="a3578-208">Buy Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)

- [<span data-ttu-id="a3578-209">パートナーセンター-Microsoft 予約の販売</span><span class="sxs-lookup"><span data-stu-id="a3578-209">Partner Center - Sell Microsoft reservations</span></span>](azure-reservations.md)

- [<span data-ttu-id="a3578-210">顧客に代わって Azure Reservations を管理する</span><span class="sxs-lookup"><span data-stu-id="a3578-210">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)