---
title: Azure プラン - サブスクリプションとリソースの管理
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーがさまざまなロールベースのアクセス制御 (RBAC) オプションを使用して、顧客の Azure リソースの運用上の制御と管理を実現する方法について説明します。
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 31e9c6862a5aa19407fa6da5e15333bb7e696720
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534932"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a><span data-ttu-id="b0e98-103">Azure プランのサブスクリプションとリソースを管理する</span><span class="sxs-lookup"><span data-stu-id="b0e98-103">Manage subscriptions and resources under the Azure plan</span></span>

<span data-ttu-id="b0e98-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="b0e98-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b0e98-105">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="b0e98-105">Admin agent</span></span>


<span data-ttu-id="b0e98-106">この記事では、CSP パートナーがさまざまなロールベースのアクセス制御 (RBAC) オプションを使用して、顧客の Azure リソースの運用上の制御と管理を実現する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="b0e98-106">This article explains how CSP partners can use different role-based access control (RBAC) options to gain operational control and management of a customer's Azure resources.</span></span> <span data-ttu-id="b0e98-107">パートナーは、顧客を Azure プランに移行すると、既定では Azure の特権管理者権限 (代理管理者によるサブスクリプション所有者権限) が割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="b0e98-107">When you transition a customer to the Azure plan, you are assigned privileged admin rights in Azure (subscription owner rights through admin on behalf of) by default.</span></span>

 > [!NOTE]
 > <span data-ttu-id="b0e98-108">Azure サブスクリプションに対する管理者権限は、サブスクリプション、リソース グループ、またはワークロード レベルで顧客が削除できます。</span><span class="sxs-lookup"><span data-stu-id="b0e98-108">Admin rights to the Azure subscription can be removed by the customer at a subscription, resource group, or workload level.</span></span> 

 <span data-ttu-id="b0e98-109">パートナーは、CSP で、ロールベースのアクセス制御機能 (RBAC) によって提供されるさまざまなオプションを使用して、顧客の Azure リソースを 24 時間体制で制御し、管理することができます。</span><span class="sxs-lookup"><span data-stu-id="b0e98-109">Partners can gain 24x7 operational control and management of a customer's Azure resources in CSP by using different options provided through the role-based access control feature (RBAC).</span></span> 

- <span data-ttu-id="b0e98-110">**代理管理者 (AOBO)** - [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) では、パートナー テナントの管理者エージェント ロールを持つすべてのユーザーに、CSP プログラムを使用して作成した Azure サブスクリプションに対する RBAC 所有者のアクセス権が付与されます。</span><span class="sxs-lookup"><span data-stu-id="b0e98-110">**Admin on Behalf Of (AOBO)** - With [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO), any user with the Admin Agent role in the partner tenant will have RBAC owner access to Azure subscriptions that you create through the CSP program.</span></span>

- <span data-ttu-id="b0e98-111">**Azure Lighthouse**:AOBO では、複数の顧客と連携する個別のグループを柔軟に作成したり、グループやユーザーに対して複数のロールを有効にしたりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="b0e98-111">**Azure Lighthouse**: AOBO doesn't allow the flexibility to create distinct groups that work with different customers, or to enable different roles for groups or users.</span></span> <span data-ttu-id="b0e98-112">Azure Lighthouse を使用すると、複数のグループを複数の顧客またはロールに割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="b0e98-112">Using Azure Lighthouse, you can assign different groups to different customers or roles.</span></span> <span data-ttu-id="b0e98-113">Azure の委任されたリソース管理によって、ユーザーには適切なレベルのアクセス権が付与されるため、管理者エージェント ロールを持つ (つまり、AOBO のフル アクセス権を持つ) ユーザーの数を減らすことができます。</span><span class="sxs-lookup"><span data-stu-id="b0e98-113">Because users will have the appropriate level of access through Azure delegated resource management, you can reduce the number of users who have the Admin Agent role (and thus have full AOBO access).</span></span> <span data-ttu-id="b0e98-114">これにより、顧客のリソースへの不要なアクセスが制限され、セキュリティを向上させることができます。</span><span class="sxs-lookup"><span data-stu-id="b0e98-114">This helps improve security by limiting unnecessary access to your customers' resources.</span></span> <span data-ttu-id="b0e98-115">また、大規模な複数の顧客をより柔軟に管理できます。</span><span class="sxs-lookup"><span data-stu-id="b0e98-115">It also gives you more flexibility to manage multiple customers at scale.</span></span> <span data-ttu-id="b0e98-116">詳細については、「[Azure Lighthouse と Cloud Solution Provider プログラム](/azure/lighthouse/concepts/cloud-solution-provider)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0e98-116">For more information, read [Azure Lighthouse and the Cloud Solution Provider program](/azure/lighthouse/concepts/cloud-solution-provider).</span></span>

