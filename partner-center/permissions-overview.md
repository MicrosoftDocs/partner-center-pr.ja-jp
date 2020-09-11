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
ms.openlocfilehash: 2e8608c194057ea811890c9c575f8964b63564f0
ms.sourcegitcommit: bcd0c09d3acd5eae4fbfca7ea6614a54d203eff6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2020
ms.locfileid: "89490600"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="3dd67-103">パートナー センターで作業する必要がある会社のユーザーにユーザーのロールとアクセス許可を割り当てる</span><span class="sxs-lookup"><span data-stu-id="3dd67-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="3dd67-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="3dd67-104">**Appropriate roles**</span></span>

- <span data-ttu-id="3dd67-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-105">Global admin</span></span>
- <span data-ttu-id="3dd67-106">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-106">User admin</span></span>
- <span data-ttu-id="3dd67-107">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-107">MPN partner admin</span></span>

<span data-ttu-id="3dd67-108">貴社の正式名称や法的住所、サポートの詳細、税金の除外の申告、銀行情報、主要な連絡先など、パートナー プロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="3dd67-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="3dd67-109">次のステップ:ユーザーにパスワードとロールを設定させて、ユーザーがパートナー センターでの作業を開始できるようにします。</span><span class="sxs-lookup"><span data-stu-id="3dd67-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="3dd67-110">パートナー センターで作業できるように従業員を設定する</span><span class="sxs-lookup"><span data-stu-id="3dd67-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="3dd67-111">ユーザーに付与するロールとアクセス許可によって、パートナー センターでのユーザーのアクセスの種類が決まります。</span><span class="sxs-lookup"><span data-stu-id="3dd67-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="3dd67-112">ロールは、貴社のビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="3dd67-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="3dd67-113">たとえば、貴社のビジネスがクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、グローバル管理者などの標準の Azure AD テナント管理ロールだけでなく、CSP プログラムに固有のロールも必要です。</span><span class="sxs-lookup"><span data-stu-id="3dd67-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="3dd67-114">各プログラムには、それに固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="3dd67-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="3dd67-115">Azure Active Directory (AAD) テナント ロールには、グローバル管理者、ユーザー管理者、および CSP のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="3dd67-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="3dd67-116">AAD 以外のロールはテナントを管理しないロールであり、MPN 管理者、ビジネス プロファイル管理者、紹介管理者、インセンティブ管理者、およびインセンティブ ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="3dd67-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="3dd67-117">パートナー センターで商取引を管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="3dd67-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="3dd67-118">**Role**</span><span class="sxs-lookup"><span data-stu-id="3dd67-118">**Role**</span></span>|<span data-ttu-id="3dd67-119">**できること**</span><span class="sxs-lookup"><span data-stu-id="3dd67-119">**What they can do**</span></span>|<span data-ttu-id="3dd67-120">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="3dd67-120">**Learn more**</span></span>|
|----------------------------------|---|:---------------------------------|
|<span data-ttu-id="3dd67-121">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-121">Global admin</span></span>|<span data-ttu-id="3dd67-122">\*    すべての特権を備えたすべての Microsoft アカウントまたはサービスへのアクセスが可能</span><span class="sxs-lookup"><span data-stu-id="3dd67-122">\*    Can access all Microsoft account/services with full privileges</span></span>|[<span data-ttu-id="3dd67-123">パートナー センター アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-123">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
|      |<span data-ttu-id="3dd67-124">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="3dd67-124">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="3dd67-125">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-125">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="3dd67-126">\*    契約、価格表、オファーの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-126">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="3dd67-127">\*    パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-127">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="3dd67-128">課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-128">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="3dd67-129">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-129">User management admin</span></span>   | <span data-ttu-id="3dd67-130">\*    ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-130">\*    View, create, and manage users</span></span>|[<span data-ttu-id="3dd67-131">パートナー センターで Microsoft Partner Network メンバーシップの特典とプランを管理する</span><span class="sxs-lookup"><span data-stu-id="3dd67-131">Manage your Microsoft Partner Network membership benefits and offers in Partner Center</span></span>](manage-your-partner-network-benefits.md)
||<span data-ttu-id="3dd67-132">\*    すべてのパートナー プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-132">\*    View all partner profiles</span></span>
||<span data-ttu-id="3dd67-133">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="3dd67-133">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="3dd67-134">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-134">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="3dd67-135">課金管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-135">Billing admin</span></span> | <span data-ttu-id="3dd67-136">- 課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-136">- View, create, and manage billing, invoices, and recon files</span></span>|[<span data-ttu-id="3dd67-137">請求書の記載事項</span><span class="sxs-lookup"><span data-stu-id="3dd67-137">Read your bill</span></span>](billing.md)
||<span data-ttu-id="3dd67-138">\*    価格の表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-138">\*    View pricing</span></span>
||<span data-ttu-id="3dd67-139">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="3dd67-139">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="3dd67-140">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-140">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="3dd67-141">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="3dd67-141">Default user</span></span>|  <span data-ttu-id="3dd67-142">マイ プロフィールの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-142">View My profile</span></span>   |[<span data-ttu-id="3dd67-143">パスワードをリセットする</span><span class="sxs-lookup"><span data-stu-id="3dd67-143">Reset your password</span></span>](reset-my-pasword.md)
|<span data-ttu-id="3dd67-144">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="3dd67-144">Admin agent</span></span> | <span data-ttu-id="3dd67-145">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-145">\*    Customer management</span></span>|[<span data-ttu-id="3dd67-146">パートナー センターでリセラー パートナーの顧客アカウントのセットアップと管理を行う</span><span class="sxs-lookup"><span data-stu-id="3dd67-146">Customer account setup and management for reseller partners in Partner Center</span></span>](customer-accounts.md)
||<span data-ttu-id="3dd67-147">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="3dd67-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="3dd67-148">\*    プロファイルの作成とデバイスへの適用</span><span class="sxs-lookup"><span data-stu-id="3dd67-148">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="3dd67-149">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-149">\*    Subscription management</span></span>
||<span data-ttu-id="3dd67-150">\*    顧客のためのサービスの正常性とサービス要求</span><span class="sxs-lookup"><span data-stu-id="3dd67-150">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="3dd67-151">\*    代理管理者特権の要求</span><span class="sxs-lookup"><span data-stu-id="3dd67-151">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="3dd67-152">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="3dd67-153">\*    請求</span><span class="sxs-lookup"><span data-stu-id="3dd67-153">\*    Billing</span></span>
||<span data-ttu-id="3dd67-154">\*    顧客の代理としての管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-154">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="3dd67-155">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="3dd67-155">\*    Register a value added reseller</span></span>
||<span data-ttu-id="3dd67-156">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="3dd67-156">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="3dd67-157">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-157">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="3dd67-158">販売代理店</span><span class="sxs-lookup"><span data-stu-id="3dd67-158">Sales agent</span></span> | <span data-ttu-id="3dd67-159">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-159">\*    Customer management</span></span>|[<span data-ttu-id="3dd67-160">顧客に課金サポートを提供し、請求に関する質問に答える</span><span class="sxs-lookup"><span data-stu-id="3dd67-160">Provide billing support for your customers and help answer their billing questions</span></span>](provide-billing-support.md)
||<span data-ttu-id="3dd67-161">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="3dd67-161">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="3dd67-162">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-162">\*    Subscription management</span></span>
||<span data-ttu-id="3dd67-163">\*    サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-163">\*    View support tickets</span></span>
||<span data-ttu-id="3dd67-164">\*    顧客との再販業者関係の要求</span><span class="sxs-lookup"><span data-stu-id="3dd67-164">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="3dd67-165">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-165">\*    View pricing and offers</span></span>
||<span data-ttu-id="3dd67-166">\*    潜在顧客の管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-166">\*    Manage customer leads</span></span>
||<span data-ttu-id="3dd67-167">\*    顧客契約の表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-167">\*    View the customer agreement</span></span>
||<span data-ttu-id="3dd67-168">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="3dd67-168">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="3dd67-169">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="3dd67-169">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="3dd67-170">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-170">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="3dd67-171">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="3dd67-171">Helpdesk agent</span></span>| <span data-ttu-id="3dd67-172">\*    顧客の検索と表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-172">\*    Search for and view a customer</span></span>|[<span data-ttu-id="3dd67-173">Microsoft への問題のエスカレーション、および Microsoft へのエスカレーションに適した問題の見極め方</span><span class="sxs-lookup"><span data-stu-id="3dd67-173">Escalate problems to Microsoft and learn which issues are more-suited to Microsoft escalation</span></span>](escalate-problems-to-microsoft.md)
||<span data-ttu-id="3dd67-174">\*    顧客の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="3dd67-174">\*    Edit customer details</span></span>
||<span data-ttu-id="3dd67-175">\*    請求またはサブスクリプション管理に関する顧客の問題の解決サポート</span><span class="sxs-lookup"><span data-stu-id="3dd67-175">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="3dd67-176">\*    顧客の代理としてのサポート要求</span><span class="sxs-lookup"><span data-stu-id="3dd67-176">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="3dd67-177">\*    顧客の代理としてのサブスクリプションと請求に関する問題の管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-177">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="3dd67-178">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="3dd67-178">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="3dd67-179">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-179">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="3dd67-180">コントロール パネル ベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="3dd67-180">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="3dd67-181">(CSP ロールと非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="3dd67-181">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="3dd67-182">CPV は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムとパートナー センター API を統合するために使用するアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="3dd67-182">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="3dd67-183">**Role**</span><span class="sxs-lookup"><span data-stu-id="3dd67-183">**Role**</span></span>   |<span data-ttu-id="3dd67-184">**できること**</span><span class="sxs-lookup"><span data-stu-id="3dd67-184">**What you can do**</span></span>|<span data-ttu-id="3dd67-185">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="3dd67-185">**Learn more**</span></span>|
|------------------------------|:----------------------------|----|
|<span data-ttu-id="3dd67-186">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-186">Global admin</span></span>| <span data-ttu-id="3dd67-187">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-187">View and manage your CPV profile</span></span>|[<span data-ttu-id="3dd67-188">CSP パートナー システムとパートナー センター API との統合を支援するためにコントロール パネル ベンダーとして登録する</span><span class="sxs-lookup"><span data-stu-id="3dd67-188">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>](enroll-as-cpv.md)
||<span data-ttu-id="3dd67-189">CPV 機能にアクセスする必要があるユーザーの表示と管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-189">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="3dd67-190">ゲスト ユーザー (AAD テナントに追加される必要があります)</span><span class="sxs-lookup"><span data-stu-id="3dd67-190">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="3dd67-191">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="3dd67-191">**Guest user**</span></span>   | <span data-ttu-id="3dd67-192">**ロール**</span><span class="sxs-lookup"><span data-stu-id="3dd67-192">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="3dd67-193">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-193">MPN partner admin</span></span>|
||<span data-ttu-id="3dd67-194">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-194">Accounts admin</span></span>|
||<span data-ttu-id="3dd67-195">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-195">Incentives admin</span></span>|
||<span data-ttu-id="3dd67-196">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-196">Business profile admin</span></span>|
||<span data-ttu-id="3dd67-197">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-197">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="3dd67-198">MPN メンバーシップと会社の管理 (AAD 以外のロール: これらのロールは、テナントではなく会社の業務を管理します)</span><span class="sxs-lookup"><span data-stu-id="3dd67-198">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="3dd67-199">**Role**</span><span class="sxs-lookup"><span data-stu-id="3dd67-199">**Role**</span></span> | <span data-ttu-id="3dd67-200">**できること**</span><span class="sxs-lookup"><span data-stu-id="3dd67-200">**What you can do**</span></span>|<span data-ttu-id="3dd67-201">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="3dd67-201">**Learn more**</span></span>|
|----------------------------|:----------------------------|-----|
|<span data-ttu-id="3dd67-202">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-202">MPN partner admin</span></span>|<span data-ttu-id="3dd67-203">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-203">\*    View, create, and manage partner service requests</span></span>|[<span data-ttu-id="3dd67-204">Microsoft Action Pack サブスクリプションや Silver コンピテンシーと Gold コンピテンシーを購入または更新する</span><span class="sxs-lookup"><span data-stu-id="3dd67-204">Buy or renew a Microsoft Action Pack subscription or silver and gold competencies</span></span>](mpn-get-action-pack.md)
||<span data-ttu-id="3dd67-205">\*    法的プロファイル、企業プロファイル、ビジネス プロファイル、MPN プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-205">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="3dd67-206">\*    ユーザーの詳細およびスキル データの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-206">\*    View user details and their skills data</span></span>
||<span data-ttu-id="3dd67-207">\*    コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-207">\*    View competencies</span></span>
||<span data-ttu-id="3dd67-208">\*    特典の表示と管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-208">\*    View and manage benefits</span></span>
||<span data-ttu-id="3dd67-209">\*    MPN オファーの表示と購入</span><span class="sxs-lookup"><span data-stu-id="3dd67-209">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="3dd67-210">\*    MPN オファーの注文履歴と請求書の表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-210">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="3dd67-211">\*    パートナー貢献度インジケーター データの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-211">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="3dd67-212">\*    利用券検証ツールでの作業</span><span class="sxs-lookup"><span data-stu-id="3dd67-212">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="3dd67-213">\*    顧客データ分析の表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-213">\*    View customer data analytics</span></span>
||<span data-ttu-id="3dd67-214">\*    会社内の他のユーザー ロールを表示しますが、ロールを割り当てることはできません</span><span class="sxs-lookup"><span data-stu-id="3dd67-214">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="3dd67-215">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="3dd67-215">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="3dd67-216">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-216">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="3dd67-217">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-217">Account admin</span></span>| <span data-ttu-id="3dd67-218">場所の追加</span><span class="sxs-lookup"><span data-stu-id="3dd67-218">Add locations</span></span>|[<span data-ttu-id="3dd67-219">場所の管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-219">Manage locations</span></span>](manage-locations.md)
|| <span data-ttu-id="3dd67-220">管理対象のアカウントに関連するプロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-220">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="3dd67-221">\*    テナント内のユーザーに対するロールの非 AAD ロールへの割り当て</span><span class="sxs-lookup"><span data-stu-id="3dd67-221">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="3dd67-222">\*    プログラムへの場所の登録</span><span class="sxs-lookup"><span data-stu-id="3dd67-222">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="3dd67-223">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="3dd67-223">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="3dd67-224">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-224">\*    View partner support tickets you create</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="3dd67-225">紹介の管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-225">Manage referrals</span></span> 

|<span data-ttu-id="3dd67-226">**Role**</span><span class="sxs-lookup"><span data-stu-id="3dd67-226">**Role**</span></span>|<span data-ttu-id="3dd67-227">**できること**</span><span class="sxs-lookup"><span data-stu-id="3dd67-227">**What you can do**</span></span>|<span data-ttu-id="3dd67-228">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="3dd67-228">**Learn more**</span></span>|
|-----------------------------|:------------------------|---|
|<span data-ttu-id="3dd67-229">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-229">Referrals admin</span></span>       |<span data-ttu-id="3dd67-230">\*    ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-230">\*    View, create, and manage business profiles</span></span>|[<span data-ttu-id="3dd67-231">顧客の問い合わせ、マーケティングに適した潜在顧客、販売に適した潜在顧客などのさまざまな潜在顧客を管理する</span><span class="sxs-lookup"><span data-stu-id="3dd67-231">Manage different leads like customer inquiries, marketing-qualified leads, and sales-qualified leads</span></span>](manage-leads.md)
||<span data-ttu-id="3dd67-232">\*    紹介の受信と管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-232">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="3dd67-233">\*    共同販売の紹介の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-233">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="3dd67-234">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-234">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="3dd67-235">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-235">Business profile admin</span></span>   |<span data-ttu-id="3dd67-236">\*    ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-236">\* View, create, and manage business profile</span></span> |[<span data-ttu-id="3dd67-237">ビジネス プロファイルの作成</span><span class="sxs-lookup"><span data-stu-id="3dd67-237">Create a business profile</span></span>](create-a-marketing-profile.md)
||<span data-ttu-id="3dd67-238">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-238">\*    View, create, and manage partner service requests</span></span>
||<span data-ttu-id="3dd67-239">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="3dd67-239">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="3dd67-240">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-240">\*    View partner support tickets you create</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="3dd67-241">インセンティブの管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-241">Manage incentives</span></span> 

|<span data-ttu-id="3dd67-242">**Role**</span><span class="sxs-lookup"><span data-stu-id="3dd67-242">**Role**</span></span> | <span data-ttu-id="3dd67-243">**できること**</span><span class="sxs-lookup"><span data-stu-id="3dd67-243">**What you can do**</span></span>|<span data-ttu-id="3dd67-244">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="3dd67-244">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="3dd67-245">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="3dd67-245">Incentives admin</span></span>|<span data-ttu-id="3dd67-246">\*    インセンティブの開始と管理</span><span class="sxs-lookup"><span data-stu-id="3dd67-246">\*    Initiates and manages incentives</span></span> |[<span data-ttu-id="3dd67-247">これらのリソースを使用してインセンティブを使い始める</span><span class="sxs-lookup"><span data-stu-id="3dd67-247">Use these resources to help you get started with incentives</span></span>](incentives-get-started-intro.md)
||<span data-ttu-id="3dd67-248">\*    インセンティブ プログラムのすべての側面の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="3dd67-248">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="3dd67-249">\*    銀行および税の詳細情報の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="3dd67-249">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="3dd67-250">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-250">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="3dd67-251">\*    サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="3dd67-251">\*    Access support</span></span>
||<span data-ttu-id="3dd67-252">\*    インセンティブ支払いについての議論</span><span class="sxs-lookup"><span data-stu-id="3dd67-252">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="3dd67-253">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="3dd67-253">Incentives user</span></span>|<span data-ttu-id="3dd67-254">\*    インセンティブ プログラムを表示可能</span><span class="sxs-lookup"><span data-stu-id="3dd67-254">\*    Can view incentives programs</span></span>
||<span data-ttu-id="3dd67-255">\*    インセンティブの申請の表示と開始が可能</span><span class="sxs-lookup"><span data-stu-id="3dd67-255">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="3dd67-256">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-256">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="3dd67-257">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="3dd67-257">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="3dd67-258">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-258">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="3dd67-259">パートナー センター インサイト データの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-259">View Partner Center Insights data</span></span>

|<span data-ttu-id="3dd67-260">**Role**</span><span class="sxs-lookup"><span data-stu-id="3dd67-260">**Role**</span></span> | <span data-ttu-id="3dd67-261">**できること**</span><span class="sxs-lookup"><span data-stu-id="3dd67-261">**What you can do**</span></span>|<span data-ttu-id="3dd67-262">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="3dd67-262">**Learn more**</span></span>|
|------------------------------|:-------------------------|---|
|<span data-ttu-id="3dd67-263">エグゼクティブ レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="3dd67-263">Executive report viewer</span></span>|<span data-ttu-id="3dd67-264">すべてのレポート データセットへのアクセス、パートナー サポート チケットの作成、作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-264">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|[<span data-ttu-id="3dd67-265">パートナー センターの分析情報で利用できる概要ダッシュボード レポート</span><span class="sxs-lookup"><span data-stu-id="3dd67-265">Overview dashboard reports available in Partner Center Insights</span></span>](pci-overview-report.md)
|<span data-ttu-id="3dd67-266">レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="3dd67-266">Report viewer</span></span>|<span data-ttu-id="3dd67-267">収益や顧客と従業員の個人データを除くデータ レポートへのアクセス、パートナー サポート チケットの作成、作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="3dd67-267">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|

## <a name="next-steps"></a><span data-ttu-id="3dd67-268">次のステップ</span><span class="sxs-lookup"><span data-stu-id="3dd67-268">Next steps</span></span>

- [<span data-ttu-id="3dd67-269">ユーザー アカウントの作成およびロールとアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="3dd67-269">Create user accounts and assign roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)
- [<span data-ttu-id="3dd67-270">新しいパートナー センター プログラムに登録する際のアカウント情報の確認</span><span class="sxs-lookup"><span data-stu-id="3dd67-270">Verify your account information when you enroll in a new Partner Center program</span></span>](verification-responses.md)










                                    
