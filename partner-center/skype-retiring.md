---
title: 一部の Skype for Business サブスクリプションを移行する
description: 有効期限が切れた Skype for Business Online プラン1サブスクリプションを持つ特定の顧客を新しい Office 365 バージョンに移行する方法とタイミングについて説明します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: c9ad5b1c0671ff1d27d25c6f92499b72d77e6c22
ms.sourcegitcommit: c40f826bb1143555bf3a1c2c806c34024f0f6019
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/02/2020
ms.locfileid: "89367626"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="4f0e5-103">Skype for Business Online プラン 1 サブスクリプションの新しい Office 365 バージョンへの移行</span><span class="sxs-lookup"><span data-stu-id="4f0e5-103">Migrate Skype for Business Online Plan 1 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="4f0e5-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="4f0e5-104">**Applies to**</span></span>

- <span data-ttu-id="4f0e5-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="4f0e5-105">Partner Center</span></span>

<span data-ttu-id="4f0e5-106">Skype for Business Online プラン1は、2018年8月1日をもって廃止される予定です。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-106">The Skype for Business Online Plan 1 will be retired, effective August 1, 2018.</span></span> <span data-ttu-id="4f0e5-107">この日付以降、新たに Skype for Business プラン 1 のサブスクリプションを購入することはできません。既存のサブスクリプションは、有効期限になると自動更新されず、更新のオプションは提供されません。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-107">After that date customers can no longer purchase new Skype for Business Plan 1 subscriptions, and existing subscriptions will not renew automatically when they expire and will not provide a renewal option.</span></span> <span data-ttu-id="4f0e5-108">サブスクリプションの詳細ページでは、Skype for Business Online プラン 1 のサブスクリプションの状態が、"自動更新: [日付]" から "有効期限: [date]" に変更されています。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-108">On the subscription's detail page, the Skype for Business Online Plan 1 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span>  

<span data-ttu-id="4f0e5-109">お客様への継続的なサービス提供のためには、有効期限が迫っている Skype for Business Online プラン 1 のサブスクリプションのお客様を、サポートされている以下の SKU オプションに移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-109">To ensure continuity for customers, you should transition customers with expiring Skype for Business Online Plan 1 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="4f0e5-110">顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

>[!NOTE]
><span data-ttu-id="4f0e5-111">Skype for Business Online プラン 1 の商用 SKU と行政機関用 SKUは、どちらも提供終了となります。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-111">Both Skype for Business Online Plan 1 commercial and government SKUs are retired.</span></span>

<span data-ttu-id="4f0e5-112">API (CREST またはパートナー センターのいずれか) を使用している場合は、サブスクリプションの終了日と auto renew = False プロパティを評価して、有効期限が迫っているサブスクリプションを検出できます。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-112">If you use the API (either CREST or Partner Center), find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="4f0e5-113">Skype for Business Online プラン 1 のサブスクリプションは、2018 年 9 月 1 日に auto renew = False に設定されます。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-113">The Skype for Business Online Plan 1 subscriptions will be set to auto renew=False on September 1, 2018.</span></span> <span data-ttu-id="4f0e5-114">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-114">You can move customers to a new plan at any time.</span></span> 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a><span data-ttu-id="4f0e5-115">Skype for Business Online プラン 1 の代替プラン</span><span class="sxs-lookup"><span data-stu-id="4f0e5-115">Skype for Business Online Plan 1 replacement plans</span></span>

<span data-ttu-id="4f0e5-116">新しいプランでは、お客様は Office 365 の新機能を活用できます。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-116">With the new plans, your customers take can advantage of newer features and functionality in Office 365.</span></span> <span data-ttu-id="4f0e5-117">料金の詳細は、パートナー センターの料金表またはプランのマトリックスに記載されています。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-117">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> 

