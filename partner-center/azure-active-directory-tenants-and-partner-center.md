---
title: パートナー センターにアクセスするよう職場アカウントをリンクする
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 会社をパートナー センター アカウントにリンクする職場アカウントを作成します。 これにより、会社の従業員がパートナー センターにアクセスできるようになります。
author: LauraBrenner
ms.author: labrenne
ms.custom: SEOAPR.20
Keywords: 職場アカウント, 電子メール, テナント, Azure テナント, アカウントの作成, ドメイン名
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: e46be80cb39233e7632a97fd511232d5ff762499
ms.sourcegitcommit: 093039319fab2a44ab147159bc4be832f1330d57
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/14/2020
ms.locfileid: "83394218"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a><span data-ttu-id="0223d-105">会社をパートナー センター アカウントにリンクする職場アカウントを作成する</span><span class="sxs-lookup"><span data-stu-id="0223d-105">Create a work account that links your company to your Partner Center account</span></span>

<span data-ttu-id="0223d-106">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="0223d-106">**Applies to**</span></span>

- <span data-ttu-id="0223d-107">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="0223d-107">Partner Center</span></span>

<span data-ttu-id="0223d-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="0223d-108">**Appropriate roles**</span></span>

- <span data-ttu-id="0223d-109">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="0223d-109">Global admin</span></span>
- <span data-ttu-id="0223d-110">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="0223d-110">User management admin</span></span>

## <a name="why-you-need-a-work-account"></a><span data-ttu-id="0223d-111">職場アカウントが必要な理由</span><span class="sxs-lookup"><span data-stu-id="0223d-111">Why you need a work account</span></span>

<span data-ttu-id="0223d-112">Microsoft は、お客様の会社の職場アカウントとお客様の新しいパートナー センター アカウントのリンク付けを必要としています。</span><span class="sxs-lookup"><span data-stu-id="0223d-112">Microsoft requires you to link your company's work account to your new Partner Center account.</span></span> <span data-ttu-id="0223d-113">このリンク付けにより、アカウント ユーザーは職場アカウントのユーザー名とパスワードを使用して、パートナー センターにサインインできるようになります。</span><span class="sxs-lookup"><span data-stu-id="0223d-113">The link enables your account users to sign in to Partner Center with their work account user names and passwords.</span></span>

## <a name="the-work-account-email-address"></a><span data-ttu-id="0223d-114">職場アカウントのメール アドレス</span><span class="sxs-lookup"><span data-stu-id="0223d-114">The work account email address</span></span>

<span data-ttu-id="0223d-115">職場アカウントまたは勤務先メールは、会社によって指定されたメール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="0223d-115">Your work account or work email is the email address provided to you by your company.</span></span> <span data-ttu-id="0223d-116">通常、職場アカウントのメールの形式は `you@yourcompany.com` です。</span><span class="sxs-lookup"><span data-stu-id="0223d-116">A work account email is usually in the format `you@yourcompany.com`.</span></span> <span data-ttu-id="0223d-117">Hotmail、Gmail、Yahoo などの個人のメール アドレスは仕事用メールではないため、パートナー センター アカウントには使用できません。</span><span class="sxs-lookup"><span data-stu-id="0223d-117">Personal email addresses such as Hotmail, Gmail, or Yahoo aren't work email and can't be used for your Partner Center account.</span></span>

<span data-ttu-id="0223d-118">有効な仕事用メール アドレスが複数ある場合は、地域部門ではなく本社に関連付けられているメール アドレスを使用します。たとえば、`contoso.uk` アドレスではなく `contoso.com` メールを使用します。</span><span class="sxs-lookup"><span data-stu-id="0223d-118">If you have more than one valid work email address, use the one that is associated to your Corporate Headquarters rather than the regional department, for example, use your `contoso.com` email rather than the `contoso.uk` address.</span></span>

> [!NOTE]  
> <span data-ttu-id="0223d-119">既存の職場アカウントの使用を決める前に、パートナー センターでの作業を必要とするアカウント内のユーザーの数を考慮してください。</span><span class="sxs-lookup"><span data-stu-id="0223d-119">Before you decide to use an existing work account, think about how many users in the account will need to work in Partner Center.</span></span> <span data-ttu-id="0223d-120">パートナー センターで作業する必要がないユーザーがアカウントにいる場合、パートナー センターで作業する必要があるユーザー用にのみ、新しいアカウントを作成することを検討してください。</span><span class="sxs-lookup"><span data-stu-id="0223d-120">If you have users in the account who won't need to work in Partner Center, consider creating a new account for only those users who will need to work in the Partner Center.</span></span>

## <a name="not-sure-if-your-company-already-has-a-work-account"></a><span data-ttu-id="0223d-121">職場アカウントが会社に既にあるかどうかわからない場合</span><span class="sxs-lookup"><span data-stu-id="0223d-121">Not sure if your company already has a work account?</span></span>

