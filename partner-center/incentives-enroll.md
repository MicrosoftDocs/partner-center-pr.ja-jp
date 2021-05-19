---
title: インセンティブの登録
ms.topic: how-to
ms.date: 04/15/2021
description: インセンティブプログラムに登録し、ユーザー管理に必要なロールを割り当てます。 この記事では、登録プロセスについて説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: 670fae58a9a0e25127eb746f38063ea300d5ee2f
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152088"
---
# <a name="enrollment-and-user-management-in-the-incentives-program"></a><span data-ttu-id="165c3-104">インセンティブプログラムにおける登録とユーザー管理</span><span class="sxs-lookup"><span data-stu-id="165c3-104">Enrollment and user management in the incentives program</span></span>

<span data-ttu-id="165c3-105">**適切なロール**: インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="165c3-105">**Appropriate roles**: Incentives admin</span></span>

>[!NOTE]
><span data-ttu-id="165c3-106">インセンティブプログラムに登録する前に、パートナーのメンバーシップセンターでパートナーセンターへの [移行](prepare-pmc-pc-migration.md)を完了している必要があります。</span><span class="sxs-lookup"><span data-stu-id="165c3-106">Before you can enroll in the incentives program you must have completed the Partner Membership Center to Partner Center [migration](prepare-pmc-pc-migration.md).</span></span>

<span data-ttu-id="165c3-107">登録プロセスは2つの手順で構成されます。</span><span class="sxs-lookup"><span data-stu-id="165c3-107">The enrollment process consists of two steps.</span></span>

<span data-ttu-id="165c3-108">**手順 1.ユーザー管理:** この手順では、パートナーセンターでインセンティブ管理者を確立します。</span><span class="sxs-lookup"><span data-stu-id="165c3-108">**Step 1. User management:** This step involves establishing the Incentive Administrator in Partner Center.</span></span>

<span data-ttu-id="165c3-109">**手順 2.登録: Microsoft は** 、インセンティブプログラムに登録するための招待を送信します。</span><span class="sxs-lookup"><span data-stu-id="165c3-109">**Step 2. Enrollment:** Microsoft sends you an invitation to enroll in your incentive program.</span></span>

## <a name="user-management"></a><span data-ttu-id="165c3-110">[ユーザー管理]</span><span class="sxs-lookup"><span data-stu-id="165c3-110">User Management</span></span>

