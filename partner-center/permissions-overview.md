---
title: ユーザー ロールとアクセス許可の割り当て | パートナー センター
ms.topic: article
ms.date: 03/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 商取引、紹介、インセンティブ、または会社の MPN メンバーシップを管理しているユーザーに最適なロールについて説明します。
author: LauraBrenner
ms.author: labrenne
keywords: ロール, アクセス許可, 管理者, エージェント
ms.localizationpriority: high
ms.openlocfilehash: fbff7f353a0055aa645467fccaa049b598b4c880
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2020
ms.locfileid: "80296399"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="abf70-104">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="abf70-104">Assign users roles and permissions</span></span>

<span data-ttu-id="abf70-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="abf70-105">**Appropriate roles**</span></span>
-    <span data-ttu-id="abf70-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-106">Global admin</span></span>
-    <span data-ttu-id="abf70-107">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-107">User admin</span></span>
-    <span data-ttu-id="abf70-108">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-108">MPN partner admin</span></span>

<span data-ttu-id="abf70-109">貴社の正式名称や法的住所、サポートの詳細、税金の除外の申告、銀行情報、主要な連絡先など、パートナー プロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="abf70-109">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="abf70-110">次に、ユーザーにパスワードとロールを設定させて、ユーザーがパートナー センターでの作業を開始できるようにします。</span><span class="sxs-lookup"><span data-stu-id="abf70-110">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="abf70-111">パートナー センターで作業できるように従業員を設定する</span><span class="sxs-lookup"><span data-stu-id="abf70-111">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="abf70-112">ユーザーに付与するロールとアクセス許可によって、パートナー センターでのユーザーのアクセスの種類が決まります。</span><span class="sxs-lookup"><span data-stu-id="abf70-112">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="abf70-113">ロールは、貴社のビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="abf70-113">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="abf70-114">たとえば、貴社のビジネスがクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、グローバル管理者などの標準の Azure AD テナント管理ロールだけでなく、CSP プログラムに固有のロールも必要です。</span><span class="sxs-lookup"><span data-stu-id="abf70-114">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="abf70-115">各プログラムには、それに固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="abf70-115">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="abf70-116">Azure Active Directory (AAD) テナント ロールには、グローバル管理者、ユーザー管理者、および CSP のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="abf70-116">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="abf70-117">AAD 以外のロールはテナントを管理しないロールであり、MPN 管理者、ビジネス プロファイル管理者、紹介管理者、インセンティブ管理者、およびインセンティブ ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="abf70-117">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="abf70-118">パートナー センターで商取引を管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="abf70-118">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="abf70-119">**Role**</span><span class="sxs-lookup"><span data-stu-id="abf70-119">**Role**</span></span>|<span data-ttu-id="abf70-120">**できること**</span><span class="sxs-lookup"><span data-stu-id="abf70-120">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="abf70-121">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-121">Global admin</span></span>|<span data-ttu-id="abf70-122">\*    すべての特権を備えたすべての Microsoft アカウントまたはサービスへのアクセスが可能</span><span class="sxs-lookup"><span data-stu-id="abf70-122">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="abf70-123">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="abf70-123">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="abf70-124">\*    契約、価格表、オファーの表示</span><span class="sxs-lookup"><span data-stu-id="abf70-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="abf70-125">\*    パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="abf70-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="abf70-126">課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="abf70-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="abf70-127">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-127">User management admin</span></span>   | <span data-ttu-id="abf70-128">\*    ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="abf70-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="abf70-129">\*    すべてのパートナー プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="abf70-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="abf70-130">\*    パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="abf70-130">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="abf70-131">課金管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-131">Billing admin</span></span> | <span data-ttu-id="abf70-132">- 課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="abf70-132">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="abf70-133">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="abf70-133">Default user</span></span>|  <span data-ttu-id="abf70-134">マイ プロフィールの表示</span><span class="sxs-lookup"><span data-stu-id="abf70-134">View My profile</span></span>   |
|<span data-ttu-id="abf70-135">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="abf70-135">Admin agent</span></span> | <span data-ttu-id="abf70-136">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="abf70-136">\*    Customer management</span></span>
||<span data-ttu-id="abf70-137">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="abf70-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="abf70-138">\*    プロファイルの作成とデバイスへの適用</span><span class="sxs-lookup"><span data-stu-id="abf70-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="abf70-139">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="abf70-139">\*    Subscription management</span></span>
||<span data-ttu-id="abf70-140">\*    顧客のためのサービスの正常性とサービス要求</span><span class="sxs-lookup"><span data-stu-id="abf70-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="abf70-141">\*    代理管理者特権の要求</span><span class="sxs-lookup"><span data-stu-id="abf70-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="abf70-142">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="abf70-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="abf70-143">\*    請求</span><span class="sxs-lookup"><span data-stu-id="abf70-143">\*    Billing</span></span>
||<span data-ttu-id="abf70-144">\*    顧客の代理としての管理</span><span class="sxs-lookup"><span data-stu-id="abf70-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="abf70-145">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="abf70-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="abf70-146">販売代理店</span><span class="sxs-lookup"><span data-stu-id="abf70-146">Sales agent</span></span> | <span data-ttu-id="abf70-147">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="abf70-147">\*    Customer management</span></span>
||<span data-ttu-id="abf70-148">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="abf70-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="abf70-149">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="abf70-149">\*    Subscription management</span></span>
||<span data-ttu-id="abf70-150">\*    サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="abf70-150">\*    View support tickets</span></span>
||<span data-ttu-id="abf70-151">\*    顧客との再販業者関係の要求</span><span class="sxs-lookup"><span data-stu-id="abf70-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="abf70-152">\*    潜在顧客の管理</span><span class="sxs-lookup"><span data-stu-id="abf70-152">\*    Manage customer leads</span></span>
||<span data-ttu-id="abf70-153">\*    顧客契約の表示</span><span class="sxs-lookup"><span data-stu-id="abf70-153">\*    View the customer agreement</span></span>
||<span data-ttu-id="abf70-154">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="abf70-154">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="abf70-155">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="abf70-155">Helpdesk agent</span></span>| <span data-ttu-id="abf70-156">\*    顧客の検索と表示</span><span class="sxs-lookup"><span data-stu-id="abf70-156">\*    Search for and view a customer</span></span>
||<span data-ttu-id="abf70-157">\*    顧客の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="abf70-157">\*    Edit customer details</span></span>
||<span data-ttu-id="abf70-158">\*    請求またはサブスクリプション管理に関する顧客の問題の解決サポート</span><span class="sxs-lookup"><span data-stu-id="abf70-158">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="abf70-159">\*    顧客の代理としてのサポート要求</span><span class="sxs-lookup"><span data-stu-id="abf70-159">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="abf70-160">\*    顧客の代理としてのサブスクリプションと請求に関する問題の管理</span><span class="sxs-lookup"><span data-stu-id="abf70-160">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="abf70-161">コントロール パネル ベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="abf70-161">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="abf70-162">(CSP ロールと非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="abf70-162">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="abf70-163">CPV は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムとパートナー センター API を統合するために使用するアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="abf70-163">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="abf70-164">**Role**</span><span class="sxs-lookup"><span data-stu-id="abf70-164">**Role**</span></span>   |<span data-ttu-id="abf70-165">**できること**</span><span class="sxs-lookup"><span data-stu-id="abf70-165">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="abf70-166">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-166">Global admin</span></span>| <span data-ttu-id="abf70-167">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="abf70-167">View and manage your CPV profile</span></span>|
||<span data-ttu-id="abf70-168">CPV 機能にアクセスする必要があるユーザーの表示と管理</span><span class="sxs-lookup"><span data-stu-id="abf70-168">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="abf70-169">ゲスト ユーザー (AAD テナントに追加される必要があります)</span><span class="sxs-lookup"><span data-stu-id="abf70-169">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="abf70-170">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="abf70-170">**Guest user**</span></span>   | <span data-ttu-id="abf70-171">**ロール**</span><span class="sxs-lookup"><span data-stu-id="abf70-171">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="abf70-172">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-172">MPN partner admin</span></span>|
||<span data-ttu-id="abf70-173">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-173">Accounts admin</span></span>|
||<span data-ttu-id="abf70-174">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-174">Incentives admin</span></span>|
||<span data-ttu-id="abf70-175">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-175">Business profile admin</span></span>|
||<span data-ttu-id="abf70-176">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-176">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="abf70-177">MPN メンバーシップと会社の管理 (AAD 以外のロール: これらのロールは、テナントではなく会社の業務を管理します)</span><span class="sxs-lookup"><span data-stu-id="abf70-177">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="abf70-178">**Role**</span><span class="sxs-lookup"><span data-stu-id="abf70-178">**Role**</span></span> | <span data-ttu-id="abf70-179">**できること**</span><span class="sxs-lookup"><span data-stu-id="abf70-179">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="abf70-180">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-180">MPN partner admin</span></span>|<span data-ttu-id="abf70-181">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="abf70-181">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="abf70-182">\*    法的プロファイル、企業プロファイル、ビジネス プロファイル、MPN プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="abf70-182">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="abf70-183">\*    ユーザーの詳細およびスキル データの表示</span><span class="sxs-lookup"><span data-stu-id="abf70-183">\*    View user details and their skills data</span></span>
||<span data-ttu-id="abf70-184">\*    コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="abf70-184">\*    View competencies</span></span>
||<span data-ttu-id="abf70-185">\*    特典の表示と管理</span><span class="sxs-lookup"><span data-stu-id="abf70-185">\*    View and manage benefits</span></span>
||<span data-ttu-id="abf70-186">\*    MPN オファーの表示と購入</span><span class="sxs-lookup"><span data-stu-id="abf70-186">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="abf70-187">\*    MPN オファーの注文履歴と請求書の表示</span><span class="sxs-lookup"><span data-stu-id="abf70-187">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="abf70-188">\*    パートナー貢献度インジケーター データの表示</span><span class="sxs-lookup"><span data-stu-id="abf70-188">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="abf70-189">\*    利用券検証ツールでの作業</span><span class="sxs-lookup"><span data-stu-id="abf70-189">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="abf70-190">\*    顧客データ分析の表示</span><span class="sxs-lookup"><span data-stu-id="abf70-190">\*    View customer data analytics</span></span>
||<span data-ttu-id="abf70-191">\*    会社内の他のユーザー ロールを表示しますが、ロールを割り当てることはできません</span><span class="sxs-lookup"><span data-stu-id="abf70-191">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="abf70-192">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-192">Account admin</span></span>| <span data-ttu-id="abf70-193">場所の追加</span><span class="sxs-lookup"><span data-stu-id="abf70-193">Add locations</span></span>
|| <span data-ttu-id="abf70-194">管理対象のアカウントに関連するプロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="abf70-194">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="abf70-195">\*    テナント内のユーザーに対するロールの非 AAD ロールへの割り当て</span><span class="sxs-lookup"><span data-stu-id="abf70-195">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="abf70-196">\*    プログラムへの場所の登録</span><span class="sxs-lookup"><span data-stu-id="abf70-196">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="abf70-197">紹介の管理</span><span class="sxs-lookup"><span data-stu-id="abf70-197">Manage referrals</span></span> 

|<span data-ttu-id="abf70-198">**Role**</span><span class="sxs-lookup"><span data-stu-id="abf70-198">**Role**</span></span>|<span data-ttu-id="abf70-199">**できること**</span><span class="sxs-lookup"><span data-stu-id="abf70-199">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="abf70-200">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-200">Referrals admin</span></span>       |<span data-ttu-id="abf70-201">\*    ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="abf70-201">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="abf70-202">\*    紹介の受信と管理</span><span class="sxs-lookup"><span data-stu-id="abf70-202">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="abf70-203">\*    共同販売の紹介の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="abf70-203">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="abf70-204">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="abf70-204">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="abf70-205">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-205">Business profile admin</span></span>   |<span data-ttu-id="abf70-206">\*    ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="abf70-206">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="abf70-207">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="abf70-207">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="abf70-208">インセンティブの管理</span><span class="sxs-lookup"><span data-stu-id="abf70-208">Manage incentives</span></span> 

|<span data-ttu-id="abf70-209">**Role**</span><span class="sxs-lookup"><span data-stu-id="abf70-209">**Role**</span></span> | <span data-ttu-id="abf70-210">**できること**</span><span class="sxs-lookup"><span data-stu-id="abf70-210">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="abf70-211">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="abf70-211">Incentives admin</span></span>|<span data-ttu-id="abf70-212">\*    インセンティブの開始と管理</span><span class="sxs-lookup"><span data-stu-id="abf70-212">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="abf70-213">\*    インセンティブ プログラムのすべての側面の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="abf70-213">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="abf70-214">\*    銀行および税の詳細情報の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="abf70-214">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="abf70-215">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="abf70-215">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="abf70-216">\*    サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="abf70-216">\*    Access support</span></span>
||<span data-ttu-id="abf70-217">\*    インセンティブ支払いについての議論</span><span class="sxs-lookup"><span data-stu-id="abf70-217">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="abf70-218">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="abf70-218">Incentives user</span></span>|<span data-ttu-id="abf70-219">\*    インセンティブ プログラムを表示可能</span><span class="sxs-lookup"><span data-stu-id="abf70-219">\*    Can view incentives programs</span></span>
||<span data-ttu-id="abf70-220">\*    インセンティブの申請の表示と開始が可能</span><span class="sxs-lookup"><span data-stu-id="abf70-220">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="abf70-221">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="abf70-221">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="abf70-222">\*    サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="abf70-222">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="abf70-223">パートナー センター インサイト データの表示</span><span class="sxs-lookup"><span data-stu-id="abf70-223">View Partner Center Insights data</span></span>

|<span data-ttu-id="abf70-224">**Role**</span><span class="sxs-lookup"><span data-stu-id="abf70-224">**Role**</span></span> | <span data-ttu-id="abf70-225">**できること**</span><span class="sxs-lookup"><span data-stu-id="abf70-225">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="abf70-226">エグゼクティブ レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="abf70-226">Executive report viewer</span></span>|<span data-ttu-id="abf70-227">すべてのレポートデータセットへのアクセス</span><span class="sxs-lookup"><span data-stu-id="abf70-227">Access to all reporting datasets</span></span>|
|<span data-ttu-id="abf70-228">レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="abf70-228">Report viewer</span></span>|<span data-ttu-id="abf70-229">収益、顧客、従業員の個人データを除くデータ レポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="abf70-229">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    