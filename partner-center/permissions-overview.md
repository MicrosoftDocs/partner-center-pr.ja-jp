---
title: ユーザー ロールとアクセス許可を割り当てる |パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: パートナー センターで作業する必要があるすべての従業員には、ロールを割り当てる必要があります。
author: labrenne
ms.author: labrenne
keywords: 役割、アクセス許可、管理エージェント
ms.localizationpriority: medium
ms.openlocfilehash: cc0e37601b16033bf31faaf5056ca0389d6f5cf6
ms.sourcegitcommit: 7961476a8fed7cd56a09c6edc8dd1e2dd7f46465
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/27/2019
ms.locfileid: "9117215"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="27039-104">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="27039-104">Assign users roles and permissions</span></span>


<span data-ttu-id="27039-105">法的名前とアドレス、サポートの詳細、税金の除外のファイル、銀行情報、会社の第一連絡先担当者などパートナー プロファイルを設定します。</span><span class="sxs-lookup"><span data-stu-id="27039-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="27039-106">次の手順: を使用してパートナー センターで作業を開始したため、パスワードとロールを設定するユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="27039-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="27039-107">パートナー センターで作業する従業員のセットアップします。</span><span class="sxs-lookup"><span data-stu-id="27039-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="27039-108">役割とアクセス許可を提供することによって、ユーザーがパートナー センターがアクセスの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="27039-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="27039-109">ロールは、ビジネスが関与する入金に関連します。</span><span class="sxs-lookup"><span data-stu-id="27039-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="27039-110">たとえば、お客様のビジネスがクラウド ソリューション プロバイダー (CSP) のビジネスの場合は、する必要はありませんのみ標準の Azure AD テナントのグローバル管理者などの管理の役割が必要がありますロールの CSP プログラムに固有です。</span><span class="sxs-lookup"><span data-stu-id="27039-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="27039-111">各プログラムには、それを特定の役割があります。</span><span class="sxs-lookup"><span data-stu-id="27039-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="27039-112">Azure Active Directory (AAD) テナントの役割には、全体管理者には、ユーザー管理者には、CSP の役割にはが含まれます。</span><span class="sxs-lookup"><span data-stu-id="27039-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="27039-113">非 AAD の役割には、MPN 管理者、ビジネス プロファイル管理者、紹介管理者、インセンティブの管理者とインセンティブ ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="27039-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="27039-114">パートナー センターでの商用のトランザクションを管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="27039-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|**<span data-ttu-id="27039-115">ロール</span><span class="sxs-lookup"><span data-stu-id="27039-115">Role</span></span>**|**<span data-ttu-id="27039-116">できること</span><span class="sxs-lookup"><span data-stu-id="27039-116">What they can do</span></span>**|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="27039-117">グローバル管理</span><span class="sxs-lookup"><span data-stu-id="27039-117">Global admin</span></span>|<span data-ttu-id="27039-118">• すべての Microsoft アカウント/サービスに完全な特権にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="27039-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="27039-119">• パートナー センターのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="27039-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="27039-120">• ビュー契約、価格表とプラン</span><span class="sxs-lookup"><span data-stu-id="27039-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="27039-121">• 表示、作成、およびパートナー ユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="27039-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="27039-122">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="27039-122">User Admin</span></span>   | <span data-ttu-id="27039-123">• 表示、作成、およびユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="27039-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="27039-124">• すべてのパートナー プロファイルを表示します。</span><span class="sxs-lookup"><span data-stu-id="27039-124">• View all partner profiles</span></span>
||<span data-ttu-id="27039-125">• 表示、作成、およびパートナー ユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="27039-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="27039-126">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="27039-126">Default user</span></span>|  <span data-ttu-id="27039-127">プロフィールを表示します。</span><span class="sxs-lookup"><span data-stu-id="27039-127">View My profile</span></span>   |
|<span data-ttu-id="27039-128">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="27039-128">Admin agent</span></span> | <span data-ttu-id="27039-129">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="27039-129">•    Customer management</span></span>
||<span data-ttu-id="27039-130">• パートナー Center< にデバイスの一覧を追加します。</span><span class="sxs-lookup"><span data-stu-id="27039-130">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="27039-131">• を作成し、デバイスにプロファイルを適用</span><span class="sxs-lookup"><span data-stu-id="27039-131">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="27039-132">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="27039-132">• Subscription management</span></span>
||<span data-ttu-id="27039-133">顧客のための • サービスの正常性とサービス要求</span><span class="sxs-lookup"><span data-stu-id="27039-133">• Service health and service requests for customers</span></span>
||<span data-ttu-id="27039-134">• 要求は、管理者特権を委任</span><span class="sxs-lookup"><span data-stu-id="27039-134">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="27039-135">• ビューの [料金とプラン</span><span class="sxs-lookup"><span data-stu-id="27039-135">• View pricing and offers</span></span>
||<span data-ttu-id="27039-136">• 請求</span><span class="sxs-lookup"><span data-stu-id="27039-136">• Billing</span></span>
||<span data-ttu-id="27039-137">• が顧客の代理として管理します。</span><span class="sxs-lookup"><span data-stu-id="27039-137">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="27039-138">• レジスタ値をリセラーを追加します。</span><span class="sxs-lookup"><span data-stu-id="27039-138">• Register a value added reseller</span></span>|
|<span data-ttu-id="27039-139">販売代理店</span><span class="sxs-lookup"><span data-stu-id="27039-139">Sales agent</span></span> | <span data-ttu-id="27039-140">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="27039-140">•    Customer management</span></span>
||<span data-ttu-id="27039-141">• パートナー センターへのデバイスの一覧の追加</span><span class="sxs-lookup"><span data-stu-id="27039-141">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="27039-142">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="27039-142">• Subscription management</span></span>
||<span data-ttu-id="27039-143">• サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="27039-143">• View support tickets</span></span>
||<span data-ttu-id="27039-144">• 要求顧客との関係</span><span class="sxs-lookup"><span data-stu-id="27039-144">• Request a relationship with a customer</span></span>
||<span data-ttu-id="27039-145">• 見込み客の管理</span><span class="sxs-lookup"><span data-stu-id="27039-145">• Manage customer leads</span></span>
||<span data-ttu-id="27039-146">• 顧客契約書の表示</span><span class="sxs-lookup"><span data-stu-id="27039-146">• View the customer agreement</span></span>
||<span data-ttu-id="27039-147">• レジスタ付加価値リセラー</span><span class="sxs-lookup"><span data-stu-id="27039-147">• Register a value-added reseller</span></span>|
|<span data-ttu-id="27039-148">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="27039-148">Helpdesk agent</span></span>| <span data-ttu-id="27039-149">• を検索し、顧客の表示</span><span class="sxs-lookup"><span data-stu-id="27039-149">•  Search for and view a customer</span></span>
||<span data-ttu-id="27039-150">• 編集顧客の詳細</span><span class="sxs-lookup"><span data-stu-id="27039-150">• Edit customer details</span></span>
||<span data-ttu-id="27039-151">• ヘルプ解決に関する顧客の問題請求やサブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="27039-151">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="27039-152">顧客の代理として • 要求のサポート (注: Office 365 サブスクリプションの場合は、このタスクを完了する管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="27039-152">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="27039-153">• サブスクリプションの管理し、請求の顧客の代理としての問題 (注: Office 365 サブスクリプションの場合は、このタスクを完了する管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="27039-153">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="27039-154">コントロール パネル (CPV) をベンダー。</span><span class="sxs-lookup"><span data-stu-id="27039-154">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="27039-155">(CSP のロールと AAD 以外のロール)</span><span class="sxs-lookup"><span data-stu-id="27039-155">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="27039-156">CPVs は、クラウド ソリューション プロバイダー (CSP) パートナーがパートナー センター Api と、システムの統合を有効にするためのアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="27039-156">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|**<span data-ttu-id="27039-157">ロール</span><span class="sxs-lookup"><span data-stu-id="27039-157">Role</span></span>**   |**<span data-ttu-id="27039-158">何ができます。</span><span class="sxs-lookup"><span data-stu-id="27039-158">What you can do</span></span>**|
|------------------------------|:----------------------------|
|<span data-ttu-id="27039-159">グローバル管理</span><span class="sxs-lookup"><span data-stu-id="27039-159">Global admin</span></span>| <span data-ttu-id="27039-160">表示し、CPV プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="27039-160">View and manage your CPV profile</span></span>|
||<span data-ttu-id="27039-161">表示し、CPV 機能へのアクセスを必要とする、ユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="27039-161">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="27039-162">MPN メンバーシップと会社 (非 AAD ロールを) 管理します。</span><span class="sxs-lookup"><span data-stu-id="27039-162">Manage MPN membership and your company (non-AAD roles)</span></span>

|**<span data-ttu-id="27039-163">ロール</span><span class="sxs-lookup"><span data-stu-id="27039-163">Role</span></span>** | **<span data-ttu-id="27039-164">何ができます。</span><span class="sxs-lookup"><span data-stu-id="27039-164">What you can do</span></span>**|
|----------------------------|:----------------------------|
|<span data-ttu-id="27039-165">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="27039-165">MPN partner admin</span></span>|<span data-ttu-id="27039-166">•Can いないテナント ユーザーを追加します。</span><span class="sxs-lookup"><span data-stu-id="27039-166">•Can add non-tenant users</span></span>
||<span data-ttu-id="27039-167">• 表示、作成、およびパートナー サービス要求を管理します。</span><span class="sxs-lookup"><span data-stu-id="27039-167">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="27039-168">• 法的ビュー、組織でビジネス、および MPN プロファイル</span><span class="sxs-lookup"><span data-stu-id="27039-168">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="27039-169">• ユーザーの詳細を表示およびスキル データ</span><span class="sxs-lookup"><span data-stu-id="27039-169">• View user details and their skills data</span></span>
||<span data-ttu-id="27039-170">• コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="27039-170">• View competencies</span></span>
||<span data-ttu-id="27039-171">• を表示して、特典を管理します。</span><span class="sxs-lookup"><span data-stu-id="27039-171">• View and manage benefits</span></span>
||<span data-ttu-id="27039-172">MPN • ビューと購入は提供します。</span><span class="sxs-lookup"><span data-stu-id="27039-172">• View and purchase MPN offers</span></span>
||<span data-ttu-id="27039-173">• ビュー MPN プランの注文履歴と請求書</span><span class="sxs-lookup"><span data-stu-id="27039-173">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="27039-174">• ビュー パートナーの貢献度データ</span><span class="sxs-lookup"><span data-stu-id="27039-174">• View partner contribution data</span></span>
||<span data-ttu-id="27039-175">• 伝票検証ツールで作業します。</span><span class="sxs-lookup"><span data-stu-id="27039-175">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="27039-176">-顧客データの分析を表示します。</span><span class="sxs-lookup"><span data-stu-id="27039-176">- View customer data analytics</span></span>
|<span data-ttu-id="27039-177">アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="27039-177">Account admin</span></span>| <span data-ttu-id="27039-178">• いないテナント ユーザーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="27039-178">•   Can add non-tenant users</span></span>
||<span data-ttu-id="27039-179">• を追加または場所の削除</span><span class="sxs-lookup"><span data-stu-id="27039-179">• Add or delete locations</span></span>
||<span data-ttu-id="27039-180">-の管理者のアカウントに関連するプロファイルを管理します。</span><span class="sxs-lookup"><span data-stu-id="27039-180">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="27039-181">非 AAD のロールにテナント内のユーザーの • 割り当ての役割</span><span class="sxs-lookup"><span data-stu-id="27039-181">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="27039-182">• プログラムへの場所への登録</span><span class="sxs-lookup"><span data-stu-id="27039-182">• Enroll locations into programs</span></span>

## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="27039-183">(非 AAD ロール) の紹介を管理します。</span><span class="sxs-lookup"><span data-stu-id="27039-183">Manage referrals (non-AAD roles)</span></span>

|**<span data-ttu-id="27039-184">ロール</span><span class="sxs-lookup"><span data-stu-id="27039-184">Role</span></span>**|**<span data-ttu-id="27039-185">何ができます。</span><span class="sxs-lookup"><span data-stu-id="27039-185">What you can do</span></span>**|
|-----------------------------|:------------------------|
|<span data-ttu-id="27039-186">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="27039-186">Referrals admin</span></span>       |<span data-ttu-id="27039-187">• ビューを作成して、ビジネス プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="27039-187">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="27039-188">• 受信し、紹介の管理</span><span class="sxs-lookup"><span data-stu-id="27039-188">• Receive and manage referrals</span></span>
||<span data-ttu-id="27039-189">• 表示、作成、およびパートナー サービス要求を管理します。</span><span class="sxs-lookup"><span data-stu-id="27039-189">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="27039-190">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="27039-190">Business profile admin</span></span>   |<span data-ttu-id="27039-191">•View、作成、およびビジネス プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="27039-191">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="27039-192">• 表示、作成、およびパートナー サービス要求を管理します。</span><span class="sxs-lookup"><span data-stu-id="27039-192">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="27039-193">インセンティブ (非 AAD ロール) を管理します。</span><span class="sxs-lookup"><span data-stu-id="27039-193">Manage Incentives  (non-AAD roles)</span></span>

|**<span data-ttu-id="27039-194">ロール</span><span class="sxs-lookup"><span data-stu-id="27039-194">Role</span></span>** | **<span data-ttu-id="27039-195">何ができます。</span><span class="sxs-lookup"><span data-stu-id="27039-195">What you can do</span></span>**|
|------------------------------|:-------------------------|
|<span data-ttu-id="27039-196">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="27039-196">Incentives admin</span></span>|<span data-ttu-id="27039-197">• を開始して、インセンティブを管理します。</span><span class="sxs-lookup"><span data-stu-id="27039-197">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="27039-198">• を表示およびインセンティブ プログラムのすべての側面を編集できます。</span><span class="sxs-lookup"><span data-stu-id="27039-198">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="27039-199">• は表示でき、銀行および税の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="27039-199">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="27039-200">• ビュー リベートや共同収益</span><span class="sxs-lookup"><span data-stu-id="27039-200">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="27039-201">• アクセスのサポート</span><span class="sxs-lookup"><span data-stu-id="27039-201">• Access support</span></span>
||<span data-ttu-id="27039-202">• 紛争インセンティブ支払い</span><span class="sxs-lookup"><span data-stu-id="27039-202">• Dispute incentives payments</span></span>|
|<span data-ttu-id="27039-203">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="27039-203">Incentives user</span></span>|<span data-ttu-id="27039-204">• は、インセンティブ プログラムを表示できます。</span><span class="sxs-lookup"><span data-stu-id="27039-204">•  Can view incentives programs</span></span>
||<span data-ttu-id="27039-205">• を表示およびインセンティブの申請を開始できます。</span><span class="sxs-lookup"><span data-stu-id="27039-205">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="27039-206">• ビュー リベートや共同収益</span><span class="sxs-lookup"><span data-stu-id="27039-206">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="27039-207">• ビュー リベートや共同収益</span><span class="sxs-lookup"><span data-stu-id="27039-207">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="27039-208">• アクセスのサポート</span><span class="sxs-lookup"><span data-stu-id="27039-208">• Access support</span></span>












