---
title: パートナーメンバーシップセンターからパートナーセンターへの移動を準備する |パートナーセンター
ms.topic: article
ms.date: 06/13/2019
description: ビジネスを PMC からパートナーセンターに移行する前に考慮すべきこと
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: d6db2dcb5ac53e29d907c09ca2b16d123b21c07f
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820570"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a><span data-ttu-id="bfa13-103">パートナーメンバーシップセンター (PMC) からパートナーセンターへの移行の準備</span><span class="sxs-lookup"><span data-stu-id="bfa13-103">Prepare for your move from Partner Membership Center (PMC) to Partner Center</span></span>

<span data-ttu-id="bfa13-104">パートナーメンバーシップセンター (PMC) からパートナーセンター (Microsoft との取引関係を管理するための単一の宛先) にメンバーシップ管理を移行しています。</span><span class="sxs-lookup"><span data-stu-id="bfa13-104">We are moving membership management from Partner Membership Center (PMC) to the partner center – the single destination to manage your business relationship with Microsoft.</span></span> <span data-ttu-id="bfa13-105">パートナーセンターへの移行は、可能な限り効率的で簡単です。</span><span class="sxs-lookup"><span data-stu-id="bfa13-105">We want your move to Partner Center to be as efficient and easy as possible.</span></span> <span data-ttu-id="bfa13-106">パートナーセンターが PMC と異なる領域をいくつか特定しましたが、移動する前に理解して準備する必要があると考えています。</span><span class="sxs-lookup"><span data-stu-id="bfa13-106">We’ve identified some areas where the Partner Center differs from PMC, and we think you will want to understand and prepare for them before you make the move.</span></span>

## <a name="account-and-identity-setup"></a><span data-ttu-id="bfa13-107">アカウントと id の設定</span><span class="sxs-lookup"><span data-stu-id="bfa13-107">Account and identity setup</span></span>

<span data-ttu-id="bfa13-108">**Azure Active Directory (Azure AD) 職場アカウントとは**</span><span class="sxs-lookup"><span data-stu-id="bfa13-108">**What is an Azure Active Directory (Azure AD) work account?**</span></span>

<span data-ttu-id="bfa13-109">Azure 職場アカウントは、Azure パブリック クラウドにおける企業の分離された専用の仮想表現です。Azure、Microsoft Intune、Office 365などの Microsoft クラウド サービスにサブスクライブすると作成されます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-109">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="bfa13-110">職場アカウントは、Azure AD のユーザーと、それらに関する情報 (電子メール、パスワード、プロファイルデータ、アクセス許可など) をホストします。</span><span class="sxs-lookup"><span data-stu-id="bfa13-110">Your work account hosts your Azure AD users and the information about them - their email, passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="bfa13-111">職場アカウントには、会社とそのセキュリティに関連するグループ、アプリケーション、およびその他の情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="bfa13-111">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span> <span data-ttu-id="bfa13-112">詳細については、</span><span class="sxs-lookup"><span data-stu-id="bfa13-112">For more information see …</span></span>

<span data-ttu-id="bfa13-113">パートナーセンターでは、職場の電子メールを使用して、個人の電子メールではなく、アカウントにサインインします。</span><span class="sxs-lookup"><span data-stu-id="bfa13-113">In the Partner Center you will use your work email to sign into your account not your personal email.</span></span>
- <span data-ttu-id="bfa13-114">職場アカウント:john@contoso.com</span><span class="sxs-lookup"><span data-stu-id="bfa13-114">Your work account: john@contoso.com</span></span>
- <span data-ttu-id="bfa13-115">個人のアカウント:John@outlook.com</span><span class="sxs-lookup"><span data-stu-id="bfa13-115">Your personal account: John@outlook.com</span></span>

