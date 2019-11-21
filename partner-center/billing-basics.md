---
title: 請求の概要 | パートナー センター
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: パートナーセンターの Azure サブスクリプションと予約に関する基本的な課金シナリオと、ライセンスベースと使用量ベースの課金の違いについて説明します。
author: LauraBrenner
ms.author: labrenne
keywords: 請求, 支払い,注文,取り消し, 注文管理, 未払い, 詐欺, 不正使用, 税, 税額控除, 調整ファイル, 調整用のファイル
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 2087b75419e0f5235e1efcc67ecdd8f203f382c1
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253208"
---
# <a name="billing-overview"></a><span data-ttu-id="1f1ab-104">請求の概要</span><span class="sxs-lookup"><span data-stu-id="1f1ab-104">Billing overview</span></span>

<span data-ttu-id="1f1ab-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="1f1ab-105">**Applies to**</span></span>

-  <span data-ttu-id="1f1ab-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="1f1ab-106">Partner Center</span></span>
-  <span data-ttu-id="1f1ab-107">CSP プログラムのパートナー</span><span class="sxs-lookup"><span data-stu-id="1f1ab-107">Partners in the CSP program</span></span>

<span data-ttu-id="1f1ab-108">お客様の代わりに購入した製品、ソリューション、サービスによっては、次の1つ以上の方法でこれらの購入に対して課金されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-108">Depending on the products, solutions, and services you buy on behalf of your customers, you'll be billed for these purchases in one or more of the following ways:</span></span>
-   [<span data-ttu-id="1f1ab-109">ライセンスベースの請求</span><span class="sxs-lookup"><span data-stu-id="1f1ab-109">License-based billing</span></span>](#licensebasedbilling)

    <span data-ttu-id="1f1ab-110">ライセンスを必要とする製品またはオンラインサービスを購入する場合は、購入したライセンスごとに請求されます (ライセンスの使用状況ではありません)。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-110">When you buy products or online services that require licenses, you're billed for each license you bought (not on license usage).</span></span> <span data-ttu-id="1f1ab-111">月 1 回または年 1 回の請求を選択できます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-111">You can choose whether to be billed once a month or once a year.</span></span> <span data-ttu-id="1f1ab-112">ビジネス ニーズが変わった場合、方法を変更したり戻したりできます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-112">If your business needs change, you can switch from one to the other and back again.</span></span> 
    
    <span data-ttu-id="1f1ab-113">月単位と年単位の請求について詳しくは、請求に関する [FAQ](https://docs.microsoft.com/partner-center/faq-about-new-billing-features) の記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-113">For more information about monthly vs. annual billing, see the billing [FAQ](https://docs.microsoft.com/partner-center/faq-about-new-billing-features).</span></span>

-   [<span data-ttu-id="1f1ab-114">使用量ベースの請求</span><span class="sxs-lookup"><span data-stu-id="1f1ab-114">Usage-based billing</span></span>](#usagebasedbilling)

    <span data-ttu-id="1f1ab-115">Azure サブスクリプションなどのオンラインサービスを購入すると、毎月の使用率に対して課金されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-115">When you buy online services such as Azure subscriptions, you're billed for monthly usage rates.</span></span> <span data-ttu-id="1f1ab-116">使用量ベースの製品の場合は、月単位の請求だけを利用できます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-116">Only monthly billing is available for usage-based products.</span></span> <span data-ttu-id="1f1ab-117">使用量ベースのサービス (Azure など) は、消費量に基づく従量制で請求されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-117">Usage-based services, such as Azure, are billed according to metered rates, based on consumption.</span></span>

-   [<span data-ttu-id="1f1ab-118">1 回限りの請求</span><span class="sxs-lookup"><span data-stu-id="1f1ab-118">One-time billing</span></span>](#onetimebilling)

    <span data-ttu-id="1f1ab-119">Azure Reservations または他のソフトウェア サブスクリプションを購入するときは、事前設定された期間について前払いします。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-119">When you buy Azure reservations or other software subscriptions, you pay in advance for a pre-set term.</span></span> <span data-ttu-id="1f1ab-120">事前に支払いを行っているので、1つの一括合計で課金されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-120">Because you're paying in advance, you're billed in one lump sum.</span></span> 
    
<span data-ttu-id="1f1ab-121">毎月の課金を選択した場合、または月ごとに課金される使用量ベースの製品を購入した場合、月々の請求日は、パートナーセンターで CSP アカウントを作成したときに選択した日付になります。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-121">If you've chosen to be billed monthly or if you've bought usage-based products that are billed monthly, your monthly billing date is the day of the month you selected when you created your CSP account on Partner Center.</span></span> <span data-ttu-id="1f1ab-122">CSP アカウントが正常に作成されると、Microsoft は請求日が記載された確認メールを送信します。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-122">After you've successfully created your CSP account, Microsoft will send a confirmation email that includes your billing date.</span></span> <span data-ttu-id="1f1ab-123">作成した後でこの日付を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-123">Once created, this date cannot be changed.</span></span> 

## <a name="pricing-and-invoicing"></a><span data-ttu-id="1f1ab-124">価格と請求</span><span class="sxs-lookup"><span data-stu-id="1f1ab-124">Pricing and invoicing</span></span>
<span data-ttu-id="1f1ab-125">価格表は毎月更新され、1 か月前に確認することができます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-125">You can find price lists one (1) month in advance, as they're updated monthly.</span></span> <span data-ttu-id="1f1ab-126">ライセンスベースの価格は、サブスクリプションの有効期間 (通常は購入日から 12 か月間) にわたって保証されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-126">License-based prices are guaranteed for the term of the subscription, usually 12 months from the purchase date.</span></span> <span data-ttu-id="1f1ab-127">使用量ベースの価格は、毎月変わる場合があります。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-127">Usage-based prices can change on a monthly basis.</span></span> 

<span data-ttu-id="1f1ab-128">製品、サービス、ソフトウェア サブスクリプションの価格はサブスクリプション期間を通して保証されますが、更新時に価格が変わる場合があります。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-128">Prices for products, services, and software subscriptions are guaranteed through the subscription duration, however prices may change when you renew.</span></span>

<span data-ttu-id="1f1ab-129">クレジットまたは調整が適用されると、次回の請求書に未払いの調整とクレジットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-129">You'll see adjustments and credits in arrears on your next billing invoice after the credit or adjustment is applied.</span></span>

<span data-ttu-id="1f1ab-130">請求書と調整ファイルは、パートナー センターの [請求書作成] ページで表示およびダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-130">You can view and download your invoices and reconciliation files from the Billing page in the Partner Center.</span></span> <span data-ttu-id="1f1ab-131">パートナー センターでは、選択した請求日の 4 日以内であれば、毎月の請求書を確認できます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-131">Note that monthly invoices are available on Partner Center within four (4) days of your selected billing date.</span></span>

## <a name="payment-terms"></a><span data-ttu-id="1f1ab-132">支払条件</span><span class="sxs-lookup"><span data-stu-id="1f1ab-132">Payment terms</span></span>

<span data-ttu-id="1f1ab-133">支払期間は正味 60 日です。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-133">Payment terms are net 60 days.</span></span> <span data-ttu-id="1f1ab-134">請求書の期限 (請求日から 60 日) までに支払う必要があります。それを過ぎると、アカウントは延滞になり、CSP での登録に影響する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-134">Invoices must be paid by the invoice due date (60 days after the billing date), or your account will be delinquent, which may impact your enrollment in CSP.</span></span> <span data-ttu-id="1f1ab-135">支払い期限の過ぎた未払い額を支払うと、中断されているアカウントのすべての機能を復旧できます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-135">You can regain full functionality of your suspended accounts when you pay the past due amount.</span></span>

### <a name="tax"></a><span data-ttu-id="1f1ab-136">Tax</span><span class="sxs-lookup"><span data-stu-id="1f1ab-136">Tax</span></span>

<span data-ttu-id="1f1ab-137">請求関係は Microsoft と (顧客ではなく) パートナーの間のものなので、パートナーの詳細に基づいてパートナーに課税されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-137">You are taxed based on your details, (not your customers') as the billing relationship is between Microsoft and you.</span></span> <span data-ttu-id="1f1ab-138">アカウントのセットアップ プロセス中に、または後でサポート要求を送信することで、税 ID を提出できます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-138">You can submit your tax ID during the account setup process or by submitting a support request later.</span></span> <span data-ttu-id="1f1ab-139">料金は次の課金サイクルに反映されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-139">You'll see the changes reflected on your next billing cycle.</span></span>

-   <span data-ttu-id="1f1ab-140">源泉徴収と売上税の除外については、サポート要求を通じて税金のドキュメントを提出する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-140">For withholding and sales tax exemption, you must submit tax documentation through a support request.</span></span> <span data-ttu-id="1f1ab-141">料金と適切な返金は次の課金サイクルに反映されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-141">You'll see the changes and appropriate refunds on your next billing cycle.</span></span>

-   <span data-ttu-id="1f1ab-142">付加価値税 (VAT) の免除については、サービス要求を通じて (Microsoft によって確認済みの)、VAT ID を提出する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-142">For value added tax (VAT) exemption, you must submit your VAT ID (validated by Microsoft) via a service request.</span></span> <span data-ttu-id="1f1ab-143">料金と適切な返金は次の課金サイクルに反映されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-143">You'll see the changes and appropriate refunds on your next billing cycle.</span></span>

<span data-ttu-id="1f1ab-144">さらに詳しい税金の詳細については、地域の税務署または税務アドバイザーにお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-144">You can find further tax details from your local tax office or tax advisor.</span></span>

## <a href="" id="licensebasedbilling"></a><span data-ttu-id="1f1ab-145">ライセンスベースの請求</span><span class="sxs-lookup"><span data-stu-id="1f1ab-145">License-based billing</span></span>

<span data-ttu-id="1f1ab-146">顧客に代わってライセンスベースの製品を購入するときに、月単位または年単位の請求を選択できます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-146">When you buy a license-based product on behalf of a customer, you can choose to be billed monthly or annually.</span></span> <span data-ttu-id="1f1ab-147">後で請求頻度を変更する場合は、以下の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-147">If you want to change your billing frequency at a later time, use the procedure below.</span></span> 

<span data-ttu-id="1f1ab-148">毎月請求されるサブスクリプションが多数あり、それらを共通の請求日にまとめたい場合は、月単位の請求から年単位の請求に切り替えると便利です。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-148">Switching from monthly billing to annual billing is useful if you have numerous subscriptions that are billed monthly and you want to align them to a common billing date.</span></span> <span data-ttu-id="1f1ab-149">個々の顧客の請求に合わせて請求日を調整するときは、年単位の請求から月単位の請求に切り替えると便利です。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-149">Switching from annual billing to monthly billing is useful in tailoring your billing dates to those of your individual customers.</span></span> 

<span data-ttu-id="1f1ab-150">請求頻度を変更すると、請求頻度を変更した日付を反映するように年間契約が更新され、新しい更新日が確立されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-150">When you change the billing frequency, the annual term is updated to reflect the date you changed the billing frequency and a new renewal date is established.</span></span> 

<span data-ttu-id="1f1ab-151">ビジネス ニーズが変化するたびに、請求頻度を変更できます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-151">You can change the billing frequency whenever your business needs change.</span></span> 

### <a name="billing-rules-for-annual-billing"></a><span data-ttu-id="1f1ab-152">年単位の請求の請求ルール</span><span class="sxs-lookup"><span data-stu-id="1f1ab-152">Billing rules for annual billing</span></span>

-   <span data-ttu-id="1f1ab-153">サブスクリプションは毎年自動更新されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-153">Subscriptions are annual and auto-renewed.</span></span>

-   <span data-ttu-id="1f1ab-154">請求は、年間サブスクリプションごとに 12 回の月払いまたは 1 回の年払いになります。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-154">Billing is in 12 monthly payments or one annual payment per annual subscription.</span></span>

-   <span data-ttu-id="1f1ab-155">前回の請求期間の終了時のライセンス数に基づき、ライセンスベースのサービスの次の請求期間分が前払いで請求されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-155">You are billed in advance for the next billing period for license-based services, based on number of licenses at the end of the prior billing period.</span></span>

-   <span data-ttu-id="1f1ab-156">ライセンス数の変更 (ライセンスの日数に基づく日割り計算) で、後で課金/クレジットが行われます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-156">You are billed/credited in arrears for any changes in the number of licenses(pro-rata calculation based on license-days).</span></span> <span data-ttu-id="1f1ab-157">日割り計算では、次の式を使用します。[ROUND((ROUND(単価 \* 数量 / 日割り計算の月の日数, 2) \* 日割り計算の日数) / 数量, 2) \* 数量]</span><span class="sxs-lookup"><span data-stu-id="1f1ab-157">Pro-rata calculation uses the following formula: [ROUND((ROUND(Unit Price \* Quantity / Number of days in pro-rated Month, 2) \* Number of pro-rated days) / Quantity, 2) \* Quantity]</span></span>

-   <span data-ttu-id="1f1ab-158">支払いは、(プロビジョニングされたライセンスではなく) 販売されたライセンスに対して請求されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-158">Payments are billed for licenses sold (not licenses provisioned).</span></span>

### <a name="to-change-the-billing-frequency-of-an-online-service"></a><span data-ttu-id="1f1ab-159">オンライン サービスの請求頻度を変更するには</span><span class="sxs-lookup"><span data-stu-id="1f1ab-159">To change the billing frequency of an online service</span></span>

1.  <span data-ttu-id="1f1ab-160">パートナー センターのメニューで **[顧客]** を選択し、サブスクリプションを変更する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-160">Select **Customers** from the Partner Center menu and then select the customer with the subscription you want to change.</span></span> 

2.  <span data-ttu-id="1f1ab-161">顧客のサブスクリプション ページで、変更するサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-161">On the customer's Subscriptions page, select the subscription you want to change.</span></span> 

3.  <span data-ttu-id="1f1ab-162">詳細ページの **[請求頻度]** で、 **[毎月]** または **[毎年]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-162">On the details page, under **Billing frequency**, select **Monthly** or **Annual**.</span></span> <span data-ttu-id="1f1ab-163">請求頻度の変更に関する重要な情報と、変更対象のサブスクリプションの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-163">You'll see a confirmation page with important information about changing billing frequency, as well as a list of the subscriptions about to be changed.</span></span> 

4.  <span data-ttu-id="1f1ab-164">**[OK]** を選択して変更するか、または **[キャンセル]** を選択して取り消します。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-164">Select **OK** to make the change, or **Cancel** to undo it.</span></span> 

### <a name="adjustmentscreditscancellations"></a><span data-ttu-id="1f1ab-165">調整/クレジット/取り消し</span><span class="sxs-lookup"><span data-stu-id="1f1ab-165">Adjustments/Credits/Cancellations</span></span>

<span data-ttu-id="1f1ab-166">ライセンスベースのサービスの取り消しに対して、早期終了手数料は課金されません。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-166">Microsoft does not charge early termination fees for cancellation of license-based services.</span></span> 

<span data-ttu-id="1f1ab-167">ライセンス ベースのサービスに対する取り消しのクレジットは、期間途中の取り消しについては未使用の日について日割り計算されます (前の式に従ったライセンスの減少も同様です)。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-167">Cancellation credits for licensed based services are pro-rated for unused days for mid-cycle cancellations (as well as license decreases per the formula above).</span></span>

## <a href="" id="usagebasedbilling"></a><span data-ttu-id="1f1ab-168">使用量ベースの請求</span><span class="sxs-lookup"><span data-stu-id="1f1ab-168">Usage-based billing</span></span>

<span data-ttu-id="1f1ab-169">Microsoft の一部の製品とサービスでは "従量課金制" の請求モデルが使用されており、使用したサービスに対してのみ請求されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-169">Some Microsoft products and services use a "pay as you go" billing model, in which you are billed only for services used.</span></span> <span data-ttu-id="1f1ab-170">たとえば、Microsoft Azure ではこのモデルが使われています。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-170">For example, Microsoft Azure uses this model.</span></span> 

### <a name="billing-rules"></a><span data-ttu-id="1f1ab-171">課金の規則</span><span class="sxs-lookup"><span data-stu-id="1f1ab-171">Billing rules</span></span>
-   <span data-ttu-id="1f1ab-172">サブスクリプションは新しい従量制サービスの料金で、毎月自動的に更新されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-172">Subscriptions are month-to-month and automatically renew at the new metered service rates.</span></span> <span data-ttu-id="1f1ab-173">毎月、前月の使用量に対して請求されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-173">You're billed each month for the previous month's usage.</span></span>

-   <span data-ttu-id="1f1ab-174">従量制サービスの料金は、請求サイクル内で変更される場合があります。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-174">Metered service rates can change within the invoice cycle.</span></span> 

    -   <span data-ttu-id="1f1ab-175">価格の増加: 30 日前に通知されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-175">Price increases: 30 days' notice is provided.</span></span>

    -   <span data-ttu-id="1f1ab-176">価格の低下: 変更日を反映します。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-176">Price decreases: reflected day of change.</span></span>

    -   <span data-ttu-id="1f1ab-177">既存のサブスクリプションでは、課金サイクルの開始時点で有効な料金が使われます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-177">Existing subscriptions use the rate in effect at the beginning of the bill cycle.</span></span>

    -   <span data-ttu-id="1f1ab-178">同じ請求サイクル内で作成される新しいサブスクリプションでは、作成日に有効なレートが使用されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-178">New subscriptions, when created within the same billing cycle, use the rate in effect on the date you create them.</span></span> 

### <a name="adjustmentscreditscancellations"></a><span data-ttu-id="1f1ab-179">調整/クレジット/取り消し</span><span class="sxs-lookup"><span data-stu-id="1f1ab-179">Adjustments/Credits/Cancellations</span></span>

<span data-ttu-id="1f1ab-180">支払いの調整は、次の月次請求書に表示されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-180">You'll see payments with adjustments on your next monthly billing invoice.</span></span>

<span data-ttu-id="1f1ab-181">使用量ベースのサービスの取り消しに対して、早期終了手数料は課金されません。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-181">Microsoft does not charge early termination fees for cancellation of usage-based services.</span></span> 

<span data-ttu-id="1f1ab-182">SLA のクレジットを含むあらゆる種類のクレジットが、次の月次請求書に表示されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-182">You'll see credits of any type, including SLA credits, on your next monthly billing invoice.</span></span>

## <a href="" id="onetimebilling"></a><span data-ttu-id="1f1ab-183">1 回限りの請求</span><span class="sxs-lookup"><span data-stu-id="1f1ab-183">One-time billing</span></span>

<span data-ttu-id="1f1ab-184">ソフトウェア サブスクリプションと Azure Reservations は、1 年または 3 年の期間で事前に購入することができます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-184">You can purchase software subscriptions and Azure reservations in advance, for one- or three-year terms.</span></span> <span data-ttu-id="1f1ab-185">事前に購入すると、全体のコストが一括で請求されます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-185">When you purchase in advance, you're billed for the entire cost in a one-lump sum.</span></span> <span data-ttu-id="1f1ab-186">この種類の請求は、1 回限りの請求と呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-186">This type of billing is called one-time billing.</span></span>

>[!IMPORTANT]
><span data-ttu-id="1f1ab-187">お客様とは異なる通貨を使用している顧客に対して Azure の予約やソフトウェアのサブスクリプションを購入した場合、既定の請求通貨は、お客様の所在地ではなく顧客の所在地に基づきます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-187">If you purchase Azure reservations and/or software subscriptions for a customer in a location with a currency different from yours, the default billing currency is based on the customer's location, not your location.</span></span> <span data-ttu-id="1f1ab-188">複数の場所に顧客がいる場合は、顧客が課金される必要がある通貨ごとに個別の請求書と調整ファイルを受け取り、適切な通貨で顧客の請求を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-188">If you have customers in multiple locations, you'll receive separate invoices and reconciliation files for each currency customers need to be billed in, allowing you to invoice your customers in the appropriate currency.</span></span> 

### <a name="manage-your-one-time-billing"></a><span data-ttu-id="1f1ab-189">1 回限りの請求を管理する</span><span class="sxs-lookup"><span data-stu-id="1f1ab-189">Manage your one-time billing</span></span>

<span data-ttu-id="1f1ab-190">**現在の請求の状態、請求書、調整ファイルを表示する**</span><span class="sxs-lookup"><span data-stu-id="1f1ab-190">**View your current billing status, invoices, and recon files**</span></span>

1.  <span data-ttu-id="1f1ab-191">パートナー センターで **[Billing]\(請求\)** 、 **[1 回限り]** の順に選択して、請求の状態を表示します。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-191">In Partner Center, select **Billing** and then **One time** to view your billing status.</span></span> 

2.  <span data-ttu-id="1f1ab-192">請求書または調整ファイルを選択して、詳細な情報を確認します。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-192">Select an invoice or recon file to view more detailed information.</span></span> 

<span data-ttu-id="1f1ab-193">**顧客の注文履歴を表示する**</span><span class="sxs-lookup"><span data-stu-id="1f1ab-193">**View a customer's order history**</span></span>

1.  <span data-ttu-id="1f1ab-194">パートナー センター メニューで、 **[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-194">Select **Customers** from the Partner Center menu.</span></span>

2.  <span data-ttu-id="1f1ab-195">**顧客**のページで、注文履歴を表示する顧客を見つけて、下矢印を選択して顧客のレコードを展開します。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-195">On your **Customers** page, find the customer whose order history you want to view and then select the down arrow to expand the customer's record.</span></span> 

3.  <span data-ttu-id="1f1ab-196">**[View orders]** (注文の表示) を選択して注文履歴を表示します。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-196">Select **View orders** to display the order history.</span></span>

<span data-ttu-id="1f1ab-197">**クレジット ノートをダウンロードする**</span><span class="sxs-lookup"><span data-stu-id="1f1ab-197">**Download a credit note**</span></span>

<span data-ttu-id="1f1ab-198">クレジットまたは再請求を要求する必要がある場合は、元の請求書をキャンセルするためのクレジットメモをお送りします。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-198">If you need to request a credit or rebill, we'll give you a credit note to cancel the original invoice.</span></span> <span data-ttu-id="1f1ab-199">次のような理由でクレジット/再請求を要求する場合があります。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-199">You might request a credit/rebill for the following reasons:</span></span>

-   <span data-ttu-id="1f1ab-200">請求先住所または発注書の訂正</span><span class="sxs-lookup"><span data-stu-id="1f1ab-200">Address or purchase order corrections</span></span>

-   <span data-ttu-id="1f1ab-201">請求書が生成された後、税金の払い戻しが適用された場合。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-201">Invoice generated and then a tax refund was applied.</span></span> <span data-ttu-id="1f1ab-202">クレジット/再請求を要求して、元の請求書に税金の払い戻しを反映させることができます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-202">You can request a credit/rebill to get the tax refund pulled back into the original invoice.</span></span> <span data-ttu-id="1f1ab-203">これは払い戻しの場合にも適用され、元の請求書のクレジット/再請求を要求し、払い戻しを受けることができます。</span><span class="sxs-lookup"><span data-stu-id="1f1ab-203">This is also true for refunds, as you can request a credit/rebill of the original invoice and then pull in a refund.</span></span>
