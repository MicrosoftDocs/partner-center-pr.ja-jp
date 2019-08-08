---
title: ユーザー ロールとアクセス許可の割り当て |パートナー センター
ms.topic: article
ms.date: 3/5/2019
description: パートナー センターで作業する必要があるすべての従業員にロールを割り当てる必要があります。
author: LauraBrenner
ms.author: labrenne
keywords: ロール, アクセス許可, 管理者, エージェント
ms.localizationpriority: medium
ms.openlocfilehash: 744ce84c47d3adaf21d8f7b790001737d6489cdb
ms.sourcegitcommit: 9d01fb30eafc523784ecc3568c05da9bbe9a1e8c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/01/2019
ms.locfileid: "68708864"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="7d05c-104">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="7d05c-104">Assign users roles and permissions</span></span>


<span data-ttu-id="7d05c-105">貴社の正式名称や法的住所、サポートの詳細、税金の除外の申告、銀行情報、主要な連絡先など、パートナー プロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="7d05c-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="7d05c-106">次に、ユーザーにパスワードとロールを設定させて、ユーザーがパートナー センターでの作業を開始できるようにします。</span><span class="sxs-lookup"><span data-stu-id="7d05c-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="7d05c-107">パートナー センターで作業できるように従業員を設定する</span><span class="sxs-lookup"><span data-stu-id="7d05c-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="7d05c-108">ユーザーに付与するロールとアクセス許可によって、パートナー センターでのユーザーのアクセスの種類が決まります。</span><span class="sxs-lookup"><span data-stu-id="7d05c-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="7d05c-109">ロールは、貴社のビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="7d05c-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="7d05c-110">たとえば、貴社のビジネスがクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、グローバル管理者などの標準の Azure AD テナント管理ロールだけでなく、CSP プログラムに固有のロールも必要です。</span><span class="sxs-lookup"><span data-stu-id="7d05c-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="7d05c-111">各プログラムには、それに固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="7d05c-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="7d05c-112">Azure Active Directory (AAD) テナント ロールには、グローバル管理者、ユーザー管理者、および CSP のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="7d05c-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="7d05c-113">非 AAD ロールとは、テナントを管理しないロールのことで、MPN admin、business profile admin、推薦 admin、インセンティブ管理者、インセンティブユーザーなどが含まれます。</span><span class="sxs-lookup"><span data-stu-id="7d05c-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="7d05c-114">パートナー センターで商取引を管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="7d05c-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="7d05c-115">**ロール**</span><span class="sxs-lookup"><span data-stu-id="7d05c-115">**Role**</span></span>|<span data-ttu-id="7d05c-116">**できること**</span><span class="sxs-lookup"><span data-stu-id="7d05c-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="7d05c-117">全体管理者</span><span class="sxs-lookup"><span data-stu-id="7d05c-117">Global admin</span></span>|<span data-ttu-id="7d05c-118">• すべての特権を備えたすべての Microsoft アカウント/サービスへのアクセス</span><span class="sxs-lookup"><span data-stu-id="7d05c-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="7d05c-119">• パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="7d05c-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7d05c-120">• 契約、価格表、キャンペーンの表示</span><span class="sxs-lookup"><span data-stu-id="7d05c-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="7d05c-121">• パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="7d05c-122">課金、請求書、および偵察ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="7d05c-123">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="7d05c-123">User management admin</span></span>   | <span data-ttu-id="7d05c-124">•ユーザーの表示、作成、および管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="7d05c-125">• すべてのパートナー プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="7d05c-125">• View all partner profiles</span></span>
||<span data-ttu-id="7d05c-126">• パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="7d05c-127">課金の管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-127">Billing admin</span></span> | <span data-ttu-id="7d05c-128">- 課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="7d05c-129">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="7d05c-129">Default user</span></span>|  <span data-ttu-id="7d05c-130">マイ プロフィールの表示</span><span class="sxs-lookup"><span data-stu-id="7d05c-130">View My profile</span></span>   |
|<span data-ttu-id="7d05c-131">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="7d05c-131">Admin agent</span></span> | <span data-ttu-id="7d05c-132">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-132">•    Customer management</span></span>
||<span data-ttu-id="7d05c-133">• パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="7d05c-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="7d05c-134">• プロファイルの作成とデバイスへの適用</span><span class="sxs-lookup"><span data-stu-id="7d05c-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="7d05c-135">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-135">• Subscription management</span></span>
||<span data-ttu-id="7d05c-136">• 顧客のためのサービスの正常性の確認とサービス要求</span><span class="sxs-lookup"><span data-stu-id="7d05c-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="7d05c-137">• 代理管理者特権の要求</span><span class="sxs-lookup"><span data-stu-id="7d05c-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="7d05c-138">• 価格とプランの表示</span><span class="sxs-lookup"><span data-stu-id="7d05c-138">• View pricing and offers</span></span>
||<span data-ttu-id="7d05c-139">• 請求</span><span class="sxs-lookup"><span data-stu-id="7d05c-139">• Billing</span></span>
||<span data-ttu-id="7d05c-140">• 顧客の代理としての管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="7d05c-141">• 付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="7d05c-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="7d05c-142">販売代理店</span><span class="sxs-lookup"><span data-stu-id="7d05c-142">Sales agent</span></span> | <span data-ttu-id="7d05c-143">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-143">•    Customer management</span></span>
||<span data-ttu-id="7d05c-144">• パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="7d05c-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="7d05c-145">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-145">• Subscription management</span></span>
||<span data-ttu-id="7d05c-146">•価格リストとプランの表示</span><span class="sxs-lookup"><span data-stu-id="7d05c-146">• View price lists and offers</span></span>
||<span data-ttu-id="7d05c-147">• サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="7d05c-147">• View support tickets</span></span>
||<span data-ttu-id="7d05c-148">• 顧客との再販業者関係の要求</span><span class="sxs-lookup"><span data-stu-id="7d05c-148">• Request a relationship with a customer</span></span>
||<span data-ttu-id="7d05c-149">• 見込み客の管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-149">• Manage customer leads</span></span>
||<span data-ttu-id="7d05c-150">• 顧客契約の表示</span><span class="sxs-lookup"><span data-stu-id="7d05c-150">• View the customer agreement</span></span>
||<span data-ttu-id="7d05c-151">• 付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="7d05c-151">• Register a value-added reseller</span></span>|
|<span data-ttu-id="7d05c-152">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="7d05c-152">Helpdesk agent</span></span>| <span data-ttu-id="7d05c-153">• 顧客の検索と表示</span><span class="sxs-lookup"><span data-stu-id="7d05c-153">•  Search for and view a customer</span></span>
||<span data-ttu-id="7d05c-154">• 顧客の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="7d05c-154">• Edit customer details</span></span>
||<span data-ttu-id="7d05c-155">• 請求やサブスクリプション管理に関する顧客の問題の解決サポート</span><span class="sxs-lookup"><span data-stu-id="7d05c-155">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="7d05c-156">• 顧客の代理としてのサポート要求 (注: Office 365 サブスクリプションの場合、このタスクを完了するには管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="7d05c-156">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="7d05c-157">• 顧客の代理としてのサブスクリプションとサービスの管理 (注: Office 365 サブスクリプションの場合、このタスクを完了するには管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="7d05c-157">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="7d05c-158">コントロール パネル ベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="7d05c-158">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="7d05c-159">(CSP ロールと非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="7d05c-159">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="7d05c-160">CPV は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムとパートナー センター API を統合するために使用するアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="7d05c-160">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="7d05c-161">**ロール**</span><span class="sxs-lookup"><span data-stu-id="7d05c-161">**Role**</span></span>   |<span data-ttu-id="7d05c-162">**できること**</span><span class="sxs-lookup"><span data-stu-id="7d05c-162">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="7d05c-163">全体管理者</span><span class="sxs-lookup"><span data-stu-id="7d05c-163">Global admin</span></span>| <span data-ttu-id="7d05c-164">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-164">View and manage your CPV profile</span></span>|
||<span data-ttu-id="7d05c-165">CPV 機能にアクセスする必要があるユーザーの表示と管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-165">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="7d05c-166">ゲスト ユーザー (AAD テナントに追加される必要があります)</span><span class="sxs-lookup"><span data-stu-id="7d05c-166">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="7d05c-167">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="7d05c-167">**Guest user**</span></span>   | <span data-ttu-id="7d05c-168">**ロール**</span><span class="sxs-lookup"><span data-stu-id="7d05c-168">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="7d05c-169">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="7d05c-169">MPN partner admin</span></span>|
||<span data-ttu-id="7d05c-170">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="7d05c-170">Accounts admin</span></span>|
||<span data-ttu-id="7d05c-171">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="7d05c-171">Incentives admin</span></span>|
||<span data-ttu-id="7d05c-172">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="7d05c-172">Business profile admin</span></span>|
||<span data-ttu-id="7d05c-173">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="7d05c-173">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="7d05c-174">MPN のメンバーシップと会社の管理 (AAD 以外のロール: これらのロールは、テナントではなく会社のビジネスを管理します)</span><span class="sxs-lookup"><span data-stu-id="7d05c-174">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="7d05c-175">**ロール**</span><span class="sxs-lookup"><span data-stu-id="7d05c-175">**Role**</span></span> | <span data-ttu-id="7d05c-176">**できること**</span><span class="sxs-lookup"><span data-stu-id="7d05c-176">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="7d05c-177">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="7d05c-177">MPN partner admin</span></span>|<span data-ttu-id="7d05c-178">•パートナーサービス要求を表示、作成、管理します</span><span class="sxs-lookup"><span data-stu-id="7d05c-178">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="7d05c-179">•法律、会社、ビジネス、および MPN のプロファイルを表示する</span><span class="sxs-lookup"><span data-stu-id="7d05c-179">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="7d05c-180">• ユーザーの詳細およびスキル データの表示</span><span class="sxs-lookup"><span data-stu-id="7d05c-180">• View user details and their skills data</span></span>
||<span data-ttu-id="7d05c-181">• コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="7d05c-181">• View competencies</span></span>
||<span data-ttu-id="7d05c-182">• 特典の表示と管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-182">• View and manage benefits</span></span>
||<span data-ttu-id="7d05c-183">• MPN オファーの表示と購入</span><span class="sxs-lookup"><span data-stu-id="7d05c-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="7d05c-184">• MPN オファーの注文履歴と請求書の表示</span><span class="sxs-lookup"><span data-stu-id="7d05c-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="7d05c-185">•パートナー貢献度インジケーターデータを表示する</span><span class="sxs-lookup"><span data-stu-id="7d05c-185">• View partner contribution indicator data</span></span>
||<span data-ttu-id="7d05c-186">• 利用券検証ツールでの作業</span><span class="sxs-lookup"><span data-stu-id="7d05c-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="7d05c-187">- 顧客データ分析の表示</span><span class="sxs-lookup"><span data-stu-id="7d05c-187">- View customer data analytics</span></span>
|| <span data-ttu-id="7d05c-188">会社内の他のユーザーロールを表示しますが、ロールを割り当てることはできません</span><span class="sxs-lookup"><span data-stu-id="7d05c-188">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="7d05c-189">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="7d05c-189">Account admin</span></span>| <span data-ttu-id="7d05c-190">場所の追加</span><span class="sxs-lookup"><span data-stu-id="7d05c-190">Add locations</span></span>
|| <span data-ttu-id="7d05c-191">管理者のアカウントに関連するプロファイルを管理する</span><span class="sxs-lookup"><span data-stu-id="7d05c-191">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="7d05c-192">• テナント内のユーザーに対するロールの非 AAD ロールへの割り当て</span><span class="sxs-lookup"><span data-stu-id="7d05c-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="7d05c-193">• プログラムへの場所の登録</span><span class="sxs-lookup"><span data-stu-id="7d05c-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="7d05c-194">参照の管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-194">Manage referrals</span></span> 

|<span data-ttu-id="7d05c-195">**ロール**</span><span class="sxs-lookup"><span data-stu-id="7d05c-195">**Role**</span></span>|<span data-ttu-id="7d05c-196">**できること**</span><span class="sxs-lookup"><span data-stu-id="7d05c-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="7d05c-197">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="7d05c-197">Referrals admin</span></span>       |<span data-ttu-id="7d05c-198">• ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="7d05c-199">• 紹介案件の受信と管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="7d05c-200">•共同販売参照の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="7d05c-201">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="7d05c-202">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="7d05c-202">Business profile admin</span></span>   |<span data-ttu-id="7d05c-203">•ビジネスプロファイルの表示、作成、および管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="7d05c-204">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="7d05c-205">インセンティブの管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-205">Manage incentives</span></span> 

|<span data-ttu-id="7d05c-206">**ロール**</span><span class="sxs-lookup"><span data-stu-id="7d05c-206">**Role**</span></span> | <span data-ttu-id="7d05c-207">**できること**</span><span class="sxs-lookup"><span data-stu-id="7d05c-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="7d05c-208">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="7d05c-208">Incentives admin</span></span>|<span data-ttu-id="7d05c-209">• インセンティブの開始と管理</span><span class="sxs-lookup"><span data-stu-id="7d05c-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="7d05c-210">• インセンティブ プログラムのすべての側面の表示と編集</span><span class="sxs-lookup"><span data-stu-id="7d05c-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="7d05c-211">• 銀行および税の詳細情報の表示と編集</span><span class="sxs-lookup"><span data-stu-id="7d05c-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="7d05c-212">• リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="7d05c-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="7d05c-213">• サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="7d05c-213">• Access support</span></span>
||<span data-ttu-id="7d05c-214">• インセンティブ支払いについての議論</span><span class="sxs-lookup"><span data-stu-id="7d05c-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="7d05c-215">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="7d05c-215">Incentives user</span></span>|<span data-ttu-id="7d05c-216">• インセンティブ プログラムの表示</span><span class="sxs-lookup"><span data-stu-id="7d05c-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="7d05c-217">• インセンティブの申請の表示と開始</span><span class="sxs-lookup"><span data-stu-id="7d05c-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="7d05c-218">• リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="7d05c-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="7d05c-219">• サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="7d05c-219">• Access support</span></span>












