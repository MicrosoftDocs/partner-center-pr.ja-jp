---
title: ユーザー ロールとアクセス許可の割り当て |パートナー センター
ms.topic: article
ms.date: 3/5/19
description: パートナー センターで作業する必要があるすべての従業員にロールを割り当てる必要があります。
author: LauraBrenner
ms.author: labrenne
keywords: ロール, アクセス許可, 管理者, エージェント
ms.localizationpriority: medium
ms.openlocfilehash: 658106548596a5fa7d02d29c0065a23caeacb83d
ms.sourcegitcommit: 59825cb626e12dfe5eb2d28e836b4573368d705e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/09/2019
ms.locfileid: "67690842"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="f962f-104">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="f962f-104">Assign users roles and permissions</span></span>


<span data-ttu-id="f962f-105">貴社の正式名称や法的住所、サポートの詳細、税金の除外の申告、銀行情報、主要な連絡先など、パートナー プロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="f962f-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="f962f-106">次に、ユーザーにパスワードとロールを設定させて、ユーザーがパートナー センターでの作業を開始できるようにします。</span><span class="sxs-lookup"><span data-stu-id="f962f-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="f962f-107">パートナー センターで作業できるように従業員を設定する</span><span class="sxs-lookup"><span data-stu-id="f962f-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="f962f-108">ユーザーに付与するロールとアクセス許可によって、パートナー センターでのユーザーのアクセスの種類が決まります。</span><span class="sxs-lookup"><span data-stu-id="f962f-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="f962f-109">ロールは、貴社のビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="f962f-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="f962f-110">たとえば、貴社のビジネスがクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、グローバル管理者などの標準の Azure AD テナント管理ロールだけでなく、CSP プログラムに固有のロールも必要です。</span><span class="sxs-lookup"><span data-stu-id="f962f-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="f962f-111">各プログラムには、それに固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="f962f-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="f962f-112">Azure Active Directory (AAD) テナント ロールには、グローバル管理者、ユーザー管理者、および CSP のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f962f-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="f962f-113">非 AAD のロールは、テナントを管理しないロールおよび MPN 管理者、ビジネス プロファイルの管理、参照の管理、インセンティブの管理者およびインセンティブのユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f962f-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="f962f-114">パートナー センターで商取引を管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="f962f-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="f962f-115">**ロール**</span><span class="sxs-lookup"><span data-stu-id="f962f-115">**Role**</span></span>|<span data-ttu-id="f962f-116">**できること**</span><span class="sxs-lookup"><span data-stu-id="f962f-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="f962f-117">全体管理者</span><span class="sxs-lookup"><span data-stu-id="f962f-117">Global admin</span></span>|<span data-ttu-id="f962f-118">• すべての特権を備えたすべての Microsoft アカウント/サービスへのアクセス</span><span class="sxs-lookup"><span data-stu-id="f962f-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="f962f-119">• パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="f962f-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="f962f-120">• 契約、価格表、キャンペーンの表示</span><span class="sxs-lookup"><span data-stu-id="f962f-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="f962f-121">• パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="f962f-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="f962f-122">表示、作成、および課金や請求書、recon ファイルを管理</span><span class="sxs-lookup"><span data-stu-id="f962f-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="f962f-123">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="f962f-123">User management admin</span></span>   | <span data-ttu-id="f962f-124">• ビューの作成、およびユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="f962f-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="f962f-125">• すべてのパートナー プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="f962f-125">• View all partner profiles</span></span>
||<span data-ttu-id="f962f-126">• パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="f962f-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="f962f-127">課金の管理</span><span class="sxs-lookup"><span data-stu-id="f962f-127">Billing admin</span></span> | <span data-ttu-id="f962f-128">- 課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="f962f-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="f962f-129">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="f962f-129">Default user</span></span>|  <span data-ttu-id="f962f-130">マイ プロフィールの表示</span><span class="sxs-lookup"><span data-stu-id="f962f-130">View My profile</span></span>   |
|<span data-ttu-id="f962f-131">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="f962f-131">Admin agent</span></span> | <span data-ttu-id="f962f-132">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="f962f-132">•    Customer management</span></span>
||<span data-ttu-id="f962f-133">• パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="f962f-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="f962f-134">• プロファイルの作成とデバイスへの適用</span><span class="sxs-lookup"><span data-stu-id="f962f-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="f962f-135">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="f962f-135">• Subscription management</span></span>
||<span data-ttu-id="f962f-136">• 顧客のためのサービスの正常性の確認とサービス要求</span><span class="sxs-lookup"><span data-stu-id="f962f-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="f962f-137">• 代理管理者特権の要求</span><span class="sxs-lookup"><span data-stu-id="f962f-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="f962f-138">• 価格とプランの表示</span><span class="sxs-lookup"><span data-stu-id="f962f-138">• View pricing and offers</span></span>
||<span data-ttu-id="f962f-139">• 請求</span><span class="sxs-lookup"><span data-stu-id="f962f-139">• Billing</span></span>
||<span data-ttu-id="f962f-140">• 顧客の代理としての管理</span><span class="sxs-lookup"><span data-stu-id="f962f-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="f962f-141">• 付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="f962f-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="f962f-142">販売代理店</span><span class="sxs-lookup"><span data-stu-id="f962f-142">Sales agent</span></span> | <span data-ttu-id="f962f-143">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="f962f-143">•    Customer management</span></span>
||<span data-ttu-id="f962f-144">• パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="f962f-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="f962f-145">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="f962f-145">• Subscription management</span></span>
||<span data-ttu-id="f962f-146">• 表示価格を一覧表示し、提供しています</span><span class="sxs-lookup"><span data-stu-id="f962f-146">• View price lists and offers</span></span>
||<span data-ttu-id="f962f-147">• サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="f962f-147">• View support tickets</span></span>
||<span data-ttu-id="f962f-148">• 顧客との再販業者関係の要求</span><span class="sxs-lookup"><span data-stu-id="f962f-148">• Request a relationship with a customer</span></span>
||<span data-ttu-id="f962f-149">• 見込み客の管理</span><span class="sxs-lookup"><span data-stu-id="f962f-149">• Manage customer leads</span></span>
||<span data-ttu-id="f962f-150">• 顧客契約の表示</span><span class="sxs-lookup"><span data-stu-id="f962f-150">• View the customer agreement</span></span>
||<span data-ttu-id="f962f-151">• 付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="f962f-151">• Register a value-added reseller</span></span>|
|<span data-ttu-id="f962f-152">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="f962f-152">Helpdesk agent</span></span>| <span data-ttu-id="f962f-153">• 顧客の検索と表示</span><span class="sxs-lookup"><span data-stu-id="f962f-153">•  Search for and view a customer</span></span>
||<span data-ttu-id="f962f-154">• 顧客の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="f962f-154">• Edit customer details</span></span>
||<span data-ttu-id="f962f-155">• 請求やサブスクリプション管理に関する顧客の問題の解決サポート</span><span class="sxs-lookup"><span data-stu-id="f962f-155">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="f962f-156">• 顧客の代理としてのサポート要求 (注: Office 365 サブスクリプションの場合、このタスクを完了するには管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="f962f-156">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="f962f-157">• 顧客の代理としてのサブスクリプションとサービスの管理 (注: Office 365 サブスクリプションの場合、このタスクを完了するには管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="f962f-157">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="f962f-158">コントロール パネル ベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="f962f-158">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="f962f-159">(CSP ロールと非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="f962f-159">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="f962f-160">CPV は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムとパートナー センター API を統合するために使用するアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="f962f-160">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="f962f-161">**ロール**</span><span class="sxs-lookup"><span data-stu-id="f962f-161">**Role**</span></span>   |<span data-ttu-id="f962f-162">**できること**</span><span class="sxs-lookup"><span data-stu-id="f962f-162">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="f962f-163">全体管理者</span><span class="sxs-lookup"><span data-stu-id="f962f-163">Global admin</span></span>| <span data-ttu-id="f962f-164">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="f962f-164">View and manage your CPV profile</span></span>|
||<span data-ttu-id="f962f-165">CPV 機能にアクセスする必要があるユーザーの表示と管理</span><span class="sxs-lookup"><span data-stu-id="f962f-165">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="f962f-166">ゲスト ユーザー (AAD テナントに追加される必要があります)</span><span class="sxs-lookup"><span data-stu-id="f962f-166">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="f962f-167">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="f962f-167">**Guest user**</span></span>   | <span data-ttu-id="f962f-168">**ロール**</span><span class="sxs-lookup"><span data-stu-id="f962f-168">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="f962f-169">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="f962f-169">MPN partner admin</span></span>|
||<span data-ttu-id="f962f-170">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="f962f-170">Accounts admin</span></span>|
||<span data-ttu-id="f962f-171">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="f962f-171">Incentives admin</span></span>|
||<span data-ttu-id="f962f-172">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="f962f-172">Business profile admin</span></span>|
||<span data-ttu-id="f962f-173">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="f962f-173">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="f962f-174">MPN メンバーシップと、会社の管理 (非 AAD のロール: これらのロール管理、テナントではなく、会社のビジネス)</span><span class="sxs-lookup"><span data-stu-id="f962f-174">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="f962f-175">**ロール**</span><span class="sxs-lookup"><span data-stu-id="f962f-175">**Role**</span></span> | <span data-ttu-id="f962f-176">**できること**</span><span class="sxs-lookup"><span data-stu-id="f962f-176">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="f962f-177">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="f962f-177">MPN partner admin</span></span>|<span data-ttu-id="f962f-178">• ビューの作成、およびパートナー サービス要求の管理</span><span class="sxs-lookup"><span data-stu-id="f962f-178">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="f962f-179">• ビューの法律、会社、ビジネス、および MPN プロファイル</span><span class="sxs-lookup"><span data-stu-id="f962f-179">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="f962f-180">• ユーザーの詳細およびスキル データの表示</span><span class="sxs-lookup"><span data-stu-id="f962f-180">• View user details and their skills data</span></span>
||<span data-ttu-id="f962f-181">• コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="f962f-181">• View competencies</span></span>
||<span data-ttu-id="f962f-182">• 特典の表示と管理</span><span class="sxs-lookup"><span data-stu-id="f962f-182">• View and manage benefits</span></span>
||<span data-ttu-id="f962f-183">• MPN オファーの表示と購入</span><span class="sxs-lookup"><span data-stu-id="f962f-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="f962f-184">• MPN オファーの注文履歴と請求書の表示</span><span class="sxs-lookup"><span data-stu-id="f962f-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="f962f-185">• パートナー コントリビューション インジケーター データの表示</span><span class="sxs-lookup"><span data-stu-id="f962f-185">• View partner contribution indicator data</span></span>
||<span data-ttu-id="f962f-186">• 利用券検証ツールでの作業</span><span class="sxs-lookup"><span data-stu-id="f962f-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="f962f-187">- 顧客データ分析の表示</span><span class="sxs-lookup"><span data-stu-id="f962f-187">- View customer data analytics</span></span>
|| <span data-ttu-id="f962f-188">会社内の他のユーザー ロールの表示が、ロールを割り当てることはできません</span><span class="sxs-lookup"><span data-stu-id="f962f-188">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="f962f-189">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="f962f-189">Account admin</span></span>| <span data-ttu-id="f962f-190">場所を追加します。</span><span class="sxs-lookup"><span data-stu-id="f962f-190">Add locations</span></span>
|| <span data-ttu-id="f962f-191">ユーザーが管理者のアカウントに関連するプロファイルを管理します。</span><span class="sxs-lookup"><span data-stu-id="f962f-191">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="f962f-192">• テナント内のユーザーに対するロールの非 AAD ロールへの割り当て</span><span class="sxs-lookup"><span data-stu-id="f962f-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="f962f-193">• プログラムへの場所の登録</span><span class="sxs-lookup"><span data-stu-id="f962f-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="f962f-194">参照を管理します。</span><span class="sxs-lookup"><span data-stu-id="f962f-194">Manage referrals</span></span> 

|<span data-ttu-id="f962f-195">**ロール**</span><span class="sxs-lookup"><span data-stu-id="f962f-195">**Role**</span></span>|<span data-ttu-id="f962f-196">**できること**</span><span class="sxs-lookup"><span data-stu-id="f962f-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="f962f-197">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="f962f-197">Referrals admin</span></span>       |<span data-ttu-id="f962f-198">• ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="f962f-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="f962f-199">• 紹介案件の受信と管理</span><span class="sxs-lookup"><span data-stu-id="f962f-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="f962f-200">• ビューの作成、および共同販売の参照の管理</span><span class="sxs-lookup"><span data-stu-id="f962f-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="f962f-201">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="f962f-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="f962f-202">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="f962f-202">Business profile admin</span></span>   |<span data-ttu-id="f962f-203">• ビューの作成、およびビジネス プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="f962f-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="f962f-204">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="f962f-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="f962f-205">インセンティブを管理します。</span><span class="sxs-lookup"><span data-stu-id="f962f-205">Manage incentives</span></span> 

|<span data-ttu-id="f962f-206">**ロール**</span><span class="sxs-lookup"><span data-stu-id="f962f-206">**Role**</span></span> | <span data-ttu-id="f962f-207">**できること**</span><span class="sxs-lookup"><span data-stu-id="f962f-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="f962f-208">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="f962f-208">Incentives admin</span></span>|<span data-ttu-id="f962f-209">• インセンティブの開始と管理</span><span class="sxs-lookup"><span data-stu-id="f962f-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="f962f-210">• インセンティブ プログラムのすべての側面の表示と編集</span><span class="sxs-lookup"><span data-stu-id="f962f-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="f962f-211">• 銀行および税の詳細情報の表示と編集</span><span class="sxs-lookup"><span data-stu-id="f962f-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="f962f-212">• リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="f962f-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="f962f-213">• サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="f962f-213">• Access support</span></span>
||<span data-ttu-id="f962f-214">• インセンティブ支払いについての議論</span><span class="sxs-lookup"><span data-stu-id="f962f-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="f962f-215">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="f962f-215">Incentives user</span></span>|<span data-ttu-id="f962f-216">• インセンティブ プログラムの表示</span><span class="sxs-lookup"><span data-stu-id="f962f-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="f962f-217">• インセンティブの申請の表示と開始</span><span class="sxs-lookup"><span data-stu-id="f962f-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="f962f-218">• リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="f962f-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="f962f-219">• サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="f962f-219">• Access support</span></span>












