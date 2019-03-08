---
title: ユーザー ロールとアクセス許可の割り当て |パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: すべての従業員がパートナー センターで動作する必要がありますが、ロールを割り当てる必要があります。
author: LauraBrenner
ms.author: labrenne
keywords: ロール, アクセス許可, 管理者, エージェント
ms.localizationpriority: medium
ms.openlocfilehash: 038a2d6f4d58bbd9a71a2b241ee68982e0e7ef0a
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587745"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="4eabe-104">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="4eabe-104">Assign users roles and permissions</span></span>


<span data-ttu-id="4eabe-105">有効な名前とアドレス、サポートの詳細、税の除外対象をファイル、銀行情報、および会社の主要な連絡先を含む、パートナーのプロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="4eabe-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="4eabe-106">次の手順: をパートナー センターで作業を開始するため、パスワードとロールを設定するユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="4eabe-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="4eabe-107">パートナー センターで使用する従業員を設定します。</span><span class="sxs-lookup"><span data-stu-id="4eabe-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="4eabe-108">役割とアクセス許可を付けると、パートナー センターにユーザーが持つアクセス権の種類を決定します。</span><span class="sxs-lookup"><span data-stu-id="4eabe-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="4eabe-109">ロールで、ビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="4eabe-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="4eabe-110">たとえば、会社がクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、必要はありませんのみ標準の Azure AD テナント グローバル管理者などの管理ロールが必要がありますの役割、CSP プログラムに固有です。</span><span class="sxs-lookup"><span data-stu-id="4eabe-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="4eabe-111">各プログラムには、固有の役割があります。</span><span class="sxs-lookup"><span data-stu-id="4eabe-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="4eabe-112">Azure Active Directory (AAD) テナント ロールには、グローバル管理者、ユーザー管理者、および CSP の役割が含まれます。</span><span class="sxs-lookup"><span data-stu-id="4eabe-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="4eabe-113">非 AAD のロールには、MPN 管理者、ビジネス プロファイルの管理、参照の管理、インセンティブの管理者およびインセンティブのユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="4eabe-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="4eabe-114">パートナー センターでの商用トランザクションを管理する (Azure AD と CSP の役割)</span><span class="sxs-lookup"><span data-stu-id="4eabe-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="4eabe-115">**ロール**</span><span class="sxs-lookup"><span data-stu-id="4eabe-115">**Role**</span></span>|<span data-ttu-id="4eabe-116">**何ができます。**</span><span class="sxs-lookup"><span data-stu-id="4eabe-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="4eabe-117">全体管理者</span><span class="sxs-lookup"><span data-stu-id="4eabe-117">Global admin</span></span>|<span data-ttu-id="4eabe-118">• 完全な特権を持つ Microsoft アカウントが/サービスすべてにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="4eabe-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="4eabe-119">• パートナー センターのサポート チケットを作成します。</span><span class="sxs-lookup"><span data-stu-id="4eabe-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="4eabe-120">• 契約の表示、価格表、および特典</span><span class="sxs-lookup"><span data-stu-id="4eabe-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="4eabe-121">• ビューの作成、およびパートナーのユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="4eabe-122">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="4eabe-122">User Admin</span></span>   | <span data-ttu-id="4eabe-123">• ビューの作成、およびユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="4eabe-124">• すべてのパートナー プロファイルを表示します。</span><span class="sxs-lookup"><span data-stu-id="4eabe-124">• View all partner profiles</span></span>
||<span data-ttu-id="4eabe-125">• ビューの作成、およびパートナーのユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="4eabe-126">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="4eabe-126">Default user</span></span>|  <span data-ttu-id="4eabe-127">マイ プロファイルを表示します。</span><span class="sxs-lookup"><span data-stu-id="4eabe-127">View My profile</span></span>   |
|<span data-ttu-id="4eabe-128">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="4eabe-128">Admin agent</span></span> | <span data-ttu-id="4eabe-129">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-129">•    Customer management</span></span>
||<span data-ttu-id="4eabe-130">• パートナー センターにデバイスのリストを追加 <</span><span class="sxs-lookup"><span data-stu-id="4eabe-130">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="4eabe-131">• の作成し、プロファイルをデバイスに適用されます。</span><span class="sxs-lookup"><span data-stu-id="4eabe-131">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="4eabe-132">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-132">• Subscription management</span></span>
||<span data-ttu-id="4eabe-133">顧客の • サービス正常性とサービス要求</span><span class="sxs-lookup"><span data-stu-id="4eabe-133">• Service health and service requests for customers</span></span>
||<span data-ttu-id="4eabe-134">• 要求が委任された管理者特権</span><span class="sxs-lookup"><span data-stu-id="4eabe-134">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="4eabe-135">• 表示価格とプランに関する</span><span class="sxs-lookup"><span data-stu-id="4eabe-135">• View pricing and offers</span></span>
||<span data-ttu-id="4eabe-136">• 請求</span><span class="sxs-lookup"><span data-stu-id="4eabe-136">• Billing</span></span>
||<span data-ttu-id="4eabe-137">• は、お客様に代わって管理を行う</span><span class="sxs-lookup"><span data-stu-id="4eabe-137">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="4eabe-138">• レジスタ値を再販業者の追加</span><span class="sxs-lookup"><span data-stu-id="4eabe-138">• Register a value added reseller</span></span>|
|<span data-ttu-id="4eabe-139">販売代理店</span><span class="sxs-lookup"><span data-stu-id="4eabe-139">Sales agent</span></span> | <span data-ttu-id="4eabe-140">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-140">•    Customer management</span></span>
||<span data-ttu-id="4eabe-141">• デバイスの一覧をパートナー センターに追加</span><span class="sxs-lookup"><span data-stu-id="4eabe-141">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="4eabe-142">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-142">• Subscription management</span></span>
||<span data-ttu-id="4eabe-143">• ビューのサポート チケット</span><span class="sxs-lookup"><span data-stu-id="4eabe-143">• View support tickets</span></span>
||<span data-ttu-id="4eabe-144">• 顧客とのリレーションシップの要求</span><span class="sxs-lookup"><span data-stu-id="4eabe-144">• Request a relationship with a customer</span></span>
||<span data-ttu-id="4eabe-145">• 潜在顧客の管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-145">• Manage customer leads</span></span>
||<span data-ttu-id="4eabe-146">• 顧客契約書の表示</span><span class="sxs-lookup"><span data-stu-id="4eabe-146">• View the customer agreement</span></span>
||<span data-ttu-id="4eabe-147">• レジスタ付加価値再販業者</span><span class="sxs-lookup"><span data-stu-id="4eabe-147">• Register a value-added reseller</span></span>|
|<span data-ttu-id="4eabe-148">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="4eabe-148">Helpdesk agent</span></span>| <span data-ttu-id="4eabe-149">• 検索し、顧客の表示</span><span class="sxs-lookup"><span data-stu-id="4eabe-149">•  Search for and view a customer</span></span>
||<span data-ttu-id="4eabe-150">• 顧客詳細の編集</span><span class="sxs-lookup"><span data-stu-id="4eabe-150">• Edit customer details</span></span>
||<span data-ttu-id="4eabe-151">• ヘルプ顧客の問題を解決課金やサブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-151">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="4eabe-152">顧客に代わって • 要求のサポート (注。管理エージェントでの Office 365 サブスクリプションには、このタスクを完了する必要があります)</span><span class="sxs-lookup"><span data-stu-id="4eabe-152">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="4eabe-153">• サブスクリプションの管理し、課金顧客に代わって問題 (注。管理エージェントでの Office 365 サブスクリプションには、このタスクを完了する必要があります)</span><span class="sxs-lookup"><span data-stu-id="4eabe-153">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="4eabe-154">コントロール パネルのベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="4eabe-154">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="4eabe-155">(CSP のロールと非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="4eabe-155">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="4eabe-156">CPVs では、パートナー センター Api と、システムを統合するためのクラウド ソリューション プロバイダー (CSP) パートナーで使用するためのアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="4eabe-156">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="4eabe-157">**ロール**</span><span class="sxs-lookup"><span data-stu-id="4eabe-157">**Role**</span></span>   |<span data-ttu-id="4eabe-158">**何ができます。**</span><span class="sxs-lookup"><span data-stu-id="4eabe-158">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="4eabe-159">全体管理者</span><span class="sxs-lookup"><span data-stu-id="4eabe-159">Global admin</span></span>| <span data-ttu-id="4eabe-160">表示および CPV プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-160">View and manage your CPV profile</span></span>|
||<span data-ttu-id="4eabe-161">表示および CPV 機能へのアクセスを必要とするユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-161">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="4eabe-162">MPN メンバーシップと会社 (非 AAD ロールを) 管理します。</span><span class="sxs-lookup"><span data-stu-id="4eabe-162">Manage MPN membership and your company (non-AAD roles)</span></span>

