---
title: 一部の Skype for Business サブスクリプションを移行する
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 有効期限が切れた Skype for Business Online プラン1サブスクリプションを持つ特定の顧客を新しい Office 365 バージョンに移行する方法とタイミングについて説明します。
author: BrentSerbus
ms.author: brserbus
keywords: Skype for Business の計画、Skype の提供終了、Office 365
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4202e146a470e2231ac33df9878be91e19fcddf3
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949614"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="94348-104">Skype for Business Online プラン 1 サブスクリプションの新しい Office 365 バージョンへの移行</span><span class="sxs-lookup"><span data-stu-id="94348-104">Migrate Skype for Business Online Plan 1 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="94348-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="94348-105">**Applies to**</span></span>

- <span data-ttu-id="94348-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="94348-106">Partner Center</span></span>

<span data-ttu-id="94348-107">Skype for Business Online プラン1は、2018年8月1日をもって廃止される予定です。</span><span class="sxs-lookup"><span data-stu-id="94348-107">The Skype for Business Online Plan 1 will be retired, effective August 1, 2018.</span></span> <span data-ttu-id="94348-108">この日付以降、新たに Skype for Business プラン 1 のサブスクリプションを購入することはできません。既存のサブスクリプションは、有効期限になると自動更新されず、更新のオプションは提供されません。</span><span class="sxs-lookup"><span data-stu-id="94348-108">After that date customers can no longer purchase new Skype for Business Plan 1 subscriptions, and existing subscriptions will not renew automatically when they expire and will not provide a renewal option.</span></span> <span data-ttu-id="94348-109">サブスクリプションの詳細ページでは、Skype for Business Online プラン 1 のサブスクリプションの状態が、"自動更新: [日付]" から "有効期限: [date]" に変更されています。</span><span class="sxs-lookup"><span data-stu-id="94348-109">On the subscription's detail page, the Skype for Business Online Plan 1 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span>  

<span data-ttu-id="94348-110">お客様への継続的なサービス提供のためには、有効期限が迫っている Skype for Business Online プラン 1 のサブスクリプションのお客様を、サポートされている以下の SKU オプションに移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="94348-110">To ensure continuity for customers, you should transition customers with expiring Skype for Business Online Plan 1 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="94348-111">顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="94348-111">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

>[!NOTE]
><span data-ttu-id="94348-112">Skype for Business Online プラン 1 の商用 SKU と行政機関用 SKUは、どちらも提供終了となります。</span><span class="sxs-lookup"><span data-stu-id="94348-112">Both Skype for Business Online Plan 1 commercial and government SKUs are retired.</span></span>

<span data-ttu-id="94348-113">API (CREST またはパートナー センターのいずれか) を使用している場合は、サブスクリプションの終了日と auto renew = False プロパティを評価して、有効期限が迫っているサブスクリプションを検出できます。</span><span class="sxs-lookup"><span data-stu-id="94348-113">If you use the API (either CREST or Partner Center), find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="94348-114">Skype for Business Online プラン 1 のサブスクリプションは、2018 年 9 月 1 日に auto renew = False に設定されます。</span><span class="sxs-lookup"><span data-stu-id="94348-114">The Skype for Business Online Plan 1 subscriptions will be set to auto renew=False on September 1, 2018.</span></span> <span data-ttu-id="94348-115">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="94348-115">You can move customers to a new plan at any time.</span></span> 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a><span data-ttu-id="94348-116">Skype for Business Online プラン 1 の代替プラン</span><span class="sxs-lookup"><span data-stu-id="94348-116">Skype for Business Online Plan 1 replacement plans</span></span>

<span data-ttu-id="94348-117">新しいプランでは、お客様は Office 365 の新機能を活用できます。</span><span class="sxs-lookup"><span data-stu-id="94348-117">With the new plans, your customers take can advantage of newer features and functionality in Office 365.</span></span> <span data-ttu-id="94348-118">料金の詳細は、パートナー センターの料金表またはプランのマトリックスに記載されています。</span><span class="sxs-lookup"><span data-stu-id="94348-118">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> 

