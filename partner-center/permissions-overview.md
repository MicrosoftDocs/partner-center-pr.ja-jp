---
title: ユーザー ロールとアクセス許可の割り当て |パートナー センター
ms.topic: article
ms.date: 3/5/19
description: すべての従業員がパートナー センターで動作する必要がありますが、ロールを割り当てる必要があります。
author: LauraBrenner
ms.author: labrenne
keywords: ロール, アクセス許可, 管理者, エージェント
ms.localizationpriority: medium
ms.openlocfilehash: 66923c8a5d4912d178ef483a883f08f40ed8378b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133902"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="c5d81-104">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="c5d81-104">Assign users roles and permissions</span></span>


<span data-ttu-id="c5d81-105">有効な名前とアドレス、サポートの詳細、税の除外対象をファイル、銀行情報、および会社の主要な連絡先を含む、パートナーのプロファイルを設定しました。</span><span class="sxs-lookup"><span data-stu-id="c5d81-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="c5d81-106">次の手順: をパートナー センターで作業を開始するため、パスワードとロールを設定するユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="c5d81-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="c5d81-107">パートナー センターで使用する従業員を設定します。</span><span class="sxs-lookup"><span data-stu-id="c5d81-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="c5d81-108">役割とアクセス許可を付けると、パートナー センターにユーザーが持つアクセス権の種類を決定します。</span><span class="sxs-lookup"><span data-stu-id="c5d81-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="c5d81-109">ロールで、ビジネスが関係しているプログラムに関連しています。</span><span class="sxs-lookup"><span data-stu-id="c5d81-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="c5d81-110">たとえば、会社がクラウド ソリューション プロバイダー (CSP) ビジネスの場合は、必要はありませんのみ標準の Azure AD テナント グローバル管理者などの管理ロールが必要がありますの役割、CSP プログラムに固有です。</span><span class="sxs-lookup"><span data-stu-id="c5d81-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="c5d81-111">各プログラムには、固有の役割があります。</span><span class="sxs-lookup"><span data-stu-id="c5d81-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="c5d81-112">Azure Active Directory (AAD) テナント ロールには、グローバル管理者、ユーザー管理者、および CSP の役割が含まれます。</span><span class="sxs-lookup"><span data-stu-id="c5d81-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="c5d81-113">非 AAD のロールには、MPN 管理者、ビジネス プロファイルの管理、参照の管理、インセンティブの管理者およびインセンティブのユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="c5d81-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="c5d81-114">パートナー センターでの商用トランザクションを管理する (Azure AD と CSP の役割)</span><span class="sxs-lookup"><span data-stu-id="c5d81-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="c5d81-115">**ロール**</span><span class="sxs-lookup"><span data-stu-id="c5d81-115">**Role**</span></span>|<span data-ttu-id="c5d81-116">**何ができます。**</span><span class="sxs-lookup"><span data-stu-id="c5d81-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="c5d81-117">全体管理者</span><span class="sxs-lookup"><span data-stu-id="c5d81-117">Global admin</span></span>|<span data-ttu-id="c5d81-118">• 完全な特権を持つ Microsoft アカウントが/サービスすべてにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="c5d81-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="c5d81-119">• パートナー センターのサポート チケットを作成します。</span><span class="sxs-lookup"><span data-stu-id="c5d81-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="c5d81-120">• 契約の表示、価格表、および特典</span><span class="sxs-lookup"><span data-stu-id="c5d81-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="c5d81-121">• ビューの作成、およびパートナーのユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="c5d81-122">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="c5d81-122">User Admin</span></span>   | <span data-ttu-id="c5d81-123">• ビューの作成、およびユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="c5d81-124">• すべてのパートナー プロファイルを表示します。</span><span class="sxs-lookup"><span data-stu-id="c5d81-124">• View all partner profiles</span></span>
||<span data-ttu-id="c5d81-125">• ビューの作成、およびパートナーのユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="c5d81-126">課金の管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-126">Billing admin</span></span> | <span data-ttu-id="c5d81-127">-表示、作成、および課金や請求書、recon ファイルを管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-127">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="c5d81-128">既定のユーザー</span><span class="sxs-lookup"><span data-stu-id="c5d81-128">Default user</span></span>|  <span data-ttu-id="c5d81-129">マイ プロファイルを表示します。</span><span class="sxs-lookup"><span data-stu-id="c5d81-129">View My profile</span></span>   |
|<span data-ttu-id="c5d81-130">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="c5d81-130">Admin agent</span></span> | <span data-ttu-id="c5d81-131">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-131">•    Customer management</span></span>
||<span data-ttu-id="c5d81-132">• パートナー センターにデバイスのリストを追加 <</span><span class="sxs-lookup"><span data-stu-id="c5d81-132">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="c5d81-133">• の作成し、プロファイルをデバイスに適用されます。</span><span class="sxs-lookup"><span data-stu-id="c5d81-133">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="c5d81-134">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-134">• Subscription management</span></span>
||<span data-ttu-id="c5d81-135">顧客の • サービス正常性とサービス要求</span><span class="sxs-lookup"><span data-stu-id="c5d81-135">• Service health and service requests for customers</span></span>
||<span data-ttu-id="c5d81-136">• 要求が委任された管理者特権</span><span class="sxs-lookup"><span data-stu-id="c5d81-136">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="c5d81-137">• 表示価格とプランに関する</span><span class="sxs-lookup"><span data-stu-id="c5d81-137">• View pricing and offers</span></span>
||<span data-ttu-id="c5d81-138">• 請求</span><span class="sxs-lookup"><span data-stu-id="c5d81-138">• Billing</span></span>
||<span data-ttu-id="c5d81-139">• は、お客様に代わって管理を行う</span><span class="sxs-lookup"><span data-stu-id="c5d81-139">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="c5d81-140">• レジスタ値を再販業者の追加</span><span class="sxs-lookup"><span data-stu-id="c5d81-140">• Register a value added reseller</span></span>|
|<span data-ttu-id="c5d81-141">販売代理店</span><span class="sxs-lookup"><span data-stu-id="c5d81-141">Sales agent</span></span> | <span data-ttu-id="c5d81-142">• 顧客の管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-142">•    Customer management</span></span>
||<span data-ttu-id="c5d81-143">• デバイスの一覧をパートナー センターに追加</span><span class="sxs-lookup"><span data-stu-id="c5d81-143">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="c5d81-144">• サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-144">• Subscription management</span></span>
||<span data-ttu-id="c5d81-145">• ビューのサポート チケット</span><span class="sxs-lookup"><span data-stu-id="c5d81-145">• View support tickets</span></span>
||<span data-ttu-id="c5d81-146">• 顧客とのリレーションシップの要求</span><span class="sxs-lookup"><span data-stu-id="c5d81-146">• Request a relationship with a customer</span></span>
||<span data-ttu-id="c5d81-147">• 潜在顧客の管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-147">• Manage customer leads</span></span>
||<span data-ttu-id="c5d81-148">• 顧客契約書の表示</span><span class="sxs-lookup"><span data-stu-id="c5d81-148">• View the customer agreement</span></span>
||<span data-ttu-id="c5d81-149">• レジスタ付加価値再販業者</span><span class="sxs-lookup"><span data-stu-id="c5d81-149">• Register a value-added reseller</span></span>|
|<span data-ttu-id="c5d81-150">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="c5d81-150">Helpdesk agent</span></span>| <span data-ttu-id="c5d81-151">• 検索し、顧客の表示</span><span class="sxs-lookup"><span data-stu-id="c5d81-151">•  Search for and view a customer</span></span>
||<span data-ttu-id="c5d81-152">• 顧客詳細の編集</span><span class="sxs-lookup"><span data-stu-id="c5d81-152">• Edit customer details</span></span>
||<span data-ttu-id="c5d81-153">• ヘルプ顧客の問題を解決課金やサブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-153">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="c5d81-154">顧客に代わって • 要求のサポート (注。管理エージェントでの Office 365 サブスクリプションには、このタスクを完了する必要があります)</span><span class="sxs-lookup"><span data-stu-id="c5d81-154">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="c5d81-155">• サブスクリプションの管理し、課金顧客に代わって問題 (注。管理エージェントでの Office 365 サブスクリプションには、このタスクを完了する必要があります)</span><span class="sxs-lookup"><span data-stu-id="c5d81-155">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="c5d81-156">コントロール パネルのベンダー (CPV)。</span><span class="sxs-lookup"><span data-stu-id="c5d81-156">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="c5d81-157">(CSP のロールと非 AAD ロール)</span><span class="sxs-lookup"><span data-stu-id="c5d81-157">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="c5d81-158">CPVs では、パートナー センター Api と、システムを統合するためのクラウド ソリューション プロバイダー (CSP) パートナーで使用するためのアプリを開発します。</span><span class="sxs-lookup"><span data-stu-id="c5d81-158">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="c5d81-159">**ロール**</span><span class="sxs-lookup"><span data-stu-id="c5d81-159">**Role**</span></span>   |<span data-ttu-id="c5d81-160">**何ができます。**</span><span class="sxs-lookup"><span data-stu-id="c5d81-160">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="c5d81-161">全体管理者</span><span class="sxs-lookup"><span data-stu-id="c5d81-161">Global admin</span></span>| <span data-ttu-id="c5d81-162">表示および CPV プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-162">View and manage your CPV profile</span></span>|
||<span data-ttu-id="c5d81-163">表示および CPV 機能へのアクセスを必要とするユーザーの管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-163">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="c5d81-164">MPN メンバーシップと会社 (非 AAD ロールを) 管理します。</span><span class="sxs-lookup"><span data-stu-id="c5d81-164">Manage MPN membership and your company (non-AAD roles)</span></span>

