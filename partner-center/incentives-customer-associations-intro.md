---
title: CPOR アソシエーションの概要
description: パートナー向けのリソース (CPOR) モデルを使用して、顧客を特定のインセンティブプログラムに関連付ける必要があるパートナー向けのリソースについて説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
ms.topic: conceptual
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 05/20/2021
ms.openlocfilehash: 9bcdd9e99f9db5271a1ca51dab01c376c938acc9
ms.sourcegitcommit: 75b84d0918802325019577930d368bc3df193ab2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/21/2021
ms.locfileid: "110236085"
---
# <a name="use-these-resources-to-make-customer-association-claims-for-specific-incentives-programs"></a><span data-ttu-id="0ffca-103">これらのリソースを使用して、特定のインセンティブプログラムに対する顧客の関連付けの要求を行う</span><span class="sxs-lookup"><span data-stu-id="0ffca-103">Use these resources to make customer association claims for specific incentives programs</span></span>

<span data-ttu-id="0ffca-104">**適切なロール**: インセンティブ admin |インセンティブユーザー</span><span class="sxs-lookup"><span data-stu-id="0ffca-104">**Appropriate roles**: Incentives admin | Incentives user</span></span>

<span data-ttu-id="0ffca-105">この記事では、次の条件を満たす Microsoft パートナー向けのリソースを共有します。</span><span class="sxs-lookup"><span data-stu-id="0ffca-105">This article shares resources for Microsoft partners who meet the following criteria:</span></span>

- <span data-ttu-id="0ffca-106">Microsoft のインセンティブプログラムの一部であるオンラインサービスアドバイザリ (OSA) 販売、Online Services Usage (OSU)-Microsoft 365、OSU-Business アプリケーションインセンティブ。</span><span class="sxs-lookup"><span data-stu-id="0ffca-106">You are part of the following Microsoft incentives programs: Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

- <span data-ttu-id="0ffca-107">Microsoft 365 または Dynamics 365 のお客様と協力して、上記のインセンティブプログラムでこのような作業の一部を参照または要求したいと考えています。</span><span class="sxs-lookup"><span data-stu-id="0ffca-107">You work with Microsoft 365 or Dynamics 365 customers and want to reference or claim some of this work in the above incentive programs.</span></span>

<span data-ttu-id="0ffca-108">条件に適合する場合は、要求パートナーのレコード (CPOR) モデルを使用して、これらのインセンティブプログラムの顧客の関連付けを作成および管理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0ffca-108">If you fit the criteria, you need to use the Claiming Partner of Record (CPOR) model to create and manage customer associations for these incentives programs.</span></span>

## <a name="explaining-claiming-partner-of-record-cpor-to-customers"></a><span data-ttu-id="0ffca-109">顧客へのレコードのパートナー (CPOR) の説明</span><span class="sxs-lookup"><span data-stu-id="0ffca-109">Explaining Claiming Partner of Record (CPOR) to customers</span></span>

<span data-ttu-id="0ffca-110">CPOR は、お客様がビジネス目標を達成し、クラウドで価値を実現するのを支援しているパートナーを特定し、それを認識できるようにします。</span><span class="sxs-lookup"><span data-stu-id="0ffca-110">CPOR enables Microsoft to identify and recognize those partners who are helping customers achieve business objectives and realize value in the cloud.</span></span> <span data-ttu-id="0ffca-111">パートナーがワークロードまたはサブスクリプションに関連付けられると、使用状況や販売された座席データにアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="0ffca-111">Once a partner associates to a workload or subscription they will obtain access to usage and/or sold seats data.</span></span> <span data-ttu-id="0ffca-112">このようなデータにアクセスすることで、パートナーはアクティブな使用状況を監視しながら、使用率を最大化する方法に関する推奨事項をお客様に提供できます。</span><span class="sxs-lookup"><span data-stu-id="0ffca-112">Access to such data enables partners to monitor active usage while providing customers with recommendations on how to maximize usage.</span></span> <span data-ttu-id="0ffca-113">パートナーは、他の顧客データにアクセスできません。</span><span class="sxs-lookup"><span data-stu-id="0ffca-113">Partners won't have access to any other customer data.</span></span> <span data-ttu-id="0ffca-114">また、CPOR アソシエーションは、Microsoft がサービスプロバイダーのエコシステムを理解するのに役立ちます。また、Microsoft は、一般的なお客様を最適にサポートするために必要なツールとプログラムを調整する方法を決定するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="0ffca-114">Additionally, the CPOR association helps Microsoft understand the ecosystem of service providers, and also helps Microsoft determine how to refine the tools and programs needed to best support our common customers.</span></span> <span data-ttu-id="0ffca-115">顧客に対する操作は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="0ffca-115">There is no action required for the customer.</span></span> <span data-ttu-id="0ffca-116">お客様は、CPOR アソシエーションをオプトアウトすることができます。</span><span class="sxs-lookup"><span data-stu-id="0ffca-116">We allow customers the opportunity to opt-out of a CPOR association.</span></span> <span data-ttu-id="0ffca-117">パートナーからのアソシエーション要求を通知する通知が送信されます。</span><span class="sxs-lookup"><span data-stu-id="0ffca-117">Customers will receive a notification informing them of the association request from partners.</span></span> <span data-ttu-id="0ffca-118">顧客がパートナーとの関連付けを拒否した場合、パートナーはレコードのパートナーとして認識されません。</span><span class="sxs-lookup"><span data-stu-id="0ffca-118">If a customer denies association to a partner, the partner won't be recognized as the partner of record.</span></span>

