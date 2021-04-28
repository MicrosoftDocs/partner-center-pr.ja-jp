---
title: パートナー センターで MPN アカウントを作成する
ms.topic: article
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Microsoft Partner Network メンバーがネットワークの特典とコンピテンシーを管理するためにパートナー センター アカウントを作成する方法について説明します。
author: ParthP
ms.author: ParthP
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 27cd00b5475914019963fad381b36b47a017dcf1
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120802"
---
# <a name="create-an-mpn-account-in-partner-center-to-manage-network-benefits-and-competencies"></a><span data-ttu-id="c3f7c-103">ネットワークの特典とコンピテンシーを管理するためにパートナー センターで MPN アカウントを作成する</span><span class="sxs-lookup"><span data-stu-id="c3f7c-103">Create an MPN account in Partner Center to manage network benefits and competencies</span></span>

<span data-ttu-id="c3f7c-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="c3f7c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c3f7c-105">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="c3f7c-105">MPN partner admin</span></span>

<span data-ttu-id="c3f7c-106">Microsoft Partner Network (MPN) を初めて利用する、MPN ID をお持ちでないパートナーは、[登録手順](https://partner.microsoft.com/dashboard/account/v3/enrollment/introduction/partnership)に従って登録を始めることができます。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-106">If you are new to Microsoft Partner Network (MPN) and don’t have an MPN ID, you can start your enrollment by following the [enrollment instructions](https://partner.microsoft.com/dashboard/account/v3/enrollment/introduction/partnership).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3f7c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c3f7c-107">Prerequisites</span></span> 

<span data-ttu-id="c3f7c-108">パートナー センターでアカウントを作成する準備ができたら、次のものを用意してください。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-108">When you are ready to create an account on Partner Center, you will need to have the following items on hand.</span></span>  <span data-ttu-id="c3f7c-109">作業を開始する前に、これらの情報を手元に準備してください。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-109">You may want to take a few minutes to gather these items before you get started:</span></span>

- <span data-ttu-id="c3f7c-110">会社の仕事用メール アドレス、または Office 365 の職場アカウント。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-110">Company work email OR Office 365 work account.</span></span> <span data-ttu-id="c3f7c-111">従業員の仕事用メール アドレスを設定するには、会社でメール ドメインを購入する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-111">Your company may need to purchase an email domain in order for you to set up work email addresses for your employees.</span></span> <span data-ttu-id="c3f7c-112">詳しくは、「[会社の職場アカウントとパートナー センター](azure-active-directory-tenants-and-partner-center.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-112">For more information, read [Your company work account and Partner Center](azure-active-directory-tenants-and-partner-center.md).</span></span> 
 
- <span data-ttu-id="c3f7c-113">組織の法人名と住所。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-113">Your company's legal business name and address.</span></span>

- <span data-ttu-id="c3f7c-114">法的合意に署名する権限。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-114">Authority to sign legal agreements.</span></span> <span data-ttu-id="c3f7c-115">登録プロセスでは、組織の代表として法的合意への署名を求められるため、その権限があることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-115">Ensure that you are authorized to sign legal agreements on your company's behalf as you'll be asked to do so during the enrollment process.</span></span>

- <span data-ttu-id="c3f7c-116">第一連絡先担当者の氏名と会社の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-116">Name and company email of the person you want to act as your primary contact.</span></span> <span data-ttu-id="c3f7c-117">マイクロソフトは貴社のセキュリティとプライバシーを確保するため、第一連絡先担当者宛てにメールを送ってメール アドレスを検証し、そのメール アドレスが貴社に属していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-117">To help ensure your company's security and privacy, we email your primary contact to verify the email address and to ensure that the email address belongs to your company.</span></span> <span data-ttu-id="c3f7c-118">第一連絡先担当者によってそのメール アドレスの正当性が確認された後、提供された情報が引き続き審査されます。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-118">After the primary contact verifies the email address, we'll continue our review of the information provided.</span></span> <span data-ttu-id="c3f7c-119">通常、確認には 3 から 5 営業日かかります。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-119">Verification usually takes 3-5 business days.</span></span> 

- <span data-ttu-id="c3f7c-120">確認プロセスの詳細については、[アカウントの確認](verification-responses.md)に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-120">For information on the verification process, see [Account verification](verification-responses.md).</span></span>

>[!NOTE]
><span data-ttu-id="c3f7c-121">お使いの Microsoft Partner Network メンバーシップが Partner Membership Center (PMC) にまだある場合は、パートナー センターにアカウントを直ちに移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-121">If your Microsoft Partner Network membership is still in Partner Membership Center (PMC), you need to migrate your account immediately to Partner Center.</span></span> <span data-ttu-id="c3f7c-122">[移行の詳細な手順に関するガイド](https://assetsprod.microsoft.com/mpn/migrate-pmc-pc-mpa-guide.pptx)をダウンロードしてください。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-122">Download the [step-by-step guide to migrate](https://assetsprod.microsoft.com/mpn/migrate-pmc-pc-mpa-guide.pptx).</span></span>

## <a name="get-started"></a><span data-ttu-id="c3f7c-123">作業開始</span><span class="sxs-lookup"><span data-stu-id="c3f7c-123">Get started</span></span>

1. <span data-ttu-id="c3f7c-124">[**作業開始**](https://partner.microsoft.com/dashboard/account/v3/enrollment/introduction/partnership)ページで、会社から支給された you@yourcompanyname.com のような仕事用メールを使用して作業を始めてください。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-124">At the [**Get started**](https://partner.microsoft.com/dashboard/account/v3/enrollment/introduction/partnership) page, start with your work email given to you by your company, for example, you@yourcompanyname.com.</span></span>

 
    <span data-ttu-id="c3f7c-125">a.</span><span class="sxs-lookup"><span data-stu-id="c3f7c-125">a.</span></span>  <span data-ttu-id="c3f7c-126">作業を続けるために、そのメールアドレスに確認コードをお送りしますので、そのメールアドレスはお客様にアクセスできる有なメール アドレスである必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-126">The email address must be valid and accessible to you because we will send a verification code to that email to continue.</span></span>

    <span data-ttu-id="c3f7c-127">b.</span><span class="sxs-lookup"><span data-stu-id="c3f7c-127">b.</span></span>  <span data-ttu-id="c3f7c-128">次のような単語が含まれるメール アドレスを使用することはできません。"info"、"admin"、"email@"</span><span class="sxs-lookup"><span data-stu-id="c3f7c-128">The email address should not contain words like "info," "admin," "email@."</span></span> <span data-ttu-id="c3f7c-129">または "marketing@.."。これらのアドレス形式はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-129">Or "marketing@..."; these address formats are not supported.</span></span>

    <span data-ttu-id="c3f7c-130">c.</span><span class="sxs-lookup"><span data-stu-id="c3f7c-130">c.</span></span>  <span data-ttu-id="c3f7c-131">MAPS を購入したり、コンピテンシーを管理したりするには、[ご自分のドメインを確認](become-global-admin.md)して管理者になることにより、このアカウントをアップグレードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-131">To purchase MAPS or manage competencies, you will have to upgrade this account by [verifying your domain](become-global-admin.md) and becoming an admin.</span></span> 

2. <span data-ttu-id="c3f7c-132">you@contoso.onmicrosoft.com などの Office 365 職場アカウントを使用して、サインインすることができます。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-132">You can sign in with your Office 365 work account, for example, you@contoso.onmicrosoft.com.</span></span>

   >[!NOTE]
   > <span data-ttu-id="c3f7c-133">既存の CSP アカウントの資格情報を使用して、MPN に登録することはできません。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-133">You can’t use your existing CSP account credentials to enroll into MPN.</span></span>

3. <span data-ttu-id="c3f7c-134">貴社の法人に関する詳細を提供してください。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-134">Provide your company's legal business details.</span></span>

<span data-ttu-id="c3f7c-135">会社のプロファイルを参照するか、会社の情報を手作業で入力することができます。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-135">You can either look up your company profile or enter company information manually.</span></span> <span data-ttu-id="c3f7c-136">会社を [Dun & Bradstreet](https://partner.microsoft.com/marketing/usisvshowcase/dunandbrad) に登録している場合は、DUNS ID を使用して会社の情報を確認してください。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-136">If your company is registered with [Dun & Bradstreet](https://partner.microsoft.com/marketing/usisvshowcase/dunandbrad), use the DUNS ID to look up your company info.</span></span> <span data-ttu-id="c3f7c-137">会社の詳細情報を自分で入力する場合は、 **[手動]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-137">If you want to provide your company details yourself, select **Manual**.</span></span>

<span data-ttu-id="c3f7c-138">会社が **アルメニア**、**ハンガリー**、**キルギス**、**モルドバ**、**ウズベキスタン**、**ロシア** にあり、住所を手動で入力する場合は、お客様の住所が確認されます。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-138">If your company is located in **Armenia**, **Hungary**, **Kyrgyzstan**, **Moldova**, **Uzbekistan**, or **Russia**, and you enter your address manually, we will validate your address for you.</span></span> <span data-ttu-id="c3f7c-139">入力したものが確認されたものと異なる場合は、確認済みの住所を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-139">If the one you enter differs from the validated one, we suggest you use the validated address.</span></span> <span data-ttu-id="c3f7c-140">これにより、国の郵便局による定義に従って、住所の要素が標準化され、正しい形式になり、配送可能になります。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-140">This ensures that the elements of the address are standardized as defined by the country's postal authority, correctly formatted, and shippable.</span></span>  

<span data-ttu-id="c3f7c-141">会社の情報を指定したら、第一連絡先担当者情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-141">Once you have provided the company info, enter the primary contact information.</span></span> <span data-ttu-id="c3f7c-142">第一連絡先担当者には、貴社の登録申請について連絡できる社内の担当者 (申請者本人または社内の他の担当者) を指定してください。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-142">The primary contact should be the person in your company we can contact about your application (this contact can be you or another person in your company).</span></span>

4. <span data-ttu-id="c3f7c-143">**[今すぐ登録する]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-143">Select **Enroll now**.</span></span>

>[!IMPORTANT]
><span data-ttu-id="c3f7c-144">マイクロソフトは貴社のセキュリティとプライバシーを確保するため、第一連絡先担当者宛てにメールを送ってメール アドレスを検証し、そのメール アドレスが貴社に属していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-144">To help ensure your company's security and privacy, we email your primary contact to verify the email address and ensure that the email address belongs to your company.</span></span> <span data-ttu-id="c3f7c-145">第一連絡先担当者によってそのメール アドレスの正当性が確認された後、提供された情報が引き続き審査されます。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-145">After the primary contact verifies the email address, we'll continue our review of the information you provided.</span></span> <span data-ttu-id="c3f7c-146">通常、確認には 3 から 5 営業日かかります。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-146">Verification usually takes 3-5 business days.</span></span> 

## <a name="how-to-view-account-details-or-view-and-download-the-mpn-agreement"></a><span data-ttu-id="c3f7c-147">アカウントの詳細を表示する方法、または MPN 契約を表示してダウンロードする方法</span><span class="sxs-lookup"><span data-stu-id="c3f7c-147">How to view account details or view and download the MPN agreement</span></span>

<span data-ttu-id="c3f7c-148">MPN の資格情報を使用して、パートナー センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-148">Sign into Partner Center with your MPN credentials.</span></span> <span data-ttu-id="c3f7c-149">[**パートナー プロファイル**](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile)を選択して、会社の法的な詳細、検証の状態、MPN ID を確認し、必要に応じて新しい MPN の場所を作成します。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-149">Select [**Partner profile**](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) to view your company’s legal details, your verification status, your MPN IDs and also create new MPN locations if needed.</span></span> 

<span data-ttu-id="c3f7c-150">また、次のスクリーンショットに示すように、左側のメニュー リンクを使用して、MPN ID のような他の重要な情報を確認したり、MPN の場所を管理したり、Microsoft Partner Agreement を表示したりすることもできます。</span><span class="sxs-lookup"><span data-stu-id="c3f7c-150">You can also view other important information like MPN Ids, manage MPN locations, and view Microsoft Partner Agreement using the left menu links as show in the following screenshot.</span></span>

:::image type="content" source="images/mpn-new.png" alt-text="パートナー プロファイル":::


## <a name="next-steps"></a><span data-ttu-id="c3f7c-152">次の手順</span><span class="sxs-lookup"><span data-stu-id="c3f7c-152">Next steps</span></span>

-  [<span data-ttu-id="c3f7c-153">ユーザーの追加とアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="c3f7c-153">Add account users and assign permissions to them</span></span>](create-user-accounts-and-set-permissions.md)

-  [<span data-ttu-id="c3f7c-154">Microsoft Action Pack サブスクリプションの購入と更新</span><span class="sxs-lookup"><span data-stu-id="c3f7c-154">Purchase or renew a subscription to Microsoft Action Pack</span></span>](mpn-get-action-pack.md)

-  [<span data-ttu-id="c3f7c-155">メンバーシップ特典を管理する</span><span class="sxs-lookup"><span data-stu-id="c3f7c-155">Manage your membership benefits</span></span>](manage-your-partner-network-benefits.md)

-  [<span data-ttu-id="c3f7c-156">Silver および Gold メンバーシップ獲得のためのコンピテンシー要件</span><span class="sxs-lookup"><span data-stu-id="c3f7c-156">Learn about competency requirements for Gold and Silver membership</span></span>](https://partner.microsoft.com/membership/competencies)

-  [<span data-ttu-id="c3f7c-157">ビジネス プロファイルの作成と Microsoft からの潜在顧客の獲得</span><span class="sxs-lookup"><span data-stu-id="c3f7c-157">Create a business profile to get sales leads from Microsoft</span></span>](create-a-marketing-profile.md)

-  [<span data-ttu-id="c3f7c-158">Microsoft から見込み情報を受け取って管理する</span><span class="sxs-lookup"><span data-stu-id="c3f7c-158">Get and manage sales leads from Microsoft</span></span>](manage-leads.md)
