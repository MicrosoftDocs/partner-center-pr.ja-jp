---
title: 顧客アカウントのユーザーを管理する
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターで顧客のユーザーを管理する-ユーザーアカウントの作成、ユーザーライセンスの追加または削除、パスワードのリセット、ユーザーアカウントの削除または復元を行います。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149895"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="4d1ed-103">顧客アカウントのユーザーとユーザーライセンスを管理する</span><span class="sxs-lookup"><span data-stu-id="4d1ed-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="4d1ed-104">**適切なロール**: 全体管理者 |ユーザー管理の管理者 |管理エージェント</span><span class="sxs-lookup"><span data-stu-id="4d1ed-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>


<span data-ttu-id="4d1ed-105">顧客のアカウントで新しいユーザーを作成および削除することができます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-105">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="4d1ed-106">また、削除後30日以内に削除した1つ以上のユーザーアカウントを復元することもできます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-106">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="4d1ed-107">ユーザーの以前のサブスクリプションの割り当ても (以前の割り当てが利用可能な場合は) 復元されます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-107">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="4d1ed-108">顧客の新しいサブスクリプションを購入する場合、顧客は、アカウントを必要とするすべてのユーザー、ユーザーのアクセス許可、および各ユーザーが必要とするサービスの一覧を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-108">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="4d1ed-109">[**顧客**] タブの [**ユーザーとライセンス**] セクションには、特定の顧客のテナントで作成されたすべてのユーザーが表示されます。これには、別の CSP パートナーから購入したライセンスや別の購入チャネルからライセンスを取得したユーザーも含まれます</span><span class="sxs-lookup"><span data-stu-id="4d1ed-109">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="4d1ed-110">一度に[複数のユーザーにサブスクリプションを割り当てる](bulk-license-provisioning-for-multiple-users.md)ことができます。これには、[Excel 互換の .csv スプレッドシート ファイル](adding-multiple-users-to-a-customer-account.md) を使って、名前をインポートします。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-110">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="4d1ed-111">顧客のユーザー アカウントを作成する</span><span class="sxs-lookup"><span data-stu-id="4d1ed-111">Create user accounts for a customer</span></span>

1. <span data-ttu-id="4d1ed-112">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-112">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="4d1ed-113">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-113">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="4d1ed-114">カスタマーメニューで、[ **ユーザーとライセンス**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-114">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="4d1ed-115">追加するユーザーごとに、**[サブスクリプションの追加]** を選び、アクセス許可やライセンスなどの情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-115">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="4d1ed-116">変更内容を **保存** します。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-116">**Save** your changes.</span></span>

5. <span data-ttu-id="4d1ed-117">必ずユーザー名と一時パスワードを記録してユーザーに送信してください。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-117">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="4d1ed-118">複数のユーザーを 1 人ずつ追加する場合は、**[別のユーザーの追加]** を使います。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-118">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="4d1ed-119">一度に複数のユーザーを追加することもできます。これには、[Excel 互換の .csv スプレッドシート ファイルをインポート](adding-multiple-users-to-a-customer-account.md)します。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-119">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="4d1ed-120">すべてのユーザーの設定が完了するまで待ち、その後で、確認画面からユーザー名とパスワードを電子メールで送信したり印刷したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-120">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="4d1ed-121">顧客のユーザー ライセンスを追加または削除する</span><span class="sxs-lookup"><span data-stu-id="4d1ed-121">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="4d1ed-122">次の手順は、Microsoft 製品のユーザーライセンスを追加または削除する場合に適用されます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-122">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="4d1ed-123">商用マーケットプレースでライセンスベースの SaaS サブスクリプションのユーザーライセンスを追加または削除するには、「 [saas サブスクリプションのライセンスを追加または削除](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-123">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="4d1ed-124">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-124">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="4d1ed-125">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="4d1ed-126">カスタマーメニューで、[ **ユーザーとライセンス**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-126">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="4d1ed-127">一覧から 1 人以上のユーザーを選びます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-127">Choose one or more users from the list.</span></span> <span data-ttu-id="4d1ed-128">たとえば、顧客が新しいライセンスを購入したばかりで、まだ持っていないユーザーに割り当てたい場合は、[ **ユーザーのフィルター** ] オプションを使用して適切なグループを検索できます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-128">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="4d1ed-129">**[ライセンスの管理]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-129">Select **Manage licenses**.</span></span> <span data-ttu-id="4d1ed-130">変更を行い、 **保存** します。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-130">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="4d1ed-131">[Azure Marketplace 製品](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)の場合、ライセンスの割り当てとライセンス認証は、製品を発行した独立系ソフトウェアベンダー (ISV) によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-131">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="4d1ed-132">顧客のユーザー パスワードをリセットする</span><span class="sxs-lookup"><span data-stu-id="4d1ed-132">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="4d1ed-133">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-133">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="4d1ed-134">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-134">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="4d1ed-135">カスタマーメニューで、[ **ユーザーとライセンス**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-135">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="4d1ed-136">一覧からユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-136">Choose the user from the list.</span></span>

4. <span data-ttu-id="4d1ed-137">画面の下部で **[パスワードのリセット]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-137">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="4d1ed-138">新しい一時的なパスワードをユーザーに送信します。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-138">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="4d1ed-139">顧客のユーザー アカウントを削除する</span><span class="sxs-lookup"><span data-stu-id="4d1ed-139">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="4d1ed-140">**パートナー センター** メニューで、**[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-140">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="4d1ed-141">一覧から顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-141">Choose the customer from the list.</span></span>

2. <span data-ttu-id="4d1ed-142">カスタマーメニューで、[ **ユーザーとライセンス**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="4d1ed-143">一覧からユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-143">Choose the user from the list.</span></span>

3. <span data-ttu-id="4d1ed-144">画面の下部にある **[ユーザー アカウントの削除]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-144">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="4d1ed-145">このアカウントを復元する必要が生じた場合、顧客の **[ユーザーとライセンス]** の一覧の **[削除されたアカウント]** タブで見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-145">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="4d1ed-146">削除したユーザーを復元できるのは、削除から 30 日以内です。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-146">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="4d1ed-147">削除されたユーザー アカウントを復元する</span><span class="sxs-lookup"><span data-stu-id="4d1ed-147">Restore deleted user accounts</span></span>

1. <span data-ttu-id="4d1ed-148">**パートナー センター** メニューの **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-148">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="4d1ed-149">[ **ユーザーとライセンス**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-149">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="4d1ed-150">**[削除したユーザー ( 人)]** タブを選びます。復元できる削除済みユーザーが存在する場合は、**(1)** 以上の数値が表示されます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-150">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="4d1ed-151">削除されたユーザーのチェック ボックスを 1 つ以上を選択し、**[復元]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-151">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="4d1ed-152">選択したすべてのユーザー アカウントが、**[ユーザーとライセンス]** ページに再び表示されます。</span><span class="sxs-lookup"><span data-stu-id="4d1ed-152">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4d1ed-153">次のステップ</span><span class="sxs-lookup"><span data-stu-id="4d1ed-153">Next steps</span></span>

- [<span data-ttu-id="4d1ed-154">複数のユーザーへのライセンスの割り当てまたは取り消し</span><span class="sxs-lookup"><span data-stu-id="4d1ed-154">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="4d1ed-155">顧客のアカウントに複数のユーザーを作成する</span><span class="sxs-lookup"><span data-stu-id="4d1ed-155">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)