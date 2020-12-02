---
title: 顧客アカウントに複数のユーザーを追加する
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客のアカウントに複数のユーザーを追加するには、コンマ区切り値 (.csv) ファイル形式を使用して、パートナーセンターにデータファイルをアップロードします。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9f1d6e2a59bd892b7b79a1e3aa532242cdd0e302
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474191"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="f9882-103">ユーザーの .csv ファイルを顧客のアカウントにアップロードする</span><span class="sxs-lookup"><span data-stu-id="f9882-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="f9882-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="f9882-104">**Appropriate roles**</span></span>

- <span data-ttu-id="f9882-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="f9882-105">Global admin</span></span>

<span data-ttu-id="f9882-106">コンマ区切り値ファイル形式 (.csv) のデータファイルをパートナーセンターにアップロードすることで、顧客のアカウントに複数のユーザーを一度に追加します。</span><span class="sxs-lookup"><span data-stu-id="f9882-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="f9882-107">顧客ユーザーのファイルを作成し、顧客アカウントにアップロードする</span><span class="sxs-lookup"><span data-stu-id="f9882-107">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="f9882-108">以下に説明するデータを使用して、コンマ区切り値 (.csv) データ ファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="f9882-108">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="f9882-109">後の手順を参照できるように、ファイルを保存します。</span><span class="sxs-lookup"><span data-stu-id="f9882-109">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="f9882-110">[顧客アカウントの複数のユーザーをインポートする場合は、「.csv ファイルのフィールド」を](file-customer-users.md)参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9882-110">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="f9882-111">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="f9882-111">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="f9882-112">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="f9882-112">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="f9882-113">顧客の [ **ユーザーとライセンス** ] タブを選択し、[ **ユーザーのアップロード**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="f9882-113">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="f9882-114">**[ユーザー情報のアップロード]** の **[参照]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="f9882-114">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="f9882-115">ファイル セレクターで、データ ファイルを選び、**[開く]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="f9882-115">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="f9882-116">**[検証]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="f9882-116">Select **Validate**.</span></span>

    <span data-ttu-id="f9882-117">**注:** ほとんどのアカウント作成エラーは、データ ファイルの問題が原因です。情報が不足している、メール アドレスの形式が正しくないか、重複している、ファイル内のレコードが多すぎるなどです。</span><span class="sxs-lookup"><span data-stu-id="f9882-117">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="f9882-118">パートナー センターでファイルが検証された後、新しいユーザーの地理的な **場所** を選びます。</span><span class="sxs-lookup"><span data-stu-id="f9882-118">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="f9882-119">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="f9882-119">Select **Save**.</span></span>
10. <span data-ttu-id="f9882-120">ユーザーの一時パスワードの情報をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="f9882-120">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="f9882-121">一時的なパスワードを含むファイルは必ずこのときにダウンロードしてください。後でこの操作を行うことはできません。</span><span class="sxs-lookup"><span data-stu-id="f9882-121">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="f9882-122">新しいユーザーは、新しいアカウントの一時的なパスワードを使用して、新しいアカウントにログインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="f9882-122">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="f9882-123">新しいユーザーには、**ライセンスとサービスを使用できる** アクセス許可が自動的に割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="f9882-123">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

## <a name="next-steps"></a><span data-ttu-id="f9882-124">次のステップ</span><span class="sxs-lookup"><span data-stu-id="f9882-124">Next steps</span></span>

- [<span data-ttu-id="f9882-125">パートナーセンターで自分の製品またはサービスを購入するためのアクセス許可を顧客に付与する</span><span class="sxs-lookup"><span data-stu-id="f9882-125">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
