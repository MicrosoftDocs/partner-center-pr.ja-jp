---
title: ユーザーにロールとアクセス許可を割り当てる
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 商取引、紹介、インセンティブ、または MPN メンバーシップをパートナー センターで管理する、会社のユーザーに最適なロールについて説明します。
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c0e7aecd7d56e1919c7f142312a9090b8ff40bd3
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434321"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="d982e-103">パートナー センターで作業する必要がある会社のユーザーにユーザーのロールとアクセス許可を割り当てる</span><span class="sxs-lookup"><span data-stu-id="d982e-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="d982e-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="d982e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d982e-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-105">Global admin</span></span>
- <span data-ttu-id="d982e-106">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-106">User admin</span></span>
- <span data-ttu-id="d982e-107">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-107">MPN partner admin</span></span>

<span data-ttu-id="d982e-108">貴社の正式名称や法的住所、サポートの詳細、税金の除外の申告、銀行情報、主要な連絡先など、パートナー プロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="d982e-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="d982e-109">次のステップ:ユーザーにパスワードとロールを設定させて、ユーザーがパートナー センターでの作業を開始できるようにします。</span><span class="sxs-lookup"><span data-stu-id="d982e-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="d982e-110">パートナー センターで作業できるように従業員を設定する</span><span class="sxs-lookup"><span data-stu-id="d982e-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="d982e-111">ユーザーに付与するロールとアクセス許可によって、パートナー センターでのユーザーのアクセスの種類が決まります。</span><span class="sxs-lookup"><span data-stu-id="d982e-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="d982e-112">ロールは、貴社のビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="d982e-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="d982e-113">たとえば、貴社のビジネスがクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、グローバル管理者などの標準の Azure AD テナント管理ロールだけでなく、CSP プログラムに固有のロールも必要です。</span><span class="sxs-lookup"><span data-stu-id="d982e-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="d982e-114">各プログラムには、それに固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="d982e-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="d982e-115">Azure Active Directory (AAD) テナント ロールには、グローバル管理者、ユーザー管理者、および CSP のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="d982e-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="d982e-116">AAD 以外のロールはテナントを管理しないロールであり、MPN 管理者、ビジネス プロファイル管理者、紹介管理者、インセンティブ管理者、およびインセンティブ ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="d982e-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="d982e-117">パートナー センターで商取引を管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="d982e-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="d982e-118">**Role**</span><span class="sxs-lookup"><span data-stu-id="d982e-118">**Role**</span></span>|<span data-ttu-id="d982e-119">**できること**</span><span class="sxs-lookup"><span data-stu-id="d982e-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="d982e-120">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-120">Global admin</span></span>|<span data-ttu-id="d982e-121">\*    すべての特権を備えたすべての Microsoft アカウントまたはサービスへのアクセスが可能</span><span class="sxs-lookup"><span data-stu-id="d982e-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="d982e-122">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="d982e-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="d982e-123">\*    契約、価格表、オファーの表示</span><span class="sxs-lookup"><span data-stu-id="d982e-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="d982e-124">\*    パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d982e-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="d982e-125">課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d982e-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="d982e-126">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-126">User management admin</span></span>   | <span data-ttu-id="d982e-127">\*    ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d982e-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="d982e-128">\*    すべてのパートナー プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="d982e-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="d982e-129">\*    パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d982e-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="d982e-130">課金管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-130">Billing admin</span></span> | <span data-ttu-id="d982e-131">- 課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d982e-131">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="d982e-132">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="d982e-132">Default user</span></span>|  <span data-ttu-id="d982e-133">マイ プロフィールの表示</span><span class="sxs-lookup"><span data-stu-id="d982e-133">View My profile</span></span>   |
|<span data-ttu-id="d982e-134">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="d982e-134">Admin agent</span></span> | <span data-ttu-id="d982e-135">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="d982e-135">\*    Customer management</span></span>
||<span data-ttu-id="d982e-136">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="d982e-136">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="d982e-137">\*    プロファイルの作成とデバイスへの適用</span><span class="sxs-lookup"><span data-stu-id="d982e-137">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="d982e-138">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="d982e-138">\*    Subscription management</span></span>
||<span data-ttu-id="d982e-139">\*    顧客のためのサービスの正常性とサービス要求</span><span class="sxs-lookup"><span data-stu-id="d982e-139">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="d982e-140">\*    代理管理者特権の要求</span><span class="sxs-lookup"><span data-stu-id="d982e-140">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="d982e-141">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="d982e-141">\*    View pricing and offers</span></span>
||<span data-ttu-id="d982e-142">\*    請求</span><span class="sxs-lookup"><span data-stu-id="d982e-142">\*    Billing</span></span>
||<span data-ttu-id="d982e-143">\*    顧客の代理としての管理</span><span class="sxs-lookup"><span data-stu-id="d982e-143">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="d982e-144">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="d982e-144">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="d982e-145">販売代理店</span><span class="sxs-lookup"><span data-stu-id="d982e-145">Sales agent</span></span> | <span data-ttu-id="d982e-146">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="d982e-146">\*    Customer management</span></span>
||<span data-ttu-id="d982e-147">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="d982e-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="d982e-148">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="d982e-148">\*    Subscription management</span></span>
||<span data-ttu-id="d982e-149">\*    サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="d982e-149">\*    View support tickets</span></span>
||<span data-ttu-id="d982e-150">\*    顧客との再販業者関係の要求</span><span class="sxs-lookup"><span data-stu-id="d982e-150">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="d982e-151">\*    潜在顧客の管理</span><span class="sxs-lookup"><span data-stu-id="d982e-151">\*    Manage customer leads</span></span>
||<span data-ttu-id="d982e-152">\*    顧客契約の表示</span><span class="sxs-lookup"><span data-stu-id="d982e-152">\*    View the customer agreement</span></span>
||<span data-ttu-id="d982e-153">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="d982e-153">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="d982e-154">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="d982e-154">Helpdesk agent</span></span>| <span data-ttu-id="d982e-155">\*    顧客の検索と表示</span><span class="sxs-lookup"><span data-stu-id="d982e-155">\*    Search for and view a customer</span></span>
||<span data-ttu-id="d982e-156">\*    顧客の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="d982e-156">\*    Edit customer details</span></span>
||<span data-ttu-id="d982e-157">\*    請求またはサブスクリプション管理に関する顧客の問題の解決サポート</span><span class="sxs-lookup"><span data-stu-id="d982e-157">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="d982e-158">\*    顧客の代理としてのサポート要求</span><span class="sxs-lookup"><span data-stu-id="d982e-158">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="d982e-159">\*    顧客の代理としてのサブスクリプションと請求に関する問題の管理</span><span class="sxs-lookup"><span data-stu-id="d982e-159">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="d982e-160">コントロール パネル ベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="d982e-160">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="d982e-161">(CSP ロールと非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="d982e-161">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="d982e-162">CPV は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムとパートナー センター API を統合するために使用するアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="d982e-162">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="d982e-163">**Role**</span><span class="sxs-lookup"><span data-stu-id="d982e-163">**Role**</span></span>   |<span data-ttu-id="d982e-164">**できること**</span><span class="sxs-lookup"><span data-stu-id="d982e-164">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="d982e-165">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-165">Global admin</span></span>| <span data-ttu-id="d982e-166">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="d982e-166">View and manage your CPV profile</span></span>|
||<span data-ttu-id="d982e-167">CPV 機能にアクセスする必要があるユーザーの表示と管理</span><span class="sxs-lookup"><span data-stu-id="d982e-167">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="d982e-168">ゲスト ユーザー (AAD テナントに追加される必要があります)</span><span class="sxs-lookup"><span data-stu-id="d982e-168">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="d982e-169">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="d982e-169">**Guest user**</span></span>   | <span data-ttu-id="d982e-170">**ロール**</span><span class="sxs-lookup"><span data-stu-id="d982e-170">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="d982e-171">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-171">MPN partner admin</span></span>|
||<span data-ttu-id="d982e-172">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-172">Accounts admin</span></span>|
||<span data-ttu-id="d982e-173">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-173">Incentives admin</span></span>|
||<span data-ttu-id="d982e-174">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-174">Business profile admin</span></span>|
||<span data-ttu-id="d982e-175">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-175">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="d982e-176">MPN メンバーシップと会社の管理 (AAD 以外のロール: これらのロールは、テナントではなく会社の業務を管理します)</span><span class="sxs-lookup"><span data-stu-id="d982e-176">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="d982e-177">**Role**</span><span class="sxs-lookup"><span data-stu-id="d982e-177">**Role**</span></span> | <span data-ttu-id="d982e-178">**できること**</span><span class="sxs-lookup"><span data-stu-id="d982e-178">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="d982e-179">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-179">MPN partner admin</span></span>|<span data-ttu-id="d982e-180">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d982e-180">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="d982e-181">\*    法的プロファイル、企業プロファイル、ビジネス プロファイル、MPN プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="d982e-181">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="d982e-182">\*    ユーザーの詳細およびスキル データの表示</span><span class="sxs-lookup"><span data-stu-id="d982e-182">\*    View user details and their skills data</span></span>
||<span data-ttu-id="d982e-183">\*    コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="d982e-183">\*    View competencies</span></span>
||<span data-ttu-id="d982e-184">\*    特典の表示と管理</span><span class="sxs-lookup"><span data-stu-id="d982e-184">\*    View and manage benefits</span></span>
||<span data-ttu-id="d982e-185">\*    MPN オファーの表示と購入</span><span class="sxs-lookup"><span data-stu-id="d982e-185">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="d982e-186">\*    MPN オファーの注文履歴と請求書の表示</span><span class="sxs-lookup"><span data-stu-id="d982e-186">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="d982e-187">\*    パートナー貢献度インジケーター データの表示</span><span class="sxs-lookup"><span data-stu-id="d982e-187">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="d982e-188">\*    利用券検証ツールでの作業</span><span class="sxs-lookup"><span data-stu-id="d982e-188">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="d982e-189">\*    顧客データ分析の表示</span><span class="sxs-lookup"><span data-stu-id="d982e-189">\*    View customer data analytics</span></span>
||<span data-ttu-id="d982e-190">\*    会社内の他のユーザー ロールを表示しますが、ロールを割り当てることはできません</span><span class="sxs-lookup"><span data-stu-id="d982e-190">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="d982e-191">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-191">Account admin</span></span>| <span data-ttu-id="d982e-192">場所の追加</span><span class="sxs-lookup"><span data-stu-id="d982e-192">Add locations</span></span>
|| <span data-ttu-id="d982e-193">管理対象のアカウントに関連するプロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="d982e-193">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="d982e-194">\*    テナント内のユーザーに対するロールの非 AAD ロールへの割り当て</span><span class="sxs-lookup"><span data-stu-id="d982e-194">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="d982e-195">\*    プログラムへの場所の登録</span><span class="sxs-lookup"><span data-stu-id="d982e-195">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="d982e-196">紹介の管理</span><span class="sxs-lookup"><span data-stu-id="d982e-196">Manage referrals</span></span> 

|<span data-ttu-id="d982e-197">**Role**</span><span class="sxs-lookup"><span data-stu-id="d982e-197">**Role**</span></span>|<span data-ttu-id="d982e-198">**できること**</span><span class="sxs-lookup"><span data-stu-id="d982e-198">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="d982e-199">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-199">Referrals admin</span></span>       |<span data-ttu-id="d982e-200">\*    ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d982e-200">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="d982e-201">\*    紹介の受信と管理</span><span class="sxs-lookup"><span data-stu-id="d982e-201">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="d982e-202">\*    共同販売の紹介の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d982e-202">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="d982e-203">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d982e-203">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="d982e-204">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-204">Business profile admin</span></span>   |<span data-ttu-id="d982e-205">\*    ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d982e-205">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="d982e-206">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="d982e-206">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="d982e-207">インセンティブの管理</span><span class="sxs-lookup"><span data-stu-id="d982e-207">Manage incentives</span></span> 

|<span data-ttu-id="d982e-208">**Role**</span><span class="sxs-lookup"><span data-stu-id="d982e-208">**Role**</span></span> | <span data-ttu-id="d982e-209">**できること**</span><span class="sxs-lookup"><span data-stu-id="d982e-209">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="d982e-210">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="d982e-210">Incentives admin</span></span>|<span data-ttu-id="d982e-211">\*    インセンティブの開始と管理</span><span class="sxs-lookup"><span data-stu-id="d982e-211">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="d982e-212">\*    インセンティブ プログラムのすべての側面の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="d982e-212">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="d982e-213">\*    銀行および税の詳細情報の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="d982e-213">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="d982e-214">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="d982e-214">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="d982e-215">\*    サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="d982e-215">\*    Access support</span></span>
||<span data-ttu-id="d982e-216">\*    インセンティブ支払いについての議論</span><span class="sxs-lookup"><span data-stu-id="d982e-216">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="d982e-217">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="d982e-217">Incentives user</span></span>|<span data-ttu-id="d982e-218">\*    インセンティブ プログラムを表示可能</span><span class="sxs-lookup"><span data-stu-id="d982e-218">\*    Can view incentives programs</span></span>
||<span data-ttu-id="d982e-219">\*    インセンティブの申請の表示と開始が可能</span><span class="sxs-lookup"><span data-stu-id="d982e-219">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="d982e-220">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="d982e-220">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="d982e-221">\*    サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="d982e-221">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="d982e-222">パートナー センター インサイト データの表示</span><span class="sxs-lookup"><span data-stu-id="d982e-222">View Partner Center Insights data</span></span>

|<span data-ttu-id="d982e-223">**Role**</span><span class="sxs-lookup"><span data-stu-id="d982e-223">**Role**</span></span> | <span data-ttu-id="d982e-224">**できること**</span><span class="sxs-lookup"><span data-stu-id="d982e-224">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="d982e-225">エグゼクティブ レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="d982e-225">Executive report viewer</span></span>|<span data-ttu-id="d982e-226">すべてのレポートデータセットへのアクセス</span><span class="sxs-lookup"><span data-stu-id="d982e-226">Access to all reporting datasets</span></span>|
|<span data-ttu-id="d982e-227">レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="d982e-227">Report viewer</span></span>|<span data-ttu-id="d982e-228">収益、顧客、従業員の個人データを除くデータ レポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="d982e-228">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    