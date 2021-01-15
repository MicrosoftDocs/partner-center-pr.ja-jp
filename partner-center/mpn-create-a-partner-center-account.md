---
title: パートナー センター アカウントを作成する
ms.topic: article
ms.date: 01/07/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Microsoft Partner Network メンバーがネットワークの特典とコンピテンシーを管理するためにパートナー センター アカウントを作成する方法について説明します。
author: ParthP
ms.author: ParthP
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c7aa97760be9fdb2cc004ffd5612826f777c05c5
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979738"
---
# <a name="create-a-partner-center-account-to-manage-network-benefits-and-competencies"></a><span data-ttu-id="9439f-103">ネットワークの特典とコンピテンシーを管理するためにパートナー センター アカウントを作成する</span><span class="sxs-lookup"><span data-stu-id="9439f-103">Create a Partner Center account to manage network benefits and competencies</span></span>

<span data-ttu-id="9439f-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="9439f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="9439f-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="9439f-105">Global admin</span></span>
- <span data-ttu-id="9439f-106">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="9439f-106">Admin agent</span></span>

<span data-ttu-id="9439f-107">パートナー センターでアカウントを作成するには、貴社が Microsoft Partner Network のメンバーである必要があります。</span><span class="sxs-lookup"><span data-stu-id="9439f-107">Before you can create an account on Partner Center, your company must be a member of the Microsoft Partner Network.</span></span> <span data-ttu-id="9439f-108">メンバーでない場合は、[今すぐ登録](https://partner.microsoft.com/commercial#)できます。</span><span class="sxs-lookup"><span data-stu-id="9439f-108">If you're not already a member of the network, you can [join now](https://partner.microsoft.com/commercial#).</span></span> <span data-ttu-id="9439f-109">パートナー センター アカウントを作成したら、こちらのビデオ「[ダッシュボードの検出](https://vimeo.com/290338211)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9439f-109">After you create a Partner Center account, watch this short video [Discover your dashboard](https://vimeo.com/290338211).</span></span>

## <a name="get-a-work-email-address-before-setting-up-a-partner-center-account"></a><span data-ttu-id="9439f-110">パートナー センター アカウントを設定する前に、仕事用メール アドレスを取得します</span><span class="sxs-lookup"><span data-stu-id="9439f-110">Get a work email address before setting up a Partner Center account</span></span>

<span data-ttu-id="9439f-111">従業員の仕事用メール アドレスを設定できるようにするには、会社でメール ドメインを購入する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9439f-111">Your company needs to purchase an email domain in order for you to be able to set up work email addresses for your employees.</span></span> <span data-ttu-id="9439f-112">これは技術的なプロセスであるため、IT 部門と協力してメール ドメインを購入してください。</span><span class="sxs-lookup"><span data-stu-id="9439f-112">Work with your IT department to buy an email domain since this is a technical process.</span></span> <span data-ttu-id="9439f-113">新しいメール アドレスを使用して、Azure AD テナントとパートナー センター アカウントを設定します。</span><span class="sxs-lookup"><span data-stu-id="9439f-113">Use the new email to set up your Azure AD tenant and your Partner Center account.</span></span>

## <a name="get-started"></a><span data-ttu-id="9439f-114">はじめに</span><span class="sxs-lookup"><span data-stu-id="9439f-114">Get started</span></span>

<span data-ttu-id="9439f-115">パートナー センターでアカウントを作成するには、次の情報を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9439f-115">To create an account on Partner Center, you'll need to have on hand the following information.</span></span> <span data-ttu-id="9439f-116">作業を開始する前に、これらの情報を手元に準備してください。</span><span class="sxs-lookup"><span data-stu-id="9439f-116">You may want to take a few minutes to gather these items before you get started:</span></span>

- <span data-ttu-id="9439f-117">全体管理者の職場メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="9439f-117">Global administrator work email.</span></span>

- <span data-ttu-id="9439f-118">会社の職場アカウントがわからない場合は、「[会社の職場アカウントとパートナー センター](azure-active-directory-tenants-and-partner-center.md)」を参照してください。会社に職場アカウントがない場合は、アカウント作成プロセス中に作成できます。</span><span class="sxs-lookup"><span data-stu-id="9439f-118">If you're not sure what your company's work account is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md) If your company doesn't have a work account, you can create one during the account creation process.</span></span> 

