---
title: パートナーのセキュリティ要件を実装する
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ユーザーに必要なセキュリティ要件を実装する方法について説明します
author: LauraBrenner
ms.author: labrenne
keywords: セキュリティ
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: d162e8c5fd3cfd335920e4cc5fc826c3622f633c
ms.sourcegitcommit: 562535a4b16a8217c1e1945b7663ca3735e1ee27
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2020
ms.locfileid: "85133267"
---
# <a name="implement-the-partner-security-requirements"></a><span data-ttu-id="6d8e5-104">パートナーのセキュリティ要件を実装する</span><span class="sxs-lookup"><span data-stu-id="6d8e5-104">Implement the partner security requirements</span></span>

<span data-ttu-id="6d8e5-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="6d8e5-105">**Appropriate roles**</span></span>

- <span data-ttu-id="6d8e5-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="6d8e5-106">Global admin</span></span>

<span data-ttu-id="6d8e5-107">お客様とパートナーのセキュリティとプライバシーは、Microsoft の最優先事項です。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-107">Security and privacy of customers and partners are top priorities for Microsoft.</span></span> <span data-ttu-id="6d8e5-108">主に侵害 ID に関連する、ますます高度になったセキュリティ攻撃の数が増え続けています。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-108">We continue to see an increasing number of more sophisticated security attacks, primarily related to compromised identities.</span></span> <span data-ttu-id="6d8e5-109">予防的な制御は、セキュリティ攻撃を阻止するための全体的な防御戦略において重要な役割を果たすので、パートナーとその顧客を保護するために、一連の必須のセキュリティ要件の適用を開始します。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-109">As preventive controls play a key role in an overall defense strategy to thwart security attacks, we will start enforcing a set of mandatory security requirements to help protect partners and their customers.</span></span>

<span data-ttu-id="6d8e5-110">このチュートリアルでは、パートナーのセキュリティ要件、それらを満たす方法、およびパートナー ディレクトリにおけるユーザーへの影響について詳しく説明します。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-110">Through this tutorial you will learn more about the partner security requirements, how to fulfill them, and the impact to users in your partner directory.</span></span>

<span data-ttu-id="6d8e5-111">クラウド ソリューション プロバイダー プログラムに参加しているすべてのパートナー、コントロール パネル ベンダー、およびアドバイザー パートナーは、パートナー テナント内の各ユーザーに対して Multi-Factor Authentication (MFA) を適用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-111">All partners who are participating in the Cloud Solution Provider program, Control Panel Vendors, and Advisor partners are required to enforce Multi-Factor Authentication (MFA) for each user in their partner tenant.</span></span> <span data-ttu-id="6d8e5-112">この適用を行うには、2 つの [Azure Active Directory ベースライン ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)を有効にします。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-112">This enforcement can be done by enabling two [Azure Active Directory baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).</span></span> <span data-ttu-id="6d8e5-113">ベースライン ポリシーは、一般的な数々の攻撃から組織を保護するうえで役立つ定義済みポリシー セットです。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-113">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="6d8e5-114">これらの一般的な攻撃には、パスワードのスプレー、リプレイ、フィッシングなどがあります。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-114">These common attacks can include password spray, replay, and phishing.</span></span> <span data-ttu-id="6d8e5-115">ベースライン ポリシーは、Azure Active Directory のすべてのエディションで使用できます。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-115">Baseline policies are available in all editions of Azure Active Directory.</span></span> <span data-ttu-id="6d8e5-116">ID ベースの攻撃がここ数年にわたって増加しているため、Microsoft はこれらのベースライン保護ポリシーをすべてのユーザーが利用できるようにしています。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-116">Microsoft is making these baseline protection policies available to everyone because identity-based attacks have been on the rise over the last few years.</span></span>

<span data-ttu-id="6d8e5-117">次の手順では、2 つの必要なベースライン ポリシーを有効にするプロセスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-117">The procedures below describe the process of enabling the two necessary baseline policies:</span></span>

- <span data-ttu-id="6d8e5-118">**管理者に MFA を要求する**  "管理者に MFA を要求する" ポリシーを有効にした場合、管理者ロールのユーザーは、認証アプリを使用して MFA に登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-118">**Require MFA for admins**  Enabling the Require MFA for admins policy will require users in the administrator roles to register for MFA using the Authenticator App.</span></span> <span data-ttu-id="6d8e5-119">MFA の登録が完了したら、管理者はサインインするたびに MFA を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-119">Once MFA registration is complete, administrators will need to perform MFA every time they sign-in.</span></span>