<span data-ttu-id="165c3-111">パートナーセンターインセンティブプログラムに登録するには、グローバル管理者またはアカウント管理者が、会社のユーザーをインセンティブ管理者として設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="165c3-111">To enroll in a Partner Center incentive program, the Global administrator or Account administrator needs to set up your company users as Incentive administrators.</span></span> <span data-ttu-id="165c3-112">パートナーアカウント、ロール、アクセス許可の詳細については、「 [パートナーセンターアカウントの管理](partner-center-account-setup.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="165c3-112">For information on partner accounts, roles, and permissions, see [Manage your Partner Center account](partner-center-account-setup.md).</span></span> <span data-ttu-id="165c3-113">グローバル管理者は、Azure Active Directory (Azure AD) を使用して、会社のユーザーを設定することもできます。</span><span class="sxs-lookup"><span data-stu-id="165c3-113">The Global administrator can also set up your company users through the Azure Active Directory (Azure AD).</span></span>

>[!NOTE]
><span data-ttu-id="165c3-114">インセンティブプログラムに登録できるのは、インセンティブ管理者だけです。</span><span class="sxs-lookup"><span data-stu-id="165c3-114">Only the Incentive administrator can enroll in incentive programs.</span></span> <span data-ttu-id="165c3-115">お客様の場所にインセンティブ管理者がいない場合は、全体管理者とアカウント管理者が1つを割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="165c3-115">If there is no Incentive administrator for your location, the Global administrator and Account administrator must assign one.</span></span> <span data-ttu-id="165c3-116">MPN Id の場所にインセンティブ管理者が割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="165c3-116">The Incentive administrator must be assigned for the location MPN IDs.</span></span> <span data-ttu-id="165c3-117">全体管理者またはアカウント管理者は、インセンティブ管理者として割り当てることもできます。</span><span class="sxs-lookup"><span data-stu-id="165c3-117">The Global administrator or Account administrator can also be assigned as the Incentive administrator.</span></span> <span data-ttu-id="165c3-118">さまざまなロールの詳細については、「 [インセンティブの管理](permissions-overview.md#manage-incentives)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="165c3-118">To learn more about different roles, see [Manage incentives](permissions-overview.md#manage-incentives).</span></span>

## <a name="enrollment-process"></a><span data-ttu-id="165c3-119">登録プロセス</span><span class="sxs-lookup"><span data-stu-id="165c3-119">Enrollment Process</span></span>

<span data-ttu-id="165c3-120">組織がインセンティブに適合すると、Microsoft は、資格のある MPNLocationID のインセンティブ管理者に招待を送信して、登録プロセスを開始します。</span><span class="sxs-lookup"><span data-stu-id="165c3-120">Once your organization is eligible for incentives, Microsoft will send an invitation to the Incentive administrator of the eligible MPNLocationID to begin the enrollment process.</span></span> <span data-ttu-id="165c3-121">この電子メールは、 **Microsoft パートナーセンター** から送信され、 **パートナーインセンティブ登録招待** を受けます。</span><span class="sxs-lookup"><span data-stu-id="165c3-121">This email will be sent from **Microsoft Partner Center**, and will have the subject **Partner Incentive Enrollment Invitation**.</span></span> <span data-ttu-id="165c3-122">招待を開き、[ ] を **選択開始する。**</span><span class="sxs-lookup"><span data-stu-id="165c3-122">Open the invitation and select **Get Started**.</span></span>

<span data-ttu-id="165c3-123">また、ホーム ページのパートナー センター表示されます。</span><span class="sxs-lookup"><span data-stu-id="165c3-123">You’ll also see an invitation on the Partner Center home page.</span></span> <span data-ttu-id="165c3-124">そのメッセージを選択すると、再び表示されません。</span><span class="sxs-lookup"><span data-stu-id="165c3-124">Once you select that message, you won’t be able to see it again.</span></span> <span data-ttu-id="165c3-125">ただし、インセンティブ管理者は引き続き、パートナー センター ダッシュボードにサインインし、左側のナビゲーションの[**インセンティブ**][で [](https://partner.microsoft.com/dashboard/)概要] を選択することで、プロセスを完了できます。</span><span class="sxs-lookup"><span data-stu-id="165c3-125">However, the Incentive Administrator can still complete the process by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) and selecting **Overview** under **Incentives** on the left nav.</span></span> <span data-ttu-id="165c3-126">[ **登録]** を選択し、プログラムの支払いプロファイルと税プロファイルを完了します。</span><span class="sxs-lookup"><span data-stu-id="165c3-126">Select **Enroll**, and then complete the payout and tax profile for the program.</span></span>

<span data-ttu-id="165c3-127">MPN の場所に対して既定の銀行プロファイルを既に設定し、インセンティブ プログラムで同じ MPN の場所に登録しようとしている場合は、[ 登録して招待に同意する] を選択すると、既定の銀行プロファイルが表示されます。</span><span class="sxs-lookup"><span data-stu-id="165c3-127">If you already have a default bank profile setup for an MPN location and you are trying to enroll for the same MPN location in an incentive program, when you select **Enroll** and accept the invitation, you will see the default bank profile.</span></span> <span data-ttu-id="165c3-128">また、MPN の場所用に作成した場合は、使用可能な税プロファイルも表示されます。</span><span class="sxs-lookup"><span data-stu-id="165c3-128">You will also be shown any available tax profile if you've created it for that MPN location.</span></span> <span data-ttu-id="165c3-129">Microsoft に必要なすべての銀行および税プロファイルの詳細がある場合は、[送信] を選択して登録を完了するように求めるメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="165c3-129">If Microsoft has all the required bank and tax profile detail, you'll be prompted to select **Submit** to complete the enrollment.</span></span> <span data-ttu-id="165c3-130">「 [既定の銀行プロファイルを設定する」を参照してください](incentives-create-and-manage-your-payout-and-tax-profiles.md#set-up-a-default-bank-profile)。</span><span class="sxs-lookup"><span data-stu-id="165c3-130">See [Set up a default bank profile](incentives-create-and-manage-your-payout-and-tax-profiles.md#set-up-a-default-bank-profile).</span></span>

<span data-ttu-id="165c3-131">また、既定の銀行プロファイル以外の銀行プロファイルを選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="165c3-131">You also have the option to choose a bank profile other than the default bank profile.</span></span> <span data-ttu-id="165c3-132">Microsoft が支払いプロファイルまたは税プロファイルまたは通貨に関する追加の詳細を必要とする場合は、続行を求めるメッセージが表示され、不足している詳細を指定するために [支払いおよび税金プロファイル] ページにリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="165c3-132">If Microsoft requires additional details for the payment or tax profiles or currency, you will be prompted to **Continue** and will be redirected to the **Payment and Tax profile** page to provide the missing details.</span></span> 

<span data-ttu-id="165c3-133">登録が完了したと見なされるのは、登録用に指定した支払いプロファイルと税プロファイルが Microsoft によって検証された場合のみです。</span><span class="sxs-lookup"><span data-stu-id="165c3-133">An enrollment is considered complete only when the payout and tax profile you provide for the enrollment is validated by Microsoft.</span></span>

<span data-ttu-id="165c3-134">特定のインセンティブ プログラムには適格性の基準が設定されていないので、すべてのパートナーが利用できます。</span><span class="sxs-lookup"><span data-stu-id="165c3-134">Certain incentive programs have no eligibility criteria, and are open to all partners.</span></span> <span data-ttu-id="165c3-135">インセンティブ管理者には、関連するインセンティブ プログラムと MPN のアクセス許可がある場合、インセンティブの概要ページにこれらのプログラムの招待が表示されます。</span><span class="sxs-lookup"><span data-stu-id="165c3-135">The Incentive administrator will see invitations for these programs on the incentive overview page, provided they have permissions for the relevant incentive program and MPN.</span></span> <span data-ttu-id="165c3-136">Microsoft は、これらのプログラムの招待を電子メールで送信しない。</span><span class="sxs-lookup"><span data-stu-id="165c3-136">Microsoft does not send email invitations for these programs.</span></span>

<span data-ttu-id="165c3-137">登録プロセスの詳細については、インセンティブ登録ガイド (サインインが [必要)](https://partner.microsoft.com/resources/detail/partner-center-incentives-enrollment-pdf) をダウンロードしてください。</span><span class="sxs-lookup"><span data-stu-id="165c3-137">For more information on the enrollment process, download the [Incentives Enrollment Guide](https://partner.microsoft.com/resources/detail/partner-center-incentives-enrollment-pdf) (sign-in required).</span></span>

## <a name="expiration-and-renewal"></a><span data-ttu-id="165c3-138">有効期限と更新</span><span class="sxs-lookup"><span data-stu-id="165c3-138">Expiration and renewal</span></span>

<span data-ttu-id="165c3-139">インセンティブの登録は、会計年度の終わりに期限切れになります。</span><span class="sxs-lookup"><span data-stu-id="165c3-139">Incentives enrollment expires at the end of the fiscal year.</span></span> <span data-ttu-id="165c3-140">ただし、有効な契約を結んでいる資格のあるパートナーをお持ちであれば、Microsoft は、インセンティブ登録を次の会計年度にロールフォワードします。</span><span class="sxs-lookup"><span data-stu-id="165c3-140">However, as long as you remain an eligible partner with an active agreement, Microsoft will roll forward your incentives enrollment into the next fiscal year.</span></span> <span data-ttu-id="165c3-141">インセンティブプログラムのルールに従って、インセンティブプログラムに必要な支払いと税金情報が完成している限り、何らかの措置を講じる必要はありません。</span><span class="sxs-lookup"><span data-stu-id="165c3-141">You don't need to take any action, as long as the payout and tax information required for the incentive program is complete as per the rules of the incentive program.</span></span>

## <a name="next-steps"></a><span data-ttu-id="165c3-142">次のステップ</span><span class="sxs-lookup"><span data-stu-id="165c3-142">Next steps</span></span>

- [<span data-ttu-id="165c3-143">プログラムの適格性を確認する</span><span class="sxs-lookup"><span data-stu-id="165c3-143">Determine your program eligibility</span></span>](incentives-determined-your-program-eligibility.md)
- [<span data-ttu-id="165c3-144">支払いと税金のプロファイルを作成して管理する</span><span class="sxs-lookup"><span data-stu-id="165c3-144">Create and manage your payout and tax profiles</span></span>](incentives-create-and-manage-your-payout-and-tax-profiles.md)