|<span data-ttu-id="c5d81-165">**ロール**</span><span class="sxs-lookup"><span data-stu-id="c5d81-165">**Role**</span></span> | <span data-ttu-id="c5d81-166">**何ができます。**</span><span class="sxs-lookup"><span data-stu-id="c5d81-166">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="c5d81-167">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="c5d81-167">MPN partner admin</span></span>|<span data-ttu-id="c5d81-168">•Can は、テナント以外のユーザーを追加します。</span><span class="sxs-lookup"><span data-stu-id="c5d81-168">•Can add non-tenant users</span></span>
||<span data-ttu-id="c5d81-169">• ビューの作成、およびパートナー サービス要求の管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-169">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="c5d81-170">• 法的ビュー、組織、ビジネス、および MPN プロファイル</span><span class="sxs-lookup"><span data-stu-id="c5d81-170">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="c5d81-171">• ユーザーの詳細の表示とそのスキル データ</span><span class="sxs-lookup"><span data-stu-id="c5d81-171">• View user details and their skills data</span></span>
||<span data-ttu-id="c5d81-172">• コンピテンシーを表示します</span><span class="sxs-lookup"><span data-stu-id="c5d81-172">• View competencies</span></span>
||<span data-ttu-id="c5d81-173">• の表示し、管理の利点があります</span><span class="sxs-lookup"><span data-stu-id="c5d81-173">• View and manage benefits</span></span>
||<span data-ttu-id="c5d81-174">MPN の提供 • ビューと購入</span><span class="sxs-lookup"><span data-stu-id="c5d81-174">• View and purchase MPN offers</span></span>
||<span data-ttu-id="c5d81-175">• MPN のビューには、注文履歴と請求書が提供しています</span><span class="sxs-lookup"><span data-stu-id="c5d81-175">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="c5d81-176">• パートナー コントリビューション データの表示</span><span class="sxs-lookup"><span data-stu-id="c5d81-176">• View partner contribution data</span></span>
||<span data-ttu-id="c5d81-177">• には、バウチャーの検証ツールを動作します。</span><span class="sxs-lookup"><span data-stu-id="c5d81-177">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="c5d81-178">-顧客データの分析を表示します。</span><span class="sxs-lookup"><span data-stu-id="c5d81-178">- View customer data analytics</span></span>
|<span data-ttu-id="c5d81-179">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="c5d81-179">Account admin</span></span>| <span data-ttu-id="c5d81-180">• は、テナント以外のユーザーを追加できます。</span><span class="sxs-lookup"><span data-stu-id="c5d81-180">•   Can add non-tenant users</span></span>
||<span data-ttu-id="c5d81-181">• を追加または場所の削除</span><span class="sxs-lookup"><span data-stu-id="c5d81-181">• Add or delete locations</span></span>
||<span data-ttu-id="c5d81-182">-ユーザーが管理者のアカウントに関連するプロファイルを管理します。</span><span class="sxs-lookup"><span data-stu-id="c5d81-182">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="c5d81-183">• 非 AAD のロールをテナントのユーザーのロールの割り当て</span><span class="sxs-lookup"><span data-stu-id="c5d81-183">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="c5d81-184">• プログラムに場所を登録します。</span><span class="sxs-lookup"><span data-stu-id="c5d81-184">• Enroll locations into programs</span></span>

