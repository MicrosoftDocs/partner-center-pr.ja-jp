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
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151204"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="197ad-103">パートナーセンターアカウントで複数のテナントを追加して管理する</span><span class="sxs-lookup"><span data-stu-id="197ad-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="197ad-104">**適切なロール**: 全体管理者 |アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="197ad-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="197ad-105">この記事では、会社の複数の Azure Active Directory (Azure AD) テナントを統合し、パートナーセンターアカウントで追加および管理する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="197ad-105">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="197ad-106">これには多くの理由があります。</span><span class="sxs-lookup"><span data-stu-id="197ad-106">There are many reasons to do so.</span></span> <span data-ttu-id="197ad-107">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="197ad-107">For example:</span></span>

- <span data-ttu-id="197ad-108">Contoso 社が Fabrikam という別の会社を買収したとします。</span><span class="sxs-lookup"><span data-stu-id="197ad-108">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="197ad-109">2つの会社を別々に残しておく必要があり、新しい従業員がパートナーセンターを使用できるようにする必要があるとします。</span><span class="sxs-lookup"><span data-stu-id="197ad-109">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="197ad-110">この場合は、新しい会社の Azure AD テナントをパートナーのグローバルアカウント (PGA) に関連付けます。</span><span class="sxs-lookup"><span data-stu-id="197ad-110">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="197ad-111">この関連付けにより、両方の企業のユーザーがパートナーセンターで作業できるようになります。</span><span class="sxs-lookup"><span data-stu-id="197ad-111">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="197ad-112">複数のテナント (たとえば、 *contoso.com*、 *contoso.uk*、 *contoso.in*) を使用してビジネスを実行する場合は、マルチテナント機能を使用して同じ PC アカウントでそれらをグループ化できます。</span><span class="sxs-lookup"><span data-stu-id="197ad-112">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="197ad-113">合併と買収のガイドラインで両方の企業のテナントを操作する必要がある場合は、 *constoso.com* テナントと *fabrikam.com* テナントの両方を使用します。</span><span class="sxs-lookup"><span data-stu-id="197ad-113">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="197ad-114">テナントのユーザーは、次のことができる必要があります。</span><span class="sxs-lookup"><span data-stu-id="197ad-114">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="197ad-115">トレーニング、デジタルダウンロード、または Microsoft 認定プロフェッショナル (MCP) のアソシエーションのパートナーセンターにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="197ad-115">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="197ad-116">Microsoft Partner Network (MPN) 管理者やインセンティブ管理者などのパートナーセンターの役割が割り当てられている。</span><span class="sxs-lookup"><span data-stu-id="197ad-116">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="197ad-117">Azure AD テナントをアカウントに追加する</span><span class="sxs-lookup"><span data-stu-id="197ad-117">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="197ad-118">グローバル管理者として [Microsoft パートナーセンター](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="197ad-118">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="197ad-119">右上にある [ **設定**] を選択し、[ **アカウントの設定**] を選択して、[ **テナント**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="197ad-119">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Azure AD プロファイル] ウィンドウの [関連付け] ボタンのスクリーンショット。"::: 

1. <span data-ttu-id="197ad-121">[ **関連付け**] を選択し、関連付けるテナントを指定します。</span><span class="sxs-lookup"><span data-stu-id="197ad-121">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="197ad-122">プロンプトで、関連付けるテナントにグローバル管理者としてサインインし、[確認] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="197ad-122">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="[Confirm new Azure AD association]/(新しいグループの関連付けを確認するAzure ADボタンのスクリーンショット。"::: 

   <span data-ttu-id="197ad-124">関連付けを確認すると、[すべての設定 **] メッセージ** が表示されます。</span><span class="sxs-lookup"><span data-stu-id="197ad-124">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="197ad-125">新しく追加されたテナントを表示するには、[テナント管理に戻 **る] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="197ad-125">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="197ad-126">テナントが別のアカウントに既に関連付けられている場合、テナントをアカウントパートナー センターできません。</span><span class="sxs-lookup"><span data-stu-id="197ad-126">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="197ad-127">アカウントからテナントを削除する</span><span class="sxs-lookup"><span data-stu-id="197ad-127">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="197ad-128">グローバル管理者として Microsoft パートナー センター に [サインインします](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="197ad-128">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="197ad-129">右上にある [設定] アイコン **を選択し** 、[アカウント設定] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="197ad-129">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="197ad-130">左側のウィンドウで、[テナント] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="197ad-130">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="197ad-131">[ **テナントのAzure AD管理] で**、[パートナー] タブ **を選択** します。</span><span class="sxs-lookup"><span data-stu-id="197ad-131">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="197ad-132">関連 **付けを** 削除するテナントの横にある [削除] を選択します。</span><span class="sxs-lookup"><span data-stu-id="197ad-132">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="現在のテナントの関連付けとその [削除] リンクのスクリーンショット。":::

   <span data-ttu-id="197ad-134">前のスクリーンショットに示すように、プライマリテナントと現在サインインしているテナントを除き、関連付けられているすべてのテナントに対して [リンクの削除] リンクが有効になっています。</span><span class="sxs-lookup"><span data-stu-id="197ad-134">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="197ad-135">テナントを削除すると、そのテナントのユーザーは パートナー センター アカウントにアクセスできなくなったので、その削除はコンピテンシーに影響を与える可能性があります。</span><span class="sxs-lookup"><span data-stu-id="197ad-135">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="197ad-136">次の手順</span><span class="sxs-lookup"><span data-stu-id="197ad-136">Next steps</span></span>

- [<span data-ttu-id="197ad-137">ユーザー アカウントの作成</span><span class="sxs-lookup"><span data-stu-id="197ad-137">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