- <span data-ttu-id="94348-119">オプション1: Office 365 Enterprise F1</span><span class="sxs-lookup"><span data-stu-id="94348-119">Option 1: Office 365 Enterprise F1</span></span>
- <span data-ttu-id="94348-120">オプション 2: Microsoft 365 Enterprise F1</span><span class="sxs-lookup"><span data-stu-id="94348-120">Option 2: Microsoft 365 Enterprise F1</span></span>
- <span data-ttu-id="94348-121">オプション 3: その他の Office 365 プラン</span><span class="sxs-lookup"><span data-stu-id="94348-121">Option 3: Other Office 365 plans</span></span>

|<span data-ttu-id="94348-122">**機能**</span><span class="sxs-lookup"><span data-stu-id="94348-122">**Feature**</span></span>    |<span data-ttu-id="94348-123">**方法 1**</span><span class="sxs-lookup"><span data-stu-id="94348-123">**Option 1**</span></span>   |<span data-ttu-id="94348-124">**方法 2**</span><span class="sxs-lookup"><span data-stu-id="94348-124">**Option 2**</span></span>   |<span data-ttu-id="94348-125">**オプション3**</span><span class="sxs-lookup"><span data-stu-id="94348-125">**Option 3**</span></span>   |
|:-----------------|:-----------------|:-------------|:------------|
|<span data-ttu-id="94348-126">Skype for Business Online プラン 1 に含まれるすべての機能の利用</span><span class="sxs-lookup"><span data-stu-id="94348-126">Get all the features included in Skype for Business Online Plan 1</span></span>|<span data-ttu-id="94348-127">はい</span><span class="sxs-lookup"><span data-stu-id="94348-127">Yes</span></span>   |<span data-ttu-id="94348-128">はい</span><span class="sxs-lookup"><span data-stu-id="94348-128">Yes</span></span>   |<span data-ttu-id="94348-129">はい</span><span class="sxs-lookup"><span data-stu-id="94348-129">Yes</span></span>   |
|<span data-ttu-id="94348-130">IM とプレゼンス</span><span class="sxs-lookup"><span data-stu-id="94348-130">IM and presence</span></span> |<span data-ttu-id="94348-131">はい</span><span class="sxs-lookup"><span data-stu-id="94348-131">Yes</span></span>   |<span data-ttu-id="94348-132">はい</span><span class="sxs-lookup"><span data-stu-id="94348-132">Yes</span></span>   |<span data-ttu-id="94348-133">はい</span><span class="sxs-lookup"><span data-stu-id="94348-133">Yes</span></span>   |
|<span data-ttu-id="94348-134">IP を経由したピアツーピア オーディオとビデオ</span><span class="sxs-lookup"><span data-stu-id="94348-134">Peer-to-peer Audio and Video over IP</span></span>|<span data-ttu-id="94348-135">はい</span><span class="sxs-lookup"><span data-stu-id="94348-135">Yes</span></span>   |<span data-ttu-id="94348-136">はい</span><span class="sxs-lookup"><span data-stu-id="94348-136">Yes</span></span>   |<span data-ttu-id="94348-137">はい</span><span class="sxs-lookup"><span data-stu-id="94348-137">Yes</span></span>   
|<span data-ttu-id="94348-138">認証ユーザーとして会議に参加</span><span class="sxs-lookup"><span data-stu-id="94348-138">Join meetings as an authenticated user</span></span>| <span data-ttu-id="94348-139">はい</span><span class="sxs-lookup"><span data-stu-id="94348-139">Yes</span></span>   |<span data-ttu-id="94348-140">はい</span><span class="sxs-lookup"><span data-stu-id="94348-140">Yes</span></span>   |<span data-ttu-id="94348-141">はい</span><span class="sxs-lookup"><span data-stu-id="94348-141">Yes</span></span>   |

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="94348-142">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="94348-142">Transition customers to new product plans</span></span>

<span data-ttu-id="94348-143">マイクロソフトは、絶えず新しい製品やサービスをパートナーに提供しています。</span><span class="sxs-lookup"><span data-stu-id="94348-143">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="94348-144">パートナーはこれに対応して、お客様を新しいサービスにアップグレードするか、お客様のサブスクリプションを廃止予定の SKU から移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="94348-144">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="94348-145">廃止された SKU から新しい SKU にお客様を移行するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="94348-145">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