- <span data-ttu-id="4f0e5-118">オプション1: Office 365 Enterprise F1</span><span class="sxs-lookup"><span data-stu-id="4f0e5-118">Option 1: Office 365 Enterprise F1</span></span>
- <span data-ttu-id="4f0e5-119">オプション 2: Microsoft 365 Enterprise F1</span><span class="sxs-lookup"><span data-stu-id="4f0e5-119">Option 2: Microsoft 365 Enterprise F1</span></span>
- <span data-ttu-id="4f0e5-120">オプション 3: その他の Office 365 プラン</span><span class="sxs-lookup"><span data-stu-id="4f0e5-120">Option 3: Other Office 365 plans</span></span>

|<span data-ttu-id="4f0e5-121">**機能**</span><span class="sxs-lookup"><span data-stu-id="4f0e5-121">**Feature**</span></span>    |<span data-ttu-id="4f0e5-122">**方法 1**</span><span class="sxs-lookup"><span data-stu-id="4f0e5-122">**Option 1**</span></span>   |<span data-ttu-id="4f0e5-123">**方法 2**</span><span class="sxs-lookup"><span data-stu-id="4f0e5-123">**Option 2**</span></span>   |<span data-ttu-id="4f0e5-124">**オプション3**</span><span class="sxs-lookup"><span data-stu-id="4f0e5-124">**Option 3**</span></span>   |
|:-----------------|:-----------------|:-------------|:------------|
|<span data-ttu-id="4f0e5-125">Skype for Business Online プラン 1 に含まれるすべての機能の利用</span><span class="sxs-lookup"><span data-stu-id="4f0e5-125">Get all the features included in Skype for Business Online Plan 1</span></span>|<span data-ttu-id="4f0e5-126">はい</span><span class="sxs-lookup"><span data-stu-id="4f0e5-126">Yes</span></span>   |<span data-ttu-id="4f0e5-127">はい</span><span class="sxs-lookup"><span data-stu-id="4f0e5-127">Yes</span></span>   |<span data-ttu-id="4f0e5-128">はい</span><span class="sxs-lookup"><span data-stu-id="4f0e5-128">Yes</span></span>   |
|<span data-ttu-id="4f0e5-129">IM とプレゼンス</span><span class="sxs-lookup"><span data-stu-id="4f0e5-129">IM and presence</span></span> |<span data-ttu-id="4f0e5-130">はい</span><span class="sxs-lookup"><span data-stu-id="4f0e5-130">Yes</span></span>   |<span data-ttu-id="4f0e5-131">はい</span><span class="sxs-lookup"><span data-stu-id="4f0e5-131">Yes</span></span>   |<span data-ttu-id="4f0e5-132">はい</span><span class="sxs-lookup"><span data-stu-id="4f0e5-132">Yes</span></span>   |
|<span data-ttu-id="4f0e5-133">IP を経由したピアツーピア オーディオとビデオ</span><span class="sxs-lookup"><span data-stu-id="4f0e5-133">Peer-to-peer Audio and Video over IP</span></span>|<span data-ttu-id="4f0e5-134">はい</span><span class="sxs-lookup"><span data-stu-id="4f0e5-134">Yes</span></span>   |<span data-ttu-id="4f0e5-135">はい</span><span class="sxs-lookup"><span data-stu-id="4f0e5-135">Yes</span></span>   |<span data-ttu-id="4f0e5-136">はい</span><span class="sxs-lookup"><span data-stu-id="4f0e5-136">Yes</span></span>   
|<span data-ttu-id="4f0e5-137">認証ユーザーとして会議に参加</span><span class="sxs-lookup"><span data-stu-id="4f0e5-137">Join meetings as an authenticated user</span></span>| <span data-ttu-id="4f0e5-138">はい</span><span class="sxs-lookup"><span data-stu-id="4f0e5-138">Yes</span></span>   |<span data-ttu-id="4f0e5-139">はい</span><span class="sxs-lookup"><span data-stu-id="4f0e5-139">Yes</span></span>   |<span data-ttu-id="4f0e5-140">はい</span><span class="sxs-lookup"><span data-stu-id="4f0e5-140">Yes</span></span>   |

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="4f0e5-141">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="4f0e5-141">Transition customers to new product plans</span></span>

