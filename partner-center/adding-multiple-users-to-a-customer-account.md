---
title: 顧客アカウントに複数のユーザーを作成する | パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: 顧客のアカウントに一度に複数のユーザーを追加できます。そのためには、コンマ区切り値ファイル形式 (.csv) のデータ ファイルをパートナー センターにアップロードします。
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: 一括アップロード, 顧客アカウントへの複数ユーザーの追加, 顧客のユーザーの追加, 顧客のユーザーの一括アップロード, 顧客アカウント, 顧客のユーザー, ユーザー
ms.localizationpriority: medium
ms.openlocfilehash: 12bb42d4e1dcf5003ac8790be777c483f216fd6f
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/29/2018
ms.locfileid: "5795675"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="25610-104">顧客アカウントへの複数ユーザーの追加</span><span class="sxs-lookup"><span data-stu-id="25610-104">Add multiple users to a customer account</span></span>

**<span data-ttu-id="25610-105">適用対象</span><span class="sxs-lookup"><span data-stu-id="25610-105">Applies to</span></span>**

-  <span data-ttu-id="25610-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="25610-106">Partner Center</span></span>

<span data-ttu-id="25610-107">追加できます複数のユーザーが顧客のアカウントをすべて一度にパートナー センターへのコンマ区切り値ファイル形式 (.csv) データ ファイルをアップロードします。</span><span class="sxs-lookup"><span data-stu-id="25610-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="25610-108">パートナー センターからサンプル データ ファイルをダウンロードして、使用するためにそれを編集または以下に定義するデータ モデルを使用して新しいデータ ファイルを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="25610-108">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="25610-109">データ ファイルの要件</span><span class="sxs-lookup"><span data-stu-id="25610-109">Data file requirements</span></span>


<span data-ttu-id="25610-110">一括アップロード プロセスを使用して顧客のアカウントに複数のユーザーを追加するには、次の要件を満たしている必要があります。</span><span class="sxs-lookup"><span data-stu-id="25610-110">To add multiple users to a customer’s account using the bulk upload process, you’ll need to meet the following requirements:</span></span>

