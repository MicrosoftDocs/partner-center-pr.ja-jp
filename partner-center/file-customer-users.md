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
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441423"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="5108c-103">.Csv ファイルを作成して顧客アカウントに複数のユーザーを追加する</span><span class="sxs-lookup"><span data-stu-id="5108c-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="5108c-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="5108c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="5108c-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="5108c-105">Global admin</span></span>

<span data-ttu-id="5108c-106">コンマ区切り値ファイル形式 (.csv) のデータファイルをパートナーセンターにアップロードすることで、顧客のアカウントに複数のユーザーを一度に追加します。</span><span class="sxs-lookup"><span data-stu-id="5108c-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="5108c-107">パートナー センターからサンプル データ ファイルをダウンロードし、それを編集して使用することも、以下に定義するデータ モデルを使用して新しいデータ ファイルを作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="5108c-107">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="5108c-108">データ ファイルの要件</span><span class="sxs-lookup"><span data-stu-id="5108c-108">Data file requirements</span></span>

<span data-ttu-id="5108c-109">一括アップロードプロセスを使用して顧客のアカウントに複数のユーザーを追加するには、次の要件を満たす必要があります。</span><span class="sxs-lookup"><span data-stu-id="5108c-109">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="5108c-110">顧客アカウントに対してグローバル管理者のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="5108c-110">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="5108c-111">各ユーザーは、顧客の電子メール ドメインに追加された、一意のメール アドレスを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5108c-111">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="5108c-112">一度に最大 100 個のレコードをアップロードすることができます。</span><span class="sxs-lookup"><span data-stu-id="5108c-112">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="5108c-113">100 を超えるユーザーを追加する必要がある場合は、追加のデータ ファイルを作成してアップロードします。</span><span class="sxs-lookup"><span data-stu-id="5108c-113">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="5108c-114">すべてのユーザーは、地理的に同じ **場所** にいる必要があります。</span><span class="sxs-lookup"><span data-stu-id="5108c-114">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="5108c-115">次に示すデータのみを入力します。</span><span class="sxs-lookup"><span data-stu-id="5108c-115">Enter only the data described below.</span></span> <span data-ttu-id="5108c-116">余分なデータがあると、アップロードに失敗します。</span><span class="sxs-lookup"><span data-stu-id="5108c-116">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="5108c-117">データ ファイルに、次のデータを入力します。</span><span class="sxs-lookup"><span data-stu-id="5108c-117">Enter the following data in the data file:</span></span>

| <span data-ttu-id="5108c-118">**列名**</span><span class="sxs-lookup"><span data-stu-id="5108c-118">**Column name**</span></span> | <span data-ttu-id="5108c-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="5108c-119">**Description**</span></span>  | <span data-ttu-id="5108c-120">**制限事項**</span><span class="sxs-lookup"><span data-stu-id="5108c-120">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="5108c-121">名</span><span class="sxs-lookup"><span data-stu-id="5108c-121">First name</span></span>  | <span data-ttu-id="5108c-122">ユーザーの名 (オプションフィールド)</span><span class="sxs-lookup"><span data-stu-id="5108c-122">User's first name (optional field)</span></span>  | <span data-ttu-id="5108c-123">50 字以内</span><span class="sxs-lookup"><span data-stu-id="5108c-123">50-character limit</span></span>  |
| <span data-ttu-id="5108c-124">姓</span><span class="sxs-lookup"><span data-stu-id="5108c-124">Last name</span></span>  | <span data-ttu-id="5108c-125">ユーザーの姓 (省略可能なフィールド)</span><span class="sxs-lookup"><span data-stu-id="5108c-125">User's last name (optional field)</span></span>  | <span data-ttu-id="5108c-126">50 字以内</span><span class="sxs-lookup"><span data-stu-id="5108c-126">50-character limit</span></span>  |
| <span data-ttu-id="5108c-127">Display name</span><span class="sxs-lookup"><span data-stu-id="5108c-127">Display name</span></span>    | <span data-ttu-id="5108c-128">パートナー センターで表示される名前 (必須フィールド)</span><span class="sxs-lookup"><span data-stu-id="5108c-128">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="5108c-129">50 字以内</span><span class="sxs-lookup"><span data-stu-id="5108c-129">50-character limit</span></span>                         |
| <span data-ttu-id="5108c-130">Email</span><span class="sxs-lookup"><span data-stu-id="5108c-130">Email</span></span>   | <span data-ttu-id="5108c-131">顧客会社のユーザーの勤務先の電子メールアドレス (必須フィールド)</span><span class="sxs-lookup"><span data-stu-id="5108c-131">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="5108c-132">各ユーザーに一意の電子メール アドレスが必要</span><span class="sxs-lookup"><span data-stu-id="5108c-132">Each user must have a unique email address</span></span> |
| <span data-ttu-id="5108c-133">状態の更新</span><span class="sxs-lookup"><span data-stu-id="5108c-133">Status update</span></span>   | <span data-ttu-id="5108c-134">新しいユーザーレコードが正常に作成されたかどうかを示すために使用されます</span><span class="sxs-lookup"><span data-stu-id="5108c-134">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="5108c-135">\*\*空白のままにする\*\*</span><span class="sxs-lookup"><span data-stu-id="5108c-135">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="5108c-136">次のステップ</span><span class="sxs-lookup"><span data-stu-id="5108c-136">Next steps</span></span>

- [<span data-ttu-id="5108c-137">顧客に複数ユーザーを追加する方法</span><span class="sxs-lookup"><span data-stu-id="5108c-137">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)