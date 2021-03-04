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
ms.openlocfilehash: 0e2bb4ceb146174da83e9c08a9ff030380298bd0
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756081"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="3cc60-103">顧客アカウントのユーザーとユーザーライセンスを管理する</span><span class="sxs-lookup"><span data-stu-id="3cc60-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="3cc60-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="3cc60-104">**Appropriate roles**</span></span>

- <span data-ttu-id="3cc60-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="3cc60-105">Global admin</span></span>
- <span data-ttu-id="3cc60-106">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="3cc60-106">User management admin</span></span>
- <span data-ttu-id="3cc60-107">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="3cc60-107">Admin agent</span></span>


<span data-ttu-id="3cc60-108">顧客のアカウントで新しいユーザーを作成および削除することができます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="3cc60-109">また、削除後30日以内に削除した1つ以上のユーザーアカウントを復元することもできます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="3cc60-110">ユーザーの以前のサブスクリプションの割り当ても (以前の割り当てが利用可能な場合は) 復元されます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="3cc60-111">顧客の新しいサブスクリプションを購入する場合、顧客は、アカウントを必要とするすべてのユーザー、ユーザーのアクセス許可、および各ユーザーが必要とするサービスの一覧を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3cc60-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="3cc60-112">[**顧客**] タブの [**ユーザーとライセンス**] セクションには、特定の顧客のテナントで作成されたすべてのユーザーが表示されます。これには、別の CSP パートナーから購入したライセンスや別の購入チャネルからライセンスを取得したユーザーも含まれます</span><span class="sxs-lookup"><span data-stu-id="3cc60-112">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="3cc60-113">一度に[複数のユーザーにサブスクリプションを割り当てる](bulk-license-provisioning-for-multiple-users.md)ことができます。これには、[Excel 互換の .csv スプレッドシート ファイル](adding-multiple-users-to-a-customer-account.md) を使って、名前をインポートします。</span><span class="sxs-lookup"><span data-stu-id="3cc60-113">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="3cc60-114">顧客のユーザー アカウントを作成する</span><span class="sxs-lookup"><span data-stu-id="3cc60-114">Create user accounts for a customer</span></span>

1. <span data-ttu-id="3cc60-115">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="3cc60-115">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3cc60-116">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-116">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3cc60-117">顧客メニューで、**[Users and Licenses]\(ユーザーとライセンス\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3cc60-117">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="3cc60-118">追加するユーザーごとに、**[サブスクリプションの追加]** を選び、アクセス許可やライセンスなどの情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="3cc60-118">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="3cc60-119">変更内容を **保存** します。</span><span class="sxs-lookup"><span data-stu-id="3cc60-119">**Save** your changes.</span></span>

