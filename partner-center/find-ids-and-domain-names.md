---
title: テナント ID、ドメイン名、ユーザーオブジェクト ID を検索します
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 組織の Azure AD のテナント ID、ドメイン名、または特定のユーザーオブジェクト ID を Azure portal の Id を検索する方法について説明します。 この情報が必要なタスクもあります。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: cb0325aae30fe57a4be2be3e37bca1ee6aa1eab8
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/01/2020
ms.locfileid: "96439245"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="2d612-104">ユーザーの重要な Id を検索する</span><span class="sxs-lookup"><span data-stu-id="2d612-104">Locate important IDs for a user</span></span>

<span data-ttu-id="2d612-105">この記事では、 [Azure portal](https://portal.azure.com/) を使用して、ユーザーに関する次の情報を検索する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="2d612-105">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="2d612-106">ユーザーの組織または会社の Microsoft Azure Active Directory (Azure AD) テナント ID</span><span class="sxs-lookup"><span data-stu-id="2d612-106">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="2d612-107">Azure AD テナントに関連付けられている組織または会社のプライマリドメイン名</span><span class="sxs-lookup"><span data-stu-id="2d612-107">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="2d612-108">ユーザーオブジェクト ID</span><span class="sxs-lookup"><span data-stu-id="2d612-108">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="2d612-109">Microsoft Azure AD テナント ID とプライマリドメイン名を検索する</span><span class="sxs-lookup"><span data-stu-id="2d612-109">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="2d612-110">Azure portal 内で Azure AD テナント ID またはプライマリドメイン名を見つけるには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="2d612-110">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="2d612-111">(テナント ID をプログラムで検索する場合は、「 [PowerShell または CLI でテナント id を検索](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)する」を参照してください)。</span><span class="sxs-lookup"><span data-stu-id="2d612-111">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="2d612-112">テナント ID は、アプリケーションまたはリソースごとに異なる名前を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="2d612-112">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="2d612-113">たとえば、テナント ID は、ディレクトリ ID、Azure Active Directory (Azure AD) テナント、Microsoft ID、または特定のレポート ( *tenantguid* も含む) と呼ばれる場合があります。</span><span class="sxs-lookup"><span data-stu-id="2d612-113">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="2d612-114">[Azure portal](https://portal.azure.com/) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="2d612-114">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="2d612-115">メニューから **[Azure Active Directory]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="2d612-115">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="メニューから [Azure Active Directory] オプションを選択する Azure portal を示します。":::

3. <span data-ttu-id="2d612-117">Azure Active Directory の **概要** ] ページが表示されます。</span><span class="sxs-lookup"><span data-stu-id="2d612-117">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="2d612-118">Azure AD のテナント ID またはプライマリドメイン名を検索するには、[ **テナント id** ] フィールドと [ **プライマリドメイン** ] フィールドを探します。</span><span class="sxs-lookup"><span data-stu-id="2d612-118">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="2d612-119">これらのフィールドは、[テナント情報] セクションに表示されます。</span><span class="sxs-lookup"><span data-stu-id="2d612-119">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="2つの強調表示されたフィールド、テナント ID、プライマリドメイン名が表示された概要ページが表示されます。":::

4. <span data-ttu-id="2d612-121">テナント ID は、他のいくつかの方法で Azure portal で確認できます。</span><span class="sxs-lookup"><span data-stu-id="2d612-121">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="2d612-122">メニューから **[Azure Active Directory]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="2d612-122">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="2d612-123">次に、メニューの [ **管理** ] セクションを見つけて、[ **プロパティ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="2d612-123">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="2d612-124">また、[プロパティ] ページには、ユーザーに関連付けられているテナント ID も表示されます。</span><span class="sxs-lookup"><span data-stu-id="2d612-124">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="[テナント ID] フィールドが強調表示された [プロパティ] ページを表示します。":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="2d612-126">ユーザーオブジェクト ID を検索する</span><span class="sxs-lookup"><span data-stu-id="2d612-126">Find the user object ID</span></span>

<span data-ttu-id="2d612-127">ドメイン名とテナント ID を検索するだけでは、必ずしも十分であるとは限りません。</span><span class="sxs-lookup"><span data-stu-id="2d612-127">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="2d612-128">また、ユーザーに割り当てられた特定のオブジェクト ID を見つける必要がある場合もあります。</span><span class="sxs-lookup"><span data-stu-id="2d612-128">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="2d612-129">Azure portal でユーザーのオブジェクト ID を検索するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="2d612-129">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="2d612-130">[Azure portal](https://portal.azure.com/) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="2d612-130">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="2d612-131">メニューから **[Azure Active Directory]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="2d612-131">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="2d612-132">メニューの [ **管理** ] セクションに移動し、[ **ユーザー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="2d612-132">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="[ユーザー] オプションが強調表示されている Azure Active Directory メニューを表示します。":::

4. <span data-ttu-id="2d612-134">[ユーザー] ページで、[検索] ボックスにユーザーの名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="2d612-134">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="特定のユーザーを検索するための検索ボックスが表示された [ユーザー] ページを表示します。":::

5. <span data-ttu-id="2d612-136">一覧に表示されているユーザーの名前を選択します。</span><span class="sxs-lookup"><span data-stu-id="2d612-136">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="検索したユーザーの行を表示するユーザーページを表示します。":::

6. <span data-ttu-id="2d612-138">ユーザーのプロファイルページで、[Id] セクションを探します。</span><span class="sxs-lookup"><span data-stu-id="2d612-138">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="2d612-139">[オブジェクト ID] フィールドが、ユーザーの一意のオブジェクト ID と共に表示されます。</span><span class="sxs-lookup"><span data-stu-id="2d612-139">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Id セクションとオブジェクト ID の強調表示されたフィールドを含むユーザープロファイルページを表示します。":::

## <a name="next-steps"></a><span data-ttu-id="2d612-141">次のステップ</span><span class="sxs-lookup"><span data-stu-id="2d612-141">Next steps</span></span>

- [<span data-ttu-id="2d612-142">PowerShell または CLI を使用してプログラムでテナント ID を検索する</span><span class="sxs-lookup"><span data-stu-id="2d612-142">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="2d612-143">ユーザープロファイルの詳細については、Azure Active Directory を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d612-143">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="2d612-144">パートナーセンターで顧客の詳細を表示またはエクスポートする方法について説明します</span><span class="sxs-lookup"><span data-stu-id="2d612-144">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

