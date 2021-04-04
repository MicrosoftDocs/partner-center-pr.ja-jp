---
title: CPOR アソシエーションの概要
description: パートナー向けのリソース (CPOR) モデルを使用して、顧客を特定のインセンティブプログラムに関連付ける必要があるパートナー向けのリソースについて説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
ms.topic: conceptual
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: 24c439d1c90663130e1676e8ceb6d503be5ea30d
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/02/2021
ms.locfileid: "106179192"
---
# <a name="use-these-resources-to-make-customer-association-claims-for-specific-incentives-programs"></a><span data-ttu-id="46218-103">これらのリソースを使用して、特定のインセンティブプログラムに対する顧客の関連付けの要求を行う</span><span class="sxs-lookup"><span data-stu-id="46218-103">Use these resources to make customer association claims for specific incentives programs</span></span>

<span data-ttu-id="46218-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="46218-104">**Appropriate roles**</span></span>

- <span data-ttu-id="46218-105">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="46218-105">Incentives admin</span></span>
- <span data-ttu-id="46218-106">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="46218-106">Incentives user</span></span>

<span data-ttu-id="46218-107">この記事では、次の条件を満たす Microsoft パートナー向けのリソースを共有します。</span><span class="sxs-lookup"><span data-stu-id="46218-107">This article shares resources for Microsoft partners who meet the following criteria:</span></span>

- <span data-ttu-id="46218-108">Microsoft のインセンティブプログラムの一部であるオンラインサービスアドバイザリ (OSA) 販売、Online Services Usage (OSU)-Microsoft 365、OSU-Business アプリケーションインセンティブ。</span><span class="sxs-lookup"><span data-stu-id="46218-108">You are part of the following Microsoft incentives programs: Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

- <span data-ttu-id="46218-109">Microsoft 365 または Dynamics 365 のお客様と協力して、上記のインセンティブプログラムでこのような作業の一部を参照または要求したいと考えています。</span><span class="sxs-lookup"><span data-stu-id="46218-109">You work with Microsoft 365 or Dynamics 365 customers and want to reference or claim some of this work in the above incentive programs.</span></span>

<span data-ttu-id="46218-110">条件に適合する場合は、要求パートナーのレコード (CPOR) モデルを使用して、これらのインセンティブプログラムの顧客の関連付けを作成および管理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="46218-110">If you fit the criteria, you need to use the Claiming Partner of Record (CPOR) model to create and manage customer associations for these incentives programs.</span></span>
 
## <a name="how-do-customer-associations-and-cpor-relate-to-incentives"></a><span data-ttu-id="46218-111">顧客の関連付けと CPOR はインセンティブとの関係はどのようなものですか?</span><span class="sxs-lookup"><span data-stu-id="46218-111">How do customer associations and CPOR relate to incentives?</span></span>

<span data-ttu-id="46218-112">Microsoft は、要求されたパートナーのレコード (CPOR) モデルを使用して、Microsoft 365 と Dynamics 365 の顧客との関連付けを管理するようになりました。</span><span class="sxs-lookup"><span data-stu-id="46218-112">Microsoft now uses the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers.</span></span>

<span data-ttu-id="46218-113">このモデルは、オンラインサービスアドバイザリ (OSA) 販売、Online Services Usage (OSU)-Microsoft 365、および OSU-Business アプリケーションインセンティブの各インセンティブプログラムのお客様との作業に適用されます。</span><span class="sxs-lookup"><span data-stu-id="46218-113">This model applies to your work with customers in the following incentives programs: Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

<span data-ttu-id="46218-114">Microsoft はすべてのインセンティブ要求を検証します。</span><span class="sxs-lookup"><span data-stu-id="46218-114">Microsoft validates all incentives claims.</span></span>

<span data-ttu-id="46218-115">この時点で、詳細を確認するメッセージが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="46218-115">At this point, we may ask you for more information.</span></span> <span data-ttu-id="46218-116">また、お客様にアソシエーション要求を通知します。</span><span class="sxs-lookup"><span data-stu-id="46218-116">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="46218-117">お客様は、5営業日以内にオプトアウトできます。オプトアウトされていない場合は、この特定のテナントとワークロードとの関連付けが公式になります。</span><span class="sxs-lookup"><span data-stu-id="46218-117">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span>

<span data-ttu-id="46218-118">顧客は、アソシエーションの要求を受け入れることによって、管理サービスを提供できるように、データの一部にアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="46218-118">By accepting your request for association, the customer is giving you access to some of their data so you can provide management services to them.</span></span> 

## <a name="resources-to-help-you-create-and-manage-customer-associations"></a><span data-ttu-id="46218-119">顧客の関連付けの作成と管理に役立つリソース</span><span class="sxs-lookup"><span data-stu-id="46218-119">Resources to help you create and manage customer associations</span></span>

<span data-ttu-id="46218-120">以下の記事では、顧客の関連付けを作成、管理、およびトラブルシューティングする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="46218-120">The below articles tell you how to create, manage, and troubleshoot customer associations.</span></span>

|  <span data-ttu-id="46218-121">**目的**</span><span class="sxs-lookup"><span data-stu-id="46218-121">**To do this**</span></span>  |  <span data-ttu-id="46218-122">**参照先**</span><span class="sxs-lookup"><span data-stu-id="46218-122">**Read this**</span></span>  |
|--------------|-----------|
| <span data-ttu-id="46218-123">顧客の関連付けを作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="46218-123">Learn how to create a customer association</span></span>  | [<span data-ttu-id="46218-124">CPOR モデルを使用して顧客の関連付けを作成する</span><span class="sxs-lookup"><span data-stu-id="46218-124">Create a customer association using the CPOR model</span></span>](submit-osa-claim.md)  |
|<span data-ttu-id="46218-125">顧客の関連付けを管理する方法を理解する</span><span class="sxs-lookup"><span data-stu-id="46218-125">Understand how to manage your customer associations</span></span>  | [<span data-ttu-id="46218-126">顧客の関連付けを管理する</span><span class="sxs-lookup"><span data-stu-id="46218-126">Manage customer associations</span></span>](incentives-manage-customer-associations.md)  |
|<span data-ttu-id="46218-127">顧客の関連付けに関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="46218-127">Troubleshoot any customer association issues</span></span>  | [<span data-ttu-id="46218-128">顧客の関連付けに関する問題</span><span class="sxs-lookup"><span data-stu-id="46218-128">Customer association issues</span></span>](incentives-customer-association-issues.md)  |

## <a name="next-steps"></a><span data-ttu-id="46218-129">次のステップ</span><span class="sxs-lookup"><span data-stu-id="46218-129">Next steps</span></span>

- <span data-ttu-id="46218-130">インセンティブは初めてですか?</span><span class="sxs-lookup"><span data-stu-id="46218-130">New to incentives?</span></span> <span data-ttu-id="46218-131">[作業を開始](incentives-get-started-intro.md)するために必要なものを見つける</span><span class="sxs-lookup"><span data-stu-id="46218-131">Discover what you need to [get started](incentives-get-started-intro.md)</span></span>
- <span data-ttu-id="46218-132">[インセンティブ共同要求の](claims-overview.md)詳細情報</span><span class="sxs-lookup"><span data-stu-id="46218-132">Learn more about [incentives co-op claims](claims-overview.md)</span></span>
