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
ms.openlocfilehash: a5e8a292ad8593dc0b94179d5f0ee418344ef9af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854691"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="d085f-104">アカウントのセットアップまたは MPN 更新に関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="d085f-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="d085f-105">**適切なロール**: 全体管理者 |MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="d085f-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="d085f-106">ここでは、パートナーセンターアカウントを設定するときに発生する一般的な問題のトラブルシューティングに関するいくつかの推奨事項を示します。</span><span class="sxs-lookup"><span data-stu-id="d085f-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="d085f-107">パートナーメンバーシップセンターから移行するときに、会社情報フィールドを編集できない場合はどうなりますか</span><span class="sxs-lookup"><span data-stu-id="d085f-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="d085f-108">会社が既にパートナーセンター (CSP アカウントなど) に存在している場合は、読み取り専用画面が表示されます。</span><span class="sxs-lookup"><span data-stu-id="d085f-108">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="d085f-109">この画面には、パートナーセンターに存在する会社に関するすべての情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="d085f-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="d085f-110">この画面の詳細を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="d085f-110">You can't change the details on this screen.</span></span> <span data-ttu-id="d085f-111">これは仕様であり、エラーではありません。</span><span class="sxs-lookup"><span data-stu-id="d085f-111">This is by design and not an error.</span></span>

<span data-ttu-id="d085f-112">[ **同意** して **続行** ] を選択して続行します。</span><span class="sxs-lookup"><span data-stu-id="d085f-112">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="d085f-113">IT 部門が **パートナーセンターへのサインアップ** を無効にしている場合</span><span class="sxs-lookup"><span data-stu-id="d085f-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="d085f-114">このメッセージは、ウイルスに感染したユーザーが無効になっているか、Azure AD テナントでウイルスによるサインアップが無効になっていることが原因で表示されます。</span><span class="sxs-lookup"><span data-stu-id="d085f-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="d085f-115">Azure AD アカウントの全体管理者は、次の PowerShell コマンドを実行して、必要な機能を有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d085f-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="d085f-116">**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="d085f-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="d085f-117">詳細については、「 [セルフサービスサインアップ](/azure/active-directory/users-groups-roles/directory-self-service-signup)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d085f-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="d085f-118">パスワードを忘れた場合</span><span class="sxs-lookup"><span data-stu-id="d085f-118">You forgot your password</span></span>

<span data-ttu-id="d085f-119">パスワードを忘れた場合は、サインインページの [ **アカウントにアクセスできない場合]** リンクを選択します。</span><span class="sxs-lookup"><span data-stu-id="d085f-119">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="d085f-120">このオプションを使用すると、パスワードをリセットしたり、グローバル管理者に新しい資格情報の割り当てを依頼したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="d085f-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="d085f-121">[会社について教えて] 画面で、"問題が発生しました" というエラーが表示されます</span><span class="sxs-lookup"><span data-stu-id="d085f-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="d085f-122">このエラー メッセージは通常、会社の電話番号で特殊文字、スペース、または国番号を誤って使用した場合に表示されます。</span><span class="sxs-lookup"><span data-stu-id="d085f-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="d085f-123">[電話番号] フィールドに入力する値には、最大 10 文字しか含めることはできません。</span><span class="sxs-lookup"><span data-stu-id="d085f-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="d085f-124">クレジット カードの購入で、"Your order was declined. (注文が拒否されました。) というエラー メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="d085f-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="d085f-125">情報を確認してください"</span><span class="sxs-lookup"><span data-stu-id="d085f-125">Please verify your information”</span></span>


<span data-ttu-id="d085f-126">常に、法人ではなく、クレジット カードに対応する住所を使用してください。</span><span class="sxs-lookup"><span data-stu-id="d085f-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="d085f-127">また、郵便番号が正しく、使用するアドレスに対応していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="d085f-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="d085f-128">オフライン支払いからオンライン支払い方法に切り替える</span><span class="sxs-lookup"><span data-stu-id="d085f-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="d085f-129">元の注文を取り消し、優先支払い方法を使用して再取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d085f-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="d085f-130">注文を取り消す方法:</span><span class="sxs-lookup"><span data-stu-id="d085f-130">To cancel an order:</span></span>

1. <span data-ttu-id="d085f-131">ダッシュボードの **[メンバーシップ オファー]** タブを選択します。</span><span class="sxs-lookup"><span data-stu-id="d085f-131">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="d085f-132">[注文の **取り消し] を選択します**</span><span class="sxs-lookup"><span data-stu-id="d085f-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="d085f-133">確認ウィンドウが表示され、最初の注文をキャンセルするには確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d085f-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d085f-134">次の手順</span><span class="sxs-lookup"><span data-stu-id="d085f-134">Next steps</span></span>

- [<span data-ttu-id="d085f-135">パートナー センター アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="d085f-135">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="d085f-136">請求書と調整ファイルを読み取る方法</span><span class="sxs-lookup"><span data-stu-id="d085f-136">How to read your bill and recon file</span></span>](read-your-bill.md)
