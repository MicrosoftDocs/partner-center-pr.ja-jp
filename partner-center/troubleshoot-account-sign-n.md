---
title: パートナーセンターのアカウントの設定または MPN の更新に関する問題のトラブルシューティング
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: パートナーセンターへの登録に関する問題のトラブルシューティング
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a516d569791356c4ba967b8835268562d1597a16
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/25/2020
ms.locfileid: "88848949"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="ae006-103">アカウントのセットアップまたは MPN 更新に関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="ae006-103">Troubleshoot account setup or MPN renewal issues</span></span>

### <a name="applies-to"></a><span data-ttu-id="ae006-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="ae006-104">Applies to</span></span>

- <span data-ttu-id="ae006-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="ae006-105">Partner Center</span></span>
 
### <a name="appropriate-roles"></a><span data-ttu-id="ae006-106">適切なロール</span><span class="sxs-lookup"><span data-stu-id="ae006-106">Appropriate roles</span></span>

- <span data-ttu-id="ae006-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="ae006-107">Global admin</span></span>
- <span data-ttu-id="ae006-108">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="ae006-108">MPN partner admin</span></span> 
 

<span data-ttu-id="ae006-109">ここでは、パートナーセンターアカウントを設定するときに発生する一般的な問題のトラブルシューティングに関するいくつかの推奨事項を示します。</span><span class="sxs-lookup"><span data-stu-id="ae006-109">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

### <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="ae006-110">パートナーメンバーシップセンターから移行するときに、会社情報フィールドを編集できない場合はどうなりますか</span><span class="sxs-lookup"><span data-stu-id="ae006-110">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="ae006-111">これは、会社が既にパートナーセンター (CSP アカウントなど) に存在している場合に発生します。読み取り専用の画面が表示され、パートナーセンターに存在する会社のすべての情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="ae006-111">This occurs in cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen which will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="ae006-112">この画面の詳細を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="ae006-112">You cannot change the details on this screen.</span></span> <span data-ttu-id="ae006-113">これは仕様であり、エラーではありません。</span><span class="sxs-lookup"><span data-stu-id="ae006-113">This is by design and not an error.</span></span>

<span data-ttu-id="ae006-114">[ **同意** して **続行** ] を選択して続行します。</span><span class="sxs-lookup"><span data-stu-id="ae006-114">Select **Accept** and **Continue** to proceed.</span></span>

### <a name="you-are-trying-to-enroll-or-to-migrate-from-partner-membership-center-and-you-receive-an-error-message-saying-that-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="ae006-115">パートナーメンバーシップセンターから登録または移行しようとしているときに、IT 部門が **パートナーセンターへのサインアップ**を無効にしたことを示すエラーメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="ae006-115">You are trying to enroll or to migrate from Partner Membership Center and you receive an error message saying that the IT department has turned off **sign up for Partner Center**.</span></span> 

<span data-ttu-id="ae006-116">このメッセージが表示されるのは、ウイルスに感染したユーザーが無効になっているか、Azure AD テナントでウイルスによるサインアップが無効になっているためです。</span><span class="sxs-lookup"><span data-stu-id="ae006-116">You see this message because viral users are disabled, or Viral Sign up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="ae006-117">Azure AD アカウントの全体管理者は、次の PowerShell コマンドを実行して、必要な機能を有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ae006-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="ae006-118">**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="ae006-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="ae006-119">詳細については、「[セルフサービスサインアップ](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae006-119">For more information, read [Self-service sign up](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

### <a name="you-forgot-your-password"></a><span data-ttu-id="ae006-120">パスワードを忘れた場合</span><span class="sxs-lookup"><span data-stu-id="ae006-120">You forgot your password</span></span>

<span data-ttu-id="ae006-121">パスワードを忘れた場合は、サインインページの [ **アカウントにアクセスできませんか?** ] リンクを選択してパスワードをリセットするか、全体管理者に新しい資格情報の割り当てを依頼してください。</span><span class="sxs-lookup"><span data-stu-id="ae006-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page to reset your password, or ask your Global admin to assign you new credentials.</span></span>

### <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="ae006-122">[会社情報をお聞かせください] 画面で、"問題が発生しました" というエラーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="ae006-122">On the “Tell us about your company” screen you receive a “Something went wrong” error</span></span>

<span data-ttu-id="ae006-123">これは通常、会社の電話番号で特殊文字、スペース、または国コードを使用している場合に発生します。</span><span class="sxs-lookup"><span data-stu-id="ae006-123">This usually happens if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="ae006-124">[電話番号] フィールドに入力する値には、最大で10文字まで含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ae006-124">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>

### <a name="you-are-trying-to-complete-the-purchase-via-credit-card-but-you-are-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="ae006-125">クレジットカードを使用して購入を完了しようとしていますが、"注文が拒否されました。</span><span class="sxs-lookup"><span data-stu-id="ae006-125">You are trying to complete the purchase via credit card, but you are receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="ae006-126">情報を確認してください "</span><span class="sxs-lookup"><span data-stu-id="ae006-126">Please verify your information”</span></span>

<span data-ttu-id="ae006-127">クレジットカードに対応するアドレスを挿入する必要があります。これは、法人に対応するものではありません。</span><span class="sxs-lookup"><span data-stu-id="ae006-127">You should always insert the address corresponding to your credit card and not corresponding to your legal entity.</span></span> <span data-ttu-id="ae006-128">また、郵便番号が正しいことと、使用するアドレスに対応していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="ae006-128">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

### <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="ae006-129">オフライン支払いからオンライン支払方法に切り替える場合</span><span class="sxs-lookup"><span data-stu-id="ae006-129">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="ae006-130">優先支払い方法を使用して、元の注文と再購入を取り消す必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae006-130">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="ae006-131">注文を取り消すには:</span><span class="sxs-lookup"><span data-stu-id="ae006-131">To cancel an order:</span></span>

1. <span data-ttu-id="ae006-132">ダッシュボードの [ **メンバーシップの提供** ] タブを選択します。</span><span class="sxs-lookup"><span data-stu-id="ae006-132">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="ae006-133">**取り消し順序**の選択</span><span class="sxs-lookup"><span data-stu-id="ae006-133">Select **Cancel order**</span></span>

3. <span data-ttu-id="ae006-134">確認ウィンドウが表示され、最初の順序を取り消すために確認を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae006-134">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>
