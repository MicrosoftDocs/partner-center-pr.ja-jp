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
ms.openlocfilehash: c87e47efc6c94e4e53a031a983a4a4e528ddc012
ms.sourcegitcommit: 59bdf42f5282262835cb7ee2bd215bbddc7686d7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/06/2020
ms.locfileid: "87839187"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="cebb8-103">パートナー センターで作業する必要がある会社のユーザーにユーザーのロールとアクセス許可を割り当てる</span><span class="sxs-lookup"><span data-stu-id="cebb8-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="cebb8-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="cebb8-104">**Appropriate roles**</span></span>

- <span data-ttu-id="cebb8-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-105">Global admin</span></span>
- <span data-ttu-id="cebb8-106">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-106">User admin</span></span>
- <span data-ttu-id="cebb8-107">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-107">MPN partner admin</span></span>

<span data-ttu-id="cebb8-108">貴社の正式名称や法的住所、サポートの詳細、税金の除外の申告、銀行情報、主要な連絡先など、パートナー プロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="cebb8-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="cebb8-109">次のステップ:ユーザーにパスワードとロールを設定させて、ユーザーがパートナー センターでの作業を開始できるようにします。</span><span class="sxs-lookup"><span data-stu-id="cebb8-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="cebb8-110">パートナー センターで作業できるように従業員を設定する</span><span class="sxs-lookup"><span data-stu-id="cebb8-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="cebb8-111">ユーザーに付与するロールとアクセス許可によって、パートナー センターでのユーザーのアクセスの種類が決まります。</span><span class="sxs-lookup"><span data-stu-id="cebb8-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="cebb8-112">ロールは、貴社のビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="cebb8-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="cebb8-113">たとえば、貴社のビジネスがクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、グローバル管理者などの標準の Azure AD テナント管理ロールだけでなく、CSP プログラムに固有のロールも必要です。</span><span class="sxs-lookup"><span data-stu-id="cebb8-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="cebb8-114">各プログラムには、それに固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="cebb8-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="cebb8-115">Azure Active Directory (AAD) テナント ロールには、グローバル管理者、ユーザー管理者、および CSP のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="cebb8-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="cebb8-116">AAD 以外のロールはテナントを管理しないロールであり、MPN 管理者、ビジネス プロファイル管理者、紹介管理者、インセンティブ管理者、およびインセンティブ ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="cebb8-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="cebb8-117">パートナー センターで商取引を管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="cebb8-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="cebb8-118">**Role**</span><span class="sxs-lookup"><span data-stu-id="cebb8-118">**Role**</span></span>|<span data-ttu-id="cebb8-119">**できること**</span><span class="sxs-lookup"><span data-stu-id="cebb8-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="cebb8-120">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-120">Global admin</span></span>|<span data-ttu-id="cebb8-121">\*    すべての特権を備えたすべての Microsoft アカウントまたはサービスへのアクセスが可能</span><span class="sxs-lookup"><span data-stu-id="cebb8-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="cebb8-122">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="cebb8-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="cebb8-123">\*    契約、価格表、オファーの表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="cebb8-124">\*    パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="cebb8-125">課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="cebb8-126">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-126">User management admin</span></span>   | <span data-ttu-id="cebb8-127">\*    ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="cebb8-128">\*    すべてのパートナー プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="cebb8-129">\*    パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="cebb8-130">課金管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-130">Billing admin</span></span> | <span data-ttu-id="cebb8-131">- 課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-131">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="cebb8-132">\*    価格の表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-132">\*    View pricing</span></span>
|<span data-ttu-id="cebb8-133">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="cebb8-133">Default user</span></span>|  <span data-ttu-id="cebb8-134">マイ プロフィールの表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-134">View My profile</span></span>   |
|<span data-ttu-id="cebb8-135">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="cebb8-135">Admin agent</span></span> | <span data-ttu-id="cebb8-136">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-136">\*    Customer management</span></span>
||<span data-ttu-id="cebb8-137">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="cebb8-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="cebb8-138">\*    プロファイルの作成とデバイスへの適用</span><span class="sxs-lookup"><span data-stu-id="cebb8-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="cebb8-139">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-139">\*    Subscription management</span></span>
||<span data-ttu-id="cebb8-140">\*    顧客のためのサービスの正常性とサービス要求</span><span class="sxs-lookup"><span data-stu-id="cebb8-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="cebb8-141">\*    代理管理者特権の要求</span><span class="sxs-lookup"><span data-stu-id="cebb8-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="cebb8-142">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="cebb8-143">\*    請求</span><span class="sxs-lookup"><span data-stu-id="cebb8-143">\*    Billing</span></span>
||<span data-ttu-id="cebb8-144">\*    顧客の代理としての管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="cebb8-145">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="cebb8-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="cebb8-146">販売代理店</span><span class="sxs-lookup"><span data-stu-id="cebb8-146">Sales agent</span></span> | <span data-ttu-id="cebb8-147">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-147">\*    Customer management</span></span>
||<span data-ttu-id="cebb8-148">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="cebb8-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="cebb8-149">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-149">\*    Subscription management</span></span>
||<span data-ttu-id="cebb8-150">\*    サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-150">\*    View support tickets</span></span>
||<span data-ttu-id="cebb8-151">\*    顧客との再販業者関係の要求</span><span class="sxs-lookup"><span data-stu-id="cebb8-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="cebb8-152">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="cebb8-153">\*    潜在顧客の管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-153">\*    Manage customer leads</span></span>
||<span data-ttu-id="cebb8-154">\*    顧客契約の表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-154">\*    View the customer agreement</span></span>
||<span data-ttu-id="cebb8-155">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="cebb8-155">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="cebb8-156">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="cebb8-156">Helpdesk agent</span></span>| <span data-ttu-id="cebb8-157">\*    顧客の検索と表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-157">\*    Search for and view a customer</span></span>
||<span data-ttu-id="cebb8-158">\*    顧客の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="cebb8-158">\*    Edit customer details</span></span>
||<span data-ttu-id="cebb8-159">\*    請求またはサブスクリプション管理に関する顧客の問題の解決サポート</span><span class="sxs-lookup"><span data-stu-id="cebb8-159">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="cebb8-160">\*    顧客の代理としてのサポート要求</span><span class="sxs-lookup"><span data-stu-id="cebb8-160">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="cebb8-161">\*    顧客の代理としてのサブスクリプションと請求に関する問題の管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-161">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="cebb8-162">コントロール パネル ベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="cebb8-162">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="cebb8-163">(CSP ロールと非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="cebb8-163">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="cebb8-164">CPV は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムとパートナー センター API を統合するために使用するアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="cebb8-164">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="cebb8-165">**Role**</span><span class="sxs-lookup"><span data-stu-id="cebb8-165">**Role**</span></span>   |<span data-ttu-id="cebb8-166">**できること**</span><span class="sxs-lookup"><span data-stu-id="cebb8-166">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="cebb8-167">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-167">Global admin</span></span>| <span data-ttu-id="cebb8-168">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-168">View and manage your CPV profile</span></span>|
||<span data-ttu-id="cebb8-169">CPV 機能にアクセスする必要があるユーザーの表示と管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-169">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="cebb8-170">ゲスト ユーザー (AAD テナントに追加される必要があります)</span><span class="sxs-lookup"><span data-stu-id="cebb8-170">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="cebb8-171">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="cebb8-171">**Guest user**</span></span>   | <span data-ttu-id="cebb8-172">**ロール**</span><span class="sxs-lookup"><span data-stu-id="cebb8-172">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="cebb8-173">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-173">MPN partner admin</span></span>|
||<span data-ttu-id="cebb8-174">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-174">Accounts admin</span></span>|
||<span data-ttu-id="cebb8-175">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-175">Incentives admin</span></span>|
||<span data-ttu-id="cebb8-176">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-176">Business profile admin</span></span>|
||<span data-ttu-id="cebb8-177">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-177">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="cebb8-178">MPN メンバーシップと会社の管理 (AAD 以外のロール: これらのロールは、テナントではなく会社の業務を管理します)</span><span class="sxs-lookup"><span data-stu-id="cebb8-178">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="cebb8-179">**Role**</span><span class="sxs-lookup"><span data-stu-id="cebb8-179">**Role**</span></span> | <span data-ttu-id="cebb8-180">**できること**</span><span class="sxs-lookup"><span data-stu-id="cebb8-180">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="cebb8-181">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-181">MPN partner admin</span></span>|<span data-ttu-id="cebb8-182">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-182">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="cebb8-183">\*    法的プロファイル、企業プロファイル、ビジネス プロファイル、MPN プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-183">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="cebb8-184">\*    ユーザーの詳細およびスキル データの表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-184">\*    View user details and their skills data</span></span>
||<span data-ttu-id="cebb8-185">\*    コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-185">\*    View competencies</span></span>
||<span data-ttu-id="cebb8-186">\*    特典の表示と管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-186">\*    View and manage benefits</span></span>
||<span data-ttu-id="cebb8-187">\*    MPN オファーの表示と購入</span><span class="sxs-lookup"><span data-stu-id="cebb8-187">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="cebb8-188">\*    MPN オファーの注文履歴と請求書の表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-188">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="cebb8-189">\*    パートナー貢献度インジケーター データの表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-189">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="cebb8-190">\*    利用券検証ツールでの作業</span><span class="sxs-lookup"><span data-stu-id="cebb8-190">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="cebb8-191">\*    顧客データ分析の表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-191">\*    View customer data analytics</span></span>
||<span data-ttu-id="cebb8-192">\*    会社内の他のユーザー ロールを表示しますが、ロールを割り当てることはできません</span><span class="sxs-lookup"><span data-stu-id="cebb8-192">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="cebb8-193">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-193">Account admin</span></span>| <span data-ttu-id="cebb8-194">場所の追加</span><span class="sxs-lookup"><span data-stu-id="cebb8-194">Add locations</span></span>
|| <span data-ttu-id="cebb8-195">管理対象のアカウントに関連するプロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-195">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="cebb8-196">\*    テナント内のユーザーに対するロールの非 AAD ロールへの割り当て</span><span class="sxs-lookup"><span data-stu-id="cebb8-196">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="cebb8-197">\*    プログラムへの場所の登録</span><span class="sxs-lookup"><span data-stu-id="cebb8-197">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="cebb8-198">紹介の管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-198">Manage referrals</span></span> 

