---
title: 顧客アカウントのユーザー管理タスク | パートナー センター
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客のユーザーアカウントを作成する方法、ユーザーライセンスを追加または削除する方法、ユーザーのパスワードをリセットする方法、ユーザーアカウントを削除する方法、または復元する方法について説明します。
ms.assetid: 41B06576-8DDD-435D-BABB-697D4AD30213
author: MaggiePucciEvans
ms.author: evansma
Keywords: 顧客管理, アカウント, アカウントの作成, ライセンス、ライセンスの割り当て, ユーザー管理, パスワード, パスワードのリセット, パスワードの変更
ms.localizationpriority: medium
ms.openlocfilehash: cd1b32a0ceb133f9513263f56a7d1e2e98dde3c5
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721363"
---
# <a name="user-management-tasks-for-customer-accounts"></a><span data-ttu-id="cb0ed-104">顧客アカウントのユーザー管理タスク</span><span class="sxs-lookup"><span data-stu-id="cb0ed-104">User management tasks for customer accounts</span></span>

<span data-ttu-id="cb0ed-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="cb0ed-105">**Applies to**</span></span>

- <span data-ttu-id="cb0ed-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="cb0ed-106">Partner Center</span></span>

<span data-ttu-id="cb0ed-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="cb0ed-107">**Appropriate roles**</span></span>

- <span data-ttu-id="cb0ed-108">グローバル管理</span><span class="sxs-lookup"><span data-stu-id="cb0ed-108">Global admin</span></span>
- <span data-ttu-id="cb0ed-109">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="cb0ed-109">User management admin</span></span>
- <span data-ttu-id="cb0ed-110">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="cb0ed-110">Admin agent</span></span>
- <span data-ttu-id="cb0ed-111">販売代理店</span><span class="sxs-lookup"><span data-stu-id="cb0ed-111">Sales agent</span></span>
- <span data-ttu-id="cb0ed-112">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="cb0ed-112">Helpdesk agent</span></span>

<span data-ttu-id="cb0ed-113">顧客のアカウントで新しいユーザーを作成および削除することができます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-113">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="cb0ed-114">また、削除後30日以内に削除した1つ以上のユーザーアカウントを復元することもできます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-114">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="cb0ed-115">ユーザーの以前のサブスクリプションの割り当ても (以前の割り当てが利用可能な場合は) 復元されます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-115">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="cb0ed-116">顧客の新しいサブスクリプションを購入する場合、顧客は、アカウントを必要とするすべてのユーザー、ユーザーのアクセス許可、および各ユーザーが必要とするサービスの一覧を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-116">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="cb0ed-117">一度に[複数のユーザーにサブスクリプションを割り当てる](bulk-license-provisioning-for-multiple-users.md)ことができます。これには、[Excel 互換の .csv スプレッドシート ファイル](adding-multiple-users-to-a-customer-account.md) を使って、名前をインポートします。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-117">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="cb0ed-118">顧客のユーザー アカウントを作成する</span><span class="sxs-lookup"><span data-stu-id="cb0ed-118">Create user accounts for a customer</span></span>

