---
title: 与信限度額の適用
ms.topic: how-to
ms.date: 05/11/2021
description: クレジット制限と計算方法について学習します。 FAQ が含まれています。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cf0d3c38b301c363a4a990db5258cf2a3f30d487
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/12/2021
ms.locfileid: "109819210"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="a570f-104">与信限度額の適用 (CLE)</span><span class="sxs-lookup"><span data-stu-id="a570f-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="a570f-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="a570f-105">**Appropriate roles**</span></span>

- <span data-ttu-id="a570f-106">課金管理者</span><span class="sxs-lookup"><span data-stu-id="a570f-106">Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="a570f-107">クレジットの制限と動作</span><span class="sxs-lookup"><span data-stu-id="a570f-107">Your credit limit and how it works</span></span>

<span data-ttu-id="a570f-108">クレジット制限は、パートナーがパートナーとして購入できる最大金額 (米国ドル単位) です。この上限は、パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="a570f-108">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="a570f-109">クレジットの上限を超えると、十分な支払いが行われたまで、新しい購入を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="a570f-109">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="a570f-110">既存のサブスクリプションは中断されずに続行されます。</span><span class="sxs-lookup"><span data-stu-id="a570f-110">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="a570f-111">クレジット制限は、Azure プラン、Azure 予約、ソフトウェア、Marketplace、Azure 145 P、Office、Dynamics 製品のオファーに適用されます。</span><span class="sxs-lookup"><span data-stu-id="a570f-111">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="a570f-112">クレジット制限は、更新や継続的な消費には適用されません。</span><span class="sxs-lookup"><span data-stu-id="a570f-112">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="a570f-113">オンボード期間中は、テナント レベルでクレジット制限が割り当てされます。</span><span class="sxs-lookup"><span data-stu-id="a570f-113">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="a570f-114">お客様の予測収益、購入力、支払い履歴に基付けています。</span><span class="sxs-lookup"><span data-stu-id="a570f-114">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="a570f-115">次に、次の数式を使用して、使用可能な残高を計算します。</span><span class="sxs-lookup"><span data-stu-id="a570f-115">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="a570f-116">**[与信限度額 – (受信購入 + 未払い請求書 + 未請求料金 – 過払い) ]**</span><span class="sxs-lookup"><span data-stu-id="a570f-116">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="a570f-117">よく寄せられる質問</span><span class="sxs-lookup"><span data-stu-id="a570f-117">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="a570f-118">クレジット制限はテナントレベルまたはグローバル レベルで設定されていますか?</span><span class="sxs-lookup"><span data-stu-id="a570f-118">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="a570f-119">テナント レベル。</span><span class="sxs-lookup"><span data-stu-id="a570f-119">The tenant level.</span></span> <span data-ttu-id="a570f-120">たとえば、米国、カナダ、日本から運用するとします。</span><span class="sxs-lookup"><span data-stu-id="a570f-120">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="a570f-121">カナダのテナントがクレジット制限に達した場合、そのテナントは、テナントで購入を試みるときに通知を受け取パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="a570f-121">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="a570f-122">その他のテナントは影響を受け "ない"。</span><span class="sxs-lookup"><span data-stu-id="a570f-122">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="a570f-123">クレジット制限を超えた場合、フル アクセスで既存の顧客とサブスクリプションにサービスを提供し続けできますか?</span><span class="sxs-lookup"><span data-stu-id="a570f-123">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="a570f-124">はい。</span><span class="sxs-lookup"><span data-stu-id="a570f-124">Yes.</span></span> <span data-ttu-id="a570f-125">顧客の既存のサブスクリプションは中断することなく継続されます。</span><span class="sxs-lookup"><span data-stu-id="a570f-125">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="a570f-126">ただし、顧客の新しいサブスクリプションを購入することはできません。</span><span class="sxs-lookup"><span data-stu-id="a570f-126">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="a570f-127">CLE は直接請求パートナーと間接プロバイダーの両方に適用されますか?</span><span class="sxs-lookup"><span data-stu-id="a570f-127">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="a570f-128">はい。両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="a570f-128">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="a570f-129">アカウントを再開するために支払いを送信した後、サブスクリプションを追加購入できる期間</span><span class="sxs-lookup"><span data-stu-id="a570f-129">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="a570f-130">Microsoft がクレジット チェック プロセスを続行するためにすべての要件を受け取ったと仮定すると、支払いから 24 時間以内に購入を再開できます。</span><span class="sxs-lookup"><span data-stu-id="a570f-130">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="a570f-131">クレジット制限を確認する方法</span><span class="sxs-lookup"><span data-stu-id="a570f-131">How can I check my credit limit?</span></span>

<span data-ttu-id="a570f-132">クレジット制限 [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) を確認し、最近の購入に関する情報を取得する場合は、 にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="a570f-132">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="a570f-133">クレームに含む請求書は、与信限度額に対してカウントされますか?</span><span class="sxs-lookup"><span data-stu-id="a570f-133">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="a570f-134">はい。</span><span class="sxs-lookup"><span data-stu-id="a570f-134">Yes.</span></span> <span data-ttu-id="a570f-135">ただし、 で Microsoft に問い合 [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) わせ、問題を解決することができます。</span><span class="sxs-lookup"><span data-stu-id="a570f-135">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="a570f-136">に書き込んだ場合、どのくらいの時間が来ますか ucmwrcsp@microsoft.com ?</span><span class="sxs-lookup"><span data-stu-id="a570f-136">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="a570f-137">応答は 24 時間以内に行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="a570f-137">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="a570f-138">Microsoft はパートナーのクレジット制限を設定するためにどのような基準を使用しますか?</span><span class="sxs-lookup"><span data-stu-id="a570f-138">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="a570f-139">予測収益、購入率、支払い履歴に基づいて、クレジット制限が決定されます。</span><span class="sxs-lookup"><span data-stu-id="a570f-139">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="a570f-140">現在、新しいコマース エクスペリエンスに対してクレジット制限が適用されていますか?</span><span class="sxs-lookup"><span data-stu-id="a570f-140">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="a570f-141">はい。</span><span class="sxs-lookup"><span data-stu-id="a570f-141">Yes.</span></span> <span data-ttu-id="a570f-142">クレジット制限は、すべての CSP プログラムと製品に適用され、パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="a570f-142">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="a570f-143">組織が与信限度額に近付いたときに通知を受け取るのは誰ですか?</span><span class="sxs-lookup"><span data-stu-id="a570f-143">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="a570f-144">組織の財務アカウントの支払い担当者が通知を受け取る必要があります。</span><span class="sxs-lookup"><span data-stu-id="a570f-144">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a570f-145">次の手順</span><span class="sxs-lookup"><span data-stu-id="a570f-145">Next steps</span></span>

[<span data-ttu-id="a570f-146">課金の基本</span><span class="sxs-lookup"><span data-stu-id="a570f-146">Billing basics</span></span>](./billing-basics.md)