5. <span data-ttu-id="3cc60-120">必ずユーザー名と一時パスワードを記録してユーザーに送信してください。</span><span class="sxs-lookup"><span data-stu-id="3cc60-120">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="3cc60-121">複数のユーザーを 1 人ずつ追加する場合は、**[別のユーザーの追加]** を使います。</span><span class="sxs-lookup"><span data-stu-id="3cc60-121">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="3cc60-122">一度に複数のユーザーを追加することもできます。これには、[Excel 互換の .csv スプレッドシート ファイルをインポート](adding-multiple-users-to-a-customer-account.md)します。</span><span class="sxs-lookup"><span data-stu-id="3cc60-122">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="3cc60-123">すべてのユーザーの設定が完了するまで待ち、その後で、確認画面からユーザー名とパスワードを電子メールで送信したり印刷したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-123">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="3cc60-124">顧客のユーザー ライセンスを追加または削除する</span><span class="sxs-lookup"><span data-stu-id="3cc60-124">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="3cc60-125">次の手順は、Microsoft 製品のユーザーライセンスを追加または削除する場合に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-125">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="3cc60-126">商用マーケットプレースでライセンスベースの SaaS サブスクリプションのユーザーライセンスを追加または削除するには、「 [saas サブスクリプションのライセンスを追加または削除](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3cc60-126">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="3cc60-127">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="3cc60-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3cc60-128">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-128">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3cc60-129">顧客メニューで、**[Users and Licenses]\(ユーザーとライセンス\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3cc60-129">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="3cc60-130">一覧から 1 人以上のユーザーを選びます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-130">Choose one or more users from the list.</span></span> <span data-ttu-id="3cc60-131">たとえば、顧客が新しいライセンスを購入したばかりで、まだライセンスを持っていないユーザーにライセンスを割り当てる場合、**[Filter users by...]** (ユーザーのフィルター条件) オプションを使って適切なグループを見つけます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-131">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="3cc60-132">**[ライセンスの管理]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-132">Select **Manage licenses**.</span></span> <span data-ttu-id="3cc60-133">変更を加えてから、**[保存]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-133">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="3cc60-134">[Azure Marketplace 製品](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)の場合、ライセンスの割り当てとライセンス認証は、製品を発行した独立系ソフトウェアベンダー (ISV) によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-134">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="3cc60-135">顧客のユーザー パスワードをリセットする</span><span class="sxs-lookup"><span data-stu-id="3cc60-135">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="3cc60-136">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="3cc60-136">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3cc60-137">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-137">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3cc60-138">顧客メニューで、**[Users and Licenses]\(ユーザーとライセンス\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3cc60-138">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="3cc60-139">一覧からユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="3cc60-139">Choose the user from the list.</span></span>

4. <span data-ttu-id="3cc60-140">画面の下部で **[パスワードのリセット]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-140">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="3cc60-141">新しい一時的なパスワードをユーザーに送信します。</span><span class="sxs-lookup"><span data-stu-id="3cc60-141">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="3cc60-142">顧客のユーザー アカウントを削除する</span><span class="sxs-lookup"><span data-stu-id="3cc60-142">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="3cc60-143">**パートナー センター** メニューで、**[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3cc60-143">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="3cc60-144">一覧から顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="3cc60-144">Choose the customer from the list.</span></span>

2. <span data-ttu-id="3cc60-145">顧客メニューで、**[Users and Licenses]\(ユーザーとライセンス\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3cc60-145">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="3cc60-146">一覧からユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="3cc60-146">Choose the user from the list.</span></span>

3. <span data-ttu-id="3cc60-147">画面の下部にある **[ユーザー アカウントの削除]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3cc60-147">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="3cc60-148">このアカウントを復元する必要が生じた場合、顧客の **[ユーザーとライセンス]** の一覧の **[削除されたアカウント]** タブで見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-148">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="3cc60-149">削除したユーザーを復元できるのは、削除から 30 日以内です。</span><span class="sxs-lookup"><span data-stu-id="3cc60-149">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="3cc60-150">削除されたユーザー アカウントを復元する</span><span class="sxs-lookup"><span data-stu-id="3cc60-150">Restore deleted user accounts</span></span>

1. <span data-ttu-id="3cc60-151">**パートナー センター** メニューの **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-151">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="3cc60-152">[ **ユーザーとライセンス**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3cc60-152">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="3cc60-153">**[削除したユーザー ( 人)]** タブを選びます。復元できる削除済みユーザーが存在する場合は、**(1)** 以上の数値が表示されます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-153">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="3cc60-154">削除されたユーザーのチェック ボックスを 1 つ以上を選択し、**[復元]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-154">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="3cc60-155">選択したすべてのユーザー アカウントが、**[ユーザーとライセンス]** ページに再び表示されます。</span><span class="sxs-lookup"><span data-stu-id="3cc60-155">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3cc60-156">次のステップ</span><span class="sxs-lookup"><span data-stu-id="3cc60-156">Next steps</span></span>

- [<span data-ttu-id="3cc60-157">複数のユーザーへのライセンスの割り当てまたは取り消し</span><span class="sxs-lookup"><span data-stu-id="3cc60-157">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="3cc60-158">顧客のアカウントに複数のユーザーを作成する</span><span class="sxs-lookup"><span data-stu-id="3cc60-158">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)