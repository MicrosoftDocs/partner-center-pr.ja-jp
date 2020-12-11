---
title: パートナー センターにアクセスするよう職場アカウントをリンクする
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 会社をパートナー センター アカウントにリンクする職場アカウントを作成します。 これにより、会社の従業員がパートナー センターにアクセスできるようになります。
author: vinayks
ms.author: vinayks
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: bc837db5a9dbcf92fbfead54b552695a218ae675
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534796"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a><span data-ttu-id="94130-104">会社をパートナー センター アカウントにリンクする職場アカウントを作成する</span><span class="sxs-lookup"><span data-stu-id="94130-104">Create a work account that links your company to your Partner Center account</span></span>

<span data-ttu-id="94130-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="94130-105">**Appropriate roles**</span></span>

- <span data-ttu-id="94130-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="94130-106">Global admin</span></span>
- <span data-ttu-id="94130-107">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="94130-107">User management admin</span></span>

## <a name="why-you-need-a-work-account"></a><span data-ttu-id="94130-108">職場アカウントが必要な理由</span><span class="sxs-lookup"><span data-stu-id="94130-108">Why you need a work account</span></span>

<span data-ttu-id="94130-109">Microsoft は、お客様の会社の職場アカウントとお客様の新しいパートナー センター アカウントのリンク付けを必要としています。</span><span class="sxs-lookup"><span data-stu-id="94130-109">Microsoft requires you to link your company's work account to your new Partner Center account.</span></span> <span data-ttu-id="94130-110">このリンク付けにより、アカウント ユーザーは職場アカウントのユーザー名とパスワードを使用して、パートナー センターにサインインできるようになります。</span><span class="sxs-lookup"><span data-stu-id="94130-110">The link enables your account users to sign in to Partner Center with their work account user names and passwords.</span></span>

## <a name="the-work-account-email-address"></a><span data-ttu-id="94130-111">職場アカウントのメール アドレス</span><span class="sxs-lookup"><span data-stu-id="94130-111">The work account email address</span></span>

<span data-ttu-id="94130-112">職場アカウントまたは勤務先メールは、会社によって指定されたメール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="94130-112">Your work account or work email is the email address provided to you by your company.</span></span> <span data-ttu-id="94130-113">通常、職場アカウントのメールの形式は `you@yourcompany.com` です。</span><span class="sxs-lookup"><span data-stu-id="94130-113">A work account email is usually in the format `you@yourcompany.com`.</span></span> <span data-ttu-id="94130-114">Hotmail、Gmail、Yahoo などの個人のメール アドレスは仕事用メールではないため、パートナー センター アカウントには使用できません。</span><span class="sxs-lookup"><span data-stu-id="94130-114">Personal email addresses such as Hotmail, Gmail, or Yahoo aren't work email and can't be used for your Partner Center account.</span></span>

<span data-ttu-id="94130-115">有効な仕事用メール アドレスが複数ある場合は、地域部門ではなく本社に関連付けられているメール アドレスを使用します。たとえば、`contoso.uk` アドレスではなく `contoso.com` メールを使用します。</span><span class="sxs-lookup"><span data-stu-id="94130-115">If you have more than one valid work email address, use the one that is associated to your Corporate Headquarters rather than the regional department, for example, use your `contoso.com` email rather than the `contoso.uk` address.</span></span>

> [!NOTE]  
> <span data-ttu-id="94130-116">既存の職場アカウントの使用を決める前に、パートナー センターでの作業を必要とするアカウント内のユーザーの数を考慮してください。</span><span class="sxs-lookup"><span data-stu-id="94130-116">Before you decide to use an existing work account, think about how many users in the account will need to work in Partner Center.</span></span> <span data-ttu-id="94130-117">パートナー センターで作業する必要がないユーザーがアカウントにいる場合、パートナー センターで作業する必要があるユーザー用にのみ、新しいアカウントを作成することを検討してください。</span><span class="sxs-lookup"><span data-stu-id="94130-117">If you have users in the account who won't need to work in Partner Center, consider creating a new account for only those users who will need to work in the Partner Center.</span></span>

## <a name="not-sure-if-your-company-already-has-a-work-account"></a><span data-ttu-id="94130-118">職場アカウントが会社に既にあるかどうかわからない場合</span><span class="sxs-lookup"><span data-stu-id="94130-118">Not sure if your company already has a work account?</span></span>

<span data-ttu-id="94130-119">会社に職場アカウントがあるかどうかわからない場合は、次の手順に従って確認します。</span><span class="sxs-lookup"><span data-stu-id="94130-119">If you're not sure whether your company has a work account, follow these steps to check.</span></span> <span data-ttu-id="94130-120">Microsoft Azure または Office 365 のアクティブなサブスクリプションがある場合は、既に職場アカウントが用意されています。</span><span class="sxs-lookup"><span data-stu-id="94130-120">If you have an active subscription to Microsoft Azure or Office 365, you already have a work account.</span></span>