## <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="c5d81-185">ゲスト ユーザーの (AAD テナントに追加する必要があります)</span><span class="sxs-lookup"><span data-stu-id="c5d81-185">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="c5d81-186">**ゲスト ユーザー**</span><span class="sxs-lookup"><span data-stu-id="c5d81-186">**Guest user**</span></span>   | <span data-ttu-id="c5d81-187">**Roles**</span><span class="sxs-lookup"><span data-stu-id="c5d81-187">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="c5d81-188">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="c5d81-188">MPN partner admin</span></span>|
||<span data-ttu-id="c5d81-189">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="c5d81-189">Accounts admin</span></span>|
||<span data-ttu-id="c5d81-190">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="c5d81-190">Incentives admin</span></span>|
||<span data-ttu-id="c5d81-191">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="c5d81-191">Business profile admin</span></span>|
||<span data-ttu-id="c5d81-192">参照の管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-192">Referrals admin</span></span>|


## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="c5d81-193">(非 AAD ロール) の参照を管理します。</span><span class="sxs-lookup"><span data-stu-id="c5d81-193">Manage referrals (non-AAD roles)</span></span>

|<span data-ttu-id="c5d81-194">**ロール**</span><span class="sxs-lookup"><span data-stu-id="c5d81-194">**Role**</span></span>|<span data-ttu-id="c5d81-195">**何ができます。**</span><span class="sxs-lookup"><span data-stu-id="c5d81-195">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="c5d81-196">参照の管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-196">Referrals admin</span></span>       |<span data-ttu-id="c5d81-197">• ビューの作成、およびビジネス プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-197">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="c5d81-198">• が受信し、参照の管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-198">• Receive and manage referrals</span></span>
||<span data-ttu-id="c5d81-199">• ビューの作成、およびパートナー サービス要求の管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-199">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="c5d81-200">ビジネス プロファイル管理者</span><span class="sxs-lookup"><span data-stu-id="c5d81-200">Business profile admin</span></span>   |<span data-ttu-id="c5d81-201">•View、作成、およびビジネス プロファイルの管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-201">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="c5d81-202">• ビューの作成、およびパートナー サービス要求の管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-202">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="c5d81-203">インセンティブ (非 AAD ロール) の管理します。</span><span class="sxs-lookup"><span data-stu-id="c5d81-203">Manage Incentives  (non-AAD roles)</span></span>

