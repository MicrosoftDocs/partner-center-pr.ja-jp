---
title: 顧客向けの Azure 予約を管理する
description: 予約を取り消す方法、予約を交換する方法、返金を要求する方法など、顧客の Azure 予約を管理する方法について説明します。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 937a7268caa5ae7872f8a3ec6dcb05f56dd9fbe5
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000256"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a><span data-ttu-id="7b3c3-103">顧客の予約 Microsoft Azure 管理、取り消し、交換、返金する</span><span class="sxs-lookup"><span data-stu-id="7b3c3-103">Manage, cancel, exchange, or refund Microsoft Azure reservations for customers</span></span>

<span data-ttu-id="7b3c3-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-104">**Applies to**</span></span>

- <span data-ttu-id="7b3c3-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="7b3c3-105">Partner Center</span></span>
- <span data-ttu-id="7b3c3-106">Microsoft Azure portal</span><span class="sxs-lookup"><span data-stu-id="7b3c3-106">Microsoft Azure portal</span></span> 
- <span data-ttu-id="7b3c3-107">CSP のパートナー</span><span class="sxs-lookup"><span data-stu-id="7b3c3-107">Partners in CSP</span></span>

<span data-ttu-id="7b3c3-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-108">**Appropriate roles**</span></span>

- <span data-ttu-id="7b3c3-109">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="7b3c3-109">Admin agent</span></span>
- <span data-ttu-id="7b3c3-110">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="7b3c3-110">Global admin</span></span>
- <span data-ttu-id="7b3c3-111">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="7b3c3-111">Helpdesk agent</span></span>
- <span data-ttu-id="7b3c3-112">販売代理店</span><span class="sxs-lookup"><span data-stu-id="7b3c3-112">Sales agent</span></span>
- <span data-ttu-id="7b3c3-113">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="7b3c3-113">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="7b3c3-114">この記事は、クラウドソリューションプロバイダー (CSP) プログラムのパートナーにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-114">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="7b3c3-115">他の種類のサブスクリプション (従量課金制、個人、Microsoft カスタマーアグリーメント、マイクロソフトエンタープライズ契約サブスクリプションなど) を使用しているお客様は、代わりに [この Azure 予約ドキュメント](/azure/cost-management-billing/reservations)を読む必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-115">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="7b3c3-116">購入後に顧客の Azure 予約を管理するには、パートナーセンターで管理する顧客と予約を選択し、Azure portal の予約に変更を加えます。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-116">To manage your customers' Azure reservations post-purchase, you'll select the customer and reservation you want to manage in Partner Center, and then make changes to the reservation in the Azure portal.</span></span>

1. <span data-ttu-id="7b3c3-117">まずパートナー センター メニューで **[顧客]** を選択し、管理対象の予約を持つ顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-117">To get started, select **Customers** from the Partner Center menu and then select the customer whose reservations you want to manage.</span></span> 

2. <span data-ttu-id="7b3c3-118">顧客の詳細ページメニューで、[ **Azure の予約** ] を選択し、管理する特定の予約を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-118">On the customer's detail page menu, select **Azure reservations** and then select the specific reservation you want to manage.</span></span>  

