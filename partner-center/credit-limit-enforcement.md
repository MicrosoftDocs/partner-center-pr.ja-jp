---
title: クレジット制限の強制
ms.topic: how-to
ms.date: 05/11/2021
description: クレジット制限と計算方法について学習します。 FAQ が含まれています。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: da3fc23a51cc70eec91a304f14189eb191c71339
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148110"
---
# <a name="credit-limit-enforcement-cle"></a><span data-ttu-id="ff82a-104">与信限度額の適用 (CLE)</span><span class="sxs-lookup"><span data-stu-id="ff82a-104">Credit limit enforcement (CLE)</span></span>

<span data-ttu-id="ff82a-105">**適切なロール**: 課金管理者</span><span class="sxs-lookup"><span data-stu-id="ff82a-105">**Appropriate roles**: Billing admin</span></span>

## <a name="your-credit-limit-and-how-it-works"></a><span data-ttu-id="ff82a-106">クレジットの制限と動作</span><span class="sxs-lookup"><span data-stu-id="ff82a-106">Your credit limit and how it works</span></span>

<span data-ttu-id="ff82a-107">クレジット制限は、パートナーがパートナーとして購入できる最大金額 (米国ドル単位) です。この上限は、パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="ff82a-107">Your credit limit is the maximum amount (in US dollars) that you as a partner can spend to purchase products or subscriptions in Partner Center.</span></span> <span data-ttu-id="ff82a-108">クレジットの上限を超えると、十分な支払いが行われたまで、新しい購入を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="ff82a-108">If you exceed your credit limit, you’ll be unable to make new purchases until sufficient payment has been made.</span></span> <span data-ttu-id="ff82a-109">既存のサブスクリプションは中断されずに続行されます。</span><span class="sxs-lookup"><span data-stu-id="ff82a-109">Your existing subscriptions will continue uninterrupted.</span></span>

<span data-ttu-id="ff82a-110">クレジット制限は、Azure プラン、Azure 予約、ソフトウェア、Marketplace、Azure 145 P、Office、Dynamics 製品のオファーに適用されます。</span><span class="sxs-lookup"><span data-stu-id="ff82a-110">Credit limits apply to offers in Azure plan, Azure reservations, Software, Marketplace, Azure 145 P, Office, and Dynamics products.</span></span> <span data-ttu-id="ff82a-111">クレジット制限は、更新や継続的な消費には適用されません。</span><span class="sxs-lookup"><span data-stu-id="ff82a-111">Credit limits do not apply to renewals and ongoing consumption.</span></span>

<span data-ttu-id="ff82a-112">オンボード期間中は、テナント レベルでクレジット制限が割り当てされます。</span><span class="sxs-lookup"><span data-stu-id="ff82a-112">We assign your credit limit at the tenant level during your onboarding period.</span></span> <span data-ttu-id="ff82a-113">お客様の予測収益、購入力、支払い履歴に基付けています。</span><span class="sxs-lookup"><span data-stu-id="ff82a-113">We base it on your forecasted revenue, purchasing prowess, and payment history.</span></span> <span data-ttu-id="ff82a-114">次に、次の数式を使用して、使用可能な残高を計算します。</span><span class="sxs-lookup"><span data-stu-id="ff82a-114">We then use the following formula to calculate your available balance:</span></span>

<span data-ttu-id="ff82a-115">**[与信限度額 – (受信購入 + 未払い請求書 + 未請求料金 – 過払い) ]**</span><span class="sxs-lookup"><span data-stu-id="ff82a-115">**[Credit Limit – (Incoming Purchase + Outstanding Unpaid Invoices + Unbilled Charges – Overpayment)]**</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="ff82a-116">よく寄せられる質問</span><span class="sxs-lookup"><span data-stu-id="ff82a-116">Frequently Asked Questions</span></span>

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a><span data-ttu-id="ff82a-117">クレジット制限はテナントレベルまたはグローバル レベルで設定されていますか?</span><span class="sxs-lookup"><span data-stu-id="ff82a-117">Is my credit limit set at the tenant or global level?</span></span>

<span data-ttu-id="ff82a-118">テナント レベル。</span><span class="sxs-lookup"><span data-stu-id="ff82a-118">The tenant level.</span></span> <span data-ttu-id="ff82a-119">たとえば、米国、カナダ、日本から運用するとします。</span><span class="sxs-lookup"><span data-stu-id="ff82a-119">For example, suppose you operate from the US, Canada, and Japan.</span></span> <span data-ttu-id="ff82a-120">カナダのテナントがクレジット制限に達した場合、そのテナントは、テナントで購入を試みるときに通知を受け取パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="ff82a-120">If the Canadian tenant reaches its credit limit, then that tenant will receive a notification when they attempt to make a purchase in Partner Center.</span></span> <span data-ttu-id="ff82a-121">その他のテナントは影響を受け "ない"。</span><span class="sxs-lookup"><span data-stu-id="ff82a-121">The other tenants will not be affected.</span></span> 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a><span data-ttu-id="ff82a-122">クレジット制限を超えた場合、フル アクセスで既存の顧客とサブスクリプションにサービスを提供し続けできますか?</span><span class="sxs-lookup"><span data-stu-id="ff82a-122">If I exceed my credit limit, can I continue servicing existing customers and subscriptions with full access?</span></span>

