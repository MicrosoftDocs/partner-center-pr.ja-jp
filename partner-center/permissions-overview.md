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
ms.openlocfilehash: b1ac34bbb92d600805465ca5f6d1b28af54cd5e1
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855133"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="5990f-103">パートナー センターで作業する必要がある会社のユーザーにユーザーのロールとアクセス許可を割り当てる</span><span class="sxs-lookup"><span data-stu-id="5990f-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="5990f-104">**対象のロール**: グローバル管理者 | ユーザー管理の管理者 | MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="5990f-104">**Appropriate roles**: Global admin | User management admin | MPN partner admin</span></span>

<span data-ttu-id="5990f-105">貴社の正式名称や法的住所、サポートの詳細、税金の除外の申告、銀行情報、主要な連絡先など、パートナー プロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="5990f-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="5990f-106">次のステップ:ユーザーにパスワードとロールを設定させて、ユーザーがパートナー センターでの作業を開始できるようにします。</span><span class="sxs-lookup"><span data-stu-id="5990f-106">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="5990f-107">パートナー センターで作業できるように従業員を設定する</span><span class="sxs-lookup"><span data-stu-id="5990f-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="5990f-108">ユーザーに付与するロールとアクセス許可によって、パートナー センターでのユーザーのアクセスの種類が決まります。</span><span class="sxs-lookup"><span data-stu-id="5990f-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="5990f-109">ロールは、貴社のビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="5990f-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="5990f-110">たとえば、貴社のビジネスがクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、グローバル管理者などの標準の Azure Active Directory テナント管理ロールだけでなく、CSP プログラムに固有のロールも必要です。</span><span class="sxs-lookup"><span data-stu-id="5990f-110">For example, if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure Active Directory tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="5990f-111">各プログラムには、それに固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="5990f-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="5990f-112">Azure Active Directory テナント ロールには、グローバル管理者、ユーザー管理者、CSP のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5990f-112">Azure Active Directory tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="5990f-113">Azure Active Directory 以外のロールはテナントを管理しないロールであり、MPN 管理者、ビジネス プロファイル管理者、紹介管理者、インセンティブ管理者、インセンティブ ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5990f-113">Non-Azure-Active-Directory roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="5990f-114">パートナー センターで商取引を管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="5990f-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="5990f-115">**Role**</span><span class="sxs-lookup"><span data-stu-id="5990f-115">**Role**</span></span>|<span data-ttu-id="5990f-116">**できること**</span><span class="sxs-lookup"><span data-stu-id="5990f-116">**What they can do**</span></span>|<span data-ttu-id="5990f-117">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="5990f-117">**Learn more**</span></span>|
|----------------------------------|---|:---------------------------------|
|<span data-ttu-id="5990f-118">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="5990f-118">Global admin</span></span>|<span data-ttu-id="5990f-119">\*    すべての特権を備えたすべての Microsoft アカウントまたはサービスへのアクセスが可能</span><span class="sxs-lookup"><span data-stu-id="5990f-119">\*    Can access all Microsoft account/services with full privileges</span></span>|[<span data-ttu-id="5990f-120">パートナー センター アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="5990f-120">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
|      |<span data-ttu-id="5990f-121">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="5990f-121">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="5990f-122">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-122">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="5990f-123">\*    契約、価格表、オファーの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="5990f-124">\*    パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="5990f-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="5990f-125">課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="5990f-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="5990f-126">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="5990f-126">User management admin</span></span>   | <span data-ttu-id="5990f-127">\*    ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="5990f-127">\*    View, create, and manage users</span></span>|[<span data-ttu-id="5990f-128">パートナー センターで Microsoft Partner Network メンバーシップの特典とプランを管理する</span><span class="sxs-lookup"><span data-stu-id="5990f-128">Manage your Microsoft Partner Network membership benefits and offers in Partner Center</span></span>](manage-your-partner-network-benefits.md)
||<span data-ttu-id="5990f-129">\*    すべてのパートナー プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="5990f-130">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="5990f-130">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="5990f-131">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-131">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="5990f-132">課金管理者</span><span class="sxs-lookup"><span data-stu-id="5990f-132">Billing admin</span></span> | <span data-ttu-id="5990f-133">- 課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="5990f-133">- View, create, and manage billing, invoices, and recon files</span></span>|[<span data-ttu-id="5990f-134">請求書の記載事項</span><span class="sxs-lookup"><span data-stu-id="5990f-134">Read your bill</span></span>](billing.md)
||<span data-ttu-id="5990f-135">\*    価格の表示</span><span class="sxs-lookup"><span data-stu-id="5990f-135">\*    View pricing</span></span>
||<span data-ttu-id="5990f-136">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="5990f-136">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="5990f-137">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-137">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="5990f-138">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="5990f-138">Default user</span></span>|  <span data-ttu-id="5990f-139">マイ プロフィールの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-139">View My profile</span></span>   |[<span data-ttu-id="5990f-140">パスワードをリセットする</span><span class="sxs-lookup"><span data-stu-id="5990f-140">Reset your password</span></span>](reset-my-pasword.md)
|<span data-ttu-id="5990f-141">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="5990f-141">Admin agent</span></span> | <span data-ttu-id="5990f-142">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="5990f-142">\*    Customer management</span></span>|[<span data-ttu-id="5990f-143">お客様とつながる</span><span class="sxs-lookup"><span data-stu-id="5990f-143">Connect with your customers</span></span>](connect-with-your-customers.md)
||<span data-ttu-id="5990f-144">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="5990f-144">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="5990f-145">\*    プロファイルの作成とデバイスへの適用</span><span class="sxs-lookup"><span data-stu-id="5990f-145">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="5990f-146">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="5990f-146">\*    Subscription management</span></span>
||<span data-ttu-id="5990f-147">\*    顧客のためのサービスの正常性とサービス要求</span><span class="sxs-lookup"><span data-stu-id="5990f-147">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="5990f-148">\*    代理管理者特権の要求</span><span class="sxs-lookup"><span data-stu-id="5990f-148">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="5990f-149">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-149">\*    View pricing and offers</span></span>
||<span data-ttu-id="5990f-150">\*    請求</span><span class="sxs-lookup"><span data-stu-id="5990f-150">\*    Billing</span></span>
||<span data-ttu-id="5990f-151">\*    顧客の代理としての管理</span><span class="sxs-lookup"><span data-stu-id="5990f-151">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="5990f-152">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="5990f-152">\*    Register a value added reseller</span></span>
||<span data-ttu-id="5990f-153">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="5990f-153">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="5990f-154">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-154">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="5990f-155">販売代理店</span><span class="sxs-lookup"><span data-stu-id="5990f-155">Sales agent</span></span> | <span data-ttu-id="5990f-156">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="5990f-156">\*    Customer management</span></span>|[<span data-ttu-id="5990f-157">顧客に課金サポートを提供し、請求に関する質問に答える</span><span class="sxs-lookup"><span data-stu-id="5990f-157">Provide billing support for your customers and help answer their billing questions</span></span>](provide-billing-support.md)
||<span data-ttu-id="5990f-158">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="5990f-158">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="5990f-159">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="5990f-159">\*    Subscription management</span></span>
||<span data-ttu-id="5990f-160">\*    サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-160">\*    View support tickets</span></span>
||<span data-ttu-id="5990f-161">\*    顧客との再販業者関係の要求</span><span class="sxs-lookup"><span data-stu-id="5990f-161">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="5990f-162">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-162">\*    View pricing and offers</span></span>
||<span data-ttu-id="5990f-163">\*    潜在顧客の管理</span><span class="sxs-lookup"><span data-stu-id="5990f-163">\*    Manage customer leads</span></span>
||<span data-ttu-id="5990f-164">\*    顧客契約の表示</span><span class="sxs-lookup"><span data-stu-id="5990f-164">\*    View the customer agreement</span></span>
||<span data-ttu-id="5990f-165">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="5990f-165">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="5990f-166">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="5990f-166">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="5990f-167">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-167">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="5990f-168">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="5990f-168">Helpdesk agent</span></span>| <span data-ttu-id="5990f-169">\*    顧客の検索と表示</span><span class="sxs-lookup"><span data-stu-id="5990f-169">\*    Search for and view a customer</span></span>|[<span data-ttu-id="5990f-170">Microsoft への問題のエスカレーション、および Microsoft へのエスカレーションに適した問題の見極め方</span><span class="sxs-lookup"><span data-stu-id="5990f-170">Escalate problems to Microsoft and learn which issues are more-suited to Microsoft escalation</span></span>](escalate-problems-to-microsoft.md)
||<span data-ttu-id="5990f-171">\*    顧客の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="5990f-171">\*    Edit customer details</span></span>
||<span data-ttu-id="5990f-172">\*    請求またはサブスクリプション管理に関する顧客の問題の解決サポート</span><span class="sxs-lookup"><span data-stu-id="5990f-172">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="5990f-173">\*    顧客の代理としてのサポート要求</span><span class="sxs-lookup"><span data-stu-id="5990f-173">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="5990f-174">\*    顧客の代理としてのサブスクリプションと請求に関する問題の管理</span><span class="sxs-lookup"><span data-stu-id="5990f-174">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="5990f-175">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="5990f-175">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="5990f-176">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-176">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a><span data-ttu-id="5990f-177">コントロール パネル ベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="5990f-177">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="5990f-178">(CSP ロールと非 Azure AD ロール)</span><span class="sxs-lookup"><span data-stu-id="5990f-178">(CSP role and non-Azure AD role)</span></span>

<span data-ttu-id="5990f-179">CPV は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムとパートナー センター API を統合するために使用するアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="5990f-179">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="5990f-180">**Role**</span><span class="sxs-lookup"><span data-stu-id="5990f-180">**Role**</span></span>   |<span data-ttu-id="5990f-181">**できること**</span><span class="sxs-lookup"><span data-stu-id="5990f-181">**What you can do**</span></span>|<span data-ttu-id="5990f-182">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="5990f-182">**Learn more**</span></span>|
|------------------------------|:----------------------------|----|
|<span data-ttu-id="5990f-183">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="5990f-183">Global admin</span></span>| <span data-ttu-id="5990f-184">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="5990f-184">View and manage your CPV profile</span></span>|[<span data-ttu-id="5990f-185">CSP パートナー システムとパートナー センター API との統合を支援するためにコントロール パネル ベンダーとして登録する</span><span class="sxs-lookup"><span data-stu-id="5990f-185">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>](enroll-as-cpv.md)
||<span data-ttu-id="5990f-186">CPV 機能にアクセスする必要があるユーザーの表示と管理</span><span class="sxs-lookup"><span data-stu-id="5990f-186">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a><span data-ttu-id="5990f-187">ゲスト ユーザー (Azure Active Directory テナントに追加する必要あり)</span><span class="sxs-lookup"><span data-stu-id="5990f-187">Guest user (must be added to the Azure Active Directory tenant)</span></span>

|<span data-ttu-id="5990f-188">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="5990f-188">**Guest user**</span></span>   | <span data-ttu-id="5990f-189">**ロール**</span><span class="sxs-lookup"><span data-stu-id="5990f-189">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="5990f-190">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="5990f-190">MPN partner admin</span></span>|
||<span data-ttu-id="5990f-191">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="5990f-191">Business profile admin</span></span>|
||<span data-ttu-id="5990f-192">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="5990f-192">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company"></a><span data-ttu-id="5990f-193">MPN メンバーシップと貴社の管理</span><span class="sxs-lookup"><span data-stu-id="5990f-193">Manage MPN membership and your company</span></span> 

<span data-ttu-id="5990f-194">次のロールは Azure Active Directory ロールではありません。</span><span class="sxs-lookup"><span data-stu-id="5990f-194">These roles are not Azure Active Directory roles.</span></span> <span data-ttu-id="5990f-195">これらのロールでは、テナントではなく会社のビジネスを管理します。</span><span class="sxs-lookup"><span data-stu-id="5990f-195">These roles manage the company business rather than the tenant.</span></span>

|<span data-ttu-id="5990f-196">**Role**</span><span class="sxs-lookup"><span data-stu-id="5990f-196">**Role**</span></span> | <span data-ttu-id="5990f-197">**できること**</span><span class="sxs-lookup"><span data-stu-id="5990f-197">**What you can do**</span></span>|<span data-ttu-id="5990f-198">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="5990f-198">**Learn more**</span></span>|
|----------------------------|:----------------------------|-----|
|<span data-ttu-id="5990f-199">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="5990f-199">MPN partner admin</span></span>|<span data-ttu-id="5990f-200">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="5990f-200">\*    View, create, and manage partner service requests</span></span>|[<span data-ttu-id="5990f-201">Microsoft Action Pack サブスクリプションや Silver コンピテンシーと Gold コンピテンシーを購入または更新する</span><span class="sxs-lookup"><span data-stu-id="5990f-201">Buy or renew a Microsoft Action Pack subscription or silver and gold competencies</span></span>](mpn-get-action-pack.md)
||<span data-ttu-id="5990f-202">\*    法的プロファイル、企業プロファイル、ビジネス プロファイル、MPN プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-202">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="5990f-203">\*    ユーザーの詳細およびスキル データの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-203">\*    View user details and their skills data</span></span>
||<span data-ttu-id="5990f-204">\*    コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-204">\*    View competencies</span></span>
||<span data-ttu-id="5990f-205">\*    特典の表示と管理</span><span class="sxs-lookup"><span data-stu-id="5990f-205">\*    View and manage benefits</span></span>
||<span data-ttu-id="5990f-206">\*    MPN オファーの表示と購入</span><span class="sxs-lookup"><span data-stu-id="5990f-206">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="5990f-207">\*    MPN オファーの注文履歴と請求書の表示</span><span class="sxs-lookup"><span data-stu-id="5990f-207">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="5990f-208">\*    パートナー貢献度インジケーター データの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-208">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="5990f-209">\*    利用券検証ツールでの作業</span><span class="sxs-lookup"><span data-stu-id="5990f-209">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="5990f-210">\*    顧客データ分析の表示</span><span class="sxs-lookup"><span data-stu-id="5990f-210">\*    View customer data analytics</span></span>
||<span data-ttu-id="5990f-211">\*    会社内の他のユーザー ロールを表示しますが、ロールを割り当てることはできません</span><span class="sxs-lookup"><span data-stu-id="5990f-211">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="5990f-212">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="5990f-212">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="5990f-213">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-213">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="5990f-214">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="5990f-214">Account admin</span></span>| <span data-ttu-id="5990f-215">場所の追加</span><span class="sxs-lookup"><span data-stu-id="5990f-215">Add locations</span></span>|[<span data-ttu-id="5990f-216">場所の管理</span><span class="sxs-lookup"><span data-stu-id="5990f-216">Manage locations</span></span>](manage-locations.md)
|| <span data-ttu-id="5990f-217">管理対象のアカウントに関連するプロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="5990f-217">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="5990f-218">\*    テナント内のユーザーに対するロールの非 Azure-Active-Directory ロールへの割り当て</span><span class="sxs-lookup"><span data-stu-id="5990f-218">\*    Assign roles for users in tenant to non-Azure-Active-Directory roles</span></span> 
||<span data-ttu-id="5990f-219">\*    プログラムへの場所の登録</span><span class="sxs-lookup"><span data-stu-id="5990f-219">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="5990f-220">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="5990f-220">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="5990f-221">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-221">\*    View partner support tickets you create</span></span>

## <a name="manage-referrals"></a><span data-ttu-id="5990f-222">紹介の管理</span><span class="sxs-lookup"><span data-stu-id="5990f-222">Manage referrals</span></span>

|<span data-ttu-id="5990f-223">**Role**</span><span class="sxs-lookup"><span data-stu-id="5990f-223">**Role**</span></span> | <span data-ttu-id="5990f-224">**できること**</span><span class="sxs-lookup"><span data-stu-id="5990f-224">**What you can do**</span></span>|<span data-ttu-id="5990f-225">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="5990f-225">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="5990f-226">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="5990f-226">Referrals admin</span></span>|<span data-ttu-id="5990f-227">パートナー センターの [紹介] タブにあるすべてのものを作成および管理する</span><span class="sxs-lookup"><span data-stu-id="5990f-227">Create and manage everything under Referrals tab in Partner Center</span></span>|[<span data-ttu-id="5990f-228">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="5990f-228">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="5990f-229">すべての共同販売の機会と潜在顧客を表示および編集できます</span><span class="sxs-lookup"><span data-stu-id="5990f-229">Can view and edit all the co-sell opportunities and leads</span></span>
||    <span data-ttu-id="5990f-230">取引にチーム メンバーを割り当てることができます</span><span class="sxs-lookup"><span data-stu-id="5990f-230">Can assign team members for a deal</span></span>
||    <span data-ttu-id="5990f-231">ビジネス プロファイルを表示および編集できます</span><span class="sxs-lookup"><span data-stu-id="5990f-231">Can view and edit business profiles</span></span>
||    <span data-ttu-id="5990f-232">成立し、取引登録の対象としてマークされている営業案件の表示と登録を行うことができます</span><span class="sxs-lookup"><span data-stu-id="5990f-232">Can view and register deals for opportunities that are marked as won and eligible for deal registration</span></span>
||    <span data-ttu-id="5990f-233">サポート チケットを作成および表示できます</span><span class="sxs-lookup"><span data-stu-id="5990f-233">Can create and view support tickets</span></span>
|<span data-ttu-id="5990f-234">紹介ユーザー</span><span class="sxs-lookup"><span data-stu-id="5990f-234">Referrals user</span></span>|<span data-ttu-id="5990f-235">チームの一員である場合にのみ共同販売の機会を作成および管理する</span><span class="sxs-lookup"><span data-stu-id="5990f-235">Create and manage co-sell opportunities only if they are a part of the team</span></span> |[<span data-ttu-id="5990f-236">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="5990f-236">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="5990f-237">ロールが割り当てられている場所の共同販売機会を作成できます。</span><span class="sxs-lookup"><span data-stu-id="5990f-237">Can create co-sell opportunities for the locations where they are assigned the role.</span></span>
||    <span data-ttu-id="5990f-238">チーム メンバーである場合、成立し、取引登録の対象としてマークされている営業案件の表示と登録を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="5990f-238">Can view and register deals for opportunities that are marked as won and eligible for deal registration if they are team member.</span></span>
||    <span data-ttu-id="5990f-239">サポート チケットを作成および表示できます</span><span class="sxs-lookup"><span data-stu-id="5990f-239">Can create and view support tickets</span></span>
|<span data-ttu-id="5990f-240">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="5990f-240">Business profile admin</span></span>|<span data-ttu-id="5990f-241">ビジネス プロファイルを作成および管理します</span><span class="sxs-lookup"><span data-stu-id="5990f-241">Create and manage business profiles</span></span> | [<span data-ttu-id="5990f-242">ビジネス プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="5990f-242">Manage business profiles</span></span>](create-a-marketing-profile.md)
||    <span data-ttu-id="5990f-243">サポート チケットを作成および表示できます</span><span class="sxs-lookup"><span data-stu-id="5990f-243">Can create and view support tickets</span></span>

<span data-ttu-id="5990f-244">新しい参照ユーザー ロールと共に、取引の場所のスコープも導入されます。</span><span class="sxs-lookup"><span data-stu-id="5990f-244">Along with the new referrals user role, we are also introducing the location scope for deals.</span></span> <span data-ttu-id="5990f-245">下の表では、場所に基づく取引アクセスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="5990f-245">The table below explains the deals-access based on the location.</span></span>

|<span data-ttu-id="5990f-246">**スコープ**</span><span class="sxs-lookup"><span data-stu-id="5990f-246">**Scope**</span></span> | <span data-ttu-id="5990f-247">**できること**</span><span class="sxs-lookup"><span data-stu-id="5990f-247">**What you can do**</span></span> |
|------------------------------|:-------------------------|
|<span data-ttu-id="5990f-248">会社全体</span><span class="sxs-lookup"><span data-stu-id="5990f-248">Entire company</span></span> | <span data-ttu-id="5990f-249">管理者とユーザーの両方が、会社内の任意の場所に対する取引を作成するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="5990f-249">Both admins and users have access to create deals for any location in their company</span></span>|
|| <span data-ttu-id="5990f-250">紹介管理者は、すべての取引を表示および編集するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="5990f-250">Referral admin has access to view and edit all the deals</span></span> |
|| <span data-ttu-id="5990f-251">紹介ユーザーは、チームの一員である場合にのみ、すべての取引を表示および編集するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="5990f-251">Referral users have access to view and edit all the deals only if they are a part of the team</span></span> |
|<span data-ttu-id="5990f-252">1 つまたは複数の場所</span><span class="sxs-lookup"><span data-stu-id="5990f-252">One or more locations</span></span> | <span data-ttu-id="5990f-253">管理者とユーザーの両方が、会社内の割り当てられた場所の取引を作成するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="5990f-253">Both admins and users have access to create deals for the assigned location in their company</span></span>|
|| <span data-ttu-id="5990f-254">紹介管理者は、割り当てられた場所に属するすべての取引を表示および編集するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="5990f-254">Referral admin has access to view and edit all the deals belonging to the assigned locations</span></span>|
|| <span data-ttu-id="5990f-255">紹介ユーザーは、チームに属している場合、割り当てられた場所に属するすべての取引を表示および編集するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="5990f-255">Referral users have access to view and edit all the deals belonging to the assigned locations if they are part of the team</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="5990f-256">インセンティブの管理</span><span class="sxs-lookup"><span data-stu-id="5990f-256">Manage incentives</span></span>

|<span data-ttu-id="5990f-257">**Role**</span><span class="sxs-lookup"><span data-stu-id="5990f-257">**Role**</span></span> | <span data-ttu-id="5990f-258">**できること**</span><span class="sxs-lookup"><span data-stu-id="5990f-258">**What you can do**</span></span>|<span data-ttu-id="5990f-259">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="5990f-259">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="5990f-260">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="5990f-260">Incentives admin</span></span>|<span data-ttu-id="5990f-261">\*    インセンティブの開始と管理</span><span class="sxs-lookup"><span data-stu-id="5990f-261">\*    Initiates and manages incentives</span></span> |[<span data-ttu-id="5990f-262">これらのリソースを使用してインセンティブを使い始める</span><span class="sxs-lookup"><span data-stu-id="5990f-262">Use these resources to help you get started with incentives</span></span>](incentives-get-started-intro.md)
||<span data-ttu-id="5990f-263">\*    インセンティブ プログラムのすべての側面の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="5990f-263">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="5990f-264">\*    銀行および税の詳細情報の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="5990f-264">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="5990f-265">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="5990f-265">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="5990f-266">\*    サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="5990f-266">\*    Access support</span></span>
||<span data-ttu-id="5990f-267">\*    インセンティブ支払いについての議論</span><span class="sxs-lookup"><span data-stu-id="5990f-267">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="5990f-268">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="5990f-268">Incentives user</span></span>|<span data-ttu-id="5990f-269">\*    インセンティブ プログラムを表示可能</span><span class="sxs-lookup"><span data-stu-id="5990f-269">\*    Can view incentives programs</span></span>
||<span data-ttu-id="5990f-270">\*    インセンティブの申請の表示と開始が可能</span><span class="sxs-lookup"><span data-stu-id="5990f-270">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="5990f-271">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="5990f-271">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="5990f-272">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="5990f-272">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="5990f-273">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-273">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="5990f-274">パートナー センター インサイト データの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-274">View Partner Center Insights data</span></span>

|<span data-ttu-id="5990f-275">**Role**</span><span class="sxs-lookup"><span data-stu-id="5990f-275">**Role**</span></span> | <span data-ttu-id="5990f-276">**できること**</span><span class="sxs-lookup"><span data-stu-id="5990f-276">**What you can do**</span></span>|<span data-ttu-id="5990f-277">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="5990f-277">**Learn more**</span></span>|
|------------------------------|:-------------------------|---|
|<span data-ttu-id="5990f-278">エグゼクティブ レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="5990f-278">Executive report viewer</span></span>|<span data-ttu-id="5990f-279">すべてのレポート データセットへのアクセス、パートナー サポート チケットの作成、作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-279">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|[<span data-ttu-id="5990f-280">パートナー センターの分析情報で利用できる概要ダッシュボード レポート</span><span class="sxs-lookup"><span data-stu-id="5990f-280">Overview dashboard reports available in Partner Center Insights</span></span>](pci-overview-report.md)
|<span data-ttu-id="5990f-281">レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="5990f-281">Report viewer</span></span>|<span data-ttu-id="5990f-282">収益や顧客と従業員の個人データを除くデータ レポートへのアクセス、パートナー サポート チケットの作成、作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="5990f-282">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|

## <a name="next-steps"></a><span data-ttu-id="5990f-283">次のステップ</span><span class="sxs-lookup"><span data-stu-id="5990f-283">Next steps</span></span>

- [<span data-ttu-id="5990f-284">ユーザー アカウントの作成およびロールとアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="5990f-284">Create user accounts and assign roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)
- [<span data-ttu-id="5990f-285">新しいパートナー センター プログラムに登録する際のアカウント情報の確認</span><span class="sxs-lookup"><span data-stu-id="5990f-285">Verify your account information when you enroll in a new Partner Center program</span></span>](verification-responses.md)
