---
title: Dynamics AX のサブスクリプションを Dynamics 365 に移行する | パートナー センター
description: Microsoft では、次世代のインテリジェント ビジネス アプリケーションである Dynamics 365 を公開しました。これにより、お客様の組織を成長、進化、および変化させ、顧客のニーズに合わせて、新しいビジネスの機会を捕らえることができます。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.localizationpriority: medium
ms.openlocfilehash: f5e03825226171b8002b260e1b00a59a5eb53ebb
ms.sourcegitcommit: 123a7f53d633c27eb5f982926d856de47afb1042
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/09/2018
ms.locfileid: "4489788"
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a><span data-ttu-id="5edc1-103">Dynamics AX のサブスクリプションを Dynamics 365 に移行する</span><span class="sxs-lookup"><span data-stu-id="5edc1-103">Migrate Dynamics AX subscriptions to Dynamics 365</span></span>

**<span data-ttu-id="5edc1-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="5edc1-104">Applies to</span></span>**

-  <span data-ttu-id="5edc1-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="5edc1-105">Partner Center</span></span>

<span data-ttu-id="5edc1-106">Microsoft では、次世代のインテリジェント ビジネス アプリケーションである Dynamics 365 を公開しました。これにより、お客様の組織を成長、進化、および変化させ、顧客のニーズに合わせて、新しいビジネスの機会を捕らえることができます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-106">Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities.</span></span> <span data-ttu-id="5edc1-107">新製品の一部として、マイクロソフトでは、2016 年 11 月 1 日に顧客向けの新しい Microsoft Dynamics サブスクリプション プランを導入しました。このプランは現行のプランと類似していますが、若干の違いがあります。</span><span class="sxs-lookup"><span data-stu-id="5edc1-107">As part of the new product, Microsoft introduced new Microsoft Dynamics subscription plans for customers on November 1st, 2016, that are similar but not identical to your current plans.</span></span>

<span data-ttu-id="5edc1-108">このドキュメントに示されている手順では、間接プロバイダーが顧客の既存の Microsoft Dynamics AX サブスクリプションと Microsoft Dymanics CRM Online サブスクリプションを Microsoft Dynamics 365 に切り替える方法を説明しています。</span><span class="sxs-lookup"><span data-stu-id="5edc1-108">The instructions in this document describe how indirect providers can switch customers’ existing Microsoft Dynamics AX subscriptions and Microsoft Dymanics CRM Online subscriptions to Microsoft Dynamics 365.</span></span> <span data-ttu-id="5edc1-109">この手順は、他の Microsoft 製品を新しいバージョンに更新する場合や、プロバイダーが顧客のサブスクリプションを新しい SKU に移行する必要がある場合にも適用されます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-109">The instructions also apply to other Microsoft products that update to new versions, requiring providers to migrate customers’ subscriptions to a new SKU.</span></span>

<span data-ttu-id="5edc1-110">Microsoft Dynamics CRM Online および AX プランは廃止されます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-110">The Microsoft Dynamics CRM Online and AX plans are retired.</span></span>  <span data-ttu-id="5edc1-111">2017 年 7 月 1 日以降は、レガシ プランへの更新ができなくなり、既存の E4 サブスクリプションも有効期限満了時に自動更新されません。</span><span class="sxs-lookup"><span data-stu-id="5edc1-111">Effective July 1, 2017, you can no longer renew into the legacy plans, also existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="5edc1-112">CRM Online と AX のサブスクリプションは終了した時点で取り消されます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-112">When CRM Online and AX subscriptions end, they will be canceled.</span></span> <span data-ttu-id="5edc1-113">お客様への継続的なサービス提供を保証するには、有効期限が迫っているサブスクリプションのお客様を、サポートされている以下の SKU オプションに移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5edc1-113">To ensure continuity for customers, plan to transition customers with expiring subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="5edc1-114">お客様のサービスが中断することを避けるため、サブスクリプションの年間終了日前に新しいサブスクリプションにお客様を移行することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5edc1-114">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span> 

