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
ms.openlocfilehash: 3feb4e678381b6fa5398bf3b3d89f6e4286e6ff1
ms.sourcegitcommit: 4feae1ea7fd3077934e3c931a5de801c96a4f995
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2020
ms.locfileid: "89040768"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="a35ea-103">パートナー センターで作業する必要がある会社のユーザーにユーザーのロールとアクセス許可を割り当てる</span><span class="sxs-lookup"><span data-stu-id="a35ea-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="a35ea-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="a35ea-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a35ea-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-105">Global admin</span></span>
- <span data-ttu-id="a35ea-106">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-106">User admin</span></span>
- <span data-ttu-id="a35ea-107">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-107">MPN partner admin</span></span>

<span data-ttu-id="a35ea-108">貴社の正式名称や法的住所、サポートの詳細、税金の除外の申告、銀行情報、主要な連絡先など、パートナー プロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="a35ea-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="a35ea-109">次のステップ:ユーザーにパスワードとロールを設定させて、ユーザーがパートナー センターでの作業を開始できるようにします。</span><span class="sxs-lookup"><span data-stu-id="a35ea-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="a35ea-110">パートナー センターで作業できるように従業員を設定する</span><span class="sxs-lookup"><span data-stu-id="a35ea-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="a35ea-111">ユーザーに付与するロールとアクセス許可によって、パートナー センターでのユーザーのアクセスの種類が決まります。</span><span class="sxs-lookup"><span data-stu-id="a35ea-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="a35ea-112">ロールは、貴社のビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="a35ea-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="a35ea-113">たとえば、貴社のビジネスがクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、グローバル管理者などの標準の Azure AD テナント管理ロールだけでなく、CSP プログラムに固有のロールも必要です。</span><span class="sxs-lookup"><span data-stu-id="a35ea-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="a35ea-114">各プログラムには、それに固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="a35ea-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="a35ea-115">Azure Active Directory (AAD) テナント ロールには、グローバル管理者、ユーザー管理者、および CSP のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="a35ea-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="a35ea-116">AAD 以外のロールはテナントを管理しないロールであり、MPN 管理者、ビジネス プロファイル管理者、紹介管理者、インセンティブ管理者、およびインセンティブ ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="a35ea-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="a35ea-117">パートナー センターで商取引を管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="a35ea-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="a35ea-118">**Role**</span><span class="sxs-lookup"><span data-stu-id="a35ea-118">**Role**</span></span>|<span data-ttu-id="a35ea-119">**できること**</span><span class="sxs-lookup"><span data-stu-id="a35ea-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="a35ea-120">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-120">Global admin</span></span>|<span data-ttu-id="a35ea-121">\*    すべての特権を備えたすべての Microsoft アカウントまたはサービスへのアクセスが可能</span><span class="sxs-lookup"><span data-stu-id="a35ea-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="a35ea-122">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="a35ea-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a35ea-123">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-123">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="a35ea-124">\*    契約、価格表、オファーの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="a35ea-125">\*    パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="a35ea-126">課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="a35ea-127">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-127">User management admin</span></span>   | <span data-ttu-id="a35ea-128">\*    ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="a35ea-129">\*    すべてのパートナー プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="a35ea-130">\*    パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-130">\*    View, create, and manage partner users</span></span>  |
||<span data-ttu-id="a35ea-131">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="a35ea-131">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a35ea-132">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-132">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="a35ea-133">課金管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-133">Billing admin</span></span> | <span data-ttu-id="a35ea-134">- 課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-134">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="a35ea-135">\*    価格の表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-135">\*    View pricing</span></span>
||<span data-ttu-id="a35ea-136">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="a35ea-136">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a35ea-137">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-137">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="a35ea-138">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="a35ea-138">Default user</span></span>|  <span data-ttu-id="a35ea-139">マイ プロフィールの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-139">View My profile</span></span>   |
|<span data-ttu-id="a35ea-140">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="a35ea-140">Admin agent</span></span> | <span data-ttu-id="a35ea-141">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-141">\*    Customer management</span></span>
||<span data-ttu-id="a35ea-142">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="a35ea-142">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="a35ea-143">\*    プロファイルの作成とデバイスへの適用</span><span class="sxs-lookup"><span data-stu-id="a35ea-143">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="a35ea-144">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-144">\*    Subscription management</span></span>
||<span data-ttu-id="a35ea-145">\*    顧客のためのサービスの正常性とサービス要求</span><span class="sxs-lookup"><span data-stu-id="a35ea-145">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="a35ea-146">\*    代理管理者特権の要求</span><span class="sxs-lookup"><span data-stu-id="a35ea-146">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="a35ea-147">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-147">\*    View pricing and offers</span></span>
||<span data-ttu-id="a35ea-148">\*    請求</span><span class="sxs-lookup"><span data-stu-id="a35ea-148">\*    Billing</span></span>
||<span data-ttu-id="a35ea-149">\*    顧客の代理としての管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-149">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="a35ea-150">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="a35ea-150">\*    Register a value added reseller</span></span>
||<span data-ttu-id="a35ea-151">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="a35ea-151">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a35ea-152">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-152">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="a35ea-153">販売代理店</span><span class="sxs-lookup"><span data-stu-id="a35ea-153">Sales agent</span></span> | <span data-ttu-id="a35ea-154">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-154">\*    Customer management</span></span>
||<span data-ttu-id="a35ea-155">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="a35ea-155">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="a35ea-156">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-156">\*    Subscription management</span></span>
||<span data-ttu-id="a35ea-157">\*    サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-157">\*    View support tickets</span></span>
||<span data-ttu-id="a35ea-158">\*    顧客との再販業者関係の要求</span><span class="sxs-lookup"><span data-stu-id="a35ea-158">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="a35ea-159">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-159">\*    View pricing and offers</span></span>
||<span data-ttu-id="a35ea-160">\*    潜在顧客の管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-160">\*    Manage customer leads</span></span>
||<span data-ttu-id="a35ea-161">\*    顧客契約の表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-161">\*    View the customer agreement</span></span>
||<span data-ttu-id="a35ea-162">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="a35ea-162">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="a35ea-163">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="a35ea-163">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a35ea-164">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-164">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="a35ea-165">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="a35ea-165">Helpdesk agent</span></span>| <span data-ttu-id="a35ea-166">\*    顧客の検索と表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-166">\*    Search for and view a customer</span></span>
||<span data-ttu-id="a35ea-167">\*    顧客の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="a35ea-167">\*    Edit customer details</span></span>
||<span data-ttu-id="a35ea-168">\*    請求またはサブスクリプション管理に関する顧客の問題の解決サポート</span><span class="sxs-lookup"><span data-stu-id="a35ea-168">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="a35ea-169">\*    顧客の代理としてのサポート要求</span><span class="sxs-lookup"><span data-stu-id="a35ea-169">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="a35ea-170">\*    顧客の代理としてのサブスクリプションと請求に関する問題の管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-170">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="a35ea-171">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="a35ea-171">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a35ea-172">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-172">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="a35ea-173">コントロール パネル ベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="a35ea-173">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="a35ea-174">(CSP ロールと非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="a35ea-174">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="a35ea-175">CPV は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムとパートナー センター API を統合するために使用するアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="a35ea-175">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="a35ea-176">**Role**</span><span class="sxs-lookup"><span data-stu-id="a35ea-176">**Role**</span></span>   |<span data-ttu-id="a35ea-177">**できること**</span><span class="sxs-lookup"><span data-stu-id="a35ea-177">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="a35ea-178">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-178">Global admin</span></span>| <span data-ttu-id="a35ea-179">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-179">View and manage your CPV profile</span></span>|
||<span data-ttu-id="a35ea-180">CPV 機能にアクセスする必要があるユーザーの表示と管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-180">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="a35ea-181">ゲスト ユーザー (AAD テナントに追加される必要があります)</span><span class="sxs-lookup"><span data-stu-id="a35ea-181">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="a35ea-182">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="a35ea-182">**Guest user**</span></span>   | <span data-ttu-id="a35ea-183">**ロール**</span><span class="sxs-lookup"><span data-stu-id="a35ea-183">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="a35ea-184">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-184">MPN partner admin</span></span>|
||<span data-ttu-id="a35ea-185">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-185">Accounts admin</span></span>|
||<span data-ttu-id="a35ea-186">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-186">Incentives admin</span></span>|
||<span data-ttu-id="a35ea-187">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-187">Business profile admin</span></span>|
||<span data-ttu-id="a35ea-188">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-188">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="a35ea-189">MPN メンバーシップと会社の管理 (AAD 以外のロール: これらのロールは、テナントではなく会社の業務を管理します)</span><span class="sxs-lookup"><span data-stu-id="a35ea-189">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="a35ea-190">**Role**</span><span class="sxs-lookup"><span data-stu-id="a35ea-190">**Role**</span></span> | <span data-ttu-id="a35ea-191">**できること**</span><span class="sxs-lookup"><span data-stu-id="a35ea-191">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="a35ea-192">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-192">MPN partner admin</span></span>|<span data-ttu-id="a35ea-193">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-193">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="a35ea-194">\*    法的プロファイル、企業プロファイル、ビジネス プロファイル、MPN プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-194">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="a35ea-195">\*    ユーザーの詳細およびスキル データの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-195">\*    View user details and their skills data</span></span>
||<span data-ttu-id="a35ea-196">\*    コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-196">\*    View competencies</span></span>
||<span data-ttu-id="a35ea-197">\*    特典の表示と管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-197">\*    View and manage benefits</span></span>
||<span data-ttu-id="a35ea-198">\*    MPN オファーの表示と購入</span><span class="sxs-lookup"><span data-stu-id="a35ea-198">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="a35ea-199">\*    MPN オファーの注文履歴と請求書の表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-199">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="a35ea-200">\*    パートナー貢献度インジケーター データの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-200">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="a35ea-201">\*    利用券検証ツールでの作業</span><span class="sxs-lookup"><span data-stu-id="a35ea-201">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="a35ea-202">\*    顧客データ分析の表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-202">\*    View customer data analytics</span></span>
||<span data-ttu-id="a35ea-203">\*    会社内の他のユーザー ロールを表示しますが、ロールを割り当てることはできません</span><span class="sxs-lookup"><span data-stu-id="a35ea-203">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="a35ea-204">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="a35ea-204">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a35ea-205">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-205">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="a35ea-206">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-206">Account admin</span></span>| <span data-ttu-id="a35ea-207">場所の追加</span><span class="sxs-lookup"><span data-stu-id="a35ea-207">Add locations</span></span>
|| <span data-ttu-id="a35ea-208">管理対象のアカウントに関連するプロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-208">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="a35ea-209">\*    テナント内のユーザーに対するロールの非 AAD ロールへの割り当て</span><span class="sxs-lookup"><span data-stu-id="a35ea-209">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="a35ea-210">\*    プログラムへの場所の登録</span><span class="sxs-lookup"><span data-stu-id="a35ea-210">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="a35ea-211">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="a35ea-211">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a35ea-212">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-212">\*    View partner support tickets you create</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="a35ea-213">紹介の管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-213">Manage referrals</span></span> 

