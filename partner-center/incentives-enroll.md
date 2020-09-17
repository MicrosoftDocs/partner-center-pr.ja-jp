---
title: インセンティブの登録
ms.topic: how-to
ms.date: 09/11/2020
description: インセンティブプログラムに登録し、ユーザー管理に必要なロールを割り当てます。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: 7f86b59708ab26a5ef02a952f34ef3558af097af
ms.sourcegitcommit: b91119c587d37b4ed36dda00c2b0b1946beb3012
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/17/2020
ms.locfileid: "90714446"
---
# <a name="enrollment-and-user-management-in-the-incentives-program"></a><span data-ttu-id="80c4f-103">インセンティブプログラムにおける登録とユーザー管理</span><span class="sxs-lookup"><span data-stu-id="80c4f-103">Enrollment and user management in the incentives program</span></span>

<span data-ttu-id="80c4f-104">**適用対象:**</span><span class="sxs-lookup"><span data-stu-id="80c4f-104">**Applies to:**</span></span>

- <span data-ttu-id="80c4f-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="80c4f-105">Partner Center</span></span>

<span data-ttu-id="80c4f-106">**適切なロール:**</span><span class="sxs-lookup"><span data-stu-id="80c4f-106">**Appropriate roles:**</span></span>

- <span data-ttu-id="80c4f-107">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="80c4f-107">Incentives admin</span></span>

>[!NOTE]
><span data-ttu-id="80c4f-108">インセンティブプログラムに登録する前に、パートナーのメンバーシップセンターでパートナーセンターへの [移行](prepare-pmc-pc-migration.md)を完了している必要があります。</span><span class="sxs-lookup"><span data-stu-id="80c4f-108">Before you can enroll in the incentives program you must have completed the Partner Membership Center to Partner Center [migration](prepare-pmc-pc-migration.md).</span></span>

<span data-ttu-id="80c4f-109">登録プロセスは2つの手順で構成されます。</span><span class="sxs-lookup"><span data-stu-id="80c4f-109">The enrollment process consists of two steps.</span></span>

<span data-ttu-id="80c4f-110">**手順 1.ユーザー管理:** この手順では、インセンティブ管理者とユーザーのアクセス許可を設定します。</span><span class="sxs-lookup"><span data-stu-id="80c4f-110">**Step 1. User management:** This step involves establishing the Incentive Administrator and user permissions.</span></span>

<span data-ttu-id="80c4f-111">**手順 2.登録: Microsoft は** 、インセンティブプログラムに登録するための招待を送信します。</span><span class="sxs-lookup"><span data-stu-id="80c4f-111">**Step 2. Enrollment:** Microsoft sends you an invitation to enroll in your incentive program.</span></span>

## <a name="user-management"></a><span data-ttu-id="80c4f-112">[ユーザー管理]</span><span class="sxs-lookup"><span data-stu-id="80c4f-112">User Management</span></span>

