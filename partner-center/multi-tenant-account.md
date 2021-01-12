---
title: パートナーセンターアカウントにテナントを追加する
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターアカウントで複数の Azure AD テナントを追加、統合、または管理する方法について説明します。 いくつかの理由についても説明します。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105556"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="f5862-104">パートナーセンターアカウントで複数のテナントを追加して管理する</span><span class="sxs-lookup"><span data-stu-id="f5862-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="f5862-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="f5862-105">**Appropriate roles**</span></span>

- <span data-ttu-id="f5862-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="f5862-106">Global admin</span></span>

<span data-ttu-id="f5862-107">この機能を使用すると、自社の複数のテナントを管理し、パートナー センター アカウントに統合できます。</span><span class="sxs-lookup"><span data-stu-id="f5862-107">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="f5862-108">パートナーセンターアカウントで複数の Azure AD テナントを管理する必要がある理由は多数あります。</span><span class="sxs-lookup"><span data-stu-id="f5862-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="f5862-109">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="f5862-109">For example:</span></span>

- <span data-ttu-id="f5862-110">会社は別の会社を購入して、新しい会社の従業員がパートナーセンターを使用できるようにすることができます。</span><span class="sxs-lookup"><span data-stu-id="f5862-110">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="f5862-111">ただし、2つの企業を別々に保つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="f5862-111">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="f5862-112">この場合は、新しい会社の Azure AD テナントとパートナーのグローバルアカウント (PGA) を関連付けます。</span><span class="sxs-lookup"><span data-stu-id="f5862-112">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="f5862-113">この関連付けにより、両方の企業のユーザーがパートナーセンターで作業できるようになります。</span><span class="sxs-lookup"><span data-stu-id="f5862-113">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="f5862-114">複数のテナントを使用してビジネスを実行する場合 (例: contoso.com、contoso.uk、contoso.in)、マルチテナントを使用して同じ PC アカウントで関連付けることができます。</span><span class="sxs-lookup"><span data-stu-id="f5862-114">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="f5862-115">合併と買収には複数のテナントを使用する必要があります (Contoso が Fabrikam を買収する場合は、Constoso.com と Fabrikam.com の両方のテナントを使用できるようにする必要があります)。</span><span class="sxs-lookup"><span data-stu-id="f5862-115">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="f5862-116">いずれかのテナントのユーザーは、次の操作を実行できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="f5862-116">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="f5862-117">トレーニング、デジタルダウンロード、MCP アソシエーションのためのパートナーセンターへのアクセス</span><span class="sxs-lookup"><span data-stu-id="f5862-117">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="f5862-118">MPN Admin、インセンティブ管理者などのパートナーセンターの役割を割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="f5862-118">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="f5862-119">アカウントに別の Azure AD テナントを追加する</span><span class="sxs-lookup"><span data-stu-id="f5862-119">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="f5862-120">全体管理者として、パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="f5862-120">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="f5862-121">**設定** アイコンで、[**アカウントの設定**] を選択し、[**テナント**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="f5862-121">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="テナントの関連付け"::: 

3. <span data-ttu-id="f5862-123">[ **別の AD テナントを関連付ける** ] を選択し、関連付けるテナントを指定します。</span><span class="sxs-lookup"><span data-stu-id="f5862-123">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="f5862-124">グローバル管理者として、関連付けるテナントにサインインし、関連付けを確認します。</span><span class="sxs-lookup"><span data-stu-id="f5862-124">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="テナントの関連付けの確認"::: 

5. <span data-ttu-id="f5862-126">確認が完了すると、すべての **設定** の通知が表示されます。</span><span class="sxs-lookup"><span data-stu-id="f5862-126">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="f5862-127">[ **テナント管理に戻る** ] を選択すると、新しく追加されたテナントが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="f5862-127">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="f5862-128">既に別のパートナーセンターアカウントに関連付けられている場合、そのテナントをアカウントに関連付けることはできません。</span><span class="sxs-lookup"><span data-stu-id="f5862-128">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="f5862-129">アカウントからテナントを削除する</span><span class="sxs-lookup"><span data-stu-id="f5862-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="f5862-130">全体管理者として、パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="f5862-130">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="f5862-131">**設定** アイコンで、[**アカウントの設定**-> テナント] を選択し、[**パートナー** ] タブをクリックします。</span><span class="sxs-lookup"><span data-stu-id="f5862-131">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="f5862-132">関連付けを解除するテナントの [ **削除** ] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="f5862-132">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="f5862-133">関連付け a テナントは、そのテナントのユーザーがパートナーセンターアカウントにアクセスできなくなることを意味します。これは、コンピテンシーに影響を与える可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f5862-133">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="f5862-134">[ **削除** ] ボタンは、現在サインインしているプライマリテナントとテナントを除く、関連付けられているすべてのテナントに対して有効になっています。</span><span class="sxs-lookup"><span data-stu-id="f5862-134">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="[削除] ボタンがあるテナント":::
 

## <a name="next-steps"></a><span data-ttu-id="f5862-136">次のステップ</span><span class="sxs-lookup"><span data-stu-id="f5862-136">Next steps</span></span>

- [<span data-ttu-id="f5862-137">ユーザーの追加</span><span class="sxs-lookup"><span data-stu-id="f5862-137">Add users</span></span>](create-user-accounts-and-set-permissions.md)






