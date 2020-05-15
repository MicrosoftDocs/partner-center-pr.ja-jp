---
title: パートナーセンターで顧客のサブスクリプションを作成する
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft が発行した製品や、サードパーティの Isv によって発行された SaaS 製品に対して顧客のサブスクリプションを販売する方法について説明します。
ms.assetid: E95F1538-60E1-464C-B72B-52764BF3A820
author: LauraBrenner
ms.author: labrenne
ms.custom: SEOAPR.20
Keywords: サブスクリプション、新規作成、サブスクリプションの追加、中断、キャンセル、中断、中断、SaaS、ライセンス、ISV、サードパーティ
ms.localizationpriority: medium
ms.openlocfilehash: 969093b1ce3ba6936800ea91fd066d73b51701c7
ms.sourcegitcommit: 093039319fab2a44ab147159bc4be832f1330d57
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/14/2020
ms.locfileid: "83394152"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="4ad5f-104">顧客のサブスクリプションの作成、中断、取り消し</span><span class="sxs-lookup"><span data-stu-id="4ad5f-104">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="4ad5f-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="4ad5f-105">**Applies to**</span></span>

- <span data-ttu-id="4ad5f-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="4ad5f-106">Partner Center</span></span>
- <span data-ttu-id="4ad5f-107">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="4ad5f-107">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="4ad5f-108">CSP パートナー</span><span class="sxs-lookup"><span data-stu-id="4ad5f-108">CSP partners</span></span>

<span data-ttu-id="4ad5f-109">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="4ad5f-109">**Appropriate roles**</span></span>

- <span data-ttu-id="4ad5f-110">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="4ad5f-110">Admin agent</span></span>
- <span data-ttu-id="4ad5f-111">課金管理者</span><span class="sxs-lookup"><span data-stu-id="4ad5f-111">Billing admin</span></span>
- <span data-ttu-id="4ad5f-112">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="4ad5f-112">Global admin</span></span>
- <span data-ttu-id="4ad5f-113">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="4ad5f-113">Helpdesk agent</span></span>
- <span data-ttu-id="4ad5f-114">販売代理店</span><span class="sxs-lookup"><span data-stu-id="4ad5f-114">Sales agent</span></span>

