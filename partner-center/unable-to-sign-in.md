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
ms.openlocfilehash: 2b67201355e748f9280d28413a8737a9b07db5c6
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431494"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a><span data-ttu-id="86258-103">パートナーセンターのサインインに関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="86258-103">Troubleshoot sign-in issues for Partner Center</span></span>

<span data-ttu-id="86258-104">**適切なロール**: パートナーセンターに関心のあるすべてのパートナー</span><span class="sxs-lookup"><span data-stu-id="86258-104">**Appropriate roles**: All partners interested in Partner Center</span></span>

<span data-ttu-id="86258-105">この記事には、パートナーセンターのサインインに関する一般的な問題の解決策が記載されています。</span><span class="sxs-lookup"><span data-stu-id="86258-105">This article contains solutions for common sign-in issues for Partner Center.</span></span>

## <a name="youve-forgotten-your-password-for-partner-center"></a><span data-ttu-id="86258-106">パートナーセンターのパスワードを忘れた</span><span class="sxs-lookup"><span data-stu-id="86258-106">You've forgotten your password for Partner Center</span></span>

<span data-ttu-id="86258-107">パスワードを忘れた場合、パートナーセンターにサインインできない場合は、サポートにお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="86258-107">If you have forgotten your password and can't sign into Partner Center, contact Support.</span></span> <span data-ttu-id="86258-108">適切な連絡先については、「 [ビジネス製品のサポート](/microsoft-365/admin/contact-support-for-business-products)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86258-108">Find the appropriate contact at [Support for Business Products](/microsoft-365/admin/contact-support-for-business-products).</span></span>

<span data-ttu-id="86258-109">Microsoft Partner Network (MPN) パートナーの方は、グローバル管理者に新しいパスワードの作成を依頼してください。</span><span class="sxs-lookup"><span data-stu-id="86258-109">If you're a Microsoft Partner Network (MPN) partner, ask your Global admin to create a new password for you.</span></span> <span data-ttu-id="86258-110">クラウドソリューションプロバイダー (CSP) の間接リセラーの場合は、Azure Active Directory (AD) テナントに新しいグローバル管理者を作成するか、委任された管理者特権を使用して新しいパスワードを作成するかを、間接プロバイダーに依頼してください。</span><span class="sxs-lookup"><span data-stu-id="86258-110">If you're a Cloud Solution Provider (CSP) Indirect reseller, ask your Indirect provider to create a new Global admin for you on your Azure Active Directory (AD) tenant or create a new password for you using their delegated admin privileges.</span></span>

<span data-ttu-id="86258-111">パスワードをリセットし、職場アカウントへのアクセス権を回復する方法の詳細については、「 [セキュリティ情報を使用して職場または学校のパスワードをリセット](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86258-111">To learn more about how you can reset your password and regain access to your work account, read [Reset your work or school password using security info](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password).</span></span>

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a><span data-ttu-id="86258-112">パートナーセンターで予想されるページまたは機能を表示または管理できない</span><span class="sxs-lookup"><span data-stu-id="86258-112">You can't view or manage the expected pages or capabilities in Partner Center</span></span>

<span data-ttu-id="86258-113">パートナーセンターのページへのアクセスは、割り当てられているロールによって制御されます。</span><span class="sxs-lookup"><span data-stu-id="86258-113">Access to pages in Partner Center is controlled by the roles that you're assigned.</span></span> <span data-ttu-id="86258-114">割り当てられているロールを確認するには、パートナーセンターで設定アイコンを選択し、[ **アカウント設定**] を選択してから、[アカウント設定] で [ **ユーザー管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="86258-114">To check which roles you're assigned, in Partner Center select the Settings icon, select **Account settings**, and then in Account settings, select **User management**.</span></span> <span data-ttu-id="86258-115">[検索] に名前を入力し、結果を表示します。</span><span class="sxs-lookup"><span data-stu-id="86258-115">In Search, type your name and then view the results.</span></span>

<span data-ttu-id="86258-116">期待されるコンピテンシー、顧客、インセンティブ、ユーザーを表示または管理できない場合は、次の解決策を試してください。</span><span class="sxs-lookup"><span data-stu-id="86258-116">If you aren't able to view or manage the competencies, customers, incentives, or users that you expect, try the following solutions:</span></span>

- <span data-ttu-id="86258-117">MPN、CSP、および紹介の機能にアクセスするには、全体管理者またはアカウント管理者に問い合わせてください。ロールと、パートナーセンターで有効になっているタスクの詳細については、「 [ユーザーにロール & アクセス許可を割り当てる](permissions-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86258-117">For access to the capabilities of MPN, CSP, and Referrals, contact your Global admin or Account admin. To learn more about roles and the tasks they enable in Partner Center, see [Assign roles & permissions to users](permissions-overview.md).</span></span>
- <span data-ttu-id="86258-118">商用マーケットプレースと Windows & Xbox、Office ストア、Microsoft Edge、およびハードウェア開発者プログラムの機能にアクセスするには、組織内の所有者または管理者の役割の担当者にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="86258-118">For access to the capabilities of the Commercial Marketplace and the Windows & Xbox, Office Store, Microsoft Edge, and Hardware developer programs, contact the person in the Owner or Manager role in your organization.</span></span> <span data-ttu-id="86258-119">ロールとアクセス許可の詳細については、「 [Microsoft パートナーセンターで商用 marketplace アカウントを管理する方法](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86258-119">To learn more about roles and permissions, see [How to manage a commercial marketplace account in Microsoft Partner Center](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).</span></span>

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a><span data-ttu-id="86258-120">パートナーセンターでプランや特典が表示されることはありません</span><span class="sxs-lookup"><span data-stu-id="86258-120">You can’t see your offer or benefits in Partner Center</span></span>

<span data-ttu-id="86258-121">サインインするための正しい資格情報を使用していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="86258-121">Confirm that you are using the correct credentials to sign in.</span></span> <span data-ttu-id="86258-122">たとえば、職場と個人のアカウントは同じように見える場合がありますが (など)、作成した個人アカウントを使用することができ abc@contoso.com ます。また、ユーザーに代わってビジネスアカウントを設定することもできます。</span><span class="sxs-lookup"><span data-stu-id="86258-122">For example, your work and personal accounts may look the same (such as abc@contoso.com), but one may be a personal account that you created and another may be a business account set up on your behalf.</span></span> <span data-ttu-id="86258-123">この場合、サインインしていても、MPN、CSP、商用 Marketplace に関連する予想される機能を表示できない場合は、職場アカウントを選択してみてください。</span><span class="sxs-lookup"><span data-stu-id="86258-123">In this case, if you are signed in, but are unable to view expected capabilities related to MPN, CSP, Commercial Marketplace, try selecting your work account.</span></span>

## <a name="next-steps"></a><span data-ttu-id="86258-124">次の手順</span><span class="sxs-lookup"><span data-stu-id="86258-124">Next steps</span></span>

- [<span data-ttu-id="86258-125">アカウント情報を確認する</span><span class="sxs-lookup"><span data-stu-id="86258-125">Verify your account information</span></span>](verification-responses.md)
- [<span data-ttu-id="86258-126">パスワードのリセット</span><span class="sxs-lookup"><span data-stu-id="86258-126">Reset my password</span></span>](reset-my-pasword.md)
- [<span data-ttu-id="86258-127">ユーザー パスワードのリセット</span><span class="sxs-lookup"><span data-stu-id="86258-127">Reset a user password</span></span>](reset-a-user-password.md)