---
title: ユーザーにロールとアクセス許可を割り当てる
ms.topic: article
ms.date: 09/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 商取引、紹介、インセンティブ、または MPN メンバーシップをパートナー センターで管理する、会社のユーザーに最適なロールについて説明します。
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperfq1
ms.openlocfilehash: 32df86887ccbea5d18d1bd8c7c34add2b1ab60e4
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006809"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="aaf6d-103">パートナー センターで作業する必要がある会社のユーザーにユーザーのロールとアクセス許可を割り当てる</span><span class="sxs-lookup"><span data-stu-id="aaf6d-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="aaf6d-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="aaf6d-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-105">Global admin</span></span>
- <span data-ttu-id="aaf6d-106">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-106">User admin</span></span>
- <span data-ttu-id="aaf6d-107">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-107">MPN partner admin</span></span>

<span data-ttu-id="aaf6d-108">貴社の正式名称や法的住所、サポートの詳細、税金の除外の申告、銀行情報、主要な連絡先など、パートナー プロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="aaf6d-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="aaf6d-109">次のステップ:ユーザーにパスワードとロールを設定させて、ユーザーがパートナー センターでの作業を開始できるようにします。</span><span class="sxs-lookup"><span data-stu-id="aaf6d-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="aaf6d-110">パートナー センターで作業できるように従業員を設定する</span><span class="sxs-lookup"><span data-stu-id="aaf6d-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="aaf6d-111">ユーザーに付与するロールとアクセス許可によって、パートナー センターでのユーザーのアクセスの種類が決まります。</span><span class="sxs-lookup"><span data-stu-id="aaf6d-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="aaf6d-112">ロールは、貴社のビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="aaf6d-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="aaf6d-113">たとえば、貴社のビジネスがクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、グローバル管理者などの標準の Azure Active Directory テナント管理ロールだけでなく、CSP プログラムに固有のロールも必要です。</span><span class="sxs-lookup"><span data-stu-id="aaf6d-113">For example, if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure Active Directory tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="aaf6d-114">各プログラムには、それに固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="aaf6d-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="aaf6d-115">Azure Active Directory テナント ロールには、グローバル管理者、ユーザー管理者、CSP のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="aaf6d-115">Azure Active Directory tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="aaf6d-116">Azure Active Directory 以外のロールはテナントを管理しないロールであり、MPN 管理者、ビジネス プロファイル管理者、紹介管理者、インセンティブ管理者、インセンティブ ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="aaf6d-116">Non-Azure-Active-Directory roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="aaf6d-117">パートナー センターで商取引を管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="aaf6d-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="aaf6d-118">**Role**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-118">**Role**</span></span>|<span data-ttu-id="aaf6d-119">**できること**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-119">**What they can do**</span></span>|<span data-ttu-id="aaf6d-120">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-120">**Learn more**</span></span>|
|----------------------------------|---|:---------------------------------|
|<span data-ttu-id="aaf6d-121">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-121">Global admin</span></span>|<span data-ttu-id="aaf6d-122">\*    すべての特権を備えたすべての Microsoft アカウントまたはサービスへのアクセスが可能</span><span class="sxs-lookup"><span data-stu-id="aaf6d-122">\*    Can access all Microsoft account/services with full privileges</span></span>|[<span data-ttu-id="aaf6d-123">パートナー センター アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-123">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
|      |<span data-ttu-id="aaf6d-124">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="aaf6d-124">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="aaf6d-125">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-125">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="aaf6d-126">\*    契約、価格表、オファーの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-126">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="aaf6d-127">\*    パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-127">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="aaf6d-128">課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-128">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="aaf6d-129">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-129">User management admin</span></span>   | <span data-ttu-id="aaf6d-130">\*    ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-130">\*    View, create, and manage users</span></span>|[<span data-ttu-id="aaf6d-131">パートナー センターで Microsoft Partner Network メンバーシップの特典とプランを管理する</span><span class="sxs-lookup"><span data-stu-id="aaf6d-131">Manage your Microsoft Partner Network membership benefits and offers in Partner Center</span></span>](manage-your-partner-network-benefits.md)
||<span data-ttu-id="aaf6d-132">\*    すべてのパートナー プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-132">\*    View all partner profiles</span></span>
||<span data-ttu-id="aaf6d-133">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="aaf6d-133">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="aaf6d-134">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-134">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="aaf6d-135">課金管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-135">Billing admin</span></span> | <span data-ttu-id="aaf6d-136">- 課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-136">- View, create, and manage billing, invoices, and recon files</span></span>|[<span data-ttu-id="aaf6d-137">請求書の記載事項</span><span class="sxs-lookup"><span data-stu-id="aaf6d-137">Read your bill</span></span>](billing.md)
||<span data-ttu-id="aaf6d-138">\*    価格の表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-138">\*    View pricing</span></span>
||<span data-ttu-id="aaf6d-139">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="aaf6d-139">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="aaf6d-140">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-140">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="aaf6d-141">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="aaf6d-141">Default user</span></span>|  <span data-ttu-id="aaf6d-142">マイ プロフィールの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-142">View My profile</span></span>   |[<span data-ttu-id="aaf6d-143">パスワードをリセットする</span><span class="sxs-lookup"><span data-stu-id="aaf6d-143">Reset your password</span></span>](reset-my-pasword.md)
|<span data-ttu-id="aaf6d-144">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="aaf6d-144">Admin agent</span></span> | <span data-ttu-id="aaf6d-145">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-145">\*    Customer management</span></span>|[<span data-ttu-id="aaf6d-146">お客様とつながる</span><span class="sxs-lookup"><span data-stu-id="aaf6d-146">Connect with your customers</span></span>](connect-with-your-customers.md)
||<span data-ttu-id="aaf6d-147">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="aaf6d-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="aaf6d-148">\*    プロファイルの作成とデバイスへの適用</span><span class="sxs-lookup"><span data-stu-id="aaf6d-148">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="aaf6d-149">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-149">\*    Subscription management</span></span>
||<span data-ttu-id="aaf6d-150">\*    顧客のためのサービスの正常性とサービス要求</span><span class="sxs-lookup"><span data-stu-id="aaf6d-150">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="aaf6d-151">\*    代理管理者特権の要求</span><span class="sxs-lookup"><span data-stu-id="aaf6d-151">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="aaf6d-152">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="aaf6d-153">\*    請求</span><span class="sxs-lookup"><span data-stu-id="aaf6d-153">\*    Billing</span></span>
||<span data-ttu-id="aaf6d-154">\*    顧客の代理としての管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-154">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="aaf6d-155">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="aaf6d-155">\*    Register a value added reseller</span></span>
||<span data-ttu-id="aaf6d-156">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="aaf6d-156">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="aaf6d-157">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-157">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="aaf6d-158">販売代理店</span><span class="sxs-lookup"><span data-stu-id="aaf6d-158">Sales agent</span></span> | <span data-ttu-id="aaf6d-159">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-159">\*    Customer management</span></span>|[<span data-ttu-id="aaf6d-160">顧客に課金サポートを提供し、請求に関する質問に答える</span><span class="sxs-lookup"><span data-stu-id="aaf6d-160">Provide billing support for your customers and help answer their billing questions</span></span>](provide-billing-support.md)
||<span data-ttu-id="aaf6d-161">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="aaf6d-161">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="aaf6d-162">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-162">\*    Subscription management</span></span>
||<span data-ttu-id="aaf6d-163">\*    サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-163">\*    View support tickets</span></span>
||<span data-ttu-id="aaf6d-164">\*    顧客との再販業者関係の要求</span><span class="sxs-lookup"><span data-stu-id="aaf6d-164">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="aaf6d-165">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-165">\*    View pricing and offers</span></span>
||<span data-ttu-id="aaf6d-166">\*    潜在顧客の管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-166">\*    Manage customer leads</span></span>
||<span data-ttu-id="aaf6d-167">\*    顧客契約の表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-167">\*    View the customer agreement</span></span>
||<span data-ttu-id="aaf6d-168">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="aaf6d-168">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="aaf6d-169">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="aaf6d-169">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="aaf6d-170">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-170">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="aaf6d-171">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="aaf6d-171">Helpdesk agent</span></span>| <span data-ttu-id="aaf6d-172">\*    顧客の検索と表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-172">\*    Search for and view a customer</span></span>|[<span data-ttu-id="aaf6d-173">Microsoft への問題のエスカレーション、および Microsoft へのエスカレーションに適した問題の見極め方</span><span class="sxs-lookup"><span data-stu-id="aaf6d-173">Escalate problems to Microsoft and learn which issues are more-suited to Microsoft escalation</span></span>](escalate-problems-to-microsoft.md)
||<span data-ttu-id="aaf6d-174">\*    顧客の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="aaf6d-174">\*    Edit customer details</span></span>
||<span data-ttu-id="aaf6d-175">\*    請求またはサブスクリプション管理に関する顧客の問題の解決サポート</span><span class="sxs-lookup"><span data-stu-id="aaf6d-175">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="aaf6d-176">\*    顧客の代理としてのサポート要求</span><span class="sxs-lookup"><span data-stu-id="aaf6d-176">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="aaf6d-177">\*    顧客の代理としてのサブスクリプションと請求に関する問題の管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-177">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="aaf6d-178">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="aaf6d-178">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="aaf6d-179">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-179">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a><span data-ttu-id="aaf6d-180">コントロール パネル ベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="aaf6d-180">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="aaf6d-181">(CSP ロールと非 Azure AD ロール)</span><span class="sxs-lookup"><span data-stu-id="aaf6d-181">(CSP role and non-Azure AD role)</span></span>