1. <span data-ttu-id="94130-121">[Azure portal](https://portal.azure.com) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="94130-121">Sign in to the [Azure portal](https://portal.azure.com).</span></span>

2. <span data-ttu-id="94130-122">メニューから Azure Active Directory を選択し、ドメイン名を選択します。</span><span class="sxs-lookup"><span data-stu-id="94130-122">Select Azure Active Directory from the menu and then select Domain Names.</span></span>

3. <span data-ttu-id="94130-123">既に職場アカウントがある場合、ドメイン名が表示されます。</span><span class="sxs-lookup"><span data-stu-id="94130-123">If you already have a work account, your domain name will be listed.</span></span>

<span data-ttu-id="94130-124">会社に職場アカウントがまだない場合は、登録プロセスを通じて無料で作成できます。</span><span class="sxs-lookup"><span data-stu-id="94130-124">If your company doesn't already have a work account, you can create one during the enrollment process.</span></span>

<span data-ttu-id="94130-125">次の図は、いくつかの一般的なシナリオの手順を示しています。</span><span class="sxs-lookup"><span data-stu-id="94130-125">The diagram below provides steps for several typical scenarios:</span></span>

- <span data-ttu-id="94130-126">職場アカウントがあるかどうかを確認する</span><span class="sxs-lookup"><span data-stu-id="94130-126">determine if you have a work account</span></span>
- <span data-ttu-id="94130-127">職場アカウントにサインインする方法を確認する</span><span class="sxs-lookup"><span data-stu-id="94130-127">determine how to sign into your work account</span></span>
- <span data-ttu-id="94130-128">新しい職場アカウントを作成する必要があるかどうかを判断する</span><span class="sxs-lookup"><span data-stu-id="94130-128">determine if you need to create a new work account</span></span>

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="職場アカウントがありますか?作成する必要がありますか?":::

<span data-ttu-id="94130-130">Azure AD でドメインを追加する方法について詳しくは、[Azure AD でのドメインの追加または関連付けに関するページ](/azure/active-directory/active-directory-add-domain)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="94130-130">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="94130-131">Microsoft Azure について</span><span class="sxs-lookup"><span data-stu-id="94130-131">About Microsoft Azure</span></span>

<span data-ttu-id="94130-132">Microsoft Azure は、マイクロソフトが管理するデータセンターのグローバル ネットワークで企業がアプリケーションの構築、展開、管理に使うことができるパブリック クラウド プラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="94130-132">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="94130-133">企業は、Azure を使って、物理的なコンピューターではなく仮想的な機能やサービスを提供する仮想 IT インフラストラクチャを構築します。</span><span class="sxs-lookup"><span data-stu-id="94130-133">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span>

<span data-ttu-id="94130-134">Azure サブスクリプションを購入すると、実質的にはセキュリティで保護された専用のスペースを Azure パブリック クラウド内に借りることになります。会社の物理的なビジネスを行うためにオフィス ビルのフロアを借りるのと大きな違いはありません。</span><span class="sxs-lookup"><span data-stu-id="94130-134">When you purchase an Azure subscription, you're essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company's physical business.</span></span> <span data-ttu-id="94130-135">オフィス ビルの所有者に対して、企業はテナントです。</span><span class="sxs-lookup"><span data-stu-id="94130-135">To the office building's owner, your company is a tenant.</span></span>

<span data-ttu-id="94130-136">Azure 職場アカウントは、Azure パブリック クラウドにおける企業の分離された専用の仮想表現です。Azure、Microsoft Intune、Office 365などの Microsoft クラウド サービスにサブスクライブすると作成されます。</span><span class="sxs-lookup"><span data-stu-id="94130-136">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="94130-137">職場アカウントには、Azure AD ユーザーとユーザーに関する情報 (パスワード、プロフィール データ、アクセス許可など) がホストされます。</span><span class="sxs-lookup"><span data-stu-id="94130-137">Your work account hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="94130-138">職場アカウントにはまた、グループ、アプリケーションや、会社とそのセキュリティに関連するその他の情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="94130-138">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span>

## <a name="next-steps"></a><span data-ttu-id="94130-139">次の手順</span><span class="sxs-lookup"><span data-stu-id="94130-139">Next steps</span></span>

- [<span data-ttu-id="94130-140">パートナー センター アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="94130-140">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="94130-141">検証状態を追跡する</span><span class="sxs-lookup"><span data-stu-id="94130-141">Track verification status</span></span>](verification-responses.md)