- <span data-ttu-id="b0e98-117">**ディレクトリまたはゲスト ユーザーまたは [サービス プリンシパル](/azure/active-directory/develop/app-objects-and-service-principals)** :CSP サブスクリプションへの詳細なアクセス権を委任するには、顧客のディレクトリにユーザーを追加するか、ゲスト ユーザーを追加して特定の RBAC ロールを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="b0e98-117">**Directory or Guest Users or [Service Principals](/azure/active-directory/develop/app-objects-and-service-principals)**: You can delegate granular access to CSP subscriptions by adding users in the customer directory or adding guest users and assigning specific RBAC roles.</span></span>

<span data-ttu-id="b0e98-118">セキュリティ対策として、作業を実行するために必要な最小限のアクセス許可をユーザーに付与することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="b0e98-118">Microsoft recommends that users have the minimum permissions they need to perform their work as a security practice.</span></span> <span data-ttu-id="b0e98-119">[Azure Active Directory Privileged Identity Management リソース](/azure/active-directory/privileged-identity-management/pim-configure)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0e98-119">See [Azure Active Directory Privileged Identity Management resources](/azure/active-directory/privileged-identity-management/pim-configure).</span></span>

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a><span data-ttu-id="b0e98-120">顧客の Azure リソースを管理するためにパートナー ID (MPN ID) を自分の資格情報にリンクする</span><span class="sxs-lookup"><span data-stu-id="b0e98-120">Link your partner ID (MPN ID)to your credentials for managing customer's Azure resources</span></span>

<span data-ttu-id="b0e98-121">次の表は、パートナー ID をさまざまな RBAC アクセス オプションに関連付けるために使用する方法をまとめたものです。</span><span class="sxs-lookup"><span data-stu-id="b0e98-121">The following table shows the methods used to associate your partner ID with various RBAC access options.</span></span>