|<span data-ttu-id="c5d81-204">**ロール**</span><span class="sxs-lookup"><span data-stu-id="c5d81-204">**Role**</span></span> | <span data-ttu-id="c5d81-205">**何ができます。**</span><span class="sxs-lookup"><span data-stu-id="c5d81-205">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="c5d81-206">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="c5d81-206">Incentives admin</span></span>|<span data-ttu-id="c5d81-207">• が開始し、インセンティブの管理</span><span class="sxs-lookup"><span data-stu-id="c5d81-207">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="c5d81-208">• を表示およびインセンティブ プログラムのすべての側面を編集できます。</span><span class="sxs-lookup"><span data-stu-id="c5d81-208">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="c5d81-209">• を表示および銀行と税の詳細を編集できます。</span><span class="sxs-lookup"><span data-stu-id="c5d81-209">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="c5d81-210">• ビュー リベートと co-op 収益</span><span class="sxs-lookup"><span data-stu-id="c5d81-210">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="c5d81-211">• アクセスのサポート</span><span class="sxs-lookup"><span data-stu-id="c5d81-211">• Access support</span></span>
||<span data-ttu-id="c5d81-212">• 争議インセンティブの支払い</span><span class="sxs-lookup"><span data-stu-id="c5d81-212">• Dispute incentives payments</span></span>|
|<span data-ttu-id="c5d81-213">インセンティブ ユーザー</span><span class="sxs-lookup"><span data-stu-id="c5d81-213">Incentives user</span></span>|<span data-ttu-id="c5d81-214">• は、インセンティブ プログラムを表示できます。</span><span class="sxs-lookup"><span data-stu-id="c5d81-214">•  Can view incentives programs</span></span>
||<span data-ttu-id="c5d81-215">• を表示およびインセンティブの要求を開始できます。</span><span class="sxs-lookup"><span data-stu-id="c5d81-215">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="c5d81-216">• ビュー リベートと co-op 収益</span><span class="sxs-lookup"><span data-stu-id="c5d81-216">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="c5d81-217">• ビュー リベートと co-op 収益</span><span class="sxs-lookup"><span data-stu-id="c5d81-217">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="c5d81-218">• アクセスのサポート</span><span class="sxs-lookup"><span data-stu-id="c5d81-218">• Access support</span></span>