3. <span data-ttu-id="7b3c3-119">[ **アクション**] で、[ **管理** ] を選択して、Azure portal の顧客の予約レコードにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-119">Under **Actions**, select **Manage** to go to the customer's reservation record in the Azure portal.</span></span> <span data-ttu-id="7b3c3-120">予約の詳細ページで、次の手順に従ってタスクを完了します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-120">On the reservation detail page, follow the steps below to complete tasks.</span></span>  

    | <span data-ttu-id="7b3c3-121">**Select**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-121">**Select**</span></span>   | <span data-ttu-id="7b3c3-122">**To**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-122">**To**</span></span>    |
    |:-----------------------------|:-----------------|
    | <span data-ttu-id="7b3c3-123">**概要**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-123">**Overview**</span></span>   | <span data-ttu-id="7b3c3-124">有効期限、スコープ、使用状況データなど、顧客の予約の詳細を表示します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-124">View details of a customer's reservation, including expiration date, scope, and utilization data.</span></span> <span data-ttu-id="7b3c3-125">**注意:** 日割り計算の払い戻しを求めるサポート要求を作成するには、**[Refund]** (払い戻し) を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-125">**NOTE** Select **Refund** to create a support request for a pro-rated refund.</span></span> <span data-ttu-id="7b3c3-126">予約期間のうち未使用の部分を交換するためのサポート要求を作成するには、**[交換]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-126">Select **Exchange** to create a support request to exchange the unused portion of your reservation term.</span></span>  
    | <span data-ttu-id="7b3c3-127">**アクセス制御 (IAM)**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-127">**Access Control (IAM)**</span></span>   | <span data-ttu-id="7b3c3-128">顧客の予約情報へのアクセスを管理します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-128">Manage access to the customer's reservation information.</span></span>|
    | <span data-ttu-id="7b3c3-129">**構成**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-129">**Configuration**</span></span>   | <span data-ttu-id="7b3c3-130">予約が関連付けられている予約のスコープや Azure サブスクリプションを変更します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-130">Change the reservation's scope and/or the Azure subscription the reservation is associated with.</span></span>    |
    | <span data-ttu-id="7b3c3-131">**プロパティ**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-131">**Properties**</span></span>   | <span data-ttu-id="7b3c3-132">予約のプロパティを表示し、予約 ID と予約注文 ID をクリップボードにコピーします。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-132">View the reservation's properties and copy to the clipboard the reservation ID and reservation order ID.</span></span> <span data-ttu-id="7b3c3-133">**注意:** 顧客に代わってサポートを要求する際には、予約 ID と予約注文 ID がサポートから求められることがあります。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-133">**NOTE** Support may ask you for the reservation ID and reservation order ID when you request support on behalf of a customer.</span></span>    |
    | <span data-ttu-id="7b3c3-134">**新しいサポート要求**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-134">**New support request**</span></span>    | <span data-ttu-id="7b3c3-135">Microsoft サポートによるヘルプを要求します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-135">Request help from Microsoft Support.</span></span>   |
 
## <a name="cancel-or-exchange-a-reservation"></a><span data-ttu-id="7b3c3-136">予約の取り消しまたは交換</span><span class="sxs-lookup"><span data-stu-id="7b3c3-136">Cancel or exchange a reservation</span></span>

<span data-ttu-id="7b3c3-137">お客様のビジネスニーズが変化した場合、予約を取り消し、返金を受けるか、予約の日割り返金額を交換して新しい予約価格に使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-137">If at any point a customer's business needs change, they may want to cancel a reservation and get a refund or exchange a reservation's prorated refund amount to be used toward the price of a new reservation.</span></span>

<span data-ttu-id="7b3c3-138">これらのシナリオのいずれにおいても、Microsoft はお客様にその金額を払い戻すため、お客様の方で顧客との間で結果として生じる財務トランザクションを管理していただけます。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-138">In both of these scenarios, Microsoft refunds the amount to you so that you can then manage the resulting financial transactions with your customers.</span></span> <span data-ttu-id="7b3c3-139">Microsoft は、請求、取り消し、または払い戻しに関して顧客と直接やりとりすることはありません。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-139">Microsoft does not contact customers directly about billing, cancellations, or refunds.</span></span>

### <a name="how-cancellations-work"></a><span data-ttu-id="7b3c3-140">取り消しのしくみ</span><span class="sxs-lookup"><span data-stu-id="7b3c3-140">How cancellations work</span></span>

