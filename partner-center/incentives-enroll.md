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
ms.openlocfilehash: c4e24c22790edddef02e7936eaef9ed788489a37
ms.sourcegitcommit: 9f6be9bc8d9a065422d1ec8388bd770eb6cd9f33
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2021
ms.locfileid: "107528541"
---
# <a name="enrollment-and-user-management-in-the-incentives-program"></a><span data-ttu-id="2da77-104">インセンティブプログラムにおける登録とユーザー管理</span><span class="sxs-lookup"><span data-stu-id="2da77-104">Enrollment and user management in the incentives program</span></span>

<span data-ttu-id="2da77-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="2da77-105">**Appropriate roles**</span></span>

- <span data-ttu-id="2da77-106">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="2da77-106">Incentives admin</span></span>

>[!NOTE]
><span data-ttu-id="2da77-107">インセンティブプログラムに登録する前に、パートナーのメンバーシップセンターでパートナーセンターへの [移行](prepare-pmc-pc-migration.md)を完了している必要があります。</span><span class="sxs-lookup"><span data-stu-id="2da77-107">Before you can enroll in the incentives program you must have completed the Partner Membership Center to Partner Center [migration](prepare-pmc-pc-migration.md).</span></span>

<span data-ttu-id="2da77-108">登録プロセスは2つの手順で構成されます。</span><span class="sxs-lookup"><span data-stu-id="2da77-108">The enrollment process consists of two steps.</span></span>

<span data-ttu-id="2da77-109">**手順 1.ユーザー管理:** この手順では、パートナーセンターでインセンティブ管理者を確立します。</span><span class="sxs-lookup"><span data-stu-id="2da77-109">**Step 1. User management:** This step involves establishing the Incentive Administrator in Partner Center.</span></span>

<span data-ttu-id="2da77-110">**手順 2.登録: Microsoft は** 、インセンティブプログラムに登録するための招待を送信します。</span><span class="sxs-lookup"><span data-stu-id="2da77-110">**Step 2. Enrollment:** Microsoft sends you an invitation to enroll in your incentive program.</span></span>

## <a name="user-management"></a><span data-ttu-id="2da77-111">[ユーザー管理]</span><span class="sxs-lookup"><span data-stu-id="2da77-111">User Management</span></span>

<span data-ttu-id="2da77-112">パートナーセンターインセンティブプログラムに登録するには、グローバル管理者またはアカウント管理者が、会社のユーザーをインセンティブ管理者として設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2da77-112">To enroll in a Partner Center incentive program, the Global administrator or Account administrator needs to set up your company users as Incentive administrators.</span></span> <span data-ttu-id="2da77-113">パートナーアカウント、ロール、アクセス許可の詳細については、「 [パートナーセンターアカウントの管理](partner-center-account-setup.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2da77-113">For information on partner accounts, roles, and permissions, see [Manage your Partner Center account](partner-center-account-setup.md).</span></span> <span data-ttu-id="2da77-114">グローバル管理者は、Azure Active Directory (Azure AD) を使用して、会社のユーザーを設定することもできます。</span><span class="sxs-lookup"><span data-stu-id="2da77-114">The Global administrator can also set up your company users through the Azure Active Directory (Azure AD).</span></span>

