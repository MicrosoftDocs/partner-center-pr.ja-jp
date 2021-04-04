---
title: ユーザーにロールとアクセス許可を割り当てる
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 商取引、紹介、インセンティブ、または MPN メンバーシップをパートナー センターで管理する、会社のユーザーに最適なロールについて説明します。
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: a6e6424dfb787bbe9510d47299f945309dd00528
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633915"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="48a8e-103">パートナー センターで作業する必要がある会社のユーザーにユーザーのロールとアクセス許可を割り当てる</span><span class="sxs-lookup"><span data-stu-id="48a8e-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="48a8e-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="48a8e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="48a8e-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="48a8e-105">Global admin</span></span>
- <span data-ttu-id="48a8e-106">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="48a8e-106">User management admin</span></span>
- <span data-ttu-id="48a8e-107">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="48a8e-107">MPN partner admin</span></span>

<span data-ttu-id="48a8e-108">貴社の正式名称や法的住所、サポートの詳細、税金の除外の申告、銀行情報、主要な連絡先など、パートナー プロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="48a8e-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="48a8e-109">次のステップ:ユーザーにパスワードとロールを設定させて、ユーザーがパートナー センターでの作業を開始できるようにします。</span><span class="sxs-lookup"><span data-stu-id="48a8e-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="48a8e-110">パートナー センターで作業できるように従業員を設定する</span><span class="sxs-lookup"><span data-stu-id="48a8e-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="48a8e-111">ユーザーに付与するロールとアクセス許可によって、パートナー センターでのユーザーのアクセスの種類が決まります。</span><span class="sxs-lookup"><span data-stu-id="48a8e-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="48a8e-112">ロールは、貴社のビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="48a8e-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="48a8e-113">たとえば、貴社のビジネスがクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、グローバル管理者などの標準の Azure Active Directory テナント管理ロールだけでなく、CSP プログラムに固有のロールも必要です。</span><span class="sxs-lookup"><span data-stu-id="48a8e-113">For example, if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure Active Directory tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="48a8e-114">各プログラムには、それに固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="48a8e-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="48a8e-115">Azure Active Directory テナント ロールには、グローバル管理者、ユーザー管理者、CSP のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="48a8e-115">Azure Active Directory tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="48a8e-116">Azure Active Directory 以外のロールはテナントを管理しないロールであり、MPN 管理者、ビジネス プロファイル管理者、紹介管理者、インセンティブ管理者、インセンティブ ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="48a8e-116">Non-Azure-Active-Directory roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="48a8e-117">パートナー センターで商取引を管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="48a8e-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="48a8e-118">**Role**</span><span class="sxs-lookup"><span data-stu-id="48a8e-118">**Role**</span></span>|<span data-ttu-id="48a8e-119">**できること**</span><span class="sxs-lookup"><span data-stu-id="48a8e-119">**What they can do**</span></span>|<span data-ttu-id="48a8e-120">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="48a8e-120">**Learn more**</span></span>|
|----------------------------------|---|:---------------------------------|
|<span data-ttu-id="48a8e-121">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="48a8e-121">Global admin</span></span>|<span data-ttu-id="48a8e-122">\*    すべての特権を備えたすべての Microsoft アカウントまたはサービスへのアクセスが可能</span><span class="sxs-lookup"><span data-stu-id="48a8e-122">\*    Can access all Microsoft account/services with full privileges</span></span>|[<span data-ttu-id="48a8e-123">パートナー センター アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-123">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
|      |<span data-ttu-id="48a8e-124">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="48a8e-124">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="48a8e-125">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-125">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="48a8e-126">\*    契約、価格表、オファーの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-126">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="48a8e-127">\*    パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-127">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="48a8e-128">課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-128">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="48a8e-129">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="48a8e-129">User management admin</span></span>   | <span data-ttu-id="48a8e-130">\*    ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-130">\*    View, create, and manage users</span></span>|[<span data-ttu-id="48a8e-131">パートナー センターで Microsoft Partner Network メンバーシップの特典とプランを管理する</span><span class="sxs-lookup"><span data-stu-id="48a8e-131">Manage your Microsoft Partner Network membership benefits and offers in Partner Center</span></span>](manage-your-partner-network-benefits.md)
||<span data-ttu-id="48a8e-132">\*    すべてのパートナー プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-132">\*    View all partner profiles</span></span>
||<span data-ttu-id="48a8e-133">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="48a8e-133">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="48a8e-134">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-134">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="48a8e-135">課金管理者</span><span class="sxs-lookup"><span data-stu-id="48a8e-135">Billing admin</span></span> | <span data-ttu-id="48a8e-136">- 課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-136">- View, create, and manage billing, invoices, and recon files</span></span>|[<span data-ttu-id="48a8e-137">請求書の記載事項</span><span class="sxs-lookup"><span data-stu-id="48a8e-137">Read your bill</span></span>](billing.md)
||<span data-ttu-id="48a8e-138">\*    価格の表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-138">\*    View pricing</span></span>
||<span data-ttu-id="48a8e-139">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="48a8e-139">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="48a8e-140">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-140">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="48a8e-141">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="48a8e-141">Default user</span></span>|  <span data-ttu-id="48a8e-142">マイ プロフィールの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-142">View My profile</span></span>   |[<span data-ttu-id="48a8e-143">パスワードをリセットする</span><span class="sxs-lookup"><span data-stu-id="48a8e-143">Reset your password</span></span>](reset-my-pasword.md)
|<span data-ttu-id="48a8e-144">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="48a8e-144">Admin agent</span></span> | <span data-ttu-id="48a8e-145">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-145">\*    Customer management</span></span>|[<span data-ttu-id="48a8e-146">お客様とつながる</span><span class="sxs-lookup"><span data-stu-id="48a8e-146">Connect with your customers</span></span>](connect-with-your-customers.md)
||<span data-ttu-id="48a8e-147">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="48a8e-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="48a8e-148">\*    プロファイルの作成とデバイスへの適用</span><span class="sxs-lookup"><span data-stu-id="48a8e-148">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="48a8e-149">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-149">\*    Subscription management</span></span>
||<span data-ttu-id="48a8e-150">\*    顧客のためのサービスの正常性とサービス要求</span><span class="sxs-lookup"><span data-stu-id="48a8e-150">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="48a8e-151">\*    代理管理者特権の要求</span><span class="sxs-lookup"><span data-stu-id="48a8e-151">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="48a8e-152">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="48a8e-153">\*    請求</span><span class="sxs-lookup"><span data-stu-id="48a8e-153">\*    Billing</span></span>
||<span data-ttu-id="48a8e-154">\*    顧客の代理としての管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-154">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="48a8e-155">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="48a8e-155">\*    Register a value added reseller</span></span>
||<span data-ttu-id="48a8e-156">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="48a8e-156">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="48a8e-157">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-157">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="48a8e-158">販売代理店</span><span class="sxs-lookup"><span data-stu-id="48a8e-158">Sales agent</span></span> | <span data-ttu-id="48a8e-159">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-159">\*    Customer management</span></span>|[<span data-ttu-id="48a8e-160">顧客に課金サポートを提供し、請求に関する質問に答える</span><span class="sxs-lookup"><span data-stu-id="48a8e-160">Provide billing support for your customers and help answer their billing questions</span></span>](provide-billing-support.md)
||<span data-ttu-id="48a8e-161">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="48a8e-161">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="48a8e-162">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-162">\*    Subscription management</span></span>
||<span data-ttu-id="48a8e-163">\*    サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-163">\*    View support tickets</span></span>
||<span data-ttu-id="48a8e-164">\*    顧客との再販業者関係の要求</span><span class="sxs-lookup"><span data-stu-id="48a8e-164">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="48a8e-165">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-165">\*    View pricing and offers</span></span>
||<span data-ttu-id="48a8e-166">\*    潜在顧客の管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-166">\*    Manage customer leads</span></span>
||<span data-ttu-id="48a8e-167">\*    顧客契約の表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-167">\*    View the customer agreement</span></span>
||<span data-ttu-id="48a8e-168">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="48a8e-168">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="48a8e-169">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="48a8e-169">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="48a8e-170">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-170">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="48a8e-171">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="48a8e-171">Helpdesk agent</span></span>| <span data-ttu-id="48a8e-172">\*    顧客の検索と表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-172">\*    Search for and view a customer</span></span>|[<span data-ttu-id="48a8e-173">Microsoft への問題のエスカレーション、および Microsoft へのエスカレーションに適した問題の見極め方</span><span class="sxs-lookup"><span data-stu-id="48a8e-173">Escalate problems to Microsoft and learn which issues are more-suited to Microsoft escalation</span></span>](escalate-problems-to-microsoft.md)
||<span data-ttu-id="48a8e-174">\*    顧客の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="48a8e-174">\*    Edit customer details</span></span>
||<span data-ttu-id="48a8e-175">\*    請求またはサブスクリプション管理に関する顧客の問題の解決サポート</span><span class="sxs-lookup"><span data-stu-id="48a8e-175">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="48a8e-176">\*    顧客の代理としてのサポート要求</span><span class="sxs-lookup"><span data-stu-id="48a8e-176">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="48a8e-177">\*    顧客の代理としてのサブスクリプションと請求に関する問題の管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-177">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="48a8e-178">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="48a8e-178">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="48a8e-179">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-179">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a><span data-ttu-id="48a8e-180">コントロール パネル ベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="48a8e-180">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="48a8e-181">(CSP ロールと非 Azure AD ロール)</span><span class="sxs-lookup"><span data-stu-id="48a8e-181">(CSP role and non-Azure AD role)</span></span>

<span data-ttu-id="48a8e-182">CPV は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムとパートナー センター API を統合するために使用するアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="48a8e-182">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="48a8e-183">**Role**</span><span class="sxs-lookup"><span data-stu-id="48a8e-183">**Role**</span></span>   |<span data-ttu-id="48a8e-184">**できること**</span><span class="sxs-lookup"><span data-stu-id="48a8e-184">**What you can do**</span></span>|<span data-ttu-id="48a8e-185">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="48a8e-185">**Learn more**</span></span>|
|------------------------------|:----------------------------|----|
|<span data-ttu-id="48a8e-186">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="48a8e-186">Global admin</span></span>| <span data-ttu-id="48a8e-187">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-187">View and manage your CPV profile</span></span>|[<span data-ttu-id="48a8e-188">CSP パートナー システムとパートナー センター API との統合を支援するためにコントロール パネル ベンダーとして登録する</span><span class="sxs-lookup"><span data-stu-id="48a8e-188">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>](enroll-as-cpv.md)
||<span data-ttu-id="48a8e-189">CPV 機能にアクセスする必要があるユーザーの表示と管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-189">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a><span data-ttu-id="48a8e-190">ゲスト ユーザー (Azure Active Directory テナントに追加する必要あり)</span><span class="sxs-lookup"><span data-stu-id="48a8e-190">Guest user (must be added to the Azure Active Directory tenant)</span></span>

|<span data-ttu-id="48a8e-191">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="48a8e-191">**Guest user**</span></span>   | <span data-ttu-id="48a8e-192">**ロール**</span><span class="sxs-lookup"><span data-stu-id="48a8e-192">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="48a8e-193">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="48a8e-193">MPN partner admin</span></span>|
||<span data-ttu-id="48a8e-194">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="48a8e-194">Business profile admin</span></span>|
||<span data-ttu-id="48a8e-195">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="48a8e-195">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company"></a><span data-ttu-id="48a8e-196">MPN メンバーシップと貴社の管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-196">Manage MPN membership and your company</span></span> 

<span data-ttu-id="48a8e-197">次のロールは Azure Active Directory ロールではありません。</span><span class="sxs-lookup"><span data-stu-id="48a8e-197">These roles are not Azure Active Directory roles.</span></span> <span data-ttu-id="48a8e-198">これらのロールでは、テナントではなく会社のビジネスを管理します。</span><span class="sxs-lookup"><span data-stu-id="48a8e-198">These roles manage the company business rather than the tenant.</span></span>

|<span data-ttu-id="48a8e-199">**Role**</span><span class="sxs-lookup"><span data-stu-id="48a8e-199">**Role**</span></span> | <span data-ttu-id="48a8e-200">**できること**</span><span class="sxs-lookup"><span data-stu-id="48a8e-200">**What you can do**</span></span>|<span data-ttu-id="48a8e-201">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="48a8e-201">**Learn more**</span></span>|
|----------------------------|:----------------------------|-----|
|<span data-ttu-id="48a8e-202">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="48a8e-202">MPN partner admin</span></span>|<span data-ttu-id="48a8e-203">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-203">\*    View, create, and manage partner service requests</span></span>|[<span data-ttu-id="48a8e-204">Microsoft Action Pack サブスクリプションや Silver コンピテンシーと Gold コンピテンシーを購入または更新する</span><span class="sxs-lookup"><span data-stu-id="48a8e-204">Buy or renew a Microsoft Action Pack subscription or silver and gold competencies</span></span>](mpn-get-action-pack.md)
||<span data-ttu-id="48a8e-205">\*    法的プロファイル、企業プロファイル、ビジネス プロファイル、MPN プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-205">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="48a8e-206">\*    ユーザーの詳細およびスキル データの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-206">\*    View user details and their skills data</span></span>
||<span data-ttu-id="48a8e-207">\*    コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-207">\*    View competencies</span></span>
||<span data-ttu-id="48a8e-208">\*    特典の表示と管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-208">\*    View and manage benefits</span></span>
||<span data-ttu-id="48a8e-209">\*    MPN オファーの表示と購入</span><span class="sxs-lookup"><span data-stu-id="48a8e-209">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="48a8e-210">\*    MPN オファーの注文履歴と請求書の表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-210">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="48a8e-211">\*    パートナー貢献度インジケーター データの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-211">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="48a8e-212">\*    利用券検証ツールでの作業</span><span class="sxs-lookup"><span data-stu-id="48a8e-212">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="48a8e-213">\*    顧客データ分析の表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-213">\*    View customer data analytics</span></span>
||<span data-ttu-id="48a8e-214">\*    会社内の他のユーザー ロールを表示しますが、ロールを割り当てることはできません</span><span class="sxs-lookup"><span data-stu-id="48a8e-214">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="48a8e-215">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="48a8e-215">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="48a8e-216">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-216">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="48a8e-217">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="48a8e-217">Account admin</span></span>| <span data-ttu-id="48a8e-218">場所の追加</span><span class="sxs-lookup"><span data-stu-id="48a8e-218">Add locations</span></span>|[<span data-ttu-id="48a8e-219">場所の管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-219">Manage locations</span></span>](manage-locations.md)
|| <span data-ttu-id="48a8e-220">管理対象のアカウントに関連するプロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-220">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="48a8e-221">\*    テナント内のユーザーに対するロールの非 Azure-Active-Directory ロールへの割り当て</span><span class="sxs-lookup"><span data-stu-id="48a8e-221">\*    Assign roles for users in tenant to non-Azure-Active-Directory roles</span></span> 
||<span data-ttu-id="48a8e-222">\*    プログラムへの場所の登録</span><span class="sxs-lookup"><span data-stu-id="48a8e-222">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="48a8e-223">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="48a8e-223">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="48a8e-224">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-224">\*    View partner support tickets you create</span></span>

