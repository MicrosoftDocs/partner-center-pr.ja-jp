---
title: CPOR アソシエーションの概要
description: パートナーのパートナーリソース (CPOR) モデルを使用して顧客を特定のインセンティブプログラムに関連付ける必要がある場合は、パートナーリソースについてお読みください。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
ms.topic: conceptual
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 08/10/2020
ms.openlocfilehash: cb9f5b6b6ddfbd9da90543152ee23ce6673ea720
ms.sourcegitcommit: 9d3f88f7008a2771b02cb4af860c6ca00eb50e42
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/17/2020
ms.locfileid: "88303238"
---
# <a name="use-these-resources-to-make-customer-association-claims-for-specific-microsoft-incentives-programs"></a><span data-ttu-id="851d9-103">これらのリソースを使用して、特定の Microsoft インセンティブプログラムに対する顧客の関連付けの要求を行う</span><span class="sxs-lookup"><span data-stu-id="851d9-103">Use these resources to make customer association claims for specific Microsoft incentives programs</span></span>

<span data-ttu-id="851d9-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="851d9-104">**Applies to**</span></span>

- <span data-ttu-id="851d9-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="851d9-105">Partner Center</span></span>
- <span data-ttu-id="851d9-106">Microsoft Partner Network のパートナー (MPN)</span><span class="sxs-lookup"><span data-stu-id="851d9-106">Partners in the Microsoft Partner Network (MPN)</span></span>

<span data-ttu-id="851d9-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="851d9-107">**Appropriate roles**</span></span>

- <span data-ttu-id="851d9-108">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="851d9-108">Incentives admin</span></span>
- <span data-ttu-id="851d9-109">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="851d9-109">Incentives user</span></span>

<span data-ttu-id="851d9-110">この記事では、次の条件を満たす Microsoft パートナー向けのリソースを共有します。</span><span class="sxs-lookup"><span data-stu-id="851d9-110">This article shares resources for Microsoft partners who meet the following criteria:</span></span>

- <span data-ttu-id="851d9-111">Microsoft インセンティブプログラム: オンラインサービスアドバイザリ (OSA) によって販売されています。オンラインサービスの使用状況 (OSU)-Microsoft 365;そして、OSU-ビジネスアプリケーションインセンティブ。</span><span class="sxs-lookup"><span data-stu-id="851d9-111">You are part of the following, Microsoft incentives programs: Online Services Advisory (OSA) Sell; Online Services Usage (OSU)-Microsoft 365; and, OSU-Business Application incentives.</span></span>

- <span data-ttu-id="851d9-112">Microsoft 365 または Dynamics 365 のお客様と協力して、上記のインセンティブプログラムでこのような作業の一部を参照または要求したいと考えています。</span><span class="sxs-lookup"><span data-stu-id="851d9-112">You work with Microsoft 365 or Dynamics 365 customers and want to reference or claim some of this work in the above incentive programs.</span></span>

<span data-ttu-id="851d9-113">条件に適合する場合は、要求パートナーのレコード (CPOR) モデルを使用して、これらのインセンティブプログラムの顧客の関連付けを作成および管理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="851d9-113">If you fit the criteria, you need to use the Claiming Partner of Record (CPOR) model to create and manage customer associations for these incentives programs.</span></span>
 
## <a name="how-do-customer-associations-and-cpor-relate-to-incentives"></a><span data-ttu-id="851d9-114">顧客の関連付けと CPOR はインセンティブとの関係はどのようなものですか?</span><span class="sxs-lookup"><span data-stu-id="851d9-114">How do customer associations and CPOR relate to incentives?</span></span>

<span data-ttu-id="851d9-115">Microsoft は、要求されたパートナーのレコード (CPOR) モデルを使用して、Microsoft 365 と Dynamics 365 の顧客との関連付けを管理するようになりました。</span><span class="sxs-lookup"><span data-stu-id="851d9-115">Microsoft now uses the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers.</span></span>

<span data-ttu-id="851d9-116">このモデルは、次のインセンティブプログラムにおけるお客様の作業に適用されます: オンラインサービスアドバイザリ (OSA) 販売オンラインサービスの使用状況 (OSU)-Microsoft 365;そして、OSU-ビジネスアプリケーションインセンティブ。</span><span class="sxs-lookup"><span data-stu-id="851d9-116">This model applies to your work with customers in the following incentives programs: Online Services Advisory (OSA) Sell; Online Services Usage (OSU)-Microsoft 365; and, OSU-Business Application incentives.</span></span>

