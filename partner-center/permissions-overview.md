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
ms.custom: SEOMAY.20, contperfq1
ms.openlocfilehash: 4839fbd6fac5f84e5a2ebc40d1f7f48da6114113
ms.sourcegitcommit: 92be474db61cc12f684850c2a7a8a8bdd5c93f97
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/05/2020
ms.locfileid: "93363624"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="f05b5-103">パートナー センターで作業する必要がある会社のユーザーにユーザーのロールとアクセス許可を割り当てる</span><span class="sxs-lookup"><span data-stu-id="f05b5-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="f05b5-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="f05b5-104">**Appropriate roles**</span></span>

- <span data-ttu-id="f05b5-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="f05b5-105">Global admin</span></span>
- <span data-ttu-id="f05b5-106">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="f05b5-106">User admin</span></span>
- <span data-ttu-id="f05b5-107">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="f05b5-107">MPN partner admin</span></span>

<span data-ttu-id="f05b5-108">貴社の正式名称や法的住所、サポートの詳細、税金の除外の申告、銀行情報、主要な連絡先など、パートナー プロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="f05b5-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="f05b5-109">次のステップ:ユーザーにパスワードとロールを設定させて、ユーザーがパートナー センターでの作業を開始できるようにします。</span><span class="sxs-lookup"><span data-stu-id="f05b5-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="f05b5-110">パートナー センターで作業できるように従業員を設定する</span><span class="sxs-lookup"><span data-stu-id="f05b5-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="f05b5-111">ユーザーに付与するロールとアクセス許可によって、パートナー センターでのユーザーのアクセスの種類が決まります。</span><span class="sxs-lookup"><span data-stu-id="f05b5-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="f05b5-112">ロールは、貴社のビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="f05b5-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="f05b5-113">たとえば、貴社のビジネスがクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、グローバル管理者などの標準の Azure Active Directory テナント管理ロールだけでなく、CSP プログラムに固有のロールも必要です。</span><span class="sxs-lookup"><span data-stu-id="f05b5-113">For example, if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure Active Directory tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="f05b5-114">各プログラムには、それに固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="f05b5-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="f05b5-115">Azure Active Directory テナント ロールには、グローバル管理者、ユーザー管理者、CSP のロールが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f05b5-115">Azure Active Directory tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="f05b5-116">Azure Active Directory 以外のロールはテナントを管理しないロールであり、MPN 管理者、ビジネス プロファイル管理者、紹介管理者、インセンティブ管理者、インセンティブ ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f05b5-116">Non-Azure-Active-Directory roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="f05b5-117">パートナー センターで商取引を管理する (Azure AD と CSP のロール)</span><span class="sxs-lookup"><span data-stu-id="f05b5-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="f05b5-118">**Role**</span><span class="sxs-lookup"><span data-stu-id="f05b5-118">**Role**</span></span>|<span data-ttu-id="f05b5-119">**できること**</span><span class="sxs-lookup"><span data-stu-id="f05b5-119">**What they can do**</span></span>|<span data-ttu-id="f05b5-120">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="f05b5-120">**Learn more**</span></span>|
|----------------------------------|---|:---------------------------------|
|<span data-ttu-id="f05b5-121">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="f05b5-121">Global admin</span></span>|<span data-ttu-id="f05b5-122">\*    すべての特権を備えたすべての Microsoft アカウントまたはサービスへのアクセスが可能</span><span class="sxs-lookup"><span data-stu-id="f05b5-122">\*    Can access all Microsoft account/services with full privileges</span></span>|[<span data-ttu-id="f05b5-123">パートナー センター アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-123">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
|      |<span data-ttu-id="f05b5-124">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="f05b5-124">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="f05b5-125">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-125">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="f05b5-126">\*    契約、価格表、オファーの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-126">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="f05b5-127">\*    パートナー ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-127">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="f05b5-128">課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-128">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="f05b5-129">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="f05b5-129">User management admin</span></span>   | <span data-ttu-id="f05b5-130">\*    ユーザーの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-130">\*    View, create, and manage users</span></span>|[<span data-ttu-id="f05b5-131">パートナー センターで Microsoft Partner Network メンバーシップの特典とプランを管理する</span><span class="sxs-lookup"><span data-stu-id="f05b5-131">Manage your Microsoft Partner Network membership benefits and offers in Partner Center</span></span>](manage-your-partner-network-benefits.md)
||<span data-ttu-id="f05b5-132">\*    すべてのパートナー プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-132">\*    View all partner profiles</span></span>
||<span data-ttu-id="f05b5-133">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="f05b5-133">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="f05b5-134">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-134">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="f05b5-135">課金管理者</span><span class="sxs-lookup"><span data-stu-id="f05b5-135">Billing admin</span></span> | <span data-ttu-id="f05b5-136">- 課金、請求書、調整ファイルの表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-136">- View, create, and manage billing, invoices, and recon files</span></span>|[<span data-ttu-id="f05b5-137">請求書の記載事項</span><span class="sxs-lookup"><span data-stu-id="f05b5-137">Read your bill</span></span>](billing.md)
||<span data-ttu-id="f05b5-138">\*    価格の表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-138">\*    View pricing</span></span>
||<span data-ttu-id="f05b5-139">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="f05b5-139">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="f05b5-140">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-140">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="f05b5-141">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="f05b5-141">Default user</span></span>|  <span data-ttu-id="f05b5-142">マイ プロフィールの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-142">View My profile</span></span>   |[<span data-ttu-id="f05b5-143">パスワードをリセットする</span><span class="sxs-lookup"><span data-stu-id="f05b5-143">Reset your password</span></span>](reset-my-pasword.md)
|<span data-ttu-id="f05b5-144">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="f05b5-144">Admin agent</span></span> | <span data-ttu-id="f05b5-145">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-145">\*    Customer management</span></span>|[<span data-ttu-id="f05b5-146">お客様とつながる</span><span class="sxs-lookup"><span data-stu-id="f05b5-146">Connect with your customers</span></span>](connect-with-your-customers.md)
||<span data-ttu-id="f05b5-147">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="f05b5-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="f05b5-148">\*    プロファイルの作成とデバイスへの適用</span><span class="sxs-lookup"><span data-stu-id="f05b5-148">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="f05b5-149">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-149">\*    Subscription management</span></span>
||<span data-ttu-id="f05b5-150">\*    顧客のためのサービスの正常性とサービス要求</span><span class="sxs-lookup"><span data-stu-id="f05b5-150">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="f05b5-151">\*    代理管理者特権の要求</span><span class="sxs-lookup"><span data-stu-id="f05b5-151">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="f05b5-152">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="f05b5-153">\*    請求</span><span class="sxs-lookup"><span data-stu-id="f05b5-153">\*    Billing</span></span>
||<span data-ttu-id="f05b5-154">\*    顧客の代理としての管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-154">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="f05b5-155">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="f05b5-155">\*    Register a value added reseller</span></span>
||<span data-ttu-id="f05b5-156">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="f05b5-156">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="f05b5-157">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-157">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="f05b5-158">販売代理店</span><span class="sxs-lookup"><span data-stu-id="f05b5-158">Sales agent</span></span> | <span data-ttu-id="f05b5-159">\*    顧客の管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-159">\*    Customer management</span></span>|[<span data-ttu-id="f05b5-160">顧客に課金サポートを提供し、請求に関する質問に答える</span><span class="sxs-lookup"><span data-stu-id="f05b5-160">Provide billing support for your customers and help answer their billing questions</span></span>](provide-billing-support.md)
||<span data-ttu-id="f05b5-161">\*    パートナー センターへのデバイス一覧の追加</span><span class="sxs-lookup"><span data-stu-id="f05b5-161">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="f05b5-162">\*    サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-162">\*    Subscription management</span></span>
||<span data-ttu-id="f05b5-163">\*    サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-163">\*    View support tickets</span></span>
||<span data-ttu-id="f05b5-164">\*    顧客との再販業者関係の要求</span><span class="sxs-lookup"><span data-stu-id="f05b5-164">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="f05b5-165">\*    価格とオファーの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-165">\*    View pricing and offers</span></span>
||<span data-ttu-id="f05b5-166">\*    潜在顧客の管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-166">\*    Manage customer leads</span></span>
||<span data-ttu-id="f05b5-167">\*    顧客契約の表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-167">\*    View the customer agreement</span></span>
||<span data-ttu-id="f05b5-168">\*    付加価値リセラーの登録</span><span class="sxs-lookup"><span data-stu-id="f05b5-168">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="f05b5-169">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="f05b5-169">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="f05b5-170">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-170">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="f05b5-171">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="f05b5-171">Helpdesk agent</span></span>| <span data-ttu-id="f05b5-172">\*    顧客の検索と表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-172">\*    Search for and view a customer</span></span>|[<span data-ttu-id="f05b5-173">Microsoft への問題のエスカレーション、および Microsoft へのエスカレーションに適した問題の見極め方</span><span class="sxs-lookup"><span data-stu-id="f05b5-173">Escalate problems to Microsoft and learn which issues are more-suited to Microsoft escalation</span></span>](escalate-problems-to-microsoft.md)
||<span data-ttu-id="f05b5-174">\*    顧客の詳細の編集</span><span class="sxs-lookup"><span data-stu-id="f05b5-174">\*    Edit customer details</span></span>
||<span data-ttu-id="f05b5-175">\*    請求またはサブスクリプション管理に関する顧客の問題の解決サポート</span><span class="sxs-lookup"><span data-stu-id="f05b5-175">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="f05b5-176">\*    顧客の代理としてのサポート要求</span><span class="sxs-lookup"><span data-stu-id="f05b5-176">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="f05b5-177">\*    顧客の代理としてのサブスクリプションと請求に関する問題の管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-177">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="f05b5-178">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="f05b5-178">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="f05b5-179">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-179">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a><span data-ttu-id="f05b5-180">コントロール パネル ベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="f05b5-180">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="f05b5-181">(CSP ロールと非 Azure AD ロール)</span><span class="sxs-lookup"><span data-stu-id="f05b5-181">(CSP role and non-Azure AD role)</span></span>

<span data-ttu-id="f05b5-182">CPV は、クラウド ソリューション プロバイダー (CSP) パートナーがシステムとパートナー センター API を統合するために使用するアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="f05b5-182">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="f05b5-183">**Role**</span><span class="sxs-lookup"><span data-stu-id="f05b5-183">**Role**</span></span>   |<span data-ttu-id="f05b5-184">**できること**</span><span class="sxs-lookup"><span data-stu-id="f05b5-184">**What you can do**</span></span>|<span data-ttu-id="f05b5-185">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="f05b5-185">**Learn more**</span></span>|
|------------------------------|:----------------------------|----|
|<span data-ttu-id="f05b5-186">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="f05b5-186">Global admin</span></span>| <span data-ttu-id="f05b5-187">CPV プロファイルの表示と管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-187">View and manage your CPV profile</span></span>|[<span data-ttu-id="f05b5-188">CSP パートナー システムとパートナー センター API との統合を支援するためにコントロール パネル ベンダーとして登録する</span><span class="sxs-lookup"><span data-stu-id="f05b5-188">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>](enroll-as-cpv.md)
||<span data-ttu-id="f05b5-189">CPV 機能にアクセスする必要があるユーザーの表示と管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-189">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a><span data-ttu-id="f05b5-190">ゲスト ユーザー (Azure Active Directory テナントに追加する必要あり)</span><span class="sxs-lookup"><span data-stu-id="f05b5-190">Guest user (must be added to the Azure Active Directory tenant)</span></span>

|<span data-ttu-id="f05b5-191">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="f05b5-191">**Guest user**</span></span>   | <span data-ttu-id="f05b5-192">**ロール**</span><span class="sxs-lookup"><span data-stu-id="f05b5-192">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="f05b5-193">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="f05b5-193">MPN partner admin</span></span>|
||<span data-ttu-id="f05b5-194">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="f05b5-194">Business profile admin</span></span>|
||<span data-ttu-id="f05b5-195">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="f05b5-195">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company"></a><span data-ttu-id="f05b5-196">MPN メンバーシップと貴社の管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-196">Manage MPN membership and your company</span></span> 

<span data-ttu-id="f05b5-197">次のロールは Azure Active Directory ロールではありません。</span><span class="sxs-lookup"><span data-stu-id="f05b5-197">These roles are not Azure Active Directory roles.</span></span> <span data-ttu-id="f05b5-198">これらのロールでは、テナントではなく会社のビジネスを管理します。</span><span class="sxs-lookup"><span data-stu-id="f05b5-198">These roles manage the company business rather than the tenant.</span></span>

|<span data-ttu-id="f05b5-199">**Role**</span><span class="sxs-lookup"><span data-stu-id="f05b5-199">**Role**</span></span> | <span data-ttu-id="f05b5-200">**できること**</span><span class="sxs-lookup"><span data-stu-id="f05b5-200">**What you can do**</span></span>|<span data-ttu-id="f05b5-201">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="f05b5-201">**Learn more**</span></span>|
|----------------------------|:----------------------------|-----|
|<span data-ttu-id="f05b5-202">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="f05b5-202">MPN partner admin</span></span>|<span data-ttu-id="f05b5-203">\*    パートナー サービス要求の表示、作成、管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-203">\*    View, create, and manage partner service requests</span></span>|[<span data-ttu-id="f05b5-204">Microsoft Action Pack サブスクリプションや Silver コンピテンシーと Gold コンピテンシーを購入または更新する</span><span class="sxs-lookup"><span data-stu-id="f05b5-204">Buy or renew a Microsoft Action Pack subscription or silver and gold competencies</span></span>](mpn-get-action-pack.md)
||<span data-ttu-id="f05b5-205">\*    法的プロファイル、企業プロファイル、ビジネス プロファイル、MPN プロファイルの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-205">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="f05b5-206">\*    ユーザーの詳細およびスキル データの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-206">\*    View user details and their skills data</span></span>
||<span data-ttu-id="f05b5-207">\*    コンピテンシーの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-207">\*    View competencies</span></span>
||<span data-ttu-id="f05b5-208">\*    特典の表示と管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-208">\*    View and manage benefits</span></span>
||<span data-ttu-id="f05b5-209">\*    MPN オファーの表示と購入</span><span class="sxs-lookup"><span data-stu-id="f05b5-209">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="f05b5-210">\*    MPN オファーの注文履歴と請求書の表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-210">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="f05b5-211">\*    パートナー貢献度インジケーター データの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-211">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="f05b5-212">\*    利用券検証ツールでの作業</span><span class="sxs-lookup"><span data-stu-id="f05b5-212">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="f05b5-213">\*    顧客データ分析の表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-213">\*    View customer data analytics</span></span>
||<span data-ttu-id="f05b5-214">\*    会社内の他のユーザー ロールを表示しますが、ロールを割り当てることはできません</span><span class="sxs-lookup"><span data-stu-id="f05b5-214">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="f05b5-215">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="f05b5-215">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="f05b5-216">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-216">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="f05b5-217">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="f05b5-217">Account admin</span></span>| <span data-ttu-id="f05b5-218">場所の追加</span><span class="sxs-lookup"><span data-stu-id="f05b5-218">Add locations</span></span>|[<span data-ttu-id="f05b5-219">場所の管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-219">Manage locations</span></span>](manage-locations.md)
|| <span data-ttu-id="f05b5-220">管理対象のアカウントに関連するプロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-220">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="f05b5-221">\*    テナント内のユーザーに対するロールの非 Azure-Active-Directory ロールへの割り当て</span><span class="sxs-lookup"><span data-stu-id="f05b5-221">\*    Assign roles for users in tenant to non-Azure-Active-Directory roles</span></span> 
||<span data-ttu-id="f05b5-222">\*    プログラムへの場所の登録</span><span class="sxs-lookup"><span data-stu-id="f05b5-222">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="f05b5-223">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="f05b5-223">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="f05b5-224">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-224">\*    View partner support tickets you create</span></span>

