---
title: インセンティブプログラムに登録する
ms.topic: how-to
ms.date: 08/13/2020
description: インセンティブプログラムに登録し、ユーザー管理に必要なロールを割り当てます。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: eae4baa3cfd49692c6b672c45ec30c8384449975
ms.sourcegitcommit: 9d3f88f7008a2771b02cb4af860c6ca00eb50e42
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/17/2020
ms.locfileid: "88427007"
---
# <a name="enroll-in-the-incentives-program"></a><span data-ttu-id="8837d-103">インセンティブプログラムに登録する</span><span class="sxs-lookup"><span data-stu-id="8837d-103">Enroll in the incentives program</span></span>

<span data-ttu-id="8837d-104">適用対象:</span><span class="sxs-lookup"><span data-stu-id="8837d-104">Applies to:</span></span>

- <span data-ttu-id="8837d-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="8837d-105">Partner Center</span></span>

>[!NOTE]
><span data-ttu-id="8837d-106">インセンティブプログラムに登録する前に、パートナーのメンバーシップセンターでパートナーセンターへの [移行](prepare-pmc-pc-migration.md)を完了している必要があります。</span><span class="sxs-lookup"><span data-stu-id="8837d-106">Before you can enroll in the incentives program you must have completed the Partner Membership Center to Partner Center [migration](prepare-pmc-pc-migration.md).</span></span>

<span data-ttu-id="8837d-107">登録プロセスは2つの手順で構成されます。</span><span class="sxs-lookup"><span data-stu-id="8837d-107">The enrollment process consists of two steps.</span></span>

<span data-ttu-id="8837d-108">**手順 1.ユーザー管理:** この手順では、インセンティブ管理者とユーザーのアクセス許可を設定します。</span><span class="sxs-lookup"><span data-stu-id="8837d-108">**Step 1. User management:** This step involves establishing the Incentive Administrator and user permissions.</span></span>

<span data-ttu-id="8837d-109">**手順 2.登録: Microsoft は** 、インセンティブプログラムに登録するための招待を送信します。</span><span class="sxs-lookup"><span data-stu-id="8837d-109">**Step 2. Enrollment:** Microsoft sends you an invitation to enroll in your incentive program.</span></span>

## <a name="user-management"></a><span data-ttu-id="8837d-110">[ユーザー管理]</span><span class="sxs-lookup"><span data-stu-id="8837d-110">User Management</span></span>