- <span data-ttu-id="9439f-119">組織の法人名と住所。</span><span class="sxs-lookup"><span data-stu-id="9439f-119">Your company's legal business name and address.</span></span>  

- <span data-ttu-id="9439f-120">法的合意に署名する権限。</span><span class="sxs-lookup"><span data-stu-id="9439f-120">Authority to sign legal agreements.</span></span> <span data-ttu-id="9439f-121">登録プロセスでは、組織の代表として法的合意への署名を求められるため、その権限があることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="9439f-121">Ensure that you are authorized to sign legal agreements on your company's behalf as you'll be asked to do so during the enrollment process.</span></span>

- <span data-ttu-id="9439f-122">第一連絡先担当者の氏名と会社の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="9439f-122">Name and company email of the person you want to act as your primary contact.</span></span> <span data-ttu-id="9439f-123">マイクロソフトは貴社のセキュリティとプライバシーを確保するため、第一連絡先担当者に、(1) このメール アドレスの持ち主がパートナー センター アカウントに登録した本人であること、および (2) このメール アドレスが貴社に属していることをメールで確認します。</span><span class="sxs-lookup"><span data-stu-id="9439f-123">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and that (2) this email address belongs to your company.</span></span> <span data-ttu-id="9439f-124">第一連絡先担当者と連絡が取れ、そのメール アドレスの正当性が確認された後、提供された情報が引き続き審査されます。</span><span class="sxs-lookup"><span data-stu-id="9439f-124">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

<span data-ttu-id="9439f-125">この情報は、アカウント作成プロセスで確認されます。</span><span class="sxs-lookup"><span data-stu-id="9439f-125">We'll verify this information during the account creation process.</span></span> <span data-ttu-id="9439f-126">確認プロセスの詳細については、[アカウントの確認](verification-responses.md)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9439f-126">For information on the verification process, see [Account verification](verification-responses.md)</span></span>
 
## <a name="create-a-partner-center-account"></a><span data-ttu-id="9439f-127">パートナー センター アカウントを作成する</span><span class="sxs-lookup"><span data-stu-id="9439f-127">Create a Partner Center account</span></span>

1.  <span data-ttu-id="9439f-128">**[ようこそ]** ページの情報を確認して **[次へ]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="9439f-128">Review the information on the **Welcome** page and then select **Next**.</span></span>

2.  <span data-ttu-id="9439f-129">職場アカウントに、全体管理者としてサインインします。</span><span class="sxs-lookup"><span data-stu-id="9439f-129">Sign in as a global admin to your company's work account.</span></span> <span data-ttu-id="9439f-130">職場アカウントについて詳しくは、「[会社の職場アカウントとパートナー センター](azure-active-directory-tenants-and-partner-center.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9439f-130">If you're not sure what your company's work account   is, see [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md).</span></span>

    <span data-ttu-id="9439f-131">会社に職場メール アカウントがある場合は、 **[サインイン]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9439f-131">Select **Sign in** if you know your company has a work email account.</span></span> <span data-ttu-id="9439f-132">次のページで、職場アカウントの全体管理者の資格情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="9439f-132">On the next page, enter global admin credentials for your company's work account.</span></span> 

    <span data-ttu-id="9439f-133">会社に職場アカウントがない場合は、ここで **[作成する]** を選んで作成します。</span><span class="sxs-lookup"><span data-stu-id="9439f-133">If your company doesn't have a work account, select **Create one** to set one up now.</span></span> <span data-ttu-id="9439f-134">職場アカウントを作成した後、その職場アカウントの全体管理者の資格情報を使ってサインインします。</span><span class="sxs-lookup"><span data-stu-id="9439f-134">After creating a work account, sign in using your global admin credentials for the work account you just created.</span></span>

