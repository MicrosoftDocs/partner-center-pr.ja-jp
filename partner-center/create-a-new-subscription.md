---
title: パートナーセンターで顧客のサブスクリプションを作成する
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft が発行した製品や、サードパーティの Isv によって発行された SaaS 製品に対して顧客のサブスクリプションを販売する方法について説明します。
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 47291be42523cbcc3aafbb76a6fd9512191ca806
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435251"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="ba360-103">顧客のサブスクリプションの作成、中断、取り消し</span><span class="sxs-lookup"><span data-stu-id="ba360-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="ba360-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="ba360-104">**Applies to**</span></span>

- <span data-ttu-id="ba360-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="ba360-105">Partner Center</span></span>
- <span data-ttu-id="ba360-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="ba360-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="ba360-107">CSP パートナー</span><span class="sxs-lookup"><span data-stu-id="ba360-107">CSP partners</span></span>

<span data-ttu-id="ba360-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="ba360-108">**Appropriate roles**</span></span>

- <span data-ttu-id="ba360-109">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="ba360-109">Admin agent</span></span>
- <span data-ttu-id="ba360-110">課金管理者</span><span class="sxs-lookup"><span data-stu-id="ba360-110">Billing admin</span></span>
- <span data-ttu-id="ba360-111">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="ba360-111">Global admin</span></span>
- <span data-ttu-id="ba360-112">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="ba360-112">Helpdesk agent</span></span>
- <span data-ttu-id="ba360-113">販売代理店</span><span class="sxs-lookup"><span data-stu-id="ba360-113">Sales agent</span></span>

<span data-ttu-id="ba360-114">パートナー センターで顧客のレコードを作成したら、カタログ内の製品へのサブスクリプションを販売できます。</span><span class="sxs-lookup"><span data-stu-id="ba360-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="ba360-115">これには、Microsoft によって発行された製品と、サードパーティ製の独立系ソフトウェアベンダー (Isv) によって[商用マーケットプレース](https://azuremarketplace.microsoft.com/marketplace)に発行されたサービスとしてのソフトウェア (SaaS) 製品が含まれます。</span><span class="sxs-lookup"><span data-stu-id="ba360-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="ba360-116">一部のプランは、顧客ごとに1つのサブスクリプションに限定されます。</span><span class="sxs-lookup"><span data-stu-id="ba360-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="ba360-117">制限のあるオファーの一覧を確認するには、パートナー センターの [料金とプラン] ページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="ba360-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ba360-118">CSP プログラムのパートナーは、パートナーセンター内の ISV 発行元から**ライセンスベース**の SaaS サブスクリプションのみを購入できます。</span><span class="sxs-lookup"><span data-stu-id="ba360-118">As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="ba360-119">つまり、ISV 発行者が利用可能にした**ライセンスベース**の SaaS プランを購入できます。これには、アクセス権を持つ[限定プラン](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)も含まれます。</span><span class="sxs-lookup"><span data-stu-id="ba360-119">This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="ba360-120">Isv (**使用量ベース**、従量制課金、使用量ベースのプランなど、azure アプリケーション、コンテナー、または vm を含む) から、他の商用 marketplace プランを購入または管理するには、 [azure 管理ポータル](https://portal.azure.com/)にアクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="ba360-120">To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based**, metered, or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/).</span></span> <span data-ttu-id="ba360-121">詳細については、「 [Purchase 市販の marketplace 製品](csp-commercial-marketplace-purchase.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba360-121">For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="ba360-122">新しいサブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="ba360-122">Create a new subscription</span></span>

