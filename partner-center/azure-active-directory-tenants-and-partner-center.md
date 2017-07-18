---
title: "Azure Active Directory テナントとパートナー センター | パートナー センター"
description: "パートナー センター アカウントを作成するには、Azure Active Directory (Azure AD) テナントが会社に必要です。 Azure AD は、マイクロソフトのクラウド ベース ディレクトリおよび ID 管理サービスです。"
author: labrenne
robots: 
ms.openlocfilehash: 9a9a3c3aa239017fe8ecf655f79acbfab6ff8a0b
ms.sourcegitcommit: d7c4ca62acd1ef1026c7d322e40f55a83a80e72a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a><span data-ttu-id="4cc80-104">Azure Active Directory テナントとパートナー センター</span><span class="sxs-lookup"><span data-stu-id="4cc80-104">Azure Active Directory tenants and Partner Center</span></span>  

**<span data-ttu-id="4cc80-105">適用対象</span><span class="sxs-lookup"><span data-stu-id="4cc80-105">Applies to</span></span>**

-  <span data-ttu-id="4cc80-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="4cc80-106">Partner Center</span></span>

## <a name="why-you-need-an-azure-ad-tenant"></a><span data-ttu-id="4cc80-107">Azure AD テナントが必要な理由</span><span class="sxs-lookup"><span data-stu-id="4cc80-107">Why you need an Azure AD tenant</span></span>

<span data-ttu-id="4cc80-108">テナント ユーザーが Azure AD (Microsoft アカウント) のユーザー名とパスワードを使ってパートナー センターにサインインできるように、組織の Azure AD テナントを新しいパートナー センター アカウントにリンクする必要があります。</span><span class="sxs-lookup"><span data-stu-id="4cc80-108">We need to link your organization’s Azure AD tenant to your new Partner Center account, so your tenant users can sign in to Partner Center with their Azure AD (Microsoft account) user names and passwords.</span></span>

<span data-ttu-id="4cc80-109">会社に Azure AD テナントが既にある場合は、そのテナントをパートナー センター アカウントにリンクできます。</span><span class="sxs-lookup"><span data-stu-id="4cc80-109">If your company already has an Azure AD tenant, you can link it to your Partner Center account.</span></span> 

>**<span data-ttu-id="4cc80-110">注</span><span class="sxs-lookup"><span data-stu-id="4cc80-110">Note</span></span>**<br> <span data-ttu-id="4cc80-111">既存の Azure AD テナントの使用を決める前に、パートナー センターで作業する必要があるテナント内のユーザーの数について考慮してください。</span><span class="sxs-lookup"><span data-stu-id="4cc80-111">Before you decide to use an existing Azure AD tenant, think about how many users in the tenant will need to work in Partner Center.</span></span> <span data-ttu-id="4cc80-112">パートナー センターで作業する必要がないユーザーがテナントにいる場合、パートナー センターで作業する必要があるユーザーだけの新しいテナントを作成することを検討してください。</span><span class="sxs-lookup"><span data-stu-id="4cc80-112">If you have users in the tenant who won’t need to work in Partner Center, consider creating a new tenant for only those users who will need to work in Partner Center.</span></span>