3.  <span data-ttu-id="9439f-135">会社の法的ビジネス プロファイルを指定または更新します。</span><span class="sxs-lookup"><span data-stu-id="9439f-135">Provide or update your company's legal business profile.</span></span>

    <span data-ttu-id="9439f-136">会社のプロファイルを参照するか、会社の情報を手作業で入力することができます。</span><span class="sxs-lookup"><span data-stu-id="9439f-136">You can either lookup your company profile or enter company information manually.</span></span> <span data-ttu-id="9439f-137">会社が [Dun & Bradstreet](https://partner.microsoft.com/marketing/usisvshowcase/dunandbrad) に登録されている場合は、DUNS ID を使用して会社の情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="9439f-137">If your company is registered with [Dun & Bradstreet](https://partner.microsoft.com/marketing/usisvshowcase/dunandbrad), use the DUNS Id to look up your company info.</span></span> <span data-ttu-id="9439f-138">会社の詳細情報を自分で入力する場合は、 **[手動]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9439f-138">If you want to provide your company details yourself, select **Manual**.</span></span>

4. <span data-ttu-id="9439f-139">会社の情報を指定したら、主要な連絡先情報を入力して、 **[今すぐ登録]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9439f-139">Once you have provided the company info, enter the primary contact information and then select **Enroll now**.</span></span>

    <span data-ttu-id="9439f-140">第一連絡先担当者には、貴社の登録申請について連絡できる社内の担当者 (申請者本人または社内の他の担当者) を指定してください。</span><span class="sxs-lookup"><span data-stu-id="9439f-140">The primary contact should be the person in your company we can contact about your application (this can be you or another person in your company).</span></span> <span data-ttu-id="9439f-141">この情報は、この担当者が貴社に勤務し、パートナーセンターアカウントに登録した本人であることを確認するためにも使われます。</span><span class="sxs-lookup"><span data-stu-id="9439f-141">We'll also use this information to verify that this person works at your company and has signed up for a Partner Center account.</span></span>

    > [!IMPORTANT]  
    > <span data-ttu-id="9439f-142">マイクロソフトは貴社のセキュリティとプライバシーを確保するため、第一連絡先担当者に、(1) このメール アドレスの持ち主がパートナー センター アカウントに登録した本人であること、および (2) このメール アドレスが貴社に属していることをメールで確認します。</span><span class="sxs-lookup"><span data-stu-id="9439f-142">To help ensure your company's security and privacy, we'll email your primary contact to verify that (1) he or she signed up for a Partner Center account, and (2) that this email address belongs to your company.</span></span> <span data-ttu-id="9439f-143">第一連絡先担当者と連絡が取れ、そのメール アドレスの正当性が確認された後、提供された情報が引き続き審査されます。</span><span class="sxs-lookup"><span data-stu-id="9439f-143">After the primary contact verifies his or her email address, we'll continue our review of the information you provided.</span></span>

5.  <span data-ttu-id="9439f-144">Microsoft Partner Network 契約の諸条件を読んで同意します。</span><span class="sxs-lookup"><span data-stu-id="9439f-144">Read and accept the terms and conditions in the Microsoft Partner Network agreement.</span></span> 

6.  <span data-ttu-id="9439f-145">管理エージェント グループに追加されたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="9439f-145">Verify that you've been added to the admin agent group.</span></span> <span data-ttu-id="9439f-146">他のユーザーの追加などを行ってアカウントの設定を完了するには、管理エージェントのアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="9439f-146">To finish setting up your account, including adding other users, you must have admin agent permissions.</span></span> <span data-ttu-id="9439f-147">アクセス許可を表示または更新するには、次の手順を実行します</span><span class="sxs-lookup"><span data-stu-id="9439f-147">Follow these steps to view or update your permissions:</span></span>

    <span data-ttu-id="9439f-148">a。</span><span class="sxs-lookup"><span data-stu-id="9439f-148">a.</span></span> <span data-ttu-id="9439f-149">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard/home**)で **[設定]** アイコンを選択し、 **[ユーザー管理]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9439f-149">From the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home**), select the **Settings** icon and then select **User management**.</span></span>  

    <span data-ttu-id="9439f-150">b.</span><span class="sxs-lookup"><span data-stu-id="9439f-150">b.</span></span> <span data-ttu-id="9439f-151">ユーザーの一覧から自分の名前を選び、 **[管理エージェント]** を選択します (まだ選択されていない場合)。</span><span class="sxs-lookup"><span data-stu-id="9439f-151">Select your name from the users list and then select **Admin agent** if it's not already selected.</span></span> <span data-ttu-id="9439f-152">**[更新]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9439f-152">Select **Update**.</span></span>  

