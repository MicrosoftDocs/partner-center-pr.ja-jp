---
title: ユーザー ロールとアクセス許可の割り当て |パートナー センター
ms.topic: article
ms.date: 10/10/2019
description: パートナー センターで作業する必要があるすべての従業員にロールを割り当てる必要があります。
author: LauraBrenner
ms.author: labrenne
keywords: ロール, アクセス許可, 管理者, エージェント
ms.localizationpriority: high
ms.openlocfilehash: 0bbc9af84b8a1464f255c17147fdc10a7504eb43
ms.sourcegitcommit: 1ccc27092949deb6f6404e64fd6a628fd7b5fd5c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/11/2019
ms.locfileid: "72276095"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="34851-104">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="34851-104">Assign users roles and permissions</span></span>


<span data-ttu-id="34851-105">貴社の正式名称や法的住所、サポートの詳細、税金の除外の申告、銀行情報、主要な連絡先など、パートナー プロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="34851-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="34851-106">次に、ユーザーにパスワードとロールを設定させて、ユーザーがパートナー センターでの作業を開始できるようにします。</span><span class="sxs-lookup"><span data-stu-id="34851-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="34851-107">パートナー センターで作業できるように従業員を設定する</span><span class="sxs-lookup"><span data-stu-id="34851-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="34851-108">ユーザーに付与するロールとアクセス許可によって、パートナー センターでのユーザーのアクセスの種類が決まります。</span><span class="sxs-lookup"><span data-stu-id="34851-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="34851-109">ロールは、貴社のビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="34851-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="34851-110">たとえば、貴社のビジネスがクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、グローバル管理者などの標準の Azure AD テナント管理ロールだけでなく、CSP プログラムに固有のロールも必要です。</span><span class="sxs-lookup"><span data-stu-id="34851-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="34851-111">各プログラムには、それに固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="34851-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="34851-112">Azure Active Directory (AAD) テナント ロールには、グローバル管理者、ユーザー管理者、および CSP のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="34851-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="34851-113">AAD 以外のロールはテナントを管理しないロールであり、MPN 管理者、ビジネス プロファイル管理者、紹介管理者、インセンティブ管理者、およびインセンティブ ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="34851-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="34851-114">パートナー センターで商取引を管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="34851-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="34851-115">**Role**</span><span class="sxs-lookup"><span data-stu-id="34851-115">**Role**</span></span>|<span data-ttu-id="34851-116">**できること**</span><span class="sxs-lookup"><span data-stu-id="34851-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="34851-117">全体管理者</span><span class="sxs-lookup"><span data-stu-id="34851-117">Global admin</span></span>|<span data-ttu-id="34851-118">• すべての特権を備えたすべての Microsoft アカウント/サービスへのアクセス</span><span class="sxs-lookup"><span data-stu-id="34851-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="34851-119">• パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="34851-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="34851-120">• 契約、価格表、キャンペーンの表示</span><span class="sxs-lookup"><span data-stu-id="34851-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="34851-121">• パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34851-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="34851-122">課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34851-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="34851-123">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="34851-123">User management admin</span></span>   | <span data-ttu-id="34851-124">• ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34851-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="34851-125">• すべてのパートナー プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="34851-125">• View all partner profiles</span></span>
||<span data-ttu-id="34851-126">• パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34851-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="34851-127">課金の管理</span><span class="sxs-lookup"><span data-stu-id="34851-127">Billing admin</span></span> | <span data-ttu-id="34851-128">- 課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34851-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="34851-129">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="34851-129">Default user</span></span>|  <span data-ttu-id="34851-130">マイ プロフィールの表示</span><span class="sxs-lookup"><span data-stu-id="34851-130">View My profile</span></span>   |
|<span data-ttu-id="34851-131">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="34851-131">Admin agent</span></span> | <span data-ttu-id="34851-132">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="34851-132">•    Customer management</span></span>
||<span data-ttu-id="34851-133">• パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="34851-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="34851-134">• プロファイルの作成とデバイスへの適用</span><span class="sxs-lookup"><span data-stu-id="34851-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="34851-135">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="34851-135">• Subscription management</span></span>
||<span data-ttu-id="34851-136">• 顧客のためのサービスの正常性の確認とサービス要求</span><span class="sxs-lookup"><span data-stu-id="34851-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="34851-137">• 代理管理者特権の要求</span><span class="sxs-lookup"><span data-stu-id="34851-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="34851-138">• 価格とプランの表示</span><span class="sxs-lookup"><span data-stu-id="34851-138">• View pricing and offers</span></span>
||<span data-ttu-id="34851-139">• 請求</span><span class="sxs-lookup"><span data-stu-id="34851-139">• Billing</span></span>
||<span data-ttu-id="34851-140">• 顧客の代理としての管理</span><span class="sxs-lookup"><span data-stu-id="34851-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="34851-141">• 付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="34851-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="34851-142">販売代理店</span><span class="sxs-lookup"><span data-stu-id="34851-142">Sales agent</span></span> | <span data-ttu-id="34851-143">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="34851-143">•    Customer management</span></span>
||<span data-ttu-id="34851-144">• パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="34851-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="34851-145">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="34851-145">• Subscription management</span></span>
||<span data-ttu-id="34851-146">• サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="34851-146">• View support tickets</span></span>
||<span data-ttu-id="34851-147">• 顧客との再販業者関係の要求</span><span class="sxs-lookup"><span data-stu-id="34851-147">• Request a relationship with a customer</span></span>
||<span data-ttu-id="34851-148">• 見込み客の管理</span><span class="sxs-lookup"><span data-stu-id="34851-148">• Manage customer leads</span></span>
||<span data-ttu-id="34851-149">• 顧客契約の表示</span><span class="sxs-lookup"><span data-stu-id="34851-149">• View the customer agreement</span></span>
||<span data-ttu-id="34851-150">• 付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="34851-150">• Register a value-added reseller</span></span>|
|<span data-ttu-id="34851-151">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="34851-151">Helpdesk agent</span></span>| <span data-ttu-id="34851-152">• 顧客の検索と表示</span><span class="sxs-lookup"><span data-stu-id="34851-152">•  Search for and view a customer</span></span>
||<span data-ttu-id="34851-153">• 顧客の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="34851-153">• Edit customer details</span></span>
||<span data-ttu-id="34851-154">• 請求やサブスクリプション管理に関する顧客の問題の解決サポート</span><span class="sxs-lookup"><span data-stu-id="34851-154">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="34851-155">• 顧客の代理としてのサポート要求 (注: Office 365 サブスクリプションの場合、このタスクを完了するには管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="34851-155">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="34851-156">• 顧客の代理としてのサブスクリプションとサービスの管理 (注: Office 365 サブスクリプションの場合、このタスクを完了するには管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="34851-156">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="34851-157">コントロール パネル ベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="34851-157">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="34851-158">(CSP ロールと非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="34851-158">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="34851-159">CPV は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムとパートナー センター API を統合するために使用するアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="34851-159">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="34851-160">**Role**</span><span class="sxs-lookup"><span data-stu-id="34851-160">**Role**</span></span>   |<span data-ttu-id="34851-161">**できること**</span><span class="sxs-lookup"><span data-stu-id="34851-161">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="34851-162">全体管理者</span><span class="sxs-lookup"><span data-stu-id="34851-162">Global admin</span></span>| <span data-ttu-id="34851-163">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="34851-163">View and manage your CPV profile</span></span>|
||<span data-ttu-id="34851-164">CPV 機能にアクセスする必要があるユーザーの表示と管理</span><span class="sxs-lookup"><span data-stu-id="34851-164">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="34851-165">ゲスト ユーザー (AAD テナントに追加される必要があります)</span><span class="sxs-lookup"><span data-stu-id="34851-165">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="34851-166">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="34851-166">**Guest user**</span></span>   | <span data-ttu-id="34851-167">**ロール**</span><span class="sxs-lookup"><span data-stu-id="34851-167">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="34851-168">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="34851-168">MPN partner admin</span></span>|
||<span data-ttu-id="34851-169">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="34851-169">Accounts admin</span></span>|
||<span data-ttu-id="34851-170">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="34851-170">Incentives admin</span></span>|
||<span data-ttu-id="34851-171">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="34851-171">Business profile admin</span></span>|
||<span data-ttu-id="34851-172">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="34851-172">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="34851-173">MPN メンバーシップと会社の管理 (AAD 以外のロール: これらのロールは、テナントではなく会社の業務を管理します)</span><span class="sxs-lookup"><span data-stu-id="34851-173">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="34851-174">**Role**</span><span class="sxs-lookup"><span data-stu-id="34851-174">**Role**</span></span> | <span data-ttu-id="34851-175">**できること**</span><span class="sxs-lookup"><span data-stu-id="34851-175">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="34851-176">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="34851-176">MPN partner admin</span></span>|<span data-ttu-id="34851-177">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34851-177">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="34851-178">• 法的プロファイル、企業プロファイル、ビジネス プロファイル、MPN プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="34851-178">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="34851-179">• ユーザーの詳細およびスキル データの表示</span><span class="sxs-lookup"><span data-stu-id="34851-179">• View user details and their skills data</span></span>
||<span data-ttu-id="34851-180">• コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="34851-180">• View competencies</span></span>
||<span data-ttu-id="34851-181">• 特典の表示と管理</span><span class="sxs-lookup"><span data-stu-id="34851-181">• View and manage benefits</span></span>
||<span data-ttu-id="34851-182">• MPN オファーの表示と購入</span><span class="sxs-lookup"><span data-stu-id="34851-182">• View and purchase MPN offers</span></span>
||<span data-ttu-id="34851-183">• MPN オファーの注文履歴と請求書の表示</span><span class="sxs-lookup"><span data-stu-id="34851-183">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="34851-184">• パートナー貢献度インジケーター データの表示</span><span class="sxs-lookup"><span data-stu-id="34851-184">• View partner contribution indicator data</span></span>
||<span data-ttu-id="34851-185">• 利用券検証ツールでの作業</span><span class="sxs-lookup"><span data-stu-id="34851-185">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="34851-186">- 顧客データ分析の表示</span><span class="sxs-lookup"><span data-stu-id="34851-186">- View customer data analytics</span></span>
|| <span data-ttu-id="34851-187">会社内の他のユーザー ロールを表示しますが、ロールを割り当てることはできません</span><span class="sxs-lookup"><span data-stu-id="34851-187">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="34851-188">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="34851-188">Account admin</span></span>| <span data-ttu-id="34851-189">場所の追加</span><span class="sxs-lookup"><span data-stu-id="34851-189">Add locations</span></span>
|| <span data-ttu-id="34851-190">管理対象のアカウントに関連するプロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="34851-190">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="34851-191">• テナント内のユーザーに対するロールの非 AAD ロールへの割り当て</span><span class="sxs-lookup"><span data-stu-id="34851-191">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="34851-192">• プログラムへの場所の登録</span><span class="sxs-lookup"><span data-stu-id="34851-192">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="34851-193">紹介の管理</span><span class="sxs-lookup"><span data-stu-id="34851-193">Manage referrals</span></span> 

|<span data-ttu-id="34851-194">**Role**</span><span class="sxs-lookup"><span data-stu-id="34851-194">**Role**</span></span>|<span data-ttu-id="34851-195">**できること**</span><span class="sxs-lookup"><span data-stu-id="34851-195">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="34851-196">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="34851-196">Referrals admin</span></span>       |<span data-ttu-id="34851-197">• ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34851-197">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="34851-198">• 紹介案件の受信と管理</span><span class="sxs-lookup"><span data-stu-id="34851-198">• Receive and manage referrals</span></span>
||<span data-ttu-id="34851-199">• 共同販売の紹介の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34851-199">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="34851-200">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34851-200">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="34851-201">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="34851-201">Business profile admin</span></span>   |<span data-ttu-id="34851-202">• ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34851-202">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="34851-203">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34851-203">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="34851-204">インセンティブの管理</span><span class="sxs-lookup"><span data-stu-id="34851-204">Manage incentives</span></span> 

|<span data-ttu-id="34851-205">**Role**</span><span class="sxs-lookup"><span data-stu-id="34851-205">**Role**</span></span> | <span data-ttu-id="34851-206">**できること**</span><span class="sxs-lookup"><span data-stu-id="34851-206">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="34851-207">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="34851-207">Incentives admin</span></span>|<span data-ttu-id="34851-208">• インセンティブの開始と管理</span><span class="sxs-lookup"><span data-stu-id="34851-208">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="34851-209">• インセンティブ プログラムのすべての側面の表示と編集</span><span class="sxs-lookup"><span data-stu-id="34851-209">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="34851-210">• 銀行および税の詳細情報の表示と編集</span><span class="sxs-lookup"><span data-stu-id="34851-210">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="34851-211">• リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="34851-211">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="34851-212">• サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="34851-212">• Access support</span></span>
||<span data-ttu-id="34851-213">• インセンティブ支払いについての議論</span><span class="sxs-lookup"><span data-stu-id="34851-213">• Dispute incentives payments</span></span>|
|<span data-ttu-id="34851-214">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="34851-214">Incentives user</span></span>|<span data-ttu-id="34851-215">• インセンティブ プログラムの表示</span><span class="sxs-lookup"><span data-stu-id="34851-215">•  Can view incentives programs</span></span>
||<span data-ttu-id="34851-216">• インセンティブの申請の表示と開始</span><span class="sxs-lookup"><span data-stu-id="34851-216">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="34851-217">• リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="34851-217">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="34851-218">• サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="34851-218">• Access support</span></span>












