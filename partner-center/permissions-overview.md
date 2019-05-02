---
title: ユーザー ロールとアクセス許可の割り当て |パートナー センター
ms.topic: article
ms.date: 3/5/19
description: パートナー センターで作業する必要があるすべての従業員にロールを割り当てる必要があります。
author: LauraBrenner
ms.author: labrenne
keywords: ロール, アクセス許可, 管理者, エージェント
ms.localizationpriority: medium
ms.openlocfilehash: 66923c8a5d4912d178ef483a883f08f40ed8378b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133902"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="d9234-104">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="d9234-104">Assign users roles and permissions</span></span>


<span data-ttu-id="d9234-105">貴社の正式名称や法的住所、サポートの詳細、税金の除外の申告、銀行情報、主要な連絡先など、パートナー プロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="d9234-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="d9234-106">次に、ユーザーにパスワードとロールを設定させて、ユーザーがパートナー センターでの作業を開始できるようにします。</span><span class="sxs-lookup"><span data-stu-id="d9234-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="d9234-107">パートナー センターで作業できるように従業員を設定する</span><span class="sxs-lookup"><span data-stu-id="d9234-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="d9234-108">ユーザーに付与するロールとアクセス許可によって、パートナー センターでのユーザーのアクセスの種類が決まります。</span><span class="sxs-lookup"><span data-stu-id="d9234-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="d9234-109">ロールは、貴社のビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="d9234-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="d9234-110">たとえば、貴社のビジネスがクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、グローバル管理者などの標準の Azure AD テナント管理ロールだけでなく、CSP プログラムに固有のロールも必要です。</span><span class="sxs-lookup"><span data-stu-id="d9234-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="d9234-111">各プログラムには、それに固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="d9234-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="d9234-112">Azure Active Directory (AAD) テナント ロールには、グローバル管理者、ユーザー管理者、および CSP のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="d9234-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="d9234-113">AAD 以外のロールには、MPN 管理者、ビジネス プロファイル管理者、紹介管理者、インセンティブ管理者、インセンティブ ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="d9234-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="d9234-114">パートナー センターで商取引を管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="d9234-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="d9234-115">**Role**</span><span class="sxs-lookup"><span data-stu-id="d9234-115">**Role**</span></span>|<span data-ttu-id="d9234-116">**できること**</span><span class="sxs-lookup"><span data-stu-id="d9234-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="d9234-117">全体管理者</span><span class="sxs-lookup"><span data-stu-id="d9234-117">Global admin</span></span>|<span data-ttu-id="d9234-118">• すべての特権を備えたすべての Microsoft アカウント/サービスへのアクセス</span><span class="sxs-lookup"><span data-stu-id="d9234-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="d9234-119">• パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="d9234-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="d9234-120">• 契約、価格表、キャンペーンの表示</span><span class="sxs-lookup"><span data-stu-id="d9234-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="d9234-121">• パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d9234-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="d9234-122">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="d9234-122">User Admin</span></span>   | <span data-ttu-id="d9234-123">• ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d9234-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="d9234-124">• すべてのパートナー プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="d9234-124">• View all partner profiles</span></span>
||<span data-ttu-id="d9234-125">• パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d9234-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="d9234-126">課金の管理</span><span class="sxs-lookup"><span data-stu-id="d9234-126">Billing admin</span></span> | <span data-ttu-id="d9234-127">- 課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d9234-127">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="d9234-128">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="d9234-128">Default user</span></span>|  <span data-ttu-id="d9234-129">マイ プロフィールの表示</span><span class="sxs-lookup"><span data-stu-id="d9234-129">View My profile</span></span>   |
|<span data-ttu-id="d9234-130">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="d9234-130">Admin agent</span></span> | <span data-ttu-id="d9234-131">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="d9234-131">•    Customer management</span></span>
||<span data-ttu-id="d9234-132">• パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="d9234-132">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="d9234-133">• プロファイルの作成とデバイスへの適用</span><span class="sxs-lookup"><span data-stu-id="d9234-133">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="d9234-134">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="d9234-134">• Subscription management</span></span>
||<span data-ttu-id="d9234-135">• 顧客のためのサービスの正常性の確認とサービス要求</span><span class="sxs-lookup"><span data-stu-id="d9234-135">• Service health and service requests for customers</span></span>
||<span data-ttu-id="d9234-136">• 代理管理者特権の要求</span><span class="sxs-lookup"><span data-stu-id="d9234-136">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="d9234-137">• 価格とプランの表示</span><span class="sxs-lookup"><span data-stu-id="d9234-137">• View pricing and offers</span></span>
||<span data-ttu-id="d9234-138">• 請求</span><span class="sxs-lookup"><span data-stu-id="d9234-138">• Billing</span></span>
||<span data-ttu-id="d9234-139">• 顧客の代理としての管理</span><span class="sxs-lookup"><span data-stu-id="d9234-139">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="d9234-140">• 付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="d9234-140">• Register a value added reseller</span></span>|
|<span data-ttu-id="d9234-141">販売代理店</span><span class="sxs-lookup"><span data-stu-id="d9234-141">Sales agent</span></span> | <span data-ttu-id="d9234-142">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="d9234-142">•    Customer management</span></span>
||<span data-ttu-id="d9234-143">• パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="d9234-143">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="d9234-144">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="d9234-144">• Subscription management</span></span>
||<span data-ttu-id="d9234-145">• サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="d9234-145">• View support tickets</span></span>
||<span data-ttu-id="d9234-146">• 顧客との再販業者関係の要求</span><span class="sxs-lookup"><span data-stu-id="d9234-146">• Request a relationship with a customer</span></span>
||<span data-ttu-id="d9234-147">• 見込み客の管理</span><span class="sxs-lookup"><span data-stu-id="d9234-147">• Manage customer leads</span></span>
||<span data-ttu-id="d9234-148">• 顧客契約の表示</span><span class="sxs-lookup"><span data-stu-id="d9234-148">• View the customer agreement</span></span>
||<span data-ttu-id="d9234-149">• 付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="d9234-149">• Register a value-added reseller</span></span>|
|<span data-ttu-id="d9234-150">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="d9234-150">Helpdesk agent</span></span>| <span data-ttu-id="d9234-151">• 顧客の検索と表示</span><span class="sxs-lookup"><span data-stu-id="d9234-151">•  Search for and view a customer</span></span>
||<span data-ttu-id="d9234-152">• 顧客の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="d9234-152">• Edit customer details</span></span>
||<span data-ttu-id="d9234-153">• 請求やサブスクリプション管理に関する顧客の問題の解決サポート</span><span class="sxs-lookup"><span data-stu-id="d9234-153">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="d9234-154">• 顧客の代理としてのサポート要求 (注: Office 365 サブスクリプションの場合、このタスクを完了するには管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="d9234-154">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="d9234-155">• 顧客の代理としてのサブスクリプションとサービスの管理 (注: Office 365 サブスクリプションの場合、このタスクを完了するには管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="d9234-155">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="d9234-156">コントロール パネル ベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="d9234-156">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="d9234-157">(CSP ロールと非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="d9234-157">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="d9234-158">CPV は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムとパートナー センター API を統合するために使用するアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="d9234-158">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="d9234-159">**Role**</span><span class="sxs-lookup"><span data-stu-id="d9234-159">**Role**</span></span>   |<span data-ttu-id="d9234-160">**できること**</span><span class="sxs-lookup"><span data-stu-id="d9234-160">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="d9234-161">全体管理者</span><span class="sxs-lookup"><span data-stu-id="d9234-161">Global admin</span></span>| <span data-ttu-id="d9234-162">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="d9234-162">View and manage your CPV profile</span></span>|
||<span data-ttu-id="d9234-163">CPV 機能にアクセスする必要があるユーザーの表示と管理</span><span class="sxs-lookup"><span data-stu-id="d9234-163">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="d9234-164">MPN メンバーシップと貴社の管理 (非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="d9234-164">Manage MPN membership and your company (non-AAD roles)</span></span>

|<span data-ttu-id="d9234-165">**Role**</span><span class="sxs-lookup"><span data-stu-id="d9234-165">**Role**</span></span> | <span data-ttu-id="d9234-166">**できること**</span><span class="sxs-lookup"><span data-stu-id="d9234-166">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="d9234-167">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="d9234-167">MPN partner admin</span></span>|<span data-ttu-id="d9234-168">• 非テナントユーザーの追加</span><span class="sxs-lookup"><span data-stu-id="d9234-168">•Can add non-tenant users</span></span>
||<span data-ttu-id="d9234-169">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d9234-169">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="d9234-170">• 法的プロファイル、組織プロファイル、ビジネス プロファイル、MPN プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="d9234-170">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="d9234-171">• ユーザーの詳細およびスキル データの表示</span><span class="sxs-lookup"><span data-stu-id="d9234-171">• View user details and their skills data</span></span>
||<span data-ttu-id="d9234-172">• コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="d9234-172">• View competencies</span></span>
||<span data-ttu-id="d9234-173">• 特典の表示と管理</span><span class="sxs-lookup"><span data-stu-id="d9234-173">• View and manage benefits</span></span>
||<span data-ttu-id="d9234-174">• MPN オファーの表示と購入</span><span class="sxs-lookup"><span data-stu-id="d9234-174">• View and purchase MPN offers</span></span>
||<span data-ttu-id="d9234-175">• MPN オファーの注文履歴と請求書の表示</span><span class="sxs-lookup"><span data-stu-id="d9234-175">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="d9234-176">• パートナーの貢献度データの表示</span><span class="sxs-lookup"><span data-stu-id="d9234-176">• View partner contribution data</span></span>
||<span data-ttu-id="d9234-177">• 利用券検証ツールでの作業</span><span class="sxs-lookup"><span data-stu-id="d9234-177">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="d9234-178">- 顧客データ分析の表示</span><span class="sxs-lookup"><span data-stu-id="d9234-178">- View customer data analytics</span></span>
|<span data-ttu-id="d9234-179">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="d9234-179">Account admin</span></span>| <span data-ttu-id="d9234-180">• 非テナントユーザーの追加</span><span class="sxs-lookup"><span data-stu-id="d9234-180">•   Can add non-tenant users</span></span>
||<span data-ttu-id="d9234-181">• 場所の追加または削除</span><span class="sxs-lookup"><span data-stu-id="d9234-181">• Add or delete locations</span></span>
||<span data-ttu-id="d9234-182">- 管理対象のアカウントに関連するプロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="d9234-182">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="d9234-183">• テナント内のユーザーに対するロールの非 AAD ロールへの割り当て</span><span class="sxs-lookup"><span data-stu-id="d9234-183">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="d9234-184">• プログラムへの場所の登録</span><span class="sxs-lookup"><span data-stu-id="d9234-184">• Enroll locations into programs</span></span>

## <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="d9234-185">ゲスト ユーザー (AAD テナントに追加される必要があります)</span><span class="sxs-lookup"><span data-stu-id="d9234-185">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="d9234-186">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="d9234-186">**Guest user**</span></span>   | <span data-ttu-id="d9234-187">**ロール**</span><span class="sxs-lookup"><span data-stu-id="d9234-187">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="d9234-188">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="d9234-188">MPN partner admin</span></span>|
||<span data-ttu-id="d9234-189">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="d9234-189">Accounts admin</span></span>|
||<span data-ttu-id="d9234-190">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="d9234-190">Incentives admin</span></span>|
||<span data-ttu-id="d9234-191">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="d9234-191">Business profile admin</span></span>|
||<span data-ttu-id="d9234-192">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="d9234-192">Referrals admin</span></span>|


## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="d9234-193">紹介の管理 (非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="d9234-193">Manage referrals (non-AAD roles)</span></span>

|<span data-ttu-id="d9234-194">**Role**</span><span class="sxs-lookup"><span data-stu-id="d9234-194">**Role**</span></span>|<span data-ttu-id="d9234-195">**できること**</span><span class="sxs-lookup"><span data-stu-id="d9234-195">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="d9234-196">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="d9234-196">Referrals admin</span></span>       |<span data-ttu-id="d9234-197">• ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d9234-197">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="d9234-198">• 紹介案件の受信と管理</span><span class="sxs-lookup"><span data-stu-id="d9234-198">• Receive and manage referrals</span></span>
||<span data-ttu-id="d9234-199">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d9234-199">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="d9234-200">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="d9234-200">Business profile admin</span></span>   |<span data-ttu-id="d9234-201">• ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d9234-201">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="d9234-202">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d9234-202">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="d9234-203">インセンティブの管理 (非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="d9234-203">Manage Incentives  (non-AAD roles)</span></span>

|<span data-ttu-id="d9234-204">**Role**</span><span class="sxs-lookup"><span data-stu-id="d9234-204">**Role**</span></span> | <span data-ttu-id="d9234-205">**できること**</span><span class="sxs-lookup"><span data-stu-id="d9234-205">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="d9234-206">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="d9234-206">Incentives admin</span></span>|<span data-ttu-id="d9234-207">• インセンティブの開始と管理</span><span class="sxs-lookup"><span data-stu-id="d9234-207">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="d9234-208">• インセンティブ プログラムのすべての側面の表示と編集</span><span class="sxs-lookup"><span data-stu-id="d9234-208">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="d9234-209">• 銀行および税の詳細情報の表示と編集</span><span class="sxs-lookup"><span data-stu-id="d9234-209">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="d9234-210">• リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="d9234-210">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="d9234-211">• サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="d9234-211">• Access support</span></span>
||<span data-ttu-id="d9234-212">• インセンティブ支払いについての議論</span><span class="sxs-lookup"><span data-stu-id="d9234-212">• Dispute incentives payments</span></span>|
|<span data-ttu-id="d9234-213">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="d9234-213">Incentives user</span></span>|<span data-ttu-id="d9234-214">• インセンティブ プログラムの表示</span><span class="sxs-lookup"><span data-stu-id="d9234-214">•  Can view incentives programs</span></span>
||<span data-ttu-id="d9234-215">• インセンティブの申請の表示と開始</span><span class="sxs-lookup"><span data-stu-id="d9234-215">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="d9234-216">• リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="d9234-216">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="d9234-217">• リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="d9234-217">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="d9234-218">• サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="d9234-218">• Access support</span></span>












