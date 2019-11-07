---
title: パートナー センター アカウントを作成する | パートナー センター
ms.topic: article
ms.date: 10/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Microsoft Partner Network メンバーがネットワークの利点とコンピテンシーを管理してビジネス プロファイルを作成するには、パートナー センター アカウントを作成する必要があります。
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: e1497003ef9ca08b61f0ae752eab654dc40b6997
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653262"
---
# <a name="create-a-partner-center-account"></a><span data-ttu-id="613ee-103">パートナー センター アカウントを作成する</span><span class="sxs-lookup"><span data-stu-id="613ee-103">Create a Partner Center account</span></span>

<span data-ttu-id="613ee-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="613ee-104">**Appropriate roles**</span></span>

- <span data-ttu-id="613ee-105">グローバル管理</span><span class="sxs-lookup"><span data-stu-id="613ee-105">Global admin</span></span>
- <span data-ttu-id="613ee-106">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="613ee-106">Admin agent</span></span>

<span data-ttu-id="613ee-107">パートナー センターでアカウントを作成するには、貴社が Microsoft Partner Network のメンバーである必要があります。</span><span class="sxs-lookup"><span data-stu-id="613ee-107">Before you can create an account on Partner Center, your company must be a member of the Microsoft Partner Network.</span></span> <span data-ttu-id="613ee-108">メンバーでない場合は、[今すぐ登録](https://partners.microsoft.com/PartnerProgram/simplifiedenrollment.aspx)できます。</span><span class="sxs-lookup"><span data-stu-id="613ee-108">If you're not already a member of the network, you can [join now](https://partners.microsoft.com/PartnerProgram/simplifiedenrollment.aspx).</span></span>  <span data-ttu-id="613ee-109">Microsoft Partner Network のメンバーシップについて詳しくは、[こちら](https://partner.microsoft.com/membership)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="613ee-109">[Learn more](https://partner.microsoft.com/membership) about membership in the Microsoft Partner Network.</span></span> <span data-ttu-id="613ee-110">パートナー センター アカウントを作成したら、こちらのビデオ「[ダッシュボードの検出](https://vimeo.com/290338211)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="613ee-110">After you create a Partner Center account, watch this short video [Discover your dashboard](https://vimeo.com/290338211).</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="613ee-111">始める前に</span><span class="sxs-lookup"><span data-stu-id="613ee-111">Before you begin</span></span>

<span data-ttu-id="613ee-112">パートナーセンターでアカウントを作成するには、次の情報を手元に用意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="613ee-112">To create an account on Partner Center, you'll need to have on hand the following information.</span></span> <span data-ttu-id="613ee-113">作業を開始する前に、これらの情報を手元に準備してください。</span><span class="sxs-lookup"><span data-stu-id="613ee-113">You may want to take a few minutes to gather these items before you get started:</span></span>

-   <span data-ttu-id="613ee-114">全体管理者の職場メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="613ee-114">Global administrator work email.</span></span>

-   <span data-ttu-id="613ee-115">会社の職場アカウントがわからない場合は、会社の[職場アカウントとパートナーセンター](azure-active-directory-tenants-and-partner-center.md)を参照してください。職場のアカウントを持っていない場合は、アカウントの作成プロセス中に作成できます。</span><span class="sxs-lookup"><span data-stu-id="613ee-115">If you're not sure what your company's work account is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md) If your company doesn't have a work account, you can create one during the account creation process.</span></span> 

-   <span data-ttu-id="613ee-116">会社の法務業務名と住所。</span><span class="sxs-lookup"><span data-stu-id="613ee-116">Your company's legal business name and address.</span></span>  

-   <span data-ttu-id="613ee-117">法的合意に署名する権限。</span><span class="sxs-lookup"><span data-stu-id="613ee-117">Authority to sign legal agreements.</span></span> <span data-ttu-id="613ee-118">登録プロセス中に要求されることを確認するため、会社の代理で法的契約に署名する権限があることを確認します。</span><span class="sxs-lookup"><span data-stu-id="613ee-118">Ensure that you are authorized to sign legal agreements on your company's behalf as you'll be asked to do so during the enrollment process.</span></span>