<span data-ttu-id="5edc1-115">サブスクリプションの詳細ページでは、有効期限の近づいたサブスクリプションに対して、サブスクリプションの状態が "自動更新: [日付]" から "有効期限: [日付]" に変更されています。</span><span class="sxs-lookup"><span data-stu-id="5edc1-115">On the subscription's detail page, you will see that for these expiring subscriptions, the subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="5edc1-116">API (CREST またはパートナー センターのいずれか) を使用している場合は、サブスクリプションの終了日と auto renew = False プロパティを評価して、有効期限が迫っているサブスクリプションを検出できます。サブスクリプションは、2017 年 7 月 1 日に ”auto renew=False” に設定されています。</span><span class="sxs-lookup"><span data-stu-id="5edc1-116">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.The subscriptions were set to auto renew=False on July 1, 2017.</span></span> <span data-ttu-id="5edc1-117">パートナー様は顧客をいつでも新しいプランに移動することができます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-117">You can move customers to a new plan at any time.</span></span> 

**<span data-ttu-id="5edc1-118">Microsoft Dynamics AX ライセンスの変更</span><span class="sxs-lookup"><span data-stu-id="5edc1-118">Microsoft Dynamics AX licensing changes</span></span>**

<span data-ttu-id="5edc1-119">Microsoft Dynamics AX 製品ラインは廃止されました。2016 年 11 月 1 日以降は利用できません。</span><span class="sxs-lookup"><span data-stu-id="5edc1-119">The Microsoft Dynamics AX product line was retired, effective November 1st, 2016.</span></span> <span data-ttu-id="5edc1-120">Dynamics 365 の新しいライセンス オプションについて詳しくは、[ライセンス ガイド](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5edc1-120">To learn more about the new licensing options for Dynamics 365, review the [Licensing Guide](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf).</span></span>

 <span data-ttu-id="5edc1-121">ライセンスの関連について詳しくは、次の表をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5edc1-121">Refer to the following table for details on license mapping:</span></span>

|**<span data-ttu-id="5edc1-122">廃止された SKU</span><span class="sxs-lookup"><span data-stu-id="5edc1-122">Retired SKU</span></span>**   |**<span data-ttu-id="5edc1-123">Dynamics 365 SKU</span><span class="sxs-lookup"><span data-stu-id="5edc1-123">Dynamics 365 SKU</span></span>**   |
|-------------------|:----------------------|
|<span data-ttu-id="5edc1-124">Enterprise SKU</span><span class="sxs-lookup"><span data-stu-id="5edc1-124">Enterprise SKU</span></span>|<span data-ttu-id="5edc1-125">Microsoft Dynamics 365 for Unified Operations または Microsoft Dynamics 365 プラン</span><span class="sxs-lookup"><span data-stu-id="5edc1-125">Microsoft Dynamics 365 for Unified Operations or Microsoft Dynamics 365 Plan</span></span> |
|<span data-ttu-id="5edc1-126">タスク</span><span class="sxs-lookup"><span data-stu-id="5edc1-126">Task</span></span>|<span data-ttu-id="5edc1-127">Microsoft Dynamics 365 for Activity</span><span class="sxs-lookup"><span data-stu-id="5edc1-127">Microsoft Dynamics 365 for Activity</span></span>
|<span data-ttu-id="5edc1-128">タスク/セルフサービス</span><span class="sxs-lookup"><span data-stu-id="5edc1-128">Task/self service</span></span>|<span data-ttu-id="5edc1-129">Microsoft Dynamics 365 for Team Members</span><span class="sxs-lookup"><span data-stu-id="5edc1-129">Microsoft Dynamics 365 for Team Members</span></span>|
|<span data-ttu-id="5edc1-130">デバイス</span><span class="sxs-lookup"><span data-stu-id="5edc1-130">Device</span></span>|<span data-ttu-id="5edc1-131">Microsoft Dynamics 365 for Operations デバイス</span><span class="sxs-lookup"><span data-stu-id="5edc1-131">Microsoft Dynamics 365 for Operations Device</span></span>|

## <a name="microsoft-dynamics-crm-online-licensing-changes"></a><span data-ttu-id="5edc1-132">Microsoft Dynamics CRM Online ライセンスの変更</span><span class="sxs-lookup"><span data-stu-id="5edc1-132">Microsoft Dynamics CRM Online licensing changes</span></span> 

**<span data-ttu-id="5edc1-133">Microsoft Dynamics CRM Online</span><span class="sxs-lookup"><span data-stu-id="5edc1-133">Microsoft Dynamics CRM Online</span></span>**

<span data-ttu-id="5edc1-134">現在の Microsoft Dynamics CRM Online プランは廃止されました。2016 年 11 月 1 日以降は利用できません。</span><span class="sxs-lookup"><span data-stu-id="5edc1-134">The current Microsoft Dynamics CRM Online plan was retired effective November 1, 2016.</span></span> <span data-ttu-id="5edc1-135">Microsoft Dynamics 365 の新しいライセンス オプションについて詳しくは、[ライセンス ガイド](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5edc1-135">To learn more about the new licensing options for microsoft Dynaics 365, review the [licensing guide](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf).</span></span> <span data-ttu-id="5edc1-136">新しいライセンス オプションについて詳しくは、[CRM Online のお客様向けの重要なお知らせ](https://go.microsoft.com/fwlink/?linkid=831667)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5edc1-136">See [Important information for CRM Online customers](https://go.microsoft.com/fwlink/?linkid=831667) to find out more about new licensing options.</span></span>

<span data-ttu-id="5edc1-137">ライセンスの関連について詳しくは、次の表をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5edc1-137">Refer to the following table for details on license mapping:</span></span>

|**<span data-ttu-id="5edc1-138">廃止された SKU</span><span class="sxs-lookup"><span data-stu-id="5edc1-138">Retired SKU</span></span>**   |**<span data-ttu-id="5edc1-139">Dynamics 365 SKU</span><span class="sxs-lookup"><span data-stu-id="5edc1-139">Dynamics 365 SKU</span></span>**   |
|-------------------|:----------------------|
|<span data-ttu-id="5edc1-140">Enterprise</span><span class="sxs-lookup"><span data-stu-id="5edc1-140">Enterprise</span></span>|<span data-ttu-id="5edc1-141">Dynamics 365 Enterprise Customer Engagement プラン</span><span class="sxs-lookup"><span data-stu-id="5edc1-141">Dynamics 365 Enterprise Customer Engagement Plan</span></span> |
|<span data-ttu-id="5edc1-142">Professional</span><span class="sxs-lookup"><span data-stu-id="5edc1-142">Professional</span></span>|<span data-ttu-id="5edc1-143">Dynamics 365 Enterprise Customer Engagement プラン、Dynamics 365 for Sales、Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="5edc1-143">Dynamics 365 Enterprise Customer Engagement Plan, Dynamics 365 for Sales, or Dynamics 365 for Customer Service</span></span>|
|<span data-ttu-id="5edc1-144">Basic</span><span class="sxs-lookup"><span data-stu-id="5edc1-144">Basic</span></span>|<span data-ttu-id="5edc1-145">Dynamics 365 for Team Members、Dynamics 365 for Sales、Dynamics 365 for Customer Service、Dynamics 365 Enterprise Customer Engagement プラン</span><span class="sxs-lookup"><span data-stu-id="5edc1-145">Dynamics 365 for Team Members, Dynamics 365 for Sales, Dynamics 365 for Customer Service, or Dynamics 365 Enterprise Customer Engagement Plan</span></span>|
|<span data-ttu-id="5edc1-146">Essential</span><span class="sxs-lookup"><span data-stu-id="5edc1-146">Essential</span></span>|<span data-ttu-id="5edc1-147">Dynamics 365 for Team Members</span><span class="sxs-lookup"><span data-stu-id="5edc1-147">Dynamics 365 for Team Members</span></span>|
|<span data-ttu-id="5edc1-148">フィールド サービスアドオン</span><span class="sxs-lookup"><span data-stu-id="5edc1-148">Field service add-on</span></span>|<span data-ttu-id="5edc1-149">Dynamics 365 Enterprise Customer Engagement プランまたは Dynamics 365 for Field Service</span><span class="sxs-lookup"><span data-stu-id="5edc1-149">Dynamics 365 Enterprise Customer Engagement Plan or Dynamics 365 for Field Service</span></span>|
|<span data-ttu-id="5edc1-150">プロジェクト サービス オートメーション アドオン</span><span class="sxs-lookup"><span data-stu-id="5edc1-150">Project Service Authomation Add-on</span></span>|<span data-ttu-id="5edc1-151">Dynamics 365 Customer Engagement プランまたは Dynamics 365 for Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="5edc1-151">Dynamics 365 Customer Engagement Plan or Dynamics 365 for Project Service Automation</span></span>|



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="5edc1-152">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="5edc1-152">Transition customers to new product plans</span></span>


<span data-ttu-id="5edc1-153">Microsoft では、新しい製品やサービスをリセラーとプロバイダー向けに継続的に提供します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-153">Microsoft continuously offers new products and services to resellers and providers.</span></span> <span data-ttu-id="5edc1-154">このような場合、リセラーは、顧客を新しいサービスにアップグレードしたり、顧客のサブスクリプションを最終的には廃止される SKU から移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5edc1-154">In these cases, a reseller may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="5edc1-155">以前の SKU から新しい SKU に顧客を移行するには、次の手順に従う必要があります。</span><span class="sxs-lookup"><span data-stu-id="5edc1-155">Migrating customers from old SKUs to newer ones requires the following sequence:</span></span>

-   <span data-ttu-id="5edc1-156">[新しいサブスクリプションを購入する](#manual-subscription-migration-purchasenewsubsc)。</span><span class="sxs-lookup"><span data-stu-id="5edc1-156">[Purchase the new subscription](#manual-subscription-migration-purchasenewsubsc);</span></span>
-   <span data-ttu-id="5edc1-157">[現在のユーザー ライセンスをもう一度割り当てる](#manual-subscription-migration-reassignlicenses)。</span><span class="sxs-lookup"><span data-stu-id="5edc1-157">[Re-assign current user licenses](#manual-subscription-migration-reassignlicenses);</span></span>
-   <span data-ttu-id="5edc1-158">[以前のサブスクリプションを取り消す](#manual-subscription-migration-cancelsubscriptions)。</span><span class="sxs-lookup"><span data-stu-id="5edc1-158">[Cancel the old subscription](#manual-subscription-migration-cancelsubscriptions).</span></span>

<span data-ttu-id="5edc1-159">次の手順では、Microsoft Dynamics AX または CRM Online から Dynamics 365 に顧客を移行します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-159">In the following procedures, you move a customer from Microsoft Dynamics AX or CRM Online to Dynamics 365.</span></span>

<span data-ttu-id="5edc1-160">この例では、リセラーは、Dynamics AX Enterprise の既存のサブスクリプションを持つユーザーを Dynamics 365 for Operations に移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5edc1-160">In this example, the reseller needs to move a customer with an existing subscription for Dynamics AX Enterprise to Dynamics 365 for Operations.</span></span> <span data-ttu-id="5edc1-161">まず、Dynamics 365 for Operations を購入します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-161">Your first step is to purchase Dynamics 365 for Operations.</span></span>  <span data-ttu-id="5edc1-162">CRM Online を使っている顧客を Microsoft Dynamics 365 へ移行する場合は、次の手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-162">Repeat these steps for a CRM Online customer moving to Microsoft Dynamics 365.</span></span>

<a href="" id="purchasenewsubsc"></a>

**<span data-ttu-id="5edc1-163">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="5edc1-163">Purchase the new subscription</span></span>**

1.  <span data-ttu-id="5edc1-164">**パートナー センター**メニューで、**顧客**を選びます、移行する顧客を選択し、**サブスクリプションの追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-164">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and choose **Add Subscriptions**.</span></span>
2.  <span data-ttu-id="5edc1-165">カタログから購入するサブスクリプション (この場合は、"業務向け Dynamics 365、Enterprise エディション") を選び、ライセンスの数を入力して、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-165">Select the subscription you want to purchase from the catalog (in this case, Dynamics 365 for Operations, Enterprise Edition), enter the number of licenses, and choose **Submit**.</span></span>

    <span data-ttu-id="5edc1-166">この時点では、顧客は以前のサブスクリプションと新しいサブスクリプションの両方を保持することになります。この例では、以前の "Dynamics AX エンタープライズ" と、新しい "対象の" サブスクリプションである "業務向け Dynamics 365、Enterprise エディション" です。</span><span class="sxs-lookup"><span data-stu-id="5edc1-166">Your customer should now have both old and new subscriptions: in this example, the old Dynamics AX Enterprise, and the new ‘target’ subscription, Dynamics 365 for Operations, Enterprise Edition.</span></span>

<a href="" id="reassignlicenses"></a><span data-ttu-id="5edc1-167">次の手順では、既存のすべてのユーザー ライセンスを新しいサブスクリプションにもう一度割り当てます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-167">The next step is to reassign all existing user licenses to the new subscription.</span></span>

**<span data-ttu-id="5edc1-168">ユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="5edc1-168">Reassign user licenses</span></span>**

1.  <span data-ttu-id="5edc1-169">**パートナー センター**メニューで、**顧客**を選びます、移行する顧客を選択し、**ユーザーとライセンス**を選択します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-169">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and choose **Users and licenses**.</span></span> <span data-ttu-id="5edc1-170">顧客の [ユーザーとライセンス] ページが開きます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-170">The customer’s Users and Licenses page opens.</span></span>
2.  <span data-ttu-id="5edc1-171">ユーザー ライセンスをもう一度割り当てるには、割り当てるユーザーを選んでから **[ライセンスの管理]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-171">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>
3.  <span data-ttu-id="5edc1-172">**[ライセンスの管理]** ページで、**[Dynamics AX エンタープライズ]** ライセンスのチェック ボックスをオフにして、**[業務向け Dynamics 365]** ライセンスを選びます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-172">On the **Manage licenses** page, clear the **Dynamics AX Enterprise** license check box and select the **Dynamics 365 for Operations** license.</span></span>
4.  <span data-ttu-id="5edc1-173">**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-173">Select **Submit**.</span></span> <span data-ttu-id="5edc1-174">確認ページに新しいライセンスの割り当てが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-174">A confirmation page lists the new license assignments.</span></span>
5.  <span data-ttu-id="5edc1-175">ライセンスをもう一度割り当てる必要がある他の顧客ユーザーについて、同じ手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-175">Continue the same steps with any other customer users that need license reassignment.</span></span>

<a href="" id="cancelsubscriptions"></a><span data-ttu-id="5edc1-176">ユーザー ライセンスを新しいサービスに移行すると、メニューの最上位にある [顧客] から以前のサブスクリプションを安全に取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-176">After moving the user licenses to the new service, you can safely cancel the old subscription at the top Customer level.</span></span>

**<span data-ttu-id="5edc1-177">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="5edc1-177">Cancel the old subscription</span></span>**

1.  <span data-ttu-id="5edc1-178">**パートナー センター**メニューで、**顧客**を選択し、移行する顧客を選択して、サブスクリプションをキャンセルするを選択します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-178">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and select the subscription you want to cancel.</span></span>
2.  <span data-ttu-id="5edc1-179">サブスクリプションの詳細ページで、サブスクリプションの **[状態]** を **[中断]** に設定します。</span><span class="sxs-lookup"><span data-stu-id="5edc1-179">In the subscription details page, set the subscription **Status** to **Suspended**.</span></span>
3.  <span data-ttu-id="5edc1-180">**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-180">Select **Submit**.</span></span>

<span data-ttu-id="5edc1-181">以前のサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="5edc1-181">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="5edc1-182">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-182">The suspended subscription will automatically be de-provisioned after 120 days.</span></span> <span data-ttu-id="5edc1-183">顧客に対しては、以前のサブスクリプションの追加コストは発生しません。</span><span class="sxs-lookup"><span data-stu-id="5edc1-183">The customer incurs no additional costs for the old subscription.</span></span>

## <a name="additional-considerations"></a><span data-ttu-id="5edc1-184">その他の考慮事項</span><span class="sxs-lookup"><span data-stu-id="5edc1-184">Additional considerations</span></span>


<span data-ttu-id="5edc1-185">さらにサブスクリプションをプロビジョニングするために、顧客をオープン チャネルからクラウド サービス プログラムに移行する場合は、それらの既存のサブスクリプションも移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5edc1-185">If your customer is moving from the Open Channel to the Cloud Services Program for further subscription provisioning, you will also need to migrate their existing subscriptions:</span></span>

-   <span data-ttu-id="5edc1-186">顧客がオープン チャネルを通じて以前のサブスクリプションを受け取る場合、新しい SKU での CSP への移行は簡単です。</span><span class="sxs-lookup"><span data-stu-id="5edc1-186">If the customer received their old subscription through the Open Channel, moving to the CSP on the new SKU is straightforward.</span></span>
-   <span data-ttu-id="5edc1-187">ユーザーがまだ顧客として確立されていない場合は、それらのユーザーを招待することができます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-187">If the customer is not yet established as your customer, you can invite them.</span></span> <span data-ttu-id="5edc1-188">詳しくは、「[Request a relationship with a customer](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx)」(顧客との関係を要求する) ヘルプ トピックをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5edc1-188">For information, see the [Request a relationship with a customer](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx) help topic.</span></span>

<span data-ttu-id="5edc1-189">顧客がお客様を間接プロバイダーとして承認すると、プロビジョニングの手順は上記の手順とほとんど同じになります。新しいサブスクリプションを購入して、ユーザー ライセンスを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="5edc1-189">After the customer accepts you as their indirect provider, the provisioning steps are mostly the same as described above: you purchase the new subscription, and then assign the user licenses.</span></span> <span data-ttu-id="5edc1-190">以前のサブスクリプションの取り消しだけが、異なる手順となります。</span><span class="sxs-lookup"><span data-stu-id="5edc1-190">The only difference involves cancellation of old subscription(s).</span></span> <span data-ttu-id="5edc1-191">新しいプロバイダーは、他のチャネルを通じて取得されたサブスクリプションの中断や取り消しを行うことができません。</span><span class="sxs-lookup"><span data-stu-id="5edc1-191">A new provider cannot cancel suspend/cancel subscriptions acquired via other channels.</span></span> <span data-ttu-id="5edc1-192">顧客が他の販売ルート (オープン チャネルなど) で以前にサブスクリプションを取得している場合、顧客自身がその販売ルートを通じてサブスクリプションを取り消す必要があります。</span><span class="sxs-lookup"><span data-stu-id="5edc1-192">If the customer acquired prior subscriptions in another sales channel, such as the Open channel, the customer will need to cancel it themselves through that channel.</span></span>

 

 