## <a name="view-mpn-account-details"></a><span data-ttu-id="9439f-153">MPN アカウントの詳細を表示する</span><span class="sxs-lookup"><span data-stu-id="9439f-153">View MPN account details</span></span>

<span data-ttu-id="9439f-154">パートナー センター アカウントを作成すると、パートナー センターに戻って、さまざまなアカウントの詳細を確認できるようになります。</span><span class="sxs-lookup"><span data-stu-id="9439f-154">Once you create a Partner Center account, you can return to Partner Center to see various account details.</span></span> <span data-ttu-id="9439f-155">これらの多くは、パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)の **[パートナー プロファイル]** ページに表示されます。</span><span class="sxs-lookup"><span data-stu-id="9439f-155">Many of these appear on the **Partner profile** page in your Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

<span data-ttu-id="9439f-156">次の詳細を確認できます。</span><span class="sxs-lookup"><span data-stu-id="9439f-156">Such details include:</span></span>

- <span data-ttu-id="9439f-157">お客様の会社の法的ビジネス プロファイル</span><span class="sxs-lookup"><span data-stu-id="9439f-157">Your company's legal business profile</span></span>

- <span data-ttu-id="9439f-158">MPN ID に関する情報</span><span class="sxs-lookup"><span data-stu-id="9439f-158">Information about your MPN ID</span></span>

- <span data-ttu-id="9439f-159">登録済みの Microsoft プログラムに関連付けられている現在の契約へのリンク</span><span class="sxs-lookup"><span data-stu-id="9439f-159">Links to current agreements associated with your enrolled Microsoft program</span></span>

  <span data-ttu-id="9439f-160">たとえば、お客様が MPN プログラムに登録されている場合、現在の Microsoft Partner Network 契約へのリンクが表示されます。</span><span class="sxs-lookup"><span data-stu-id="9439f-160">For example, if you are enrolled in the MPN program, you'll see a link to the current Microsoft Partner Network agreement.</span></span> <span data-ttu-id="9439f-161">クラウド ソリューション プロバイダー (CSP) プログラムなどの他のパートナー プログラムに登録されている場合は、Microsoft Partner Agreement などの他の契約へのリンクも表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9439f-161">If you're enrolled in other partner programs, like the Cloud Solution Provider (CSP) program, you may also see links to other agreements, such as the Microsoft Partner Agreement.</span></span> 

  > [!NOTE]
  > <span data-ttu-id="9439f-162">これらの種類のリンクが表示されるのは、契約の確認、アクセス、ダウンロードが必要になる場合や、署名の日付を確認する場合などに便利です。</span><span class="sxs-lookup"><span data-stu-id="9439f-162">Seeing these types of links may be useful if you ever want to review, access, or download an agreement, or, check the date it was signed.</span></span>

### <a name="how-to-view-account-details-or-view-and-download-the-mpn-agreement"></a><span data-ttu-id="9439f-163">アカウントの詳細を表示する方法、または MPN 契約を表示してダウンロードする方法</span><span class="sxs-lookup"><span data-stu-id="9439f-163">How to view account details or view and download the MPN agreement</span></span>

<span data-ttu-id="9439f-164">アカウントの詳細を表示する場合や、MPN 契約を表示してダウンロードする場合は、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="9439f-164">Follow these steps to view account details or view and download the MPN agreement:</span></span>

1. <span data-ttu-id="9439f-165">職場アカウントのユーザー名とパスワードを使用して、パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="9439f-165">Using your work account username and password, sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="9439f-166">[概要] ページが表示されます。</span><span class="sxs-lookup"><span data-stu-id="9439f-166">An Overview page appears.</span></span> <span data-ttu-id="9439f-167">([概要] ページが表示されない場合は、左側のナビゲーション メニューから **[概要]** を選択します)。</span><span class="sxs-lookup"><span data-stu-id="9439f-167">(If you do not see the Overview page, select **Overview** from the left-navigation menu.)</span></span>

3. <span data-ttu-id="9439f-168">ダッシュボードの右上隅にある歯車アイコンを選択し、 **[パートナーの設定]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9439f-168">Select the Gear icon in the top-right corner of the dashboard, then select **Partner settings**.</span></span> <span data-ttu-id="9439f-169">すると、[パートナー プロファイル] ページが表示されます。</span><span class="sxs-lookup"><span data-stu-id="9439f-169">This takes you to the Partner profile page.</span></span>