|<span data-ttu-id="b0e98-122">**カテゴリ**</span><span class="sxs-lookup"><span data-stu-id="b0e98-122">**Category**</span></span>   |<span data-ttu-id="b0e98-123">**シナリオ**</span><span class="sxs-lookup"><span data-stu-id="b0e98-123">**Scenario**</span></span>   |<span data-ttu-id="b0e98-124">**MPN ID の関連付け**</span><span class="sxs-lookup"><span data-stu-id="b0e98-124">**MPN ID association**</span></span>|
|-----------------|:------------------------|:------------------|
|<span data-ttu-id="b0e98-125">AOBO</span><span class="sxs-lookup"><span data-stu-id="b0e98-125">AOBO</span></span>   |<span data-ttu-id="b0e98-126">CSP ダイレクト パートナーまたはインダイレクト プロバイダーは、AOBO を使用して、CSP ダイレクト パートナーまたはインダイレクト プロバイダーをサブスクリプションの既定の所有者にする顧客のサブスクリプションを作成します。CSP のダイレクト パートナーまたはインダイレクト プロバイダーは、AOBO を使用して、サブスクリプションへのアクセス権をインダイレクト リセラーに付与します。</span><span class="sxs-lookup"><span data-stu-id="b0e98-126">CSP direct partner or indirect provider creates the subscription for the customer making the CSP direct partner or indirect provider default owner of the subscription using AOBO.; CSP direct partner or indirect provider give indirect reseller access to the subscription using AOBO.</span></span>|<span data-ttu-id="b0e98-127">自動 (パートナーの作業は不要)</span><span class="sxs-lookup"><span data-stu-id="b0e98-127">Automatic (no partner work required)</span></span>|
|<span data-ttu-id="b0e98-128">Azure Lighthouse</span><span class="sxs-lookup"><span data-stu-id="b0e98-128">Azure Lighthouse</span></span>|<span data-ttu-id="b0e98-129">パートナーは、新しい[マネージド サービス オファーをマーケットプレースに](/azure/lighthouse/concepts/managed-services-offers)作成します。</span><span class="sxs-lookup"><span data-stu-id="b0e98-129">Partner creates a new [Managed Services offer in Marketplace](/azure/lighthouse/concepts/managed-services-offers).</span></span> <span data-ttu-id="b0e98-130">このオファーが CSP サブスクリプションで承認されると、パートナーは CSP サブスクリプションにアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="b0e98-130">This offer is accepted on the CSP subscription and partner gets access to the CSP subscription.</span></span>|<span data-ttu-id="b0e98-131">自動 (パートナーの作業は不要)</span><span class="sxs-lookup"><span data-stu-id="b0e98-131">Automatic (no partner work required)</span></span>|
|<span data-ttu-id="b0e98-132">Azure Lighthouse</span><span class="sxs-lookup"><span data-stu-id="b0e98-132">Azure Lighthouse</span></span>|<span data-ttu-id="b0e98-133">パートナーは、Azure サブスクリプションで [ARM テンプレート](/azure/lighthouse/how-to/onboard-customer)をデプロイします</span><span class="sxs-lookup"><span data-stu-id="b0e98-133">Partner deploys [ARM template](/azure/lighthouse/how-to/onboard-customer) in Azure subscription</span></span>|<span data-ttu-id="b0e98-134">パートナーは、パートナー テナントのユーザーまたはサービス プリンシパルに MPN ID を関連付ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0e98-134">Partner needs to associate the MPN ID to the user or service principal in the partner tenant.</span></span> <span data-ttu-id="b0e98-135">詳細については、[パートナー ID のリンク](/azure/billing/billing-partner-admin-link-started)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0e98-135">For more information - [Link Partner ID](/azure/billing/billing-partner-admin-link-started).</span></span>|
|<span data-ttu-id="b0e98-136">ディレクトリまたはゲスト ユーザー</span><span class="sxs-lookup"><span data-stu-id="b0e98-136">Directory or guest user</span></span>|<span data-ttu-id="b0e98-137">パートナーは、顧客のディレクトリに新しいユーザーまたはサービス プリンシパルを作成し、ユーザーに CSP サブスクリプションへのアクセス権を付与します。</span><span class="sxs-lookup"><span data-stu-id="b0e98-137">Partner creates a new user or service principal in the customer directory and gives access to the CSP subscription to the user.</span></span> <span data-ttu-id="b0e98-138">パートナーは、顧客のディレクトリに新しいユーザーまたはサービス プリンシパルを作成します。</span><span class="sxs-lookup"><span data-stu-id="b0e98-138">Partner creates a new user or service principal in the customer directory.</span></span> <span data-ttu-id="b0e98-139">パートナーは、グループにユーザーを追加し、グループへの CSP サブスクリプションへのアクセス権を付与します。</span><span class="sxs-lookup"><span data-stu-id="b0e98-139">Partner adds the user to a group and gives access to the CSP subscription to the group.</span></span>|<span data-ttu-id="b0e98-140">パートナーは、顧客テナントのユーザーまたはサービス プリンシパルに MPN ID を関連付ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0e98-140">Partner needs to associate the MPN ID to the user or service principal in the customer tenant.</span></span> <span data-ttu-id="b0e98-141">詳細については、[パートナー ID のリンク](/azure/billing/billing-partner-admin-link-started)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0e98-141">For more information - [Link Partner ID](/azure/billing/billing-partner-admin-link-started).</span></span>|

## <a name="confirm-that-you-have-admin-access"></a><span data-ttu-id="b0e98-142">管理者アクセス権を持っていることを確認する</span><span class="sxs-lookup"><span data-stu-id="b0e98-142">Confirm that you have admin access</span></span>

<span data-ttu-id="b0e98-143">顧客のサービスを管理し、獲得したクレジットを受け取るには、管理者アクセス権が必要です。</span><span class="sxs-lookup"><span data-stu-id="b0e98-143">You require admin access to manage your customer's services and to received earned credits.</span></span> <span data-ttu-id="b0e98-144">獲得したクレジットの詳細については、[パートナー獲得クレジット](partner-earned-credit.md)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0e98-144">Read [Partner earned credits](partner-earned-credit.md) for detailed information on earned credits.</span></span> <span data-ttu-id="b0e98-145">管理者アクセス権を持っていることを確認するには、2 つの方法があります。</span><span class="sxs-lookup"><span data-stu-id="b0e98-145">You have two ways to make sure you know that you have admin access.</span></span>

- <span data-ttu-id="b0e98-146">毎日の利用状況ファイルを確認する - これを判断するには、毎日の使用量ファイル内の単価と実効単価を見て、割引が適用されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="b0e98-146">Review the daily usage file - This can be determined by reviewing the unit price and effective unit price within the daily usage file and confirming if a discount is being applied.</span></span> <span data-ttu-id="b0e98-147">割引が適用されている場合は管理者です。</span><span class="sxs-lookup"><span data-stu-id="b0e98-147">If you are receiving the discount you are the admin.</span></span>

- <span data-ttu-id="b0e98-148">Azure Monitor のアラートを作成する - RBAC のアクセスが CSP サブスクリプションから削除されたことが通知する Azure Monitor のアクティビティ ログ [アラート](/azure/azure-monitor/platform/alerts-activity-log)を作成します。</span><span class="sxs-lookup"><span data-stu-id="b0e98-148">Create an Azure monitor alert - You can create an Azure Monitor activity log [alert](/azure/azure-monitor/platform/alerts-activity-log) to be notified of  when your RBAC access is removed from CSP subscription.</span></span>

