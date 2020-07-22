---
title: ユーザー アカウントの作成とロールの割り当て
description: 各従業員がパートナー センターにアクセスできるように前もってロールを割り当てる必要があります。 ユーザー アカウントの作成、ロールの割り当て、およびアクセス許可の設定の方法について説明します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: c7d04307be7a81cf3501e1b50e278cf1a012afcd
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435191"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="2eb75-104">ユーザー アカウントの作成およびロールとアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="2eb75-104">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="2eb75-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="2eb75-105">**Appropriate roles**</span></span>

- <span data-ttu-id="2eb75-106">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="2eb75-106">Account admin</span></span>
- <span data-ttu-id="2eb75-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="2eb75-107">Global admin</span></span>
- <span data-ttu-id="2eb75-108">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="2eb75-108">User management admin</span></span>

<span data-ttu-id="2eb75-109">パートナー センターへのアクセスを必要とする従業員に対してユーザー アカウントを作成します。</span><span class="sxs-lookup"><span data-stu-id="2eb75-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="2eb75-110">これらのタスクは、ユーザー管理の管理者、アカウント管理者、またはグローバル管理者が実行する必要があります。これらのタスクを実行するユーザーには、ユーザー管理者またはグローバル管理者の Azure Active Directory (AAD) ロールも割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2eb75-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="2eb75-111">AAD ロールの詳細については、「[Azure Active Directory での管理者ロールのアクセス許可](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2eb75-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="2eb75-112">［新しいユーザーを追加する］</span><span class="sxs-lookup"><span data-stu-id="2eb75-112">Add a new user</span></span>

1. <span data-ttu-id="2eb75-113">パートナー センターの右上にある **[設定]** アイコンから、 **[ユーザー管理]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="2eb75-113">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="2eb75-114">**[ユーザーの追加]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="2eb75-114">Select **Add user**.</span></span>

3. <span data-ttu-id="2eb75-115">ユーザーのフル ネームと一意のメール アドレスを入力します。</span><span class="sxs-lookup"><span data-stu-id="2eb75-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="2eb75-116">ユーザーに割り当てるエージェントの種類や管理者の種類を選択します。</span><span class="sxs-lookup"><span data-stu-id="2eb75-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="2eb75-117">パートナー センターへのアクセスは役割ベースであるため、アクセス許可を割り当てることで、ユーザーのビューをカスタマイズして特定のタスクに必要な機能のみを表示できます。</span><span class="sxs-lookup"><span data-stu-id="2eb75-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="2eb75-118">ユーザーがロールの割り当てを必要としている場合、 **[ユーザー管理]** に移動して全体管理者をフィルター処理することで、連絡する全体管理者を見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="2eb75-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="2eb75-119">**[追加]** を選択してユーザー アカウントを作成します。</span><span class="sxs-lookup"><span data-stu-id="2eb75-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="2eb75-120">次のページで、ユーザーの詳細を確認します。</span><span class="sxs-lookup"><span data-stu-id="2eb75-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="2eb75-121">このページに表示される、新しいユーザーのサインイン情報を書き留めます。</span><span class="sxs-lookup"><span data-stu-id="2eb75-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="2eb75-122">この情報は後から確認できないため、必ず書き留めて新しいユーザーに送信してください。</span><span class="sxs-lookup"><span data-stu-id="2eb75-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="2eb75-123">ユーザーは、ユーザー名と一時パスワードを使ってパートナー センターにサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="2eb75-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="2eb75-124">ユーザーがパートナーセンターに初めてサインインすると、パスワードの変更を求めるメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="2eb75-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 


### <a name="find-your-global-admin"></a><span data-ttu-id="2eb75-125">グローバル管理者を見つける</span><span class="sxs-lookup"><span data-stu-id="2eb75-125">Find your global admin</span></span>

<span data-ttu-id="2eb75-126">ユーザーのロールを変更する必要がある場合、または新しいユーザーに特定のロールを割り当てる必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="2eb75-126">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="2eb75-127">ロールを変更したり、新しいユーザーにロールを割り当てたりできるグローバル管理者を探すには、パートナー センターの上部にある**設定アイコン**から **[ユーザー管理]** を選択し、グローバル管理者でフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="2eb75-127">To find a global admin who can make role changes or assign roles to a new user, from the **Settings icon** at the top right of the Partner Center, select **User management** and filter on global admin.</span></span> 


### <a name="new-global-admin"></a><span data-ttu-id="2eb75-128">新しいグローバル管理者</span><span class="sxs-lookup"><span data-stu-id="2eb75-128">New global admin</span></span>

<span data-ttu-id="2eb75-129">グローバル管理者が退職し、別のユーザーにこのロールを割り当てる必要がある場合は、Azure または Office 365 チームのいずれかにチケットを送信できます。</span><span class="sxs-lookup"><span data-stu-id="2eb75-129">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="2eb75-130">これを行う方法については、次のいずれかのオプションを選択してください。</span><span class="sxs-lookup"><span data-stu-id="2eb75-130">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="2eb75-131">Azure の新しいグローバル管理者</span><span class="sxs-lookup"><span data-stu-id="2eb75-131">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="2eb75-132">Office 365 の新しいグローバル管理者</span><span class="sxs-lookup"><span data-stu-id="2eb75-132">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="2eb75-133">ユーザーにロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="2eb75-133">Assign user roles</span></span>

<span data-ttu-id="2eb75-134">パートナー センターで作業するには、ロールが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2eb75-134">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="2eb75-135">現時点では、ロールには、Azure Active Directory テナントのロール、クラウド ソリューション プロバイダー (CSP) のロール、および AAD 以外の会社のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="2eb75-135">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="2eb75-136">個々の会社で、これらのロールのすべてが必要になることがあります。</span><span class="sxs-lookup"><span data-stu-id="2eb75-136">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="2eb75-137">パートナー センターにアクセスするには、テナントで個々のユーザーがリストされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2eb75-137">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="2eb75-138">ロールの割り当ては、追加のアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="2eb75-138">Role assignments provide additional access.</span></span>


<span data-ttu-id="2eb75-139">**AAD テナントのロールには以下が含まれます**:</span><span class="sxs-lookup"><span data-stu-id="2eb75-139">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="2eb75-140">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="2eb75-140">Global admin</span></span>
- <span data-ttu-id="2eb75-141">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="2eb75-141">User admin</span></span>

<span data-ttu-id="2eb75-142">**CSP のロールには以下が含まれます**:</span><span class="sxs-lookup"><span data-stu-id="2eb75-142">**CSP roles include**:</span></span>
- <span data-ttu-id="2eb75-143">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="2eb75-143">Admin agent</span></span>
- <span data-ttu-id="2eb75-144">課金管理者</span><span class="sxs-lookup"><span data-stu-id="2eb75-144">Billing admin</span></span>
- <span data-ttu-id="2eb75-145">販売代理店</span><span class="sxs-lookup"><span data-stu-id="2eb75-145">Sales agent</span></span>
- <span data-ttu-id="2eb75-146">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="2eb75-146">Helpdesk agent</span></span>

<span data-ttu-id="2eb75-147">**MPN のメンバーシップと会社を管理するロール (非 AAD)**</span><span class="sxs-lookup"><span data-stu-id="2eb75-147">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="2eb75-148">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="2eb75-148">MPN partner admin</span></span>
- <span data-ttu-id="2eb75-149">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="2eb75-149">Account admin</span></span>
- <span data-ttu-id="2eb75-150">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="2eb75-150">Referral admin</span></span>
- <span data-ttu-id="2eb75-151">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="2eb75-151">Business profile admin</span></span>
- <span data-ttu-id="2eb75-152">インセンティブ管理者とユーザー</span><span class="sxs-lookup"><span data-stu-id="2eb75-152">Incentives admin and user</span></span>

<span data-ttu-id="2eb75-153">**コントロール パネル ベンダーは CSP であり、非 AAD ロールです**。</span><span class="sxs-lookup"><span data-stu-id="2eb75-153">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="2eb75-154">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="2eb75-154">Global admin</span></span>

<span data-ttu-id="2eb75-155">**ゲスト ユーザー**は、AAD テナントの一部である必要があり、任意の非 AAD ロールを持つことができます。</span><span class="sxs-lookup"><span data-stu-id="2eb75-155">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="2eb75-156">ロールの詳細と各ロールで実行できる機能については、「[ユーザーのアクセス許可を割り当てる](permissions-overview.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2eb75-156">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="2eb75-157">ユーザーの Microsoft Learn アカウントをパートナー センターに関連付ける</span><span class="sxs-lookup"><span data-stu-id="2eb75-157">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="2eb75-158">ユーザーがコンピテンシー取得のために実行しているトレーニングとラーニングのパスを確認できるようにするには、MCP ID をパートナー センター アカウントに関連付ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="2eb75-158">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="2eb75-159">全体管理者は、新しいユーザーを追加するときに、そのユーザーの MCP ID を本人のアカウントに関連付けるよう必ず通知してください。</span><span class="sxs-lookup"><span data-stu-id="2eb75-159">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="2eb75-160">MCP ID をパートナー センター アカウントに関連付ける方法</span><span class="sxs-lookup"><span data-stu-id="2eb75-160">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="2eb75-161">パートナー センター ダッシュボードで、ダッシュボードの右上隅にある **[アカウント]** アイコンを選択し、 **[My profile]\(プロファイル\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="2eb75-161">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="2eb75-162">**[Your learning]\(ラーニング\)** では、お客様の Microsoft Learning アカウントを関連付けることができます。また、Microsoft アカウントを Partner University に接続することもできます。</span><span class="sxs-lookup"><span data-stu-id="2eb75-162">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>
