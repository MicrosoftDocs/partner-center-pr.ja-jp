---
title: Office 365 E4 サブスクリプションの Office 365 の新しいバージョンへの移行 | パートナー センター
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 エディションは、2017 年 4 月 7 日に廃止されました。 Office 365 の新しいバージョンに、お客様のサブスクリプションを移行する方法について説明します。
author: jasonwhowell
ms.author: jasonh
ms.localizationpriority: medium
ms.openlocfilehash: ead92169ce7b3f1c2e697b6d4e983603c17d39fc
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390881"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="9b232-104">Office 365 E4 サブスクリプションの Office 365 の新しいバージョンへの移行</span><span class="sxs-lookup"><span data-stu-id="9b232-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="9b232-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="9b232-105">**Applies to**</span></span>

-  <span data-ttu-id="9b232-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="9b232-106">Partner Center</span></span>

<span data-ttu-id="9b232-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="9b232-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="9b232-108">全体管理者</span><span class="sxs-lookup"><span data-stu-id="9b232-108">Global admin</span></span>
-   <span data-ttu-id="9b232-109">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="9b232-109">User admin</span></span>
-   <span data-ttu-id="9b232-110">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="9b232-110">Admin agent</span></span>
-   <span data-ttu-id="9b232-111">販売代理店</span><span class="sxs-lookup"><span data-stu-id="9b232-111">Sales agent</span></span>