<span data-ttu-id="bfa13-116">職場の電子メールは、Azure active directory テナントの一部です。</span><span class="sxs-lookup"><span data-stu-id="bfa13-116">Your work email is part of your Azure active directory tenant.</span></span> <span data-ttu-id="bfa13-117">パートナーセンターでアカウントを作成するには、AAD テナントが必要です。</span><span class="sxs-lookup"><span data-stu-id="bfa13-117">To have an account in Partner Center, you need to have an AAD tenant.</span></span> <span data-ttu-id="bfa13-118">Azure Active Directory の詳細については、「 [Azure AD でのディレクトリの作成」](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfa13-118">For more information on Azure Active Directory, read [Create your directory in Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).</span></span>

<span data-ttu-id="bfa13-119">**PMC からパートナーセンターに移行するときは、Microsoft と AAD テナント (たとえば、Office 365) を使用していて、CSP ビジネス用のテナントもある場合、パートナーセンターにサインインするアカウントを指定します。**</span><span class="sxs-lookup"><span data-stu-id="bfa13-119">**When you move to Partner Center from PMC, what account should you sign into Partner Center with if you have an AAD tenant with Microsoft (for Office 365 for example) and you also have a tenant for your CSP business?**</span></span>

<span data-ttu-id="bfa13-120">CSP アカウントまたは MPN 職場の電子メールアカウントを使用して、パートナーセンターにサインインできます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-120">You can sign into Partner Center with either the CSP account or your MPN work email account.</span></span> <span data-ttu-id="bfa13-121">CSP 職場の電子メールアドレスを使用してサインインすることを選択した場合、ダッシュボードの左側のナビゲーションに MPN と CSP の両方のプログラム情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-121">If you choose to sign in using your CSP work email, the left navigation on your dashboard will display both MPN and CSP program information.</span></span> <span data-ttu-id="bfa13-122">MPN Azure AD テナントの職場の電子メールアドレスでサインインすると、MPN プログラムの情報のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-122">If you sign in with your MPN Azure AD tenant work email, you will see only your MPN program information.</span></span> <span data-ttu-id="bfa13-123">ユーザーロールは MPN と CSP で異なります。 MPN と CSP の両方のビジネスで同じアカウントを使用する場合は、それに応じてユーザーロールを割り当てるようにしてください。</span><span class="sxs-lookup"><span data-stu-id="bfa13-123">User roles differ between MPN and CSP so if you use the same account for both MPN and CSP business, be sure you assign user roles accordingly.</span></span> <span data-ttu-id="bfa13-124">ユーザーロールの詳細については、「[ユーザーロールとアクセス許可の割り当て](permissions-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfa13-124">For information on user roles, read [Assign user roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="bfa13-125">**AAD グローバル管理者ロールと PMC MPN 全体管理者ロールの違いは何ですか。**</span><span class="sxs-lookup"><span data-stu-id="bfa13-125">**What is the difference between the AAD global admin role and the PMC MPN global admin role?**</span></span>

<span data-ttu-id="bfa13-126">これらは、異なるアクセス許可を持つ2つの完全に異なるロールです。</span><span class="sxs-lookup"><span data-stu-id="bfa13-126">These are two completely different roles with different permissions.</span></span> <span data-ttu-id="bfa13-127">パートナーセンターの AAD テナントのグローバル管理者は、テナントを管理します。ユーザーの追加または削除、パスワード、ロール、およびアクセス許可の提供と管理を行い、パートナーセンターですべての会社のプログラムにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-127">The AAD tenant global admin in Partner Center administers the tenant – adds or removes users, provides and manages passwords, roles and permissions, and has access to all their company’s programs in Partner Center.</span></span> 

<span data-ttu-id="bfa13-128">PMC の MPN グローバル管理者ロールは、次の操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-128">The MPN global admin role in PMC could do the following:</span></span>

- <span data-ttu-id="bfa13-129">会社および会社のすべての場所に関連付けられているすべてのデータを表示および編集する</span><span class="sxs-lookup"><span data-stu-id="bfa13-129">View and edit all the data associated with the company and all of the  company's locations</span></span>

-  <span data-ttu-id="bfa13-130">グローバルレベルまたはローカルレベルで管理者を追加します。</span><span class="sxs-lookup"><span data-stu-id="bfa13-130">Add administrators at the global or local level.</span></span>  <span data-ttu-id="bfa13-131">また、グローバル管理者は、任意の場所にグローバル管理者アクセス権を割り当てることができます。これにより、関連付けられている場所に関係なく、グローバルアクセス権が付与されます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-131">Also, Global admins can assign any person at any location Global Administrator Access which grants them global access regardless of which location they're associated with.</span></span>
-  <span data-ttu-id="bfa13-132">次のようなパートナー向けの UI 関数を実行します。</span><span class="sxs-lookup"><span data-stu-id="bfa13-132">Perform any partner facing UI function including:</span></span> 

-  <span data-ttu-id="bfa13-133">ユーザーの追加と削除</span><span class="sxs-lookup"><span data-stu-id="bfa13-133">Add/remove users</span></span>

 - <span data-ttu-id="bfa13-134">ロールの割り当て/削除</span><span class="sxs-lookup"><span data-stu-id="bfa13-134">Assign/remove roles</span></span> 

 - <span data-ttu-id="bfa13-135">場所の追加/削除/更新</span><span class="sxs-lookup"><span data-stu-id="bfa13-135">Add/remove/update locations</span></span> 

 - <span data-ttu-id="bfa13-136">コンピテンシー/マップの購入</span><span class="sxs-lookup"><span data-stu-id="bfa13-136">Purchase competency/maps</span></span> 

-  <span data-ttu-id="bfa13-137">特典の表示</span><span class="sxs-lookup"><span data-stu-id="bfa13-137">View benefits</span></span>

<span data-ttu-id="bfa13-138">MPN 全体管理者がパートナーセンターに移動すると、そのロールは、パートナーセンターのグローバル管理者とは異なるアクセス許可とタスクを持つ MPN Partner admin と呼ばれます。パートナーセンターのロールとアクセス許可の詳細については、「[ユーザーロールとアクセス許可の割り当て](permissions-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfa13-138">When the MPN global admin moves to Partner Center the role is called the MPN partner admin which has different permissions and tasks than the Partner Center global admin. For more information on roles and permissions in Partner Center, read [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="bfa13-139">**パートナーセンターのゲストユーザーロールを含むユーザーロール**</span><span class="sxs-lookup"><span data-stu-id="bfa13-139">**User roles including guest user roles in Partner Center**</span></span>

<span data-ttu-id="bfa13-140">パートナーセンターには、実行する必要のある作業の種類に応じて、さまざまな種類のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="bfa13-140">Partner Center has different types of roles depending on the types of work needed to be done.</span></span> <span data-ttu-id="bfa13-141">全体管理者などのロール Azure AD ロールがあります。</span><span class="sxs-lookup"><span data-stu-id="bfa13-141">There are roles such as global admin that are Azure AD roles.</span></span> <span data-ttu-id="bfa13-142">一部のロールは、クラウドサービスプロバイダープログラムやインセンティブなどのプログラムに固有のものであり、MPN に固有の役割があります。</span><span class="sxs-lookup"><span data-stu-id="bfa13-142">Some of the roles are specific to programs such as the Cloud Service Provider program or incentives, and there are roles that are specific to MPN.</span></span> <span data-ttu-id="bfa13-143">すべてのパートナーセンターの役割については、「[ユーザーロールとアクセス許可の割り当て](permissions-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfa13-143">To find out what all the Partner Center roles are, read [Assign users roles and permissions](permissions-overview.md).</span></span>



<span data-ttu-id="bfa13-144">**PMC からパートナーセンターに移行すると、ユーザーの役割はどうなりますか。**</span><span class="sxs-lookup"><span data-stu-id="bfa13-144">**What happens to my users' roles when they move from PMC to Partner Center?**</span></span>

<span data-ttu-id="bfa13-145">移行を実行する MPN のグローバル管理者または主要プログラムの連絡先を除き、PMC のすべてのユーザーが管理者の役割を失います。</span><span class="sxs-lookup"><span data-stu-id="bfa13-145">Except for the MPN global admin or primary program contact who conducts the migration, all users in PMC will lose their admin roles.</span></span> <span data-ttu-id="bfa13-146">移行を完了する個人は、パートナーセンターでロールを割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="bfa13-146">The individual who completes the migration will need to assign roles in Partner Center.</span></span> <span data-ttu-id="bfa13-147">パートナーセンターのロールは、PMC の役割とは異なります。</span><span class="sxs-lookup"><span data-stu-id="bfa13-147">The roles in Partner Center differ from those in PMC.</span></span> <span data-ttu-id="bfa13-148">パートナーセンターのユーザーロールの詳細については、[ユーザーロールとアクセス許可の割り当て] (アクセス許可-overview.md と[PMC からパートナーセンターへの移動](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles)) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfa13-148">Read [Assign users roles and permissions](permissions-overview.md and [Moving from PMC to Partner Center](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles) for more on user roles in Partner Center.</span></span>


<span data-ttu-id="bfa13-149">**会社のプロファイルとビジネスプロファイルの違いは何ですか。**</span><span class="sxs-lookup"><span data-stu-id="bfa13-149">**What’s the difference between my company profile and my business profile?**</span></span>

<span data-ttu-id="bfa13-150">会社のプロファイルは、住所、場所、主要連絡先、銀行、税金の詳細を含む会社の情報です。</span><span class="sxs-lookup"><span data-stu-id="bfa13-150">Your company profile is the information about your company that includes address, locations, primary contact, bank and tax details.</span></span>

<span data-ttu-id="bfa13-151">ビジネスプロファイルは顧客に自分で提示する方法であり、ロゴ、ビジネスフォーカスの詳細、専門知識などを表示するマーケティングページです。</span><span class="sxs-lookup"><span data-stu-id="bfa13-151">Your business profile is how you present yourself to customers and is a marketing page that displays your logo, details on your business focus, your expertise, etc.</span></span>

<span data-ttu-id="bfa13-152">**アカウントの統合とは何ですか。**</span><span class="sxs-lookup"><span data-stu-id="bfa13-152">**What does account consolidation mean for my account?**</span></span>

<span data-ttu-id="bfa13-153">同じ Azure AD テナントを使用して複数の MPN アカウントをパートナーセンターに移行すると、システムによって自動的に認識され、アカウントを統合するように求めるメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-153">If you use the same Azure AD tenant to migrate multiple MPN accounts into Partner Center, the system will automatically recognize that and ask you to consolidate your accounts.</span></span> <span data-ttu-id="bfa13-154">これは、同じ Azure AD テナントに複数のドメインが関連付けられている場合でも当てはまります。</span><span class="sxs-lookup"><span data-stu-id="bfa13-154">This is true even if you have multiple domains associated to the same Azure AD tenant.</span></span> 

<span data-ttu-id="bfa13-155">別の AAD テナントを使用してパートナーセンターに移行することもできますが、この結果には、コンピテンシーの分離評価と追加の購入コストが発生することに注意してください。</span><span class="sxs-lookup"><span data-stu-id="bfa13-155">You could still decide to migrate to Partner Center using separate AAD tenants, but please note this results in isolated evaluation of your competencies and extra purchase costs.</span></span> 

<span data-ttu-id="bfa13-156">**複数の AAD テナントと1つの MPN アカウントがある場合、パートナーセンターでそれらをリンクすることはできますか?**</span><span class="sxs-lookup"><span data-stu-id="bfa13-156">**If I have multiple AAD tenants and a single MPN account, is it possible to link them in Partner Center?**</span></span>

<span data-ttu-id="bfa13-157">はい。パートナーセンターでは、複数の Azure AD テナントを1つのパートナーセンターアカウントにリンクできます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-157">Yes, in Partner Center you can link multiple Azure AD tenants to single Partner Center account.</span></span>
<span data-ttu-id="bfa13-158">詳細については、こちらをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="bfa13-158">Learn more here.</span></span> 

<span data-ttu-id="bfa13-159">**複数の Azure AD テナントを1つのパートナーセンターアカウントに追加する場合、制限はありますか。**</span><span class="sxs-lookup"><span data-stu-id="bfa13-159">**Are there restrictions to adding multiple Azure AD tenants to a single Partner Center account?**</span></span>

<span data-ttu-id="bfa13-160">Azure AD テナントが既に既存のパートナーセンターアカウントに関連付けられている場合、マルチテナント機能を使用して新しいパートナーセンターアカウントに関連付けることはできません。</span><span class="sxs-lookup"><span data-stu-id="bfa13-160">If the Azure AD tenant is already associated to an existing Partner Center account, it can't be associated to new Partner Center accounts using the multi-tenancy feature.</span></span> <span data-ttu-id="bfa13-161">また、Azure AD テナントは1つのパートナーセンターアカウントにのみ関連付けることができますが、パートナーセンターアカウントには複数のテナントを関連付けることができます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-161">Another way to think of it is, an Azure AD tenant can only be associated to one Partner Center account, but a Partner Center account can have multiple tenants associated to it.</span></span>

## <a name="microsoft-partner-network-mpn-membership-migration"></a><span data-ttu-id="bfa13-162">Microsoft Partner Network (MPN) メンバーシップの移行</span><span class="sxs-lookup"><span data-stu-id="bfa13-162">Microsoft Partner Network (MPN) membership migration</span></span> 

<span data-ttu-id="bfa13-163">**PMC からパートナーセンターへの移行を実行できるのはだれですか?**</span><span class="sxs-lookup"><span data-stu-id="bfa13-163">**Who can perform the move from PMC to Partner Center?**</span></span>

<span data-ttu-id="bfa13-164">会社の MPN のグローバル管理者または主要プログラムの連絡先 (これら2つの役割は多くの場合、同じ人物によって保持されます) は、移動を開始して実行できます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-164">Your company MPN global admin or the primary program contact (these two roles are often held by the same person) can initiate and perform the move.</span></span>

<span data-ttu-id="bfa13-165">**移行を完了したユーザーは、パートナーセンターの会社の法的プロファイルに関する主要な連絡先になりますか。**</span><span class="sxs-lookup"><span data-stu-id="bfa13-165">**Will the person completing the migration become the primary contact on the company legal profile in Partner Center?**</span></span>

<span data-ttu-id="bfa13-166">ただし、プライマリ連絡先は必ずしも契約に署名する権限を持つユーザーである必要があります。</span><span class="sxs-lookup"><span data-stu-id="bfa13-166">Not necessarily, however, the primary contact needs to be someone who has authorization to sign agreements.</span></span>

<span data-ttu-id="bfa13-167">**Microsoft が自分の MPN メンバーシップを移行できますか?**</span><span class="sxs-lookup"><span data-stu-id="bfa13-167">**Can Microsoft migrate my MPN membership for me?**</span></span>

<span data-ttu-id="bfa13-168">No.</span><span class="sxs-lookup"><span data-stu-id="bfa13-168">No.</span></span> <span data-ttu-id="bfa13-169">Microsoft は、パートナーセンターへのメンバーシップアカウントの移行を支援するものではありません。</span><span class="sxs-lookup"><span data-stu-id="bfa13-169">Microsoft cannot help you move your membership account to partner center.</span></span> <span data-ttu-id="bfa13-170">移行プロセスを開始するには、職場アカウント (サインイン資格情報) を使用して PMC にサインインし、アカウントを移動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bfa13-170">You will need to move your account by signing into PMC with your work account (sign in credentials)to begin the migration process.</span></span> <span data-ttu-id="bfa13-171">アカウントを移動する手順を完了したら、メンバーシップの管理を開始し、ユーザーロールとアクセス許可をチームに割り当てて、特典にアクセスしてメンバーシップの管理に役立てることができます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-171">After you’ve completed the steps to move your account you can start managing your membership and  assign user roles and permissions to your team so they can access benefits and help manage the membership.</span></span> <span data-ttu-id="bfa13-172">Microsoft は、現在のコンピテンシー、特典、場所情報、インセンティブの銀行/税金情報、パートナー大学アクセスを含む MCP の関連付けを自動的に移行します。</span><span class="sxs-lookup"><span data-stu-id="bfa13-172">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="bfa13-173">Microsoft は、現在のコンピテンシー、特典、場所情報、インセンティブの銀行/税金情報、パートナー大学アクセスを含む MCP の関連付けを自動的に移行します。</span><span class="sxs-lookup"><span data-stu-id="bfa13-173">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="bfa13-174">**更新ポリシーはどのように変更されますか。**</span><span class="sxs-lookup"><span data-stu-id="bfa13-174">**How will the renewal policy change?**</span></span>

 <span data-ttu-id="bfa13-175">パートナーセンターでは、更新期間は、記念日から30日までとなります。</span><span class="sxs-lookup"><span data-stu-id="bfa13-175">In Partner Center, the renewal window is from your anniversary date through the following 30 days.</span></span>

<span data-ttu-id="bfa13-176">**パートナーセンターに移行した後も、コンピテンシーは変更されませんか?**</span><span class="sxs-lookup"><span data-stu-id="bfa13-176">**Will our competencies remain unchanged after we move to Partner Center?**</span></span>

<span data-ttu-id="bfa13-177">はい、パートナーセンターへの移動によって compentencies は影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="bfa13-177">Yes, compentencies will not be affected by the move to Partner Center.</span></span> <span data-ttu-id="bfa13-178">不一致に気付いた場合は、[サポート](https://partner.microsoft.com/support)にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="bfa13-178">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>


 <span data-ttu-id="bfa13-179">**私たちの特典 (クラウドの特典、テクニカルサポート、ソフトウェアの特典、Visual Studio など) は、移行後に変更されますか。**</span><span class="sxs-lookup"><span data-stu-id="bfa13-179">**Will my benefits (including cloud benefits, technical support, software benefits, Visual Studio) change after we move?**</span></span>

 <span data-ttu-id="bfa13-180">対象となる特典は変更されません。</span><span class="sxs-lookup"><span data-stu-id="bfa13-180">Your eligible benefits will not change.</span></span> <span data-ttu-id="bfa13-181">不一致に気付いた場合は、[サポート](https://partner.microsoft.com/support)にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="bfa13-181">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>

 <span data-ttu-id="bfa13-182">**Visual Studio の特典が割り当てられている Microsoft アカウントは使用できますか?**</span><span class="sxs-lookup"><span data-stu-id="bfa13-182">**Will our Microsoft accounts that have Visual Studio benefits allocations be honored?**</span></span>


 <span data-ttu-id="bfa13-183">可能。</span><span class="sxs-lookup"><span data-stu-id="bfa13-183">Yes.</span></span> <span data-ttu-id="bfa13-184">Visual Studio の特典は、MSAs に割り当てられ、保持されます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-184">Visual Studio benefits allocated to MSAs will be honored and retained.</span></span> <span data-ttu-id="bfa13-185">また、パートナーセンターでは更新後も保持されます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-185">They will also be preserved after renewal in Partner Center.</span></span> <span data-ttu-id="bfa13-186">ただし、パートナーセンターに移行した後に MSA 割り当てを削除しても、パートナーセンターに戻すことはできません。</span><span class="sxs-lookup"><span data-stu-id="bfa13-186">However, if you remove an MSA allocation once migrated in Partner Center, it can’t be added  back into Partner Center.</span></span>

<span data-ttu-id="bfa13-187">パートナーセンターでは、パートナーが Azure AD テナントの MPN admin である同じテナントから、MSA である仕事用アカウントとゲストユーザーアカウントを追加できます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-187">In Partner Center, a partner can add work accounts and guest user accounts which are MSA from the same tenant where the partner is MPN admin in the Azure AD tenant.</span></span> <span data-ttu-id="bfa13-188">パートナーが複数の Azure AD テナントのグローバル管理者であり、これらすべてのテナントが同じパートナーセンターアカウントに関連付けられている場合、パートナーは、これらすべてのテナントのユーザーを Visual Studio の特典と Azure の使用量ベースの割り当てに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-188">If the partner is a global admin in multiple Azure AD tenants and all these tenants are associated to the same Partner Center account, then the partner is allowed to add users across all these tenants into the Visual Studio benefits and Azure usage-based allocations.</span></span>

<span data-ttu-id="bfa13-189">ゲストユーザーは、MPN admin または全体管理者によって Visual Studio の使用量ベースのサブスクリプションを割り当てることができますが、ゲストユーザーは、MSA を使用してパートナーセンターにサインインすることはできません。</span><span class="sxs-lookup"><span data-stu-id="bfa13-189">Although guest users can be assigned usage-based subscriptions of Visual Studio by the MPN admin or global admin, guest users can't sign in to Partner Center using their MSA.</span></span> <span data-ttu-id="bfa13-190">ただし、ゲストユーザーは、Azure と Visual Studio にサインインして、割り当てられた特典を検証して使用することができます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-190">Guest users can, however, sign in to Azure and Visual Studio to validate and use their assigned benefits.</span></span>


 <span data-ttu-id="bfa13-191">**MCP の関連付けとパートナーの大学のアクセスを管理するにはどうすればよいですか。**</span><span class="sxs-lookup"><span data-stu-id="bfa13-191">**How should we manage our MCP associations and our Partner University access?**</span></span>

 <span data-ttu-id="bfa13-192">PMC から移動する MCP の関連付けに変更はありません。</span><span class="sxs-lookup"><span data-stu-id="bfa13-192">There are no changes to MCP associations that move from PMC.</span></span> <span data-ttu-id="bfa13-193">ただし、パートナーセンターに移行した後の新しい従業員は、パートナーセンターで関連付ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="bfa13-193">However, any new new employees after you move to Partner Center will need to be associated in Partner Center.</span></span> <span data-ttu-id="bfa13-194">既存のユーザーに対するパートナーの大学のアクセス許可はすべて残りますが、パートナーの大学にアクセスする方法については、新しい従業員が[トレーニングセンター](https://partner.microsoft.com/training)にアクセスしてください。</span><span class="sxs-lookup"><span data-stu-id="bfa13-194">All your Partner University permissions for existing users will remain but any new employees should go to [the training center](https://partner.microsoft.com/training) for information on how to gain access to Partner University.</span></span>

 <span data-ttu-id="bfa13-195">**パートナーセンターに移行したら、MCP 情報を表示操作方法ますか?**</span><span class="sxs-lookup"><span data-stu-id="bfa13-195">**How do I view MCP information once I move to Partner Center?**</span></span>

<span data-ttu-id="bfa13-196">ダッシュボードの左側のナビゲーションで **[コンピテンシー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="bfa13-196">Select **Competencies** from the left nav on the dashboard.</span></span> <span data-ttu-id="bfa13-197">**[コンピテンシー]** ページで、スキルレポートをダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-197">From the **Competencies** page you are able to download the skills report.</span></span> <span data-ttu-id="bfa13-198">スキルレポートには、パートナーセンターのコンピテンシーとプログラムに関連するスキルを獲得したユーザーの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-198">The skills report will list your users who have acquired skills relevant to the competencies and programs in Partner Center.</span></span> <span data-ttu-id="bfa13-199">ユーザーがスキルを獲得していても、自分が作業しているコンピテンシーに関連していないスキルは、レポートに表示されません。</span><span class="sxs-lookup"><span data-stu-id="bfa13-199">If your users have gained skills but those skills are not relevant to the competencies which you are working toward, they will not be listed in the report.</span></span>


 <span data-ttu-id="bfa13-200">**顧客参照はパートナーセンターで使用されていますか?**</span><span class="sxs-lookup"><span data-stu-id="bfa13-200">**Are customer references used in Partner Center?**</span></span>

 <span data-ttu-id="bfa13-201">いいえ、パートナーセンターのコンピテンシー要件を満たすために顧客参照は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="bfa13-201">No, you don't need customer references to meet competency requirements in Partner Center.</span></span>

 <span data-ttu-id="bfa13-202">**レコードの関連付けのパートナーはパートナーセンターに移行されますか?**</span><span class="sxs-lookup"><span data-stu-id="bfa13-202">**Will Partner of Record associations move to Partner Center?**</span></span>

 <span data-ttu-id="bfa13-203">はい、パートナーのレコードに変更はありません。</span><span class="sxs-lookup"><span data-stu-id="bfa13-203">Yes, there is no change to Partner of Record.</span></span> <span data-ttu-id="bfa13-204">[パートナー ID を顧客にリンクする方法の](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)詳細については、こちらを参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfa13-204">Find out more about [linking your partner ID to your customers](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).</span></span>

<span data-ttu-id="bfa13-205">**パートナーセンターへの移行により、インセンティブへの影響はありますか。**</span><span class="sxs-lookup"><span data-stu-id="bfa13-205">**Is there an impact to incentives because of the move to Partner Center?**</span></span>

<span data-ttu-id="bfa13-206">いいえ。場所を統合せずにアカウントを移動した場合、インセンティブへの影響はありません。</span><span class="sxs-lookup"><span data-stu-id="bfa13-206">No, there is no impact to incentives if you have moved your account without consolidating locations.</span></span> <span data-ttu-id="bfa13-207">PMC に複数のアカウントがあり、パートナーセンターに移行する際に、グローバルアカウントに統合することにした場合、インセンティブは失われませんが、インセンティブの支払いに遅れが生じる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="bfa13-207">If your business has multiple accounts in PMC and, when you move to Partner Center you decide to consolidate into a global account, there will be no loss to incentives but there may be a delay in incentive payout.</span></span> <span data-ttu-id="bfa13-208">インセンティブプログラムに含まれているすべての PMC アカウントを移動しない場合は、それらのアカウントに関連付けられているインセンティブを停止することができます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-208">If you don't move all your PMC accounts that have been involved in incentives programs, you may stop earning incentives that are tied to those accounts.</span></span>


<span data-ttu-id="bfa13-209">**パートナーセンターのインセンティブユーザーロールとは**</span><span class="sxs-lookup"><span data-stu-id="bfa13-209">**What are the incentive user roles in Partner Center?**</span></span> 

<span data-ttu-id="bfa13-210">パートナーセンターのインセンティブロールは、場所ベースであり、インセンティブ管理者とインセンティブユーザーを含みます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-210">Incentive roles in Partner Center are location-based and include Incentives admin and Incentives user.</span></span> <span data-ttu-id="bfa13-211">これらのロールで実行できる操作の詳細については、「[ユーザーロールとアクセス許可の割り当て](permissions-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bfa13-211">For more information on what those roles can do, see [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="bfa13-212">**インセンティブユーザーはグローバルレベルと場所レベルで割り当てることができますか。**</span><span class="sxs-lookup"><span data-stu-id="bfa13-212">**Can incentives users be assigned at the global and location level?**</span></span>

 <span data-ttu-id="bfa13-213">可能。</span><span class="sxs-lookup"><span data-stu-id="bfa13-213">Yes.</span></span> <span data-ttu-id="bfa13-214">すべての場所のインセンティブ管理者にインセンティブ管理者を割り当てるか、各場所に独自のインセンティブ管理者を割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-214">You can assign an incentives admin to be the incentives admin for all locations or each location can have its own incentives admin.</span></span>

 <span data-ttu-id="bfa13-215">**インセンティブはグローバルレベルまたは場所レベルで支払うことができますか。**</span><span class="sxs-lookup"><span data-stu-id="bfa13-215">**Can incentives be paid at the global or location level?**</span></span>

 <span data-ttu-id="bfa13-216">インセンティブは、場所レベルでのみ支払われます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-216">Incentives are paid only at the location level.</span></span>

<span data-ttu-id="bfa13-217">**紹介に関しては、作成できるビジネスプロファイルの数を確認できます。**</span><span class="sxs-lookup"><span data-stu-id="bfa13-217">**Regarding referrals, how many business profiles can we create?**</span></span>

<span data-ttu-id="bfa13-218">会社では、会社の関心を完全に表すために必要な数のビジネスプロファイルを作成できます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-218">Your company can create as many business profiles as your need for fully represent your company's interests.</span></span> <span data-ttu-id="bfa13-219">各ビジネスプロファイルでは、国ごとに1つの場所に最大5つの場所を表示できます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-219">In each business profile, you can list up to five locations, one location per country.</span></span> <span data-ttu-id="bfa13-220">各ビジネスプロファイルは、それぞれの場所の参照を受け取ることができます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-220">Each of the business profiles can receive referrals for each of its locations.</span></span>

<span data-ttu-id="bfa13-221">**紹介はどのように割り当てられますか。どのような変更が必要ですか。たとえば、ある市場にグローバル企業があり、その他の市場に拠点がある場合、紹介はどのように割り当てられますか。**</span><span class="sxs-lookup"><span data-stu-id="bfa13-221">**How will referrals be assigned, what changes can I expect? For example, if I have a global company in one market and locations in other markets, how will referrals be assigned?**</span></span>

<span data-ttu-id="bfa13-222">参照は、顧客が定義する検索パラメーターに基づいて割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-222">Referrals are assigned based on the search parameters that the customer defines.</span></span> <span data-ttu-id="bfa13-223">1つまたは複数の場所があるかどうかにかかわらず、顧客が目的の場所を指定し、他のパラメーターを満たすビジネスがある場合は、その場所に参照が表示されます。</span><span class="sxs-lookup"><span data-stu-id="bfa13-223">So regardless of whether you have one location or many, if the customers specifies a desired location and you have a business there that meets the other parameters, then the referral would go to that location.</span></span>








