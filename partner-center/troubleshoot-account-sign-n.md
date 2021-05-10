---
title: アカウントまたは MPN の更新パートナー センターの設定に関するトラブルシューティング
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: アプリケーションに登録しようとするときに発生する問題パートナー センター。 回答は、支払い方法やパスワードの忘れなどによる課題に対処します。
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686264"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="bfe30-104">アカウントのセットアップまたは MPN の更新に関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="bfe30-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="bfe30-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="bfe30-105">**Appropriate roles**</span></span>

- <span data-ttu-id="bfe30-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="bfe30-106">Global admin</span></span>
- <span data-ttu-id="bfe30-107">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="bfe30-107">MPN partner admin</span></span>
 
<span data-ttu-id="bfe30-108">次に示すのは、アカウントのセットアップ時に発生する一般的な問題のトラブルシューティングパートナー センターです。</span><span class="sxs-lookup"><span data-stu-id="bfe30-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="bfe30-109">会社の情報フィールドを編集できないPartner Membership Centerから移行するとどうなるか</span><span class="sxs-lookup"><span data-stu-id="bfe30-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="bfe30-110">会社が既に パートナー センター に存在する場合 (CSP アカウントなど)、読み取り専用画面が表示されます。</span><span class="sxs-lookup"><span data-stu-id="bfe30-110">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="bfe30-111">この画面には、会社に関する情報が表示されます。この画面は、パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="bfe30-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="bfe30-112">この画面で詳細を変更できない。</span><span class="sxs-lookup"><span data-stu-id="bfe30-112">You can't change the details on this screen.</span></span> <span data-ttu-id="bfe30-113">これは設計上の問題であり、エラーではありません。</span><span class="sxs-lookup"><span data-stu-id="bfe30-113">This is by design and not an error.</span></span>

<span data-ttu-id="bfe30-114">[同意 **して続行]** **を選択して** 続行します。</span><span class="sxs-lookup"><span data-stu-id="bfe30-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="bfe30-115">IT 部門が [サインアップ] をオフに **したパートナー センター**</span><span class="sxs-lookup"><span data-stu-id="bfe30-115">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="bfe30-116">このメッセージが表示されるのは、バイラル ユーザーが無効になっているか、またはバイラル サインアップがテナントの Azure ADされます。</span><span class="sxs-lookup"><span data-stu-id="bfe30-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="bfe30-117">次の PowerShell コマンドを実行Azure ADアカウントのグローバル管理者は、必要な機能を有効にできます。</span><span class="sxs-lookup"><span data-stu-id="bfe30-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="bfe30-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="bfe30-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="bfe30-119">詳細については、「セルフサービス サインアップ [」を参照してください](/azure/active-directory/users-groups-roles/directory-self-service-signup)。</span><span class="sxs-lookup"><span data-stu-id="bfe30-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="bfe30-120">パスワードを忘れた</span><span class="sxs-lookup"><span data-stu-id="bfe30-120">You forgot your password</span></span>

<span data-ttu-id="bfe30-121">パスワードを忘れた場合は、サインイン ページの [アカウントにアクセスできませんか **?** ] リンクを選択します。</span><span class="sxs-lookup"><span data-stu-id="bfe30-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="bfe30-122">このオプションを使用すると、パスワードをリセットしたり、グローバル管理者に新しい資格情報を割り当て要求したりできます。</span><span class="sxs-lookup"><span data-stu-id="bfe30-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="bfe30-123">[会社について教えて] 画面で、"問題が発生しました" というエラーが表示されます</span><span class="sxs-lookup"><span data-stu-id="bfe30-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="bfe30-124">このエラーメッセージは、通常、会社の電話番号で特殊文字、スペース、または国コードを使用している場合に表示されます。</span><span class="sxs-lookup"><span data-stu-id="bfe30-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="bfe30-125">[電話番号] フィールドに入力する値には、最大で10文字まで含めることができます。</span><span class="sxs-lookup"><span data-stu-id="bfe30-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="bfe30-126">クレジットカードの購入で、"注文が拒否されました。</span><span class="sxs-lookup"><span data-stu-id="bfe30-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="bfe30-127">情報を確認してください "</span><span class="sxs-lookup"><span data-stu-id="bfe30-127">Please verify your information”</span></span>


<span data-ttu-id="bfe30-128">法人ではなく、クレジットカードに対応する住所を常に使用してください。</span><span class="sxs-lookup"><span data-stu-id="bfe30-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="bfe30-129">また、郵便番号が正しいことと、使用するアドレスに対応していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="bfe30-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="bfe30-130">オフライン支払いからオンライン支払方法に切り替える場合</span><span class="sxs-lookup"><span data-stu-id="bfe30-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="bfe30-131">優先支払い方法を使用して、元の注文と再購入を取り消す必要があります。</span><span class="sxs-lookup"><span data-stu-id="bfe30-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="bfe30-132">注文を取り消すには:</span><span class="sxs-lookup"><span data-stu-id="bfe30-132">To cancel an order:</span></span>

1. <span data-ttu-id="bfe30-133">ダッシュボードの [ **メンバーシップの提供** ] タブを選択します。</span><span class="sxs-lookup"><span data-stu-id="bfe30-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="bfe30-134">**取り消し順序** の選択</span><span class="sxs-lookup"><span data-stu-id="bfe30-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="bfe30-135">確認ウィンドウが表示され、最初の順序を取り消すために確認を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="bfe30-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bfe30-136">次の手順</span><span class="sxs-lookup"><span data-stu-id="bfe30-136">Next steps</span></span>

- [<span data-ttu-id="bfe30-137">パートナー センター アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="bfe30-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="bfe30-138">請求書と偵察を読む方法</span><span class="sxs-lookup"><span data-stu-id="bfe30-138">How to read your bill and recon file</span></span>](read-your-bill.md)
