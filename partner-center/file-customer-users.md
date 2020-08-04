---
title: 顧客アカウントの複数のユーザーをインポートするための .csv ファイルのフィールド
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客アカウントに複数のユーザーを追加するには、適切なフィールドを含むコンマ区切り値 (.csv) ファイルを作成します。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2020
ms.locfileid: "87528182"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="f3421-103">.Csv ファイルを作成して顧客アカウントに複数のユーザーを追加する</span><span class="sxs-lookup"><span data-stu-id="f3421-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="f3421-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="f3421-104">**Applies to**</span></span>

- <span data-ttu-id="f3421-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="f3421-105">Partner Center</span></span>

<span data-ttu-id="f3421-106">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="f3421-106">**Appropriate roles**</span></span>

- <span data-ttu-id="f3421-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="f3421-107">Global admin</span></span>

<span data-ttu-id="f3421-108">コンマ区切り値ファイル形式 (.csv) のデータファイルをパートナーセンターにアップロードすることで、顧客のアカウントに複数のユーザーを一度に追加します。</span><span class="sxs-lookup"><span data-stu-id="f3421-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="f3421-109">パートナー センターからサンプル データ ファイルをダウンロードし、それを編集して使用することも、以下に定義するデータ モデルを使用して新しいデータ ファイルを作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="f3421-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="f3421-110">データ ファイルの要件</span><span class="sxs-lookup"><span data-stu-id="f3421-110">Data file requirements</span></span>

<span data-ttu-id="f3421-111">一括アップロードプロセスを使用して顧客のアカウントに複数のユーザーを追加するには、次の要件を満たす必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3421-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="f3421-112">顧客アカウントに対してグローバル管理者のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3421-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="f3421-113">各ユーザーは、顧客の電子メール ドメインに追加された、一意のメール アドレスを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3421-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="f3421-114">一度に最大 100 個のレコードをアップロードすることができます。</span><span class="sxs-lookup"><span data-stu-id="f3421-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="f3421-115">100 を超えるユーザーを追加する必要がある場合は、追加のデータ ファイルを作成してアップロードします。</span><span class="sxs-lookup"><span data-stu-id="f3421-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="f3421-116">すべてのユーザーは、地理的に同じ**場所**にいる必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3421-116">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="f3421-117">次に示すデータのみを入力します。</span><span class="sxs-lookup"><span data-stu-id="f3421-117">Enter only the data described below.</span></span> <span data-ttu-id="f3421-118">余分なデータがあると、アップロードに失敗します。</span><span class="sxs-lookup"><span data-stu-id="f3421-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="f3421-119">データ ファイルに、次のデータを入力します。</span><span class="sxs-lookup"><span data-stu-id="f3421-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="f3421-120">**列名**</span><span class="sxs-lookup"><span data-stu-id="f3421-120">**Column name**</span></span> | <span data-ttu-id="f3421-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="f3421-121">**Description**</span></span>  | <span data-ttu-id="f3421-122">**制限事項**</span><span class="sxs-lookup"><span data-stu-id="f3421-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="f3421-123">名</span><span class="sxs-lookup"><span data-stu-id="f3421-123">First name</span></span>  | <span data-ttu-id="f3421-124">ユーザーの名 (オプションフィールド)</span><span class="sxs-lookup"><span data-stu-id="f3421-124">User's first name (optional field)</span></span>  | <span data-ttu-id="f3421-125">50 字以内</span><span class="sxs-lookup"><span data-stu-id="f3421-125">50-character limit</span></span>  |
| <span data-ttu-id="f3421-126">姓</span><span class="sxs-lookup"><span data-stu-id="f3421-126">Last name</span></span>  | <span data-ttu-id="f3421-127">ユーザーの姓 (省略可能なフィールド)</span><span class="sxs-lookup"><span data-stu-id="f3421-127">User's last name (optional field)</span></span>  | <span data-ttu-id="f3421-128">50 字以内</span><span class="sxs-lookup"><span data-stu-id="f3421-128">50-character limit</span></span>  |
| <span data-ttu-id="f3421-129">表示名</span><span class="sxs-lookup"><span data-stu-id="f3421-129">Display name</span></span>    | <span data-ttu-id="f3421-130">パートナー センターで表示される名前 (必須フィールド)</span><span class="sxs-lookup"><span data-stu-id="f3421-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="f3421-131">50 字以内</span><span class="sxs-lookup"><span data-stu-id="f3421-131">50-character limit</span></span>                         |
| <span data-ttu-id="f3421-132">電子メール</span><span class="sxs-lookup"><span data-stu-id="f3421-132">Email</span></span>   | <span data-ttu-id="f3421-133">顧客会社のユーザーの勤務先の電子メールアドレス (必須フィールド)</span><span class="sxs-lookup"><span data-stu-id="f3421-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="f3421-134">各ユーザーに一意の電子メール アドレスが必要</span><span class="sxs-lookup"><span data-stu-id="f3421-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="f3421-135">状態の更新</span><span class="sxs-lookup"><span data-stu-id="f3421-135">Status update</span></span>   | <span data-ttu-id="f3421-136">新しいユーザー レコードが正常に作成されたかどうかを示すために使用される</span><span class="sxs-lookup"><span data-stu-id="f3421-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="f3421-137">\*\*空白のままにする\*\*</span><span class="sxs-lookup"><span data-stu-id="f3421-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="f3421-138">次の手順</span><span class="sxs-lookup"><span data-stu-id="f3421-138">Next steps</span></span>

- [<span data-ttu-id="f3421-139">顧客に複数のユーザーを追加する方法</span><span class="sxs-lookup"><span data-stu-id="f3421-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)