- <span data-ttu-id="6d8e5-120">**エンド ユーザー保護**  "エンド ユーザー保護" は、ディレクトリ内のすべてのユーザーを保護する、リスクベースの MFA ベースライン ポリシーです。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-120">**End user protection**  End user protection is a risk-based MFA baseline policy that protects all users in a directory.</span></span> <span data-ttu-id="6d8e5-121">このポリシーを有効にすると、すべてのユーザーが認証アプリを使用して MFA に登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-121">Enabling this policy requires all users to register for MFA using the Authenticator App.</span></span> <span data-ttu-id="6d8e5-122">この MFA 登録プロンプトは 14 日間無視できますが、この期間を過ぎると、MFA に登録するまで、そのユーザーのサインインはブロックされます。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-122">Users can ignore the MFA registration prompt for 14 days, after which they will be blocked from signing in until they register for MFA.</span></span> <span data-ttu-id="6d8e5-123">MFA に登録されると、ユーザーは危険なサインインの試行中にのみ MFA が求められます。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-123">Once registered for MFA, users will be prompted for MFA only during risky sign-in attempts.</span></span> <span data-ttu-id="6d8e5-124">危害を受けたユーザー アカウントについては、パスワードをリセットし、リスク イベントを無視するまでブロックされます。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-124">Compromised user accounts are blocked until their password is reset and risk events have been dismissed.</span></span>

<span data-ttu-id="6d8e5-125">これらのポリシーを有効にすると、各ユーザーが Azure MFA を追加コストなしで利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-125">Once these policies are enabled, each user will be able to utilize Azure MFA at no additional cost.</span></span> <span data-ttu-id="6d8e5-126">サードパーティ ソリューションを使用している場合は、Microsoft の商用クラウド サービスにアクセスするときに、各ユーザーに MFA を適用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-126">If you are using a third-party solution, then you are required to enforce MFA for each user when accessing Microsoft Commercial cloud services.</span></span>

>[!NOTE]
><span data-ttu-id="6d8e5-127">MFA はパートナー ディレクトリ内のすべてのユーザーに適用されるため、ユーザーの資格情報を利用する自動化や統合に影響します。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-127">Since MFA will be enforced for every user in the partner directory, there will be an impact to any automation or integration that utilizes user credentials.</span></span> <span data-ttu-id="6d8e5-128">この影響に対処するには、自動化または統合が Microsoft の商用クラウド サービスに接続する方法を変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-128">To address this impact, you will need to modify the way your automation or integration connects to Microsoft commercial cloud services.</span></span> <span data-ttu-id="6d8e5-129">接続しているサービスでトークン ベースの認証がサポートされている場合は、[セキュリティで保護されたアプリケーション モデル フレームワーク](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)を実装することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-129">If the service you are connecting to supports token-based authentication, then it is recommended that you implement the [Secure Application Model framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).</span></span>

## <a name="step-one-block-any-existing-legacy-authentication-protocols"></a><span data-ttu-id="6d8e5-130">手順 1:既存のレガシ認証プロトコルをブロックする</span><span class="sxs-lookup"><span data-stu-id="6d8e5-130">Step one: Block any existing legacy authentication protocols</span></span>

<span data-ttu-id="6d8e5-131">"管理者に MFA を要求する" および "エンド ユーザー保護" ポリシーを有効にする前に、ユーザーがレガシ認証プロトコルを使用していないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-131">Before you enable the Require MFA for admins and End user protection policies, ensure that your users are not using legacy authentication protocols.</span></span> <span data-ttu-id="6d8e5-132">詳しくは、[方法:条件付きアクセスを使用した Azure AD に対する以前の認証のブロック](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use)に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-132">See the article [How to: Block legacy authentication to Azure AD with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use) for more information.</span></span>

## <a name="step-two-enable-the-require-mfa-for-admins-baseline-policy"></a><span data-ttu-id="6d8e5-133">手順 2:"管理者に MFA を要求する" ベースライン ポリシーを有効にする</span><span class="sxs-lookup"><span data-stu-id="6d8e5-133">Step two: Enable the Require MFA for admins baseline policy</span></span>