<span data-ttu-id="ff82a-123">はい。</span><span class="sxs-lookup"><span data-stu-id="ff82a-123">Yes.</span></span> <span data-ttu-id="ff82a-124">お客様の既存のサブスクリプションは、中断されることなく継続されます。</span><span class="sxs-lookup"><span data-stu-id="ff82a-124">Your customers’ existing subscriptions will continue without interruption.</span></span> <span data-ttu-id="ff82a-125">ただし、顧客の新しいサブスクリプションを購入することはできません。</span><span class="sxs-lookup"><span data-stu-id="ff82a-125">However, you cannot buy new subscriptions for your customers.</span></span>

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a><span data-ttu-id="ff82a-126">CLE は、直接請求パートナーと間接プロバイダーの両方に適用されますか。</span><span class="sxs-lookup"><span data-stu-id="ff82a-126">Does CLE apply to both direct bill partners and indirect providers?</span></span>

<span data-ttu-id="ff82a-127">はい、両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="ff82a-127">Yes, it applies to both.</span></span>

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a><span data-ttu-id="ff82a-128">アカウントを復元するために支払いを送信した後、サブスクリプションをさらに購入できますか?</span><span class="sxs-lookup"><span data-stu-id="ff82a-128">After I submit my payment to reinstate my account, when can I purchase more subscriptions?</span></span> 

<span data-ttu-id="ff82a-129">支払いから24時間以内に購入を再開できるはずです。クレジットチェックプロセスを進めるために、Microsoft がすべての要件を受けたと想定しています。</span><span class="sxs-lookup"><span data-stu-id="ff82a-129">You should be able to resume purchasing within 24 hours of your payment, assuming Microsoft has received all the requirements to proceed with the credit check process.</span></span>

### <a name="how-can-i-check-my-credit-limit"></a><span data-ttu-id="ff82a-130">クレジットの上限を確認するにはどうすればよいですか?</span><span class="sxs-lookup"><span data-stu-id="ff82a-130">How can I check my credit limit?</span></span>

<span data-ttu-id="ff82a-131">[ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com)クレジットの上限を確認し、最近の購入に関する情報を取得するには、にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="ff82a-131">Contact [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to see your credit limit and get information about recent purchases.</span></span>

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a><span data-ttu-id="ff82a-132">紛争にある請求書は、クレジットの上限に対してカウントされますか?</span><span class="sxs-lookup"><span data-stu-id="ff82a-132">Do invoices that are in dispute count against the credit limit?</span></span>

<span data-ttu-id="ff82a-133">はい。</span><span class="sxs-lookup"><span data-stu-id="ff82a-133">Yes.</span></span> <span data-ttu-id="ff82a-134">ただし、Microsoft に連絡して [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) 問題を解決することができます。</span><span class="sxs-lookup"><span data-stu-id="ff82a-134">However, you can contact Microsoft at [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) to resolve the issue.</span></span>

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a><span data-ttu-id="ff82a-135">書き込みが行われた場合、すぐにはどうなり ucmwrcsp@microsoft.com ますか。</span><span class="sxs-lookup"><span data-stu-id="ff82a-135">How soon will I hear back if I write to ucmwrcsp@microsoft.com?</span></span>

<span data-ttu-id="ff82a-136">24時間未満の応答が必要です。</span><span class="sxs-lookup"><span data-stu-id="ff82a-136">You should have a response in less than 24 hours.</span></span> 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a><span data-ttu-id="ff82a-137">Microsoft はパートナーの信用限度を設定するためにどのような基準を使用しますか?</span><span class="sxs-lookup"><span data-stu-id="ff82a-137">What criteria does Microsoft use for setting a partner’s credit limit?</span></span>

<span data-ttu-id="ff82a-138">予測収益、購入 prowess、および支払い履歴に基づいて、お客様のクレジットの上限が決定されます。</span><span class="sxs-lookup"><span data-stu-id="ff82a-138">We determine your credit limit based on your forecasted revenue, purchasing prowess, and payment history.</span></span>

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a><span data-ttu-id="ff82a-139">現在、新しいコマースエクスペリエンスに対して与信限度が適用されていますか。</span><span class="sxs-lookup"><span data-stu-id="ff82a-139">Is the credit limit currently enforced on the New Commerce Experience?</span></span>

<span data-ttu-id="ff82a-140">はい。</span><span class="sxs-lookup"><span data-stu-id="ff82a-140">Yes.</span></span> <span data-ttu-id="ff82a-141">クレジットの制限は、パートナーセンターのすべての CSP プログラムと製品に適用されます。</span><span class="sxs-lookup"><span data-stu-id="ff82a-141">Credit limits apply to all CSP programs and products in Partner Center.</span></span>

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a><span data-ttu-id="ff82a-142">組織のクレジットの上限に近づいたときに通知を受けるのはだれですか。</span><span class="sxs-lookup"><span data-stu-id="ff82a-142">Who will receive the notification when my organization is nearing its credit limit?</span></span>

<span data-ttu-id="ff82a-143">組織の Finance アカウントの買掛金の連絡先に通知が届きます。</span><span class="sxs-lookup"><span data-stu-id="ff82a-143">Your organization's Finance Account Payable contact should receive the notification.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ff82a-144">次のステップ</span><span class="sxs-lookup"><span data-stu-id="ff82a-144">Next steps</span></span>

[<span data-ttu-id="ff82a-145">課金の基本</span><span class="sxs-lookup"><span data-stu-id="ff82a-145">Billing basics</span></span>](./billing-basics.md)