1. <span data-ttu-id="cb0ed-119">パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-119">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="cb0ed-120">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-120">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="cb0ed-121">顧客メニューの **[ユーザーとライセンス]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-121">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="cb0ed-122">追加するユーザーごとに、 **[サブスクリプションの追加]** を選び、アクセス許可やライセンスなどの情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-122">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="cb0ed-123">変更内容を保存するには、 **[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-123">**Save** your changes.</span></span>

5. <span data-ttu-id="cb0ed-124">必ずユーザー名と一時的なパスワードを記録してユーザーに送信してください。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-124">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="cb0ed-125">複数のユーザーを 1 人ずつ追加する場合は、 **[別のユーザーの追加]** を使います。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-125">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="cb0ed-126">一度に複数のユーザーを追加することもできます。これには、[Excel 互換の .csv スプレッドシート ファイルをインポート](adding-multiple-users-to-a-customer-account.md)します。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-126">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="cb0ed-127">すべてのユーザーの設定が完了するまで待ち、その後で、確認画面からユーザー名とパスワードを電子メールで送信したり印刷したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-127">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="cb0ed-128">顧客のユーザー ライセンスを追加または削除する</span><span class="sxs-lookup"><span data-stu-id="cb0ed-128">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="cb0ed-129">次の手順は、Microsoft 製品のユーザーライセンスを追加または削除する場合に適用されます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-129">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="cb0ed-130">商用マーケットプレースでライセンスベースの SaaS サブスクリプションのユーザーライセンスを追加または削除するには、「 [saas サブスクリプションのライセンスを追加または削除](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-130">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="cb0ed-131">パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-131">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="cb0ed-132">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-132">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="cb0ed-133">顧客メニューの **[ユーザーとライセンス]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-133">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="cb0ed-134">一覧から 1 人以上のユーザーを選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-134">Choose one or more users from the list.</span></span> <span data-ttu-id="cb0ed-135">たとえば、顧客が新しいライセンスを購入したばかりで、まだライセンスを持っていないユーザーにライセンスを割り当てる場合、 **[Filter users by...]** (ユーザーのフィルター条件) オプションを使って適切なグループを見つけます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-135">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="cb0ed-136">**[ライセンスの管理]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-136">Select **Manage licenses**.</span></span> <span data-ttu-id="cb0ed-137">変更を加えてから、 **[保存]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-137">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="cb0ed-138">[Azure Marketplace 製品](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)の場合、ライセンスの割り当てとライセンス認証は、製品を発行した独立系ソフトウェアベンダー (ISV) によって管理されます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-138">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="cb0ed-139">顧客のユーザー パスワードをリセットする</span><span class="sxs-lookup"><span data-stu-id="cb0ed-139">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="cb0ed-140">パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-140">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="cb0ed-141">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-141">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="cb0ed-142">顧客メニューの **[ユーザーとライセンス]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="cb0ed-143">一覧からユーザーを選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-143">Choose the user from the list.</span></span>

4.  <span data-ttu-id="cb0ed-144">画面の下部で **[パスワードのリセット]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-144">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="cb0ed-145">新しい一時的なパスワードをユーザーに送信します。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-145">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="cb0ed-146">顧客のユーザー アカウントを削除する</span><span class="sxs-lookup"><span data-stu-id="cb0ed-146">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="cb0ed-147">**パートナー センター** メニューで、 **[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-147">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="cb0ed-148">一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-148">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="cb0ed-149">顧客メニューの **[ユーザーとライセンス]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-149">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="cb0ed-150">一覧からユーザーを選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-150">Choose the user from the list.</span></span>

3.  <span data-ttu-id="cb0ed-151">画面の下部で **[Delete user account]** (ユーザー アカウントの削除) を選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-151">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="cb0ed-152">このアカウントを復元する必要が生じた場合、顧客の **[ユーザーとライセンス]** の一覧の **[削除されたアカウント]** タブで見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-152">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="cb0ed-153">削除したユーザーを復元できるのは、削除から 30 日以内です。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-153">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="cb0ed-154">削除されたユーザー アカウントを復元する</span><span class="sxs-lookup"><span data-stu-id="cb0ed-154">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="cb0ed-155">**パートナー センター** メニューの **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-155">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="cb0ed-156">**[ユーザーとライセンス]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-156">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="cb0ed-157">**[削除したユーザー ( 人)]** タブを選びます。復元できる削除済みユーザーが存在する場合は、 **(1)** 以上の数値が表示されます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-157">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="cb0ed-158">削除されたユーザーのチェック ボックスを 1 つ以上を選択し、 **[復元]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-158">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="cb0ed-159">選択したすべてのユーザー アカウントが、 **[ユーザーとライセンス]** ページに再び表示されます。</span><span class="sxs-lookup"><span data-stu-id="cb0ed-159">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="cb0ed-160">関連トピック</span><span class="sxs-lookup"><span data-stu-id="cb0ed-160">Related topics</span></span>


[<span data-ttu-id="cb0ed-161">複数のユーザーへのライセンスの割り当てまたは取り消し</span><span class="sxs-lookup"><span data-stu-id="cb0ed-161">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="cb0ed-162">顧客のアカウントに複数のユーザーを作成する</span><span class="sxs-lookup"><span data-stu-id="cb0ed-162">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)