<span data-ttu-id="aaf6d-182">CPV は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムとパートナー センター API を統合するために使用するアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="aaf6d-182">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="aaf6d-183">**Role**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-183">**Role**</span></span>   |<span data-ttu-id="aaf6d-184">**できること**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-184">**What you can do**</span></span>|<span data-ttu-id="aaf6d-185">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-185">**Learn more**</span></span>|
|------------------------------|:----------------------------|----|
|<span data-ttu-id="aaf6d-186">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-186">Global admin</span></span>| <span data-ttu-id="aaf6d-187">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-187">View and manage your CPV profile</span></span>|[<span data-ttu-id="aaf6d-188">CSP パートナー システムとパートナー センター API との統合を支援するためにコントロール パネル ベンダーとして登録する</span><span class="sxs-lookup"><span data-stu-id="aaf6d-188">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>](enroll-as-cpv.md)
||<span data-ttu-id="aaf6d-189">CPV 機能にアクセスする必要があるユーザーの表示と管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-189">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a><span data-ttu-id="aaf6d-190">ゲスト ユーザー (Azure Active Directory テナントに追加する必要あり)</span><span class="sxs-lookup"><span data-stu-id="aaf6d-190">Guest user (must be added to the Azure Active Directory tenant)</span></span>

|<span data-ttu-id="aaf6d-191">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-191">**Guest user**</span></span>   | <span data-ttu-id="aaf6d-192">**ロール**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-192">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="aaf6d-193">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-193">MPN partner admin</span></span>|
||<span data-ttu-id="aaf6d-194">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-194">Accounts admin</span></span>|
||<span data-ttu-id="aaf6d-195">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-195">Incentives admin</span></span>|
||<span data-ttu-id="aaf6d-196">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-196">Business profile admin</span></span>|
||<span data-ttu-id="aaf6d-197">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-197">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company"></a><span data-ttu-id="aaf6d-198">MPN メンバーシップと貴社の管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-198">Manage MPN membership and your company</span></span> 