-   <span data-ttu-id="25610-111">顧客アカウントに対してグローバル管理者のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="25610-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="25610-112">各ユーザーは、顧客の電子メール ドメインに追加された、一意のメール アドレスを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="25610-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="25610-113">一度に最大 100 個のレコードをアップロードすることができます。</span><span class="sxs-lookup"><span data-stu-id="25610-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="25610-114">100 を超えるユーザーを追加する必要がある場合は、追加のデータ ファイルを作成してアップロードします。</span><span class="sxs-lookup"><span data-stu-id="25610-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="25610-115">すべてのユーザーは、地理的に同じ**場所**にいる必要があります。</span><span class="sxs-lookup"><span data-stu-id="25610-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="25610-116">次に示すデータのみを入力します。</span><span class="sxs-lookup"><span data-stu-id="25610-116">Enter only the data described below.</span></span> <span data-ttu-id="25610-117">余分なデータがあると、アップロードに失敗します。</span><span class="sxs-lookup"><span data-stu-id="25610-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="25610-118">データ ファイルに、次のデータを入力します。</span><span class="sxs-lookup"><span data-stu-id="25610-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **<span data-ttu-id="25610-119">列名</span><span class="sxs-lookup"><span data-stu-id="25610-119">Column name</span></span>** | **<span data-ttu-id="25610-120">説明</span><span class="sxs-lookup"><span data-stu-id="25610-120">Description</span></span>**                                                              | **<span data-ttu-id="25610-121">制限事項</span><span class="sxs-lookup"><span data-stu-id="25610-121">Limitation</span></span>**                             |
| <span data-ttu-id="25610-122">名</span><span class="sxs-lookup"><span data-stu-id="25610-122">First name</span></span>      | <span data-ttu-id="25610-123">ユーザーの名 (省略可能なフィールド)</span><span class="sxs-lookup"><span data-stu-id="25610-123">User’s first name (optional field)</span></span>                                           | <span data-ttu-id="25610-124">50 文字の制限</span><span class="sxs-lookup"><span data-stu-id="25610-124">50-character limit</span></span>                         |
| <span data-ttu-id="25610-125">姓</span><span class="sxs-lookup"><span data-stu-id="25610-125">Last name</span></span>       | <span data-ttu-id="25610-126">ユーザーの姓 (省略可能なフィールド)</span><span class="sxs-lookup"><span data-stu-id="25610-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="25610-127">50 文字の制限</span><span class="sxs-lookup"><span data-stu-id="25610-127">50-character limit</span></span>                         |
| <span data-ttu-id="25610-128">表示名</span><span class="sxs-lookup"><span data-stu-id="25610-128">Display name</span></span>    | <span data-ttu-id="25610-129">パートナー センター (必須フィールド) で表示される名前</span><span class="sxs-lookup"><span data-stu-id="25610-129">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="25610-130">50 文字の制限</span><span class="sxs-lookup"><span data-stu-id="25610-130">50-character limit</span></span>                         |
| <span data-ttu-id="25610-131">メール</span><span class="sxs-lookup"><span data-stu-id="25610-131">Email</span></span>           | <span data-ttu-id="25610-132">顧客の会社でのユーザーの業務用メール アドレス (必須フィールド)</span><span class="sxs-lookup"><span data-stu-id="25610-132">User’s business email address at customer company (required field)</span></span>           | <span data-ttu-id="25610-133">ユーザーごとに一意のメール アドレスが必要</span><span class="sxs-lookup"><span data-stu-id="25610-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="25610-134">状態の更新</span><span class="sxs-lookup"><span data-stu-id="25610-134">Status update</span></span>   | <span data-ttu-id="25610-135">新しいユーザー レコードが正常に作成されたかどうかを示すために使用される</span><span class="sxs-lookup"><span data-stu-id="25610-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="25610-136">\*\*空白のままにする\* \ \*</span><span class="sxs-lookup"><span data-stu-id="25610-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="25610-137">複数のユーザー アカウントを作成するには</span><span class="sxs-lookup"><span data-stu-id="25610-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="25610-138">以下に説明するデータを使用して、コンマ区切り値 (.csv) データ ファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="25610-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="25610-139">後の手順を参照できるように、ファイルを保存します。</span><span class="sxs-lookup"><span data-stu-id="25610-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="25610-140">**パートナー センター**メニューで、**顧客**を選択し、一覧から顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="25610-140">From the **Partner Center** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="25610-141">**[ユーザーのアップロード]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="25610-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="25610-142">**[ユーザー情報のアップロード]** の **[参照]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="25610-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="25610-143">ファイル セレクターで、データ ファイルを選び、**[開く]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="25610-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="25610-144">**[検証]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="25610-144">Select **Validate**.</span></span>

    <span data-ttu-id="25610-145">**注:** ほとんどのアカウント作成エラーはデータ ファイルの情報、形式が正しくないまたは重複しているメール アドレス、またはファイル内のレコードが多すぎるが不足してなどの問題が原因です。</span><span class="sxs-lookup"><span data-stu-id="25610-145">**Note**Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

7.  <span data-ttu-id="25610-146">パートナー センターでは、ファイルを検証後、は、新しいユーザーの地理的な**場所**を選択します。</span><span class="sxs-lookup"><span data-stu-id="25610-146">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="25610-147">**[保存]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="25610-147">Select **Save**.</span></span>
9.  <span data-ttu-id="25610-148">ユーザーの一時的なパスワードの情報をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="25610-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="25610-149">**重要:** 一時的なパスワードを含むファイルは必ずこのときにダウンロードしてください。後でこの操作をすることはできません。</span><span class="sxs-lookup"><span data-stu-id="25610-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="25610-150">新しいユーザーは、新しいアカウントの一時的なパスワードを使用して、新しいアカウントにログインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="25610-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="25610-151">新しいユーザーは、**ライセンスとサービスの使用**のアクセス許可と自動的に割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="25610-151">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