|<span data-ttu-id="cebb8-199">**Role**</span><span class="sxs-lookup"><span data-stu-id="cebb8-199">**Role**</span></span>|<span data-ttu-id="cebb8-200">**できること**</span><span class="sxs-lookup"><span data-stu-id="cebb8-200">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="cebb8-201">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-201">Referrals admin</span></span>       |<span data-ttu-id="cebb8-202">\*    ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-202">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="cebb8-203">\*    紹介の受信と管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-203">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="cebb8-204">\*    共同販売の紹介の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-204">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="cebb8-205">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-205">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="cebb8-206">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-206">Business profile admin</span></span>   |<span data-ttu-id="cebb8-207">\*    ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-207">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="cebb8-208">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-208">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="cebb8-209">インセンティブの管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-209">Manage incentives</span></span> 

|<span data-ttu-id="cebb8-210">**Role**</span><span class="sxs-lookup"><span data-stu-id="cebb8-210">**Role**</span></span> | <span data-ttu-id="cebb8-211">**できること**</span><span class="sxs-lookup"><span data-stu-id="cebb8-211">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="cebb8-212">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="cebb8-212">Incentives admin</span></span>|<span data-ttu-id="cebb8-213">\*    インセンティブの開始と管理</span><span class="sxs-lookup"><span data-stu-id="cebb8-213">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="cebb8-214">\*    インセンティブ プログラムのすべての側面の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="cebb8-214">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="cebb8-215">\*    銀行および税の詳細情報の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="cebb8-215">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="cebb8-216">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-216">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="cebb8-217">\*    サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="cebb8-217">\*    Access support</span></span>
||<span data-ttu-id="cebb8-218">\*    インセンティブ支払いについての議論</span><span class="sxs-lookup"><span data-stu-id="cebb8-218">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="cebb8-219">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="cebb8-219">Incentives user</span></span>|<span data-ttu-id="cebb8-220">\*    インセンティブ プログラムを表示可能</span><span class="sxs-lookup"><span data-stu-id="cebb8-220">\*    Can view incentives programs</span></span>
||<span data-ttu-id="cebb8-221">\*    インセンティブの申請の表示と開始が可能</span><span class="sxs-lookup"><span data-stu-id="cebb8-221">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="cebb8-222">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-222">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="cebb8-223">\*    サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="cebb8-223">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="cebb8-224">パートナー センター インサイト データの表示</span><span class="sxs-lookup"><span data-stu-id="cebb8-224">View Partner Center Insights data</span></span>

|<span data-ttu-id="cebb8-225">**Role**</span><span class="sxs-lookup"><span data-stu-id="cebb8-225">**Role**</span></span> | <span data-ttu-id="cebb8-226">**できること**</span><span class="sxs-lookup"><span data-stu-id="cebb8-226">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="cebb8-227">エグゼクティブ レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="cebb8-227">Executive report viewer</span></span>|<span data-ttu-id="cebb8-228">すべてのレポートデータセットへのアクセス</span><span class="sxs-lookup"><span data-stu-id="cebb8-228">Access to all reporting datasets</span></span>|
|<span data-ttu-id="cebb8-229">レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="cebb8-229">Report viewer</span></span>|<span data-ttu-id="cebb8-230">収益、顧客、従業員の個人データを除くデータ レポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="cebb8-230">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    
