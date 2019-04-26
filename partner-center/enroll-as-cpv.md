---
title: コントロール パネルのベンダーとパートナー センターの登録 |パートナー センター
ms.topic: article
ms.date: 12/11/2018
Description: コントロール パネルのベンダーとパートナー センターに登録する方法
author: LauraBrenner
ms.author: labrenne
keywords: コントロール パネルの仕入先、CPV アプリを登録、CPV アプリの管理
ms.localizationpriority: medium
ms.openlocfilehash: 7d00cfc7addf120a3b42597cda3758597533dd5e
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "62135562"
---
# <a name="enroll-in-partner-center-as-a-control-panel-vendor"></a><span data-ttu-id="6ce53-104">コントロール パネルのベンダーとパートナー センターに登録します。</span><span class="sxs-lookup"><span data-stu-id="6ce53-104">Enroll in Partner Center as a Control Panel Vendor</span></span>

<span data-ttu-id="6ce53-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="6ce53-105">**Applies to**</span></span>

- <span data-ttu-id="6ce53-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="6ce53-106">Partner Center</span></span>

<span data-ttu-id="6ce53-107">コントロール パネル仕入先 (CPV) では、パートナー センター Api と、システムを統合するためのクラウド ソリューション プロバイダー (CSP) パートナーで使用するアプリケーションを開発している独立系ソフトウェア ベンダーです。</span><span class="sxs-lookup"><span data-stu-id="6ce53-107">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="6ce53-108">コントロール パネルのベンダーは、パートナー センター ダッシュ ボードに直接アクセスできる CSP パートナーまたはパートナー センター Api ではありません。</span><span class="sxs-lookup"><span data-stu-id="6ce53-108">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="6ce53-109">現在のコントロール パネル仕入先 (CPV) または Microsoft パートナーを使用する新しい CPV であるかどうか Microsoft が必要になりました、アプリケーションを登録し、Cloud Solution Provider パートナーをサポートするためにパートナー センターに登録します。</span><span class="sxs-lookup"><span data-stu-id="6ce53-109">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="6ce53-110">アカウントを作成するには、CPV パートナーは、既存の CSP パートナーのテナント、または既存の CPV テナントを使用できます。 またはオンボード プロセスの一環として、新しいテナントを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="6ce53-110">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="6ce53-111">CPV パートナー CSP の既存のテナントを使用する場合、別のマルチ テナント アプリケーションを作成し、パートナー センターで CPV アクティビティに登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ce53-111">If the CPV partner chooses to use the existing CSP tenant, then they’ll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="6ce53-112">アプリケーションは、CSP および CPV の両方のアプリケーションとして登録することはできません。</span><span class="sxs-lookup"><span data-stu-id="6ce53-112">An application can’t be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="6ce53-113">パートナー センターに登録して、アプリケーションを登録したら、パートナー センター Api へのアクセス必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ce53-113">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="6ce53-114">Microsoft は、サンド ボックスの情報をパートナー センターの通知を使用して連絡します。</span><span class="sxs-lookup"><span data-stu-id="6ce53-114">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="6ce53-115">ただし、サンド ボックス アカウントが既にあるを場合は、引き続き使用します。</span><span class="sxs-lookup"><span data-stu-id="6ce53-115">If, however, you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="6ce53-116">新しいサンド ボックスを使用する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="6ce53-116">You won’t need a new sandbox.</span></span>   

<span data-ttu-id="6ce53-117">レビュー、 [Microsoft コントロール パネルの仕入先契約](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="6ce53-117">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="6ce53-118">パートナー センターでの操作</span><span class="sxs-lookup"><span data-stu-id="6ce53-118">Working in Partner Center</span></span>
<span data-ttu-id="6ce53-119">パートナー センター CPV エクスペリエンスに登録されているし、できます CPV 契約書に同意します。</span><span class="sxs-lookup"><span data-stu-id="6ce53-119">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement you can:</span></span>

- <span data-ttu-id="6ce53-120">(追加アプリケーションを Azure ポータルの登録し、パートナー センターでアプリケーションの登録を解除) マルチ テナント アプリケーションを管理します。</span><span class="sxs-lookup"><span data-stu-id="6ce53-120">Manage multi-tenant applications (add applications to Azure portal, register and unregister applications in Partner Center).</span></span>

>[!Note] 
><span data-ttu-id="6ce53-121">CPVs は、パートナー センター Api の承認を取得するには、パートナー センターでアプリケーションを登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ce53-121">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="6ce53-122">アプリケーションだけで、Azure portal を追加する、パートナー センター Api の CPV アプリケーションが承認されることはできません。</span><span class="sxs-lookup"><span data-stu-id="6ce53-122">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="6ce53-123">表示および CPV プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="6ce53-123">View and manage your CPV profile</span></span> 

- <span data-ttu-id="6ce53-124">表示および CPV 機能へのアクセスを必要とするユーザーを管理します。</span><span class="sxs-lookup"><span data-stu-id="6ce53-124">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="6ce53-125">唯一の役割を CPV が持つことができます。 全体管理者は、します。</span><span class="sxs-lookup"><span data-stu-id="6ce53-125">The only role a CPV can have is global admin.</span></span>


