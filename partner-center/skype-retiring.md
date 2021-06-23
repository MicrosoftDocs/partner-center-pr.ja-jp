---
title: Skype for Business サブスクリプションの移行
description: 有効期限が切れた Skype for Business Online プラン1サブスクリプションを持つ特定の顧客を新しい Office 365 バージョンに移行する方法とタイミングについて説明します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: a8de5b824a24b07607b5365848ec1027ca0d08e8
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551539"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="4b890-103">Skype for Business Online プラン 1 サブスクリプションの新しい Office 365 バージョンへの移行</span><span class="sxs-lookup"><span data-stu-id="4b890-103">Migrate Skype for Business Online Plan 1 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="4b890-104">**適切なロール**: Sales agent</span><span class="sxs-lookup"><span data-stu-id="4b890-104">**Appropriate roles**: Sales agent</span></span>

<span data-ttu-id="4b890-105">Skype for Business Online プラン1は、2018年8月1日をもって廃止される予定です。</span><span class="sxs-lookup"><span data-stu-id="4b890-105">The Skype for Business Online Plan 1 will be retired, effective August 1, 2018.</span></span> <span data-ttu-id="4b890-106">この日付以降、新たに Skype for Business プラン 1 のサブスクリプションを購入することはできません。既存のサブスクリプションは、有効期限になると自動更新されず、更新のオプションは提供されません。</span><span class="sxs-lookup"><span data-stu-id="4b890-106">After that date customers can no longer purchase new Skype for Business Plan 1 subscriptions, and existing subscriptions will not renew automatically when they expire and will not provide a renewal option.</span></span> <span data-ttu-id="4b890-107">サブスクリプションの詳細ページでは、Skype for Business Online プラン 1 のサブスクリプションの状態が、"自動更新: [日付]" から "有効期限: [date]" に変更されています。</span><span class="sxs-lookup"><span data-stu-id="4b890-107">On the subscription's detail page, the Skype for Business Online Plan 1 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span>  

<span data-ttu-id="4b890-108">お客様への継続的なサービス提供のためには、有効期限が迫っている Skype for Business Online プラン 1 のサブスクリプションのお客様を、サポートされている以下の SKU オプションに移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4b890-108">To ensure continuity for customers, you should transition customers with expiring Skype for Business Online Plan 1 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="4b890-109">顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="4b890-109">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

>[!NOTE]
><span data-ttu-id="4b890-110">Skype for Business Online プラン 1 の商用 SKU と行政機関用 SKUは、どちらも提供終了となります。</span><span class="sxs-lookup"><span data-stu-id="4b890-110">Both Skype for Business Online Plan 1 commercial and government SKUs are retired.</span></span>

<span data-ttu-id="4b890-111">API (コマース REST (CREST) またはパートナーセンター) を使用する場合は、サブスクリプションの終了日を自動更新 = False プロパティと共に評価して、期限切れのサブスクリプションを見つけます。</span><span class="sxs-lookup"><span data-stu-id="4b890-111">If you use the API (either Commerce REST (CREST) or Partner Center), find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="4b890-112">Skype for Business Online プラン 1 のサブスクリプションは、2018 年 9 月 1 日に auto renew = False に設定されます。</span><span class="sxs-lookup"><span data-stu-id="4b890-112">The Skype for Business Online Plan 1 subscriptions will be set to auto renew=False on September 1, 2018.</span></span> <span data-ttu-id="4b890-113">お客様は、いつでも新しいプランに移動できます。</span><span class="sxs-lookup"><span data-stu-id="4b890-113">You can move customers to a new plan at any time.</span></span> 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a><span data-ttu-id="4b890-114">Skype for Business Online プラン 1 の代替プラン</span><span class="sxs-lookup"><span data-stu-id="4b890-114">Skype for Business Online Plan 1 replacement plans</span></span>

<span data-ttu-id="4b890-115">新しいプランでは、お客様は Office 365 の新機能を活用できます。</span><span class="sxs-lookup"><span data-stu-id="4b890-115">With the new plans, your customers take can advantage of newer features and functionality in Office 365.</span></span> <span data-ttu-id="4b890-116">料金の詳細は、パートナー センターの料金表またはプランのマトリックスに記載されています。</span><span class="sxs-lookup"><span data-stu-id="4b890-116">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> 

- <span data-ttu-id="4b890-117">オプション1: Office 365 Enterprise F1</span><span class="sxs-lookup"><span data-stu-id="4b890-117">Option 1: Office 365 Enterprise F1</span></span>
- <span data-ttu-id="4b890-118">オプション 2: Microsoft 365 Enterprise F1</span><span class="sxs-lookup"><span data-stu-id="4b890-118">Option 2: Microsoft 365 Enterprise F1</span></span>
- <span data-ttu-id="4b890-119">オプション 3: その他の Office 365 プラン</span><span class="sxs-lookup"><span data-stu-id="4b890-119">Option 3: Other Office 365 plans</span></span>