<span data-ttu-id="aaf6d-199">次のロールは Azure Active Directory ロールではありません。</span><span class="sxs-lookup"><span data-stu-id="aaf6d-199">These roles are not Azure Active Directory roles.</span></span> <span data-ttu-id="aaf6d-200">これらのロールでは、テナントではなく会社のビジネスを管理します。</span><span class="sxs-lookup"><span data-stu-id="aaf6d-200">These roles manage the company business rather than the tenant.</span></span>

|<span data-ttu-id="aaf6d-201">**Role**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-201">**Role**</span></span> | <span data-ttu-id="aaf6d-202">**できること**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-202">**What you can do**</span></span>|<span data-ttu-id="aaf6d-203">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-203">**Learn more**</span></span>|
|----------------------------|:----------------------------|-----|
|<span data-ttu-id="aaf6d-204">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-204">MPN partner admin</span></span>|<span data-ttu-id="aaf6d-205">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-205">\*    View, create, and manage partner service requests</span></span>|[<span data-ttu-id="aaf6d-206">Microsoft Action Pack サブスクリプションや Silver コンピテンシーと Gold コンピテンシーを購入または更新する</span><span class="sxs-lookup"><span data-stu-id="aaf6d-206">Buy or renew a Microsoft Action Pack subscription or silver and gold competencies</span></span>](mpn-get-action-pack.md)
||<span data-ttu-id="aaf6d-207">\*    法的プロファイル、企業プロファイル、ビジネス プロファイル、MPN プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-207">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="aaf6d-208">\*    ユーザーの詳細およびスキル データの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-208">\*    View user details and their skills data</span></span>
||<span data-ttu-id="aaf6d-209">\*    コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-209">\*    View competencies</span></span>
||<span data-ttu-id="aaf6d-210">\*    特典の表示と管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-210">\*    View and manage benefits</span></span>
||<span data-ttu-id="aaf6d-211">\*    MPN オファーの表示と購入</span><span class="sxs-lookup"><span data-stu-id="aaf6d-211">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="aaf6d-212">\*    MPN オファーの注文履歴と請求書の表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-212">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="aaf6d-213">\*    パートナー貢献度インジケーター データの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-213">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="aaf6d-214">\*    利用券検証ツールでの作業</span><span class="sxs-lookup"><span data-stu-id="aaf6d-214">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="aaf6d-215">\*    顧客データ分析の表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-215">\*    View customer data analytics</span></span>
||<span data-ttu-id="aaf6d-216">\*    会社内の他のユーザー ロールを表示しますが、ロールを割り当てることはできません</span><span class="sxs-lookup"><span data-stu-id="aaf6d-216">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="aaf6d-217">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="aaf6d-217">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="aaf6d-218">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-218">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="aaf6d-219">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-219">Account admin</span></span>| <span data-ttu-id="aaf6d-220">場所の追加</span><span class="sxs-lookup"><span data-stu-id="aaf6d-220">Add locations</span></span>|[<span data-ttu-id="aaf6d-221">場所の管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-221">Manage locations</span></span>](manage-locations.md)
|| <span data-ttu-id="aaf6d-222">管理対象のアカウントに関連するプロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-222">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="aaf6d-223">\*    テナント内のユーザーに対するロールの非 Azure-Active-Directory ロールへの割り当て</span><span class="sxs-lookup"><span data-stu-id="aaf6d-223">\*    Assign roles for users in tenant to non-Azure-Active-Directory roles</span></span> 
||<span data-ttu-id="aaf6d-224">\*    プログラムへの場所の登録</span><span class="sxs-lookup"><span data-stu-id="aaf6d-224">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="aaf6d-225">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="aaf6d-225">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="aaf6d-226">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-226">\*    View partner support tickets you create</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="aaf6d-227">紹介の管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-227">Manage referrals</span></span> 

|<span data-ttu-id="aaf6d-228">**Role**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-228">**Role**</span></span>|<span data-ttu-id="aaf6d-229">**できること**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-229">**What you can do**</span></span>|<span data-ttu-id="aaf6d-230">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-230">**Learn more**</span></span>|
|-----------------------------|:------------------------|---|
|<span data-ttu-id="aaf6d-231">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-231">Referrals admin</span></span>       |<span data-ttu-id="aaf6d-232">\*    ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-232">\*    View, create, and manage business profiles</span></span>|[<span data-ttu-id="aaf6d-233">顧客の問い合わせ、マーケティングに適した潜在顧客、販売に適した潜在顧客などのさまざまな潜在顧客を管理する</span><span class="sxs-lookup"><span data-stu-id="aaf6d-233">Manage different leads like customer inquiries, marketing-qualified leads, and sales-qualified leads</span></span>](manage-leads.md)
||<span data-ttu-id="aaf6d-234">\*    紹介の受信と管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-234">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="aaf6d-235">\*    共同販売の紹介の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-235">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="aaf6d-236">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-236">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="aaf6d-237">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-237">Business profile admin</span></span>   |<span data-ttu-id="aaf6d-238">\*    ビジネス プロファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-238">\* View, create, and manage business profile</span></span> |[<span data-ttu-id="aaf6d-239">ビジネス プロファイルの作成</span><span class="sxs-lookup"><span data-stu-id="aaf6d-239">Create a business profile</span></span>](create-a-marketing-profile.md)
||<span data-ttu-id="aaf6d-240">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-240">\*    View, create, and manage partner service requests</span></span>
||<span data-ttu-id="aaf6d-241">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="aaf6d-241">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="aaf6d-242">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-242">\*    View partner support tickets you create</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="aaf6d-243">インセンティブの管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-243">Manage incentives</span></span> 

|<span data-ttu-id="aaf6d-244">**Role**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-244">**Role**</span></span> | <span data-ttu-id="aaf6d-245">**できること**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-245">**What you can do**</span></span>|<span data-ttu-id="aaf6d-246">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-246">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="aaf6d-247">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="aaf6d-247">Incentives admin</span></span>|<span data-ttu-id="aaf6d-248">\*    インセンティブの開始と管理</span><span class="sxs-lookup"><span data-stu-id="aaf6d-248">\*    Initiates and manages incentives</span></span> |[<span data-ttu-id="aaf6d-249">これらのリソースを使用してインセンティブを使い始める</span><span class="sxs-lookup"><span data-stu-id="aaf6d-249">Use these resources to help you get started with incentives</span></span>](incentives-get-started-intro.md)
||<span data-ttu-id="aaf6d-250">\*    インセンティブ プログラムのすべての側面の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="aaf6d-250">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="aaf6d-251">\*    銀行および税の詳細情報の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="aaf6d-251">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="aaf6d-252">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-252">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="aaf6d-253">\*    サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="aaf6d-253">\*    Access support</span></span>
||<span data-ttu-id="aaf6d-254">\*    インセンティブ支払いについての議論</span><span class="sxs-lookup"><span data-stu-id="aaf6d-254">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="aaf6d-255">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="aaf6d-255">Incentives user</span></span>|<span data-ttu-id="aaf6d-256">\*    インセンティブ プログラムを表示可能</span><span class="sxs-lookup"><span data-stu-id="aaf6d-256">\*    Can view incentives programs</span></span>
||<span data-ttu-id="aaf6d-257">\*    インセンティブの申請の表示と開始が可能</span><span class="sxs-lookup"><span data-stu-id="aaf6d-257">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="aaf6d-258">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-258">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="aaf6d-259">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="aaf6d-259">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="aaf6d-260">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-260">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="aaf6d-261">パートナー センター インサイト データの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-261">View Partner Center Insights data</span></span>

|<span data-ttu-id="aaf6d-262">**Role**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-262">**Role**</span></span> | <span data-ttu-id="aaf6d-263">**できること**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-263">**What you can do**</span></span>|<span data-ttu-id="aaf6d-264">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="aaf6d-264">**Learn more**</span></span>|
|------------------------------|:-------------------------|---|
|<span data-ttu-id="aaf6d-265">エグゼクティブ レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="aaf6d-265">Executive report viewer</span></span>|<span data-ttu-id="aaf6d-266">すべてのレポート データセットへのアクセス、パートナー サポート チケットの作成、作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-266">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|[<span data-ttu-id="aaf6d-267">パートナー センターの分析情報で利用できる概要ダッシュボード レポート</span><span class="sxs-lookup"><span data-stu-id="aaf6d-267">Overview dashboard reports available in Partner Center Insights</span></span>](pci-overview-report.md)
|<span data-ttu-id="aaf6d-268">レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="aaf6d-268">Report viewer</span></span>|<span data-ttu-id="aaf6d-269">収益や顧客と従業員の個人データを除くデータ レポートへのアクセス、パートナー サポート チケットの作成、作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="aaf6d-269">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|

## <a name="next-steps"></a><span data-ttu-id="aaf6d-270">次のステップ</span><span class="sxs-lookup"><span data-stu-id="aaf6d-270">Next steps</span></span>

- [<span data-ttu-id="aaf6d-271">ユーザー アカウントの作成およびロールとアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="aaf6d-271">Create user accounts and assign roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)
- [<span data-ttu-id="aaf6d-272">新しいパートナー センター プログラムに登録する際のアカウント情報の確認</span><span class="sxs-lookup"><span data-stu-id="aaf6d-272">Verify your account information when you enroll in a new Partner Center program</span></span>](verification-responses.md)
