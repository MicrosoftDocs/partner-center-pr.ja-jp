---
title: ユーザー ロールとアクセス許可の割り当て |パートナー センター
ms.topic: article
ms.date: 10/10/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 商取引、紹介、インセンティブ、または会社の MPN メンバーシップを管理しているユーザーに最適なロールについて説明します。
author: LauraBrenner
ms.author: labrenne
keywords: ロール, アクセス許可, 管理者, エージェント
ms.localizationpriority: high
ms.openlocfilehash: e0f53e2f1aae51a1287a2e347fa9014b5d75ea03
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004131"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="34ba7-104">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="34ba7-104">Assign users roles and permissions</span></span>

<span data-ttu-id="34ba7-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="34ba7-105">**Appropriate roles**</span></span>
-   <span data-ttu-id="34ba7-106">全体管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-106">Global admin</span></span>
-   <span data-ttu-id="34ba7-107">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-107">User admin</span></span>
-   <span data-ttu-id="34ba7-108">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-108">MPN partner admin</span></span>

<span data-ttu-id="34ba7-109">貴社の正式名称や法的住所、サポートの詳細、税金の除外の申告、銀行情報、主要な連絡先など、パートナー プロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="34ba7-109">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="34ba7-110">次に、ユーザーにパスワードとロールを設定させて、ユーザーがパートナー センターでの作業を開始できるようにします。</span><span class="sxs-lookup"><span data-stu-id="34ba7-110">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="34ba7-111">パートナー センターで作業できるように従業員を設定する</span><span class="sxs-lookup"><span data-stu-id="34ba7-111">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="34ba7-112">ユーザーに付与するロールとアクセス許可によって、パートナー センターでのユーザーのアクセスの種類が決まります。</span><span class="sxs-lookup"><span data-stu-id="34ba7-112">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="34ba7-113">ロールは、貴社のビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="34ba7-113">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="34ba7-114">たとえば、貴社のビジネスがクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、グローバル管理者などの標準の Azure AD テナント管理ロールだけでなく、CSP プログラムに固有のロールも必要です。</span><span class="sxs-lookup"><span data-stu-id="34ba7-114">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="34ba7-115">各プログラムには、それに固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="34ba7-115">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="34ba7-116">Azure Active Directory (AAD) テナント ロールには、グローバル管理者、ユーザー管理者、および CSP のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="34ba7-116">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="34ba7-117">AAD 以外のロールはテナントを管理しないロールであり、MPN 管理者、ビジネス プロファイル管理者、紹介管理者、インセンティブ管理者、およびインセンティブ ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="34ba7-117">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="34ba7-118">パートナー センターで商取引を管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="34ba7-118">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="34ba7-119">**Role**</span><span class="sxs-lookup"><span data-stu-id="34ba7-119">**Role**</span></span>|<span data-ttu-id="34ba7-120">**できること**</span><span class="sxs-lookup"><span data-stu-id="34ba7-120">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="34ba7-121">全体管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-121">Global admin</span></span>|<span data-ttu-id="34ba7-122">• すべての特権を備えたすべての Microsoft アカウント/サービスへのアクセス</span><span class="sxs-lookup"><span data-stu-id="34ba7-122">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="34ba7-123">• パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="34ba7-123">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="34ba7-124">• 契約、価格表、キャンペーンの表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-124">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="34ba7-125">• パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-125">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="34ba7-126">課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="34ba7-127">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-127">User management admin</span></span>   | <span data-ttu-id="34ba7-128">• ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-128">•    View, create, and manage users</span></span>
||<span data-ttu-id="34ba7-129">• すべてのパートナー プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-129">• View all partner profiles</span></span>
||<span data-ttu-id="34ba7-130">• パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-130">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="34ba7-131">課金の管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-131">Billing admin</span></span> | <span data-ttu-id="34ba7-132">- 課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-132">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="34ba7-133">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="34ba7-133">Default user</span></span>|  <span data-ttu-id="34ba7-134">マイ プロフィールの表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-134">View My profile</span></span>   |
|<span data-ttu-id="34ba7-135">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="34ba7-135">Admin agent</span></span> | <span data-ttu-id="34ba7-136">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-136">•    Customer management</span></span>
||<span data-ttu-id="34ba7-137">• パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="34ba7-137">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="34ba7-138">• プロファイルの作成とデバイスへの適用</span><span class="sxs-lookup"><span data-stu-id="34ba7-138">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="34ba7-139">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-139">• Subscription management</span></span>
||<span data-ttu-id="34ba7-140">• 顧客のためのサービスの正常性の確認とサービス要求</span><span class="sxs-lookup"><span data-stu-id="34ba7-140">• Service health and service requests for customers</span></span>
||<span data-ttu-id="34ba7-141">• 代理管理者特権の要求</span><span class="sxs-lookup"><span data-stu-id="34ba7-141">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="34ba7-142">• 価格とプランの表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-142">• View pricing and offers</span></span>
||<span data-ttu-id="34ba7-143">• 請求</span><span class="sxs-lookup"><span data-stu-id="34ba7-143">• Billing</span></span>
||<span data-ttu-id="34ba7-144">• 顧客の代理としての管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-144">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="34ba7-145">• 付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="34ba7-145">• Register a value added reseller</span></span>|
|<span data-ttu-id="34ba7-146">販売代理店</span><span class="sxs-lookup"><span data-stu-id="34ba7-146">Sales agent</span></span> | <span data-ttu-id="34ba7-147">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-147">•    Customer management</span></span>
||<span data-ttu-id="34ba7-148">• パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="34ba7-148">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="34ba7-149">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-149">• Subscription management</span></span>
||<span data-ttu-id="34ba7-150">• サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-150">• View support tickets</span></span>
||<span data-ttu-id="34ba7-151">• 顧客との再販業者関係の要求</span><span class="sxs-lookup"><span data-stu-id="34ba7-151">• Request a relationship with a customer</span></span>
||<span data-ttu-id="34ba7-152">• 見込み客の管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-152">• Manage customer leads</span></span>
||<span data-ttu-id="34ba7-153">• 顧客契約の表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-153">• View the customer agreement</span></span>
||<span data-ttu-id="34ba7-154">• 付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="34ba7-154">• Register a value-added reseller</span></span>|
|<span data-ttu-id="34ba7-155">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="34ba7-155">Helpdesk agent</span></span>| <span data-ttu-id="34ba7-156">• 顧客の検索と表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-156">•  Search for and view a customer</span></span>
||<span data-ttu-id="34ba7-157">• 顧客の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="34ba7-157">• Edit customer details</span></span>
||<span data-ttu-id="34ba7-158">• 請求やサブスクリプション管理に関する顧客の問題の解決サポート</span><span class="sxs-lookup"><span data-stu-id="34ba7-158">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="34ba7-159">• 顧客の代理としてのサポート要求 (注: Office 365 サブスクリプションの場合、このタスクを完了するには管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="34ba7-159">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="34ba7-160">• 顧客の代理としてのサブスクリプションとサービスの管理 (注: Office 365 サブスクリプションの場合、このタスクを完了するには管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="34ba7-160">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="34ba7-161">コントロール パネル ベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="34ba7-161">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="34ba7-162">(CSP ロールと非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="34ba7-162">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="34ba7-163">CPV は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムとパートナー センター API を統合するために使用するアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="34ba7-163">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="34ba7-164">**Role**</span><span class="sxs-lookup"><span data-stu-id="34ba7-164">**Role**</span></span>   |<span data-ttu-id="34ba7-165">**できること**</span><span class="sxs-lookup"><span data-stu-id="34ba7-165">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="34ba7-166">全体管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-166">Global admin</span></span>| <span data-ttu-id="34ba7-167">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-167">View and manage your CPV profile</span></span>|
||<span data-ttu-id="34ba7-168">CPV 機能にアクセスする必要があるユーザーの表示と管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-168">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="34ba7-169">ゲスト ユーザー (AAD テナントに追加される必要があります)</span><span class="sxs-lookup"><span data-stu-id="34ba7-169">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="34ba7-170">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="34ba7-170">**Guest user**</span></span>   | <span data-ttu-id="34ba7-171">**ロール**</span><span class="sxs-lookup"><span data-stu-id="34ba7-171">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="34ba7-172">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-172">MPN partner admin</span></span>|
||<span data-ttu-id="34ba7-173">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-173">Accounts admin</span></span>|
||<span data-ttu-id="34ba7-174">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-174">Incentives admin</span></span>|
||<span data-ttu-id="34ba7-175">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-175">Business profile admin</span></span>|
||<span data-ttu-id="34ba7-176">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-176">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="34ba7-177">MPN メンバーシップと会社の管理 (AAD 以外のロール: これらのロールは、テナントではなく会社の業務を管理します)</span><span class="sxs-lookup"><span data-stu-id="34ba7-177">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="34ba7-178">**Role**</span><span class="sxs-lookup"><span data-stu-id="34ba7-178">**Role**</span></span> | <span data-ttu-id="34ba7-179">**できること**</span><span class="sxs-lookup"><span data-stu-id="34ba7-179">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="34ba7-180">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-180">MPN partner admin</span></span>|<span data-ttu-id="34ba7-181">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-181">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="34ba7-182">• 法的プロファイル、企業プロファイル、ビジネス プロファイル、MPN プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-182">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="34ba7-183">• ユーザーの詳細およびスキル データの表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-183">• View user details and their skills data</span></span>
||<span data-ttu-id="34ba7-184">• コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-184">• View competencies</span></span>
||<span data-ttu-id="34ba7-185">• 特典の表示と管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-185">• View and manage benefits</span></span>
||<span data-ttu-id="34ba7-186">• MPN オファーの表示と購入</span><span class="sxs-lookup"><span data-stu-id="34ba7-186">• View and purchase MPN offers</span></span>
||<span data-ttu-id="34ba7-187">• MPN オファーの注文履歴と請求書の表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-187">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="34ba7-188">• パートナー貢献度インジケーター データの表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-188">• View partner contribution indicator data</span></span>
||<span data-ttu-id="34ba7-189">• 利用券検証ツールでの作業</span><span class="sxs-lookup"><span data-stu-id="34ba7-189">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="34ba7-190">- 顧客データ分析の表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-190">- View customer data analytics</span></span>
|| <span data-ttu-id="34ba7-191">会社内の他のユーザー ロールを表示しますが、ロールを割り当てることはできません</span><span class="sxs-lookup"><span data-stu-id="34ba7-191">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="34ba7-192">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-192">Account admin</span></span>| <span data-ttu-id="34ba7-193">場所の追加</span><span class="sxs-lookup"><span data-stu-id="34ba7-193">Add locations</span></span>
|| <span data-ttu-id="34ba7-194">管理対象のアカウントに関連するプロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-194">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="34ba7-195">• テナント内のユーザーに対するロールの非 AAD ロールへの割り当て</span><span class="sxs-lookup"><span data-stu-id="34ba7-195">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="34ba7-196">• プログラムへの場所の登録</span><span class="sxs-lookup"><span data-stu-id="34ba7-196">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="34ba7-197">紹介の管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-197">Manage referrals</span></span> 

|<span data-ttu-id="34ba7-198">**Role**</span><span class="sxs-lookup"><span data-stu-id="34ba7-198">**Role**</span></span>|<span data-ttu-id="34ba7-199">**できること**</span><span class="sxs-lookup"><span data-stu-id="34ba7-199">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="34ba7-200">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-200">Referrals admin</span></span>       |<span data-ttu-id="34ba7-201">• ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-201">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="34ba7-202">• 紹介案件の受信と管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-202">• Receive and manage referrals</span></span>
||<span data-ttu-id="34ba7-203">• 共同販売の紹介の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-203">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="34ba7-204">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-204">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="34ba7-205">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-205">Business profile admin</span></span>   |<span data-ttu-id="34ba7-206">• ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-206">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="34ba7-207">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-207">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="34ba7-208">インセンティブの管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-208">Manage incentives</span></span> 

|<span data-ttu-id="34ba7-209">**Role**</span><span class="sxs-lookup"><span data-stu-id="34ba7-209">**Role**</span></span> | <span data-ttu-id="34ba7-210">**できること**</span><span class="sxs-lookup"><span data-stu-id="34ba7-210">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="34ba7-211">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="34ba7-211">Incentives admin</span></span>|<span data-ttu-id="34ba7-212">• インセンティブの開始と管理</span><span class="sxs-lookup"><span data-stu-id="34ba7-212">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="34ba7-213">• インセンティブ プログラムのすべての側面の表示と編集</span><span class="sxs-lookup"><span data-stu-id="34ba7-213">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="34ba7-214">• 銀行および税の詳細情報の表示と編集</span><span class="sxs-lookup"><span data-stu-id="34ba7-214">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="34ba7-215">• リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-215">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="34ba7-216">• サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="34ba7-216">• Access support</span></span>
||<span data-ttu-id="34ba7-217">• インセンティブ支払いについての議論</span><span class="sxs-lookup"><span data-stu-id="34ba7-217">• Dispute incentives payments</span></span>|
|<span data-ttu-id="34ba7-218">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="34ba7-218">Incentives user</span></span>|<span data-ttu-id="34ba7-219">• インセンティブ プログラムの表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-219">•  Can view incentives programs</span></span>
||<span data-ttu-id="34ba7-220">• インセンティブの申請の表示と開始</span><span class="sxs-lookup"><span data-stu-id="34ba7-220">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="34ba7-221">• リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="34ba7-221">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="34ba7-222">• サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="34ba7-222">• Access support</span></span>












