---
title: 顧客アカウントに複数のユーザーを作成する | パートナー センター
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: コンマ区切り値ファイル形式 (.csv) のデータファイルをパートナーセンターにアップロードすることで、顧客のアカウントに複数のユーザーを一度に追加する方法について説明します。
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: 一括アップロード, 顧客アカウントへの複数ユーザーの追加, 顧客のユーザーの追加, 顧客のユーザーの一括アップロード, 顧客アカウント, 顧客のユーザー, ユーザー
ms.localizationpriority: medium
ms.openlocfilehash: 2195d23074a3e7c397b5f557fd3bed9ec0cc518e
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721988"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="68de7-104">顧客アカウントに複数のユーザーを追加する</span><span class="sxs-lookup"><span data-stu-id="68de7-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="68de7-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="68de7-105">**Applies to**</span></span>

- <span data-ttu-id="68de7-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="68de7-106">Partner Center</span></span>

<span data-ttu-id="68de7-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="68de7-107">**Appropriate roles**</span></span>

- <span data-ttu-id="68de7-108">グローバル管理</span><span class="sxs-lookup"><span data-stu-id="68de7-108">Global admin</span></span>

<span data-ttu-id="68de7-109">顧客のアカウントに一度に複数のユーザーを追加できます。そのためには、コンマ区切り値ファイル形式 (.csv) のデータ ファイルをパートナー センターにアップロードします。</span><span class="sxs-lookup"><span data-stu-id="68de7-109">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="68de7-110">パートナー センターからサンプル データ ファイルをダウンロードし、それを編集して使用することも、以下に定義するデータ モデルを使用して新しいデータ ファイルを作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="68de7-110">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="68de7-111">データ ファイルの要件</span><span class="sxs-lookup"><span data-stu-id="68de7-111">Data file requirements</span></span>