<span data-ttu-id="7b3c3-141">顧客はいつでも予約の取り消しを要求できます (払い戻し額は 1 年あたり $50,000 までに制限されます)。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-141">Customers can request to cancel a reservation at any time (refund amount capped at $50,000 per year).</span></span> <span data-ttu-id="7b3c3-142">予約を取り消すと、お客様は、Azure 予約の残りの月の金額を早期終了料金で返すことができます。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-142">Canceling a reservation allows the customer to return the amount of the remaining months of an Azure reservation for an early termination fee.</span></span> <span data-ttu-id="7b3c3-143">残りの日割り残高は、早期終了料金から、お客様のアカウントを返金できるように、お客様のアカウントに返金されます。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-143">The remaining prorated balance, minus the early termination fee, is refunded to your account so that you can refund the customer's account.</span></span> 

<span data-ttu-id="7b3c3-144">取り消しの詳細と料金については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-144">See below for cancellation details and fees.</span></span>


|<span data-ttu-id="7b3c3-145">**取消日**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-145">**Cancellation date**</span></span><br> <span data-ttu-id="7b3c3-146">(日数)</span><span class="sxs-lookup"><span data-stu-id="7b3c3-146">(days)</span></span>   |<span data-ttu-id="7b3c3-147">**使用方法**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-147">**Usage**</span></span>    |<span data-ttu-id="7b3c3-148">**クレジット**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-148">**Credit**</span></span>  |<span data-ttu-id="7b3c3-149">**中途解約**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-149">**Early termination**</span></span><br> <span data-ttu-id="7b3c3-150">料金</span><span class="sxs-lookup"><span data-stu-id="7b3c3-150">fee</span></span>    |<span data-ttu-id="7b3c3-151">**払い戻し上限額**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-151">**Refund cap**</span></span> | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|<span data-ttu-id="7b3c3-152">5 日以下</span><span class="sxs-lookup"><span data-stu-id="7b3c3-152">5 or fewer</span></span>                         | <span data-ttu-id="7b3c3-153">いいえ</span><span class="sxs-lookup"><span data-stu-id="7b3c3-153">No</span></span>          | <span data-ttu-id="7b3c3-154">100%</span><span class="sxs-lookup"><span data-stu-id="7b3c3-154">100%</span></span>       | <span data-ttu-id="7b3c3-155">いいえ</span><span class="sxs-lookup"><span data-stu-id="7b3c3-155">No</span></span>                              | <span data-ttu-id="7b3c3-156">50,000 米国ドル</span><span class="sxs-lookup"><span data-stu-id="7b3c3-156">$50,000 USD</span></span>   |
|<span data-ttu-id="7b3c3-157">5 日以下</span><span class="sxs-lookup"><span data-stu-id="7b3c3-157">5 or fewer</span></span>                         | <span data-ttu-id="7b3c3-158">はい</span><span class="sxs-lookup"><span data-stu-id="7b3c3-158">Yes</span></span>         | <span data-ttu-id="7b3c3-159">日割り</span><span class="sxs-lookup"><span data-stu-id="7b3c3-159">Pro-rated</span></span>  | <span data-ttu-id="7b3c3-160">いいえ</span><span class="sxs-lookup"><span data-stu-id="7b3c3-160">No</span></span>                              | <span data-ttu-id="7b3c3-161">50,000 米国ドル</span><span class="sxs-lookup"><span data-stu-id="7b3c3-161">$50,000 USD</span></span>   |
|<span data-ttu-id="7b3c3-162">6 日以上</span><span class="sxs-lookup"><span data-stu-id="7b3c3-162">More than 5</span></span>                        | <span data-ttu-id="7b3c3-163">いいえ</span><span class="sxs-lookup"><span data-stu-id="7b3c3-163">No</span></span>          | <span data-ttu-id="7b3c3-164">日割り</span><span class="sxs-lookup"><span data-stu-id="7b3c3-164">Pro-rated</span></span>  | <span data-ttu-id="7b3c3-165">12%</span><span class="sxs-lookup"><span data-stu-id="7b3c3-165">12%</span></span>                             | <span data-ttu-id="7b3c3-166">50,000 米国ドル</span><span class="sxs-lookup"><span data-stu-id="7b3c3-166">$50,000 USD</span></span>   |
|<span data-ttu-id="7b3c3-167">6 日以上</span><span class="sxs-lookup"><span data-stu-id="7b3c3-167">More than 5</span></span>                        | <span data-ttu-id="7b3c3-168">はい</span><span class="sxs-lookup"><span data-stu-id="7b3c3-168">Yes</span></span>         | <span data-ttu-id="7b3c3-169">日割り</span><span class="sxs-lookup"><span data-stu-id="7b3c3-169">Pro-rated</span></span>  | <span data-ttu-id="7b3c3-170">12%</span><span class="sxs-lookup"><span data-stu-id="7b3c3-170">12%</span></span>                             | <span data-ttu-id="7b3c3-171">50,000 米国ドル</span><span class="sxs-lookup"><span data-stu-id="7b3c3-171">$50,000 USD</span></span>   |

