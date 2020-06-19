---
title: 顧客アカウントに複数のユーザーを追加する
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客のアカウントに複数のユーザーを一度に追加する方法について説明します。 コンマ区切り値 (.csv) ファイル形式を使用して、パートナーセンターにデータファイルをアップロードします。
author: LauraBrenner
ms.author: labrenne
keywords: 一括アップロード, 顧客アカウントへの複数ユーザーの追加, 顧客のユーザーの追加, 顧客のユーザーの一括アップロード, 顧客アカウント, 顧客のユーザー, ユーザー
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 09bb83b82cf1db78a54af9bab98a5cbdaa00c0d9
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991080"
---
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a><span data-ttu-id="46122-105">顧客アカウントに複数のユーザーを追加する-パートナーセンターにデータファイルをアップロードする</span><span class="sxs-lookup"><span data-stu-id="46122-105">Add multiple users to a customer account - upload a data file to Partner Center</span></span>

<span data-ttu-id="46122-106">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="46122-106">**Applies to**</span></span>

- <span data-ttu-id="46122-107">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="46122-107">Partner Center</span></span>

<span data-ttu-id="46122-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="46122-108">**Appropriate roles**</span></span>

- <span data-ttu-id="46122-109">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="46122-109">Global admin</span></span>

<span data-ttu-id="46122-110">顧客のアカウントに一度に複数のユーザーを追加できます。そのためには、コンマ区切り値ファイル形式 (.csv) のデータ ファイルをパートナー センターにアップロードします。</span><span class="sxs-lookup"><span data-stu-id="46122-110">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="46122-111">パートナー センターからサンプル データ ファイルをダウンロードし、それを編集して使用することも、以下に定義するデータ モデルを使用して新しいデータ ファイルを作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="46122-111">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="46122-112">データ ファイルの要件</span><span class="sxs-lookup"><span data-stu-id="46122-112">Data file requirements</span></span>

