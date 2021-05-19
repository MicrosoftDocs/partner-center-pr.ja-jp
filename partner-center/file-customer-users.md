---
title: 顧客アカウントの複数のユーザーをインポートする .csv ファイルのフィールド
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客アカウントに複数のユーザーを追加するには、適切なフィールドを含むコンマ区切り値 (.csv) ファイルを作成します。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150983"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="7221f-103">.csv ファイルを作成して複数のユーザーを顧客アカウントに追加する</span><span class="sxs-lookup"><span data-stu-id="7221f-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="7221f-104">**適切なロール**: グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="7221f-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="7221f-105">コンマ区切り値ファイル形式 (.csv) のデータ ファイルを パートナー センター にアップロードして、複数のユーザーを顧客のアカウントに一度に追加します。</span><span class="sxs-lookup"><span data-stu-id="7221f-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="7221f-106">パートナー センターからサンプル データ ファイルをダウンロードし、それを編集して使用することも、以下に定義するデータ モデルを使用して新しいデータ ファイルを作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="7221f-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="7221f-107">データ ファイルの要件</span><span class="sxs-lookup"><span data-stu-id="7221f-107">Data file requirements</span></span>

<span data-ttu-id="7221f-108">一括アップロード プロセスを使用して複数のユーザーを顧客のアカウントに追加するには、次の要件を満たす必要があります。</span><span class="sxs-lookup"><span data-stu-id="7221f-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="7221f-109">顧客アカウントに対してグローバル管理者のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="7221f-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="7221f-110">各ユーザーは、顧客の電子メール ドメインに追加された、一意のメール アドレスを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7221f-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="7221f-111">一度に最大 100 個のレコードをアップロードすることができます。</span><span class="sxs-lookup"><span data-stu-id="7221f-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="7221f-112">100 を超えるユーザーを追加する必要がある場合は、追加のデータ ファイルを作成してアップロードします。</span><span class="sxs-lookup"><span data-stu-id="7221f-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="7221f-113">すべてのユーザーは、地理的に同じ **場所** にいる必要があります。</span><span class="sxs-lookup"><span data-stu-id="7221f-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="7221f-114">次に示すデータのみを入力します。</span><span class="sxs-lookup"><span data-stu-id="7221f-114">Enter only the data described below.</span></span> <span data-ttu-id="7221f-115">余分なデータがあると、アップロードに失敗します。</span><span class="sxs-lookup"><span data-stu-id="7221f-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="7221f-116">データ ファイルに、次のデータを入力します。</span><span class="sxs-lookup"><span data-stu-id="7221f-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="7221f-117">**列名**</span><span class="sxs-lookup"><span data-stu-id="7221f-117">**Column name**</span></span> | <span data-ttu-id="7221f-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="7221f-118">**Description**</span></span>  | <span data-ttu-id="7221f-119">**制限事項**</span><span class="sxs-lookup"><span data-stu-id="7221f-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="7221f-120">名</span><span class="sxs-lookup"><span data-stu-id="7221f-120">First name</span></span>  | <span data-ttu-id="7221f-121">ユーザーの名 (省略可能なフィールド)</span><span class="sxs-lookup"><span data-stu-id="7221f-121">User's first name (optional field)</span></span>  | <span data-ttu-id="7221f-122">50 字以内</span><span class="sxs-lookup"><span data-stu-id="7221f-122">50-character limit</span></span>  |
| <span data-ttu-id="7221f-123">姓</span><span class="sxs-lookup"><span data-stu-id="7221f-123">Last name</span></span>  | <span data-ttu-id="7221f-124">ユーザーの姓 (省略可能なフィールド)</span><span class="sxs-lookup"><span data-stu-id="7221f-124">User's last name (optional field)</span></span>  | <span data-ttu-id="7221f-125">50 字以内</span><span class="sxs-lookup"><span data-stu-id="7221f-125">50-character limit</span></span>  |
| <span data-ttu-id="7221f-126">表示名</span><span class="sxs-lookup"><span data-stu-id="7221f-126">Display name</span></span>    | <span data-ttu-id="7221f-127">パートナー センターで表示される名前 (必須フィールド)</span><span class="sxs-lookup"><span data-stu-id="7221f-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="7221f-128">50 字以内</span><span class="sxs-lookup"><span data-stu-id="7221f-128">50-character limit</span></span>                         |
| <span data-ttu-id="7221f-129">電子メール</span><span class="sxs-lookup"><span data-stu-id="7221f-129">Email</span></span>   | <span data-ttu-id="7221f-130">顧客企業のユーザーのビジネス 用メール アドレス (必須フィールド)</span><span class="sxs-lookup"><span data-stu-id="7221f-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="7221f-131">各ユーザーに一意の電子メール アドレスが必要</span><span class="sxs-lookup"><span data-stu-id="7221f-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="7221f-132">状態の更新</span><span class="sxs-lookup"><span data-stu-id="7221f-132">Status update</span></span>   | <span data-ttu-id="7221f-133">新しいユーザー レコードが正常に作成されたかどうかを示すために使用されます</span><span class="sxs-lookup"><span data-stu-id="7221f-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="7221f-134">\*\*空白のままにする\*\*</span><span class="sxs-lookup"><span data-stu-id="7221f-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="7221f-135">次のステップ</span><span class="sxs-lookup"><span data-stu-id="7221f-135">Next steps</span></span>

- [<span data-ttu-id="7221f-136">顧客に複数ユーザーを追加する方法</span><span class="sxs-lookup"><span data-stu-id="7221f-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)