### <a name="how-exchanges-work"></a><span data-ttu-id="7b3c3-172">交換のしくみ</span><span class="sxs-lookup"><span data-stu-id="7b3c3-172">How exchanges work</span></span> 

<span data-ttu-id="7b3c3-173">顧客がお客様から最初に購入した予約ではなく、別の予約を購入する場合、顧客は交換を要求できます。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-173">If a customer wants to buy a different reservation than the one they originally bought from you, they can request an exchange.</span></span> <span data-ttu-id="7b3c3-174">予約の交換は、顧客が新しい予約の価格に対して日割り返金金額を使用できるようにするため、予約を取り消すことに代わる魅力的な方法です。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-174">Exchanging a reservation can be an attractive alternative to canceling a reservation because it allows the customer to use the prorated refund amount toward the price of the new reservation.</span></span> 

<span data-ttu-id="7b3c3-175">日割りの払い戻し額がお客様のアカウントに入金されるため、お客様から顧客に交換を提供します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-175">The prorated refund amount is credited to your account so that you can offer the customer an exchange.</span></span>

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a><span data-ttu-id="7b3c3-176">顧客に代わって払い戻しまたは交換を申請する</span><span class="sxs-lookup"><span data-stu-id="7b3c3-176">Request a refund or exchange on behalf of a customer</span></span>

<span data-ttu-id="7b3c3-177">お客様の代わりに返金または交換のサポートリクエストを申請するには、パートナーセンターで顧客と予約を選択し、Azure portal にサポートリクエストを作成します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-177">To file a support request for a refund or exchange on behalf of your customers, you'll select the customer and reservation in Partner Center, and then create the support request in the Azure portal.</span></span> 

>[!NOTE]
><span data-ttu-id="7b3c3-178">Microsoft サポート担当者から、予約 ID と予約注文 ID が求められることがあります。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-178">Microsoft Support agents may ask you to provide the reservation ID and reservation order ID.</span></span> <span data-ttu-id="7b3c3-179">この情報は、Azure portal の予約の [ **プロパティ** ] ページで確認できます。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-179">You can find this information on the reservation's **Properties** page in the Azure portal.</span></span>

1. <span data-ttu-id="7b3c3-180">まずパートナー センター メニューで **[顧客]** を選択し、払い戻しを受ける顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-180">To get started, select **Customers** from the Partner Center menu and then select the customer who wants a refund.</span></span> 

2. <span data-ttu-id="7b3c3-181">顧客の詳細ページで、[ **Azure の予約** ] を選択し、顧客が返金を希望する特定の予約を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-181">On the customer's detail page, select **Azure reservations** and then select the specific reservation the customer wants refunded.</span></span>  

3. <span data-ttu-id="7b3c3-182">[ **アクション**] で、[ **返金** ] を選択して Azure portal の顧客の予約レコードにアクセスし、サポート要求を開始します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-182">Under **Actions**, select **Refund** to go to the customer's reservation record in the Azure portal and initiate a support request.</span></span>  

