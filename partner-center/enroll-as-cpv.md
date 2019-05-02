---
title: コントロール パネル ベンダーとしてパートナー センターに登録する | パートナー センター
ms.topic: article
ms.date: 12/11/2018
Description: コントロール パネル ベンダーとしてパートナー センターに登録する方法です
author: LauraBrenner
ms.author: labrenne
keywords: コントロール パネル ベンダー, CPV アプリを登録, CPV アプリの管理
ms.localizationpriority: medium
ms.openlocfilehash: 7d00cfc7addf120a3b42597cda3758597533dd5e
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135562"
---
# <a name="enroll-in-partner-center-as-a-control-panel-vendor"></a><span data-ttu-id="ee0a3-104">コントロール パネル ベンダーとしてパートナー センターに登録する</span><span class="sxs-lookup"><span data-stu-id="ee0a3-104">Enroll in Partner Center as a Control Panel Vendor</span></span>

<span data-ttu-id="ee0a3-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="ee0a3-105">**Applies to**</span></span>

- <span data-ttu-id="ee0a3-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="ee0a3-106">Partner Center</span></span>

<span data-ttu-id="ee0a3-107">コントロール パネル ベンダー (CPV) は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムをパートナー センター API と統合するために使用できるアプリケーションを開発する独立系ソフトウェア ベンダーです。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-107">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="ee0a3-108">コントロール パネル ベンダーは、パートナー センター ダッシュボードまたはパートナー センター API に直接アクセスできる CSP パートナーではありません。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-108">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="ee0a3-109">現在既にコントロール パネル ベンダー (CPV) であっても、または Microsoft パートナーと協力したい新しい CPV であっても、Microsoft は CPV に、アプリケーションを登録し、クラウド ソリューション プロバイダー パートナーをサポートするため、パートナー センターに登録することを要求します。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-109">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="ee0a3-110">アカウントを作成するには、CPV パートナーは、既存の CSP パートナーのテナントや既存の CPV テナントを使用するか、またはオンボード プロセスの一環として新しいテナントを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-110">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="ee0a3-111">既存の CSP テナントを使用する CPV パートナーは、別のマルチテナント アプリケーションを作成し、パートナー センターで CPV アクティビティ用に登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-111">If the CPV partner chooses to use the existing CSP tenant, then they’ll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="ee0a3-112">1 つのアプリケーションを、CSP アプリケーションおよび CPV アプリケーションの両方として登録することはできません。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-112">An application can’t be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="ee0a3-113">パートナー センターに登録して、アプリケーションを登録したら、パートナー センター API にアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-113">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="ee0a3-114">Microsoft は、パートナーのサンドボックス情報を使用してパートナー センターの通知経由で連絡します。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-114">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="ee0a3-115">ただし、パートナーがサンドボックス アカウントを既に持っている場合は、それを引き続き使用します。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-115">If, however, you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="ee0a3-116">新しいサンドボックスは必要ありません。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-116">You won’t need a new sandbox.</span></span>   

<span data-ttu-id="ee0a3-117">「[Microsoft Control Panel Vendor agreement (Microsoft コントロール パネル ベンダー契約)](https://go.microsoft.com/fwlink/?linkid=2055198)」を確認してください</span><span class="sxs-lookup"><span data-stu-id="ee0a3-117">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="ee0a3-118">パートナー センターでの操作</span><span class="sxs-lookup"><span data-stu-id="ee0a3-118">Working in Partner Center</span></span>
<span data-ttu-id="ee0a3-119">パートナー センター CPV エクスペリエンスに登録し、CPV 契約に同意した後は、次のことを実行できます。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-119">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement you can:</span></span>

- <span data-ttu-id="ee0a3-120">マルチテナント アプリケーションを管理する (Azure portal へのアプリケーションの追加、パートナー センターでのアプリケーションの登録と登録解除)。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-120">Manage multi-tenant applications (add applications to Azure portal, register and unregister applications in Partner Center).</span></span>

>[!Note] 
><span data-ttu-id="ee0a3-121">CPV は、パートナー センター API の承認を取得するには、パートナー センターでアプリケーションを登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-121">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="ee0a3-122">Azure portal にアプリケーションを追加するだけでは、CPV アプリケーションはパートナー センター API に対して承認されません。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-122">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="ee0a3-123">CPV プロファイルを表示および管理する</span><span class="sxs-lookup"><span data-stu-id="ee0a3-123">View and manage your CPV profile</span></span> 

- <span data-ttu-id="ee0a3-124">CPV 機能にアクセスする必要があるユーザーを表示および管理する。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-124">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="ee0a3-125">CPV が持つことのできる唯一のロールは、グローバル管理者です。</span><span class="sxs-lookup"><span data-stu-id="ee0a3-125">The only role a CPV can have is global admin.</span></span>