1. <span data-ttu-id="ba360-123">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="ba360-123">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="ba360-124">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="ba360-124">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="ba360-125">**[サブスクリプションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba360-125">Select **Add subscription**.</span></span> <span data-ttu-id="ba360-126">[**オンラインサービス**] タブには、利用可能なすべての Marketplace SaaS プランが表示されます。</span><span class="sxs-lookup"><span data-stu-id="ba360-126">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="ba360-127">特定の種類のサブスクリプションのみを表示するには、使用可能なフィルターで選択を行います。</span><span class="sxs-lookup"><span data-stu-id="ba360-127">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="ba360-128">**発行元**: microsoft からのプランのみを表示し、isv によって発行された商用 marketplace 製品を表示するには、[**パートナー** ]**を選択し**ます。</span><span class="sxs-lookup"><span data-stu-id="ba360-128">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="ba360-129">**課金の種類**: 使用するサブスクリプションの種類 (**ライセンス**または使用) を選択し**ます。**</span><span class="sxs-lookup"><span data-stu-id="ba360-129">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="ba360-130">請求頻度を月次と年次のいずれかに決定するのに役立つ情報については、[新しい請求機能についてよく寄せられる質問](faq-about-new-billing-features.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba360-130">See [FAQ about new billing features](faq-about-new-billing-features.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="ba360-131">**カテゴリ**: **Enterprise**、 **Small Business**、または**試用版**を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba360-131">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="ba360-132">試用版サブスクリプションについては、「[Microsoft 製品の試用版を顧客に提供する](offer-your-customers-trials-of-microsoft-products.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="ba360-132">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="ba360-133">顧客用に購入する製品サブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="ba360-133">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="ba360-134">表示される製品は、顧客セグメントの種類 (教育、政府など) と、適用したフィルターによって異なります。</span><span class="sxs-lookup"><span data-stu-id="ba360-134">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="ba360-135">Marketplace に表示されるプランによっては、特定の顧客または特定の CSP パートナーが常に利用できるとは限りません。</span><span class="sxs-lookup"><span data-stu-id="ba360-135">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="ba360-136">次の原因があります。</span><span class="sxs-lookup"><span data-stu-id="ba360-136">This can be because:</span></span>

   - <span data-ttu-id="ba360-137">お客様は既にその製品のサブスクリプションを持っているため、1つのみを使用できます</span><span class="sxs-lookup"><span data-stu-id="ba360-137">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="ba360-138">お客様のサブスクリプションが中断されている可能性があります (この場合は、新しいサブスクリプションを購入するのではなく、サブスクリプションを再アクティブ化することができます)。</span><span class="sxs-lookup"><span data-stu-id="ba360-138">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="ba360-139">ISV SaaS プランでは、プランを購入できない理由がいくつかあります。 ISV は、お客様の請求先の国または地域をサポートしていない可能性があります。ISV は、CSP プログラムを通じてプランを利用できるようにしないことを選択した可能性があります。または、ISV が特定の CSP パートナーのみ[に対してプランを](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)作成した可能性もあります。</span><span class="sxs-lookup"><span data-stu-id="ba360-139">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="ba360-140">ISV プランは、パートナーセンター (たとえば、コンテナーや使用量ベースのプランなど) によって不可能されない場合もあります。</span><span class="sxs-lookup"><span data-stu-id="ba360-140">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="ba360-141">追加するサブスクリプションごとに、必要に応じてライセンスの数を入力し、[**カートに追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba360-141">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="ba360-142">サブスクリプションの追加が完了したら、[**レビュー** ] を選択して注文を確認します。</span><span class="sxs-lookup"><span data-stu-id="ba360-142">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="ba360-143">注文を確認し、これらのサブスクリプションを購入する準備ができたら、[**購入**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba360-143">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="ba360-144">顧客のサブスクリプションを購入すると、次のことが行われます。</span><span class="sxs-lookup"><span data-stu-id="ba360-144">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="ba360-145">サブスクリプションを確認または編集するには、その顧客の [**サブスクリプション**] ページからサブスクリプション名を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba360-145">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="ba360-146">ここでは、使用可能な場合はアドオン ライセンスを選択したり、ライセンスの数を変更したり、サブスクリプションを中断したりできます。</span><span class="sxs-lookup"><span data-stu-id="ba360-146">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="ba360-147">**ISV SaaS (ライセンスベース) サブスクリプションの場合:**</span><span class="sxs-lookup"><span data-stu-id="ba360-147">**For ISV SaaS (license-based) subscriptions:**</span></span>
    - <span data-ttu-id="ba360-148">ISV 発行元のサイトへのリンクが表示されます。</span><span class="sxs-lookup"><span data-stu-id="ba360-148">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="ba360-149">このリンクは、顧客のサブスクリプションのデプロイまたはアカウントの設定を完了するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="ba360-149">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="ba360-150">お客様やお客様には、この種類の ISV サブスクリプションのセットアップ/プロビジョニングを完了するための手順を記載した電子メールが届きません。)</span><span class="sxs-lookup"><span data-stu-id="ba360-150">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="ba360-151">サブスクリプションに30日間の無料試用版が付属している場合は、無料試用期間が自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="ba360-151">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="ba360-152">CSP プログラムのパートナーとして、お客様に購入したプランの無料試用期間を免除することはできません。</span><span class="sxs-lookup"><span data-stu-id="ba360-152">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="ba360-153">無料試用期間が終了すると、サブスクリプション期間が開始され、サブスクリプションが有料ステータスに変換されます。</span><span class="sxs-lookup"><span data-stu-id="ba360-153">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="ba360-154">サブスクリプションは、同じスケジュールに従って autorenew されます。</span><span class="sxs-lookup"><span data-stu-id="ba360-154">The subscription will then autorenew according to the same schedule.</span></span>

## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="ba360-155">サブスクリプションを中断または取り消す</span><span class="sxs-lookup"><span data-stu-id="ba360-155">Suspend or cancel a subscription</span></span>

<span data-ttu-id="ba360-156">顧客から要請があった場合、または未払いや詐欺が発生した場合、パートナーはサブスクリプションを中断するか取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="ba360-156">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="ba360-157">サブスクリプションの中断</span><span class="sxs-lookup"><span data-stu-id="ba360-157">Suspend a subscription</span></span>

<span data-ttu-id="ba360-158">サブスクリプションの状態を **[中断]** に変更すると、ユーザーはサインインしたり、サービスにアクセスしたりできなくなります。</span><span class="sxs-lookup"><span data-stu-id="ba360-158">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="ba360-159">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="ba360-159">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="ba360-160">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="ba360-160">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="ba360-161">管理対象のサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="ba360-161">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="ba360-162">**[状態]** セクションで **[保留]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba360-162">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="ba360-163">次に、変更内容を**送信**します。</span><span class="sxs-lookup"><span data-stu-id="ba360-163">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="ba360-164">90 日以内、または 90 日にアカウントが開かれた時点から最初の課金までの日数を加えた期間 (最大 120 日) 以内にサブスクリプションを再アクティブ化しない限り、すべてのデータは削除されます。</span><span class="sxs-lookup"><span data-stu-id="ba360-164">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="ba360-165">サブスクリプションを中断するときに、**[中断]** ボタンの下に表示される日付は、サブスクリプションを再アクティブ化しない場合に自動的に期限切れになる日付です。</span><span class="sxs-lookup"><span data-stu-id="ba360-165">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> <span data-ttu-id="ba360-166">詳細については、「[新しい請求機能に関する FAQ](faq-about-new-billing-features.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba360-166">For more information, see [FAQ about new billing features](faq-about-new-billing-features.md).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="ba360-167">サブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="ba360-167">Cancel a subscription</span></span>

<span data-ttu-id="ba360-168">パートナーセンターの[コマーシャルマーケットプレース](csp-commercial-marketplace-overview.md)内で、サードパーティの ISV 発行元からライセンスベースの SaaS サブスクリプションを取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="ba360-168">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="ba360-169">取り消し期間内にキャンセルした場合は、全額返金されます。</span><span class="sxs-lookup"><span data-stu-id="ba360-169">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="ba360-170">ISV プランの場合、毎月請求されます。</span><span class="sxs-lookup"><span data-stu-id="ba360-170">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="ba360-171">注文を行ってから24時間以内に取り消した場合は、次の請求書で全額のクレジットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="ba360-171">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="ba360-172">注文を行ってから24時間後にキャンセルした場合、キャンセルは更新時に実行されるようにスケジュールされます。</span><span class="sxs-lookup"><span data-stu-id="ba360-172">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="ba360-173">年ごとに請求されるプランの場合:</span><span class="sxs-lookup"><span data-stu-id="ba360-173">For offers billed annually:</span></span>

- <span data-ttu-id="ba360-174">注文を行ってから14日以内に取り消すと、次の請求書に対して完全なクレジットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="ba360-174">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="ba360-175">注文を行ってから14日後にキャンセルした場合、キャンセルは更新時に実行されるようにスケジュールされます。</span><span class="sxs-lookup"><span data-stu-id="ba360-175">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="ba360-176">これらの期間が経過すると、サブスクリプションを取り消すオプションが表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="ba360-176">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="ba360-177">使用量ベースおよび従量制課金 (仮想マシンまたはコンテナーを使用するサードパーティの ISV サービスなど) は、返品の対象にはなりません。</span><span class="sxs-lookup"><span data-stu-id="ba360-177">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="ba360-178">使用量ベースのサービスは、取り消し方法としてプロビジョニング解除できます。</span><span class="sxs-lookup"><span data-stu-id="ba360-178">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="ba360-179">料金は使用後に課金されるため、これらのサービスは返金の対象にはなりません。</span><span class="sxs-lookup"><span data-stu-id="ba360-179">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="ba360-180">ISV 発行元から取得したライセンスベースの SaaS サブスクリプションを取り消すには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="ba360-180">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="ba360-181">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="ba360-181">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="ba360-182">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="ba360-182">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="ba360-183">キャンセルするサブスクリプションを見つけます。</span><span class="sxs-lookup"><span data-stu-id="ba360-183">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="ba360-184">[**状態**] 列で、[**キャンセル**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba360-184">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="ba360-185">次に、変更内容を**送信**します。</span><span class="sxs-lookup"><span data-stu-id="ba360-185">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="ba360-186">ダイアログボックスが表示されたら、関連する詳細情報を入力し、[**送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba360-186">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="ba360-187">キャンセルを確認するには、[**はい、キャンセル**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba360-187">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="ba360-188">Api を使用して Azure Marketplace サブスクリプションをキャンセルすることもできます。</span><span class="sxs-lookup"><span data-stu-id="ba360-188">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="ba360-189">これを行うには、「 [Azure Marketplace サブスクリプションをキャンセル](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba360-189">To do so, see [Cancel an Azure Marketplace subscription](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="ba360-190">商用マーケットプレースのサブスクリプションを自動的に更新するかどうかを選択する</span><span class="sxs-lookup"><span data-stu-id="ba360-190">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="ba360-191">既定では、アクティブなサブスクリプションは、サブスクリプション期間の期限が切れると自動的に更新するように設定されます。</span><span class="sxs-lookup"><span data-stu-id="ba360-191">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="ba360-192">[商用 marketplace 製品のサブスクリプション](csp-commercial-marketplace-overview.md)については、必要に応じてサブスクリプションを自動的に更新しないように選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="ba360-192">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="ba360-193">アクティブな商用 marketplace サブスクリプションを自動的に更新しないようにするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="ba360-193">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="ba360-194">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="ba360-194">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="ba360-195">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="ba360-195">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="ba360-196">**[サブスクリプション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba360-196">Select **Subscriptions**.</span></span> <span data-ttu-id="ba360-197">これには、顧客用に購入したライセンスベースのサブスクリプションが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="ba360-197">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="ba360-198">[**サブスクリプション**] 列で、変更するサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="ba360-198">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="ba360-199">[サブスクリプションの詳細] ページで、[**状態**] セクションを見つけて、[**自動更新**] ボックスをオフにします。</span><span class="sxs-lookup"><span data-stu-id="ba360-199">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="ba360-200">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ba360-200">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ba360-201">次のステップ</span><span class="sxs-lookup"><span data-stu-id="ba360-201">Next steps</span></span>

- [<span data-ttu-id="ba360-202">顧客のために商用マーケットプレースの製品を購入する</span><span class="sxs-lookup"><span data-stu-id="ba360-202">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="ba360-203">顧客向けの商用 marketplace 製品を管理する</span><span class="sxs-lookup"><span data-stu-id="ba360-203">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="ba360-204">商業マーケットプレースの概要</span><span class="sxs-lookup"><span data-stu-id="ba360-204">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)
