---
title: ユーザー ロールとアクセス許可の割り当て |パートナー センター
ms.topic: article
ms.date: 3/5/19
description: パートナー センターで作業する必要があるすべての従業員にロールを割り当てる必要があります。
author: LauraBrenner
ms.author: labrenne
keywords: ロール, アクセス許可, 管理者, エージェント
ms.localizationpriority: medium
ms.openlocfilehash: 65a2f7f373fc57f86cfffa73aafd3b7095fe2c04
ms.sourcegitcommit: be8086534ec73937f2be9bcc495c2627423c50f6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "67396729"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="8af09-104">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="8af09-104">Assign users roles and permissions</span></span>


<span data-ttu-id="8af09-105">貴社の正式名称や法的住所、サポートの詳細、税金の除外の申告、銀行情報、主要な連絡先など、パートナー プロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="8af09-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="8af09-106">次に、ユーザーにパスワードとロールを設定させて、ユーザーがパートナー センターでの作業を開始できるようにします。</span><span class="sxs-lookup"><span data-stu-id="8af09-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="8af09-107">パートナー センターで作業できるように従業員を設定する</span><span class="sxs-lookup"><span data-stu-id="8af09-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="8af09-108">ユーザーに付与するロールとアクセス許可によって、パートナー センターでのユーザーのアクセスの種類が決まります。</span><span class="sxs-lookup"><span data-stu-id="8af09-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="8af09-109">ロールは、貴社のビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="8af09-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="8af09-110">たとえば、貴社のビジネスがクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、グローバル管理者などの標準の Azure AD テナント管理ロールだけでなく、CSP プログラムに固有のロールも必要です。</span><span class="sxs-lookup"><span data-stu-id="8af09-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="8af09-111">各プログラムには、それに固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="8af09-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="8af09-112">Azure Active Directory (AAD) テナント ロールには、グローバル管理者、ユーザー管理者、および CSP のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="8af09-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="8af09-113">非 AAD のロールは、テナントを管理しないロールおよび MPN 管理者、ビジネス プロファイルの管理、参照の管理、インセンティブの管理者およびインセンティブのユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="8af09-113">Non-AAD roles are those roles that do not manage the tenant and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="8af09-114">パートナー センターで商取引を管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="8af09-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="8af09-115">**ロール**</span><span class="sxs-lookup"><span data-stu-id="8af09-115">**Role**</span></span>|<span data-ttu-id="8af09-116">**できること**</span><span class="sxs-lookup"><span data-stu-id="8af09-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="8af09-117">全体管理者</span><span class="sxs-lookup"><span data-stu-id="8af09-117">Global admin</span></span>|<span data-ttu-id="8af09-118">• すべての特権を備えたすべての Microsoft アカウント/サービスへのアクセス</span><span class="sxs-lookup"><span data-stu-id="8af09-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="8af09-119">• パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="8af09-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="8af09-120">• 契約、価格表、キャンペーンの表示</span><span class="sxs-lookup"><span data-stu-id="8af09-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="8af09-121">• パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="8af09-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="8af09-122">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="8af09-122">User Admin</span></span>   | <span data-ttu-id="8af09-123">• ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="8af09-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="8af09-124">• すべてのパートナー プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="8af09-124">• View all partner profiles</span></span>
||<span data-ttu-id="8af09-125">• パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="8af09-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="8af09-126">課金の管理</span><span class="sxs-lookup"><span data-stu-id="8af09-126">Billing admin</span></span> | <span data-ttu-id="8af09-127">- 課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="8af09-127">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="8af09-128">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="8af09-128">Default user</span></span>|  <span data-ttu-id="8af09-129">マイ プロフィールの表示</span><span class="sxs-lookup"><span data-stu-id="8af09-129">View My profile</span></span>   |
|<span data-ttu-id="8af09-130">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="8af09-130">Admin agent</span></span> | <span data-ttu-id="8af09-131">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="8af09-131">•    Customer management</span></span>
||<span data-ttu-id="8af09-132">• パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="8af09-132">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="8af09-133">• プロファイルの作成とデバイスへの適用</span><span class="sxs-lookup"><span data-stu-id="8af09-133">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="8af09-134">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="8af09-134">• Subscription management</span></span>
||<span data-ttu-id="8af09-135">• 顧客のためのサービスの正常性の確認とサービス要求</span><span class="sxs-lookup"><span data-stu-id="8af09-135">• Service health and service requests for customers</span></span>
||<span data-ttu-id="8af09-136">• 代理管理者特権の要求</span><span class="sxs-lookup"><span data-stu-id="8af09-136">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="8af09-137">• 価格とプランの表示</span><span class="sxs-lookup"><span data-stu-id="8af09-137">• View pricing and offers</span></span>
||<span data-ttu-id="8af09-138">• 請求</span><span class="sxs-lookup"><span data-stu-id="8af09-138">• Billing</span></span>
||<span data-ttu-id="8af09-139">• 顧客の代理としての管理</span><span class="sxs-lookup"><span data-stu-id="8af09-139">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="8af09-140">• 付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="8af09-140">• Register a value added reseller</span></span>|
|<span data-ttu-id="8af09-141">販売代理店</span><span class="sxs-lookup"><span data-stu-id="8af09-141">Sales agent</span></span> | <span data-ttu-id="8af09-142">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="8af09-142">•    Customer management</span></span>
||<span data-ttu-id="8af09-143">• パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="8af09-143">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="8af09-144">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="8af09-144">• Subscription management</span></span>
||<span data-ttu-id="8af09-145">• 表示価格を一覧表示し、提供しています</span><span class="sxs-lookup"><span data-stu-id="8af09-145">• View price lists and offers</span></span>
||<span data-ttu-id="8af09-146">• サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="8af09-146">• View support tickets</span></span>
||<span data-ttu-id="8af09-147">• 顧客との再販業者関係の要求</span><span class="sxs-lookup"><span data-stu-id="8af09-147">• Request a relationship with a customer</span></span>
||<span data-ttu-id="8af09-148">• 見込み客の管理</span><span class="sxs-lookup"><span data-stu-id="8af09-148">• Manage customer leads</span></span>
||<span data-ttu-id="8af09-149">• 顧客契約の表示</span><span class="sxs-lookup"><span data-stu-id="8af09-149">• View the customer agreement</span></span>
||<span data-ttu-id="8af09-150">• 付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="8af09-150">• Register a value-added reseller</span></span>|
|<span data-ttu-id="8af09-151">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="8af09-151">Helpdesk agent</span></span>| <span data-ttu-id="8af09-152">• 顧客の検索と表示</span><span class="sxs-lookup"><span data-stu-id="8af09-152">•  Search for and view a customer</span></span>
||<span data-ttu-id="8af09-153">• 顧客の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="8af09-153">• Edit customer details</span></span>
||<span data-ttu-id="8af09-154">• 請求やサブスクリプション管理に関する顧客の問題の解決サポート</span><span class="sxs-lookup"><span data-stu-id="8af09-154">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="8af09-155">• 顧客の代理としてのサポート要求 (注: Office 365 サブスクリプションの場合、このタスクを完了するには管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="8af09-155">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="8af09-156">• 顧客の代理としてのサブスクリプションとサービスの管理 (注: Office 365 サブスクリプションの場合、このタスクを完了するには管理者エージェントの役割が必要です)</span><span class="sxs-lookup"><span data-stu-id="8af09-156">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="8af09-157">コントロール パネル ベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="8af09-157">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="8af09-158">(CSP ロールと非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="8af09-158">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="8af09-159">CPV は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムとパートナー センター API を統合するために使用するアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="8af09-159">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="8af09-160">**ロール**</span><span class="sxs-lookup"><span data-stu-id="8af09-160">**Role**</span></span>   |<span data-ttu-id="8af09-161">**できること**</span><span class="sxs-lookup"><span data-stu-id="8af09-161">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="8af09-162">全体管理者</span><span class="sxs-lookup"><span data-stu-id="8af09-162">Global admin</span></span>| <span data-ttu-id="8af09-163">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="8af09-163">View and manage your CPV profile</span></span>|
||<span data-ttu-id="8af09-164">CPV 機能にアクセスする必要があるユーザーの表示と管理</span><span class="sxs-lookup"><span data-stu-id="8af09-164">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="8af09-165">ゲスト ユーザー (AAD テナントに追加される必要があります)</span><span class="sxs-lookup"><span data-stu-id="8af09-165">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="8af09-166">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="8af09-166">**Guest user**</span></span>   | <span data-ttu-id="8af09-167">**ロール**</span><span class="sxs-lookup"><span data-stu-id="8af09-167">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="8af09-168">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="8af09-168">MPN partner admin</span></span>|
||<span data-ttu-id="8af09-169">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="8af09-169">Accounts admin</span></span>|
||<span data-ttu-id="8af09-170">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="8af09-170">Incentives admin</span></span>|
||<span data-ttu-id="8af09-171">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="8af09-171">Business profile admin</span></span>|
||<span data-ttu-id="8af09-172">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="8af09-172">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="8af09-173">MPN メンバーシップと、会社の管理 (非 AAD のロール: これらのロール管理、テナントではなく、会社のビジネス)</span><span class="sxs-lookup"><span data-stu-id="8af09-173">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="8af09-174">**ロール**</span><span class="sxs-lookup"><span data-stu-id="8af09-174">**Role**</span></span> | <span data-ttu-id="8af09-175">**できること**</span><span class="sxs-lookup"><span data-stu-id="8af09-175">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="8af09-176">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="8af09-176">MPN partner admin</span></span>|<span data-ttu-id="8af09-177">• 非テナントユーザーの追加</span><span class="sxs-lookup"><span data-stu-id="8af09-177">•Can add non-tenant users</span></span>
||<span data-ttu-id="8af09-178">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="8af09-178">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="8af09-179">• 法的プロファイル、組織プロファイル、ビジネス プロファイル、MPN プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="8af09-179">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="8af09-180">• ユーザーの詳細およびスキル データの表示</span><span class="sxs-lookup"><span data-stu-id="8af09-180">• View user details and their skills data</span></span>
||<span data-ttu-id="8af09-181">• コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="8af09-181">• View competencies</span></span>
||<span data-ttu-id="8af09-182">• 特典の表示と管理</span><span class="sxs-lookup"><span data-stu-id="8af09-182">• View and manage benefits</span></span>
||<span data-ttu-id="8af09-183">• MPN オファーの表示と購入</span><span class="sxs-lookup"><span data-stu-id="8af09-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="8af09-184">• MPN オファーの注文履歴と請求書の表示</span><span class="sxs-lookup"><span data-stu-id="8af09-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="8af09-185">• パートナーの貢献度データの表示</span><span class="sxs-lookup"><span data-stu-id="8af09-185">• View partner contribution data</span></span>
||<span data-ttu-id="8af09-186">• 利用券検証ツールでの作業</span><span class="sxs-lookup"><span data-stu-id="8af09-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="8af09-187">- 顧客データ分析の表示</span><span class="sxs-lookup"><span data-stu-id="8af09-187">- View customer data analytics</span></span>
|<span data-ttu-id="8af09-188">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="8af09-188">Account admin</span></span>| <span data-ttu-id="8af09-189">• 非テナントユーザーの追加</span><span class="sxs-lookup"><span data-stu-id="8af09-189">•   Can add non-tenant users</span></span>
||<span data-ttu-id="8af09-190">• 場所の追加または削除</span><span class="sxs-lookup"><span data-stu-id="8af09-190">• Add or delete locations</span></span>
||<span data-ttu-id="8af09-191">- 管理対象のアカウントに関連するプロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="8af09-191">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="8af09-192">• テナント内のユーザーに対するロールの非 AAD ロールへの割り当て</span><span class="sxs-lookup"><span data-stu-id="8af09-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="8af09-193">• プログラムへの場所の登録</span><span class="sxs-lookup"><span data-stu-id="8af09-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="8af09-194">参照を管理します。</span><span class="sxs-lookup"><span data-stu-id="8af09-194">Manage referrals</span></span> 

|<span data-ttu-id="8af09-195">**ロール**</span><span class="sxs-lookup"><span data-stu-id="8af09-195">**Role**</span></span>|<span data-ttu-id="8af09-196">**できること**</span><span class="sxs-lookup"><span data-stu-id="8af09-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="8af09-197">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="8af09-197">Referrals admin</span></span>       |<span data-ttu-id="8af09-198">• ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="8af09-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="8af09-199">• 紹介案件の受信と管理</span><span class="sxs-lookup"><span data-stu-id="8af09-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="8af09-200">• ビューの作成、および共同販売の参照の管理</span><span class="sxs-lookup"><span data-stu-id="8af09-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="8af09-201">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="8af09-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="8af09-202">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="8af09-202">Business profile admin</span></span>   |<span data-ttu-id="8af09-203">• ビューの作成、およびビジネス プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="8af09-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="8af09-204">• パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="8af09-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="8af09-205">インセンティブを管理します。</span><span class="sxs-lookup"><span data-stu-id="8af09-205">Manage incentives</span></span> 

|<span data-ttu-id="8af09-206">**ロール**</span><span class="sxs-lookup"><span data-stu-id="8af09-206">**Role**</span></span> | <span data-ttu-id="8af09-207">**できること**</span><span class="sxs-lookup"><span data-stu-id="8af09-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="8af09-208">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="8af09-208">Incentives admin</span></span>|<span data-ttu-id="8af09-209">• インセンティブの開始と管理</span><span class="sxs-lookup"><span data-stu-id="8af09-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="8af09-210">• インセンティブ プログラムのすべての側面の表示と編集</span><span class="sxs-lookup"><span data-stu-id="8af09-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="8af09-211">• 銀行および税の詳細情報の表示と編集</span><span class="sxs-lookup"><span data-stu-id="8af09-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="8af09-212">• リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="8af09-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="8af09-213">• サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="8af09-213">• Access support</span></span>
||<span data-ttu-id="8af09-214">• インセンティブ支払いについての議論</span><span class="sxs-lookup"><span data-stu-id="8af09-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="8af09-215">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="8af09-215">Incentives user</span></span>|<span data-ttu-id="8af09-216">• インセンティブ プログラムの表示</span><span class="sxs-lookup"><span data-stu-id="8af09-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="8af09-217">• インセンティブの申請の表示と開始</span><span class="sxs-lookup"><span data-stu-id="8af09-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="8af09-218">• リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="8af09-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="8af09-219">• リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="8af09-219">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="8af09-220">• サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="8af09-220">• Access support</span></span>