<span data-ttu-id="6d8e5-134">"管理者に MFA を要求する" ベースライン ポリシーでは、最も特権の高い Azure AD ロールと見なされる次のディレクトリ ロールに MFA が必要になります。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-134">The Require MFA for admin baseline policy requires MFA for the following directory roles, considered to be the most privileged Azure AD roles:</span></span>

- <span data-ttu-id="6d8e5-135">全体管理者</span><span class="sxs-lookup"><span data-stu-id="6d8e5-135">Global administrator</span></span>
- <span data-ttu-id="6d8e5-136">SharePoint 管理者</span><span class="sxs-lookup"><span data-stu-id="6d8e5-136">SharePoint administrator</span></span>
- <span data-ttu-id="6d8e5-137">Exchange 管理者</span><span class="sxs-lookup"><span data-stu-id="6d8e5-137">Exchange administrator</span></span>
- <span data-ttu-id="6d8e5-138">条件付きアクセス管理者</span><span class="sxs-lookup"><span data-stu-id="6d8e5-138">Conditional access administrator</span></span>
- <span data-ttu-id="6d8e5-139">セキュリティ管理者</span><span class="sxs-lookup"><span data-stu-id="6d8e5-139">Security administrator</span></span>
- <span data-ttu-id="6d8e5-140">ヘルプデスク管理者およびパスワード管理者</span><span class="sxs-lookup"><span data-stu-id="6d8e5-140">Helpdesk administrator/Password administrator</span></span>
- <span data-ttu-id="6d8e5-141">課金管理者</span><span class="sxs-lookup"><span data-stu-id="6d8e5-141">Billing administrator</span></span>
- <span data-ttu-id="6d8e5-142">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="6d8e5-142">User administrator</span></span>

<span data-ttu-id="6d8e5-143">"管理者に MFA を要求する" ポリシーを有効にするときに、上記の 9 つの管理者ロールは、認証アプリを使用して MFA に登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-143">Upon enabling the Require MFA for admins policy, the above nine administrator roles will be required to register for MFA using the Authenticator App.</span></span> <span data-ttu-id="6d8e5-144">MFA の登録が完了したら、管理者はサインインするたびに MFA を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-144">Once MFA registration is complete, administrators will need to perform MFA every single time they sign-in.</span></span>

<span data-ttu-id="6d8e5-145">ご自身の組織にこれらのアカウントがあり、スクリプトまたはコードで使用されている場合は、それを [マネージド ID](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview) に置き換えることを検討してください。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-145">If your organization has these accounts in use in scripts or code, consider replacing them with [managed identities](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).</span></span>

<span data-ttu-id="6d8e5-146">このポリシーを有効にして管理者を保護するには:</span><span class="sxs-lookup"><span data-stu-id="6d8e5-146">To enable this policy and protect your administrators:</span></span>

1. <span data-ttu-id="6d8e5-147">全体管理者、セキュリティ管理者、または条件付きアクセス管理者として  **Azure portal**  にサインインします。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-147">Sign in to the **Azure portal** as a Global Administrator, Security Administrator, or Conditional Access Administrator.</span></span>

2. <span data-ttu-id="6d8e5-148">**[Azure Active Directory]**  >  **[条件付きアクセス]** に移動します。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-148">Browse to **Azure Active Directory** > **Conditional Access**.</span></span>

