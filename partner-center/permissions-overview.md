---
title: ユーザー ロールとアクセス許可を割り当てる |パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: パートナー センターで作業する必要があるすべての従業員には、ロールを割り当てる必要があります。
author: labrenne
ms.author: labrenne
keywords: 役割、アクセス許可、管理エージェント
ms.localizationpriority: medium
ms.openlocfilehash: d811cb76b03b1784eaf926052e6a00151b2fc347
ms.sourcegitcommit: bfbb5b5edb381e219134be5a3e4a97bfe232288f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "9086730"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="132f7-104">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="132f7-104">Assign users roles and permissions</span></span>


<span data-ttu-id="132f7-105">法的名前とアドレス、サポートの詳細、税金の除外のファイル、銀行情報、会社の第一連絡先担当者などパートナー プロファイルを設定します。</span><span class="sxs-lookup"><span data-stu-id="132f7-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="132f7-106">次の手順: を使用してパートナー センターで作業を開始したため、パスワードとロールを設定するユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="132f7-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="132f7-107">パートナー センターで作業する従業員のセットアップします。</span><span class="sxs-lookup"><span data-stu-id="132f7-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="132f7-108">役割とアクセス許可を提供することによって、ユーザーがパートナー センターがアクセスの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="132f7-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="132f7-109">ロールは、ビジネスが関与する入金に関連します。</span><span class="sxs-lookup"><span data-stu-id="132f7-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="132f7-110">たとえば、お客様のビジネスがクラウド ソリューション プロバイダー (CSP) のビジネスの場合は、する必要はありませんのみ標準の Azure AD テナントのグローバル管理者などの管理の役割が必要がありますロールの CSP プログラムに固有です。</span><span class="sxs-lookup"><span data-stu-id="132f7-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="132f7-111">各プログラムには、それを特定の役割があります。</span><span class="sxs-lookup"><span data-stu-id="132f7-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="132f7-112">Azure Active Directory (AAD) テナントの役割には、全体管理者には、ユーザー管理者には、CSP の役割にはが含まれます。</span><span class="sxs-lookup"><span data-stu-id="132f7-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="132f7-113">非 AAD の役割には、MPN 管理者、ビジネス プロファイル管理者、紹介管理者、インセンティブの管理者とインセンティブ ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="132f7-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="132f7-114">パートナー センターでの商用のトランザクションを管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="132f7-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|**<span data-ttu-id="132f7-115">ロール</span><span class="sxs-lookup"><span data-stu-id="132f7-115">Role</span></span>**|**<span data-ttu-id="132f7-116">できること</span><span class="sxs-lookup"><span data-stu-id="132f7-116">What they can do</span></span>**|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="132f7-117">グローバル管理</span><span class="sxs-lookup"><span data-stu-id="132f7-117">Global admin</span></span>|<span data-ttu-id="132f7-118">• すべての Microsoft アカウント/サービスに完全な特権にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="132f7-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="132f7-119">• パートナー センターのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="132f7-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="132f7-120">• ビュー契約、価格表とプラン</span><span class="sxs-lookup"><span data-stu-id="132f7-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="132f7-121">• 表示、作成、およびパートナー ユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="132f7-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="132f7-122">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="132f7-122">User Admin</span></span>   | <span data-ttu-id="132f7-123">• 表示、作成、およびユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="132f7-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="132f7-124">• すべてのパートナー プロファイルを表示します。</span><span class="sxs-lookup"><span data-stu-id="132f7-124">• View all partner profiles</span></span>
||<span data-ttu-id="132f7-125">• 表示、作成、およびパートナー ユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="132f7-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="132f7-126">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="132f7-126">Default user</span></span>|  <span data-ttu-id="132f7-127">プロフィールを表示します。</span><span class="sxs-lookup"><span data-stu-id="132f7-127">View My profile</span></span>   |
|<span data-ttu-id="132f7-128">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="132f7-128">Admin agent</span></span> | <span data-ttu-id="132f7-129">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="132f7-129">•    Customer management</span></span>
||<span data-ttu-id="132f7-130">• パートナー Center< にデバイスの一覧を追加します。</span><span class="sxs-lookup"><span data-stu-id="132f7-130">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="132f7-131">• を作成し、デバイスにプロファイルを適用</span><span class="sxs-lookup"><span data-stu-id="132f7-131">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="132f7-132">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="132f7-132">• Subscription management</span></span>
||<span data-ttu-id="132f7-133">顧客のための • サービスの正常性とサービス要求</span><span class="sxs-lookup"><span data-stu-id="132f7-133">• Service health and service requests for customers</span></span>
||<span data-ttu-id="132f7-134">• 要求は、管理者特権を委任</span><span class="sxs-lookup"><span data-stu-id="132f7-134">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="132f7-135">• ビューの [料金とプラン</span><span class="sxs-lookup"><span data-stu-id="132f7-135">• View pricing and offers</span></span>
||<span data-ttu-id="132f7-136">• 請求</span><span class="sxs-lookup"><span data-stu-id="132f7-136">• Billing</span></span>
||<span data-ttu-id="132f7-137">• が顧客の代理として管理します。</span><span class="sxs-lookup"><span data-stu-id="132f7-137">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="132f7-138">• レジスタ値をリセラーを追加します。</span><span class="sxs-lookup"><span data-stu-id="132f7-138">• Register a value added reseller</span></span>|
|<span data-ttu-id="132f7-139">販売代理店</span><span class="sxs-lookup"><span data-stu-id="132f7-139">Sales agent</span></span> | <span data-ttu-id="132f7-140">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="132f7-140">•    Customer management</span></span>
||<span data-ttu-id="132f7-141">• パートナー センターへのデバイスの一覧の追加</span><span class="sxs-lookup"><span data-stu-id="132f7-141">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="132f7-142">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="132f7-142">• Subscription management</span></span>
||<span data-ttu-id="132f7-143">• サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="132f7-143">• View support tickets</span></span>
||<span data-ttu-id="132f7-144">• 要求顧客との関係</span><span class="sxs-lookup"><span data-stu-id="132f7-144">• Request a relationship with a customer</span></span>
||<span data-ttu-id="132f7-145">• 見込み客の管理</span><span class="sxs-lookup"><span data-stu-id="132f7-145">• Manage customer leads</span></span>
||<span data-ttu-id="132f7-146">• 顧客契約書の表示</span><span class="sxs-lookup"><span data-stu-id="132f7-146">• View the customer agreement</span></span>
||<span data-ttu-id="132f7-147">• レジスタ付加価値リセラー</span><span class="sxs-lookup"><span data-stu-id="132f7-147">• Register a value-added reseller</span></span>|
|<span data-ttu-id="132f7-148">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="132f7-148">Helpdesk agent</span></span>| <span data-ttu-id="132f7-149">• を検索し、顧客の表示</span><span class="sxs-lookup"><span data-stu-id="132f7-149">•  Search for and view a customer</span></span>
||<span data-ttu-id="132f7-150">• 編集顧客の詳細</span><span class="sxs-lookup"><span data-stu-id="132f7-150">• Edit customer details</span></span>
||<span data-ttu-id="132f7-151">• ヘルプ解決に関する顧客の問題請求やサブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="132f7-151">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="132f7-152">顧客の代理として • 要求のサポート (注: Office 365 サブスクリプションの場合は、このタスクを完了する管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="132f7-152">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="132f7-153">• サブスクリプションの管理し、請求の顧客の代理としての問題 (注: Office 365 サブスクリプションの場合は、このタスクを完了する管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="132f7-153">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="132f7-154">コントロール パネル (CPV) をベンダー。</span><span class="sxs-lookup"><span data-stu-id="132f7-154">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="132f7-155">(CSP のロールと AAD 以外のロール)</span><span class="sxs-lookup"><span data-stu-id="132f7-155">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="132f7-156">CPVs は、クラウド ソリューション プロバイダー (CSP) パートナーがパートナー センター Api と、システムの統合を有効にするためのアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="132f7-156">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|**<span data-ttu-id="132f7-157">ロール</span><span class="sxs-lookup"><span data-stu-id="132f7-157">Role</span></span>**   |**<span data-ttu-id="132f7-158">何ができます。</span><span class="sxs-lookup"><span data-stu-id="132f7-158">What you can do</span></span>**|
|------------------------------|:----------------------------|
|<span data-ttu-id="132f7-159">グローバル管理</span><span class="sxs-lookup"><span data-stu-id="132f7-159">Global admin</span></span>| <span data-ttu-id="132f7-160">表示し、CPV プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="132f7-160">View and manage your CPV profile</span></span>|
||<span data-ttu-id="132f7-161">表示し、CPV 機能へのアクセスを必要とする、ユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="132f7-161">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="132f7-162">MPN メンバーシップと会社 (非 AAD ロールを) 管理します。</span><span class="sxs-lookup"><span data-stu-id="132f7-162">Manage MPN membership and your company (non-AAD roles)</span></span>

|**<span data-ttu-id="132f7-163">ロール</span><span class="sxs-lookup"><span data-stu-id="132f7-163">Role</span></span>** | **<span data-ttu-id="132f7-164">何ができます。</span><span class="sxs-lookup"><span data-stu-id="132f7-164">What you can do</span></span>**|
|----------------------------|:----------------------------|
|<span data-ttu-id="132f7-165">MPN 管理者</span><span class="sxs-lookup"><span data-stu-id="132f7-165">MPN admin</span></span>|<span data-ttu-id="132f7-166">•Can いないテナント ユーザーを追加します。</span><span class="sxs-lookup"><span data-stu-id="132f7-166">•Can add non-tenant users</span></span>
||<span data-ttu-id="132f7-167">• 表示、作成、およびパートナー サービス要求を管理します。</span><span class="sxs-lookup"><span data-stu-id="132f7-167">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="132f7-168">• 法的ビュー、組織でビジネス、および MPN プロファイル</span><span class="sxs-lookup"><span data-stu-id="132f7-168">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="132f7-169">• ユーザーの詳細を表示およびスキル データ</span><span class="sxs-lookup"><span data-stu-id="132f7-169">• View user details and their skills data</span></span>
||<span data-ttu-id="132f7-170">• コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="132f7-170">• View competencies</span></span>
||<span data-ttu-id="132f7-171">• を表示して、特典を管理します。</span><span class="sxs-lookup"><span data-stu-id="132f7-171">• View and manage benefits</span></span>
||<span data-ttu-id="132f7-172">MPN • ビューと購入は提供します。</span><span class="sxs-lookup"><span data-stu-id="132f7-172">• View and purchase MPN offers</span></span>
||<span data-ttu-id="132f7-173">• ビュー MPN プランの注文履歴と請求書</span><span class="sxs-lookup"><span data-stu-id="132f7-173">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="132f7-174">• がパートナーの貢献度データを表示できます。</span><span class="sxs-lookup"><span data-stu-id="132f7-174">• Can view partner contribution data</span></span>
||<span data-ttu-id="132f7-175">• 伝票検証ツールで作業します。</span><span class="sxs-lookup"><span data-stu-id="132f7-175">• Can work in the Voucher Validation tool</span></span>|
|<span data-ttu-id="132f7-176">アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="132f7-176">Account admin</span></span>| <span data-ttu-id="132f7-177">• いないテナント ユーザーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="132f7-177">•   Can add non-tenant users</span></span>
||<span data-ttu-id="132f7-178">• を追加または場所の削除</span><span class="sxs-lookup"><span data-stu-id="132f7-178">• Add or delete locations</span></span>
||<span data-ttu-id="132f7-179">-の管理者のアカウントに関連するプロファイルを管理します。</span><span class="sxs-lookup"><span data-stu-id="132f7-179">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="132f7-180">非 AAD のロールにテナント内のユーザーの • 割り当ての役割</span><span class="sxs-lookup"><span data-stu-id="132f7-180">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="132f7-181">• プログラムへの場所への登録</span><span class="sxs-lookup"><span data-stu-id="132f7-181">• Enroll locations into programs</span></span>

## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="132f7-182">(非 AAD ロール) の紹介を管理します。</span><span class="sxs-lookup"><span data-stu-id="132f7-182">Manage referrals (non-AAD roles)</span></span>

|**<span data-ttu-id="132f7-183">ロール</span><span class="sxs-lookup"><span data-stu-id="132f7-183">Role</span></span>**|**<span data-ttu-id="132f7-184">何ができます。</span><span class="sxs-lookup"><span data-stu-id="132f7-184">What you can do</span></span>**|
|-----------------------------|:------------------------|
|<span data-ttu-id="132f7-185">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="132f7-185">Referrals admin</span></span>       |<span data-ttu-id="132f7-186">• ビューを作成して、ビジネス プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="132f7-186">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="132f7-187">• 受信し、紹介の管理</span><span class="sxs-lookup"><span data-stu-id="132f7-187">• Receive and manage referrals</span></span>
||<span data-ttu-id="132f7-188">• 表示、作成、およびパートナー サービス要求を管理します。</span><span class="sxs-lookup"><span data-stu-id="132f7-188">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="132f7-189">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="132f7-189">Business profile admin</span></span>   |<span data-ttu-id="132f7-190">•View、作成、およびビジネス プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="132f7-190">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="132f7-191">• 表示、作成、およびパートナー サービス要求を管理します。</span><span class="sxs-lookup"><span data-stu-id="132f7-191">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="132f7-192">インセンティブ (非 AAD ロール) を管理します。</span><span class="sxs-lookup"><span data-stu-id="132f7-192">Manage Incentives  (non-AAD roles)</span></span>

|**<span data-ttu-id="132f7-193">ロール</span><span class="sxs-lookup"><span data-stu-id="132f7-193">Role</span></span>** | **<span data-ttu-id="132f7-194">何ができます。</span><span class="sxs-lookup"><span data-stu-id="132f7-194">What you can do</span></span>**|
|------------------------------|:-------------------------|
|<span data-ttu-id="132f7-195">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="132f7-195">Incentives admin</span></span>|<span data-ttu-id="132f7-196">• を開始して、インセンティブを管理します。</span><span class="sxs-lookup"><span data-stu-id="132f7-196">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="132f7-197">• を表示およびインセンティブ プログラムのすべての側面を編集できます。</span><span class="sxs-lookup"><span data-stu-id="132f7-197">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="132f7-198">• は表示でき、銀行および税の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="132f7-198">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="132f7-199">• ビュー リベートや共同収益</span><span class="sxs-lookup"><span data-stu-id="132f7-199">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="132f7-200">• アクセスのサポート</span><span class="sxs-lookup"><span data-stu-id="132f7-200">• Access support</span></span>
||<span data-ttu-id="132f7-201">• 紛争インセンティブ支払い</span><span class="sxs-lookup"><span data-stu-id="132f7-201">• Dispute incentives payments</span></span>|
|<span data-ttu-id="132f7-202">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="132f7-202">Incentives user</span></span>|<span data-ttu-id="132f7-203">• は、インセンティブ プログラムを表示できます。</span><span class="sxs-lookup"><span data-stu-id="132f7-203">•  Can view incentives programs</span></span>
||<span data-ttu-id="132f7-204">• を表示およびインセンティブの申請を開始できます。</span><span class="sxs-lookup"><span data-stu-id="132f7-204">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="132f7-205">• ビュー リベートや共同収益</span><span class="sxs-lookup"><span data-stu-id="132f7-205">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="132f7-206">• ビュー リベートや共同収益</span><span class="sxs-lookup"><span data-stu-id="132f7-206">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="132f7-207">• アクセスのサポート</span><span class="sxs-lookup"><span data-stu-id="132f7-207">• Access support</span></span>