<span data-ttu-id="9b232-112">Office 365 Enterprise E4 プランは、2017 年 4 月 7 日に廃止されました。</span><span class="sxs-lookup"><span data-stu-id="9b232-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="9b232-113">これ以降、新しい Office 365 E4 サブスクリプションを購入することはできません。また、既存の E4 サブスクリプションは期限切れになっても、自動更新されません。</span><span class="sxs-lookup"><span data-stu-id="9b232-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="9b232-114">E4 サブスクリプションは終了した時点で取り消されます。</span><span class="sxs-lookup"><span data-stu-id="9b232-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="9b232-115">お客様への継続的なサービス提供を保証するには、有効期限が迫っている E4 サブスクリプションのお客様を、サポートされている以下の SKU オプションに移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b232-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="9b232-116">顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="9b232-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="9b232-117">Office 365 Enterprise E4 は、商用 SKU と政府機関用 SKU の両方が廃止されました。</span><span class="sxs-lookup"><span data-stu-id="9b232-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="9b232-118">サブスクリプションの詳細ページでは、E4 サブスクリプションの状態が、"自動更新: [日付]" から "有効期限: [date]" に変更されています。</span><span class="sxs-lookup"><span data-stu-id="9b232-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="9b232-119">API (CREST またはパートナー センターのいずれか) を使用している場合は、サブスクリプションの終了日と auto renew = False プロパティを評価して、有効期限が迫っているサブスクリプションを検出できます。</span><span class="sxs-lookup"><span data-stu-id="9b232-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="9b232-120">E4 サブスクリプションは、2017 年 4 月 7 日に ”auto renew=False” に設定されています。</span><span class="sxs-lookup"><span data-stu-id="9b232-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="9b232-121">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="9b232-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="9b232-122">Office 365 Enterprise E4 エディションの置換の計画</span><span class="sxs-lookup"><span data-stu-id="9b232-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="9b232-123">E4 と同じ機能を維持するか、お客様に Office 365 と Skype for Business Online の新しい機能を提供するかを選択できます。</span><span class="sxs-lookup"><span data-stu-id="9b232-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="9b232-124">料金の詳細は、パートナー センターの料金表またはプランのマトリックスに記載されています。</span><span class="sxs-lookup"><span data-stu-id="9b232-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="9b232-125">Secure Product Enterprise E3 または Secure Productive Enterprise E5 は、それぞれ Office 365 Enterprise E3 または Office 365 Enterprise E5 の次のオプションに置き換えることができます。</span><span class="sxs-lookup"><span data-stu-id="9b232-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="9b232-126">オプション1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="9b232-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="9b232-127">オプション2: Office 365 Enterprise E3 + Skype for Business クラウド PBX</span><span class="sxs-lookup"><span data-stu-id="9b232-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="9b232-128">オプション3: Office 365 Enterprise E3 + Skype for Business Plus CAL (料金と機能は E4 相当)</span><span class="sxs-lookup"><span data-stu-id="9b232-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="9b232-129">オプション4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="9b232-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="9b232-130">機能</span><span class="sxs-lookup"><span data-stu-id="9b232-130">Feature</span></span> | <span data-ttu-id="9b232-131">オプション 1</span><span class="sxs-lookup"><span data-stu-id="9b232-131">Option 1</span></span> | <span data-ttu-id="9b232-132">オプション 2</span><span class="sxs-lookup"><span data-stu-id="9b232-132">Option 2</span></span> | <span data-ttu-id="9b232-133">オプション 3</span><span class="sxs-lookup"><span data-stu-id="9b232-133">Option 3</span></span> | <span data-ttu-id="9b232-134">オプション 4</span><span class="sxs-lookup"><span data-stu-id="9b232-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="9b232-135">Office 365 Enterprise E4 に含まれるすべての機能に対応</span><span class="sxs-lookup"><span data-stu-id="9b232-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="9b232-136">はい</span><span class="sxs-lookup"><span data-stu-id="9b232-136">Yes</span></span> | <span data-ttu-id="9b232-137">はい</span><span class="sxs-lookup"><span data-stu-id="9b232-137">Yes</span></span> | <span data-ttu-id="9b232-138">はい</span><span class="sxs-lookup"><span data-stu-id="9b232-138">Yes</span></span> | <span data-ttu-id="9b232-139">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-139">No</span></span> |
| <span data-ttu-id="9b232-140">Office 365 での電話番号の管理</span><span class="sxs-lookup"><span data-stu-id="9b232-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="9b232-141">はい</span><span class="sxs-lookup"><span data-stu-id="9b232-141">Yes</span></span> | <span data-ttu-id="9b232-142">はい</span><span class="sxs-lookup"><span data-stu-id="9b232-142">Yes</span></span> | <span data-ttu-id="9b232-143">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-143">No</span></span> | <span data-ttu-id="9b232-144">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-144">No</span></span> |
| <span data-ttu-id="9b232-145">オンプレミスと Office 365 の両方による電話番号の管理 (ハイブリッド展開)</span><span class="sxs-lookup"><span data-stu-id="9b232-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="9b232-146">はい</span><span class="sxs-lookup"><span data-stu-id="9b232-146">Yes</span></span> | <span data-ttu-id="9b232-147">はい</span><span class="sxs-lookup"><span data-stu-id="9b232-147">Yes</span></span> | <span data-ttu-id="9b232-148">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-148">No</span></span> | <span data-ttu-id="9b232-149">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-149">No</span></span> |
| <span data-ttu-id="9b232-150">PSTN 音声通話プランの追加オプション</span><span class="sxs-lookup"><span data-stu-id="9b232-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="9b232-151">はい</span><span class="sxs-lookup"><span data-stu-id="9b232-151">Yes</span></span> | <span data-ttu-id="9b232-152">はい</span><span class="sxs-lookup"><span data-stu-id="9b232-152">Yes</span></span> | <span data-ttu-id="9b232-153">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-153">No</span></span> | <span data-ttu-id="9b232-154">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-154">No</span></span> |
| <span data-ttu-id="9b232-155">PSTN 会議機能</span><span class="sxs-lookup"><span data-stu-id="9b232-155">PSTN Conferencing?</span></span> | <span data-ttu-id="9b232-156">はい</span><span class="sxs-lookup"><span data-stu-id="9b232-156">Yes</span></span> | <span data-ttu-id="9b232-157">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-157">No</span></span> | <span data-ttu-id="9b232-158">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-158">No</span></span> | <span data-ttu-id="9b232-159">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-159">No</span></span> |
| <span data-ttu-id="9b232-160">コラボレーション、分析、セキュリティの高度なツール</span><span class="sxs-lookup"><span data-stu-id="9b232-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="9b232-161">はい</span><span class="sxs-lookup"><span data-stu-id="9b232-161">Yes</span></span> | <span data-ttu-id="9b232-162">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-162">No</span></span> | <span data-ttu-id="9b232-163">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-163">No</span></span> | <span data-ttu-id="9b232-164">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-164">No</span></span> |
| <span data-ttu-id="9b232-165">対話型のレポート、ダッシュ ボード、データのビジュアル化</span><span class="sxs-lookup"><span data-stu-id="9b232-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="9b232-166">はい</span><span class="sxs-lookup"><span data-stu-id="9b232-166">Yes</span></span> | <span data-ttu-id="9b232-167">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-167">No</span></span> | <span data-ttu-id="9b232-168">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-168">No</span></span> | <span data-ttu-id="9b232-169">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-169">No</span></span> | 
| <span data-ttu-id="9b232-170">データ セキュリティとコンプライアンスを詳細に制御するための組み込みのプライバシー機能、透過性、洗練されたユーザー コントロール</span><span class="sxs-lookup"><span data-stu-id="9b232-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="9b232-171">はい</span><span class="sxs-lookup"><span data-stu-id="9b232-171">Yes</span></span> | <span data-ttu-id="9b232-172">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-172">No</span></span> | <span data-ttu-id="9b232-173">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-173">No</span></span> | <span data-ttu-id="9b232-174">いいえ</span><span class="sxs-lookup"><span data-stu-id="9b232-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="9b232-175">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="9b232-175">Transition customers to new product plans</span></span>

