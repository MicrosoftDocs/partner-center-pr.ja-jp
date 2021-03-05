---
title: パートナーセンターアカウントにテナントを追加する
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターアカウントで複数の Azure AD テナントを追加、統合、または管理する方法と、その方法について説明します。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124807"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="38a11-103">パートナーセンターアカウントで複数のテナントを追加して管理する</span><span class="sxs-lookup"><span data-stu-id="38a11-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="38a11-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="38a11-104">**Appropriate roles**</span></span>

- <span data-ttu-id="38a11-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="38a11-105">Global admin</span></span>
- <span data-ttu-id="38a11-106">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="38a11-106">Account admin</span></span>

<span data-ttu-id="38a11-107">この記事では、会社の複数の Azure Active Directory (Azure AD) テナントを統合し、パートナーセンターアカウントで追加および管理する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="38a11-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="38a11-108">これには多くの理由があります。</span><span class="sxs-lookup"><span data-stu-id="38a11-108">There are many reasons to do so.</span></span> <span data-ttu-id="38a11-109">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="38a11-109">For example:</span></span>

- <span data-ttu-id="38a11-110">Contoso 社が Fabrikam という別の会社を買収したとします。</span><span class="sxs-lookup"><span data-stu-id="38a11-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="38a11-111">2つの会社を別々に残しておく必要があり、新しい従業員がパートナーセンターを使用できるようにする必要があるとします。</span><span class="sxs-lookup"><span data-stu-id="38a11-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="38a11-112">この場合は、新しい会社の Azure AD テナントをパートナーのグローバルアカウント (PGA) に関連付けます。</span><span class="sxs-lookup"><span data-stu-id="38a11-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="38a11-113">この関連付けにより、両方の企業のユーザーがパートナーセンターで作業できるようになります。</span><span class="sxs-lookup"><span data-stu-id="38a11-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="38a11-114">複数のテナント (たとえば、 *contoso.com*、 *contoso.uk*、 *contoso.in*) を使用してビジネスを実行する場合は、マルチテナント機能を使用して同じ PC アカウントでそれらをグループ化できます。</span><span class="sxs-lookup"><span data-stu-id="38a11-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="38a11-115">合併と買収のガイドラインで両方の企業のテナントを操作する必要がある場合は、 *constoso.com* テナントと *fabrikam.com* テナントの両方を使用します。</span><span class="sxs-lookup"><span data-stu-id="38a11-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="38a11-116">テナントのユーザーは、次のことができる必要があります。</span><span class="sxs-lookup"><span data-stu-id="38a11-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="38a11-117">トレーニング、デジタルダウンロード、または Microsoft 認定プロフェッショナル (MCP) のアソシエーションのパートナーセンターにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="38a11-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="38a11-118">Microsoft Partner Network (MPN) 管理者やインセンティブ管理者などのパートナーセンターの役割が割り当てられている。</span><span class="sxs-lookup"><span data-stu-id="38a11-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="38a11-119">Azure AD テナントをアカウントに追加する</span><span class="sxs-lookup"><span data-stu-id="38a11-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="38a11-120">グローバル管理者として [Microsoft パートナーセンター](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="38a11-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="38a11-121">右上にある [ **設定**] を選択し、[ **アカウントの設定**] を選択して、[ **テナント**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="38a11-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Azure AD プロファイル] ウィンドウの [関連付け] ボタンのスクリーンショット。"::: 

1. <span data-ttu-id="38a11-123">[ **関連付け**] を選択し、関連付けるテナントを指定します。</span><span class="sxs-lookup"><span data-stu-id="38a11-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="38a11-124">プロンプトで、関連付けるテナントにグローバル管理者としてサインインし、[ **確認**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="38a11-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="[新しい Azure AD の関連付けの確認] ウィンドウの [確認] ボタンのスクリーンショット。"::: 

   <span data-ttu-id="38a11-126">関連付けを確認すると、すべての **設定** メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="38a11-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="38a11-127">新しく追加されたテナントを表示するには、[ **テナント管理に戻る**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="38a11-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="38a11-128">既に別のパートナーセンターアカウントに関連付けられている場合、そのテナントをアカウントに関連付けることはできません。</span><span class="sxs-lookup"><span data-stu-id="38a11-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="38a11-129">アカウントからテナントを削除する</span><span class="sxs-lookup"><span data-stu-id="38a11-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="38a11-130">グローバル管理者として [Microsoft パートナーセンター](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="38a11-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="38a11-131">右上にある [ **設定** ] アイコンを選択し、[ **アカウントの設定**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="38a11-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="38a11-132">左側のウィンドウで、[ **テナント**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="38a11-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="38a11-133">[ **Azure AD テナントの管理**] で、[ **パートナー** ] タブを選択します。</span><span class="sxs-lookup"><span data-stu-id="38a11-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="38a11-134">関連付けを削除するテナントの横にある [ **削除** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="38a11-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="現在のテナントの関連付けとその削除リンクのスクリーンショット。":::

   <span data-ttu-id="38a11-136">前のスクリーンショットに示されているように、関連付けられているすべてのテナントに対して [ **削除** ] リンクが有効になっています。ただし、プライマリテナントと、現在サインインしているテナントは除きます。</span><span class="sxs-lookup"><span data-stu-id="38a11-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="38a11-137">テナントを削除すると、そのテナントのユーザーはパートナーセンターアカウントにアクセスできなくなり、削除がコンピテンシーに影響を与える可能性があります。</span><span class="sxs-lookup"><span data-stu-id="38a11-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="38a11-138">次の手順</span><span class="sxs-lookup"><span data-stu-id="38a11-138">Next steps</span></span>

- [<span data-ttu-id="38a11-139">ユーザー アカウントの作成</span><span class="sxs-lookup"><span data-stu-id="38a11-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






