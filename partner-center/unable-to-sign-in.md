---
title: サインインしてサインインできないパートナー センター
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 考えられる原因をトラブルシューティングし、パートナー センター にサインインできない場合の解決策について学習します。パスワードのリセット、ロールの確認、資格情報の確認の詳細を確認してください。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f4af8c48e2bbe65f58549b542447c80b699332be
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818798"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a><span data-ttu-id="c9e4a-103">サインインに関する問題のトラブルシューティングを行パートナー センター</span><span class="sxs-lookup"><span data-stu-id="c9e4a-103">Troubleshoot sign-in issues for Partner Center</span></span>

<span data-ttu-id="c9e4a-104">**適切なロール**: このロールに関心を持つパートナー センター</span><span class="sxs-lookup"><span data-stu-id="c9e4a-104">**Appropriate roles**: All partners interested in Partner Center</span></span>

<span data-ttu-id="c9e4a-105">この記事には、サインインに関する一般的なサインインに関する問題の解決策パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-105">This article contains solutions for common sign-in issues for Partner Center.</span></span>

## <a name="youve-forgotten-your-password-for-partner-center"></a><span data-ttu-id="c9e4a-106">パスワードを忘れた場合パートナー センター</span><span class="sxs-lookup"><span data-stu-id="c9e4a-106">You've forgotten your password for Partner Center</span></span>

<span data-ttu-id="c9e4a-107">パスワードを忘れてサインインできない場合は、サポートパートナー センター問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-107">If you have forgotten your password and can't sign into Partner Center, contact Support.</span></span> <span data-ttu-id="c9e4a-108">適切な連絡先については、「 [ビジネス製品のサポート」を参照してください](/microsoft-365/admin/contact-support-for-business-products)。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-108">Find the appropriate contact at [Support for Business Products](/microsoft-365/admin/contact-support-for-business-products).</span></span>

<span data-ttu-id="c9e4a-109">MPN パートナーの場合は、グローバル管理者に新しいパスワードの作成を求める。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-109">If you're an MPN partner, ask your Global admin to create a new password for you.</span></span> <span data-ttu-id="c9e4a-110">CSP 間接リセラーの場合は、間接プロバイダーに、Azure AD テナントで新しいグローバル管理者を作成するか、委任された管理者特権を使用して新しいパスワードを作成してください。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-110">If you're a CSP Indirect reseller, ask your Indirect provider to create a new Global admin for you on your Azure AD tenant or create a new password for you using their delegated admin privileges.</span></span>

<span data-ttu-id="c9e4a-111">パスワードをリセットし、仕事用アカウントへのアクセスを回復する方法の詳細については、「セキュリティ情報を使用して仕事または学校のパスワードをリセット [する」を参照してください](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-111">To learn more about how you can reset your password and regain access to your work account, read [Reset your work or school password using security info](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password).</span></span>

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a><span data-ttu-id="c9e4a-112">必要なページまたは機能を表示または管理パートナー センター</span><span class="sxs-lookup"><span data-stu-id="c9e4a-112">You can't view or manage the expected pages or capabilities in Partner Center</span></span>

<span data-ttu-id="c9e4a-113">ロール内のページパートナー センター、割り当てられているロールによって制御されます。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-113">Access to pages in Partner Center is controlled by the roles that you're assigned.</span></span> <span data-ttu-id="c9e4a-114">割り当てられているロールを確認するには、[設定] アイコンを選択パートナー センターアカウント設定]を選択し、[アカウント設定] で [ユーザー管理] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-114">To check which roles you're assigned, in Partner Center select the Settings icon, select **Account settings**, and then in Account settings, select **User management**.</span></span> <span data-ttu-id="c9e4a-115">[検索] に名前を入力し、結果を表示します。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-115">In Search, type your name and then view the results.</span></span>

<span data-ttu-id="c9e4a-116">コンピテンシー、顧客、インセンティブ、またはユーザーを表示または管理できない場合は、次のソリューションを試してください。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-116">If you aren't able to view or manage the competencies, customers, incentives, or users that you expect, try the following solutions:</span></span>

- <span data-ttu-id="c9e4a-117">MPN、CSP、紹介の機能にアクセスするには、グローバル管理者またはアカウント管理者にお問い合わせください。ロールと、ロールで有効にするタスクの詳細については、「パートナー センターにロールを割り当てる」& [を参照してください](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-117">For access to the capabilities of MPN, CSP, and Referrals, contact your Global admin or Account admin. To learn more about roles and the tasks they enable in Partner Center, see [Assign roles & permissions to users](permissions-overview.md).</span></span>
- <span data-ttu-id="c9e4a-118">商用マーケットプレースと Windows & Xbox、Office ストア、Microsoft Edge、およびハードウェア開発者プログラムの機能にアクセスするには、組織内の所有者または管理者の役割の担当者にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-118">For access to the capabilities of the Commercial Marketplace and the Windows & Xbox, Office Store, Microsoft Edge, and Hardware developer programs, contact the person in the Owner or Manager role in your organization.</span></span> <span data-ttu-id="c9e4a-119">ロールとアクセス許可の詳細については、「 [Microsoft パートナーセンターで商用 marketplace アカウントを管理する方法](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-119">To learn more about roles and permissions, see [How to manage a commercial marketplace account in Microsoft Partner Center](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions).</span></span>

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a><span data-ttu-id="c9e4a-120">パートナーセンターでプランや特典が表示されることはありません</span><span class="sxs-lookup"><span data-stu-id="c9e4a-120">You can’t see your offer or benefits in Partner Center</span></span>

<span data-ttu-id="c9e4a-121">サインインするための正しい資格情報を使用していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-121">Confirm that you are using the correct credentials to sign in.</span></span> <span data-ttu-id="c9e4a-122">たとえば、職場と個人のアカウントは同じように見える場合がありますが (など)、作成した個人アカウントを使用することができ abc@contoso.com ます。また、ユーザーに代わってビジネスアカウントを設定することもできます。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-122">For example, your work and personal accounts may look the same (such as abc@contoso.com), but one may be a personal account that you created and another may be a business account set up on your behalf.</span></span> <span data-ttu-id="c9e4a-123">この場合、サインインしていても、MPN、CSP、商用 Marketplace に関連する予想される機能を表示できない場合は、職場アカウントを選択してみてください。</span><span class="sxs-lookup"><span data-stu-id="c9e4a-123">In this case, if you are signed in, but are unable to view expected capabilities related to MPN, CSP, Commercial Marketplace, try selecting your work account.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c9e4a-124">次の手順</span><span class="sxs-lookup"><span data-stu-id="c9e4a-124">Next steps</span></span>

- [<span data-ttu-id="c9e4a-125">アカウント情報を確認する</span><span class="sxs-lookup"><span data-stu-id="c9e4a-125">Verify your account information</span></span>](verification-responses.md)
- [<span data-ttu-id="c9e4a-126">パスワードのリセット</span><span class="sxs-lookup"><span data-stu-id="c9e4a-126">Reset my password</span></span>](reset-my-pasword.md)
- [<span data-ttu-id="c9e4a-127">ユーザー パスワードのリセット</span><span class="sxs-lookup"><span data-stu-id="c9e4a-127">Reset a user password</span></span>](reset-a-user-password.md)