<span data-ttu-id="0223d-122">会社に職場アカウントがあるかどうかわからない場合は、次の手順に従って確認します。</span><span class="sxs-lookup"><span data-stu-id="0223d-122">If you're not sure whether your company has a work account, follow these steps to check.</span></span> <span data-ttu-id="0223d-123">Microsoft Azure または Office 365 のアクティブなサブスクリプションがある場合は、既に職場アカウントが用意されています。</span><span class="sxs-lookup"><span data-stu-id="0223d-123">If you have an active subscription to Microsoft Azure or Office 365, you already have a work account.</span></span>

1. <span data-ttu-id="0223d-124">[Azure portal](https://portal.azure.com) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="0223d-124">Sign in to the [Azure portal](https://portal.azure.com).</span></span>

2. <span data-ttu-id="0223d-125">メニューから Azure Active Directory を選択し、ドメイン名を選択します。</span><span class="sxs-lookup"><span data-stu-id="0223d-125">Select Azure Active Directory from the menu and then select Domain Names.</span></span>

3. <span data-ttu-id="0223d-126">既に職場アカウントがある場合、ドメイン名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="0223d-126">If you already have a work account, your domain name will be listed.</span></span>

<span data-ttu-id="0223d-127">会社に職場アカウントがまだない場合は、登録プロセスを通じて無料で作成できます。</span><span class="sxs-lookup"><span data-stu-id="0223d-127">If your company doesn't already have a work account, you can create one during the enrollment process.</span></span>

<span data-ttu-id="0223d-128">次の図は、いくつかの一般的なシナリオの手順を示しています。</span><span class="sxs-lookup"><span data-stu-id="0223d-128">The diagram below provides steps for several typical scenarios:</span></span>

- <span data-ttu-id="0223d-129">職場アカウントがあるかどうかを確認する</span><span class="sxs-lookup"><span data-stu-id="0223d-129">determine if you have a work account</span></span>
- <span data-ttu-id="0223d-130">職場アカウントにサインインする方法を確認する</span><span class="sxs-lookup"><span data-stu-id="0223d-130">determine how to sign into your work account</span></span>
- <span data-ttu-id="0223d-131">新しい職場アカウントを作成する必要があるかどうかを判断する</span><span class="sxs-lookup"><span data-stu-id="0223d-131">determine if you need to create a new work account</span></span>

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="職場アカウントがありますか?作成する必要がありますか?":::

<span data-ttu-id="0223d-133">Azure AD でドメインを追加する方法について詳しくは、[Azure AD でのドメインの追加または関連付けに関するページ](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0223d-133">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="0223d-134">Microsoft Azure について</span><span class="sxs-lookup"><span data-stu-id="0223d-134">About Microsoft Azure</span></span>

<span data-ttu-id="0223d-135">Microsoft Azure は、マイクロソフトが管理するデータセンターのグローバル ネットワークで企業がアプリケーションの構築、展開、管理に使うことができるパブリック クラウド プラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="0223d-135">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="0223d-136">企業は、Azure を使って、物理的なコンピューターではなく仮想的な機能やサービスを提供する仮想 IT インフラストラクチャを構築します。</span><span class="sxs-lookup"><span data-stu-id="0223d-136">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span>

<span data-ttu-id="0223d-137">Azure サブスクリプションを購入すると、実質的にはセキュリティで保護された専用のスペースを Azure パブリック クラウド内に借りることになります。会社の物理的なビジネスを行うためにオフィス ビルのフロアを借りるのと大きな違いはありません。</span><span class="sxs-lookup"><span data-stu-id="0223d-137">When you purchase an Azure subscription, you're essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company's physical business.</span></span> <span data-ttu-id="0223d-138">オフィス ビルの所有者に対して、企業はテナントです。</span><span class="sxs-lookup"><span data-stu-id="0223d-138">To the office building's owner, your company is a tenant.</span></span>

<span data-ttu-id="0223d-139">Azure 職場アカウントは、Azure パブリック クラウドにおける企業の分離された専用の仮想表現です。Azure、Microsoft Intune、Office 365などの Microsoft クラウド サービスにサブスクライブすると作成されます。</span><span class="sxs-lookup"><span data-stu-id="0223d-139">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="0223d-140">職場アカウントには、Azure AD ユーザーとユーザーに関する情報 (パスワード、プロフィール データ、アクセス許可など) がホストされます。</span><span class="sxs-lookup"><span data-stu-id="0223d-140">Your work account hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="0223d-141">職場アカウントにはまた、グループ、アプリケーションや、会社とそのセキュリティに関連するその他の情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="0223d-141">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span>
