---
title: パートナーセンターのアカウントの設定または MPN の更新に関する問題のトラブルシューティング
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: パートナーセンターに登録しようとしたときに発生する問題のトラブルシューティングを行います。 回答は、支払い方法やパスワードを忘れた場合の課題に対処します。
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d990a2cb4dcb69dfc76e8a4f0d40fd4912b4f8a0
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/19/2020
ms.locfileid: "92174845"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="7ac2b-104">アカウントのセットアップまたは MPN 更新に関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="7ac2b-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="7ac2b-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="7ac2b-105">**Applies to**</span></span>

- <span data-ttu-id="7ac2b-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="7ac2b-106">Partner Center</span></span>
 
<span data-ttu-id="7ac2b-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="7ac2b-107">**Appropriate roles**</span></span>

- <span data-ttu-id="7ac2b-108">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="7ac2b-108">Global admin</span></span>
- <span data-ttu-id="7ac2b-109">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="7ac2b-109">MPN partner admin</span></span> 
 
<span data-ttu-id="7ac2b-110">ここでは、パートナーセンターアカウントを設定するときに発生する一般的な問題のトラブルシューティングに関するいくつかの推奨事項を示します。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-110">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="7ac2b-111">パートナーメンバーシップセンターから移行するときに、会社情報フィールドを編集できない場合はどうなりますか</span><span class="sxs-lookup"><span data-stu-id="7ac2b-111">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="7ac2b-112">会社が既にパートナーセンター (CSP アカウントなど) に存在している場合は、読み取り専用画面が表示されます。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-112">In cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="7ac2b-113">この画面には、パートナーセンターに存在する会社に関するすべての情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-113">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="7ac2b-114">この画面の詳細を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-114">You can't change the details on this screen.</span></span> <span data-ttu-id="7ac2b-115">これは仕様であり、エラーではありません。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-115">This is by design and not an error.</span></span>

<span data-ttu-id="7ac2b-116">[ **同意** して **続行** ] を選択して続行します。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-116">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="7ac2b-117">IT 部門が **パートナーセンターへのサインアップ**を無効にしている場合。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-117">If the IT department has turned off **sign up for Partner Center**.</span></span>

<span data-ttu-id="7ac2b-118">このメッセージは、ウイルスに感染したユーザーが無効になっているか、Azure AD テナントでウイルスによるサインアップが無効になっていることが原因で表示されます。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-118">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="7ac2b-119">Azure AD アカウントの全体管理者は、次の PowerShell コマンドを実行して、必要な機能を有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-119">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="7ac2b-120">**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="7ac2b-120">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="7ac2b-121">詳細については、「[セルフサービスサインアップ](/azure/active-directory/users-groups-roles/directory-self-service-signup)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-121">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="7ac2b-122">パスワードを忘れた場合</span><span class="sxs-lookup"><span data-stu-id="7ac2b-122">You forgot your password</span></span>

<span data-ttu-id="7ac2b-123">パスワードを忘れた場合は、サインインページの [ **アカウントにアクセスできない場合]** リンクを選択します。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-123">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="7ac2b-124">このオプションを使用すると、パスワードをリセットしたり、グローバル管理者に新しい資格情報の割り当てを依頼したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-124">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-scree-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="7ac2b-125">「お客様の会社について教えてください」というエラーが発生すると、"問題が発生しました" というエラーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-125">On the “Tell us about your company” scree, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="7ac2b-126">このエラーメッセージは、通常、会社の電話番号で特殊文字、スペース、または国コードを使用している場合に表示されます。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-126">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="7ac2b-127">[電話番号] フィールドに入力する値には、最大で10文字まで含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-127">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="7ac2b-128">クレジットカードの購入で、"注文が拒否されました。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-128">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="7ac2b-129">情報を確認してください "</span><span class="sxs-lookup"><span data-stu-id="7ac2b-129">Please verify your information”</span></span>


<span data-ttu-id="7ac2b-130">法人ではなく、クレジットカードに対応する住所を常に使用してください。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-130">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="7ac2b-131">また、郵便番号が正しいことと、使用するアドレスに対応していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-131">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="7ac2b-132">オフライン支払いからオンライン支払方法に切り替える場合</span><span class="sxs-lookup"><span data-stu-id="7ac2b-132">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="7ac2b-133">優先支払い方法を使用して、元の注文と再購入を取り消す必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-133">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="7ac2b-134">注文を取り消すには:</span><span class="sxs-lookup"><span data-stu-id="7ac2b-134">To cancel an order:</span></span>

1. <span data-ttu-id="7ac2b-135">ダッシュボードの [ **メンバーシップの提供** ] タブを選択します。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-135">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="7ac2b-136">**取り消し順序**の選択</span><span class="sxs-lookup"><span data-stu-id="7ac2b-136">Select **Cancel order**</span></span>

3. <span data-ttu-id="7ac2b-137">確認ウィンドウが表示され、最初の順序を取り消すために確認を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ac2b-137">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7ac2b-138">次の手順</span><span class="sxs-lookup"><span data-stu-id="7ac2b-138">Next steps</span></span>

- [<span data-ttu-id="7ac2b-139">パートナー センター アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="7ac2b-139">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="7ac2b-140">請求書と偵察を読む方法</span><span class="sxs-lookup"><span data-stu-id="7ac2b-140">How to read your bill and recon file</span></span>](read-your-bill.md)