## <a name="how-do-customer-associations-and-cpor-relate-to-incentives"></a><span data-ttu-id="0ffca-119">顧客の関連付けと CPOR はインセンティブとの関係はどのようなものですか?</span><span class="sxs-lookup"><span data-stu-id="0ffca-119">How do customer associations and CPOR relate to incentives?</span></span>

<span data-ttu-id="0ffca-120">Microsoft では現在、指名パートナーの指定 (CPOR) モデルを使用して、お客様の Microsoft 365 Dynamics 365 のお客様との関連付けを管理しています。</span><span class="sxs-lookup"><span data-stu-id="0ffca-120">Microsoft now uses the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers.</span></span>

<span data-ttu-id="0ffca-121">このモデルは、オンライン サービス アドバイザリ (OSA) の販売、オンライン サービスの使用状況 (OSU)-Microsoft 365、および OSU-Business アプリケーション インセンティブ) の顧客との作業に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0ffca-121">This model applies to your work with customers in the following incentives programs: Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

<span data-ttu-id="0ffca-122">Microsoft は、すべてのインセンティブ要求を検証します。</span><span class="sxs-lookup"><span data-stu-id="0ffca-122">Microsoft validates all incentives claims.</span></span>

<span data-ttu-id="0ffca-123">この時点で、詳細を求める場合があります。</span><span class="sxs-lookup"><span data-stu-id="0ffca-123">At this point, we may ask you for more information.</span></span> <span data-ttu-id="0ffca-124">また、関連付け要求を顧客に通知します。</span><span class="sxs-lookup"><span data-stu-id="0ffca-124">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="0ffca-125">お客様はオプトアウトする 5 営業日を持っています。オプトアウトしない場合、この特定のテナントとワークロードとの関連付けは公式になります。</span><span class="sxs-lookup"><span data-stu-id="0ffca-125">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span>

<span data-ttu-id="0ffca-126">関連付け要求に同意することで、顧客は一部のデータにアクセスして、管理サービスを提供することができます。</span><span class="sxs-lookup"><span data-stu-id="0ffca-126">By accepting your request for association, the customer is giving you access to some of their data so you can provide management services to them.</span></span> 

## <a name="resources-to-help-you-create-and-manage-customer-associations"></a><span data-ttu-id="0ffca-127">顧客の関連付けを作成および管理するのに役立つリソース</span><span class="sxs-lookup"><span data-stu-id="0ffca-127">Resources to help you create and manage customer associations</span></span>


|  <span data-ttu-id="0ffca-128">**目的**</span><span class="sxs-lookup"><span data-stu-id="0ffca-128">**To do this**</span></span>  |  <span data-ttu-id="0ffca-129">**参照先**</span><span class="sxs-lookup"><span data-stu-id="0ffca-129">**Read this**</span></span>  |
|--------------|-----------|
| <span data-ttu-id="0ffca-130">顧客の関連付けを作成する方法を確認する</span><span class="sxs-lookup"><span data-stu-id="0ffca-130">Learn how to create a customer association</span></span>  | [<span data-ttu-id="0ffca-131">CPOR モデルを使用して顧客の関連付けを作成する</span><span class="sxs-lookup"><span data-stu-id="0ffca-131">Create a customer association using the CPOR model</span></span>](submit-osa-claim.md)  |
|<span data-ttu-id="0ffca-132">顧客の関連付けを管理する方法を理解する</span><span class="sxs-lookup"><span data-stu-id="0ffca-132">Understand how to manage your customer associations</span></span>  | [<span data-ttu-id="0ffca-133">顧客の関連付けを管理する</span><span class="sxs-lookup"><span data-stu-id="0ffca-133">Manage customer associations</span></span>](incentives-manage-customer-associations.md)  |
|<span data-ttu-id="0ffca-134">顧客の関連付けに関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="0ffca-134">Troubleshoot any customer association issues</span></span>  | [<span data-ttu-id="0ffca-135">顧客の関連付けに関する問題</span><span class="sxs-lookup"><span data-stu-id="0ffca-135">Customer association issues</span></span>](incentives-customer-association-issues.md)  |

## <a name="next-steps"></a><span data-ttu-id="0ffca-136">次の手順</span><span class="sxs-lookup"><span data-stu-id="0ffca-136">Next steps</span></span>

- <span data-ttu-id="0ffca-137">インセンティブは新規ですか?</span><span class="sxs-lookup"><span data-stu-id="0ffca-137">New to incentives?</span></span> <span data-ttu-id="0ffca-138">開始するために必要な情報 [を見つめる](incentives-get-started-intro.md)</span><span class="sxs-lookup"><span data-stu-id="0ffca-138">Discover what you need to [get started](incentives-get-started-intro.md)</span></span>
- <span data-ttu-id="0ffca-139">インセンティブの [共同要求の詳細を確認する](claims-overview.md)</span><span class="sxs-lookup"><span data-stu-id="0ffca-139">Learn more about [incentives co-op claims](claims-overview.md)</span></span>
