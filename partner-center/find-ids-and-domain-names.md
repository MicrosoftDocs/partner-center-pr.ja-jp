---
title: テナント ID、ドメイン名、ユーザー オブジェクト ID を検索する
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 組織の Azure portal テナント ID、ドメイン名、または特定のユーザー オブジェクト ID Azure AD ID を検索する方法について説明します。 一部のタスクでは、この情報が必要です。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 5da41cdbfa7aa1780b31e170a2398e8e7c65df27
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150864"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="e7d75-104">ユーザーの重要な ID を見つける</span><span class="sxs-lookup"><span data-stu-id="e7d75-104">Locate important IDs for a user</span></span>

<span data-ttu-id="e7d75-105">**適切なロール**: グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="e7d75-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="e7d75-106">この記事では、ユーザーの次の [情報Azure portal](https://portal.azure.com/) を検索する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="e7d75-106">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="e7d75-107">ユーザー Microsoft Azure Active DirectoryまたはAzure ADのテナント ID (テナント ID)</span><span class="sxs-lookup"><span data-stu-id="e7d75-107">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="e7d75-108">テナントに関連付けられている組織または会社のプライマリ ドメインAzure AD名</span><span class="sxs-lookup"><span data-stu-id="e7d75-108">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="e7d75-109">ユーザー オブジェクト ID</span><span class="sxs-lookup"><span data-stu-id="e7d75-109">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="e7d75-110">テナント ID Microsoft Azure ADドメイン名を見つける</span><span class="sxs-lookup"><span data-stu-id="e7d75-110">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="e7d75-111">次の手順に従って、Azure AD内のテナント ID またはプライマリ ドメイン名をAzure portal。</span><span class="sxs-lookup"><span data-stu-id="e7d75-111">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="e7d75-112">(プログラムでテナント ID を検索する場合は、「PowerShell または CLI を使用してテナント ID を検索する [」を参照してください](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell))。</span><span class="sxs-lookup"><span data-stu-id="e7d75-112">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="e7d75-113">テナント ID は、異なるアプリケーションまたはリソースで異なる名前と呼ばれる場合があります。</span><span class="sxs-lookup"><span data-stu-id="e7d75-113">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="e7d75-114">たとえば、テナント ID は、ディレクトリ ID、Azure Active Directory (Azure AD) テナント、Microsoft ID、または特定のレポート *(tenantguid*) と呼ばれる場合があります。</span><span class="sxs-lookup"><span data-stu-id="e7d75-114">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="e7d75-115">[Azure portal](https://portal.azure.com/) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="e7d75-115">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="e7d75-116">メニューから **[Azure Active Directory]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e7d75-116">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="メニュー Azure portalオプションを選択Azure Active Directoryオプションの一覧が表示されます。":::

3. <span data-ttu-id="e7d75-118">[Azure Active Directory **の概要** ] ページが表示されます。</span><span class="sxs-lookup"><span data-stu-id="e7d75-118">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="e7d75-119">テナント ID またはAzure ADドメイン名を検索するには、[テナント **ID]** フィールドと [プライマリ ドメイン] **フィールドを探** します。</span><span class="sxs-lookup"><span data-stu-id="e7d75-119">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="e7d75-120">これらのフィールドは、[テナント情報] セクションに表示されます。</span><span class="sxs-lookup"><span data-stu-id="e7d75-120">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="テナント ID とプライマリ ドメイン名の 2 つのフィールドが強調表示された [概要] ページが表示されます。":::

4. <span data-ttu-id="e7d75-122">テナント ID は、他のいくつかの方法Azure portalで確認できます。</span><span class="sxs-lookup"><span data-stu-id="e7d75-122">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="e7d75-123">メニューから **[Azure Active Directory]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e7d75-123">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="e7d75-124">次に、メニューの [ **管理]** セクションを見つけて、[プロパティ] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="e7d75-124">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="e7d75-125">また、[プロパティ] ページには、ユーザーに関連付けられているテナント ID も表示されます。</span><span class="sxs-lookup"><span data-stu-id="e7d75-125">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="[テナント ID] フィールドが強調表示された [プロパティ] ページを表示します。":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="e7d75-127">ユーザーオブジェクト ID を検索する</span><span class="sxs-lookup"><span data-stu-id="e7d75-127">Find the user object ID</span></span>

<span data-ttu-id="e7d75-128">ドメイン名とテナント ID を検索するだけでは、必ずしも十分であるとは限りません。</span><span class="sxs-lookup"><span data-stu-id="e7d75-128">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="e7d75-129">また、ユーザーに割り当てられた特定のオブジェクト ID を見つける必要がある場合もあります。</span><span class="sxs-lookup"><span data-stu-id="e7d75-129">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="e7d75-130">Azure portal でユーザーのオブジェクト ID を検索するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="e7d75-130">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="e7d75-131">[Azure portal](https://portal.azure.com/) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="e7d75-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="e7d75-132">メニューから **[Azure Active Directory]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e7d75-132">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="e7d75-133">メニューの [ **管理** ] セクションに移動し、[ **ユーザー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e7d75-133">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="[ユーザー] オプションが強調表示されている Azure Active Directory メニューを表示します。":::

4. <span data-ttu-id="e7d75-135">[ユーザー] ページで、[検索] ボックスにユーザーの名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="e7d75-135">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="特定のユーザーを検索するための検索ボックスが表示された [ユーザー] ページを表示します。":::

5. <span data-ttu-id="e7d75-137">一覧に表示されているユーザーの名前を選択します。</span><span class="sxs-lookup"><span data-stu-id="e7d75-137">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="検索したユーザーの行を表示するユーザーページを表示します。":::

6. <span data-ttu-id="e7d75-139">ユーザーのプロファイルページで、[Id] セクションを探します。</span><span class="sxs-lookup"><span data-stu-id="e7d75-139">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="e7d75-140">[オブジェクト ID] フィールドが、ユーザーの一意のオブジェクト ID と共に表示されます。</span><span class="sxs-lookup"><span data-stu-id="e7d75-140">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Id セクションとオブジェクト ID の強調表示されたフィールドを含むユーザープロファイルページを表示します。":::

## <a name="next-steps"></a><span data-ttu-id="e7d75-142">次のステップ</span><span class="sxs-lookup"><span data-stu-id="e7d75-142">Next steps</span></span>

- [<span data-ttu-id="e7d75-143">PowerShell または CLI を使用してプログラムでテナント ID を検索する</span><span class="sxs-lookup"><span data-stu-id="e7d75-143">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="e7d75-144">ユーザープロファイルの詳細については、Azure Active Directory を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7d75-144">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="e7d75-145">パートナーセンターで顧客の詳細を表示またはエクスポートする方法について説明します</span><span class="sxs-lookup"><span data-stu-id="e7d75-145">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

