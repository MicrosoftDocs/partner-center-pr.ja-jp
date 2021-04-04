---
title: Office 365 E4 サブスクリプションの移行
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 エディションは、2017 年 4 月 7 日に廃止されました。 Office 365 の新しいバージョンに、お客様のサブスクリプションを移行する方法について説明します。
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132623"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="a319b-104">Office 365 E4 サブスクリプションの Office 365 の新しいバージョンへの移行</span><span class="sxs-lookup"><span data-stu-id="a319b-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="a319b-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="a319b-105">**Appropriate roles**</span></span>

- <span data-ttu-id="a319b-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="a319b-106">Global admin</span></span>
- <span data-ttu-id="a319b-107">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="a319b-107">User management admin</span></span>
- <span data-ttu-id="a319b-108">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="a319b-108">Admin agent</span></span>
- <span data-ttu-id="a319b-109">販売代理店</span><span class="sxs-lookup"><span data-stu-id="a319b-109">Sales agent</span></span>

<span data-ttu-id="a319b-110">Office 365 Enterprise E4 プランは、2017 年 4 月 7 日に廃止されました。</span><span class="sxs-lookup"><span data-stu-id="a319b-110">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="a319b-111">これ以降、新しい Office 365 E4 サブスクリプションを購入することはできません。また、既存の E4 サブスクリプションは期限切れになっても、自動更新されません。</span><span class="sxs-lookup"><span data-stu-id="a319b-111">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="a319b-112">E4 サブスクリプションは終了した時点で取り消されます。</span><span class="sxs-lookup"><span data-stu-id="a319b-112">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="a319b-113">お客様への継続的なサービス提供を保証するには、有効期限が迫っている E4 サブスクリプションのお客様を、サポートされている以下の SKU オプションに移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a319b-113">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="a319b-114">顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="a319b-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="a319b-115">Office 365 Enterprise E4 は、商用 SKU と政府機関用 SKU の両方が廃止されました。</span><span class="sxs-lookup"><span data-stu-id="a319b-115">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="a319b-116">サブスクリプションの詳細ページでは、E4 サブスクリプションの状態が、"自動更新: [日付]" から "有効期限: [date]" に変更されています。</span><span class="sxs-lookup"><span data-stu-id="a319b-116">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="a319b-117">API (CREST またはパートナー センターのいずれか) を使用している場合は、サブスクリプションの終了日と auto renew = False プロパティを評価して、有効期限が迫っているサブスクリプションを検出できます。</span><span class="sxs-lookup"><span data-stu-id="a319b-117">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="a319b-118">E4 サブスクリプションは、2017 年 4 月 7 日に ”auto renew=False” に設定されています。</span><span class="sxs-lookup"><span data-stu-id="a319b-118">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="a319b-119">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="a319b-119">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="a319b-120">Office 365 Enterprise E4 エディションの置換の計画</span><span class="sxs-lookup"><span data-stu-id="a319b-120">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="a319b-121">E4 と同じ機能を維持するか、お客様に Office 365 と Skype for Business Online の新しい機能を提供するかを選択できます。</span><span class="sxs-lookup"><span data-stu-id="a319b-121">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="a319b-122">料金の詳細は、パートナー センターの料金表またはプランのマトリックスに記載されています。</span><span class="sxs-lookup"><span data-stu-id="a319b-122">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="a319b-123">Secure Product Enterprise E3 または Secure Productive Enterprise E5 は、それぞれ Office 365 Enterprise E3 または Office 365 Enterprise E5 の次のオプションに置き換えることができます。</span><span class="sxs-lookup"><span data-stu-id="a319b-123">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="a319b-124">オプション1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="a319b-124">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="a319b-125">オプション2: Office 365 Enterprise E3 + Skype for Business クラウド PBX</span><span class="sxs-lookup"><span data-stu-id="a319b-125">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="a319b-126">オプション3: Office 365 Enterprise E3 + Skype for Business Plus CAL (料金と機能は E4 相当)</span><span class="sxs-lookup"><span data-stu-id="a319b-126">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="a319b-127">オプション4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="a319b-127">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="a319b-128">機能</span><span class="sxs-lookup"><span data-stu-id="a319b-128">Feature</span></span> | <span data-ttu-id="a319b-129">方法 1</span><span class="sxs-lookup"><span data-stu-id="a319b-129">Option 1</span></span> | <span data-ttu-id="a319b-130">方法 2</span><span class="sxs-lookup"><span data-stu-id="a319b-130">Option 2</span></span> | <span data-ttu-id="a319b-131">オプション 3</span><span class="sxs-lookup"><span data-stu-id="a319b-131">Option 3</span></span> | <span data-ttu-id="a319b-132">オプション 4</span><span class="sxs-lookup"><span data-stu-id="a319b-132">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="a319b-133">Office 365 Enterprise E4 に含まれるすべての機能に対応</span><span class="sxs-lookup"><span data-stu-id="a319b-133">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="a319b-134">はい</span><span class="sxs-lookup"><span data-stu-id="a319b-134">Yes</span></span> | <span data-ttu-id="a319b-135">はい</span><span class="sxs-lookup"><span data-stu-id="a319b-135">Yes</span></span> | <span data-ttu-id="a319b-136">はい</span><span class="sxs-lookup"><span data-stu-id="a319b-136">Yes</span></span> | <span data-ttu-id="a319b-137">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-137">No</span></span> |
| <span data-ttu-id="a319b-138">Office 365 での電話番号の管理</span><span class="sxs-lookup"><span data-stu-id="a319b-138">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="a319b-139">はい</span><span class="sxs-lookup"><span data-stu-id="a319b-139">Yes</span></span> | <span data-ttu-id="a319b-140">はい</span><span class="sxs-lookup"><span data-stu-id="a319b-140">Yes</span></span> | <span data-ttu-id="a319b-141">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-141">No</span></span> | <span data-ttu-id="a319b-142">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-142">No</span></span> |
| <span data-ttu-id="a319b-143">オンプレミスと Office 365 の両方による電話番号の管理 (ハイブリッド展開)</span><span class="sxs-lookup"><span data-stu-id="a319b-143">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="a319b-144">はい</span><span class="sxs-lookup"><span data-stu-id="a319b-144">Yes</span></span> | <span data-ttu-id="a319b-145">はい</span><span class="sxs-lookup"><span data-stu-id="a319b-145">Yes</span></span> | <span data-ttu-id="a319b-146">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-146">No</span></span> | <span data-ttu-id="a319b-147">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-147">No</span></span> |
| <span data-ttu-id="a319b-148">PSTN 音声通話プランの追加オプション</span><span class="sxs-lookup"><span data-stu-id="a319b-148">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="a319b-149">はい</span><span class="sxs-lookup"><span data-stu-id="a319b-149">Yes</span></span> | <span data-ttu-id="a319b-150">はい</span><span class="sxs-lookup"><span data-stu-id="a319b-150">Yes</span></span> | <span data-ttu-id="a319b-151">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-151">No</span></span> | <span data-ttu-id="a319b-152">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-152">No</span></span> |
| <span data-ttu-id="a319b-153">PSTN 会議機能</span><span class="sxs-lookup"><span data-stu-id="a319b-153">PSTN Conferencing?</span></span> | <span data-ttu-id="a319b-154">はい</span><span class="sxs-lookup"><span data-stu-id="a319b-154">Yes</span></span> | <span data-ttu-id="a319b-155">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-155">No</span></span> | <span data-ttu-id="a319b-156">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-156">No</span></span> | <span data-ttu-id="a319b-157">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-157">No</span></span> |
| <span data-ttu-id="a319b-158">コラボレーション、分析、セキュリティの高度なツール</span><span class="sxs-lookup"><span data-stu-id="a319b-158">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="a319b-159">はい</span><span class="sxs-lookup"><span data-stu-id="a319b-159">Yes</span></span> | <span data-ttu-id="a319b-160">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-160">No</span></span> | <span data-ttu-id="a319b-161">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-161">No</span></span> | <span data-ttu-id="a319b-162">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-162">No</span></span> |
| <span data-ttu-id="a319b-163">対話型のレポート、ダッシュ ボード、データのビジュアル化</span><span class="sxs-lookup"><span data-stu-id="a319b-163">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="a319b-164">はい</span><span class="sxs-lookup"><span data-stu-id="a319b-164">Yes</span></span> | <span data-ttu-id="a319b-165">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-165">No</span></span> | <span data-ttu-id="a319b-166">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-166">No</span></span> | <span data-ttu-id="a319b-167">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-167">No</span></span> | 
| <span data-ttu-id="a319b-168">データ セキュリティとコンプライアンスを詳細に制御するための組み込みのプライバシー機能、透過性、洗練されたユーザー コントロール</span><span class="sxs-lookup"><span data-stu-id="a319b-168">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="a319b-169">はい</span><span class="sxs-lookup"><span data-stu-id="a319b-169">Yes</span></span> | <span data-ttu-id="a319b-170">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-170">No</span></span> | <span data-ttu-id="a319b-171">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-171">No</span></span> | <span data-ttu-id="a319b-172">いいえ</span><span class="sxs-lookup"><span data-stu-id="a319b-172">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="a319b-173">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="a319b-173">Transition customers to new product plans</span></span>