<span data-ttu-id="68de7-112">一括アップロードプロセスを使用して顧客のアカウントに複数のユーザーを追加するには、次の要件を満たす必要があります。</span><span class="sxs-lookup"><span data-stu-id="68de7-112">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="68de7-113">顧客アカウントに対してグローバル管理者のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="68de7-113">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="68de7-114">各ユーザーは、顧客の電子メール ドメインに追加された、一意のメール アドレスを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="68de7-114">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="68de7-115">一度に最大 100 個のレコードをアップロードすることができます。</span><span class="sxs-lookup"><span data-stu-id="68de7-115">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="68de7-116">100 を超えるユーザーを追加する必要がある場合は、追加のデータ ファイルを作成してアップロードします。</span><span class="sxs-lookup"><span data-stu-id="68de7-116">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="68de7-117">すべてのユーザーは、地理的に同じ**場所**にいる必要があります。</span><span class="sxs-lookup"><span data-stu-id="68de7-117">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="68de7-118">次に示すデータのみを入力します。</span><span class="sxs-lookup"><span data-stu-id="68de7-118">Enter only the data described below.</span></span> <span data-ttu-id="68de7-119">余分なデータがあると、アップロードに失敗します。</span><span class="sxs-lookup"><span data-stu-id="68de7-119">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="68de7-120">データ ファイルに、次のデータを入力します。</span><span class="sxs-lookup"><span data-stu-id="68de7-120">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="68de7-121">**列の名前**</span><span class="sxs-lookup"><span data-stu-id="68de7-121">**Column name**</span></span> | <span data-ttu-id="68de7-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="68de7-122">**Description**</span></span>                                                              | <span data-ttu-id="68de7-123">**制限事項**</span><span class="sxs-lookup"><span data-stu-id="68de7-123">**Limitation**</span></span>                             |
| <span data-ttu-id="68de7-124">名</span><span class="sxs-lookup"><span data-stu-id="68de7-124">First name</span></span>      | <span data-ttu-id="68de7-125">ユーザーの名 (オプションフィールド)</span><span class="sxs-lookup"><span data-stu-id="68de7-125">User's first name (optional field)</span></span>                                           | <span data-ttu-id="68de7-126">50 文字の制限</span><span class="sxs-lookup"><span data-stu-id="68de7-126">50-character limit</span></span>                         |
| <span data-ttu-id="68de7-127">姓</span><span class="sxs-lookup"><span data-stu-id="68de7-127">Last name</span></span>       | <span data-ttu-id="68de7-128">ユーザーの姓 (省略可能なフィールド)</span><span class="sxs-lookup"><span data-stu-id="68de7-128">User's last name (optional field)</span></span>                                            | <span data-ttu-id="68de7-129">50 文字の制限</span><span class="sxs-lookup"><span data-stu-id="68de7-129">50-character limit</span></span>                         |
| <span data-ttu-id="68de7-130">表示名</span><span class="sxs-lookup"><span data-stu-id="68de7-130">Display name</span></span>    | <span data-ttu-id="68de7-131">パートナー センターで表示される名前 (必須フィールド)</span><span class="sxs-lookup"><span data-stu-id="68de7-131">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="68de7-132">50 文字の制限</span><span class="sxs-lookup"><span data-stu-id="68de7-132">50-character limit</span></span>                         |
| <span data-ttu-id="68de7-133">[メール]</span><span class="sxs-lookup"><span data-stu-id="68de7-133">Email</span></span>           | <span data-ttu-id="68de7-134">顧客会社のユーザーの勤務先の電子メールアドレス (必須フィールド)</span><span class="sxs-lookup"><span data-stu-id="68de7-134">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="68de7-135">ユーザーごとに一意のメール アドレスが必要</span><span class="sxs-lookup"><span data-stu-id="68de7-135">Each user must have a unique email address</span></span> |
| <span data-ttu-id="68de7-136">状態の更新</span><span class="sxs-lookup"><span data-stu-id="68de7-136">Status update</span></span>   | <span data-ttu-id="68de7-137">新しいユーザー レコードが正常に作成されたかどうかを示すために使用される</span><span class="sxs-lookup"><span data-stu-id="68de7-137">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="68de7-138">\*\*空白のままにする\*\*</span><span class="sxs-lookup"><span data-stu-id="68de7-138">\*\*Leave empty\*\*</span></span>                        |

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="68de7-139">複数のユーザー アカウントを作成するには</span><span class="sxs-lookup"><span data-stu-id="68de7-139">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="68de7-140">以下に説明するデータを使用して、コンマ区切り値 (.csv) データ ファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="68de7-140">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="68de7-141">後の手順を参照できるように、ファイルを保存します。</span><span class="sxs-lookup"><span data-stu-id="68de7-141">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="68de7-142">パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="68de7-142">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="68de7-143">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="68de7-143">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="68de7-144">顧客の **[ユーザーとライセンス]** タブを選択し、 **[ユーザーのアップロード]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="68de7-144">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="68de7-145">**[ユーザー情報のアップロード]** の **[参照]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="68de7-145">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="68de7-146">ファイル セレクターで、データ ファイルを選び、 **[開く]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="68de7-146">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="68de7-147">**[検証]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="68de7-147">Select **Validate**.</span></span>

    <span data-ttu-id="68de7-148">**注:**    ほとんどのアカウント作成エラーは、情報が不足している、メール アドレスの形式が正しくないか重複している、ファイル内のレコードが多すぎるなどのデータ ファイルの問題が原因です。</span><span class="sxs-lookup"><span data-stu-id="68de7-148">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="68de7-149">パートナー センターでファイルが検証された後、新しいユーザーの地理的な**場所**を選びます。</span><span class="sxs-lookup"><span data-stu-id="68de7-149">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="68de7-150">**[保存]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="68de7-150">Select **Save**.</span></span>
10. <span data-ttu-id="68de7-151">ユーザーの一時的なパスワードの情報をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="68de7-151">Download the temporary password information for the users.</span></span>

<span data-ttu-id="68de7-152">**重要:** 一時的なパスワードを含むファイルは必ずこのときにダウンロードしてください。後でこの操作をすることはできません。</span><span class="sxs-lookup"><span data-stu-id="68de7-152">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="68de7-153">新しいユーザーは、新しいアカウントの一時的なパスワードを使用して、新しいアカウントにログインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="68de7-153">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="68de7-154">新しいユーザーには、**ライセンスとサービスを使用できる**アクセス許可が自動的に割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="68de7-154">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



