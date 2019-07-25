---
title: パートナーのセキュリティ要件に関する FAQ |パートナーセンター
ms.topic: article
ms.date: 07/18/2019
description: パートナーのセキュリティ要件についてよく寄せられる質問
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, クラウドソリューションプロバイダー, Cloud Solution Provider プログラム, CSP, コントロールパネルベンダ, CPV, multi-factor authentication, MFA, 安全なアプリケーションモデル, セキュリティで保護されたアプリモデル, セキュリティ
ms.localizationpriority: medium
ms.openlocfilehash: 1a178dc71f8042e6b39a316c6c889b619aaed12c
ms.sourcegitcommit: 5c8ac1b6d29d183d85582d6eb32e37b91dd8c6c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2019
ms.locfileid: "68315551"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a><span data-ttu-id="90d25-104">パートナーのセキュリティ要件についてよく寄せられる質問</span><span class="sxs-lookup"><span data-stu-id="90d25-104">Frequently asked questions about the partner security requirements</span></span>

<span data-ttu-id="90d25-105">この記事では、[パートナーのセキュリティ要件](partner-security-requirements.md)に関してよく寄せられる質問をいくつか紹介します。</span><span class="sxs-lookup"><span data-stu-id="90d25-105">This article contains some frequently asked questions for the [partner security requirements](partner-security-requirements.md).</span></span> <span data-ttu-id="90d25-106">よく寄せられる質問の一覧については、[こちら](http://assetsprod.microsoft.com/security-requirements-faq.pdf)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90d25-106">You can find a comprehensive list of frequently asked questions [here](http://assetsprod.microsoft.com/security-requirements-faq.pdf).</span></span>

## <a name="conditional-access"></a><span data-ttu-id="90d25-107">条件付きアクセス</span><span class="sxs-lookup"><span data-stu-id="90d25-107">Conditional Access</span></span>

### <a name="can-conditional-access-be-used"></a><span data-ttu-id="90d25-108">条件付きアクセスを使用できますか?</span><span class="sxs-lookup"><span data-stu-id="90d25-108">Can conditional access be used?</span></span>

<span data-ttu-id="90d25-109">はい。条件付きアクセスを使用して、パートナーテナントの各ユーザー (サービスアカウントを含む) に MFA を適用できます。</span><span class="sxs-lookup"><span data-stu-id="90d25-109">Yes, you can use conditional access to enforce MFA for each user, including service accounts, in your partner tenant.</span></span> <span data-ttu-id="90d25-110">ただし、パートナーになるという高度な特権がある場合は、各ユーザーが単一の認証ごとに MFA チャレンジを使用できるようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="90d25-110">However, given the highly privileged nature of being a partner we need to ensure that each user has an MFA challenge for every single authentication.</span></span> <span data-ttu-id="90d25-111">これは、MFA の要件を回避する条件付きアクセスの機能を利用できないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="90d25-111">This means you will not be able to leverage feature of conditional access that circumvent the requirement for MFA.</span></span>

## <a name="multi-factor-authentication"></a><span data-ttu-id="90d25-112">多要素認証</span><span class="sxs-lookup"><span data-stu-id="90d25-112">Multi-Factor Authentication</span></span>

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a><span data-ttu-id="90d25-113">お客様はパートナーのセキュリティ要件の対象ですか?</span><span class="sxs-lookup"><span data-stu-id="90d25-113">Are my customers subject to the partner security requirements?</span></span>

<span data-ttu-id="90d25-114">いいえ。お客様の Azure AD テナントの各ユーザーに対して MFA を強制する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="90d25-114">No, it is not required that you enforce MFA for each user in your customer's Azure AD tenants.</span></span> <span data-ttu-id="90d25-115">ただし、各顧客を操作して、ユーザーの保護に最適な方法を決定することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="90d25-115">However, it is recommended that you work with each customer to determine how best to protect their users.</span></span>

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a><span data-ttu-id="90d25-116">アプリパスワードは、ベースライン保護ポリシーと共に使用できますか。</span><span class="sxs-lookup"><span data-stu-id="90d25-116">Can app passwords be used with the baseline protection policies?</span></span>

<span data-ttu-id="90d25-117">はい。[アプリパスワード](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="90d25-117">Yes, [app passwords](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) can be used.</span></span> <span data-ttu-id="90d25-118">[ここ](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)に記載されているアプリパスワードを使用する際の考慮事項を確認し、ニーズに応じてサポートされているかどうかを判断する必要があります。</span><span class="sxs-lookup"><span data-stu-id="90d25-118">You should review the considerations for using app passwords documented [here](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) to determine if they are supported for your need.</span></span>

### <a name="can-any-user-be-excluded-from-this-requirement"></a><span data-ttu-id="90d25-119">どのユーザーでもこの要件を除外することはできますか。</span><span class="sxs-lookup"><span data-stu-id="90d25-119">Can any user be excluded from this requirement?</span></span> 

<span data-ttu-id="90d25-120">いいえ。パートナーテナントの各ユーザー (サービスアカウントを含む) は、MFA を使用した認証を要求されます。</span><span class="sxs-lookup"><span data-stu-id="90d25-120">No, each user, including service accounts, in your partner tenant will be required to authenticate using MFA.</span></span>

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a><span data-ttu-id="90d25-121">パートナーのセキュリティ要件は統合サンドボックスに適用されますか。</span><span class="sxs-lookup"><span data-stu-id="90d25-121">Do the partner security requirements apply to the integration sandbox?</span></span>

<span data-ttu-id="90d25-122">はい、パートナーのセキュリティ要件は統合サンドボックスに適用されます。</span><span class="sxs-lookup"><span data-stu-id="90d25-122">Yes, the partner security requirements apply to the integration sandbox.</span></span> <span data-ttu-id="90d25-123">これは、統合サンドボックステナントのユーザーに適切な MFA ソリューションを実装する必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="90d25-123">This means you will need to implement the appropriate MFA solution for users in the integration sandbox tenant.</span></span> <span data-ttu-id="90d25-124">MFA を提供するには、ベースライン保護ポリシーを実装することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="90d25-124">It is recommended that you implement the baseline protection policies to provide MFA.</span></span>

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a><span data-ttu-id="90d25-125">緊急アクセス (休憩) アカウントを構成操作方法には</span><span class="sxs-lookup"><span data-stu-id="90d25-125">How do I configure an emergency access (break glass) account?</span></span>

<span data-ttu-id="90d25-126">Azure AD テナントから誤ってロックアウトされるのを防ぐために、1つまたは2つの緊急アクセスアカウントを作成することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="90d25-126">It considered best practice to create one or two emergency access accounts to prevent being inadvertently locked out of your Azure AD tenant.</span></span> <span data-ttu-id="90d25-127">パートナーのセキュリティ要件に関しては、各ユーザーが MFA を使用して認証する必要があります。</span><span class="sxs-lookup"><span data-stu-id="90d25-127">With respect to the partner security requirements, it is required that each user authenticate using MFA.</span></span> <span data-ttu-id="90d25-128">したがって、これは緊急アクセスアカウントの定義を変更する必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="90d25-128">So, this means you will need to modify the definition of an emergency access account.</span></span> <span data-ttu-id="90d25-129">MFA のためのサードパーティソリューションを利用しているアカウントを使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="90d25-129">It could be an account that is leveraging a third-party solution for MFA.</span></span>

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a><span data-ttu-id="90d25-130">ゲストユーザーは、パートナーのセキュリティ要件によってどのような影響を受けますか。</span><span class="sxs-lookup"><span data-stu-id="90d25-130">How will guest users be impacted by the partner security requirements?</span></span>

<span data-ttu-id="90d25-131">パートナーテナント内のリソースにアクセスするときは、ゲストユーザーが MFA を使用して認証する必要があります。</span><span class="sxs-lookup"><span data-stu-id="90d25-131">Guest users will be required to authenticate using MFA, when accessing resources in your partner tenant.</span></span> <span data-ttu-id="90d25-132">パートナーのセキュリティ要件は、ゲストユーザーが独自のテナントのリソースにアクセスすることには影響しません。</span><span class="sxs-lookup"><span data-stu-id="90d25-132">The partner security requirements will have no impact on the guest user will accessing resources in their own tenant.</span></span>

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a><span data-ttu-id="90d25-133">サードパーティのソリューションを使用している場合は Active Directory フェデレーションサービス (ADFS) が必要ですか?</span><span class="sxs-lookup"><span data-stu-id="90d25-133">If I am using a third-party solution is Active Directory Federation Service (ADFS) required?</span></span> 

<span data-ttu-id="90d25-134">いいえ、サードパーティのソリューションを使用している場合は、Active Directory フェデレーションサービス (ADFS) を用意する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="90d25-134">No, it is not required to have Active Directory Federation Service (ADFS) if you are using a third-party solution.</span></span> <span data-ttu-id="90d25-135">ソリューションのベンダーと協力して、ソリューションの要件を決定することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="90d25-135">It is recommended that you work with the vendor of the solution determine what the requirements for their solution are.</span></span>

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a><span data-ttu-id="90d25-136">ベースライン保護ポリシーを有効にする必要がありますか。</span><span class="sxs-lookup"><span data-stu-id="90d25-136">Is it a requirement to enable the baseline protection policies?</span></span>

<span data-ttu-id="90d25-137">いいえ。ベースライン保護ポリシーを有効にする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="90d25-137">No, it is not required that you enable the baseline protection policies.</span></span> <span data-ttu-id="90d25-138">唯一の要件は、パートナーテナント内のユーザー (サービスアカウントを含む) ごとに MFA を適用することです。</span><span class="sxs-lookup"><span data-stu-id="90d25-138">The only requirement is that you enforce MFA for each user, including service accounts, in your partner tenant.</span></span>

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a><span data-ttu-id="90d25-139">ベースライン保護ポリシーの実装により、どのような検証オプションが提供されますか。</span><span class="sxs-lookup"><span data-stu-id="90d25-139">What verification options are provided through the implementation of the baseline protection policies?</span></span> 

<span data-ttu-id="90d25-140">ベースライン保護ポリシーの実装によって利用可能な MFA のバージョンに関して、使用可能な認証オプションは authenticator アプリだけです。</span><span class="sxs-lookup"><span data-stu-id="90d25-140">With respect to the version of MFA that is available through the implementation of the baseline protection polices, the only verification option available is an authenticator app.</span></span> <span data-ttu-id="90d25-141">通話とテキストメッセージメッセージの使用は、安全性が低いと見なされます。</span><span class="sxs-lookup"><span data-stu-id="90d25-141">The use of a phone call and text message message is considered less secure.</span></span> <span data-ttu-id="90d25-142">そのため、これらのオプションは、このバージョンの MFA では使用できません。</span><span class="sxs-lookup"><span data-stu-id="90d25-142">So, these options are not available through this version of MFA.</span></span>

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a><span data-ttu-id="90d25-143">Azure AD Connect によって使用されるサービスアカウントは、パートナーのセキュリティ要件の影響を受けますか。</span><span class="sxs-lookup"><span data-stu-id="90d25-143">Will the service account used by Azure AD Connect be impacted by the partner security requirements?</span></span>

<span data-ttu-id="90d25-144">いいえ。 Azure AD Connect によって使用されるサービスアカウントは、パートナーのセキュリティ要件による影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="90d25-144">No, the service account used by Azure AD Connect will not be impacted by the partner security requirements.</span></span> <span data-ttu-id="90d25-145">MFA を適用した結果として Azure AD Connect の問題が発生した場合は、Microsoft サポートに問い合わせてテクニカルサポートを依頼してください。</span><span class="sxs-lookup"><span data-stu-id="90d25-145">If you experience an issue with Azure AD Connect as result of enforcing MFA, then open a technical support request with Microsoft support.</span></span>