## <a name="manage-referrals"></a><span data-ttu-id="f05b5-225">紹介の管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-225">Manage referrals</span></span>

> [!Note]
><span data-ttu-id="f05b5-226">新しい紹介ユーザー ロールは、2020 年 11 月 16 日から使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="f05b5-226">The new Referrals user role will be available starting 16th November 2020.</span></span> <span data-ttu-id="f05b5-227">既存の紹介管理者は、会社全体を対象とした紹介管理者ロールを保持します。</span><span class="sxs-lookup"><span data-stu-id="f05b5-227">Existing referral admins will retain their referral admin role scoped to the entire company.</span></span>

|<span data-ttu-id="f05b5-228">**Role**</span><span class="sxs-lookup"><span data-stu-id="f05b5-228">**Role**</span></span> | <span data-ttu-id="f05b5-229">**できること**</span><span class="sxs-lookup"><span data-stu-id="f05b5-229">**What you can do**</span></span>|<span data-ttu-id="f05b5-230">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="f05b5-230">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="f05b5-231">紹介管理者</span><span class="sxs-lookup"><span data-stu-id="f05b5-231">Referrals admin</span></span>|<span data-ttu-id="f05b5-232">パートナー センターの [紹介] タブにあるすべてのものを作成および管理する</span><span class="sxs-lookup"><span data-stu-id="f05b5-232">Create and manage everything under Referrals tab in Partner Center</span></span>|[<span data-ttu-id="f05b5-233">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="f05b5-233">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="f05b5-234">すべての共同販売の機会と潜在顧客を表示および編集できます</span><span class="sxs-lookup"><span data-stu-id="f05b5-234">Can view and edit all the co-sell opportunities and leads</span></span>
||    <span data-ttu-id="f05b5-235">取引にチーム メンバーを割り当てることができます</span><span class="sxs-lookup"><span data-stu-id="f05b5-235">Can assign team members for a deal</span></span>
||    <span data-ttu-id="f05b5-236">ビジネス プロファイルを表示および編集できます</span><span class="sxs-lookup"><span data-stu-id="f05b5-236">Can view and edit business profiles</span></span>
||    <span data-ttu-id="f05b5-237">成立し、取引登録の対象としてマークされている営業案件の表示と登録を行うことができます</span><span class="sxs-lookup"><span data-stu-id="f05b5-237">Can view and register deals for opportunities that are marked as won and eligible for deal registration</span></span>
||    <span data-ttu-id="f05b5-238">サポート チケットを作成および表示できます</span><span class="sxs-lookup"><span data-stu-id="f05b5-238">Can create and view support tickets</span></span>
|<span data-ttu-id="f05b5-239">紹介ユーザー</span><span class="sxs-lookup"><span data-stu-id="f05b5-239">Referrals user</span></span>|<span data-ttu-id="f05b5-240">チームの一員である場合にのみ共同販売の機会を作成および管理する</span><span class="sxs-lookup"><span data-stu-id="f05b5-240">Create and manage co-sell opportunities only if they are a part of the team</span></span> |[<span data-ttu-id="f05b5-241">共同販売の機会を管理する</span><span class="sxs-lookup"><span data-stu-id="f05b5-241">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="f05b5-242">ロールが割り当てられている場所の共同販売機会を作成できます。</span><span class="sxs-lookup"><span data-stu-id="f05b5-242">Can create co-sell opportunities for the locations where they are assigned the role.</span></span>
||    <span data-ttu-id="f05b5-243">チーム メンバーである場合、成立し、取引登録の対象としてマークされている営業案件の表示と登録を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="f05b5-243">Can view and register deals for opportunities that are marked as won and eligible for deal registration if they are team member.</span></span>
||    <span data-ttu-id="f05b5-244">サポート チケットを作成および表示できます</span><span class="sxs-lookup"><span data-stu-id="f05b5-244">Can create and view support tickets</span></span>
|<span data-ttu-id="f05b5-245">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="f05b5-245">Business profile admin</span></span>|<span data-ttu-id="f05b5-246">ビジネス プロファイルを作成および管理します</span><span class="sxs-lookup"><span data-stu-id="f05b5-246">Create and manage business profiles</span></span> | [<span data-ttu-id="f05b5-247">ビジネス プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-247">Manage business profiles</span></span>](create-a-marketing-profile.md)
||    <span data-ttu-id="f05b5-248">サポート チケットを作成および表示できます</span><span class="sxs-lookup"><span data-stu-id="f05b5-248">Can create and view support tickets</span></span>

<span data-ttu-id="f05b5-249">新しい参照ユーザー ロールと共に、取引の場所のスコープも導入されます。</span><span class="sxs-lookup"><span data-stu-id="f05b5-249">Along with the new referrals user role, we are also introducing the location scope for deals.</span></span> <span data-ttu-id="f05b5-250">下の表では、場所に基づく取引アクセスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="f05b5-250">The table below explains the deals-access based on the location.</span></span>

|<span data-ttu-id="f05b5-251">**スコープ**</span><span class="sxs-lookup"><span data-stu-id="f05b5-251">**Scope**</span></span> | <span data-ttu-id="f05b5-252">**できること**</span><span class="sxs-lookup"><span data-stu-id="f05b5-252">**What you can do**</span></span> |
|------------------------------|:-------------------------|
|<span data-ttu-id="f05b5-253">会社全体</span><span class="sxs-lookup"><span data-stu-id="f05b5-253">Entire company</span></span> | <span data-ttu-id="f05b5-254">管理者とユーザーの両方が、会社内の任意の場所に対する取引を作成するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="f05b5-254">Both admins and users have access to create deals for any location in their company</span></span>|
|| <span data-ttu-id="f05b5-255">紹介管理者は、すべての取引を表示および編集するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="f05b5-255">Referral admin has access to view and edit all the deals</span></span> |
|| <span data-ttu-id="f05b5-256">紹介ユーザーは、チームの一員である場合にのみ、すべての取引を表示および編集するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="f05b5-256">Referral users have access to view and edit all the deals only if they are a part of the team</span></span> |
|<span data-ttu-id="f05b5-257">1 つまたは複数の場所</span><span class="sxs-lookup"><span data-stu-id="f05b5-257">One or more locations</span></span> | <span data-ttu-id="f05b5-258">管理者とユーザーの両方が、会社内の割り当てられた場所の取引を作成するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="f05b5-258">Both admins and users have access to create deals for the assigned location in their company</span></span>|
|| <span data-ttu-id="f05b5-259">紹介管理者は、割り当てられた場所に属するすべての取引を表示および編集するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="f05b5-259">Referral admin has access to view and edit all the deals belonging to the assigned locations</span></span>|
|| <span data-ttu-id="f05b5-260">紹介ユーザーは、チームに属している場合、割り当てられた場所に属するすべての取引を表示および編集するためのアクセス権を持っています</span><span class="sxs-lookup"><span data-stu-id="f05b5-260">Referral users have access to view and edit all the deals belonging to the assigned locations if they are part of the team</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="f05b5-261">インセンティブの管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-261">Manage incentives</span></span>

|<span data-ttu-id="f05b5-262">**Role**</span><span class="sxs-lookup"><span data-stu-id="f05b5-262">**Role**</span></span> | <span data-ttu-id="f05b5-263">**できること**</span><span class="sxs-lookup"><span data-stu-id="f05b5-263">**What you can do**</span></span>|<span data-ttu-id="f05b5-264">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="f05b5-264">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="f05b5-265">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="f05b5-265">Incentives admin</span></span>|<span data-ttu-id="f05b5-266">\*    インセンティブの開始と管理</span><span class="sxs-lookup"><span data-stu-id="f05b5-266">\*    Initiates and manages incentives</span></span> |[<span data-ttu-id="f05b5-267">これらのリソースを使用してインセンティブを使い始める</span><span class="sxs-lookup"><span data-stu-id="f05b5-267">Use these resources to help you get started with incentives</span></span>](incentives-get-started-intro.md)
||<span data-ttu-id="f05b5-268">\*    インセンティブ プログラムのすべての側面の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="f05b5-268">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="f05b5-269">\*    銀行および税の詳細情報の表示と編集が可能</span><span class="sxs-lookup"><span data-stu-id="f05b5-269">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="f05b5-270">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-270">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="f05b5-271">\*    サポートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="f05b5-271">\*    Access support</span></span>
||<span data-ttu-id="f05b5-272">\*    インセンティブ支払いについての議論</span><span class="sxs-lookup"><span data-stu-id="f05b5-272">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="f05b5-273">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="f05b5-273">Incentives user</span></span>|<span data-ttu-id="f05b5-274">\*    インセンティブ プログラムを表示可能</span><span class="sxs-lookup"><span data-stu-id="f05b5-274">\*    Can view incentives programs</span></span>
||<span data-ttu-id="f05b5-275">\*    インセンティブの申請の表示と開始が可能</span><span class="sxs-lookup"><span data-stu-id="f05b5-275">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="f05b5-276">\*    リベートや共同収益の表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-276">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="f05b5-277">\*    パートナー センターへのサポート チケットの作成</span><span class="sxs-lookup"><span data-stu-id="f05b5-277">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="f05b5-278">\*    作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-278">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="f05b5-279">パートナー センター インサイト データの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-279">View Partner Center Insights data</span></span>

|<span data-ttu-id="f05b5-280">**Role**</span><span class="sxs-lookup"><span data-stu-id="f05b5-280">**Role**</span></span> | <span data-ttu-id="f05b5-281">**できること**</span><span class="sxs-lookup"><span data-stu-id="f05b5-281">**What you can do**</span></span>|<span data-ttu-id="f05b5-282">**詳細情報**</span><span class="sxs-lookup"><span data-stu-id="f05b5-282">**Learn more**</span></span>|
|------------------------------|:-------------------------|---|
|<span data-ttu-id="f05b5-283">エグゼクティブ レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="f05b5-283">Executive report viewer</span></span>|<span data-ttu-id="f05b5-284">すべてのレポート データセットへのアクセス、パートナー サポート チケットの作成、作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-284">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|[<span data-ttu-id="f05b5-285">パートナー センターの分析情報で利用できる概要ダッシュボード レポート</span><span class="sxs-lookup"><span data-stu-id="f05b5-285">Overview dashboard reports available in Partner Center Insights</span></span>](pci-overview-report.md)
|<span data-ttu-id="f05b5-286">レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="f05b5-286">Report viewer</span></span>|<span data-ttu-id="f05b5-287">収益や顧客と従業員の個人データを除くデータ レポートへのアクセス、パートナー サポート チケットの作成、作成されたパートナー サポート チケットの表示</span><span class="sxs-lookup"><span data-stu-id="f05b5-287">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|

## <a name="next-steps"></a><span data-ttu-id="f05b5-288">次のステップ</span><span class="sxs-lookup"><span data-stu-id="f05b5-288">Next steps</span></span>

- [<span data-ttu-id="f05b5-289">ユーザー アカウントの作成およびロールとアクセス許可の設定</span><span class="sxs-lookup"><span data-stu-id="f05b5-289">Create user accounts and assign roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)
- [<span data-ttu-id="f05b5-290">新しいパートナー センター プログラムに登録する際のアカウント情報の確認</span><span class="sxs-lookup"><span data-stu-id="f05b5-290">Verify your account information when you enroll in a new Partner Center program</span></span>](verification-responses.md)