4. <span data-ttu-id="7b3c3-183">**[新しいサポート要求]** ページで、次の手順に従って払い戻しを申請します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-183">On the **New support request** page, follow the steps below to request a refund.</span></span> <span data-ttu-id="7b3c3-184">各手順の後には、**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-184">Select **Next** after each step.</span></span> 

   |<span data-ttu-id="7b3c3-185">**Step**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-185">**Step**</span></span>                    |<span data-ttu-id="7b3c3-186">**選択内容**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-186">**Selections**</span></span>    |
   |:---------------------------|:-----------------|
   |<span data-ttu-id="7b3c3-187">**1基本**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-187">**1 Basics**</span></span>                |<span data-ttu-id="7b3c3-188">問題の種類: 請求</span><span class="sxs-lookup"><span data-stu-id="7b3c3-188">Issue type: Billing.</span></span>  |
   |<span data-ttu-id="7b3c3-189">**2問題**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-189">**2 Problem**</span></span>               |<span data-ttu-id="7b3c3-190">問題の種類: 予約管理</span><span class="sxs-lookup"><span data-stu-id="7b3c3-190">Problem type: Reservation management.</span></span> <span data-ttu-id="7b3c3-191">カテゴリ: 交換と払い戻し</span><span class="sxs-lookup"><span data-stu-id="7b3c3-191">Category: Exchanges and refunds.</span></span> |
   |<span data-ttu-id="7b3c3-192">**3 連絡先情報**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-192">**3 Contact information**</span></span>   |<span data-ttu-id="7b3c3-193">基本設定を選択し、必要な情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-193">Select your preferences and enter the required information.</span></span> 

5. <span data-ttu-id="7b3c3-194">完了したら **[作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-194">Select **Create** when done.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="7b3c3-195">Azure Reservations に関するリソース</span><span class="sxs-lookup"><span data-stu-id="7b3c3-195">Azure reservations resources</span></span>

|<span data-ttu-id="7b3c3-196">**対象**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-196">**For information about**</span></span>   |<span data-ttu-id="7b3c3-197">**参照先**</span><span class="sxs-lookup"><span data-stu-id="7b3c3-197">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="7b3c3-198">CSP での Azure Reservations 概要</span><span class="sxs-lookup"><span data-stu-id="7b3c3-198">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="7b3c3-199">Microsoft Azure Reserved Instances の販売</span><span class="sxs-lookup"><span data-stu-id="7b3c3-199">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md) |
|<span data-ttu-id="7b3c3-200">パートナー センターで顧客の Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="7b3c3-200">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="7b3c3-201">Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="7b3c3-201">Buy Azure reservations</span></span>](azure-reservations-buying.md) |
|<span data-ttu-id="7b3c3-202">適切な VM サイズの判断と顧客による VM 使用状況の確認</span><span class="sxs-lookup"><span data-stu-id="7b3c3-202">Determine the correct VM size and verify customer VM usage</span></span>   | [<span data-ttu-id="7b3c3-203">Azure Reservation の最大使用量に対応する VM サイズ</span><span class="sxs-lookup"><span data-stu-id="7b3c3-203">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="7b3c3-204">パートナー センター API を使用して Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="7b3c3-204">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="7b3c3-205">[Azure Reserved VM Instances の購入](/partner-center/develop/purchase-azure-reservations) (パートナー センター開発者向けドキュメント)</span><span class="sxs-lookup"><span data-stu-id="7b3c3-205">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="7b3c3-206">購入したサブスクリプションから独自の Azure 予約を購入するためのアクセス許可を顧客に付与します。</span><span class="sxs-lookup"><span data-stu-id="7b3c3-206">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="7b3c3-207">独自の Azure 予約を購入するためのアクセス許可を顧客に付与する</span><span class="sxs-lookup"><span data-stu-id="7b3c3-207">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |