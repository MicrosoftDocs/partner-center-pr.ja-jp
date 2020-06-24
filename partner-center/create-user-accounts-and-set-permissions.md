---
title: ユーザー アカウントの作成とロールの割り当て
description: 各従業員がパートナー センターにアクセスできるように前もってロールを割り当てる必要があります。 ユーザー アカウントの作成、ロールの割り当て、およびアクセス許可の設定の方法について説明します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.custom: SEOAPR.20
Keywords: ロール, アクセス許可,ユーザーの追加, ロールの割り当て, 管理者, エージェント,
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: f73a134193f975357ec2257711f283a6360d33eb
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991416"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="730b2-105">ユーザー アカウントの作成およびロールとアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="730b2-105">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="730b2-106">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="730b2-106">**Appropriate roles**</span></span>

- <span data-ttu-id="730b2-107">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="730b2-107">Account admin</span></span>
- <span data-ttu-id="730b2-108">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="730b2-108">Global admin</span></span>
- <span data-ttu-id="730b2-109">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="730b2-109">User management admin</span></span>

<span data-ttu-id="730b2-110">パートナー センターへのアクセスを必要とする従業員に対してユーザー アカウントを作成します。</span><span class="sxs-lookup"><span data-stu-id="730b2-110">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="730b2-111">これらのタスクは、ユーザー管理の管理者、アカウント管理者、またはグローバル管理者が実行する必要があります。これらのタスクを実行するユーザーには、ユーザー管理者またはグローバル管理者の Azure Active Directory (AAD) ロールも割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="730b2-111">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="730b2-112">AAD ロールの詳細については、「[Azure Active Directory での管理者ロールのアクセス許可](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="730b2-112">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="730b2-113">［新しいユーザーを追加する］</span><span class="sxs-lookup"><span data-stu-id="730b2-113">Add a new user</span></span>

1. <span data-ttu-id="730b2-114">パートナー センターの右上にある **[設定]** アイコンから、 **[ユーザー管理]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="730b2-114">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="730b2-115">**[ユーザーの追加]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="730b2-115">Select **Add user**.</span></span>

3. <span data-ttu-id="730b2-116">ユーザーのフル ネームと一意のメール アドレスを入力します。</span><span class="sxs-lookup"><span data-stu-id="730b2-116">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="730b2-117">ユーザーに割り当てるエージェントの種類や管理者の種類を選択します。</span><span class="sxs-lookup"><span data-stu-id="730b2-117">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="730b2-118">パートナー センターへのアクセスは役割ベースであるため、アクセス許可を割り当てることで、ユーザーのビューをカスタマイズして特定のタスクに必要な機能のみを表示できます。</span><span class="sxs-lookup"><span data-stu-id="730b2-118">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="730b2-119">ユーザーがロールの割り当てを必要としている場合、 **[ユーザー管理]** に移動して全体管理者をフィルター処理することで、連絡する全体管理者を見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="730b2-119">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="730b2-120">**[追加]** を選択してユーザー アカウントを作成します。</span><span class="sxs-lookup"><span data-stu-id="730b2-120">Select **Add** to create the user account.</span></span> <span data-ttu-id="730b2-121">次のページで、ユーザーの詳細を確認します。</span><span class="sxs-lookup"><span data-stu-id="730b2-121">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="730b2-122">このページに表示される、新しいユーザーのサインイン情報を書き留めます。</span><span class="sxs-lookup"><span data-stu-id="730b2-122">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="730b2-123">この情報は後から確認できないため、必ず書き留めて新しいユーザーに送信してください。</span><span class="sxs-lookup"><span data-stu-id="730b2-123">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="730b2-124">ユーザーは、ユーザー名と一時パスワードを使ってパートナー センターにサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="730b2-124">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="730b2-125">ユーザーがパートナーセンターに初めてサインインすると、パスワードの変更を求めるメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="730b2-125">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 


### <a name="find-your-global-admin"></a><span data-ttu-id="730b2-126">グローバル管理者を見つける</span><span class="sxs-lookup"><span data-stu-id="730b2-126">Find your global admin</span></span>

<span data-ttu-id="730b2-127">ユーザーのロールを変更する必要がある場合、または新しいユーザーに特定のロールを割り当てる必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="730b2-127">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="730b2-128">ロールを変更したり、新しいユーザーにロールを割り当てたりできるグローバル管理者を探すには、パートナー センターの上部にある**設定アイコン**から **[ユーザー管理]** を選択し、グローバル管理者でフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="730b2-128">To find a global admin who can make role changes or assign roles to a new user, from the **Settings icon** at the top right of the Partner Center, select **User management** and filter on global admin.</span></span> 


### <a name="new-global-admin"></a><span data-ttu-id="730b2-129">新しいグローバル管理者</span><span class="sxs-lookup"><span data-stu-id="730b2-129">New global admin</span></span>

<span data-ttu-id="730b2-130">グローバル管理者が退職し、別のユーザーにこのロールを割り当てる必要がある場合は、Azure または Office 365 チームのいずれかにチケットを送信できます。</span><span class="sxs-lookup"><span data-stu-id="730b2-130">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="730b2-131">これを行う方法については、次のいずれかのオプションを選択してください。</span><span class="sxs-lookup"><span data-stu-id="730b2-131">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="730b2-132">Azure の新しいグローバル管理者</span><span class="sxs-lookup"><span data-stu-id="730b2-132">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="730b2-133">Office 365 の新しいグローバル管理者</span><span class="sxs-lookup"><span data-stu-id="730b2-133">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="730b2-134">ユーザーにロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="730b2-134">Assign user roles</span></span>

<span data-ttu-id="730b2-135">パートナー センターで作業するには、ロールが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="730b2-135">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="730b2-136">現時点では、ロールには、Azure Active Directory テナントのロール、クラウド ソリューション プロバイダー (CSP) のロール、および AAD 以外の会社のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="730b2-136">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="730b2-137">個々の会社で、これらのロールのすべてが必要になることがあります。</span><span class="sxs-lookup"><span data-stu-id="730b2-137">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="730b2-138">パートナー センターにアクセスするには、テナントで個々のユーザーがリストされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="730b2-138">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="730b2-139">ロールの割り当ては、追加のアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="730b2-139">Role assignments provide additional access.</span></span>


<span data-ttu-id="730b2-140">**AAD テナントのロールには以下が含まれます**:</span><span class="sxs-lookup"><span data-stu-id="730b2-140">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="730b2-141">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="730b2-141">Global admin</span></span>
- <span data-ttu-id="730b2-142">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="730b2-142">User admin</span></span>

<span data-ttu-id="730b2-143">**CSP のロールには以下が含まれます**:</span><span class="sxs-lookup"><span data-stu-id="730b2-143">**CSP roles include**:</span></span>
- <span data-ttu-id="730b2-144">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="730b2-144">Admin agent</span></span>
- <span data-ttu-id="730b2-145">課金管理者</span><span class="sxs-lookup"><span data-stu-id="730b2-145">Billing admin</span></span>
- <span data-ttu-id="730b2-146">販売代理店</span><span class="sxs-lookup"><span data-stu-id="730b2-146">Sales agent</span></span>
- <span data-ttu-id="730b2-147">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="730b2-147">Helpdesk agent</span></span>

<span data-ttu-id="730b2-148">**MPN のメンバーシップと会社を管理するロール (非 AAD)**</span><span class="sxs-lookup"><span data-stu-id="730b2-148">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="730b2-149">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="730b2-149">MPN partner admin</span></span>
- <span data-ttu-id="730b2-150">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="730b2-150">Account admin</span></span>
- <span data-ttu-id="730b2-151">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="730b2-151">Referral admin</span></span>
- <span data-ttu-id="730b2-152">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="730b2-152">Business profile admin</span></span>
- <span data-ttu-id="730b2-153">インセンティブ管理者とユーザー</span><span class="sxs-lookup"><span data-stu-id="730b2-153">Incentives admin and user</span></span>

<span data-ttu-id="730b2-154">**コントロール パネル ベンダーは CSP であり、非 AAD ロールです**。</span><span class="sxs-lookup"><span data-stu-id="730b2-154">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="730b2-155">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="730b2-155">Global admin</span></span>

<span data-ttu-id="730b2-156">**ゲスト ユーザー**は、AAD テナントの一部である必要があり、任意の非 AAD ロールを持つことができます。</span><span class="sxs-lookup"><span data-stu-id="730b2-156">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="730b2-157">ロールの詳細と各ロールで実行できる機能については、「[ユーザーのアクセス許可を割り当てる](permissions-overview.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="730b2-157">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="730b2-158">ユーザーの Microsoft Learn アカウントをパートナー センターに関連付ける</span><span class="sxs-lookup"><span data-stu-id="730b2-158">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="730b2-159">ユーザーがコンピテンシー取得のために実行しているトレーニングとラーニングのパスを確認できるようにするには、MCP ID をパートナー センター アカウントに関連付ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="730b2-159">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="730b2-160">全体管理者は、新しいユーザーを追加するときに、そのユーザーの MCP ID を本人のアカウントに関連付けるよう必ず通知してください。</span><span class="sxs-lookup"><span data-stu-id="730b2-160">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="730b2-161">MCP ID をパートナー センター アカウントに関連付ける方法</span><span class="sxs-lookup"><span data-stu-id="730b2-161">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="730b2-162">パートナー センター ダッシュボードで、ダッシュボードの右上隅にある **[アカウント]** アイコンを選択し、 **[My profile]\(プロファイル\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="730b2-162">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="730b2-163">**[Your learning]\(ラーニング\)** では、お客様の Microsoft Learning アカウントを関連付けることができます。また、Microsoft アカウントを Partner University に接続することもできます。</span><span class="sxs-lookup"><span data-stu-id="730b2-163">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>