4. <span data-ttu-id="9439f-170">[パートナー プロファイル] ページには、さまざまな領域が表示されます。</span><span class="sxs-lookup"><span data-stu-id="9439f-170">From the Partner profile page, you'll see different areas.</span></span> <span data-ttu-id="9439f-171">これには、 **[Legal business profile]\(法的ビジネス プロファイル\)** や **[プログラム情報]** 領域が含まれます。</span><span class="sxs-lookup"><span data-stu-id="9439f-171">These include a **Legal business profile** area and a **Program info** area.</span></span>

5. <span data-ttu-id="9439f-172">**[プログラム情報]** の下にある **[MPN プログラムの状態]** フィールドを見つけます。</span><span class="sxs-lookup"><span data-stu-id="9439f-172">Under **Program info**, locate the **MPN program status** field.</span></span> <span data-ttu-id="9439f-173">ここに、Microsoft Partner Network 契約へのリンクが表示されています。</span><span class="sxs-lookup"><span data-stu-id="9439f-173">This displays a link to your Microsoft Partner Network agreement.</span></span> <span data-ttu-id="9439f-174">また、プログラムでのお客様の現在の状態についても表示されています。</span><span class="sxs-lookup"><span data-stu-id="9439f-174">It also describes your current status in the program.</span></span>


   :::image type="content" source="images/accountsettings/mpn-program-info-download-mpn-agreement.png" alt-text="[パートナー プロファイル] ページの [プログラム情報] 領域の画像。この領域の [MPN プログラムの状態] フィールドと、関連付けられている Microsoft Partner Network 契約へのリンクが赤枠で強調表示されている。":::

6. <span data-ttu-id="9439f-176">この契約を表示またはダウンロードするには、 **[Microsoft Partner Network 契約]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9439f-176">To view or download this agreement, select **Microsoft Partner Network agreement**.</span></span>  

> [!NOTE]
> <span data-ttu-id="9439f-177">また、クラウド ソリューション プロバイダー (CSP) プログラムに登録されている場合は Microsoft Partner Agreement など、他の登録済みプログラムに関する他の契約も上記の手順で表示またはダウンロードすることができます。</span><span class="sxs-lookup"><span data-stu-id="9439f-177">You can also use the above steps to view or download other agreements for other, enrolled programs, such as the Microsoft Partner Agreement if you happen to be enrolled in the Cloud Solution Provider (CSP) program.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9439f-178">次の手順</span><span class="sxs-lookup"><span data-stu-id="9439f-178">Next steps</span></span>

-   [<span data-ttu-id="9439f-179">ユーザーの追加とアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="9439f-179">Add account users and assign permissions to them</span></span>](create-user-accounts-and-set-permissions.md)

-   [<span data-ttu-id="9439f-180">Microsoft Action Pack サブスクリプションの購入と更新</span><span class="sxs-lookup"><span data-stu-id="9439f-180">Purchase or renew a subscription to Microsoft Action Pack</span></span>](mpn-get-action-pack.md)

-   [<span data-ttu-id="9439f-181">メンバーシップ特典を管理する</span><span class="sxs-lookup"><span data-stu-id="9439f-181">Manage your membership benefits</span></span>](manage-your-partner-network-benefits.md)

-   [<span data-ttu-id="9439f-182">Silver および Gold メンバーシップ獲得のためのコンピテンシー要件</span><span class="sxs-lookup"><span data-stu-id="9439f-182">Learn about competency requirements for Gold and Silver membership</span></span>](https://partner.microsoft.com/membership/competencies)

-   [<span data-ttu-id="9439f-183">ビジネス プロファイルの作成と Microsoft からの潜在顧客の獲得</span><span class="sxs-lookup"><span data-stu-id="9439f-183">Create a business profile to get sales leads from Microsoft</span></span>](create-a-marketing-profile.md)

-   [<span data-ttu-id="9439f-184">Microsoft から見込み情報を受け取って管理する</span><span class="sxs-lookup"><span data-stu-id="9439f-184">Get and manage sales leads from Microsoft</span></span>](manage-leads.md)
