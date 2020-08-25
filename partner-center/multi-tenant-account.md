---
title: パートナーセンターアカウントにテナントを追加する
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターアカウントを使用して複数のテナントを管理する
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ecdfcbd4801bee34be298030016d7366b12d7db3
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/25/2020
ms.locfileid: "88846964"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="1b4ac-103">パートナーセンターアカウントで複数のテナントを追加して管理する</span><span class="sxs-lookup"><span data-stu-id="1b4ac-103">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="1b4ac-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="1b4ac-104">**Applies to**</span></span>

- <span data-ttu-id="1b4ac-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="1b4ac-105">Partner Center</span></span>

<span data-ttu-id="1b4ac-106">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="1b4ac-106">**Appropriate roles**</span></span>

- <span data-ttu-id="1b4ac-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="1b4ac-107">Global admin</span></span>

<span data-ttu-id="1b4ac-108">この機能を使用すると、自社の複数のテナントを管理し、パートナー センター アカウントに統合できます。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-108">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="1b4ac-109">パートナーセンターアカウントで複数の Azure AD テナントを管理する必要がある理由は多数あります。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-109">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="1b4ac-110">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-110">For example:</span></span>

- <span data-ttu-id="1b4ac-111">会社は別の会社を購入して、新しい会社の従業員がパートナーセンターを使用できるようにすることができます。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-111">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="1b4ac-112">ただし、2つの企業を別々に保つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-112">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="1b4ac-113">この場合は、新しい会社の Azure AD テナントとパートナーのグローバルアカウント (PGA) を関連付けます。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-113">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="1b4ac-114">この関連付けにより、両方の企業のユーザーがパートナーセンターで作業できるようになります。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-114">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="1b4ac-115">複数のテナントを使用してビジネスを実行する場合 (例: contoso.com、contoso.uk、contoso.in)、マルチテナントを使用して同じ PC アカウントで関連付けることができます。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-115">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="1b4ac-116">合併と買収には複数のテナントを使用する必要があります (Contoso が Fabrikam を買収する場合は、Constoso.com と Fabrikam.com の両方のテナントを使用できるようにする必要があります)。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-116">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="1b4ac-117">いずれかのテナントのユーザーは、次の操作を実行できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-117">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="1b4ac-118">トレーニング、デジタルダウンロード、MCP アソシエーションのためのパートナーセンターへのアクセス</span><span class="sxs-lookup"><span data-stu-id="1b4ac-118">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="1b4ac-119">MPN Admin、インセンティブ管理者などのパートナーセンターの役割を割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-119">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="1b4ac-120">アカウントに別の Azure AD テナントを追加する</span><span class="sxs-lookup"><span data-stu-id="1b4ac-120">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="1b4ac-121">全体管理者として、パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-121">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="1b4ac-122">**設定**アイコンで、[**アカウントの設定**] を選択し、[**テナント**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-122">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="テナントの関連付け"::: 

3. <span data-ttu-id="1b4ac-124">[ **別の AD テナントを関連付ける** ] を選択し、関連付けるテナントを指定します。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-124">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="1b4ac-125">グローバル管理者として、関連付けるテナントにサインインし、関連付けを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-125">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="テナントの関連付けの確認"::: 

5. <span data-ttu-id="1b4ac-127">確認が完了すると、すべての **設定** の通知が表示されます。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-127">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="1b4ac-128">[ **テナント管理に戻る** ] を選択すると、新しく追加されたテナントが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-128">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="1b4ac-129">既に別のパートナーセンターアカウントに関連付けられている場合、そのテナントをアカウントに関連付けることはできません。</span><span class="sxs-lookup"><span data-stu-id="1b4ac-129">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="1b4ac-130">次の手順</span><span class="sxs-lookup"><span data-stu-id="1b4ac-130">Next steps</span></span>

- [<span data-ttu-id="1b4ac-131">ユーザーの追加</span><span class="sxs-lookup"><span data-stu-id="1b4ac-131">Add users</span></span>](create-user-accounts-and-set-permissions.md)
