---
title: コントロール パネル ベンダーとして登録する
description: パートナーセンターで、CSP パートナーシステムとパートナーセンター Api をより適切に統合できるように、パートナーセンターでコントロールパネルベンダー (CPV) として登録する方法について説明します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: edc0ea8f0fda58f23cbce82bc7023a3277517cc3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147141"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="156cf-103">CSP パートナー システムとパートナー センター API との統合を支援するためにコントロール パネル ベンダーとして登録する</span><span class="sxs-lookup"><span data-stu-id="156cf-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="156cf-104">**適切なロール**: グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="156cf-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="156cf-105">コントロール パネル ベンダー (CPV) は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムをパートナー センター API と統合するために使用できるアプリケーションを開発する独立系ソフトウェア ベンダーです。</span><span class="sxs-lookup"><span data-stu-id="156cf-105">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="156cf-106">コントロール パネル ベンダーは、パートナー センター ダッシュボードまたはパートナー センター API に直接アクセスできる CSP パートナーではありません。</span><span class="sxs-lookup"><span data-stu-id="156cf-106">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="156cf-107">現在既にコントロール パネル ベンダー (CPV) であっても、または Microsoft パートナーと協力したい新しい CPV であっても、Microsoft は CPV に、アプリケーションを登録し、クラウド ソリューション プロバイダー パートナーをサポートするため、パートナー センターに登録することを要求します。</span><span class="sxs-lookup"><span data-stu-id="156cf-107">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="156cf-108">アカウントを作成するには、CPV パートナーは、既存の CSP パートナーのテナントや既存の CPV テナントを使用するか、またはオンボード プロセスの一環として新しいテナントを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="156cf-108">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="156cf-109">CPV パートナーが既存の CSP テナントを使用することを選択した場合は、個別のマルチテナントアプリケーションを作成し、それらを CPV アクティビティのパートナーセンターに登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="156cf-109">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="156cf-110">アプリケーションを CSP と CPV アプリケーションの両方として登録することはできません。</span><span class="sxs-lookup"><span data-stu-id="156cf-110">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="156cf-111">パートナー センターに登録して、アプリケーションを登録したら、パートナー センター API にアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="156cf-111">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="156cf-112">サンドボックスアカウントが必要な場合は、Microsoft サポート要求を通じて Microsoft にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="156cf-112">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="156cf-113">サンドボックスアカウントを既に持っている場合は、引き続き使用します。</span><span class="sxs-lookup"><span data-stu-id="156cf-113">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="156cf-114">新しいサンドボックスは必要ありません</span><span class="sxs-lookup"><span data-stu-id="156cf-114">You won't need a new sandbox</span></span>

<span data-ttu-id="156cf-115">「[Microsoft Control Panel Vendor agreement (Microsoft コントロール パネル ベンダー契約)](https://go.microsoft.com/fwlink/?linkid=2055198)」を確認してください</span><span class="sxs-lookup"><span data-stu-id="156cf-115">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="156cf-116">パートナー センターでの操作</span><span class="sxs-lookup"><span data-stu-id="156cf-116">Working in Partner Center</span></span>

<span data-ttu-id="156cf-117">パートナーセンターの CPV エクスペリエンスに登録し、CPV 契約に同意すると、次のことができるようになります。</span><span class="sxs-lookup"><span data-stu-id="156cf-117">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="156cf-118">マルチテナントアプリケーションを管理します (アプリケーションを追加して、パートナーセンターでアプリケーションを Azure portal、登録、登録解除します)。</span><span class="sxs-lookup"><span data-stu-id="156cf-118">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="156cf-119">CPV は、パートナー センター API の承認を取得するには、パートナー センターでアプリケーションを登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="156cf-119">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="156cf-120">Azure portal にアプリケーションを追加するだけでは、CPV アプリケーションはパートナー センター API に対して承認されません。</span><span class="sxs-lookup"><span data-stu-id="156cf-120">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="156cf-121">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="156cf-121">View and manage your CPV profile</span></span> 

- <span data-ttu-id="156cf-122">CPV 機能にアクセスする必要があるユーザーを表示および管理する。</span><span class="sxs-lookup"><span data-stu-id="156cf-122">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="156cf-123">CPV が持つことができる唯一のロールは、全体管理者です。</span><span class="sxs-lookup"><span data-stu-id="156cf-123">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="156cf-124">次のステップ</span><span class="sxs-lookup"><span data-stu-id="156cf-124">Next steps</span></span>

<span data-ttu-id="156cf-125">-[パートナーセンターアカウントにテナントを追加する](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="156cf-125">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>