<span data-ttu-id="8837d-111">インセンティブプログラムに登録するには、グローバル管理者またはアカウント管理者が会社のユーザーを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8837d-111">To enroll in an incentive program, the Global Administrator or Account Administrator needs to set up your company users.</span></span> <span data-ttu-id="8837d-112">インセンティブ管理者を割り当て、インセンティブユーザーのアクセス許可を付与する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8837d-112">They must assign an Incentive Administrator(s) and grant Incentive User permissions.</span></span> <span data-ttu-id="8837d-113">パートナーアカウント、ロール、アクセス許可の詳細については、「 [パートナーセンターアカウントの管理](partner-center-account-setup.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8837d-113">For information on partner accounts, roles, and permissions, see [Manage your Partner Center account](partner-center-account-setup.md).</span></span> <span data-ttu-id="8837d-114">グローバル管理者は、Azure Active Directory (AAD) を使用して会社のユーザーを設定することもできます。</span><span class="sxs-lookup"><span data-stu-id="8837d-114">The Global Administrator can also set up your company users through the Azure Active Directory (AAD).</span></span>

<span data-ttu-id="8837d-115">組織がインセンティブの対象となると、Microsoft はグローバル管理者、アカウント管理者、インセンティブ管理者に招待を送信します。</span><span class="sxs-lookup"><span data-stu-id="8837d-115">Once your organization is eligible for incentives, Microsoft will send invitations to the Global Administrator, Account Administrator, and Incentive Administrator.</span></span>

>[!NOTE]
><span data-ttu-id="8837d-116">インセンティブプログラムに登録できるのは、インセンティブ管理者だけです。</span><span class="sxs-lookup"><span data-stu-id="8837d-116">Only the Incentive Administrator can enroll in incentive programs.</span></span> <span data-ttu-id="8837d-117">お客様の場所にインセンティブ管理者がいない場合は、全体管理者とアカウント管理者が1つを割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="8837d-117">If there is no Incentive Administrator for your location, the Global Administrator and Account Administrator must assign one.</span></span> <span data-ttu-id="8837d-118">MPN Id の場所にインセンティブ管理者が割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8837d-118">The Incentive Administrator must be assigned for the location MPN IDs.</span></span> <span data-ttu-id="8837d-119">全体管理者またはアカウント管理者は、インセンティブ管理者として割り当てることもできます。</span><span class="sxs-lookup"><span data-stu-id="8837d-119">The Global Administrator or Account Administrator can also be assigned as the Incentive Administrator.</span></span>

## <a name="enrollment-process"></a><span data-ttu-id="8837d-120">登録プロセス</span><span class="sxs-lookup"><span data-stu-id="8837d-120">Enrollment Process</span></span>

<span data-ttu-id="8837d-121">組織がインセンティブの対象となると、Microsoft は、対象となる MPNLocationID の MPN 管理者に招待を送信してプロセスを開始します。</span><span class="sxs-lookup"><span data-stu-id="8837d-121">Once your organization is eligible for incentives, Microsoft will send an invitation to the MPN Admin of the eligible MPNLocationID to start the process.</span></span> <span data-ttu-id="8837d-122">この電子メールは、 **Microsoft パートナーセンター**から送信され、 **パートナーインセンティブ登録招待**を受けます。</span><span class="sxs-lookup"><span data-stu-id="8837d-122">This email will be sent from **Microsoft Partner Center**, and will have the subject **Partner Incentive Enrollment Invitation**.</span></span> <span data-ttu-id="8837d-123">招待を開き、[ **開始**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8837d-123">Open the invitation and select **Get Started**.</span></span>

<span data-ttu-id="8837d-124">パートナーセンターのホームページにも、招待が表示されます。</span><span class="sxs-lookup"><span data-stu-id="8837d-124">You’ll also see an invitation on the Partner Center home page.</span></span> <span data-ttu-id="8837d-125">このメッセージを選択すると、再度表示することはできません。</span><span class="sxs-lookup"><span data-stu-id="8837d-125">Once you select that message, you won’t be able to see it again.</span></span> <span data-ttu-id="8837d-126">ただし、管理者は、 [パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)で [ユーザーの管理] に移動してプロセスを開始できます。</span><span class="sxs-lookup"><span data-stu-id="8837d-126">However, the Admin can still start the process by going to User Management in the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

## <a name="expiration-and-renewal"></a><span data-ttu-id="8837d-127">有効期限と更新</span><span class="sxs-lookup"><span data-stu-id="8837d-127">Expiration and renewal</span></span>

<span data-ttu-id="8837d-128">インセンティブの登録は、会計年度の終了時に期限切れになります。</span><span class="sxs-lookup"><span data-stu-id="8837d-128">Incentives enrollment expires at the end of the fiscal year.</span></span> <span data-ttu-id="8837d-129">ただし、有効な契約を結んでいる資格のあるパートナーをお持ちであれば、Microsoft は、インセンティブ登録を次の会計年度にロールフォワードします。</span><span class="sxs-lookup"><span data-stu-id="8837d-129">However, as long as you remain an eligible partner with an active agreement, Microsoft will roll forward your incentives enrollment into the next fiscal year.</span></span> <span data-ttu-id="8837d-130">何らかのアクションをとる必要はありません。</span><span class="sxs-lookup"><span data-stu-id="8837d-130">You don't need to take any action.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8837d-131">次の手順</span><span class="sxs-lookup"><span data-stu-id="8837d-131">Next steps</span></span>

- [<span data-ttu-id="8837d-132">プログラムの適格性を確認する</span><span class="sxs-lookup"><span data-stu-id="8837d-132">Determine your program eligibility</span></span>](incentives-determined-your-program-eligibility.md)