>[!NOTE]
><span data-ttu-id="2da77-115">インセンティブプログラムに登録できるのは、インセンティブ管理者だけです。</span><span class="sxs-lookup"><span data-stu-id="2da77-115">Only the Incentive administrator can enroll in incentive programs.</span></span> <span data-ttu-id="2da77-116">お客様の場所にインセンティブ管理者がいない場合は、全体管理者とアカウント管理者が1つを割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="2da77-116">If there is no Incentive administrator for your location, the Global administrator and Account administrator must assign one.</span></span> <span data-ttu-id="2da77-117">MPN Id の場所にインセンティブ管理者が割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2da77-117">The Incentive administrator must be assigned for the location MPN IDs.</span></span> <span data-ttu-id="2da77-118">全体管理者またはアカウント管理者は、インセンティブ管理者として割り当てることもできます。</span><span class="sxs-lookup"><span data-stu-id="2da77-118">The Global administrator or Account administrator can also be assigned as the Incentive administrator.</span></span> <span data-ttu-id="2da77-119">さまざまなロールの詳細については、「 [インセンティブの管理](permissions-overview.md#manage-incentives)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2da77-119">To learn more about different roles, see [Manage incentives](permissions-overview.md#manage-incentives).</span></span>

## <a name="enrollment-process"></a><span data-ttu-id="2da77-120">登録プロセス</span><span class="sxs-lookup"><span data-stu-id="2da77-120">Enrollment Process</span></span>

<span data-ttu-id="2da77-121">組織がインセンティブに適合すると、Microsoft は、資格のある MPNLocationID のインセンティブ管理者に招待を送信して、登録プロセスを開始します。</span><span class="sxs-lookup"><span data-stu-id="2da77-121">Once your organization is eligible for incentives, Microsoft will send an invitation to the Incentive administrator of the eligible MPNLocationID to begin the enrollment process.</span></span> <span data-ttu-id="2da77-122">この電子メールは、 **Microsoft パートナーセンター** から送信され、 **パートナーインセンティブ登録招待** を受けます。</span><span class="sxs-lookup"><span data-stu-id="2da77-122">This email will be sent from **Microsoft Partner Center**, and will have the subject **Partner Incentive Enrollment Invitation**.</span></span> <span data-ttu-id="2da77-123">招待を開き、[ **開始**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="2da77-123">Open the invitation and select **Get Started**.</span></span>

<span data-ttu-id="2da77-124">パートナーセンターのホームページにも、招待が表示されます。</span><span class="sxs-lookup"><span data-stu-id="2da77-124">You’ll also see an invitation on the Partner Center home page.</span></span> <span data-ttu-id="2da77-125">このメッセージを選択すると、再度表示することはできません。</span><span class="sxs-lookup"><span data-stu-id="2da77-125">Once you select that message, you won’t be able to see it again.</span></span> <span data-ttu-id="2da77-126">ただし、インセンティブ管理者は、[パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインし、左側のナビゲーションの [**インセンティブ**] の下にある [**概要**] を選択して、プロセスを完了できます。</span><span class="sxs-lookup"><span data-stu-id="2da77-126">However, the Incentive Administrator can still complete the process by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) and selecting **Overview** under **Incentives** on the left nav.</span></span> <span data-ttu-id="2da77-127">[ **登録**] を選択し、プログラムの支払いと税金のプロファイルを完了します。</span><span class="sxs-lookup"><span data-stu-id="2da77-127">Select **Enroll**, and then complete the payout and tax profile for the program.</span></span>

<span data-ttu-id="2da77-128">MPN の場所に既定の銀行プロファイルが既に設定されていて、インセンティブプログラムに同じ MPN の場所を登録しようとしている場合は、[ **登録** ] を選択して招待を受け入れると、既定の銀行プロファイルが表示されます。</span><span class="sxs-lookup"><span data-stu-id="2da77-128">If you already have a default bank profile setup for an MPN location and you are trying to enroll for the same MPN location in an incentive program, when you select **Enroll** and accept the invitation, you will see the default bank profile.</span></span> <span data-ttu-id="2da77-129">また、MPN の場所用に作成した場合は、使用可能な税金プロファイルも表示されます。</span><span class="sxs-lookup"><span data-stu-id="2da77-129">You will also be shown any available tax profile if you've created it for that MPN location.</span></span> <span data-ttu-id="2da77-130">Microsoft が必要な銀行と税金のプロファイルの詳細をすべて持っている場合は、[ **送信** ] を選択して登録を完了するように求められます。</span><span class="sxs-lookup"><span data-stu-id="2da77-130">If Microsoft has all the required bank and tax profile detail, you'll be prompted to select **Submit** to complete the enrollment.</span></span> <span data-ttu-id="2da77-131">「 [既定の銀行プロファイルを設定する](incentives-create-and-manage-your-payout-and-tax-profiles.md#set-up-a-default-bank-profile)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2da77-131">See [Set up a default bank profile](incentives-create-and-manage-your-payout-and-tax-profiles.md#set-up-a-default-bank-profile).</span></span>

<span data-ttu-id="2da77-132">既定の銀行プロファイル以外の銀行プロファイルを選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="2da77-132">You also have the option to choose a bank profile other than the default bank profile.</span></span> <span data-ttu-id="2da77-133">マイクロソフトが支払いまたは税金のプロファイルまたは通貨に関する追加情報を必要とする場合は、 **続行** するように求められます。詳細については、[ **支払と税金のプロファイル** ] ページにリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="2da77-133">If Microsoft requires additional details for the payment or tax profiles or currency, you will be prompted to **Continue** and will be redirected to the **Payment and Tax profile** page to provide the missing details.</span></span> 

<span data-ttu-id="2da77-134">登録に対して指定した支払いと税金プロファイルが Microsoft によって検証された場合にのみ、登録が完了したと見なされます。</span><span class="sxs-lookup"><span data-stu-id="2da77-134">An enrollment is considered complete only when the payout and tax profile you provide for the enrollment is validated by Microsoft.</span></span>

<span data-ttu-id="2da77-135">特定のインセンティブプログラムは、すべてのパートナーに提供されています。</span><span class="sxs-lookup"><span data-stu-id="2da77-135">Certain incentive programs have no eligibility criteria, and are open to all partners.</span></span> <span data-ttu-id="2da77-136">インセンティブ管理者は、関連するインセンティブプログラムおよび MPN に対するアクセス許可を持っている場合、インセンティブの概要ページにこれらのプログラムの招待を表示します。</span><span class="sxs-lookup"><span data-stu-id="2da77-136">The Incentive administrator will see invitations for these programs on the incentive overview page, provided they have permissions for the relevant incentive program and MPN.</span></span> <span data-ttu-id="2da77-137">Microsoft は、これらのプログラムに対して電子メールの招待状を送信しません。</span><span class="sxs-lookup"><span data-stu-id="2da77-137">Microsoft does not send email invitations for these programs.</span></span>

<span data-ttu-id="2da77-138">登録プロセスの詳細については、 [インセンティブ登録ガイド](https://partner.microsoft.com/resources/detail/partner-center-incentives-enrollment-pdf) をダウンロードしてください (サインインが必要です)。</span><span class="sxs-lookup"><span data-stu-id="2da77-138">For more information on the enrollment process, download the [Incentives Enrollment Guide](https://partner.microsoft.com/resources/detail/partner-center-incentives-enrollment-pdf) (sign-in required).</span></span>

## <a name="expiration-and-renewal"></a><span data-ttu-id="2da77-139">有効期限と更新</span><span class="sxs-lookup"><span data-stu-id="2da77-139">Expiration and renewal</span></span>

<span data-ttu-id="2da77-140">インセンティブの登録は、会計年度の終了時に期限切れになります。</span><span class="sxs-lookup"><span data-stu-id="2da77-140">Incentives enrollment expires at the end of the fiscal year.</span></span> <span data-ttu-id="2da77-141">ただし、有効な契約を結んでいる資格のあるパートナーをお持ちであれば、Microsoft は、インセンティブ登録を次の会計年度にロールフォワードします。</span><span class="sxs-lookup"><span data-stu-id="2da77-141">However, as long as you remain an eligible partner with an active agreement, Microsoft will roll forward your incentives enrollment into the next fiscal year.</span></span> <span data-ttu-id="2da77-142">インセンティブプログラムのルールに従って、インセンティブプログラムに必要な支払いと税金情報が完成している限り、何らかの措置を講じる必要はありません。</span><span class="sxs-lookup"><span data-stu-id="2da77-142">You don't need to take any action, as long as the payout and tax information required for the incentive program is complete as per the rules of the incentive program.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2da77-143">次のステップ</span><span class="sxs-lookup"><span data-stu-id="2da77-143">Next steps</span></span>

- [<span data-ttu-id="2da77-144">プログラムの適格性を確認する</span><span class="sxs-lookup"><span data-stu-id="2da77-144">Determine your program eligibility</span></span>](incentives-determined-your-program-eligibility.md)
- [<span data-ttu-id="2da77-145">支払いと税金のプロファイルを作成して管理する</span><span class="sxs-lookup"><span data-stu-id="2da77-145">Create and manage your payout and tax profiles</span></span>](incentives-create-and-manage-your-payout-and-tax-profiles.md)
