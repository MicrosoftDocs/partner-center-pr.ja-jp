---
title: パートナーセンターで顧客のサブスクリプションを作成する
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft によって発行された製品や、サードパーティの Isv によって発行された SaaS 製品について、顧客にサブスクリプションを販売する方法について説明します。
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201410"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="99921-103">顧客のサブスクリプションの作成、中断、取り消し</span><span class="sxs-lookup"><span data-stu-id="99921-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="99921-104">**適用対象**: パートナーセンター |米国政府向け Microsoft Cloud パートナーセンター</span><span class="sxs-lookup"><span data-stu-id="99921-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="99921-105">**適切なロール**: 管理エージェント |課金管理者 |全体管理者 |ヘルプデスクエージェント |営業担当者</span><span class="sxs-lookup"><span data-stu-id="99921-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="99921-106">パートナー センターで顧客のレコードを作成したら、カタログ内の製品へのサブスクリプションを販売できます。</span><span class="sxs-lookup"><span data-stu-id="99921-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="99921-107">これには、Microsoft によって発行された製品と、サードパーティ製の Isv (独立系ソフトウェアベンダー) によって発行されたサービスとしてのソフトウェア (SaaS) 製品が含ま[れます。](https://azuremarketplace.microsoft.com/marketplace)</span><span class="sxs-lookup"><span data-stu-id="99921-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="99921-108">一部のプランは、顧客ごとに1つのサブスクリプションに限定されます。</span><span class="sxs-lookup"><span data-stu-id="99921-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="99921-109">制限のあるオファーの一覧を確認するには、パートナー センターの [料金とプラン] ページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="99921-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="99921-110">CSP プログラムのパートナーとして、パートナーセンター内の ISV 発行元から **ライセンスベース** または **従量制** の SaaS サブスクリプションを購入することができます。</span><span class="sxs-lookup"><span data-stu-id="99921-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="99921-111">つまり、ISV 発行者が利用可能にした **ライセンスベース** または **従量制** の SaaS プランを購入できます。これには、アクセス権のある [限定プラン](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) も含まれます。</span><span class="sxs-lookup"><span data-stu-id="99921-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="99921-112">Isv (Azure アプリケーション、コンテナー、または Vm を含む使用量ベースのプランなど) から、他の商用 marketplace プランを購入または管理するには、 [Azure portal](https://portal.azure.com/)にアクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="99921-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

>[!NOTE]
><span data-ttu-id="99921-113">パートナーセンターのすべての日付と時刻は、協定世界時 (UTC) で指定されます。</span><span class="sxs-lookup"><span data-stu-id="99921-113">All dates and times in Partner Center are given in the Universal Time Coordinated (UTC) time standard.</span></span> <span data-ttu-id="99921-114">これは、現地時刻から最大24時間まで異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="99921-114">This can differ by up to 24 hours from your local time.</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="99921-115">新しいサブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="99921-115">Create a new subscription</span></span>

1. <span data-ttu-id="99921-116">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="99921-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="99921-117">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="99921-117">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="99921-118">**[サブスクリプションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="99921-118">Select **Add subscription**.</span></span> <span data-ttu-id="99921-119">[ **オンラインサービス** ] タブには、利用可能なすべての Marketplace SaaS プランが表示されます。</span><span class="sxs-lookup"><span data-stu-id="99921-119">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="99921-120">特定の種類のサブスクリプションのみを表示するには、使用可能なフィルターで選択を行います。</span><span class="sxs-lookup"><span data-stu-id="99921-120">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="99921-121">**発行元**: microsoft からのプランのみを表示し、isv によって発行された商用 marketplace 製品を表示するには、[**パートナー** ]**を選択し** ます。</span><span class="sxs-lookup"><span data-stu-id="99921-121">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="99921-122">**課金の種類**: 使用するサブスクリプションの種類 (**ライセンス** または使用) を選択し **ます。**</span><span class="sxs-lookup"><span data-stu-id="99921-122">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="99921-123">月単位および年間請求頻度の決定に役立つ情報については、 [ライセンスベースの課金](license-based-billing.md) に関する情報を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99921-123">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="99921-124">**カテゴリ**: **Enterprise**、 **Small Business**、または **試用版** を選択します。</span><span class="sxs-lookup"><span data-stu-id="99921-124">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="99921-125">試用版サブスクリプションについては、「[Microsoft 製品の試用版を顧客に提供する](offer-your-customers-trials-of-microsoft-products.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="99921-125">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="99921-126">顧客用に購入する製品サブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="99921-126">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="99921-127">表示される製品は、顧客セグメントの種類 (教育、政府など) と適用したフィルターによって異なります。</span><span class="sxs-lookup"><span data-stu-id="99921-127">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="99921-128">Marketplace に表示される一部のオファーは、特定の顧客または特定の CSP パートナーが常に利用できるとは限りではありません。</span><span class="sxs-lookup"><span data-stu-id="99921-128">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="99921-129">これは、次の理由で可能です。</span><span class="sxs-lookup"><span data-stu-id="99921-129">This can be because:</span></span>

   - <span data-ttu-id="99921-130">顧客は既にその製品のサブスクリプションを持ち、1 つしか許可されません</span><span class="sxs-lookup"><span data-stu-id="99921-130">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="99921-131">顧客のサブスクリプションが中断されている可能性があります (この場合は、新しいサブスクリプションを購入するのではなく、サブスクリプションを再アクティブ化できます)。</span><span class="sxs-lookup"><span data-stu-id="99921-131">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="99921-132">ISV SaaS オファーの場合、オファーを購入できない理由がいくつかある場合があります。ISV は、顧客の請求先の国または地域をサポートしていない可能性があります。ISV は、CSP プログラムを通じてオファーを利用できない場合があります。または、ISV が特定の CSP[](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)パートナー専用のオファーを作成した可能性があります。</span><span class="sxs-lookup"><span data-stu-id="99921-132">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="99921-133">ISV オファーは、コンテナーや一部の使用量ベースのオファーパートナー センターサービスを通じて取引できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="99921-133">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="99921-134">追加するサブスクリプションごとに、ライセンスの数 (必要に応じて) を入力し、[カートに追加] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="99921-134">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="99921-135">サブスクリプションの追加が完了したら、[注文の確認と **確認** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="99921-135">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="99921-136">注文を確認し、これらのサブスクリプションを購入する準備ができたら、[購入] を選択 **します**。</span><span class="sxs-lookup"><span data-stu-id="99921-136">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="99921-137">顧客のサブスクリプションを購入すると、次の処理が行われます。</span><span class="sxs-lookup"><span data-stu-id="99921-137">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="99921-138">サブスクリプションを確認または編集するには、その顧客の [サブスクリプション] ページからサブスクリプション名 **を選択** します。</span><span class="sxs-lookup"><span data-stu-id="99921-138">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="99921-139">ここでは、使用可能な場合はアドオン ライセンスを選択したり、ライセンスの数を変更したり、サブスクリプションを中断したりできます。</span><span class="sxs-lookup"><span data-stu-id="99921-139">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="99921-140">**ISV SaaS (ライセンスベースおよび測定) サブスクリプションの場合:**</span><span class="sxs-lookup"><span data-stu-id="99921-140">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="99921-141">ISV 発行元のサイトへのリンクが表示されます。</span><span class="sxs-lookup"><span data-stu-id="99921-141">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="99921-142">このリンクは、顧客のサブスクリプションのデプロイまたはアカウントの設定を完了するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="99921-142">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="99921-143">お客様も顧客も、この種類の ISV サブスクリプションのアカウントの設定/プロビジョニングを完了する手順を記載した電子メールを受け取る必要があります)。)</span><span class="sxs-lookup"><span data-stu-id="99921-143">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="99921-144">サブスクリプションに 30 日間の無料試用版が付属している場合は、無料試用版期間が自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="99921-144">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="99921-145">CSP プログラムのパートナーは、顧客向けに購入したオファーの無料試用期間を無料で提供することはできません。</span><span class="sxs-lookup"><span data-stu-id="99921-145">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="99921-146">無料試用期間が終了すると、サブスクリプション期間が開始され、サブスクリプションが有料ステータスに変換されます。</span><span class="sxs-lookup"><span data-stu-id="99921-146">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="99921-147">サブスクリプションは、同じスケジュールに従って自動更新されます。</span><span class="sxs-lookup"><span data-stu-id="99921-147">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="99921-148">アドオンでサブスクリプションを更新する</span><span class="sxs-lookup"><span data-stu-id="99921-148">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="99921-149">アドオンを購入するには、まず、顧客がアクティブな基本サブスクリプションを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="99921-149">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="99921-150">カタログを通じてアドオンを購入することはできません。</span><span class="sxs-lookup"><span data-stu-id="99921-150">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="99921-151">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="99921-151">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="99921-152">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="99921-152">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="99921-153">管理対象のサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="99921-153">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="99921-154">[ **状態** ] セクションの下には、サブスクリプションで使用可能なアドオンの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="99921-154">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="99921-155">必要なアドオンごとにライセンスの数を更新します。</span><span class="sxs-lookup"><span data-stu-id="99921-155">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="99921-156">次に、変更内容を **送信** します。</span><span class="sxs-lookup"><span data-stu-id="99921-156">Then **Submit** your changes.</span></span>

<span data-ttu-id="99921-157">パートナーセンターを通じてアドオンを購入する機能は、直接請求と間接プロバイダーにのみ提供されます。</span><span class="sxs-lookup"><span data-stu-id="99921-157">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="99921-158">基本要件と使用可能なリージョンに基づいて、対象となるアドオンのみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="99921-158">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="99921-159">価格とプランの詳細については、クラウドリセラープランのマトリックスを参照してください。</span><span class="sxs-lookup"><span data-stu-id="99921-159">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="99921-160">ベース サブスクリプションを中断すると、関連するすべてのアドオンも中断されます。</span><span class="sxs-lookup"><span data-stu-id="99921-160">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="99921-161">アドオンの開始日はベース サブスクリプションに合わせられ、料金は最初の請求書において請求開始日から請求終了日の対する比例配分で計算されます。</span><span class="sxs-lookup"><span data-stu-id="99921-161">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="99921-162">詳細については、「 [ライセンスベースの課金](license-based-billing.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99921-162">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="99921-163">サブスクリプションを中断または取り消す</span><span class="sxs-lookup"><span data-stu-id="99921-163">Suspend or cancel a subscription</span></span>

<span data-ttu-id="99921-164">顧客から要請があった場合、または未払いや詐欺が発生した場合、パートナーはサブスクリプションを中断するか取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="99921-164">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="99921-165">サブスクリプションの中断</span><span class="sxs-lookup"><span data-stu-id="99921-165">Suspend a subscription</span></span>

<span data-ttu-id="99921-166">サブスクリプションの状態を **[中断]** に変更すると、ユーザーはサインインしたり、サービスにアクセスしたりできなくなります。</span><span class="sxs-lookup"><span data-stu-id="99921-166">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="99921-167">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="99921-167">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="99921-168">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="99921-168">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="99921-169">管理対象のサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="99921-169">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="99921-170">**[状態]** セクションで **[保留]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="99921-170">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="99921-171">次に、変更内容を **送信** します。</span><span class="sxs-lookup"><span data-stu-id="99921-171">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="99921-172">90 日以内、または 90 日にアカウントが開かれた時点から最初の課金までの日数を加えた期間 (最大 120 日) 以内にサブスクリプションを再アクティブ化しない限り、すべてのデータは削除されます。</span><span class="sxs-lookup"><span data-stu-id="99921-172">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="99921-173">サブスクリプションを中断するときに、**[中断]** ボタンの下に表示される日付は、サブスクリプションを再アクティブ化しない場合に自動的に期限切れになる日付です。</span><span class="sxs-lookup"><span data-stu-id="99921-173">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="99921-174">CSP サブスクリプションでは、サービスがまだ動作しているものの、サブスクリプションで請求料金が生成されない期限切れの期間 (web ダイレクトサブスクリプションの方法) がありません。</span><span class="sxs-lookup"><span data-stu-id="99921-174">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="99921-175">CSP サブスクリプションは、アクティブまたは中断 (または完全に削除) のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="99921-175">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="99921-176">サブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="99921-176">Cancel a subscription</span></span>

<span data-ttu-id="99921-177">パートナーセンターの [コマーシャルマーケットプレース](csp-commercial-marketplace-overview.md)内で、サードパーティの ISV 発行元からライセンスベースの SaaS サブスクリプションを取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="99921-177">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="99921-178">取り消し期間内にキャンセルした場合は、全額返金されます。</span><span class="sxs-lookup"><span data-stu-id="99921-178">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="99921-179">ISV プランの場合、毎月請求されます。</span><span class="sxs-lookup"><span data-stu-id="99921-179">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="99921-180">注文を行ってから24時間以内に取り消した場合は、次の請求書で全額のクレジットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="99921-180">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="99921-181">注文を行ってから24時間後にキャンセルした場合、キャンセルは更新時に実行されるようにスケジュールされます。</span><span class="sxs-lookup"><span data-stu-id="99921-181">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="99921-182">年ごとに請求されるプランの場合:</span><span class="sxs-lookup"><span data-stu-id="99921-182">For offers billed annually:</span></span>

- <span data-ttu-id="99921-183">注文を行ってから14日以内に取り消すと、次の請求書に対して完全なクレジットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="99921-183">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="99921-184">注文を行ってから14日後にキャンセルした場合、キャンセルは更新時に実行されるようにスケジュールされます。</span><span class="sxs-lookup"><span data-stu-id="99921-184">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="99921-185">これらの期間が経過すると、サブスクリプションを取り消すオプションが表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="99921-185">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="99921-186">使用量ベースおよび測定されたサード パーティの ISV サービス (仮想マシンやコンテナーを使用するサービスなど) は、返品の対象ではありません。</span><span class="sxs-lookup"><span data-stu-id="99921-186">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="99921-187">使用量ベースのサービスは、取り消し方法としてプロビジョニング解除できます。</span><span class="sxs-lookup"><span data-stu-id="99921-187">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="99921-188">料金は使用後に課金されます。このため、これらのサービスは返金の対象ではありません。</span><span class="sxs-lookup"><span data-stu-id="99921-188">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="99921-189">ISV 発行元から取得したライセンスベースの SaaS サブスクリプションを取り消すには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="99921-189">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="99921-190">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="99921-190">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="99921-191">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="99921-191">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="99921-192">取り消すサブスクリプションを見つける。</span><span class="sxs-lookup"><span data-stu-id="99921-192">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="99921-193">[状態] **列で** 、[キャンセル] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="99921-193">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="99921-194">次に、変更内容を **送信** します。</span><span class="sxs-lookup"><span data-stu-id="99921-194">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="99921-195">ダイアログ ボックスが表示されたら、関連する詳細を入力し、[送信] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="99921-195">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="99921-196">取り消しを確定するには、[はい、キャンセル **] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="99921-196">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="99921-197">また、API を使用してサブスクリプションのAzure Marketplaceを取り消す方法を選択できます。</span><span class="sxs-lookup"><span data-stu-id="99921-197">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="99921-198">これを行うには、「サブスクリプションのキャンセル [」をAzure Marketplaceしてください](/partner-center/develop/cancel-an-azure-marketplace-subscription)。</span><span class="sxs-lookup"><span data-stu-id="99921-198">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="99921-199">商用マーケットプレースのサブスクリプションを自動的に更新するかどうかを選択する</span><span class="sxs-lookup"><span data-stu-id="99921-199">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="99921-200">既定では、アクティブなサブスクリプションは、サブスクリプション期間の期限が切れると自動的に更新するように設定されます。</span><span class="sxs-lookup"><span data-stu-id="99921-200">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="99921-201">コマーシャル [マーケットプレース製品のサブスクリプションの](csp-commercial-marketplace-overview.md)場合は、必要に応じて、サブスクリプションを自動的に更新しない方法を選択できます。</span><span class="sxs-lookup"><span data-stu-id="99921-201">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="99921-202">アクティブなコマーシャル マーケットプレース サブスクリプションの自動更新を停止するには:</span><span class="sxs-lookup"><span data-stu-id="99921-202">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="99921-203">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="99921-203">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="99921-204">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="99921-204">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="99921-205">**[サブスクリプション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="99921-205">Select **Subscriptions**.</span></span> <span data-ttu-id="99921-206">これにより、顧客に対して購入したライセンス ベースのサブスクリプションが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="99921-206">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="99921-207">[サブスクリプション **]** 列で、変更するサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="99921-207">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="99921-208">サブスクリプションの詳細ページで、[状態] セクション **を見つけて** 、[ **自動更新] ボックスをオフ** にします。</span><span class="sxs-lookup"><span data-stu-id="99921-208">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="99921-209">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="99921-209">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="99921-210">次のステップ</span><span class="sxs-lookup"><span data-stu-id="99921-210">Next steps</span></span>

- [<span data-ttu-id="99921-211">顧客のために商用マーケットプレースの製品を購入する</span><span class="sxs-lookup"><span data-stu-id="99921-211">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="99921-212">顧客向けコマーシャル マーケットプレース製品を管理する</span><span class="sxs-lookup"><span data-stu-id="99921-212">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="99921-213">商業マーケットプレースの概要</span><span class="sxs-lookup"><span data-stu-id="99921-213">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)