### <a name="create-an-azure-monitor-alert"></a><span data-ttu-id="b0e98-149">Azure Monitor のアラートを作成する</span><span class="sxs-lookup"><span data-stu-id="b0e98-149">Create an Azure monitor alert</span></span>

1. <span data-ttu-id="b0e98-150">アラートを作成します。</span><span class="sxs-lookup"><span data-stu-id="b0e98-150">Create alert.</span></span>

   :::image type="content" source="images/azure/azurealert1.png" alt-text="Azure アラート":::

2. <span data-ttu-id="b0e98-152">アラートを受け取るアクションの種類を選択します。たとえば、メールを送信するように指定すると、ロールの割り当ての削除が発生した場合に通知するメールが送信されます。</span><span class="sxs-lookup"><span data-stu-id="b0e98-152">Select the type of action you want the alert to take.For example, if you specify that you want an email, you will receive an email notifying you if any role assignment deletion occurs.</span></span>

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="アラートを構成する":::

### <a name="aobo-removal"></a><span data-ttu-id="b0e98-154">AOBO の削除</span><span class="sxs-lookup"><span data-stu-id="b0e98-154">AOBO removal</span></span>

<span data-ttu-id="b0e98-155">顧客は、Azure portal で **[アクセス制御]** に移動してサブスクリプションへのアクセスを管理できます。</span><span class="sxs-lookup"><span data-stu-id="b0e98-155">Customers can manage access to their subscriptions by going to **Access Control** on the Azure portal.</span></span> <span data-ttu-id="b0e98-156">**[ロールの割り当て]** タブで、 **[アクセス許可の削除]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b0e98-156">From the **Role assignments** tab, they select **Remove access**.</span></span> <span data-ttu-id="b0e98-157">この操作が行われた場合は、以下のように対処します。</span><span class="sxs-lookup"><span data-stu-id="b0e98-157">If this happens, you can:</span></span>

- <span data-ttu-id="b0e98-158">顧客と話し、管理者アクセス権を回復できるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="b0e98-158">Talk with your customer to see if admin access can be reinstated.</span></span>

- <span data-ttu-id="b0e98-159">[ロールベースのアクセス制御 (RBAC)](/azure/role-based-access-control/overview) を介して付与されたアクセス権を使用します。</span><span class="sxs-lookup"><span data-stu-id="b0e98-159">Use the access provided through [role-based access control (RBAC)](/azure/role-based-access-control/overview).</span></span>

- <span data-ttu-id="b0e98-160">[Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/) を介して付与されたアクセス権を使用します。</span><span class="sxs-lookup"><span data-stu-id="b0e98-160">Use access provided through [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).</span></span>

<span data-ttu-id="b0e98-161">ロールベースのアクセス権は、管理者アクセス権とは異なります。</span><span class="sxs-lookup"><span data-stu-id="b0e98-161">Role-based access differs from admin access.</span></span> <span data-ttu-id="b0e98-162">ロールでは、できることと実行できないことが明確に分かれています。</span><span class="sxs-lookup"><span data-stu-id="b0e98-162">Roles delimit precisely what you can and can't do.</span></span> <span data-ttu-id="b0e98-163">管理者アクセス権の方が広範囲です。</span><span class="sxs-lookup"><span data-stu-id="b0e98-163">Admin access is broader.</span></span>

<span data-ttu-id="b0e98-164">PEC を獲得できるロールを確認するには、[パートナー獲得クレジットのロールとアクセス許可](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0e98-164">To see the roles eligible to earn PEC, read [Roles and permissions for the partner earned credit](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2).</span></span>

## <a name="next-steps"></a><span data-ttu-id="b0e98-165">次の手順</span><span class="sxs-lookup"><span data-stu-id="b0e98-165">Next steps</span></span>

- [<span data-ttu-id="b0e98-166">Azure CSP サブスクリプションの管理者特権を取り消したり元に戻したりする</span><span class="sxs-lookup"><span data-stu-id="b0e98-166">Revoking and reinstating admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)

- [<span data-ttu-id="b0e98-167">パートナー獲得クレジット - 概要</span><span class="sxs-lookup"><span data-stu-id="b0e98-167">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- [<span data-ttu-id="b0e98-168">マネージド サービスのパートナー獲得クレジット</span><span class="sxs-lookup"><span data-stu-id="b0e98-168">Partner earned credit for managed services</span></span>](partner-earned-credit-explanation.md)