-   <span data-ttu-id="613ee-119">第一連絡先担当者の氏名と会社の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="613ee-119">Name and company email of the person you want to act as your primary contact.</span></span> <span data-ttu-id="613ee-120">会社のセキュリティとプライバシーを確保するために、主要連絡先に電子メールを送信して、(1) パートナーセンターアカウントにサインアップしたこと、および (2) この電子メールアドレスが会社に属していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="613ee-120">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and that (2) this email address belongs to your company.</span></span> <span data-ttu-id="613ee-121">主要連絡先が電子メールアドレスを確認した後、お客様から提供された情報のレビューを続行します。</span><span class="sxs-lookup"><span data-stu-id="613ee-121">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

<span data-ttu-id="613ee-122">この情報は、アカウントの作成プロセス中に確認します。</span><span class="sxs-lookup"><span data-stu-id="613ee-122">We'll verify this information during the account creation process.</span></span> 
 
## <a name="create-a-partner-center-account"></a><span data-ttu-id="613ee-123">パートナー センター アカウントを作成する</span><span class="sxs-lookup"><span data-stu-id="613ee-123">Create a Partner Center account</span></span>

1.  <span data-ttu-id="613ee-124">**[ようこそ]** ページの情報を確認して **[次へ]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="613ee-124">Review the information on the **Welcome** page and then select **Next**.</span></span>

2.  <span data-ttu-id="613ee-125">職場アカウントに、全体管理者としてサインインします。</span><span class="sxs-lookup"><span data-stu-id="613ee-125">Sign in as a global admin to your company's work account.</span></span> <span data-ttu-id="613ee-126">会社の職場アカウントがわからない場合は、[会社の職場アカウントとパートナーセンター](azure-active-directory-tenants-and-partner-center.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="613ee-126">If you're not sure what your company's work account   is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md).</span></span>

    <span data-ttu-id="613ee-127">会社に職場メール アカウントがある場合は、 **[サインイン]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="613ee-127">Select **Sign in** if you know your company has a work email account.</span></span> <span data-ttu-id="613ee-128">次のページで、職場アカウントの全体管理者の資格情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="613ee-128">On the next page, enter global admin credentials for your company's work account.</span></span> 

    <span data-ttu-id="613ee-129">会社に職場のアカウントがない場合は、 **[作成]** を選択して、今すぐ設定します。</span><span class="sxs-lookup"><span data-stu-id="613ee-129">If your company doesn't have a work account, select **Create one** to set one up now.</span></span> <span data-ttu-id="613ee-130">職場アカウントを作成したら、作成した職場アカウントのグローバル管理者の資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="613ee-130">After creating a work account, sign in using your global admin credentials for the work account you just created.</span></span>

3.  <span data-ttu-id="613ee-131">会社の法的ビジネスプロファイルと主要連絡先情報を指定または更新し、 **[今すぐ登録]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="613ee-131">Provide or update your company's legal business profile and primary contact information and then select **Enroll now**.</span></span> 

    <span data-ttu-id="613ee-132">第一連絡先担当者には、貴社の登録申請について連絡できる社内の担当者 (申請者本人または社内の他の担当者) を指定してください。</span><span class="sxs-lookup"><span data-stu-id="613ee-132">The primary contact should be the person in your company we can contact about your application (this can be you or another person in your company).</span></span> <span data-ttu-id="613ee-133">この情報は、この担当者が貴社に勤務し、パートナーセンターアカウントに登録した本人であることを確認するためにも使われます。</span><span class="sxs-lookup"><span data-stu-id="613ee-133">We'll also use this information to verify that this person works at your company and has signed up for a Partner Center account.</span></span>

    > [!IMPORTANT]  
    > <span data-ttu-id="613ee-134">会社のセキュリティとプライバシーを確保するために、主要連絡先に電子メールを送信して、(1) パートナーセンターアカウントにサインアップしたこと、および (2) この電子メールアドレスが会社に属していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="613ee-134">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and (2) that this email address belongs to your company.</span></span> <span data-ttu-id="613ee-135">主要連絡先が電子メールアドレスを確認した後、お客様から提供された情報のレビューを続行します。</span><span class="sxs-lookup"><span data-stu-id="613ee-135">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

