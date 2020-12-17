---
title: 多要素認証を使用してユーザーを設定する
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 従業員に MFA を設定する方法について説明します
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 355258fd20f867052fa8598e688630005262bb16
ms.sourcegitcommit: ab2ca3c5990b7f920df4ecb9c611d5b1046ec111
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/16/2020
ms.locfileid: "97578289"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="3485f-103">多要素認証を使用してユーザーを設定する</span><span class="sxs-lookup"><span data-stu-id="3485f-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="3485f-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="3485f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="3485f-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="3485f-105">Global admin</span></span>

<span data-ttu-id="3485f-106">プライバシーの保護とセキュリティの強化は、マイクロソフトの最優先事項の 1 つです。</span><span class="sxs-lookup"><span data-stu-id="3485f-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="3485f-107">最善の防御とは予防することで、私たちの強さが、最も弱いリンクと同程度でしかないことはわかっています。</span><span class="sxs-lookup"><span data-stu-id="3485f-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="3485f-108">そのために、エコシステムの全員が行動し、適切なセキュリティ保護を確保する必要があるのです。</span><span class="sxs-lookup"><span data-stu-id="3485f-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="3485f-109">すべてのパートナーが、パートナー テナント内のユーザーに対して多要素認証 (MFA) を有効にすることを強くお勧めします。</span><span class="sxs-lookup"><span data-stu-id="3485f-109">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="3485f-110">ユーザーに多要素認証を追加する</span><span class="sxs-lookup"><span data-stu-id="3485f-110">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="3485f-111">このタスクを完了するには、会社のグローバル管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="3485f-111">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="3485f-112">ユーザーを Azure AD テナントに追加する時点で MFA を有効にするのが最も簡単です。</span><span class="sxs-lookup"><span data-stu-id="3485f-112">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="3485f-113">[Azure portal](https://portal.azure.com) にサインインし、 **[ユーザー管理]** にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="3485f-113">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="3485f-114">**[多要素認証]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3485f-114">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="3485f-115">有効にするユーザーを選択し、 **[有効]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3485f-115">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="3485f-116">これで、このユーザーに対して MFA が有効になります。</span><span class="sxs-lookup"><span data-stu-id="3485f-116">This will enable MFA for this user.</span></span> <span data-ttu-id="3485f-117">有効にすると、そのユーザーが初めてサインインするときに MFA 検証をセットアップするように求められます。</span><span class="sxs-lookup"><span data-stu-id="3485f-117">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="3485f-118">その後のサインインでは、メールかテキスト メッセージのいずれか設定した方で届いたコードを入力するよう求められます。</span><span class="sxs-lookup"><span data-stu-id="3485f-118">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="検証する方法を指定する":::

>[!NOTE]
><span data-ttu-id="3485f-120">ユーザーが MFA を使用することを **強制** するには、上記と同じ手順を使用して **[強制]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3485f-120">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="3485f-121">詳細については、「[ユーザーごとの Azure Multi-Factor Authentication を有効にしてサインイン イベントのセキュリティを確保する](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3485f-121">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="3485f-122">どのユーザーも最初は  **[無効]** です。</span><span class="sxs-lookup"><span data-stu-id="3485f-122">All users start out **Disabled**.</span></span> <span data-ttu-id="3485f-123">ユーザーごとに Azure Multi-Factor Authentication に登録すると、そのユーザーの状態が  **[有効]** に変わります。</span><span class="sxs-lookup"><span data-stu-id="3485f-123">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="3485f-124">有効にされたユーザーがサインインして登録プロセスを完了すると、その状態は  **[強制]** に変わります。</span><span class="sxs-lookup"><span data-stu-id="3485f-124">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="3485f-125">次のステップ</span><span class="sxs-lookup"><span data-stu-id="3485f-125">Next steps</span></span>

- [<span data-ttu-id="3485f-126">ユーザーにロールとアクセス許可を割り当てる</span><span class="sxs-lookup"><span data-stu-id="3485f-126">Assign roles and permissions to users</span></span>](permissions-overview.md)