|<span data-ttu-id="4b890-120">**機能**</span><span class="sxs-lookup"><span data-stu-id="4b890-120">**Feature**</span></span>    |<span data-ttu-id="4b890-121">**方法 1**</span><span class="sxs-lookup"><span data-stu-id="4b890-121">**Option 1**</span></span>   |<span data-ttu-id="4b890-122">**方法 2**</span><span class="sxs-lookup"><span data-stu-id="4b890-122">**Option 2**</span></span>   |<span data-ttu-id="4b890-123">**オプション3**</span><span class="sxs-lookup"><span data-stu-id="4b890-123">**Option 3**</span></span>   |
|:-----------------|:-----------------|:-------------|:------------|
|<span data-ttu-id="4b890-124">Skype for Business Online プラン 1 に含まれるすべての機能の利用</span><span class="sxs-lookup"><span data-stu-id="4b890-124">Get all the features included in Skype for Business Online Plan 1</span></span>|<span data-ttu-id="4b890-125">はい</span><span class="sxs-lookup"><span data-stu-id="4b890-125">Yes</span></span>   |<span data-ttu-id="4b890-126">はい</span><span class="sxs-lookup"><span data-stu-id="4b890-126">Yes</span></span>   |<span data-ttu-id="4b890-127">はい</span><span class="sxs-lookup"><span data-stu-id="4b890-127">Yes</span></span>   |
|<span data-ttu-id="4b890-128">IM とプレゼンス</span><span class="sxs-lookup"><span data-stu-id="4b890-128">IM and presence</span></span> |<span data-ttu-id="4b890-129">はい</span><span class="sxs-lookup"><span data-stu-id="4b890-129">Yes</span></span>   |<span data-ttu-id="4b890-130">はい</span><span class="sxs-lookup"><span data-stu-id="4b890-130">Yes</span></span>   |<span data-ttu-id="4b890-131">はい</span><span class="sxs-lookup"><span data-stu-id="4b890-131">Yes</span></span>   |
|<span data-ttu-id="4b890-132">IP を経由したピアツーピア オーディオとビデオ</span><span class="sxs-lookup"><span data-stu-id="4b890-132">Peer-to-peer Audio and Video over IP</span></span>|<span data-ttu-id="4b890-133">はい</span><span class="sxs-lookup"><span data-stu-id="4b890-133">Yes</span></span>   |<span data-ttu-id="4b890-134">はい</span><span class="sxs-lookup"><span data-stu-id="4b890-134">Yes</span></span>   |<span data-ttu-id="4b890-135">はい</span><span class="sxs-lookup"><span data-stu-id="4b890-135">Yes</span></span>   
|<span data-ttu-id="4b890-136">認証ユーザーとして会議に参加</span><span class="sxs-lookup"><span data-stu-id="4b890-136">Join meetings as an authenticated user</span></span>| <span data-ttu-id="4b890-137">はい</span><span class="sxs-lookup"><span data-stu-id="4b890-137">Yes</span></span>   |<span data-ttu-id="4b890-138">はい</span><span class="sxs-lookup"><span data-stu-id="4b890-138">Yes</span></span>   |<span data-ttu-id="4b890-139">はい</span><span class="sxs-lookup"><span data-stu-id="4b890-139">Yes</span></span>   |

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="4b890-140">顧客を新しい製品プランに移行する</span><span class="sxs-lookup"><span data-stu-id="4b890-140">Transition customers to new product plans</span></span>

<span data-ttu-id="4b890-141">マイクロソフトは、絶えず新しい製品やサービスをパートナーに提供しています。</span><span class="sxs-lookup"><span data-stu-id="4b890-141">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="4b890-142">パートナーはこれに対応して、お客様を新しいサービスにアップグレードするか、お客様のサブスクリプションを廃止予定の SKU から移行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4b890-142">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="4b890-143">廃止された SKU から新しい SKU にお客様を移行するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="4b890-143">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

- <span data-ttu-id="4b890-144">新しいサブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="4b890-144">Purchase the new subscription</span></span>
- <span data-ttu-id="4b890-145">現在のユーザー ライセンスをもう一度割り当てる</span><span class="sxs-lookup"><span data-stu-id="4b890-145">Reassign current user licenses</span></span>
- <span data-ttu-id="4b890-146">以前のサブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="4b890-146">Cancel old subscription</span></span>

