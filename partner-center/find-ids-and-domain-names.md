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
ms.openlocfilehash: 17b0100bf5e45e931a765a73fb98afddf6dba656
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172253"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="bbd71-104">ユーザーの重要な Id を検索する</span><span class="sxs-lookup"><span data-stu-id="bbd71-104">Locate important IDs for a user</span></span>

<span data-ttu-id="bbd71-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="bbd71-105">**Appropriate roles**</span></span>

- <span data-ttu-id="bbd71-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="bbd71-106">Global admin</span></span>

<span data-ttu-id="bbd71-107">この記事では、 [Azure portal](https://portal.azure.com/) を使用して、ユーザーに関する次の情報を検索する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="bbd71-107">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="bbd71-108">ユーザーの組織または会社の Microsoft Azure Active Directory (Azure AD) テナント ID</span><span class="sxs-lookup"><span data-stu-id="bbd71-108">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="bbd71-109">Azure AD テナントに関連付けられている組織または会社のプライマリドメイン名</span><span class="sxs-lookup"><span data-stu-id="bbd71-109">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="bbd71-110">ユーザーオブジェクト ID</span><span class="sxs-lookup"><span data-stu-id="bbd71-110">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="bbd71-111">Microsoft Azure AD テナント ID とプライマリドメイン名を検索する</span><span class="sxs-lookup"><span data-stu-id="bbd71-111">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="bbd71-112">Azure portal 内で Azure AD テナント ID またはプライマリドメイン名を見つけるには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="bbd71-112">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="bbd71-113">(テナント ID をプログラムで検索する場合は、「 [PowerShell または CLI でテナント id を検索](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)する」を参照してください)。</span><span class="sxs-lookup"><span data-stu-id="bbd71-113">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="bbd71-114">テナント ID は、アプリケーションまたはリソースごとに異なる名前を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="bbd71-114">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="bbd71-115">たとえば、テナント ID は、ディレクトリ ID、Azure Active Directory (Azure AD) テナント、Microsoft ID、または特定のレポート ( *tenantguid* も含む) と呼ばれる場合があります。</span><span class="sxs-lookup"><span data-stu-id="bbd71-115">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="bbd71-116">[Azure portal](https://portal.azure.com/) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="bbd71-116">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="bbd71-117">メニューから **[Azure Active Directory]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="bbd71-117">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="メニューから [Azure Active Directory] オプションを選択する Azure portal を示します。":::

3. <span data-ttu-id="bbd71-119">Azure Active Directory の **概要** ] ページが表示されます。</span><span class="sxs-lookup"><span data-stu-id="bbd71-119">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="bbd71-120">Azure AD のテナント ID またはプライマリドメイン名を検索するには、[ **テナント id** ] フィールドと [ **プライマリドメイン** ] フィールドを探します。</span><span class="sxs-lookup"><span data-stu-id="bbd71-120">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="bbd71-121">これらのフィールドは、[テナント情報] セクションに表示されます。</span><span class="sxs-lookup"><span data-stu-id="bbd71-121">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="2つの強調表示されたフィールド、テナント ID、プライマリドメイン名が表示された概要ページが表示されます。":::

4. <span data-ttu-id="bbd71-123">テナント ID は、他のいくつかの方法で Azure portal で確認できます。</span><span class="sxs-lookup"><span data-stu-id="bbd71-123">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="bbd71-124">メニューから **[Azure Active Directory]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="bbd71-124">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="bbd71-125">次に、メニューの [ **管理** ] セクションを見つけて、[ **プロパティ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="bbd71-125">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="bbd71-126">また、[プロパティ] ページには、ユーザーに関連付けられているテナント ID も表示されます。</span><span class="sxs-lookup"><span data-stu-id="bbd71-126">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="[テナント ID] フィールドが強調表示された [プロパティ] ページを表示します。":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="bbd71-128">ユーザーオブジェクト ID を検索する</span><span class="sxs-lookup"><span data-stu-id="bbd71-128">Find the user object ID</span></span>

<span data-ttu-id="bbd71-129">ドメイン名とテナント ID を検索するだけでは、必ずしも十分であるとは限りません。</span><span class="sxs-lookup"><span data-stu-id="bbd71-129">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="bbd71-130">また、ユーザーに割り当てられた特定のオブジェクト ID を見つける必要がある場合もあります。</span><span class="sxs-lookup"><span data-stu-id="bbd71-130">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="bbd71-131">Azure portal でユーザーのオブジェクト ID を検索するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="bbd71-131">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="bbd71-132">[Azure portal](https://portal.azure.com/) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="bbd71-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="bbd71-133">メニューから **[Azure Active Directory]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="bbd71-133">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="bbd71-134">メニューの [ **管理** ] セクションに移動し、[ **ユーザー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="bbd71-134">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="[ユーザー] オプションが強調表示されている Azure Active Directory メニューを表示します。":::

4. <span data-ttu-id="bbd71-136">[ユーザー] ページで、[検索] ボックスにユーザーの名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="bbd71-136">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="特定のユーザーを検索するための検索ボックスが表示された [ユーザー] ページを表示します。":::

5. <span data-ttu-id="bbd71-138">一覧に表示されているユーザーの名前を選択します。</span><span class="sxs-lookup"><span data-stu-id="bbd71-138">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="検索したユーザーの行を表示するユーザーページを表示します。":::

6. <span data-ttu-id="bbd71-140">ユーザーのプロファイルページで、[Id] セクションを探します。</span><span class="sxs-lookup"><span data-stu-id="bbd71-140">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="bbd71-141">[オブジェクト ID] フィールドが、ユーザーの一意のオブジェクト ID と共に表示されます。</span><span class="sxs-lookup"><span data-stu-id="bbd71-141">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Id セクションとオブジェクト ID の強調表示されたフィールドを含むユーザープロファイルページを表示します。":::

## <a name="next-steps"></a><span data-ttu-id="bbd71-143">次のステップ</span><span class="sxs-lookup"><span data-stu-id="bbd71-143">Next steps</span></span>

- [<span data-ttu-id="bbd71-144">PowerShell または CLI を使用してプログラムでテナント ID を検索する</span><span class="sxs-lookup"><span data-stu-id="bbd71-144">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="bbd71-145">ユーザープロファイルの詳細については、Azure Active Directory を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bbd71-145">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="bbd71-146">パートナーセンターで顧客の詳細を表示またはエクスポートする方法について説明します</span><span class="sxs-lookup"><span data-stu-id="bbd71-146">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

