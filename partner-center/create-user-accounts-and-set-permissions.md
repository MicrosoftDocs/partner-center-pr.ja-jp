---
title: ユーザー アカウントの作成とロールの割り当て
description: 各従業員がパートナー センターにアクセスできるように前もってロールを割り当てる必要があります。 ユーザー アカウントの作成、ロールの割り当て、およびアクセス許可の設定の方法について説明します。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: c8fad4432f9aabba69877d80038ec9e2665c639d
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492536"
---
# <a name="create-user-accounts"></a><span data-ttu-id="4c863-104">ユーザー アカウントの作成</span><span class="sxs-lookup"><span data-stu-id="4c863-104">Create user accounts</span></span>  

<span data-ttu-id="4c863-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="4c863-105">**Appropriate roles**</span></span>

- <span data-ttu-id="4c863-106">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="4c863-106">Account admin</span></span>
- <span data-ttu-id="4c863-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="4c863-107">Global admin</span></span>
- <span data-ttu-id="4c863-108">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="4c863-108">User management admin</span></span>

<span data-ttu-id="4c863-109">パートナー センターへのアクセスを必要とする従業員に対してユーザー アカウントを作成します。</span><span class="sxs-lookup"><span data-stu-id="4c863-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="4c863-110">これらのタスクは、ユーザー管理の管理者、アカウント管理者、またはグローバル管理者が実行する必要があります。これらのタスクを実行するユーザーには、ユーザー管理者またはグローバル管理者の Azure Active Directory (AAD) ロールも割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4c863-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="4c863-111">AAD ロールの詳細については、「[Azure Active Directory での管理者ロールのアクセス許可](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c863-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="4c863-112">［新しいユーザーを追加する］</span><span class="sxs-lookup"><span data-stu-id="4c863-112">Add a new user</span></span>

1. <span data-ttu-id="4c863-113">パートナー センターの右上にある **[設定]** アイコンから、 **[Account settings]\(アカウントの設定\)** 、 **[ユーザー管理]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="4c863-113">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="4c863-114">**[ユーザーの追加]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="4c863-114">Select **Add user**.</span></span>

3. <span data-ttu-id="4c863-115">ユーザーのフル ネームと一意のメール アドレスを入力します。</span><span class="sxs-lookup"><span data-stu-id="4c863-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="4c863-116">ユーザーに割り当てるエージェントの種類や管理者の種類を選択します。</span><span class="sxs-lookup"><span data-stu-id="4c863-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="4c863-117">パートナー センターへのアクセスは役割ベースであるため、アクセス許可を割り当てることで、ユーザーのビューをカスタマイズして特定のタスクに必要な機能のみを表示できます。</span><span class="sxs-lookup"><span data-stu-id="4c863-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="4c863-118">ユーザーがロールの割り当てを必要としている場合、 **[ユーザー管理]** に移動して全体管理者をフィルター処理することで、連絡する全体管理者を見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="4c863-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="4c863-119">**[追加]** を選択してユーザー アカウントを作成します。</span><span class="sxs-lookup"><span data-stu-id="4c863-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="4c863-120">次のページで、ユーザーの詳細を確認します。</span><span class="sxs-lookup"><span data-stu-id="4c863-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="4c863-121">このページに表示される、新しいユーザーのサインイン情報を書き留めます。</span><span class="sxs-lookup"><span data-stu-id="4c863-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="4c863-122">この情報は後から確認できないため、必ず書き留めて新しいユーザーに送信してください。</span><span class="sxs-lookup"><span data-stu-id="4c863-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="4c863-123">ユーザーは、ユーザー名と一時パスワードを使ってパートナー センターにサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="4c863-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="4c863-124">ユーザーがパートナーセンターに初めてサインインすると、パスワードの変更を求めるメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="4c863-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="4c863-125">ユーザーにロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="4c863-125">Assign user roles</span></span>

<span data-ttu-id="4c863-126">パートナー センターで作業するには、ロールが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4c863-126">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="4c863-127">現時点では、ロールには、Azure Active Directory テナントのロール、クラウド ソリューション プロバイダー (CSP) のロール、および AAD 以外の会社のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="4c863-127">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="4c863-128">個々の会社で、これらのロールのすべてが必要になることがあります。</span><span class="sxs-lookup"><span data-stu-id="4c863-128">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="4c863-129">パートナー センターにアクセスするには、テナントで個々のユーザーがリストされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4c863-129">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="4c863-130">ロールの割り当ては、追加のアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="4c863-130">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4c863-131">次の手順</span><span class="sxs-lookup"><span data-stu-id="4c863-131">Next steps</span></span>

- [<span data-ttu-id="4c863-132">パートナー センターで作業する必要がある従業員にユーザーのロールとアクセス許可を割り当てる</span><span class="sxs-lookup"><span data-stu-id="4c863-132">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
