---
title: パートナーセンターにサインインできません
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 考えられる原因のトラブルシューティングと、パートナーセンターにサインインできない場合の解決策については、パスワードのリセット、ロールの確認、および資格情報の確認に関するページを参照してください。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17087727afcaf3dbcf47801f8668388c370758e7
ms.sourcegitcommit: 9b04509f3830462628c1bb6af2ca41ed68b52619
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/09/2021
ms.locfileid: "107266573"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a><span data-ttu-id="a916c-103">パートナーセンターのサインインに関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="a916c-103">Troubleshoot sign-in issues for Partner Center</span></span>

<span data-ttu-id="a916c-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="a916c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a916c-105">パートナーセンターに関心のあるすべてのパートナー</span><span class="sxs-lookup"><span data-stu-id="a916c-105">All partners interested in Partner Center</span></span>

<span data-ttu-id="a916c-106">この記事には、パートナーセンターのサインインに関する一般的な問題の解決策が記載されています。</span><span class="sxs-lookup"><span data-stu-id="a916c-106">This article contains solutions for common sign-in issues for Partner Center.</span></span>

## <a name="youve-forgotten-your-password-for-partner-center"></a><span data-ttu-id="a916c-107">パートナーセンターのパスワードを忘れた</span><span class="sxs-lookup"><span data-stu-id="a916c-107">You've forgotten your password for Partner Center</span></span>

<span data-ttu-id="a916c-108">パスワードを忘れた場合、パートナーセンターにサインインできない場合は、サポートにお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="a916c-108">If you have forgotten your password and can't sign into Partner Center, contact Support.</span></span> <span data-ttu-id="a916c-109">適切な連絡先については、「 [ビジネス製品のサポート](/microsoft-365/admin/contact-support-for-business-products)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a916c-109">Find the appropriate contact at [Support for Business Products](/microsoft-365/admin/contact-support-for-business-products).</span></span>

<span data-ttu-id="a916c-110">MPN パートナーの方は、グローバル管理者に新しいパスワードの作成を依頼してください。</span><span class="sxs-lookup"><span data-stu-id="a916c-110">If you're an MPN partner, ask your Global admin to create a new password for you.</span></span> <span data-ttu-id="a916c-111">CSP 間接リセラーの場合は、Azure AD テナントに新しいグローバル管理者を作成するか、代理管理者権限を使用して新しいパスワードを作成するかを、間接プロバイダーに依頼してください。</span><span class="sxs-lookup"><span data-stu-id="a916c-111">If you're a CSP Indirect reseller, ask your Indirect provider to create a new Global admin for you on your Azure AD tenant or create a new password for you using their delegated admin privileges.</span></span>

<span data-ttu-id="a916c-112">パスワードをリセットし、職場アカウントへのアクセス権を回復する方法の詳細については、「 [セキュリティ情報を使用して職場または学校のパスワードをリセット](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a916c-112">To learn more about how you can reset your password and regain access to your work account, read [Reset your work or school password using security info](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password).</span></span>

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a><span data-ttu-id="a916c-113">パートナーセンターで予想されるページまたは機能を表示または管理できない</span><span class="sxs-lookup"><span data-stu-id="a916c-113">You can't view or manage the expected pages or capabilities in Partner Center</span></span>

<span data-ttu-id="a916c-114">パートナーセンターのページへのアクセスは、割り当てられているロールによって制御されます。</span><span class="sxs-lookup"><span data-stu-id="a916c-114">Access to pages in Partner Center is controlled by the roles that you're assigned.</span></span> <span data-ttu-id="a916c-115">割り当てられているロールを確認するには、パートナーセンターで設定アイコンを選択し、[ **アカウント設定**] を選択してから、[アカウント設定] で [ **ユーザー管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a916c-115">To check which roles you're assigned, in Partner Center select the Settings icon, select **Account settings**, and then in Account settings, select **User management**.</span></span> <span data-ttu-id="a916c-116">[検索] に名前を入力し、結果を表示します。</span><span class="sxs-lookup"><span data-stu-id="a916c-116">In Search, type your name and then view the results.</span></span>

<span data-ttu-id="a916c-117">期待されるコンピテンシー、顧客、インセンティブ、ユーザーを表示または管理できない場合は、次の解決策を試してください。</span><span class="sxs-lookup"><span data-stu-id="a916c-117">If you aren't able to view or manage the competencies, customers, incentives, or users that you expect, try the following solutions:</span></span>

- <span data-ttu-id="a916c-118">MPN、CSP、および紹介の機能にアクセスするには、全体管理者またはアカウント管理者に問い合わせてください。ロールと、パートナーセンターで有効になっているタスクの詳細については、「 [ユーザーにロール & アクセス許可を割り当てる](permissions-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a916c-118">For access to the capabilities of MPN, CSP, and Referrals, contact your Global admin or Account admin. To learn more about roles and the tasks they enable in Partner Center, see [Assign roles & permissions to users](permissions-overview.md).</span></span>
- <span data-ttu-id="a916c-119">商用マーケットプレースと Windows & Xbox、Office ストア、Microsoft Edge、およびハードウェア開発者プログラムの機能にアクセスするには、組織内の所有者または管理者の役割の担当者にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="a916c-119">For access to the capabilities of the Commercial Marketplace and the Windows & Xbox, Office Store, Microsoft Edge, and Hardware developer programs, contact the person in the Owner or Manager role in your organization.</span></span> <span data-ttu-id="a916c-120">ロールとアクセス許可の詳細については、「 [Microsoft パートナーセンターで商用 marketplace アカウントを管理する方法](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a916c-120">To learn more about roles and permissions, see [How to manage a commercial marketplace account in Microsoft Partner Center](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).</span></span>

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a><span data-ttu-id="a916c-121">パートナーセンターでプランや特典が表示されることはありません</span><span class="sxs-lookup"><span data-stu-id="a916c-121">You can’t see your offer or benefits in Partner Center</span></span>

<span data-ttu-id="a916c-122">サインインするための正しい資格情報を使用していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a916c-122">Confirm that you are using the correct credentials to sign in.</span></span> <span data-ttu-id="a916c-123">たとえば、職場と個人のアカウントは同じように見える場合がありますが (など)、作成した個人アカウントを使用することができ abc@contoso.com ます。また、ユーザーに代わってビジネスアカウントを設定することもできます。</span><span class="sxs-lookup"><span data-stu-id="a916c-123">For example, your work and personal accounts may look the same (such as abc@contoso.com), but one may be a personal account that you created and another may be a business account set up on your behalf.</span></span> <span data-ttu-id="a916c-124">この場合、サインインしていても、MPN、CSP、商用 Marketplace に関連する予想される機能を表示できない場合は、職場アカウントを選択してみてください。</span><span class="sxs-lookup"><span data-stu-id="a916c-124">In this case, if you are signed in, but are unable to view expected capabilities related to MPN, CSP, Commercial Marketplace, try selecting your work account.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a916c-125">次のステップ</span><span class="sxs-lookup"><span data-stu-id="a916c-125">Next steps</span></span>

- [<span data-ttu-id="a916c-126">アカウント情報を確認する</span><span class="sxs-lookup"><span data-stu-id="a916c-126">Verify your account information</span></span>](verification-responses.md)
- [<span data-ttu-id="a916c-127">パスワードのリセット</span><span class="sxs-lookup"><span data-stu-id="a916c-127">Reset my password</span></span>](reset-my-pasword.md)
- [<span data-ttu-id="a916c-128">ユーザー パスワードのリセット</span><span class="sxs-lookup"><span data-stu-id="a916c-128">Reset a user password</span></span>](reset-a-user-password.md)