|<span data-ttu-id="4eabe-163">**ロール**</span><span class="sxs-lookup"><span data-stu-id="4eabe-163">**Role**</span></span> | <span data-ttu-id="4eabe-164">**何ができます。**</span><span class="sxs-lookup"><span data-stu-id="4eabe-164">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="4eabe-165">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="4eabe-165">MPN partner admin</span></span>|<span data-ttu-id="4eabe-166">•Can は、テナント以外のユーザーを追加します。</span><span class="sxs-lookup"><span data-stu-id="4eabe-166">•Can add non-tenant users</span></span>
||<span data-ttu-id="4eabe-167">• ビューの作成、およびパートナー サービス要求の管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-167">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="4eabe-168">• 法的ビュー、組織、ビジネス、および MPN プロファイル</span><span class="sxs-lookup"><span data-stu-id="4eabe-168">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="4eabe-169">• ユーザーの詳細の表示とそのスキル データ</span><span class="sxs-lookup"><span data-stu-id="4eabe-169">• View user details and their skills data</span></span>
||<span data-ttu-id="4eabe-170">• コンピテンシーを表示します</span><span class="sxs-lookup"><span data-stu-id="4eabe-170">• View competencies</span></span>
||<span data-ttu-id="4eabe-171">• の表示し、管理の利点があります</span><span class="sxs-lookup"><span data-stu-id="4eabe-171">• View and manage benefits</span></span>
||<span data-ttu-id="4eabe-172">MPN の提供 • ビューと購入</span><span class="sxs-lookup"><span data-stu-id="4eabe-172">• View and purchase MPN offers</span></span>
||<span data-ttu-id="4eabe-173">• MPN のビューには、注文履歴と請求書が提供しています</span><span class="sxs-lookup"><span data-stu-id="4eabe-173">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="4eabe-174">• パートナー コントリビューション データの表示</span><span class="sxs-lookup"><span data-stu-id="4eabe-174">• View partner contribution data</span></span>
||<span data-ttu-id="4eabe-175">• には、バウチャーの検証ツールを動作します。</span><span class="sxs-lookup"><span data-stu-id="4eabe-175">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="4eabe-176">-顧客データの分析を表示します。</span><span class="sxs-lookup"><span data-stu-id="4eabe-176">- View customer data analytics</span></span>
|<span data-ttu-id="4eabe-177">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="4eabe-177">Account admin</span></span>| <span data-ttu-id="4eabe-178">• は、テナント以外のユーザーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="4eabe-178">•   Can add non-tenant users</span></span>
||<span data-ttu-id="4eabe-179">• を追加または場所の削除</span><span class="sxs-lookup"><span data-stu-id="4eabe-179">• Add or delete locations</span></span>
||<span data-ttu-id="4eabe-180">-ユーザーが管理者のアカウントに関連するプロファイルを管理します。</span><span class="sxs-lookup"><span data-stu-id="4eabe-180">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="4eabe-181">• 非 AAD のロールをテナントのユーザーのロールの割り当て</span><span class="sxs-lookup"><span data-stu-id="4eabe-181">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="4eabe-182">• プログラムに場所を登録します。</span><span class="sxs-lookup"><span data-stu-id="4eabe-182">• Enroll locations into programs</span></span>

## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="4eabe-183">(非 AAD ロール) の参照を管理します。</span><span class="sxs-lookup"><span data-stu-id="4eabe-183">Manage referrals (non-AAD roles)</span></span>

|<span data-ttu-id="4eabe-184">**ロール**</span><span class="sxs-lookup"><span data-stu-id="4eabe-184">**Role**</span></span>|<span data-ttu-id="4eabe-185">**何ができます。**</span><span class="sxs-lookup"><span data-stu-id="4eabe-185">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="4eabe-186">参照の管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-186">Referrals admin</span></span>       |<span data-ttu-id="4eabe-187">• ビューの作成、およびビジネス プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-187">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="4eabe-188">• が受信し、参照の管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-188">• Receive and manage referrals</span></span>
||<span data-ttu-id="4eabe-189">• ビューの作成、およびパートナー サービス要求の管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-189">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="4eabe-190">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="4eabe-190">Business profile admin</span></span>   |<span data-ttu-id="4eabe-191">•View、作成、およびビジネス プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-191">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="4eabe-192">• ビューの作成、およびパートナー サービス要求の管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-192">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="4eabe-193">インセンティブ (非 AAD ロール) の管理します。</span><span class="sxs-lookup"><span data-stu-id="4eabe-193">Manage Incentives  (non-AAD roles)</span></span>