<span data-ttu-id="4ad5f-115">パートナー センターで顧客のレコードを作成したら、カタログ内の製品へのサブスクリプションを販売できます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-115">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="4ad5f-116">これには、Microsoft によって発行された製品と、サードパーティ製の独立系ソフトウェアベンダー (Isv) によって[商用マーケットプレース](https://azuremarketplace.microsoft.com/marketplace)に発行されたサービスとしてのソフトウェア (SaaS) 製品が含まれます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-116">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="4ad5f-117">一部のプランは、顧客ごとに1つのサブスクリプションに限定されます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-117">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="4ad5f-118">制限のあるオファーの一覧を確認するには、パートナー センターの [料金とプラン] ページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-118">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4ad5f-119">CSP プログラムのパートナーは、パートナーセンター内の ISV 発行元から**ライセンスベース**の SaaS サブスクリプションのみを購入できます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-119">As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="4ad5f-120">つまり、ISV 発行者が利用可能にした**ライセンスベース**の SaaS プランを購入できます。これには、アクセス権を持つ[限定プラン](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)も含まれます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-120">This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="4ad5f-121">Isv (**使用量ベース**、従量制課金、使用量ベースのプランなど、azure アプリケーション、コンテナー、または vm を含む) から、他の商用 marketplace プランを購入または管理するには、 [azure 管理ポータル](https://portal.azure.com/)にアクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-121">To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based**, metered, or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/).</span></span> <span data-ttu-id="4ad5f-122">詳細については、「 [Purchase 市販の marketplace 製品](csp-commercial-marketplace-purchase.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-122">For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="4ad5f-123">新しいサブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="4ad5f-123">Create a new subscription</span></span>

1. <span data-ttu-id="4ad5f-124">[パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-124">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="4ad5f-125">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="4ad5f-126">**[サブスクリプションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-126">Select **Add subscription**.</span></span> <span data-ttu-id="4ad5f-127">[**オンラインサービス**] タブには、利用可能なすべての Marketplace SaaS プランが表示されます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-127">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="4ad5f-128">特定の種類のサブスクリプションのみを表示するには、使用可能なフィルターで選択を行います。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-128">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="4ad5f-129">**発行元**: microsoft からのプランのみを表示し、isv によって発行された商用 marketplace 製品を表示するには、[**パートナー** ]**を選択し**ます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-129">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="4ad5f-130">**課金の種類**: 使用するサブスクリプションの種類 (**ライセンス**または使用) を選択し**ます。**</span><span class="sxs-lookup"><span data-stu-id="4ad5f-130">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="4ad5f-131">請求頻度を月次と年次のいずれかに決定するのに役立つ情報については、[新しい請求機能についてよく寄せられる質問](faq-about-new-billing-features.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-131">See [FAQ about new billing features](faq-about-new-billing-features.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="4ad5f-132">**カテゴリ**: **Enterprise**、 **Small Business**、または**試用版**を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-132">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="4ad5f-133">試用版サブスクリプションについては、「[Microsoft 製品の試用版を顧客に提供する](offer-your-customers-trials-of-microsoft-products.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-133">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="4ad5f-134">顧客用に購入する製品サブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-134">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="4ad5f-135">表示される製品は、顧客セグメントの種類 (教育、政府など) と、適用したフィルターによって異なります。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-135">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="4ad5f-136">Marketplace に表示されるプランによっては、特定の顧客または特定の CSP パートナーが常に利用できるとは限りません。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-136">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="4ad5f-137">次の原因があります。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-137">This can be because:</span></span>

   - <span data-ttu-id="4ad5f-138">お客様は既にその製品のサブスクリプションを持っているため、1つのみを使用できます</span><span class="sxs-lookup"><span data-stu-id="4ad5f-138">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="4ad5f-139">お客様のサブスクリプションが中断されている可能性があります (この場合は、新しいサブスクリプションを購入するのではなく、サブスクリプションを再アクティブ化することができます)。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-139">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="4ad5f-140">ISV SaaS プランでは、プランを購入できない理由がいくつかあります。 ISV は、お客様の請求先の国または地域をサポートしていない可能性があります。ISV は、CSP プログラムを通じてプランを利用できるようにしないことを選択した可能性があります。または、ISV が特定の CSP パートナーのみ[に対してプランを](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)作成した可能性もあります。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-140">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="4ad5f-141">ISV プランは、パートナーセンター (たとえば、コンテナーや使用量ベースのプランなど) によって不可能されない場合もあります。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-141">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="4ad5f-142">追加するサブスクリプションごとに、必要に応じてライセンスの数を入力し、[**カートに追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-142">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="4ad5f-143">サブスクリプションの追加が完了したら、[**レビュー** ] を選択して注文を確認します。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-143">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="4ad5f-144">注文を確認し、これらのサブスクリプションを購入する準備ができたら、[**購入**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-144">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="4ad5f-145">顧客のサブスクリプションを購入すると、次のことが行われます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-145">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="4ad5f-146">サブスクリプションを確認または編集するには、その顧客の [**サブスクリプション**] ページからサブスクリプション名を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-146">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="4ad5f-147">ここでは、使用可能な場合はアドオン ライセンスを選択したり、ライセンスの数を変更したり、サブスクリプションを中断したりできます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-147">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="4ad5f-148">**ISV SaaS (ライセンスベース) サブスクリプションの場合:**</span><span class="sxs-lookup"><span data-stu-id="4ad5f-148">**For ISV SaaS (license-based) subscriptions:**</span></span>
    - <span data-ttu-id="4ad5f-149">ISV 発行元のサイトへのリンクが表示されます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-149">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="4ad5f-150">このリンクは、顧客のサブスクリプションのデプロイまたはアカウントの設定を完了するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-150">This link should help you complete the deployment or account setup of the customer's subscription.</span></span> <span data-ttu-id="4ad5f-151">(この種類の ISV サブスクリプションをセットアップまたはプロビジョニングするためのアカウントを設定するための手順を記載した電子メールは、お客様もお客様にも送信されないことに注意してください)。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-151">(Note that neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="4ad5f-152">サブスクリプションに30日間の無料試用版が付属している場合は、無料試用期間が自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-152">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="4ad5f-153">CSP プログラムのパートナーとして、お客様に購入したプランの無料試用期間を免除することはできません。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-153">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="4ad5f-154">無料試用期間が終了すると、サブスクリプション期間が開始され、サブスクリプションが有料ステータスに変換されます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-154">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="4ad5f-155">サブスクリプションは、同じスケジュールに従って autorenew されます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-155">The subscription will then autorenew according to the same schedule.</span></span>

## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="4ad5f-156">サブスクリプションを中断または取り消す</span><span class="sxs-lookup"><span data-stu-id="4ad5f-156">Suspend or cancel a subscription</span></span>

<span data-ttu-id="4ad5f-157">顧客から要請があった場合、または未払いや詐欺が発生した場合、パートナーはサブスクリプションを中断するか取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-157">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="4ad5f-158">サブスクリプションの中断</span><span class="sxs-lookup"><span data-stu-id="4ad5f-158">Suspend a subscription</span></span>

<span data-ttu-id="4ad5f-159">サブスクリプションの状態を **[中断]** に変更すると、ユーザーはサインインしたり、サービスにアクセスしたりできなくなります。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-159">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="4ad5f-160">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-160">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="4ad5f-161">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-161">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="4ad5f-162">管理対象のサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-162">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="4ad5f-163">**[状態]** セクションで **[保留]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-163">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="4ad5f-164">次に、変更内容を**送信**します。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-164">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="4ad5f-165">90 日以内、または 90 日にアカウントが開かれた時点から最初の課金までの日数を加えた期間 (最大 120 日) 以内にサブスクリプションを再アクティブ化しない限り、すべてのデータは削除されます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-165">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="4ad5f-166">サブスクリプションを中断するときに、**[中断]** ボタンの下に表示される日付は、サブスクリプションを再アクティブ化しない場合に自動的に期限切れになる日付です。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-166">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> <span data-ttu-id="4ad5f-167">詳細については、「[新しい請求機能に関する FAQ](faq-about-new-billing-features.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-167">For more information, see [FAQ about new billing features](faq-about-new-billing-features.md).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="4ad5f-168">サブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="4ad5f-168">Cancel a subscription</span></span>

<span data-ttu-id="4ad5f-169">パートナーセンターの[コマーシャルマーケットプレース](csp-commercial-marketplace-overview.md)内で、サードパーティの ISV 発行元からライセンスベースの SaaS サブスクリプションを取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-169">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="4ad5f-170">取り消し期間内にキャンセルした場合は、全額返金されます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-170">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="4ad5f-171">ISV プランの場合、毎月請求されます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-171">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="4ad5f-172">注文を行ってから24時間以内に取り消した場合は、次の請求書で全額のクレジットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-172">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="4ad5f-173">注文を行ってから24時間後にキャンセルした場合、キャンセルは更新時に実行されるようにスケジュールされます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-173">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="4ad5f-174">年ごとに請求されるプランの場合:</span><span class="sxs-lookup"><span data-stu-id="4ad5f-174">For offers billed annually:</span></span>

- <span data-ttu-id="4ad5f-175">注文を行ってから14日以内に取り消すと、次の請求書に対して完全なクレジットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-175">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="4ad5f-176">注文を行ってから14日後にキャンセルした場合、キャンセルは更新時に実行されるようにスケジュールされます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-176">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="4ad5f-177">これらの期間が経過すると、サブスクリプションを取り消すオプションが表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-177">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="4ad5f-178">使用量ベースおよび従量制課金 (仮想マシンまたはコンテナーを使用するサードパーティの ISV サービスなど) は、返品の対象にはなりません。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-178">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="4ad5f-179">使用量ベースのサービスは、取り消し方法としてプロビジョニング解除できます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-179">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="4ad5f-180">料金は使用後に課金されるため、これらのサービスは返金の対象にはなりません。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-180">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="4ad5f-181">ISV 発行元から取得したライセンスベースの SaaS サブスクリプションを取り消すには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-181">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="4ad5f-182">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-182">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="4ad5f-183">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-183">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="4ad5f-184">キャンセルするサブスクリプションを見つけます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-184">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="4ad5f-185">[**状態**] 列で、[**キャンセル**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-185">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="4ad5f-186">次に、変更内容を**送信**します。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-186">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="4ad5f-187">ダイアログボックスが表示されたら、関連する詳細情報を入力し、[**送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-187">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="4ad5f-188">キャンセルを確認するには、[**はい、キャンセル**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-188">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="4ad5f-189">Api を使用して Azure Marketplace サブスクリプションをキャンセルすることもできます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-189">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="4ad5f-190">これを行うには、「 [Azure Marketplace サブスクリプションをキャンセル](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-190">To do so, see [Cancel an Azure Marketplace subscription](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="4ad5f-191">商用マーケットプレースのサブスクリプションを自動的に更新するかどうかを選択する</span><span class="sxs-lookup"><span data-stu-id="4ad5f-191">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="4ad5f-192">既定では、アクティブなサブスクリプションは、サブスクリプション期間の有効期限が切れると自動的に更新されるように設定されます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-192">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="4ad5f-193">[商用マーケットプレース製品のサブスクリプション](csp-commercial-marketplace-overview.md)では、必要に応じて、サブスクリプションを自動的に更新しないことを選択できます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-193">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="4ad5f-194">アクティブな商用 marketplace サブスクリプションを自動的に更新しないようにするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-194">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="4ad5f-195">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-195">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="4ad5f-196">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-196">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="4ad5f-197">**[サブスクリプション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-197">Select **Subscriptions**.</span></span> <span data-ttu-id="4ad5f-198">これには、顧客用に購入したライセンスベースのサブスクリプションが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-198">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="4ad5f-199">[**サブスクリプション**] 列で、変更するサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-199">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="4ad5f-200">[サブスクリプションの詳細] ページで、[**状態**] セクションを見つけて、[**自動更新**] ボックスをオフにします。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-200">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="4ad5f-201">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="4ad5f-201">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4ad5f-202">次のステップ</span><span class="sxs-lookup"><span data-stu-id="4ad5f-202">Next steps</span></span>

- [<span data-ttu-id="4ad5f-203">顧客のために商用マーケットプレースの製品を購入する</span><span class="sxs-lookup"><span data-stu-id="4ad5f-203">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="4ad5f-204">顧客向けの商用 marketplace 製品を管理する</span><span class="sxs-lookup"><span data-stu-id="4ad5f-204">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="4ad5f-205">商業マーケットプレースの概要</span><span class="sxs-lookup"><span data-stu-id="4ad5f-205">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)
