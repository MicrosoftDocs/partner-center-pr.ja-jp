---
title: 請求の概要 |パートナー センター
ms.topic: article
ms.date: 10/29/2018
Description: Information on basic billing scenarios and the differences between license-based and usage-based billing
author: labrenne
ms.author: labrenne
keywords: 請求, 支払い,注文,取り消し, 注文管理, 未払い, 詐欺, 不正使用, 税, 税額控除, 調整ファイル, 調整用のファイル
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 96a859fda2ba8641c701888c4a865b1a1278c268
ms.sourcegitcommit: 777225c8bf16e4a8811a9d88aceb45fcba1cd959
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/11/2018
ms.locfileid: "8917604"
---
# <a name="billing-overview"></a><span data-ttu-id="55745-103">請求の概要</span><span class="sxs-lookup"><span data-stu-id="55745-103">Billing overview</span></span>

**<span data-ttu-id="55745-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="55745-104">Applies to</span></span>**

-  <span data-ttu-id="55745-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="55745-105">Partner Center</span></span>
-  <span data-ttu-id="55745-106">CSP プログラムのパートナー</span><span class="sxs-lookup"><span data-stu-id="55745-106">Partners in the CSP program</span></span>

<span data-ttu-id="55745-107">によっては、製品、ソリューションとサービスの顧客に代わって購入するには、次の方法の 1 つ以上でこれらの購入料金が請求されます。</span><span class="sxs-lookup"><span data-stu-id="55745-107">Depending on the products, solutions, and services you buy on behalf of your customers, you’ll be billed for these purchases in one or more of the following ways:</span></span>
-   [<span data-ttu-id="55745-108">ライセンス ベースの課金</span><span class="sxs-lookup"><span data-stu-id="55745-108">License-based billing</span></span>](#licensebasedbilling)

    <span data-ttu-id="55745-109">製品またはライセンスを必要とするオンライン サービスを購入した場合 (ライセンスの使用状況) ではなく購入した各ライセンスの料金を請求します。</span><span class="sxs-lookup"><span data-stu-id="55745-109">When you buy products or online services that require licenses, you’re billed for each license you bought (not on license usage).</span></span> <span data-ttu-id="55745-110">1 か月に 1 回または年間に 1 回請求するかどうかを選択できます。</span><span class="sxs-lookup"><span data-stu-id="55745-110">You can choose whether to be billed once a month or once a year.</span></span> <span data-ttu-id="55745-111">お客様のビジネス ニーズが変化する場合、他のいずれかからの切り替えし、再びできます。</span><span class="sxs-lookup"><span data-stu-id="55745-111">If your business needs change, you can switch from one to the other and back again.</span></span> 
    
    <span data-ttu-id="55745-112">年次請求と月次について詳しくは、請求の[よく寄せられる質問](https://docs.microsoft.com/en-us/partner-center/faq-about-new-billing-features)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55745-112">For more information about monthly vs. annual billing, see the billing [FAQ](https://docs.microsoft.com/en-us/partner-center/faq-about-new-billing-features).</span></span>

-   [<span data-ttu-id="55745-113">使用量ベースの課金</span><span class="sxs-lookup"><span data-stu-id="55745-113">Usage-based billing</span></span>](#usagebasedbilling)

    <span data-ttu-id="55745-114">Azure サブスクリプションなどのオンライン サービスを購入した場合は、月次請求の使用率の請求しています。</span><span class="sxs-lookup"><span data-stu-id="55745-114">When you buy online services such as Azure subscriptions, you’re billed for monthly usage rates.</span></span> <span data-ttu-id="55745-115">のみ月次請求は、製品の使用量ベースの使用できます。</span><span class="sxs-lookup"><span data-stu-id="55745-115">Only monthly billing is available for usage-based products.</span></span> <span data-ttu-id="55745-116">Azure など使用量ベースのサービスは、使用に基づいて従量制課金されます。</span><span class="sxs-lookup"><span data-stu-id="55745-116">Usage-based services, such as Azure, are billed according to metered rates, based on consumption.</span></span>

-   [<span data-ttu-id="55745-117">1 回限りの請求</span><span class="sxs-lookup"><span data-stu-id="55745-117">One-time billing</span></span>](#onetimebilling)

    <span data-ttu-id="55745-118">Azure 予約またはその他のソフトウェア サブスクリプションを購入した場合は、事前に定義された期間の事前に支払い。</span><span class="sxs-lookup"><span data-stu-id="55745-118">When you buy Azure reservations or other software subscriptions, you pay in advance for a pre-set term.</span></span> <span data-ttu-id="55745-119">事前に、料金を支払っているためには、一括の 1 つに請求します。</span><span class="sxs-lookup"><span data-stu-id="55745-119">Because you’re paying in advance, you’re billed in one lump sum.</span></span> 
    
<span data-ttu-id="55745-120">月次請求を選択した場合、または月次請求は使用量ベースの製品を購入した場合は、月次請求日は、パートナー センターでの CSP アカウントを作成する際に選択するか月の日です。</span><span class="sxs-lookup"><span data-stu-id="55745-120">If you’ve chosen to be billed monthly or if you’ve bought usage-based products that are billed monthly, your monthly billing date is the day of the month you selected when you created your CSP account on Partner Center.</span></span> <span data-ttu-id="55745-121">CSP アカウントが正常に作成したら、Microsoft には、請求日が含まれている確認メールが送信されます。</span><span class="sxs-lookup"><span data-stu-id="55745-121">After you’ve successfully created your CSP account, Microsoft will send a confirmation email that includes your billing date.</span></span>

## <a name="pricing-and-invoicing"></a><span data-ttu-id="55745-122">[料金と請求</span><span class="sxs-lookup"><span data-stu-id="55745-122">Pricing and invoicing</span></span>
<span data-ttu-id="55745-123">価格表は毎月更新され、1 か月前に確認することができます。</span><span class="sxs-lookup"><span data-stu-id="55745-123">You can find price lists one (1) month in advance, as they're updated monthly.</span></span> <span data-ttu-id="55745-124">ライセンスベースの価格は、サブスクリプションの有効期間 (通常は購入日から 12 か月間) にわたって保証されます。</span><span class="sxs-lookup"><span data-stu-id="55745-124">License-based prices are guaranteed for the term of the subscription, usually 12 months from the purchase date.</span></span> <span data-ttu-id="55745-125">使用量ベースの価格は、毎月変わる場合があります。</span><span class="sxs-lookup"><span data-stu-id="55745-125">Usage-based prices can change on a monthly basis.</span></span> 

<span data-ttu-id="55745-126">製品、サービス、およびソフトウェア サブスクリプションの価格は、更新すると、価格を変更することがありますが、サブスクリプション期間を通じて保証されます。</span><span class="sxs-lookup"><span data-stu-id="55745-126">Prices for products, services, and software subscriptions are guaranteed through the subscription duration, however prices may change when you renew.</span></span>

<span data-ttu-id="55745-127">クレジットまたは調整が適用されると、次回の請求書に未払いの調整とクレジットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="55745-127">You'll see adjustments and credits in arrears on your next billing invoice after the credit or adjustment is applied.</span></span>

<span data-ttu-id="55745-128">請求書と調整ファイルは、パートナー センターの課金ページで表示およびダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="55745-128">You can view and download your invoices and reconciliation files from the Billing page in the Partner Center.</span></span> <span data-ttu-id="55745-129">パートナー センターでは、選択した請求日の 4 日以内であれば、毎月の請求書を確認できます。</span><span class="sxs-lookup"><span data-stu-id="55745-129">Note that monthly invoices are available on Partner Center within four (4) days of your selected billing date.</span></span>

## <a name="payment-terms"></a><span data-ttu-id="55745-130">支払条件</span><span class="sxs-lookup"><span data-stu-id="55745-130">Payment terms</span></span>

<span data-ttu-id="55745-131">支払条件は、net 60 日間です。</span><span class="sxs-lookup"><span data-stu-id="55745-131">Payment terms are net 60 days.</span></span> <span data-ttu-id="55745-132">請求書支払う必要がある期限 (請求日後 60 日)、または自分のアカウントの請求書が延滞、CSP への登録に影響する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="55745-132">Invoices must be paid by the invoice due date (60 days after the billing date), or your account will be delinquent, which may impact your enrollment in CSP.</span></span> <span data-ttu-id="55745-133">過去の支払時に、中断されたアカウントのすべての機能を回復できます期限金額。</span><span class="sxs-lookup"><span data-stu-id="55745-133">You can regain full functionality of your suspended accounts when you pay the past due amount.</span></span>

### <a name="tax"></a><span data-ttu-id="55745-134">税金</span><span class="sxs-lookup"><span data-stu-id="55745-134">Tax</span></span>

<span data-ttu-id="55745-135">ベースの詳細については、(顧客ではなく) に課税はは請求関係は Microsoft と貴社の間です。</span><span class="sxs-lookup"><span data-stu-id="55745-135">You are taxed based on your details, (not your customers') as the billing relationship is between Microsoft and you.</span></span> <span data-ttu-id="55745-136">アカウントのセットアップ プロセス中に、または後でサポート要求を送信することで、税金 ID を提出することができます。</span><span class="sxs-lookup"><span data-stu-id="55745-136">You can submit your tax ID during the account setup process or by submitting a support request later.</span></span> <span data-ttu-id="55745-137">料金は次の課金サイクルに反映されます。</span><span class="sxs-lookup"><span data-stu-id="55745-137">You'll see the changes reflected on your next billing cycle.</span></span>

-   <span data-ttu-id="55745-138">源泉徴収と売上税の除外は、サポート要求を通じて税金のドキュメントを提出する必要があります。</span><span class="sxs-lookup"><span data-stu-id="55745-138">For withholding and sales tax exemption, you must submit tax documentation through a support request.</span></span> <span data-ttu-id="55745-139">料金と適切な返金は次の課金サイクルに反映されます。</span><span class="sxs-lookup"><span data-stu-id="55745-139">You'll see the changes and appropriate refunds on your next billing cycle.</span></span>

-   <span data-ttu-id="55745-140">付加価値税 (VAT) の免除については、サービス要求を通じて (Microsoft によって確認済みの)、VAT ID を提出する必要があります。</span><span class="sxs-lookup"><span data-stu-id="55745-140">For value added tax (VAT) exemption, you must submit your VAT ID (validated by Microsoft) via a service request.</span></span> <span data-ttu-id="55745-141">料金と適切な返金は次の課金サイクルに反映されます。</span><span class="sxs-lookup"><span data-stu-id="55745-141">You'll see the changes and appropriate refunds on your next billing cycle.</span></span>

<span data-ttu-id="55745-142">税の詳細については、地域の税務署または税務アドバイザーをさらに検索することができます。</span><span class="sxs-lookup"><span data-stu-id="55745-142">You can find further tax details from your local tax office or tax advisor.</span></span>

## <a href="" id="licensebasedbilling"></a><span data-ttu-id="55745-143">ライセンス ベースの課金</span><span class="sxs-lookup"><span data-stu-id="55745-143">License-based billing</span></span>

<span data-ttu-id="55745-144">顧客の代理としてのライセンス ベースの製品を購入した場合は、月次または年次請求を選択できます。</span><span class="sxs-lookup"><span data-stu-id="55745-144">When you buy a license-based product on behalf of a customer, you can choose to be billed monthly or annually.</span></span> <span data-ttu-id="55745-145">後で、請求頻度を変更する場合は、次の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="55745-145">If you want to change your billing frequency at a later time, use the procedure below.</span></span> 

<span data-ttu-id="55745-146">月次請求は多数のサブスクリプションがあり、一般的な請求日に揃えたりする場合は、月次請求から年次請求に切り替えると便利です。</span><span class="sxs-lookup"><span data-stu-id="55745-146">Switching from monthly billing to annual billing is useful if you have numerous subscriptions that are billed monthly and you want to align them to a common billing date.</span></span> <span data-ttu-id="55745-147">月次請求を年次請求に切り替えることは、個々 のお客様の請求日の調整に便利です。</span><span class="sxs-lookup"><span data-stu-id="55745-147">Switching from annual billing to monthly billing is useful in tailoring your billing dates to those of your individual customers.</span></span> 

<span data-ttu-id="55745-148">請求頻度を変更すると、年次という用語が請求頻度を変更した日付と新しい更新日の確立を反映するように更新されます。</span><span class="sxs-lookup"><span data-stu-id="55745-148">When you change the billing frequency, the annual term is updated to reflect the date you changed the billing frequency and a new renewal date is established.</span></span> 

<span data-ttu-id="55745-149">ビジネス ニーズ変更されるたびに、請求頻度を変更できます。</span><span class="sxs-lookup"><span data-stu-id="55745-149">You can change the billing frequency whenever your business needs change.</span></span> 

### <a name="billing-rules-for-annual-billing"></a><span data-ttu-id="55745-150">年次請求の課金の規則</span><span class="sxs-lookup"><span data-stu-id="55745-150">Billing rules for annual billing</span></span>

-   <span data-ttu-id="55745-151">サブスクリプションは毎年自動更新されます。</span><span class="sxs-lookup"><span data-stu-id="55745-151">Subscriptions are annual and auto-renewed.</span></span>

-   <span data-ttu-id="55745-152">課金は、12 か月の支払いまたは 1 つの年次支払い年間サブスクリプションごとにします。</span><span class="sxs-lookup"><span data-stu-id="55745-152">Billing is in 12 monthly payments or one annual payment per annual subscription.</span></span>

-   <span data-ttu-id="55745-153">以前の課金期間の終了時のライセンス数に基づいて、ライセンス ベースのサービスの次の課金期間について前払いで課金されます。</span><span class="sxs-lookup"><span data-stu-id="55745-153">You are billed in advance for the next billing period for license-based services, based on number of licenses at the end of the prior billing period.</span></span>

-   <span data-ttu-id="55745-154">ライセンス数の変更 (ライセンスの日数に基づく日割り計算) で、後で課金/クレジットが行われます。</span><span class="sxs-lookup"><span data-stu-id="55745-154">You are billed/credited in arrears for any changes in the number of licenses(pro-rata calculation based on license-days).</span></span> <span data-ttu-id="55745-155">日割り計算では、次の式を使用します。[ROUND((ROUND(単価 \* 数量 / 日割り計算の月の日数, 2) \* 日割り計算の日数) / 数量, 2) \* 数量]</span><span class="sxs-lookup"><span data-stu-id="55745-155">Pro-rata calculation uses the following formula: [ROUND((ROUND(Unit Price \* Quantity / Number of days in pro-rated Month, 2) \* Number of pro-rated days) / Quantity, 2) \* Quantity]</span></span>

-   <span data-ttu-id="55745-156">販売 (ライセンス プロビジョニングではない) のライセンスは、支払いが課金されます。</span><span class="sxs-lookup"><span data-stu-id="55745-156">Payments are billed for licenses sold (not licenses provisioned).</span></span>

### <a name="to-change-the-billing-frequency-of-an-online-service"></a><span data-ttu-id="55745-157">オンライン サービスの請求頻度を変更するには</span><span class="sxs-lookup"><span data-stu-id="55745-157">To change the billing frequency of an online service</span></span>

1.  <span data-ttu-id="55745-158">パートナー センター メニューから**顧客**を選択し、サブスクリプションを変更する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="55745-158">Select **Customers** from the Partner Center menu and then select the customer with the subscription you want to change.</span></span> 

2.  <span data-ttu-id="55745-159">顧客のサブスクリプションのページを変更するサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="55745-159">On the customer's Subscriptions page, select the subscription you want to change.</span></span> 

3.  <span data-ttu-id="55745-160">[詳細] ページの [**請求頻度**を**月次請求**または**年次**を選択します。</span><span class="sxs-lookup"><span data-stu-id="55745-160">On the details page, under **Billing frequency**, select **Monthly** or **Annual**.</span></span> <span data-ttu-id="55745-161">請求頻度は、できるだけを変更するサブスクリプションの一覧の変更に関する重要な情報の確認ページが表示されます。</span><span class="sxs-lookup"><span data-stu-id="55745-161">You’ll see a confirmation page with important information about changing billing frequency, as well as a list of the subscriptions about to be changed.</span></span> 

4.  <span data-ttu-id="55745-162">変更を加えるには、 **[ok]** または元に戻すこと**をキャンセル**を選択します。</span><span class="sxs-lookup"><span data-stu-id="55745-162">Select **OK** to make the change, or **Cancel** to undo it.</span></span> 

### <a name="adjustmentscreditscancellations"></a><span data-ttu-id="55745-163">調整/クレジット/取り消し</span><span class="sxs-lookup"><span data-stu-id="55745-163">Adjustments/Credits/Cancellations</span></span>

<span data-ttu-id="55745-164">Microsoft は、ライセンス ベース サービスの取り消しに対して終了早期の料金を課金しません。</span><span class="sxs-lookup"><span data-stu-id="55745-164">Microsoft does not charge early termination fees for cancellation of license-based services.</span></span> 

<span data-ttu-id="55745-165">ライセンス ベースのサービスに対する取り消しのクレジットは、期間途中の取り消しについては未使用の日について日割り計算されます (前の式に従ったライセンスの減少も同様です)。</span><span class="sxs-lookup"><span data-stu-id="55745-165">Cancellation credits for licensed based services are pro-rated for unused days for mid-cycle cancellations (as well as license decreases per the formula above).</span></span>

## <a href="" id="usagebasedbilling"></a><span data-ttu-id="55745-166">使用量ベースの課金</span><span class="sxs-lookup"><span data-stu-id="55745-166">Usage-based billing</span></span>

<span data-ttu-id="55745-167">一部の Microsoft 製品とサービスを使用したサービスについてのみ課金されます、「従量」請求モデルを使用します。</span><span class="sxs-lookup"><span data-stu-id="55745-167">Some Microsoft products and services use a "pay as you go" billing model, in which you are billed only for services used.</span></span> <span data-ttu-id="55745-168">たとえば、Microsoft Azure は、このモデルを使用します。</span><span class="sxs-lookup"><span data-stu-id="55745-168">For example, Microsoft Azure uses this model.</span></span> 

### <a name="billing-rules"></a><span data-ttu-id="55745-169">課金の規則</span><span class="sxs-lookup"><span data-stu-id="55745-169">Billing rules</span></span>
-   <span data-ttu-id="55745-170">サブスクリプションは月単位と、新しい従量制サービスの料金で自動的に更新します。</span><span class="sxs-lookup"><span data-stu-id="55745-170">Subscriptions are month-to-month and automatically renew at the new metered service rates.</span></span> <span data-ttu-id="55745-171">前月の使用状況について、毎月の請求をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="55745-171">You're billed each month for the previous month's usage.</span></span>

-   <span data-ttu-id="55745-172">従量制サービスの料金は、請求サイクル内で変更される場合があります。</span><span class="sxs-lookup"><span data-stu-id="55745-172">Metered service rates can change within the invoice cycle.</span></span> 

    -   <span data-ttu-id="55745-173">価格の増加: 30 日前に通知されます。</span><span class="sxs-lookup"><span data-stu-id="55745-173">Price increases: 30 days' notice is provided.</span></span>

    -   <span data-ttu-id="55745-174">価格の低下: 変更日を反映します。</span><span class="sxs-lookup"><span data-stu-id="55745-174">Price decreases: reflected day of change.</span></span>

    -   <span data-ttu-id="55745-175">既存のサブスクリプションでは、課金サイクルの開始時点で有効な料金が使われます。</span><span class="sxs-lookup"><span data-stu-id="55745-175">Existing subscriptions use the rate in effect at the beginning of the bill cycle.</span></span>

    -   <span data-ttu-id="55745-176">新しいサブスクリプションを同じの請求サイクル内で作成されたときは、作成日に有効で、レートを使用します。</span><span class="sxs-lookup"><span data-stu-id="55745-176">New subscriptions, when created within the same billing cycle, use the rate in effect on the date you create them.</span></span> 

### <a name="adjustmentscreditscancellations"></a><span data-ttu-id="55745-177">調整/クレジット/取り消し</span><span class="sxs-lookup"><span data-stu-id="55745-177">Adjustments/Credits/Cancellations</span></span>

<span data-ttu-id="55745-178">支払いの調整は、次の月次請求書に表示されます。</span><span class="sxs-lookup"><span data-stu-id="55745-178">You'll see payments with adjustments on your next monthly billing invoice.</span></span>

<span data-ttu-id="55745-179">Microsoft は、使用量ベースのサービスの取り消しに対して終了早期の料金を課金しません。</span><span class="sxs-lookup"><span data-stu-id="55745-179">Microsoft does not charge early termination fees for cancellation of usage-based services.</span></span> 

<span data-ttu-id="55745-180">SLA のクレジットを含むあらゆる種類のクレジットが、次の月次請求書に表示されます。</span><span class="sxs-lookup"><span data-stu-id="55745-180">You'll see credits of any type, including SLA credits, on your next monthly billing invoice.</span></span>

## <a href="" id="onetimebilling"></a><span data-ttu-id="55745-181">1 回限りの請求</span><span class="sxs-lookup"><span data-stu-id="55745-181">One-time billing</span></span>

<span data-ttu-id="55745-182">1 年または 3 年の用語のソフトウェア サブスクリプションと Azure reservations を事前に購入できます。</span><span class="sxs-lookup"><span data-stu-id="55745-182">You can purchase software subscriptions and Azure reservations in advance, for one- or three-year terms.</span></span> <span data-ttu-id="55745-183">事前に購入すると、1 つ一括で全体のコストの料金を請求しています。</span><span class="sxs-lookup"><span data-stu-id="55745-183">When you purchase in advance, you're billed for the entire cost in a one-lump sum.</span></span> <span data-ttu-id="55745-184">この種類の請求には、1 回限りの請求が呼び出されます。</span><span class="sxs-lookup"><span data-stu-id="55745-184">This type of billing is called one-time billing.</span></span>

>[!IMPORTANT]
><span data-ttu-id="55745-185">Azure reservations や通貨が異なるとの位置で顧客のソフトウェア サブスクリプションを購入した場合、既定の請求通貨は、場所ではなく、顧客の場所にベースします。</span><span class="sxs-lookup"><span data-stu-id="55745-185">If you purchase Azure reservations and/or software subscriptions for a customer in a location with a currency different from yours, the default billing currency is based on the customer’s location, not your location.</span></span> <span data-ttu-id="55745-186">お客様が複数の場所である、個別の請求書し、各通貨についての調整ファイルに請求する必要が、適切な通貨で顧客に請求することができます。</span><span class="sxs-lookup"><span data-stu-id="55745-186">If you have customers in multiple locations, you’ll receive separate invoices and reconciliation files for each currency customers need to be billed in, allowing you to invoice your customers in the appropriate currency.</span></span> 

### <a name="manage-your-one-time-billing"></a><span data-ttu-id="55745-187">1 回限りの請求を管理する</span><span class="sxs-lookup"><span data-stu-id="55745-187">Manage your one-time billing</span></span>

**<span data-ttu-id="55745-188">現在の請求の状態、請求書、調整ファイルを表示する</span><span class="sxs-lookup"><span data-stu-id="55745-188">View your current billing status, invoices, and recon files</span></span>**

1.  <span data-ttu-id="55745-189">パートナー センターで、**請求**とを選択し、 **1 回**して請求の状態を表示します。</span><span class="sxs-lookup"><span data-stu-id="55745-189">In Partner Center, select **Billing** and then **One time** to view your billing status.</span></span> 

2.  <span data-ttu-id="55745-190">請求書または調整ファイルを選択して、詳細な情報を確認します。</span><span class="sxs-lookup"><span data-stu-id="55745-190">Select an invoice or recon file to view more detailed information.</span></span> 

**<span data-ttu-id="55745-191">顧客の注文履歴を表示する</span><span class="sxs-lookup"><span data-stu-id="55745-191">View a customer’s order history</span></span>**

1.  <span data-ttu-id="55745-192">パートナー センター メニューから**顧客**を選択します。</span><span class="sxs-lookup"><span data-stu-id="55745-192">Select **Customers** from the Partner Center menu.</span></span>

2.  <span data-ttu-id="55745-193">**[顧客]** ページで、注文履歴を表示する対象の顧客を見つけ、下矢印を選択して顧客レコードを展開します。</span><span class="sxs-lookup"><span data-stu-id="55745-193">On your **Customers** page, find the customer whose order history you want to view and then select the down arrow to expand the customer’s record.</span></span> 

3.  <span data-ttu-id="55745-194">**[View orders]** (注文の表示) を選択して注文履歴を表示します。</span><span class="sxs-lookup"><span data-stu-id="55745-194">Select **View orders** to display the order history.</span></span>

**<span data-ttu-id="55745-195">クレジット メモをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="55745-195">Download a credit note</span></span>**

<span data-ttu-id="55745-196">クレジット_カードまたは再請求額を要求する必要がある場合紹介する元の請求書をキャンセルするクレジット メモします。</span><span class="sxs-lookup"><span data-stu-id="55745-196">If you need to request a credit or rebill, we’ll give you a credit note to cancel the original invoice.</span></span> <span data-ttu-id="55745-197">次の理由でクレジット/再請求額を要求する場合があります。</span><span class="sxs-lookup"><span data-stu-id="55745-197">You might request a credit/rebill for the following reasons:</span></span>

-   <span data-ttu-id="55745-198">アドレスまたは購入順序の修正</span><span class="sxs-lookup"><span data-stu-id="55745-198">Address or purchase order corrections</span></span>

-   <span data-ttu-id="55745-199">請求書が生成され、税払い戻しの適用されます。</span><span class="sxs-lookup"><span data-stu-id="55745-199">Invoice generated and then a tax refund was applied.</span></span> <span data-ttu-id="55745-200">元の請求書に課税払い戻しを取得するのには、クレジット/再を要求することができます。</span><span class="sxs-lookup"><span data-stu-id="55745-200">You can request a credit/rebill to get the tax refund pulled back into the original invoice.</span></span> <span data-ttu-id="55745-201">これは返金を true に設定を元の請求書とし、払い戻しでプルのクレジット/再請求を要求することができます。</span><span class="sxs-lookup"><span data-stu-id="55745-201">This is also true for refunds, as you can request a credit/rebill of the original invoice and then pull in a refund.</span></span>