4.  <span data-ttu-id="613ee-136">Microsoft Partner Network 契約の諸条件を読んで同意します。</span><span class="sxs-lookup"><span data-stu-id="613ee-136">Read and accept the terms and conditions in the Microsoft Partner Network agreement.</span></span> 

5.  <span data-ttu-id="613ee-137">管理エージェントグループに追加されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="613ee-137">Verify that you've been added to the admin agent group.</span></span> <span data-ttu-id="613ee-138">他のユーザーの追加などを行ってアカウントの設定を完了するには、管理エージェントのアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="613ee-138">To finish setting up your account, including adding other users, you must have admin agent permissions.</span></span> <span data-ttu-id="613ee-139">アクセス許可を表示または更新するには、次の手順を実行します</span><span class="sxs-lookup"><span data-stu-id="613ee-139">Follow these steps to view or update your permissions:</span></span>

    <span data-ttu-id="613ee-140">」を参照します。</span><span class="sxs-lookup"><span data-stu-id="613ee-140">a.</span></span> <span data-ttu-id="613ee-141">パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard/home**)から**設定**アイコンを選択し、 **[ユーザー管理]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="613ee-141">From the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home**), select the **Settings** icon and then select **User management**.</span></span>  

    <span data-ttu-id="613ee-142">b.</span><span class="sxs-lookup"><span data-stu-id="613ee-142">b.</span></span> <span data-ttu-id="613ee-143">ユーザー 一覧から名前を選択し、まだ選択されていない場合は **管理エージェント** を選択します。</span><span class="sxs-lookup"><span data-stu-id="613ee-143">Select your name from the users list and then select **Admin agent** if it's not already selected.</span></span> <span data-ttu-id="613ee-144">**[更新]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="613ee-144">Select **Update**.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="613ee-145">次のステップ</span><span class="sxs-lookup"><span data-stu-id="613ee-145">Next steps</span></span>

-   [<span data-ttu-id="613ee-146">ユーザーの追加とアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="613ee-146">Add account users and assign permissions to them</span></span>](create-user-accounts-and-set-permissions.md)

-   [<span data-ttu-id="613ee-147">Microsoft Action Pack サブスクリプションの購入と更新</span><span class="sxs-lookup"><span data-stu-id="613ee-147">Purchase or renew a subscription to Microsoft Action Pack</span></span>](mpn-get-action-pack.md)

-   [<span data-ttu-id="613ee-148">メンバーシップ特典を管理する</span><span class="sxs-lookup"><span data-stu-id="613ee-148">Manage your membership benefits</span></span>](manage-your-partner-network-benefits.md)

-   [<span data-ttu-id="613ee-149">Silver および Gold メンバーシップ獲得のためのコンピテンシー要件</span><span class="sxs-lookup"><span data-stu-id="613ee-149">Learn about competency requirements for Gold and Silver membership</span></span>](https://partner.microsoft.com/membership/competencies)

-   [<span data-ttu-id="613ee-150">ビジネス プロファイルの作成と Microsoft からの潜在顧客の獲得</span><span class="sxs-lookup"><span data-stu-id="613ee-150">Create a business profile to get sales leads from Microsoft</span></span>](create-a-marketing-profile.md)

-   [<span data-ttu-id="613ee-151">Microsoft から見込み情報を受け取って管理する</span><span class="sxs-lookup"><span data-stu-id="613ee-151">Get and manage sales leads from Microsoft</span></span>](responding-to-referrals.md)