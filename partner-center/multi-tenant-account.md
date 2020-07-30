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
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389517"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="b461e-103">パートナーセンターアカウントで複数のテナントを追加して管理する</span><span class="sxs-lookup"><span data-stu-id="b461e-103">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="b461e-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="b461e-104">**Applies to**</span></span>

- <span data-ttu-id="b461e-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="b461e-105">Partner Center</span></span>

<span data-ttu-id="b461e-106">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="b461e-106">**Appropriate roles**</span></span>

- <span data-ttu-id="b461e-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="b461e-107">Global admin</span></span>

<span data-ttu-id="b461e-108">パートナーセンターアカウントで複数の Azure AD テナントを管理する必要がある理由は多数あります。</span><span class="sxs-lookup"><span data-stu-id="b461e-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="b461e-109">たとえば、会社で別の会社を購入し、新しい会社の従業員がパートナーセンターを使用できるようにしたいとします。</span><span class="sxs-lookup"><span data-stu-id="b461e-109">For example, your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="b461e-110">ただし、2つの企業を別々に保つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="b461e-110">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="b461e-111">この場合は、新しい会社の Azure AD テナントとパートナーのグローバルアカウント (PNG) を関連付けます。</span><span class="sxs-lookup"><span data-stu-id="b461e-111">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PNG).</span></span> <span data-ttu-id="b461e-112">この関連付けにより、両方の企業のユーザーがパートナーセンターで作業できるようになります。</span><span class="sxs-lookup"><span data-stu-id="b461e-112">This association would enable users in both companies to work in Partner Center.</span></span>

## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="b461e-113">アカウントに別の Azure AD テナントを追加する</span><span class="sxs-lookup"><span data-stu-id="b461e-113">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="b461e-114">全体管理者として、パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="b461e-114">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="b461e-115">**設定**アイコンで、[**アカウントの設定**] を選択し、[**テナント**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b461e-115">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="テナントの関連付け"::: 

3. <span data-ttu-id="b461e-117">[**別の AD テナントを関連付ける**] を選択し、関連付けるテナントを指定します。</span><span class="sxs-lookup"><span data-stu-id="b461e-117">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="b461e-118">グローバル管理者として、関連付けるテナントにサインインし、関連付けを確認します。</span><span class="sxs-lookup"><span data-stu-id="b461e-118">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="テナントの関連付けの確認"::: 

5. <span data-ttu-id="b461e-120">確認が完了すると、すべての**設定**の通知が表示されます。</span><span class="sxs-lookup"><span data-stu-id="b461e-120">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="b461e-121">[**テナント管理に戻る**] を選択すると、新しく追加されたテナントが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="b461e-121">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span>
 
## <a name="next-steps"></a><span data-ttu-id="b461e-122">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b461e-122">Next steps</span></span>

- [<span data-ttu-id="b461e-123">ユーザーの追加</span><span class="sxs-lookup"><span data-stu-id="b461e-123">Add users</span></span>](create-user-accounts-and-set-permissions.md)
