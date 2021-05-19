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
ms.openlocfilehash: f738ddace805838cdf202c23cca8535c11cbdf54
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151561"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="299d9-104">Office 365 E4 サブスクリプションの Office 365 の新しいバージョンへの移行</span><span class="sxs-lookup"><span data-stu-id="299d9-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="299d9-105">**適切なロール**: 全体管理者 |ユーザー管理の管理者 |管理エージェント |営業担当者</span><span class="sxs-lookup"><span data-stu-id="299d9-105">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="299d9-106">Office 365 Enterprise E4 プランは、2017 年 4 月 7 日に廃止されました。</span><span class="sxs-lookup"><span data-stu-id="299d9-106">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="299d9-107">これ以降、新しい Office 365 E4 サブスクリプションを購入することはできません。また、既存の E4 サブスクリプションは期限切れになっても、自動更新されません。</span><span class="sxs-lookup"><span data-stu-id="299d9-107">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="299d9-108">E4 サブスクリプションは終了した時点で取り消されます。</span><span class="sxs-lookup"><span data-stu-id="299d9-108">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="299d9-109">お客様への継続的なサービス提供を保証するには、有効期限が迫っている E4 サブスクリプションのお客様を、サポートされている以下の SKU オプションに移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="299d9-109">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="299d9-110">顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="299d9-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="299d9-111">Office 365 Enterprise E4 は、商用 SKU と政府機関用 SKU の両方が廃止されました。</span><span class="sxs-lookup"><span data-stu-id="299d9-111">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="299d9-112">サブスクリプションの詳細ページでは、E4 サブスクリプションの状態が、"自動更新: [日付]" から "有効期限: [date]" に変更されています。</span><span class="sxs-lookup"><span data-stu-id="299d9-112">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="299d9-113">API (CREST またはパートナー センターのいずれか) を使用している場合は、サブスクリプションの終了日と auto renew = False プロパティを評価して、有効期限が迫っているサブスクリプションを検出できます。</span><span class="sxs-lookup"><span data-stu-id="299d9-113">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="299d9-114">E4 サブスクリプションは、2017 年 4 月 7 日に ”auto renew=False” に設定されています。</span><span class="sxs-lookup"><span data-stu-id="299d9-114">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="299d9-115">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="299d9-115">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="299d9-116">Office 365 Enterprise E4 エディションの置換の計画</span><span class="sxs-lookup"><span data-stu-id="299d9-116">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="299d9-117">E4 と同じ機能を維持するか、お客様に Office 365 と Skype for Business Online の新しい機能を提供するかを選択できます。</span><span class="sxs-lookup"><span data-stu-id="299d9-117">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="299d9-118">料金の詳細は、パートナー センターの料金表またはプランのマトリックスに記載されています。</span><span class="sxs-lookup"><span data-stu-id="299d9-118">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="299d9-119">Secure Product Enterprise E3 または Secure Productive Enterprise E5 は、それぞれ Office 365 Enterprise E3 または Office 365 Enterprise E5 の次のオプションに置き換えることができます。</span><span class="sxs-lookup"><span data-stu-id="299d9-119">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="299d9-120">オプション1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="299d9-120">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="299d9-121">オプション2: Office 365 Enterprise E3 + Skype for Business クラウド PBX</span><span class="sxs-lookup"><span data-stu-id="299d9-121">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="299d9-122">オプション3: Office 365 Enterprise E3 + Skype for Business Plus CAL (料金と機能は E4 相当)</span><span class="sxs-lookup"><span data-stu-id="299d9-122">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="299d9-123">オプション4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="299d9-123">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="299d9-124">機能</span><span class="sxs-lookup"><span data-stu-id="299d9-124">Feature</span></span> | <span data-ttu-id="299d9-125">方法 1</span><span class="sxs-lookup"><span data-stu-id="299d9-125">Option 1</span></span> | <span data-ttu-id="299d9-126">方法 2</span><span class="sxs-lookup"><span data-stu-id="299d9-126">Option 2</span></span> | <span data-ttu-id="299d9-127">オプション 3</span><span class="sxs-lookup"><span data-stu-id="299d9-127">Option 3</span></span> | <span data-ttu-id="299d9-128">オプション 4</span><span class="sxs-lookup"><span data-stu-id="299d9-128">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="299d9-129">Office 365 Enterprise E4 に含まれるすべての機能に対応</span><span class="sxs-lookup"><span data-stu-id="299d9-129">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="299d9-130">Yes</span><span class="sxs-lookup"><span data-stu-id="299d9-130">Yes</span></span> | <span data-ttu-id="299d9-131">Yes</span><span class="sxs-lookup"><span data-stu-id="299d9-131">Yes</span></span> | <span data-ttu-id="299d9-132">はい</span><span class="sxs-lookup"><span data-stu-id="299d9-132">Yes</span></span> | <span data-ttu-id="299d9-133">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-133">No</span></span> |
| <span data-ttu-id="299d9-134">Office 365 での電話番号の管理</span><span class="sxs-lookup"><span data-stu-id="299d9-134">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="299d9-135">Yes</span><span class="sxs-lookup"><span data-stu-id="299d9-135">Yes</span></span> | <span data-ttu-id="299d9-136">はい</span><span class="sxs-lookup"><span data-stu-id="299d9-136">Yes</span></span> | <span data-ttu-id="299d9-137">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-137">No</span></span> | <span data-ttu-id="299d9-138">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-138">No</span></span> |
| <span data-ttu-id="299d9-139">オンプレミスと Office 365 の両方による電話番号の管理 (ハイブリッド展開)</span><span class="sxs-lookup"><span data-stu-id="299d9-139">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="299d9-140">Yes</span><span class="sxs-lookup"><span data-stu-id="299d9-140">Yes</span></span> | <span data-ttu-id="299d9-141">はい</span><span class="sxs-lookup"><span data-stu-id="299d9-141">Yes</span></span> | <span data-ttu-id="299d9-142">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-142">No</span></span> | <span data-ttu-id="299d9-143">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-143">No</span></span> |
| <span data-ttu-id="299d9-144">PSTN 音声通話プランの追加オプション</span><span class="sxs-lookup"><span data-stu-id="299d9-144">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="299d9-145">Yes</span><span class="sxs-lookup"><span data-stu-id="299d9-145">Yes</span></span> | <span data-ttu-id="299d9-146">はい</span><span class="sxs-lookup"><span data-stu-id="299d9-146">Yes</span></span> | <span data-ttu-id="299d9-147">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-147">No</span></span> | <span data-ttu-id="299d9-148">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-148">No</span></span> |
| <span data-ttu-id="299d9-149">PSTN 会議機能</span><span class="sxs-lookup"><span data-stu-id="299d9-149">PSTN Conferencing?</span></span> | <span data-ttu-id="299d9-150">はい</span><span class="sxs-lookup"><span data-stu-id="299d9-150">Yes</span></span> | <span data-ttu-id="299d9-151">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-151">No</span></span> | <span data-ttu-id="299d9-152">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-152">No</span></span> | <span data-ttu-id="299d9-153">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-153">No</span></span> |
| <span data-ttu-id="299d9-154">コラボレーション、分析、セキュリティの高度なツール</span><span class="sxs-lookup"><span data-stu-id="299d9-154">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="299d9-155">はい</span><span class="sxs-lookup"><span data-stu-id="299d9-155">Yes</span></span> | <span data-ttu-id="299d9-156">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-156">No</span></span> | <span data-ttu-id="299d9-157">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-157">No</span></span> | <span data-ttu-id="299d9-158">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-158">No</span></span> |
| <span data-ttu-id="299d9-159">対話型のレポート、ダッシュ ボード、データのビジュアル化</span><span class="sxs-lookup"><span data-stu-id="299d9-159">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="299d9-160">はい</span><span class="sxs-lookup"><span data-stu-id="299d9-160">Yes</span></span> | <span data-ttu-id="299d9-161">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-161">No</span></span> | <span data-ttu-id="299d9-162">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-162">No</span></span> | <span data-ttu-id="299d9-163">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-163">No</span></span> | 
| <span data-ttu-id="299d9-164">データ セキュリティとコンプライアンスを詳細に制御するための組み込みのプライバシー機能、透過性、洗練されたユーザー コントロール</span><span class="sxs-lookup"><span data-stu-id="299d9-164">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="299d9-165">はい</span><span class="sxs-lookup"><span data-stu-id="299d9-165">Yes</span></span> | <span data-ttu-id="299d9-166">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-166">No</span></span> | <span data-ttu-id="299d9-167">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-167">No</span></span> | <span data-ttu-id="299d9-168">いいえ</span><span class="sxs-lookup"><span data-stu-id="299d9-168">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="299d9-169">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="299d9-169">Transition customers to new product plans</span></span>

