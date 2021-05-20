---
title: 顧客アカウントに複数のユーザーを追加する
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客のアカウントに複数のユーザーを追加するには、コンマ区切り値 (.csv) ファイル形式を使用して パートナー センター にデータ ファイルをアップロードします。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150473"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="c8216-103">ユーザーの .csv ファイルを顧客のアカウントにアップロードする</span><span class="sxs-lookup"><span data-stu-id="c8216-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="c8216-104">**適切なロール**: グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="c8216-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="c8216-105">コンマ区切り値ファイル形式 (.csv) のデータ ファイルを パートナー センター にアップロードして、複数のユーザーを顧客のアカウントに一度に追加します。</span><span class="sxs-lookup"><span data-stu-id="c8216-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="c8216-106">顧客ユーザーのファイルを作成し、顧客アカウントにアップロードする</span><span class="sxs-lookup"><span data-stu-id="c8216-106">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="c8216-107">以下に説明するデータを使用して、コンマ区切り値 (.csv) データ ファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="c8216-107">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="c8216-108">後の手順を参照できるように、ファイルを保存します。</span><span class="sxs-lookup"><span data-stu-id="c8216-108">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="c8216-109">顧客 [アカウントの複数のユーザーをインポートするには、「.csv ファイルのフィールド」を参照してください](file-customer-users.md)。</span><span class="sxs-lookup"><span data-stu-id="c8216-109">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="c8216-110">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="c8216-110">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="c8216-111">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="c8216-111">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="c8216-112">顧客の [ユーザーとライセンス] **タブを選択し** 、[ユーザーのアップロード] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="c8216-112">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="c8216-113">**[ユーザー情報のアップロード]** の **[参照]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="c8216-113">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="c8216-114">ファイル セレクターで、データ ファイルを選び、**[開く]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="c8216-114">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="c8216-115">**[検証]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c8216-115">Select **Validate**.</span></span>

    <span data-ttu-id="c8216-116">**注:** ほとんどのアカウント作成エラーは、データ ファイルの問題が原因です。情報が不足している、メール アドレスの形式が正しくないか、重複している、ファイル内のレコードが多すぎるなどです。</span><span class="sxs-lookup"><span data-stu-id="c8216-116">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="c8216-117">パートナー センターでファイルが検証された後、新しいユーザーの地理的な **場所** を選びます。</span><span class="sxs-lookup"><span data-stu-id="c8216-117">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="c8216-118">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c8216-118">Select **Save**.</span></span>
10. <span data-ttu-id="c8216-119">ユーザーの一時パスワードの情報をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="c8216-119">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="c8216-120">一時的なパスワードを含むファイルは必ずこのときにダウンロードしてください。後でこの操作を行うことはできません。</span><span class="sxs-lookup"><span data-stu-id="c8216-120">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="c8216-121">新しいユーザーは、新しいアカウントの一時的なパスワードを使用して、新しいアカウントにログインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8216-121">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="c8216-122">新しいユーザーには、ライセンスとサービスを使用できる **のアクセス許可が自動的に割り当てられます**。</span><span class="sxs-lookup"><span data-stu-id="c8216-122">New users are automatically assigned permissions of **Can use licenses and services**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="c8216-123">次のステップ</span><span class="sxs-lookup"><span data-stu-id="c8216-123">Next steps</span></span>

- [<span data-ttu-id="c8216-124">顧客に独自の製品パートナー センター購入するアクセス許可を付与する</span><span class="sxs-lookup"><span data-stu-id="c8216-124">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