|<span data-ttu-id="4eabe-194">**ロール**</span><span class="sxs-lookup"><span data-stu-id="4eabe-194">**Role**</span></span> | <span data-ttu-id="4eabe-195">**何ができます。**</span><span class="sxs-lookup"><span data-stu-id="4eabe-195">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="4eabe-196">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="4eabe-196">Incentives admin</span></span>|<span data-ttu-id="4eabe-197">• が開始し、インセンティブの管理</span><span class="sxs-lookup"><span data-stu-id="4eabe-197">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="4eabe-198">• を表示およびインセンティブ プログラムのすべての側面を編集できます。</span><span class="sxs-lookup"><span data-stu-id="4eabe-198">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="4eabe-199">• を表示および銀行と税の詳細を編集できます。</span><span class="sxs-lookup"><span data-stu-id="4eabe-199">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="4eabe-200">• ビュー リベートと co-op 収益</span><span class="sxs-lookup"><span data-stu-id="4eabe-200">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="4eabe-201">• アクセスのサポート</span><span class="sxs-lookup"><span data-stu-id="4eabe-201">• Access support</span></span>
||<span data-ttu-id="4eabe-202">• 争議インセンティブの支払い</span><span class="sxs-lookup"><span data-stu-id="4eabe-202">• Dispute incentives payments</span></span>|
|<span data-ttu-id="4eabe-203">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="4eabe-203">Incentives user</span></span>|<span data-ttu-id="4eabe-204">• は、インセンティブ プログラムを表示できます。</span><span class="sxs-lookup"><span data-stu-id="4eabe-204">•  Can view incentives programs</span></span>
||<span data-ttu-id="4eabe-205">• を表示およびインセンティブの要求を開始できます。</span><span class="sxs-lookup"><span data-stu-id="4eabe-205">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="4eabe-206">• ビュー リベートと co-op 収益</span><span class="sxs-lookup"><span data-stu-id="4eabe-206">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="4eabe-207">• ビュー リベートと co-op 収益</span><span class="sxs-lookup"><span data-stu-id="4eabe-207">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="4eabe-208">• アクセスのサポート</span><span class="sxs-lookup"><span data-stu-id="4eabe-208">• Access support</span></span>