<span data-ttu-id="299d9-170">マイクロソフトは、絶えず新しい製品やサービスをパートナーに提供しています。</span><span class="sxs-lookup"><span data-stu-id="299d9-170">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="299d9-171">パートナーはこれに対応して、お客様を新しいサービスにアップグレードするか、お客様のサブスクリプションを廃止予定の SKU から移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="299d9-171">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="299d9-172">廃止された SKU から新しい SKU にお客様を移行するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="299d9-172">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="299d9-173">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="299d9-173">Purchase the new subscription</span></span>
-   <span data-ttu-id="299d9-174">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="299d9-174">Reassign current user licenses</span></span>
-   <span data-ttu-id="299d9-175">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="299d9-175">Cancel the old subscription</span></span>

<span data-ttu-id="299d9-176">お客様の Office 365 Enterprise E4 サブスクリプションを上記の表のいずれかのオプションに移行するには、以下の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="299d9-176">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="299d9-177">手順 1 - 新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="299d9-177">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="299d9-178">**パートナー センター** メニューで **[顧客]** を選択し、移行する顧客を選択した後、**[サブスクリプションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="299d9-178">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="299d9-179">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="299d9-179">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="299d9-180">お客様には、古いサブスクリプションと新しいサブスクリプション、古い Office 365 Enterprise E4 サブスクリプション、新しい ' ターゲット ' サブスクリプション (オプション 1-Office 365 Enterprise E5 など) の両方が含まれるようになります。</span><span class="sxs-lookup"><span data-stu-id="299d9-180">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="299d9-181">手順 2 - お客様のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="299d9-181">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="299d9-182">**パートナー センター** メニューで **[顧客]** を選択し、移行する顧客を選択した後、**[ユーザーとライセンス]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="299d9-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="299d9-183">顧客の [ユーザーとライセンス] ページが開きます。</span><span class="sxs-lookup"><span data-stu-id="299d9-183">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="299d9-184">ユーザーライセンスを再割り当てするには、再割り当てするユーザーを選択し、[ **ライセンスの管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="299d9-184">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="299d9-185">**[ライセンスの管理]** ページで、**Office 365 Enterprise E4** のライセンスのチェック ボックスをオフにし、お客様の移行先サブスクリプションの新しいサービス プランを選びます。</span><span class="sxs-lookup"><span data-stu-id="299d9-185">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="299d9-186">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="299d9-186">Select **Submit**.</span></span> <span data-ttu-id="299d9-187">確認ページに新しいライセンスの割り当てが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="299d9-187">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="299d9-188">ライセンスをもう一度割り当てる必要がある他のお客様ユーザーについて、同じ手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="299d9-188">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="299d9-189">ユーザー ライセンスを新しいサービスに移行した後は、メニューの最上位レベルの [顧客] で、廃止されたサブスクリプションを安全に取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="299d9-189">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="299d9-190">手順 3 - 以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="299d9-190">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="299d9-191">**パートナー センター** メニューで、**[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="299d9-191">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="299d9-192">移行するお客様を選び、取り消すサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="299d9-192">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="299d9-193">サブスクリプションの詳細ページで、サブスクリプションの状態を **[中断]** に設定します。</span><span class="sxs-lookup"><span data-stu-id="299d9-193">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="299d9-194">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="299d9-194">Select **Submit**.</span></span>

<span data-ttu-id="299d9-195">以前のサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="299d9-195">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="299d9-196">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="299d9-196">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="299d9-197">お客様には、以前のサブスクリプションの追加コストは発生しません。</span><span class="sxs-lookup"><span data-stu-id="299d9-197">The customer incurs no additional costs for the old subscription.</span></span>



 