<span data-ttu-id="851d9-117">Microsoft はすべてのインセンティブ要求を検証します。</span><span class="sxs-lookup"><span data-stu-id="851d9-117">Microsoft validates all incentives claims.</span></span>

<span data-ttu-id="851d9-118">この時点で、詳細を確認するメッセージが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="851d9-118">At this point, we may ask you for more information.</span></span> <span data-ttu-id="851d9-119">また、お客様にアソシエーション要求を通知します。</span><span class="sxs-lookup"><span data-stu-id="851d9-119">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="851d9-120">お客様は、5営業日以内にオプトアウトできます。オプトアウトされていない場合は、この特定のテナントとワークロードとの関連付けが公式になります。</span><span class="sxs-lookup"><span data-stu-id="851d9-120">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span>

<span data-ttu-id="851d9-121">顧客は、アソシエーションの要求を受け入れることによって、管理サービスを提供できるように、データの一部にアクセスすることができます。</span><span class="sxs-lookup"><span data-stu-id="851d9-121">By accepting your request for association, the customer is giving you access to some of their data so you can provide management services to them.</span></span> 

## <a name="resources-to-help-you-create-and-manage-customer-associations"></a><span data-ttu-id="851d9-122">顧客の関連付けの作成と管理に役立つリソース</span><span class="sxs-lookup"><span data-stu-id="851d9-122">Resources to help you create and manage customer associations</span></span>

<span data-ttu-id="851d9-123">以下の記事では、顧客の関連付けを作成、管理、およびトラブルシューティングする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="851d9-123">The below articles tell you how to create, manage, and troubleshoot customer associations.</span></span>

|  <span data-ttu-id="851d9-124">**目的**</span><span class="sxs-lookup"><span data-stu-id="851d9-124">**To do this**</span></span>  |  <span data-ttu-id="851d9-125">**参照先**</span><span class="sxs-lookup"><span data-stu-id="851d9-125">**Read this**</span></span>  |
|--------------|-----------|
| <span data-ttu-id="851d9-126">顧客の関連付けを作成する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="851d9-126">Learn how to create a customer association</span></span>  | [<span data-ttu-id="851d9-127">CPOR モデルを使用して顧客の関連付けを作成する</span><span class="sxs-lookup"><span data-stu-id="851d9-127">Create a customer association using the CPOR model</span></span>](submit-osa-claim.md)  |
|<span data-ttu-id="851d9-128">顧客の関連付けを管理する方法を理解する</span><span class="sxs-lookup"><span data-stu-id="851d9-128">Understand how to manage your customer associations</span></span>  | [<span data-ttu-id="851d9-129">顧客の関連付けを管理する</span><span class="sxs-lookup"><span data-stu-id="851d9-129">Manage customer associations</span></span>](incentives-manage-customer-associations.md)  |
|<span data-ttu-id="851d9-130">顧客の関連付けに関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="851d9-130">Troubleshoot any customer association issues</span></span>  | [<span data-ttu-id="851d9-131">顧客の関連付けに関する問題</span><span class="sxs-lookup"><span data-stu-id="851d9-131">Customer association issues</span></span>](incentives-customer-association-issues.md)  |

## <a name="next-steps"></a><span data-ttu-id="851d9-132">次の手順</span><span class="sxs-lookup"><span data-stu-id="851d9-132">Next steps</span></span>

- <span data-ttu-id="851d9-133">インセンティブは初めてですか?</span><span class="sxs-lookup"><span data-stu-id="851d9-133">New to incentives?</span></span> <span data-ttu-id="851d9-134">[作業を開始](incentives-get-started-intro.md)するために必要なものを見つける</span><span class="sxs-lookup"><span data-stu-id="851d9-134">Discover what you need to [get started](incentives-get-started-intro.md)</span></span>
- <span data-ttu-id="851d9-135">[インセンティブ共同要求の](claims-overview.md)詳細情報</span><span class="sxs-lookup"><span data-stu-id="851d9-135">Learn more about [incentives co-op claims](claims-overview.md)</span></span>