- <span data-ttu-id="94348-146">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="94348-146">Purchase the new subscription</span></span>
- <span data-ttu-id="94348-147">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="94348-147">Reassign current user licenses</span></span>
- <span data-ttu-id="94348-148">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="94348-148">Cancel old subscription</span></span>

### <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="94348-149">新しいプランにお客様を移行する</span><span class="sxs-lookup"><span data-stu-id="94348-149">Migrate your customers to new plans</span></span>

1. <span data-ttu-id="94348-150">新しいサブスクリプションを購入するには、**パートナー センター メニュー**で **[顧客]** を選び、移行する顧客を選んでから、**[サブスクリプションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="94348-150">To purchase the new subscription, from the **Partner Center menu**, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="94348-151">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="94348-151">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="94348-152">お客様には、古い Skype for Business Online プラン1サブスクリプションと、オプション 1-Office 365 Enterprise F1 などの新しい "ターゲット" サブスクリプションの両方が含まれるようになりました。</span><span class="sxs-lookup"><span data-stu-id="94348-152">Your customer should now have both old and new subscriptions, the old Skype for Business Online Plan 1  subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

3. <span data-ttu-id="94348-153">顧客のユーザーのライセンスをもう一度割り当てるには、**パートナー センター** メニューで **[顧客]** を選び、移行する顧客を選んでから **[ユーザーとライセンス]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="94348-153">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="94348-154">顧客の [ユーザーとライセンス] ページが開きます。</span><span class="sxs-lookup"><span data-stu-id="94348-154">The customer's Users and Licenses page opens.</span></span>

4. <span data-ttu-id="94348-155">ユーザー ライセンスをもう一度割り当てるには、割り当てるユーザーを選んで **[ライセンスの管理]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="94348-155">To reassign user license, select the user to reassign and then select **Manage licenses.**</span></span>

5. <span data-ttu-id="94348-156">**[ライセンスの管理]** ページで、Skype for Business Online プラン 1 のライセンスのチェック ボックスをオフにし、お客様の移行先サブスクリプションの新しいサービス プランを選びます。</span><span class="sxs-lookup"><span data-stu-id="94348-156">On the **Manage licenses** page, clear the Skype for Business Online Plan 1 license check box and select a new service plan for the subscription the customer is moving to.</span></span>

6. <span data-ttu-id="94348-157">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="94348-157">Select **Submit**.</span></span> <span data-ttu-id="94348-158">確認ページに新しいライセンスの割り当てが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="94348-158">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="94348-159">ライセンスの割り当てが必要な他のユーザーにも同じプロセスを続行します。</span><span class="sxs-lookup"><span data-stu-id="94348-159">Continue this same process for other users who need license assignments.</span></span>

<span data-ttu-id="94348-160">ユーザー ライセンスを新しいサービスに移行した後は、顧客レベルで廃止されたサブスクリプションを安全に取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="94348-160">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

7. <span data-ttu-id="94348-161">**パートナー センター** メニューで、**[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="94348-161">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="94348-162">サブスクリプションをキャンセルする顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="94348-162">Select the customer whose subscription you are canceling.</span></span>

8. <span data-ttu-id="94348-163">サブスクリプションの詳細ページで、サブスクリプションを **[中断]** に設定します。</span><span class="sxs-lookup"><span data-stu-id="94348-163">In the subscription detail page, set the subscription to **Suspended**.</span></span>

9. <span data-ttu-id="94348-164">[送信] を選択し**ます。**</span><span class="sxs-lookup"><span data-stu-id="94348-164">Select **Submit.**</span></span>

<span data-ttu-id="94348-165">以前のサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="94348-165">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="94348-166">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="94348-166">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="94348-167">お客様には、以前のサブスクリプションの追加コストは発生しません。</span><span class="sxs-lookup"><span data-stu-id="94348-167">The customer incurs no additional costs for the old subscription.</span></span>