|<span data-ttu-id="a35ea-214">**Role**</span><span class="sxs-lookup"><span data-stu-id="a35ea-214">**Role**</span></span>|<span data-ttu-id="a35ea-215">**できること**</span><span class="sxs-lookup"><span data-stu-id="a35ea-215">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="a35ea-216">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-216">Referrals admin</span></span>       |<span data-ttu-id="a35ea-217">\*    ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-217">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="a35ea-218">\*    紹介の受信と管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-218">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="a35ea-219">\*    共同販売の紹介の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-219">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="a35ea-220">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-220">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="a35ea-221">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-221">Business profile admin</span></span>   |<span data-ttu-id="a35ea-222">\*    ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-222">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="a35ea-223">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-223">\*    View, create, and manage partner service requests</span></span>
||<span data-ttu-id="a35ea-224">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="a35ea-224">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a35ea-225">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-225">\*    View partner support tickets you create</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="a35ea-226">インセンティブの管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-226">Manage incentives</span></span> 

|<span data-ttu-id="a35ea-227">**Role**</span><span class="sxs-lookup"><span data-stu-id="a35ea-227">**Role**</span></span> | <span data-ttu-id="a35ea-228">**できること**</span><span class="sxs-lookup"><span data-stu-id="a35ea-228">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="a35ea-229">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="a35ea-229">Incentives admin</span></span>|<span data-ttu-id="a35ea-230">\*    インセンティブの開始と管理</span><span class="sxs-lookup"><span data-stu-id="a35ea-230">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="a35ea-231">\*    インセンティブ プログラムのすべての側面の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="a35ea-231">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="a35ea-232">\*    銀行および税の詳細情報の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="a35ea-232">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="a35ea-233">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-233">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="a35ea-234">\*    サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="a35ea-234">\*    Access support</span></span>
||<span data-ttu-id="a35ea-235">\*    インセンティブ支払いについての議論</span><span class="sxs-lookup"><span data-stu-id="a35ea-235">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="a35ea-236">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="a35ea-236">Incentives user</span></span>|<span data-ttu-id="a35ea-237">\*    インセンティブ プログラムを表示可能</span><span class="sxs-lookup"><span data-stu-id="a35ea-237">\*    Can view incentives programs</span></span>
||<span data-ttu-id="a35ea-238">\*    インセンティブの申請の表示と開始が可能</span><span class="sxs-lookup"><span data-stu-id="a35ea-238">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="a35ea-239">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-239">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="a35ea-240">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="a35ea-240">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a35ea-241">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-241">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="a35ea-242">パートナー センター インサイト データの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-242">View Partner Center Insights data</span></span>

|<span data-ttu-id="a35ea-243">**Role**</span><span class="sxs-lookup"><span data-stu-id="a35ea-243">**Role**</span></span> | <span data-ttu-id="a35ea-244">**できること**</span><span class="sxs-lookup"><span data-stu-id="a35ea-244">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="a35ea-245">エグゼクティブ レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="a35ea-245">Executive report viewer</span></span>|<span data-ttu-id="a35ea-246">すべてのレポート データセットへのアクセス、パートナー サポート チケットの作成、作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-246">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|
|<span data-ttu-id="a35ea-247">レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="a35ea-247">Report viewer</span></span>|<span data-ttu-id="a35ea-248">収益や顧客と従業員の個人データを除くデータ レポートへのアクセス、パートナー サポート チケットの作成、作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="a35ea-248">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|












                                    