<span data-ttu-id="46122-113">一括アップロードプロセスを使用して顧客のアカウントに複数のユーザーを追加するには、次の要件を満たす必要があります。</span><span class="sxs-lookup"><span data-stu-id="46122-113">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="46122-114">顧客アカウントに対してグローバル管理者のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="46122-114">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="46122-115">各ユーザーは、顧客の電子メール ドメインに追加された、一意のメール アドレスを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="46122-115">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="46122-116">一度に最大 100 個のレコードをアップロードすることができます。</span><span class="sxs-lookup"><span data-stu-id="46122-116">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="46122-117">100 を超えるユーザーを追加する必要がある場合は、追加のデータ ファイルを作成してアップロードします。</span><span class="sxs-lookup"><span data-stu-id="46122-117">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="46122-118">すべてのユーザーは、地理的に同じ**場所**にいる必要があります。</span><span class="sxs-lookup"><span data-stu-id="46122-118">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="46122-119">次に示すデータのみを入力します。</span><span class="sxs-lookup"><span data-stu-id="46122-119">Enter only the data described below.</span></span> <span data-ttu-id="46122-120">余分なデータがあると、アップロードに失敗します。</span><span class="sxs-lookup"><span data-stu-id="46122-120">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="46122-121">データ ファイルに、次のデータを入力します。</span><span class="sxs-lookup"><span data-stu-id="46122-121">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="46122-122">**列名**</span><span class="sxs-lookup"><span data-stu-id="46122-122">**Column name**</span></span> | <span data-ttu-id="46122-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="46122-123">**Description**</span></span>                                                              | <span data-ttu-id="46122-124">**制限事項**</span><span class="sxs-lookup"><span data-stu-id="46122-124">**Limitation**</span></span>                             |
| <span data-ttu-id="46122-125">名</span><span class="sxs-lookup"><span data-stu-id="46122-125">First name</span></span>      | <span data-ttu-id="46122-126">ユーザーの名 (オプションフィールド)</span><span class="sxs-lookup"><span data-stu-id="46122-126">User's first name (optional field)</span></span>                                           | <span data-ttu-id="46122-127">50 字以内</span><span class="sxs-lookup"><span data-stu-id="46122-127">50-character limit</span></span>                         |
| <span data-ttu-id="46122-128">姓</span><span class="sxs-lookup"><span data-stu-id="46122-128">Last name</span></span>       | <span data-ttu-id="46122-129">ユーザーの姓 (省略可能なフィールド)</span><span class="sxs-lookup"><span data-stu-id="46122-129">User's last name (optional field)</span></span>                                            | <span data-ttu-id="46122-130">50 字以内</span><span class="sxs-lookup"><span data-stu-id="46122-130">50-character limit</span></span>                         |
| <span data-ttu-id="46122-131">表示名</span><span class="sxs-lookup"><span data-stu-id="46122-131">Display name</span></span>    | <span data-ttu-id="46122-132">パートナー センターで表示される名前 (必須フィールド)</span><span class="sxs-lookup"><span data-stu-id="46122-132">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="46122-133">50 字以内</span><span class="sxs-lookup"><span data-stu-id="46122-133">50-character limit</span></span>                         |
| <span data-ttu-id="46122-134">電子メール</span><span class="sxs-lookup"><span data-stu-id="46122-134">Email</span></span>           | <span data-ttu-id="46122-135">顧客会社のユーザーの勤務先の電子メールアドレス (必須フィールド)</span><span class="sxs-lookup"><span data-stu-id="46122-135">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="46122-136">各ユーザーに一意の電子メール アドレスが必要</span><span class="sxs-lookup"><span data-stu-id="46122-136">Each user must have a unique email address</span></span> |
| <span data-ttu-id="46122-137">状態の更新</span><span class="sxs-lookup"><span data-stu-id="46122-137">Status update</span></span>   | <span data-ttu-id="46122-138">新しいユーザー レコードが正常に作成されたかどうかを示すために使用される</span><span class="sxs-lookup"><span data-stu-id="46122-138">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="46122-139">\*\*空白のままにする\*\*</span><span class="sxs-lookup"><span data-stu-id="46122-139">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="46122-140">複数のユーザー アカウントを作成するには</span><span class="sxs-lookup"><span data-stu-id="46122-140">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="46122-141">以下に説明するデータを使用して、コンマ区切り値 (.csv) データ ファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="46122-141">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="46122-142">後の手順を参照できるように、ファイルを保存します。</span><span class="sxs-lookup"><span data-stu-id="46122-142">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="46122-143">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="46122-143">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="46122-144">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="46122-144">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="46122-145">顧客の [**ユーザーとライセンス**] タブを選択し、[**ユーザーのアップロード**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="46122-145">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="46122-146">**[ユーザー情報のアップロード]** の **[参照]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="46122-146">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="46122-147">ファイル セレクターで、データ ファイルを選び、**[開く]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="46122-147">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="46122-148">**[検証]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="46122-148">Select **Validate**.</span></span>

    <span data-ttu-id="46122-149">**メモ**   ほとんどのアカウント作成エラーは、不足している情報、間違った形式の電子メールアドレス、またはファイル内のレコードの数が多すぎるなど、データファイルの問題が原因で発生します。</span><span class="sxs-lookup"><span data-stu-id="46122-149">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="46122-150">パートナー センターでファイルが検証された後、新しいユーザーの地理的な**場所**を選びます。</span><span class="sxs-lookup"><span data-stu-id="46122-150">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="46122-151">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="46122-151">Select **Save**.</span></span>
10. <span data-ttu-id="46122-152">ユーザーの一時パスワードの情報をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="46122-152">Download the temporary password information for the users.</span></span>

<span data-ttu-id="46122-153">**重要:** 一時的なパスワードを含むファイルは必ずこのときにダウンロードしてください。後でこの操作をすることはできません。</span><span class="sxs-lookup"><span data-stu-id="46122-153">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="46122-154">新しいユーザーは、新しいアカウントの一時的なパスワードを使用して、新しいアカウントにログインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="46122-154">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="46122-155">新しいユーザーには、**ライセンスとサービスを使用できる**アクセス許可が自動的に割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="46122-155">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