<span data-ttu-id="a319b-174">マイクロソフトは、絶えず新しい製品やサービスをパートナーに提供しています。</span><span class="sxs-lookup"><span data-stu-id="a319b-174">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="a319b-175">パートナーはこれに対応して、お客様を新しいサービスにアップグレードするか、お客様のサブスクリプションを廃止予定の SKU から移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a319b-175">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="a319b-176">廃止された SKU から新しい SKU にお客様を移行するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="a319b-176">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="a319b-177">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="a319b-177">Purchase the new subscription</span></span>
-   <span data-ttu-id="a319b-178">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="a319b-178">Reassign current user licenses</span></span>
-   <span data-ttu-id="a319b-179">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="a319b-179">Cancel the old subscription</span></span>

<span data-ttu-id="a319b-180">お客様の Office 365 Enterprise E4 サブスクリプションを上記の表のいずれかのオプションに移行するには、以下の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="a319b-180">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="a319b-181">手順 1 - 新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="a319b-181">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="a319b-182">**パートナー センター** メニューで **[顧客]** を選択し、移行する顧客を選択した後、**[サブスクリプションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a319b-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="a319b-183">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="a319b-183">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="a319b-184">お客様には、古いサブスクリプションと新しいサブスクリプション、古い Office 365 Enterprise E4 サブスクリプション、新しい ' ターゲット ' サブスクリプション (オプション 1-Office 365 Enterprise E5 など) の両方が含まれるようになります。</span><span class="sxs-lookup"><span data-stu-id="a319b-184">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="a319b-185">手順 2 - お客様のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="a319b-185">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="a319b-186">**パートナー センター** メニューで **[顧客]** を選択し、移行する顧客を選択した後、**[ユーザーとライセンス]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a319b-186">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="a319b-187">顧客の [ユーザーとライセンス] ページが開きます。</span><span class="sxs-lookup"><span data-stu-id="a319b-187">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="a319b-188">ユーザーライセンスを再割り当てするには、再割り当てするユーザーを選択し、[ **ライセンスの管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a319b-188">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="a319b-189">**[ライセンスの管理]** ページで、**Office 365 Enterprise E4** のライセンスのチェック ボックスをオフにし、お客様の移行先サブスクリプションの新しいサービス プランを選びます。</span><span class="sxs-lookup"><span data-stu-id="a319b-189">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="a319b-190">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a319b-190">Select **Submit**.</span></span> <span data-ttu-id="a319b-191">確認ページに新しいライセンスの割り当てが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="a319b-191">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="a319b-192">ライセンスをもう一度割り当てる必要がある他のお客様ユーザーについて、同じ手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="a319b-192">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="a319b-193">ユーザー ライセンスを新しいサービスに移行した後は、メニューの最上位レベルの [顧客] で、廃止されたサブスクリプションを安全に取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="a319b-193">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="a319b-194">手順 3 - 以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="a319b-194">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="a319b-195">**パートナー センター** メニューで、**[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a319b-195">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="a319b-196">移行するお客様を選び、取り消すサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="a319b-196">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="a319b-197">サブスクリプションの詳細ページで、サブスクリプションの状態を **[中断]** に設定します。</span><span class="sxs-lookup"><span data-stu-id="a319b-197">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="a319b-198">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a319b-198">Select **Submit**.</span></span>

<span data-ttu-id="a319b-199">以前のサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="a319b-199">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="a319b-200">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="a319b-200">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="a319b-201">お客様には、以前のサブスクリプションの追加コストは発生しません。</span><span class="sxs-lookup"><span data-stu-id="a319b-201">The customer incurs no additional costs for the old subscription.</span></span>



 



