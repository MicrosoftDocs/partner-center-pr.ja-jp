---
title: ユーザー アカウントの作成とロールの割り当て
description: 各従業員がパートナー センターにアクセスできるように前もってロールを割り当てる必要があります。 ユーザー アカウントの作成、ロールの割り当て、およびアクセス許可の設定の方法について説明します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: 637e88205d9944f7220e227b5101220d94ed42db
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000436"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="7d0e1-104">ユーザー アカウントの作成およびロールとアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="7d0e1-104">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="7d0e1-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="7d0e1-105">**Appropriate roles**</span></span>

- <span data-ttu-id="7d0e1-106">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="7d0e1-106">Account admin</span></span>
- <span data-ttu-id="7d0e1-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="7d0e1-107">Global admin</span></span>
- <span data-ttu-id="7d0e1-108">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="7d0e1-108">User management admin</span></span>

<span data-ttu-id="7d0e1-109">パートナー センターへのアクセスを必要とする従業員に対してユーザー アカウントを作成します。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="7d0e1-110">これらのタスクは、ユーザー管理の管理者、アカウント管理者、またはグローバル管理者が実行する必要があります。これらのタスクを実行するユーザーには、ユーザー管理者またはグローバル管理者の Azure Active Directory (AAD) ロールも割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="7d0e1-111">AAD ロールの詳細については、「[Azure Active Directory での管理者ロールのアクセス許可](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="7d0e1-112">［新しいユーザーを追加する］</span><span class="sxs-lookup"><span data-stu-id="7d0e1-112">Add a new user</span></span>

1. <span data-ttu-id="7d0e1-113">パートナー センターの右上にある **[設定]** アイコンから、 **[ユーザー管理]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-113">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="7d0e1-114">**[ユーザーの追加]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-114">Select **Add user**.</span></span>

3. <span data-ttu-id="7d0e1-115">ユーザーのフル ネームと一意のメール アドレスを入力します。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="7d0e1-116">ユーザーに割り当てるエージェントの種類や管理者の種類を選択します。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="7d0e1-117">パートナー センターへのアクセスは役割ベースであるため、アクセス許可を割り当てることで、ユーザーのビューをカスタマイズして特定のタスクに必要な機能のみを表示できます。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="7d0e1-118">ユーザーがロールの割り当てを必要としている場合、 **[ユーザー管理]** に移動して全体管理者をフィルター処理することで、連絡する全体管理者を見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="7d0e1-119">**[追加]** を選択してユーザー アカウントを作成します。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="7d0e1-120">次のページで、ユーザーの詳細を確認します。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="7d0e1-121">このページに表示される、新しいユーザーのサインイン情報を書き留めます。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="7d0e1-122">この情報は後から確認できないため、必ず書き留めて新しいユーザーに送信してください。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="7d0e1-123">ユーザーは、ユーザー名と一時パスワードを使ってパートナー センターにサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="7d0e1-124">ユーザーがパートナーセンターに初めてサインインすると、パスワードの変更を求めるメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 

## <a name="find-the-role-youve-been-assigned"></a><span data-ttu-id="7d0e1-125">割り当てられたロールを見つける</span><span class="sxs-lookup"><span data-stu-id="7d0e1-125">Find the role you've been assigned</span></span>

<span data-ttu-id="7d0e1-126">グローバル管理者から知らされていない場合、次の手順を実行して、パートナー センターでロールを確認できます。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-126">If your global admin hasn't told you, you can find out what role you have in Partner Center by doing the following:</span></span>

1. <span data-ttu-id="7d0e1-127">パートナー センター [ダッシュボード]https://partner.microsoft.com/dashboard/home) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-127">Sign into Partner Center [dashboard]https://partner.microsoft.com/dashboard/home).</span></span>

1. <span data-ttu-id="7d0e1-128">**[アカウントの設定]** アイコンを選択してから、 **[マイ プロフィール]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-128">Select the **Account settings** icon and then select **My profile**.</span></span>
 
1. <span data-ttu-id="7d0e1-129">**[ロールおよびアクセス許可]** タブを選択します。ロールとアクセス許可が表示されます。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-129">Select the **Roles and permissions** tab. You will see your roles and permissions.</span></span>
 

>[!Note]
><span data-ttu-id="7d0e1-130">サインイン時にプログラムが表示されない場合は通常、そのプログラムで作業するための適切なアクセス許可がないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-130">If you don't see a program when you sign in, it usually means you don't have the correct permissions to work in that program.</span></span> <span data-ttu-id="7d0e1-131">たとえば、サインイン時にインセンティブ ページが表示されない場合、インセンティブのアクセス許可がありません。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-131">So, for example, if you don't see the Incentives page when you sign in, you don't have Incentives permissions.</span></span> <span data-ttu-id="7d0e1-132">グローバル管理者から、必要なアクセス許可を付与してもらうことができます。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-132">Your global admin can give you needed permissions.</span></span>


## <a name="find-your-global-admin"></a><span data-ttu-id="7d0e1-133">グローバル管理者を見つける</span><span class="sxs-lookup"><span data-stu-id="7d0e1-133">Find your global admin</span></span>

<span data-ttu-id="7d0e1-134">ユーザーのロールを変更する必要がある場合、または新しいユーザーに特定のロールを割り当てる必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-134">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="7d0e1-135">ロールの変更を行ったり、新しいユーザーにロールを割り当てたりできるグローバル管理者を見つけるには、パートナー センターの右上にある **[アカウントの設定] アイコン**から **[ユーザー管理]** を選択し、グローバル管理者でフィルター処理します。または、 **[マイ プロフィール]** に移動し、 **[ロールとアクセス許可]** を選択して、アクセス許可の昇格をサポートする管理者の名前の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-135">To find a global admin who can make role changes or assign roles to a new user, from the **Account settings icon** at the top right of the Partner Center, select **User management** and filter on global admin, or you can go to **My profile**, select **Roles and permissions** and see a list of the different admins who can help you elevate your permissions.</span></span> 


## <a name="new-global-admin"></a><span data-ttu-id="7d0e1-136">新しいグローバル管理者</span><span class="sxs-lookup"><span data-stu-id="7d0e1-136">New global admin</span></span>

<span data-ttu-id="7d0e1-137">グローバル管理者が退職し、別のユーザーにこのロールを割り当てる必要がある場合は、Azure または Office 365 チームのいずれかにチケットを送信できます。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-137">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="7d0e1-138">これを行う方法については、次のいずれかのオプションを選択してください。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-138">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="7d0e1-139">Azure の新しいグローバル管理者</span><span class="sxs-lookup"><span data-stu-id="7d0e1-139">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="7d0e1-140">Office 365 の新しいグローバル管理者</span><span class="sxs-lookup"><span data-stu-id="7d0e1-140">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="7d0e1-141">ユーザーにロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="7d0e1-141">Assign user roles</span></span>

<span data-ttu-id="7d0e1-142">パートナー センターで作業するには、ロールが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-142">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="7d0e1-143">現時点では、ロールには、Azure Active Directory テナントのロール、クラウド ソリューション プロバイダー (CSP) のロール、および AAD 以外の会社のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-143">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="7d0e1-144">個々の会社で、これらのロールのすべてが必要になることがあります。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-144">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="7d0e1-145">パートナー センターにアクセスするには、テナントで個々のユーザーがリストされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-145">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="7d0e1-146">ロールの割り当ては、追加のアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-146">Role assignments provide additional access.</span></span>


<span data-ttu-id="7d0e1-147">**AAD テナントのロールには以下が含まれます**:</span><span class="sxs-lookup"><span data-stu-id="7d0e1-147">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="7d0e1-148">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="7d0e1-148">Global admin</span></span>
- <span data-ttu-id="7d0e1-149">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="7d0e1-149">User admin</span></span>

<span data-ttu-id="7d0e1-150">**CSP のロールには以下が含まれます**:</span><span class="sxs-lookup"><span data-stu-id="7d0e1-150">**CSP roles include**:</span></span>
- <span data-ttu-id="7d0e1-151">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="7d0e1-151">Admin agent</span></span>
- <span data-ttu-id="7d0e1-152">課金管理者</span><span class="sxs-lookup"><span data-stu-id="7d0e1-152">Billing admin</span></span>
- <span data-ttu-id="7d0e1-153">販売代理店</span><span class="sxs-lookup"><span data-stu-id="7d0e1-153">Sales agent</span></span>
- <span data-ttu-id="7d0e1-154">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="7d0e1-154">Helpdesk agent</span></span>

<span data-ttu-id="7d0e1-155">**MPN のメンバーシップと会社を管理するロール (非 AAD)**</span><span class="sxs-lookup"><span data-stu-id="7d0e1-155">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="7d0e1-156">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="7d0e1-156">MPN partner admin</span></span>
- <span data-ttu-id="7d0e1-157">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="7d0e1-157">Account admin</span></span>
- <span data-ttu-id="7d0e1-158">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="7d0e1-158">Referral admin</span></span>
- <span data-ttu-id="7d0e1-159">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="7d0e1-159">Business profile admin</span></span>
- <span data-ttu-id="7d0e1-160">インセンティブ管理者とユーザー</span><span class="sxs-lookup"><span data-stu-id="7d0e1-160">Incentives admin and user</span></span>

<span data-ttu-id="7d0e1-161">**コントロール パネル ベンダーは CSP であり、非 AAD ロールです**。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-161">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="7d0e1-162">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="7d0e1-162">Global admin</span></span>

<span data-ttu-id="7d0e1-163">**ゲスト ユーザー**は、AAD テナントの一部である必要があり、任意の非 AAD ロールを持つことができます。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-163">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="7d0e1-164">ロールの詳細と各ロールで実行できる機能については、「[ユーザーのアクセス許可を割り当てる](permissions-overview.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-164">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="7d0e1-165">ユーザーの Microsoft Learn アカウントをパートナー センターに関連付ける</span><span class="sxs-lookup"><span data-stu-id="7d0e1-165">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="7d0e1-166">ユーザーがコンピテンシー取得のために実行しているトレーニングとラーニングのパスを確認できるようにするには、MCP ID をパートナー センター アカウントに関連付ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-166">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="7d0e1-167">全体管理者は、新しいユーザーを追加するときに、そのユーザーの MCP ID を本人のアカウントに関連付けるよう必ず通知してください。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-167">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="7d0e1-168">MCP ID をパートナー センター アカウントに関連付ける方法</span><span class="sxs-lookup"><span data-stu-id="7d0e1-168">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="7d0e1-169">パートナー センター ダッシュボードで、ダッシュボードの右上隅にある **[アカウント]** アイコンを選択し、 **[My profile]\(プロファイル\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-169">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="7d0e1-170">**[Your learning]\(ラーニング\)** では、お客様の Microsoft Learning アカウントを関連付けることができます。また、Microsoft アカウントを Partner University に接続することもできます。</span><span class="sxs-lookup"><span data-stu-id="7d0e1-170">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7d0e1-171">次の手順</span><span class="sxs-lookup"><span data-stu-id="7d0e1-171">Next steps</span></span>

- [<span data-ttu-id="7d0e1-172">パートナー センターで作業する必要がある会社のユーザーにユーザーのロールとアクセス許可を割り当てる</span><span class="sxs-lookup"><span data-stu-id="7d0e1-172">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>](permissions-overview.md)