<span data-ttu-id="4cc80-113">Azure AD テナントが会社にまだない場合は、登録プロセスを通じて無料で作成できます。</span><span class="sxs-lookup"><span data-stu-id="4cc80-113">If your company doesn’t already have an Azure AD tenant, you can create one for free during the enrollment process.</span></span> <span data-ttu-id="4cc80-114">**[Azure Active Directory にサインインします]** ページで **[新しいテナントを作成する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="4cc80-114">Select **Create new tenant** on the **Sign in to Azure Active Directory** page.</span></span> 

### <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a><span data-ttu-id="4cc80-115">Azure AD テナントが会社に既にあるかどうかわからない場合</span><span class="sxs-lookup"><span data-stu-id="4cc80-115">Not sure if your company already has an Azure AD tenant?</span></span>

<span data-ttu-id="4cc80-116">Azure AD テナントが会社にあるかどうかわからない場合、次の手順に従って確認します。</span><span class="sxs-lookup"><span data-stu-id="4cc80-116">If you’re not sure whether your company has an Azure AD tenant, follow these steps to check.</span></span> <span data-ttu-id="4cc80-117">Microsoft Azure または Office 365 のアクティブなサブスクリプションがある場合、既に Azure AD テナントがある点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="4cc80-117">Note that If you have an active subscription to Microsoft Azure or Office 365, you already have an Azure AD tenant.</span></span>
1.  <span data-ttu-id="4cc80-118">Azure 管理ポータル (https://ms.portal.azure.com) にサインインする</span><span class="sxs-lookup"><span data-stu-id="4cc80-118">Sign in to the Azure admin portal at https://ms.portal.azure.com</span></span>
2.  <span data-ttu-id="4cc80-119">メニューから Azure Active Directory を選択し、ドメイン名を選択します。</span><span class="sxs-lookup"><span data-stu-id="4cc80-119">Select Azure Active Directory from the menu and then select Domain Names.</span></span>
3.  <span data-ttu-id="4cc80-120">既にテナントがある場合、ドメイン名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="4cc80-120">If you already have a tenant, your domain name will be listed.</span></span>

### <a name="using-an-existing-tenant"></a><span data-ttu-id="4cc80-121">既存のテナントを使う場合</span><span class="sxs-lookup"><span data-stu-id="4cc80-121">Using an existing tenant?</span></span>

<span data-ttu-id="4cc80-122">既存の Azure AD テナントを使おうとしてもサインインで問題が発生する場合、状況に最も合うシナリオを次の図から探し、推奨される手順に従います。</span><span class="sxs-lookup"><span data-stu-id="4cc80-122">If you want to use an existing Azure AD tenant but you’re having trouble signing in, find the scenario on the diagram below that best matches your situation and follow the recommended steps.</span></span> 

![Azure AD テナントがあるか、もう 1 つ作成する必要がある場合](images/onboardingAADFlow.png)

<span data-ttu-id="4cc80-124">Azure AD でドメインを追加する方法について詳しくは、[Azure AD でのドメインの追加または関連付けに関するページ](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4cc80-124">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="4cc80-125">Microsoft Azure について</span><span class="sxs-lookup"><span data-stu-id="4cc80-125">About Microsoft Azure</span></span>

<span data-ttu-id="4cc80-126">Microsoft Azure は、マイクロソフトが管理するデータセンターのグローバル ネットワークで企業がアプリケーションの構築、展開、管理に使うことができるパブリック クラウド プラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="4cc80-126">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="4cc80-127">企業は、Azure を使って、物理的なコンピューターではなく仮想的な機能やサービスを提供する仮想 IT インフラストラクチャを構築します。</span><span class="sxs-lookup"><span data-stu-id="4cc80-127">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span> 

<span data-ttu-id="4cc80-128">Azure サブスクリプションを購入すると、実質的にはセキュリティで保護された専用のペースを Azure パブリック クラウド内に借りることになります。会社の物理的なビジネスを行うためにオフィス ビルのフロアを借りるのと大きな違いはありません。</span><span class="sxs-lookup"><span data-stu-id="4cc80-128">When you purchase an Azure subscription, you’re essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company’s physical business.</span></span> <span data-ttu-id="4cc80-129">オフィス ビルの所有者に対して、企業はテナントです。</span><span class="sxs-lookup"><span data-stu-id="4cc80-129">To the office building’s owner, your company is a tenant.</span></span> 

<span data-ttu-id="4cc80-130">Azure AD テナントは、Azure パブリック クラウドにおける企業の分離された専用の仮想表現です。Azure、Microsoft Intune、Office 365などの Microsoft クラウド サービスにサブスクライブすると作成されます。</span><span class="sxs-lookup"><span data-stu-id="4cc80-130">An Azure AD tenant is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span> 

<span data-ttu-id="4cc80-131">テナントには、Azure AD ユーザーとユーザーに関する情報 (パスワード、プロフィール データ、アクセス許可など) がホストされます。</span><span class="sxs-lookup"><span data-stu-id="4cc80-131">Your tenant hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="4cc80-132">テナントには、グループ、アプリケーション、および会社とそのセキュリティに関連する他の情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="4cc80-132">The tenant also contains groups,applications, and other information pertaining to a company and its security.</span></span> 

<span data-ttu-id="4cc80-133">Azure AD について詳しくは、[Azure Active Directory のドキュメント](https://docs.microsoft.com/ azure/active-directory/)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4cc80-133">To learn more about Azure AD, see the [Azure Active Directory Documentation](https://docs.microsoft.com/ azure/active-directory/).</span></span> 