### <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="4b890-147">新しいプランにお客様を移行する</span><span class="sxs-lookup"><span data-stu-id="4b890-147">Migrate your customers to new plans</span></span>

1. <span data-ttu-id="4b890-148">新しいサブスクリプションを購入するには、**パートナー センター メニュー** で **[顧客]** を選び、移行する顧客を選んでから、**[サブスクリプションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="4b890-148">To purchase the new subscription, from the **Partner Center menu**, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="4b890-149">購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="4b890-149">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="4b890-150">お客様には、古い Skype for Business Online プラン1サブスクリプションと、オプション 1-Office 365 Enterprise F1 などの新しい "ターゲット" サブスクリプションの両方が含まれるようになりました。</span><span class="sxs-lookup"><span data-stu-id="4b890-150">Your customer should now have both old and new subscriptions, the old Skype for Business Online Plan 1  subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

3. <span data-ttu-id="4b890-151">顧客のユーザーのライセンスをもう一度割り当てるには、**パートナー センター** メニューで **[顧客]** を選び、移行する顧客を選んでから **[ユーザーとライセンス]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="4b890-151">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="4b890-152">顧客の [ユーザーとライセンス] ページが開きます。</span><span class="sxs-lookup"><span data-stu-id="4b890-152">The customer's Users and Licenses page opens.</span></span>

4. <span data-ttu-id="4b890-153">ユーザー ライセンスをもう一度割り当てるには、割り当てるユーザーを選んで **[ライセンスの管理]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="4b890-153">To reassign user license, select the user to reassign and then select **Manage licenses.**</span></span>

5. <span data-ttu-id="4b890-154">**[ライセンスの管理]** ページで、Skype for Business Online プラン 1 のライセンスのチェック ボックスをオフにし、お客様の移行先サブスクリプションの新しいサービス プランを選びます。</span><span class="sxs-lookup"><span data-stu-id="4b890-154">On the **Manage licenses** page, clear the Skype for Business Online Plan 1 license check box and select a new service plan for the subscription the customer is moving to.</span></span>

6. <span data-ttu-id="4b890-155">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="4b890-155">Select **Submit**.</span></span> <span data-ttu-id="4b890-156">確認ページに新しいライセンスの割り当てが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="4b890-156">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="4b890-157">ライセンスの割り当てが必要な他のユーザーにも同じプロセスを続行します。</span><span class="sxs-lookup"><span data-stu-id="4b890-157">Continue this same process for other users who need license assignments.</span></span>

<span data-ttu-id="4b890-158">ユーザー ライセンスを新しいサービスに移行した後は、顧客レベルで廃止されたサブスクリプションを安全に取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="4b890-158">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

7. <span data-ttu-id="4b890-159">**パートナー センター** メニューで、**[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="4b890-159">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="4b890-160">サブスクリプションをキャンセルする顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="4b890-160">Select the customer whose subscription you are canceling.</span></span>

8. <span data-ttu-id="4b890-161">サブスクリプションの詳細ページで、サブスクリプションを **[中断]** に設定します。</span><span class="sxs-lookup"><span data-stu-id="4b890-161">In the subscription detail page, set the subscription to **Suspended**.</span></span>

9. <span data-ttu-id="4b890-162">[送信] を選択し **ます。**</span><span class="sxs-lookup"><span data-stu-id="4b890-162">Select **Submit.**</span></span>

<span data-ttu-id="4b890-163">以前のサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="4b890-163">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="4b890-164">中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。</span><span class="sxs-lookup"><span data-stu-id="4b890-164">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="4b890-165">お客様には、以前のサブスクリプションの追加コストは発生しません。</span><span class="sxs-lookup"><span data-stu-id="4b890-165">The customer incurs no additional costs for the old subscription.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4b890-166">次の手順</span><span class="sxs-lookup"><span data-stu-id="4b890-166">Next steps</span></span>

- [<span data-ttu-id="4b890-167">アドバイザー: クライアントが Office 365 を試すための試用版への招待を作成して送信する</span><span class="sxs-lookup"><span data-stu-id="4b890-167">Advisors: Create and send a trial invitation for clients to try Office 365</span></span>](advisors-create-a-trial-invitation.md)
- [<span data-ttu-id="4b890-168">アドバイザー: Office 365 試用版への招待と購入プランを使用して、クライアントベースを構築する</span><span class="sxs-lookup"><span data-stu-id="4b890-168">Advisors: Build your client base with Office 365 trial invitations and purchase offers</span></span>](advisors-build-your-business.md)
- [<span data-ttu-id="4b890-169">アドバイザー: 購入プランを作成する</span><span class="sxs-lookup"><span data-stu-id="4b890-169">Advisors: Create a purchase offer</span></span>](advisor-create-a-purchase-offer.md)