## <a name="manage-referrals"></a><span data-ttu-id="48a8e-225">紹介の管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-225">Manage referrals</span></span>

|<span data-ttu-id="48a8e-226">**Role**</span><span class="sxs-lookup"><span data-stu-id="48a8e-226">**Role**</span></span> | <span data-ttu-id="48a8e-227">**できること**</span><span class="sxs-lookup"><span data-stu-id="48a8e-227">**What you can do**</span></span>|<span data-ttu-id="48a8e-228">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="48a8e-228">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="48a8e-229">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="48a8e-229">Referrals admin</span></span>|<span data-ttu-id="48a8e-230">パートナー センターの [紹介] タブにあるすべてのものを作成および管理する</span><span class="sxs-lookup"><span data-stu-id="48a8e-230">Create and manage everything under Referrals tab in Partner Center</span></span>|[<span data-ttu-id="48a8e-231">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="48a8e-231">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="48a8e-232">すべての共同販売の機会と潜在顧客を表示および編集できます</span><span class="sxs-lookup"><span data-stu-id="48a8e-232">Can view and edit all the co-sell opportunities and leads</span></span>
||    <span data-ttu-id="48a8e-233">取引にチーム メンバーを割り当てることができます</span><span class="sxs-lookup"><span data-stu-id="48a8e-233">Can assign team members for a deal</span></span>
||    <span data-ttu-id="48a8e-234">ビジネス プロファイルを表示および編集できます</span><span class="sxs-lookup"><span data-stu-id="48a8e-234">Can view and edit business profiles</span></span>
||    <span data-ttu-id="48a8e-235">成立し、取引登録の対象としてマークされている営業案件の表示と登録を行うことができます</span><span class="sxs-lookup"><span data-stu-id="48a8e-235">Can view and register deals for opportunities that are marked as won and eligible for deal registration</span></span>
||    <span data-ttu-id="48a8e-236">サポート チケットを作成および表示できます</span><span class="sxs-lookup"><span data-stu-id="48a8e-236">Can create and view support tickets</span></span>
|<span data-ttu-id="48a8e-237">紹介ユーザー</span><span class="sxs-lookup"><span data-stu-id="48a8e-237">Referrals user</span></span>|<span data-ttu-id="48a8e-238">チームの一員である場合にのみ共同販売の機会を作成および管理する</span><span class="sxs-lookup"><span data-stu-id="48a8e-238">Create and manage co-sell opportunities only if they are a part of the team</span></span> |[<span data-ttu-id="48a8e-239">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="48a8e-239">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="48a8e-240">ロールが割り当てられている場所の共同販売機会を作成できます。</span><span class="sxs-lookup"><span data-stu-id="48a8e-240">Can create co-sell opportunities for the locations where they are assigned the role.</span></span>
||    <span data-ttu-id="48a8e-241">チーム メンバーである場合、成立し、取引登録の対象としてマークされている営業案件の表示と登録を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="48a8e-241">Can view and register deals for opportunities that are marked as won and eligible for deal registration if they are team member.</span></span>
||    <span data-ttu-id="48a8e-242">サポート チケットを作成および表示できます</span><span class="sxs-lookup"><span data-stu-id="48a8e-242">Can create and view support tickets</span></span>
|<span data-ttu-id="48a8e-243">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="48a8e-243">Business profile admin</span></span>|<span data-ttu-id="48a8e-244">ビジネス プロファイルを作成および管理します</span><span class="sxs-lookup"><span data-stu-id="48a8e-244">Create and manage business profiles</span></span> | [<span data-ttu-id="48a8e-245">ビジネス プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-245">Manage business profiles</span></span>](create-a-marketing-profile.md)
||    <span data-ttu-id="48a8e-246">サポート チケットを作成および表示できます</span><span class="sxs-lookup"><span data-stu-id="48a8e-246">Can create and view support tickets</span></span>

<span data-ttu-id="48a8e-247">新しい参照ユーザー ロールと共に、取引の場所のスコープも導入されます。</span><span class="sxs-lookup"><span data-stu-id="48a8e-247">Along with the new referrals user role, we are also introducing the location scope for deals.</span></span> <span data-ttu-id="48a8e-248">下の表では、場所に基づく取引アクセスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="48a8e-248">The table below explains the deals-access based on the location.</span></span>

|<span data-ttu-id="48a8e-249">**スコープ**</span><span class="sxs-lookup"><span data-stu-id="48a8e-249">**Scope**</span></span> | <span data-ttu-id="48a8e-250">**できること**</span><span class="sxs-lookup"><span data-stu-id="48a8e-250">**What you can do**</span></span> |
|------------------------------|:-------------------------|
|<span data-ttu-id="48a8e-251">会社全体</span><span class="sxs-lookup"><span data-stu-id="48a8e-251">Entire company</span></span> | <span data-ttu-id="48a8e-252">管理者とユーザーの両方が、会社内の任意の場所に対する取引を作成するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="48a8e-252">Both admins and users have access to create deals for any location in their company</span></span>|
|| <span data-ttu-id="48a8e-253">紹介管理者は、すべての取引を表示および編集するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="48a8e-253">Referral admin has access to view and edit all the deals</span></span> |
|| <span data-ttu-id="48a8e-254">紹介ユーザーは、チームの一員である場合にのみ、すべての取引を表示および編集するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="48a8e-254">Referral users have access to view and edit all the deals only if they are a part of the team</span></span> |
|<span data-ttu-id="48a8e-255">1 つまたは複数の場所</span><span class="sxs-lookup"><span data-stu-id="48a8e-255">One or more locations</span></span> | <span data-ttu-id="48a8e-256">管理者とユーザーの両方が、会社内の割り当てられた場所の取引を作成するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="48a8e-256">Both admins and users have access to create deals for the assigned location in their company</span></span>|
|| <span data-ttu-id="48a8e-257">紹介管理者は、割り当てられた場所に属するすべての取引を表示および編集するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="48a8e-257">Referral admin has access to view and edit all the deals belonging to the assigned locations</span></span>|
|| <span data-ttu-id="48a8e-258">紹介ユーザーは、チームに属している場合、割り当てられた場所に属するすべての取引を表示および編集するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="48a8e-258">Referral users have access to view and edit all the deals belonging to the assigned locations if they are part of the team</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="48a8e-259">インセンティブの管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-259">Manage incentives</span></span>

|<span data-ttu-id="48a8e-260">**Role**</span><span class="sxs-lookup"><span data-stu-id="48a8e-260">**Role**</span></span> | <span data-ttu-id="48a8e-261">**できること**</span><span class="sxs-lookup"><span data-stu-id="48a8e-261">**What you can do**</span></span>|<span data-ttu-id="48a8e-262">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="48a8e-262">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="48a8e-263">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="48a8e-263">Incentives admin</span></span>|<span data-ttu-id="48a8e-264">\*    インセンティブの開始と管理</span><span class="sxs-lookup"><span data-stu-id="48a8e-264">\*    Initiates and manages incentives</span></span> |[<span data-ttu-id="48a8e-265">これらのリソースを使用してインセンティブを使い始める</span><span class="sxs-lookup"><span data-stu-id="48a8e-265">Use these resources to help you get started with incentives</span></span>](incentives-get-started-intro.md)
||<span data-ttu-id="48a8e-266">\*    インセンティブ プログラムのすべての側面の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="48a8e-266">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="48a8e-267">\*    銀行および税の詳細情報の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="48a8e-267">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="48a8e-268">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-268">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="48a8e-269">\*    サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="48a8e-269">\*    Access support</span></span>
||<span data-ttu-id="48a8e-270">\*    インセンティブ支払いについての議論</span><span class="sxs-lookup"><span data-stu-id="48a8e-270">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="48a8e-271">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="48a8e-271">Incentives user</span></span>|<span data-ttu-id="48a8e-272">\*    インセンティブ プログラムを表示可能</span><span class="sxs-lookup"><span data-stu-id="48a8e-272">\*    Can view incentives programs</span></span>
||<span data-ttu-id="48a8e-273">\*    インセンティブの申請の表示と開始が可能</span><span class="sxs-lookup"><span data-stu-id="48a8e-273">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="48a8e-274">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-274">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="48a8e-275">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="48a8e-275">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="48a8e-276">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-276">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="48a8e-277">パートナー センター インサイト データの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-277">View Partner Center Insights data</span></span>

|<span data-ttu-id="48a8e-278">**Role**</span><span class="sxs-lookup"><span data-stu-id="48a8e-278">**Role**</span></span> | <span data-ttu-id="48a8e-279">**できること**</span><span class="sxs-lookup"><span data-stu-id="48a8e-279">**What you can do**</span></span>|<span data-ttu-id="48a8e-280">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="48a8e-280">**Learn more**</span></span>|
|------------------------------|:-------------------------|---|
|<span data-ttu-id="48a8e-281">エグゼクティブ レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="48a8e-281">Executive report viewer</span></span>|<span data-ttu-id="48a8e-282">すべてのレポート データセットへのアクセス、パートナー サポート チケットの作成、作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-282">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|[<span data-ttu-id="48a8e-283">パートナー センターの分析情報で利用できる概要ダッシュボード レポート</span><span class="sxs-lookup"><span data-stu-id="48a8e-283">Overview dashboard reports available in Partner Center Insights</span></span>](pci-overview-report.md)
|<span data-ttu-id="48a8e-284">レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="48a8e-284">Report viewer</span></span>|<span data-ttu-id="48a8e-285">収益や顧客と従業員の個人データを除くデータ レポートへのアクセス、パートナー サポート チケットの作成、作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="48a8e-285">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|

## <a name="next-steps"></a><span data-ttu-id="48a8e-286">次のステップ</span><span class="sxs-lookup"><span data-stu-id="48a8e-286">Next steps</span></span>

- [<span data-ttu-id="48a8e-287">ユーザー アカウントの作成およびロールとアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="48a8e-287">Create user accounts and assign roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)
- [<span data-ttu-id="48a8e-288">新しいパートナー センター プログラムに登録する際のアカウント情報の確認</span><span class="sxs-lookup"><span data-stu-id="48a8e-288">Verify your account information when you enroll in a new Partner Center program</span></span>](verification-responses.md)
