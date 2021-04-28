---
title: Kaizala Pro サブスクリプションを Microsoft 365 に移行する
description: Kaizala Pro サブスクリプションを Microsoft 365 または Office 365 バージョンに移行する方法について説明します。 お客様の移行の詳細については、この記事をご覧ください。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 96d18c8f728c56b705d378ac56dcf46e777157f0
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172406"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="ab665-104">Kaizala Pro スタンドアロンサブスクリプションを Microsoft 365 または Office 365 バージョンに移行する</span><span class="sxs-lookup"><span data-stu-id="ab665-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="ab665-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="ab665-105">**Appropriate roles**</span></span>

- <span data-ttu-id="ab665-106">販売代理店</span><span class="sxs-lookup"><span data-stu-id="ab665-106">Sales agent</span></span>

<span data-ttu-id="ab665-107">2020年7月1日より、Microsoft は Kaizala Pro スタンドアロンサービスの売上を終了します。</span><span class="sxs-lookup"><span data-stu-id="ab665-107">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="ab665-108">お客様は、この日より後に新しい Kaizala Pro サブスクリプションを購入することはできなくなります。また、既存の Kaizala Pro サブスクリプションは、有効期限が切れると自動的に更新されません。</span><span class="sxs-lookup"><span data-stu-id="ab665-108">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="ab665-109">お客様の継続性を確保するには、Kaizala Pro スタンドアロンサブスクリプションが期限切れになっているお客様を、サポートされている SKU オプション (下記参照) に移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ab665-109">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="ab665-110">顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="ab665-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="ab665-111">API (CREST またはパートナーセンター) を使用する場合、[自動更新] プロパティを false に設定して、サブスクリプションの終了日を評価することで、期限切れのサブスクリプションを検出できます `auto renew = False` 。</span><span class="sxs-lookup"><span data-stu-id="ab665-111">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="ab665-112">E4 サブスクリプションは `auto renew=False` 、2020年7月1日に設定されます。</span><span class="sxs-lookup"><span data-stu-id="ab665-112">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="ab665-113">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="ab665-113">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="ab665-114">Kaizala Pro スタンドアロン置換プラン</span><span class="sxs-lookup"><span data-stu-id="ab665-114">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="ab665-115">新しいプランでは、お客様は Microsoft 365 の新しい機能を利用できます。</span><span class="sxs-lookup"><span data-stu-id="ab665-115">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="ab665-116">料金の詳細は、パートナー センターの料金表またはプランのマトリックスに記載されています。</span><span class="sxs-lookup"><span data-stu-id="ab665-116">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="ab665-117">次を含む [**ビジネス向け Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2):</span><span class="sxs-lookup"><span data-stu-id="ab665-117">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="ab665-118">Microsoft 365 Business Basic</span><span class="sxs-lookup"><span data-stu-id="ab665-118">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="ab665-119">Microsoft 365 Business Standard</span><span class="sxs-lookup"><span data-stu-id="ab665-119">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="ab665-120">Microsoft 365 Business Premium</span><span class="sxs-lookup"><span data-stu-id="ab665-120">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="ab665-121">[**最前線の Microsoft 365**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)(次を含む):</span><span class="sxs-lookup"><span data-stu-id="ab665-121">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="ab665-122">Microsoft 365 F3 (旧称 Microsoft 365 F1) と Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="ab665-122">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="ab665-123">以下を含む、 [**Enterprise の Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans):</span><span class="sxs-lookup"><span data-stu-id="ab665-123">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="ab665-124">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="ab665-124">Office 365 E1</span></span>
   - <span data-ttu-id="ab665-125">Microsoft 365 E3 および Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="ab665-125">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="ab665-126">Microsoft 365 E5 および Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="ab665-126">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="ab665-127">以下を含む [**教育の Microsoft 365**](https://www.microsoft.com/education/buy-license/microsoft365):</span><span class="sxs-lookup"><span data-stu-id="ab665-127">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="ab665-128">Microsoft 365 A1 と Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="ab665-128">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="ab665-129">Microsoft 365 A3 と Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="ab665-129">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="ab665-130">Microsoft 365 A5 と Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="ab665-130">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="ab665-131">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="ab665-131">Transition customers to new product plans</span></span>

<span data-ttu-id="ab665-132">マイクロソフトは、絶えず新しい製品やサービスをパートナーに提供しています。</span><span class="sxs-lookup"><span data-stu-id="ab665-132">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="ab665-133">パートナーはこれに対応して、お客様を新しいサービスにアップグレードするか、お客様のサブスクリプションを廃止予定の SKU から移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ab665-133">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="ab665-134">廃止された SKU から新しい SKU にお客様を移行するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="ab665-134">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="ab665-135">A.</span><span class="sxs-lookup"><span data-stu-id="ab665-135">A.</span></span> <span data-ttu-id="ab665-136">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="ab665-136">Purchase the new subscription</span></span>

<span data-ttu-id="ab665-137">B.</span><span class="sxs-lookup"><span data-stu-id="ab665-137">B.</span></span> <span data-ttu-id="ab665-138">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="ab665-138">Reassign current user licenses</span></span>

<span data-ttu-id="ab665-139">C.</span><span class="sxs-lookup"><span data-stu-id="ab665-139">C.</span></span> <span data-ttu-id="ab665-140">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="ab665-140">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="ab665-141">新しいプランにお客様を移行する</span><span class="sxs-lookup"><span data-stu-id="ab665-141">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="ab665-142">A.</span><span class="sxs-lookup"><span data-stu-id="ab665-142">A.</span></span> <span data-ttu-id="ab665-143">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="ab665-143">Purchase the new subscription</span></span>

1. <span data-ttu-id="ab665-144">新しいサブスクリプションを購入するには、 **パートナーセンター** メニューから [ **顧客**] を選択し、移動する顧客を選択して、[ **サブスクリプションの追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ab665-144">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="ab665-145">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="ab665-145">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="ab665-146">お客様は、以前のサブスクリプションと新しいサブスクリプション (オプション 1-Office 365 Enterprise F1 など) の両方を使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="ab665-146">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="ab665-147">B.</span><span class="sxs-lookup"><span data-stu-id="ab665-147">B.</span></span> <span data-ttu-id="ab665-148">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="ab665-148">Reassign current user licenses</span></span>

1. <span data-ttu-id="ab665-149">顧客のユーザーのライセンスをもう一度割り当てるには、**パートナー センター** メニューで **[顧客]** を選び、移行する顧客を選んでから **[ユーザーとライセンス]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="ab665-149">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="ab665-150">顧客の [ユーザーとライセンス] ページが開きます。</span><span class="sxs-lookup"><span data-stu-id="ab665-150">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="ab665-151">ユーザーライセンスを再割り当てするには、再割り当てするユーザーを選択し、[ **ライセンスの管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ab665-151">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="ab665-152">[ **ライセンスの管理** ] ページで、[Kaizala Pro スタンドアロンライセンス] チェックボックスをオフにし、顧客の移動先のサブスクリプションの新しいサービスプランを選択します。</span><span class="sxs-lookup"><span data-stu-id="ab665-152">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="ab665-153">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ab665-153">Select **Submit**.</span></span> <span data-ttu-id="ab665-154">確認ページに新しいライセンスの割り当てが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="ab665-154">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="ab665-155">ライセンスの割り当てが必要な他のユーザーにも同じプロセスを続行します。</span><span class="sxs-lookup"><span data-stu-id="ab665-155">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="ab665-156">C.</span><span class="sxs-lookup"><span data-stu-id="ab665-156">C.</span></span> <span data-ttu-id="ab665-157">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="ab665-157">Cancel old subscription</span></span>

<span data-ttu-id="ab665-158">ユーザー ライセンスを新しいサービスに移行した後は、顧客レベルで廃止されたサブスクリプションを安全に取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="ab665-158">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="ab665-159">**パートナー センター** メニューで、**[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ab665-159">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="ab665-160">サブスクリプションをキャンセルする顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="ab665-160">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="ab665-161">サブスクリプションの詳細ページで、サブスクリプションを **[中断]** に設定します。</span><span class="sxs-lookup"><span data-stu-id="ab665-161">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="ab665-162">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ab665-162">Select **Submit**.</span></span>

<span data-ttu-id="ab665-163">以前のサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="ab665-163">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="ab665-164">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="ab665-164">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="ab665-165">お客様には、以前のサブスクリプションの追加コストは発生しません。</span><span class="sxs-lookup"><span data-stu-id="ab665-165">The customer incurs no additional costs for the old subscription.</span></span>