<span data-ttu-id="4f0e5-142">マイクロソフトは、絶えず新しい製品やサービスをパートナーに提供しています。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-142">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="4f0e5-143">パートナーはこれに対応して、お客様を新しいサービスにアップグレードするか、お客様のサブスクリプションを廃止予定の SKU から移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-143">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="4f0e5-144">廃止された SKU から新しい SKU にお客様を移行するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-144">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

- <span data-ttu-id="4f0e5-145">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="4f0e5-145">Purchase the new subscription</span></span>
- <span data-ttu-id="4f0e5-146">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="4f0e5-146">Reassign current user licenses</span></span>
- <span data-ttu-id="4f0e5-147">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="4f0e5-147">Cancel old subscription</span></span>

### <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="4f0e5-148">新しいプランにお客様を移行する</span><span class="sxs-lookup"><span data-stu-id="4f0e5-148">Migrate your customers to new plans</span></span>

1. <span data-ttu-id="4f0e5-149">新しいサブスクリプションを購入するには、**パートナー センター メニュー**で **[顧客]** を選び、移行する顧客を選んでから、**[サブスクリプションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-149">To purchase the new subscription, from the **Partner Center menu**, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="4f0e5-150">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-150">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="4f0e5-151">お客様には、古い Skype for Business Online プラン1サブスクリプションと、オプション 1-Office 365 Enterprise F1 などの新しい "ターゲット" サブスクリプションの両方が含まれるようになりました。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-151">Your customer should now have both old and new subscriptions, the old Skype for Business Online Plan 1  subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

3. <span data-ttu-id="4f0e5-152">顧客のユーザーのライセンスをもう一度割り当てるには、**パートナー センター** メニューで **[顧客]** を選び、移行する顧客を選んでから **[ユーザーとライセンス]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-152">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="4f0e5-153">顧客の [ユーザーとライセンス] ページが開きます。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-153">The customer's Users and Licenses page opens.</span></span>

4. <span data-ttu-id="4f0e5-154">ユーザー ライセンスをもう一度割り当てるには、割り当てるユーザーを選んで **[ライセンスの管理]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-154">To reassign user license, select the user to reassign and then select **Manage licenses.**</span></span>

5. <span data-ttu-id="4f0e5-155">**[ライセンスの管理]** ページで、Skype for Business Online プラン 1 のライセンスのチェック ボックスをオフにし、お客様の移行先サブスクリプションの新しいサービス プランを選びます。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-155">On the **Manage licenses** page, clear the Skype for Business Online Plan 1 license check box and select a new service plan for the subscription the customer is moving to.</span></span>

6. <span data-ttu-id="4f0e5-156">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-156">Select **Submit**.</span></span> <span data-ttu-id="4f0e5-157">確認ページに新しいライセンスの割り当てが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-157">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="4f0e5-158">ライセンスの割り当てが必要な他のユーザーにも同じプロセスを続行します。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-158">Continue this same process for other users who need license assignments.</span></span>

<span data-ttu-id="4f0e5-159">ユーザー ライセンスを新しいサービスに移行した後は、顧客レベルで廃止されたサブスクリプションを安全に取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-159">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

7. <span data-ttu-id="4f0e5-160">**パートナー センター** メニューで、**[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-160">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="4f0e5-161">サブスクリプションをキャンセルする顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-161">Select the customer whose subscription you are canceling.</span></span>

8. <span data-ttu-id="4f0e5-162">サブスクリプションの詳細ページで、サブスクリプションを **[中断]** に設定します。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-162">In the subscription detail page, set the subscription to **Suspended**.</span></span>

9. <span data-ttu-id="4f0e5-163">[送信] を選択し **ます。**</span><span class="sxs-lookup"><span data-stu-id="4f0e5-163">Select **Submit.**</span></span>

<span data-ttu-id="4f0e5-164">以前のサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-164">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="4f0e5-165">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-165">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="4f0e5-166">お客様には、以前のサブスクリプションの追加コストは発生しません。</span><span class="sxs-lookup"><span data-stu-id="4f0e5-166">The customer incurs no additional costs for the old subscription.</span></span>