<span data-ttu-id="9b232-176">マイクロソフトは、絶えず新しい製品やサービスをパートナーに提供しています。</span><span class="sxs-lookup"><span data-stu-id="9b232-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="9b232-177">パートナーはこれに対応して、お客様を新しいサービスにアップグレードするか、お客様のサブスクリプションを廃止予定の SKU から移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9b232-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="9b232-178">廃止された SKU から新しい SKU にお客様を移行するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="9b232-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="9b232-179">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="9b232-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="9b232-180">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="9b232-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="9b232-181">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="9b232-181">Cancel the old subscription</span></span>

<span data-ttu-id="9b232-182">お客様の Office 365 Enterprise E4 サブスクリプションを上記の表のいずれかのオプションに移行するには、以下の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="9b232-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="9b232-183">手順 1 - 新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="9b232-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="9b232-184">**パートナー センター** メニューで **[顧客]** を選択し、移行する顧客を選択した後、 **[サブスクリプションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9b232-184">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="9b232-185">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、 **[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="9b232-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="9b232-186">お客様には、古いサブスクリプションと新しいサブスクリプション、古い Office 365 Enterprise E4 サブスクリプション、新しい ' ターゲット ' サブスクリプション (オプション 1-Office 365 Enterprise E5 など) の両方が含まれるようになります。</span><span class="sxs-lookup"><span data-stu-id="9b232-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="9b232-187">手順 2 - お客様のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="9b232-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="9b232-188">**パートナー センター** メニューで **[顧客]** を選択し、移行する顧客を選択した後、 **[ユーザーとライセンス]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9b232-188">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="9b232-189">顧客の [ユーザーとライセンス] ページが開きます。</span><span class="sxs-lookup"><span data-stu-id="9b232-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="9b232-190">ユーザー ライセンスをもう一度割り当てるには、割り当てるユーザーを選んで **[ライセンスの管理]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="9b232-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="9b232-191">**[ライセンスの管理]** ページで、**Office 365 Enterprise E4** のライセンスのチェック ボックスをオフにし、お客様の移行先サブスクリプションの新しいサービス プランを選びます。</span><span class="sxs-lookup"><span data-stu-id="9b232-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="9b232-192">**[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9b232-192">Select **Submit**.</span></span> <span data-ttu-id="9b232-193">確認ページに新しいライセンスの割り当てが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="9b232-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="9b232-194">ライセンスをもう一度割り当てる必要がある他のお客様ユーザーについて、同じ手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="9b232-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="9b232-195">ユーザー ライセンスを新しいサービスに移行した後は、メニューの最上位レベルの [顧客] で、廃止されたサブスクリプションを安全に取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="9b232-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="9b232-196">手順 3 - 以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="9b232-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="9b232-197">**パートナー センター** メニューで、 **[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9b232-197">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="9b232-198">移行するお客様を選び、取り消すサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="9b232-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="9b232-199">サブスクリプションの詳細ページで、サブスクリプションの状態を **[中断]** に設定します。</span><span class="sxs-lookup"><span data-stu-id="9b232-199">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="9b232-200">**[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9b232-200">Select **Submit**.</span></span>

<span data-ttu-id="9b232-201">以前のサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="9b232-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="9b232-202">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="9b232-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="9b232-203">お客様には、以前のサブスクリプションの追加コストは発生しません。</span><span class="sxs-lookup"><span data-stu-id="9b232-203">The customer incurs no additional costs for the old subscription.</span></span>



 



