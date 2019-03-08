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
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584245"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="b0796-104">顧客アカウントへの複数ユーザーの追加</span><span class="sxs-lookup"><span data-stu-id="b0796-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="b0796-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="b0796-105">**Applies to**</span></span>

-  <span data-ttu-id="b0796-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="b0796-106">Partner Center</span></span>

<span data-ttu-id="b0796-107">複数のユーザー アカウントに追加できる顧客のすべて一度にパートナー センターをコンマ区切り値 (.csv) ファイル形式でデータ ファイルをアップロードしています。</span><span class="sxs-lookup"><span data-stu-id="b0796-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="b0796-108">パートナー センターからサンプル データ ファイルをダウンロードして、自分の用途にそれを編集または以下に定義されたデータ モデルを使用して、新しいデータ ファイルを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="b0796-108">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="b0796-109">データ ファイルの要件</span><span class="sxs-lookup"><span data-stu-id="b0796-109">Data file requirements</span></span>


<span data-ttu-id="b0796-110">一括アップロード プロセスを使用して顧客のアカウントに複数のユーザーを追加するには、次の要件を満たしている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0796-110">To add multiple users to a customer’s account using the bulk upload process, you’ll need to meet the following requirements:</span></span>

-   <span data-ttu-id="b0796-111">顧客アカウントに対してグローバル管理者のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="b0796-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="b0796-112">各ユーザーは、顧客の電子メール ドメインに追加された、一意のメール アドレスを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0796-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="b0796-113">一度に最大 100 個のレコードをアップロードすることができます。</span><span class="sxs-lookup"><span data-stu-id="b0796-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="b0796-114">100 を超えるユーザーを追加する必要がある場合は、追加のデータ ファイルを作成してアップロードします。</span><span class="sxs-lookup"><span data-stu-id="b0796-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="b0796-115">すべてのユーザーは、地理的に同じ**場所**にいる必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0796-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="b0796-116">次に示すデータのみを入力します。</span><span class="sxs-lookup"><span data-stu-id="b0796-116">Enter only the data described below.</span></span> <span data-ttu-id="b0796-117">余分なデータがあると、アップロードに失敗します。</span><span class="sxs-lookup"><span data-stu-id="b0796-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="b0796-118">データ ファイルに、次のデータを入力します。</span><span class="sxs-lookup"><span data-stu-id="b0796-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="b0796-119">**列名**</span><span class="sxs-lookup"><span data-stu-id="b0796-119">**Column name**</span></span> | <span data-ttu-id="b0796-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0796-120">**Description**</span></span>                                                              | <span data-ttu-id="b0796-121">**制限事項**</span><span class="sxs-lookup"><span data-stu-id="b0796-121">**Limitation**</span></span>                             |
| <span data-ttu-id="b0796-122">名</span><span class="sxs-lookup"><span data-stu-id="b0796-122">First name</span></span>      | <span data-ttu-id="b0796-123">ユーザーの名 (省略可能なフィールド)</span><span class="sxs-lookup"><span data-stu-id="b0796-123">User’s first name (optional field)</span></span>                                           | <span data-ttu-id="b0796-124">50 文字の制限</span><span class="sxs-lookup"><span data-stu-id="b0796-124">50-character limit</span></span>                         |
| <span data-ttu-id="b0796-125">姓</span><span class="sxs-lookup"><span data-stu-id="b0796-125">Last name</span></span>       | <span data-ttu-id="b0796-126">ユーザーの姓 (省略可能なフィールド)</span><span class="sxs-lookup"><span data-stu-id="b0796-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="b0796-127">50 文字の制限</span><span class="sxs-lookup"><span data-stu-id="b0796-127">50-character limit</span></span>                         |
| <span data-ttu-id="b0796-128">表示名</span><span class="sxs-lookup"><span data-stu-id="b0796-128">Display name</span></span>    | <span data-ttu-id="b0796-129">パートナー センター (必須フィールド) に表示される名前</span><span class="sxs-lookup"><span data-stu-id="b0796-129">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="b0796-130">50 文字の制限</span><span class="sxs-lookup"><span data-stu-id="b0796-130">50-character limit</span></span>                         |
| <span data-ttu-id="b0796-131">Email</span><span class="sxs-lookup"><span data-stu-id="b0796-131">Email</span></span>           | <span data-ttu-id="b0796-132">顧客の会社でのユーザーの業務用メール アドレス (必須フィールド)</span><span class="sxs-lookup"><span data-stu-id="b0796-132">User’s business email address at customer company (required field)</span></span>           | <span data-ttu-id="b0796-133">ユーザーごとに一意のメール アドレスが必要</span><span class="sxs-lookup"><span data-stu-id="b0796-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="b0796-134">状態の更新</span><span class="sxs-lookup"><span data-stu-id="b0796-134">Status update</span></span>   | <span data-ttu-id="b0796-135">新しいユーザー レコードが正常に作成されたかどうかを示すために使用される</span><span class="sxs-lookup"><span data-stu-id="b0796-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="b0796-136">\*\*空のままに\*\*</span><span class="sxs-lookup"><span data-stu-id="b0796-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="b0796-137">複数のユーザー アカウントを作成するには</span><span class="sxs-lookup"><span data-stu-id="b0796-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="b0796-138">以下に説明するデータを使用して、コンマ区切り値 (.csv) データ ファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="b0796-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="b0796-139">後の手順を参照できるように、ファイルを保存します。</span><span class="sxs-lookup"><span data-stu-id="b0796-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="b0796-140">**パートナー センター**メニューの **顧客**、一覧から顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="b0796-140">From the **Partner Center** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="b0796-141">**[ユーザーのアップロード]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="b0796-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="b0796-142">**[ユーザー情報のアップロード]** の **[参照]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="b0796-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="b0796-143">ファイル セレクターで、データ ファイルを選び、**[開く]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="b0796-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="b0796-144">**[検証]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="b0796-144">Select **Validate**.</span></span>

    <span data-ttu-id="b0796-145">**注**  データ ファイルの問題などについては、正しくないか重複している電子メール アドレス、またはファイル内のレコードが多すぎますが不足しているほとんどのアカウントの作成エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="b0796-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

7.  <span data-ttu-id="b0796-146">パートナー センターでは、ファイルを検証後、は、地理的な選択**場所**新しいユーザー向けです。</span><span class="sxs-lookup"><span data-stu-id="b0796-146">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="b0796-147">**[保存]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="b0796-147">Select **Save**.</span></span>
9.  <span data-ttu-id="b0796-148">ユーザーの一時的なパスワードの情報をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="b0796-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="b0796-149">**大事な：** 一時パスワードを持つファイルをダウンロードすることを確認するように後でこれを行うことはできません。</span><span class="sxs-lookup"><span data-stu-id="b0796-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="b0796-150">新しいユーザーは、新しいアカウントの一時的なパスワードを使用して、新しいアカウントにログインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0796-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="b0796-151">新しいユーザーには、**ライセンスとサービスを使用できる**アクセス許可が自動的に割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="b0796-151">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