<span data-ttu-id="80c4f-113">インセンティブプログラムに登録するには、グローバル管理者またはアカウント管理者が会社のユーザーを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="80c4f-113">To enroll in an incentive program, the Global Administrator or Account Administrator needs to set up your company users.</span></span> <span data-ttu-id="80c4f-114">インセンティブ管理者を割り当て、インセンティブユーザーのアクセス許可を付与する必要があります。</span><span class="sxs-lookup"><span data-stu-id="80c4f-114">They must assign an Incentive Administrator(s) and grant Incentive User permissions.</span></span> <span data-ttu-id="80c4f-115">パートナーアカウント、ロール、アクセス許可の詳細については、「 [パートナーセンターアカウントの管理](partner-center-account-setup.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80c4f-115">For information on partner accounts, roles, and permissions, see [Manage your Partner Center account](partner-center-account-setup.md).</span></span> <span data-ttu-id="80c4f-116">グローバル管理者は、Azure Active Directory (Azure AD) を使用して、会社のユーザーを設定することもできます。</span><span class="sxs-lookup"><span data-stu-id="80c4f-116">The Global Administrator can also set up your company users through the Azure Active Directory (Azure AD).</span></span>

<span data-ttu-id="80c4f-117">組織がインセンティブの対象となると、Microsoft はグローバル管理者、アカウント管理者、インセンティブ管理者に招待を送信します。</span><span class="sxs-lookup"><span data-stu-id="80c4f-117">Once your organization is eligible for incentives, Microsoft will send invitations to the Global Administrator, Account Administrator, and Incentive Administrator.</span></span>

>[!NOTE]
><span data-ttu-id="80c4f-118">インセンティブプログラムに登録できるのは、インセンティブ管理者だけです。</span><span class="sxs-lookup"><span data-stu-id="80c4f-118">Only the Incentive Administrator can enroll in incentive programs.</span></span> <span data-ttu-id="80c4f-119">お客様の場所にインセンティブ管理者がいない場合は、全体管理者とアカウント管理者が1つを割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="80c4f-119">If there is no Incentive Administrator for your location, the Global Administrator and Account Administrator must assign one.</span></span> <span data-ttu-id="80c4f-120">MPN Id の場所にインセンティブ管理者が割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="80c4f-120">The Incentive Administrator must be assigned for the location MPN IDs.</span></span> <span data-ttu-id="80c4f-121">全体管理者またはアカウント管理者は、インセンティブ管理者として割り当てることもできます。</span><span class="sxs-lookup"><span data-stu-id="80c4f-121">The Global Administrator or Account Administrator can also be assigned as the Incentive Administrator.</span></span>

## <a name="enrollment-process"></a><span data-ttu-id="80c4f-122">登録プロセス</span><span class="sxs-lookup"><span data-stu-id="80c4f-122">Enrollment Process</span></span>

<span data-ttu-id="80c4f-123">組織がインセンティブの対象となると、Microsoft は、対象となる MPNLocationID の MPN 管理者に招待を送信してプロセスを開始します。</span><span class="sxs-lookup"><span data-stu-id="80c4f-123">Once your organization is eligible for incentives, Microsoft will send an invitation to the MPN Admin of the eligible MPNLocationID to start the process.</span></span> <span data-ttu-id="80c4f-124">この電子メールは、 **Microsoft パートナーセンター**から送信され、 **パートナーインセンティブ登録招待**を受けます。</span><span class="sxs-lookup"><span data-stu-id="80c4f-124">This email will be sent from **Microsoft Partner Center**, and will have the subject **Partner Incentive Enrollment Invitation**.</span></span> <span data-ttu-id="80c4f-125">招待を開き、[ **開始**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="80c4f-125">Open the invitation and select **Get Started**.</span></span>

<span data-ttu-id="80c4f-126">パートナーセンターのホームページにも、招待が表示されます。</span><span class="sxs-lookup"><span data-stu-id="80c4f-126">You’ll also see an invitation on the Partner Center home page.</span></span> <span data-ttu-id="80c4f-127">このメッセージを選択すると、再度表示することはできません。</span><span class="sxs-lookup"><span data-stu-id="80c4f-127">Once you select that message, you won’t be able to see it again.</span></span> <span data-ttu-id="80c4f-128">ただし、管理者は、 [パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/) にサインインして [ **ユーザー管理**] を選択することで、プロセスを開始できます。</span><span class="sxs-lookup"><span data-stu-id="80c4f-128">However, the Admin can still start the process by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) and selecting **User Management**.</span></span>

## <a name="expiration-and-renewal"></a><span data-ttu-id="80c4f-129">有効期限と更新</span><span class="sxs-lookup"><span data-stu-id="80c4f-129">Expiration and renewal</span></span>

<span data-ttu-id="80c4f-130">インセンティブの登録は、会計年度の終了時に期限切れになります。</span><span class="sxs-lookup"><span data-stu-id="80c4f-130">Incentives enrollment expires at the end of the fiscal year.</span></span> <span data-ttu-id="80c4f-131">ただし、有効な契約を結んでいる資格のあるパートナーをお持ちであれば、Microsoft は、インセンティブ登録を次の会計年度にロールフォワードします。</span><span class="sxs-lookup"><span data-stu-id="80c4f-131">However, as long as you remain an eligible partner with an active agreement, Microsoft will roll forward your incentives enrollment into the next fiscal year.</span></span> <span data-ttu-id="80c4f-132">何らかのアクションをとる必要はありません。</span><span class="sxs-lookup"><span data-stu-id="80c4f-132">You don't need to take any action.</span></span>

## <a name="next-steps"></a><span data-ttu-id="80c4f-133">次の手順</span><span class="sxs-lookup"><span data-stu-id="80c4f-133">Next steps</span></span>

- [<span data-ttu-id="80c4f-134">プログラムの適格性を確認する</span><span class="sxs-lookup"><span data-stu-id="80c4f-134">Determine your program eligibility</span></span>](incentives-determined-your-program-eligibility.md)