3. <span data-ttu-id="6d8e5-149">ポリシーの一覧で、 **[ベースライン ポリシー: 管理者に MFA を要求する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-149">In the list of policies, select **Baseline policy: Require MFA for admins**.</span></span>

4. <span data-ttu-id="6d8e5-150">**[ポリシーを有効にする]** を **[ポリシーをすぐに有効にする]** に設定します。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-150">Set **Enable policy** to **Use policy immediately**.</span></span>

5. <span data-ttu-id="6d8e5-151"> *\*[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-151">Select **Save**.</span></span>

<span data-ttu-id="6d8e5-152">このポリシーを有効にすると、上記の管理者ロールのユーザーには、追加のセキュリティ情報を提供し、モバイル アプリを構成するように求めるプロンプトがサインイン時に表示されます。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-152">Once you’ve enabled this policy, users in the above administrator roles will be prompted on sign-in to provide additional security information and configure the mobile app.</span></span> <span data-ttu-id="6d8e5-153">これが完了すると、適切なクラウド サービスにサインインできるようになります。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-153">Once this is complete, they’ll be able to sign in to the appropriate cloud service.</span></span>

## <a name="step-three-enable-the-end-user-protection-baseline-policy"></a><span data-ttu-id="6d8e5-154">手順 3:"エンド ユーザー保護" ベースライン ポリシーを有効にする</span><span class="sxs-lookup"><span data-stu-id="6d8e5-154">Step three: Enable the End user protection baseline policy</span></span>

<span data-ttu-id="6d8e5-155">エンド ユーザー保護ベースライン ポリシーでは、ディレクトリ内のすべてのユーザーが保護されます。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-155">The End user protection baseline policy protects all users in a directory.</span></span> <span data-ttu-id="6d8e5-156">このポリシーを有効にすると、すべてのユーザーが 14 日以内に Azure MFA に登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-156">Enabling this policy requires all users to register for Azure MFA within 14 days.</span></span> <span data-ttu-id="6d8e5-157">登録が完了すると、ユーザーは、リスクの高いサインイン試行中にのみ MFA を要求されます。この動作は、今後パートナーのテナントに対して変更されます。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-157">Once registered, users will be prompted for MFA only during risky sign-in attempts, this behavior will change for partner tenants in the future.</span></span> <span data-ttu-id="6d8e5-158">危害を受けたユーザー アカウントについては、パスワードをリセットし、リスクを無視するまでブロックされます。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-158">Compromised user accounts are blocked until password reset and risk dismissal.</span></span>

<span data-ttu-id="6d8e5-159">ポリシー [ベースライン ポリシー:エンド ユーザー保護] は事前に構成されており、Azure portal で [条件付きアクセス] ブレードに移動すると上部に表示されます。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-159">The policy Baseline policy: End user protection comes pre-configured and will show up at the top when you navigate to the Conditional Access blade in Azure portal.</span></span>

<span data-ttu-id="6d8e5-160">このポリシーを有効にしてユーザーを保護するには:</span><span class="sxs-lookup"><span data-stu-id="6d8e5-160">To enable this policy and protect your users:</span></span>

1. <span data-ttu-id="6d8e5-161">全体管理者、セキュリティ管理者、または条件付きアクセス管理者として  **Azure portal**  にサインインします。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-161">Sign in to the **Azure portal** as a Global Administrator, Security Administrator, or Conditional Access Administrator.</span></span>

2. <span data-ttu-id="6d8e5-162">**[Azure Active Directory]**  >  **[条件付きアクセス]** に移動します。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-162">Browse to **Azure Active Directory** > **Conditional Access**.</span></span>

3. <span data-ttu-id="6d8e5-163">ポリシーの一覧で、 **[ベースライン ポリシー: エンド ユーザーの保護 (プレビュー)]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-163">In the list of policies, select **Baseline policy: End user protection (preview)**.</span></span>

4. <span data-ttu-id="6d8e5-164">**[ポリシーを有効にする]** を **[ポリシーをすぐに有効にする]** に設定します。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-164">Set **Enable policy** to **Use policy immediately**.</span></span>

5. <span data-ttu-id="6d8e5-165"> *\*[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-165">Select **Save**.</span></span>

<span data-ttu-id="6d8e5-166">このポリシーを有効にすると、すべてのユーザーに、追加のセキュリティ情報を提供し、モバイル アプリを構成するように求めるプロンプトがサインイン時に表示されます。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-166">Once you’ve enabled this policy, all users will be prompted on sign-in to provide additional security information and configure the mobile app.</span></span> <span data-ttu-id="6d8e5-167">これが完了すると、適切なクラウド サービスにサインインできるようになります。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-167">Once this is complete, they’ll be able to sign in to the appropriate cloud service.</span></span>

>[!NOTE]
><span data-ttu-id="6d8e5-168">パートナーのセキュリティ要件が適用されるまでは、"管理者に MFA を要求する" ベースライン ポリシーの対象になっていないユーザーには、リスクに基づく MFA のみが求められます。</span><span class="sxs-lookup"><span data-stu-id="6d8e5-168">Until the partner security requirements are enforced, users who are not covered by the Require MFA for admins baseline policy will only be prompted for MFA based on risk.</span></span>