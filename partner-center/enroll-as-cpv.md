---
title: コントロール パネル ベンダーとして登録する
description: パートナーセンターでコントロールパネルベンダ (CPV) として登録する方法について説明します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/20/2020
ms.openlocfilehash: 79d46b306795c1261fb8e9af45e7c102b9e79601
ms.sourcegitcommit: c40f826bb1143555bf3a1c2c806c34024f0f6019
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/02/2020
ms.locfileid: "89366736"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="2c14b-103">CSP パートナーシステムとパートナーセンター Api との統合に役立つ、コントロールパネルのベンダとして登録する</span><span class="sxs-lookup"><span data-stu-id="2c14b-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>

<span data-ttu-id="2c14b-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="2c14b-104">**Applies to**</span></span>

- <span data-ttu-id="2c14b-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="2c14b-105">Partner Center</span></span>

<span data-ttu-id="2c14b-106">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="2c14b-106">**Appropriate roles**</span></span>

- <span data-ttu-id="2c14b-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="2c14b-107">Global admin</span></span>

<span data-ttu-id="2c14b-108">コントロール パネル ベンダー (CPV) は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムをパートナー センター API と統合するために使用できるアプリケーションを開発する独立系ソフトウェア ベンダーです。</span><span class="sxs-lookup"><span data-stu-id="2c14b-108">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="2c14b-109">コントロール パネル ベンダーは、パートナー センター ダッシュボードまたはパートナー センター API に直接アクセスできる CSP パートナーではありません。</span><span class="sxs-lookup"><span data-stu-id="2c14b-109">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="2c14b-110">現在既にコントロール パネル ベンダー (CPV) であっても、または Microsoft パートナーと協力したい新しい CPV であっても、Microsoft は CPV に、アプリケーションを登録し、クラウド ソリューション プロバイダー パートナーをサポートするため、パートナー センターに登録することを要求します。</span><span class="sxs-lookup"><span data-stu-id="2c14b-110">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="2c14b-111">アカウントを作成するには、CPV パートナーは、既存の CSP パートナーのテナントや既存の CPV テナントを使用するか、またはオンボード プロセスの一環として新しいテナントを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="2c14b-111">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="2c14b-112">CPV パートナーが既存の CSP テナントを使用することを選択した場合は、個別のマルチテナントアプリケーションを作成し、それらを CPV アクティビティのパートナーセンターに登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2c14b-112">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="2c14b-113">アプリケーションを CSP と CPV アプリケーションの両方として登録することはできません。</span><span class="sxs-lookup"><span data-stu-id="2c14b-113">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="2c14b-114">パートナー センターに登録して、アプリケーションを登録したら、パートナー センター API にアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="2c14b-114">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="2c14b-115">Microsoft は、パートナーのサンドボックス情報を使用してパートナー センターの通知経由で連絡します。</span><span class="sxs-lookup"><span data-stu-id="2c14b-115">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="2c14b-116">サンドボックスアカウントを既に持っている場合は、引き続き使用します。</span><span class="sxs-lookup"><span data-stu-id="2c14b-116">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="2c14b-117">新しいサンドボックスは必要ありません。</span><span class="sxs-lookup"><span data-stu-id="2c14b-117">You won't need a new sandbox.</span></span>

<span data-ttu-id="2c14b-118">「[Microsoft Control Panel Vendor agreement (Microsoft コントロール パネル ベンダー契約)](https://go.microsoft.com/fwlink/?linkid=2055198)」を確認してください</span><span class="sxs-lookup"><span data-stu-id="2c14b-118">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="2c14b-119">パートナー センターでの操作</span><span class="sxs-lookup"><span data-stu-id="2c14b-119">Working in Partner Center</span></span>
<span data-ttu-id="2c14b-120">パートナーセンターの CPV エクスペリエンスに登録し、CPV 契約に同意すると、次のことができるようになります。</span><span class="sxs-lookup"><span data-stu-id="2c14b-120">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="2c14b-121">マルチテナントアプリケーションを管理します (アプリケーションを追加して、パートナーセンターでアプリケーションを Azure portal、登録、登録解除します)。</span><span class="sxs-lookup"><span data-stu-id="2c14b-121">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="2c14b-122">CPV は、パートナー センター API の承認を取得するには、パートナー センターでアプリケーションを登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2c14b-122">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="2c14b-123">Azure portal にアプリケーションを追加するだけでは、CPV アプリケーションはパートナー センター API に対して承認されません。</span><span class="sxs-lookup"><span data-stu-id="2c14b-123">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="2c14b-124">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="2c14b-124">View and manage your CPV profile</span></span> 

- <span data-ttu-id="2c14b-125">CPV 機能にアクセスする必要があるユーザーを表示および管理する。</span><span class="sxs-lookup"><span data-stu-id="2c14b-125">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="2c14b-126">CPV が持つことができる唯一のロールは、全体管理者です。</span><span class="sxs-lookup"><span data-stu-id="2c14b-126">Global admin is the only role a CPV can have.</span></span>


