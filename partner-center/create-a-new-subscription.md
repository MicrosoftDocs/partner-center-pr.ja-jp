---
title: 顧客サブスクリプションを作成パートナー センター
ms.topic: how-to
ms.date: 05/17/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft によって発行された製品と、サード パーティの ISV によって発行された SaaS 製品のサブスクリプションを顧客に販売する方法について説明します。
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 3269fa994d704c0a0dae067087bad8589a7ce031
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148201"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="da950-103">顧客のサブスクリプションの作成、中断、取り消し</span><span class="sxs-lookup"><span data-stu-id="da950-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="da950-104">**適用対象**: パートナー センター |パートナー センターのMicrosoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="da950-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="da950-105">**適切なロール**: 管理エージェント |課金管理者|グローバル管理者|ヘルプデスク エージェント |セールス エージェント</span><span class="sxs-lookup"><span data-stu-id="da950-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="da950-106">パートナー センターで顧客のレコードを作成したら、カタログ内の製品へのサブスクリプションを販売できます。</span><span class="sxs-lookup"><span data-stu-id="da950-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="da950-107">これには、サード パーティの独立系ソフトウェア ベンダー (ISV) によってコマーシャル マーケットプレースに発行された Microsoft およびサービスとしてのソフトウェア (SaaS) 製品によって公開された製品が [含まれます](https://azuremarketplace.microsoft.com/marketplace)。</span><span class="sxs-lookup"><span data-stu-id="da950-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="da950-108">一部のオファーは、顧客ごとに 1 つのサブスクリプションに制限されます。</span><span class="sxs-lookup"><span data-stu-id="da950-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="da950-109">制限のあるオファーの一覧を確認するには、パートナー センターの [料金とプラン] ページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="da950-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="da950-110">CSP プログラムのパートナーは、ライセンスベースまたは測定された **SaaS** サブスクリプションを、パートナー センター 内の ISV パブリッシャーから購入できます。</span><span class="sxs-lookup"><span data-stu-id="da950-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="da950-111">つまり、ISV 発行元が利用できるライセンスベースまたは測定された **SaaS** オファー (アクセス権を持 [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)つ排他的なオファーを含む) を購入できます。</span><span class="sxs-lookup"><span data-stu-id="da950-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="da950-112">ISV から他の商用マーケットプレース オファー (Azure アプリケーション、コンテナー、VM を含む使用量ベースのオファーなど) を購入または管理するには、次のページに移動する必要[Azure portal。](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="da950-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="da950-113">新しいサブスクリプションを作成する</span><span class="sxs-lookup"><span data-stu-id="da950-113">Create a new subscription</span></span>

1. <span data-ttu-id="da950-114">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="da950-114">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="da950-115">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="da950-115">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="da950-116">**[サブスクリプションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="da950-116">Select **Add subscription**.</span></span> <span data-ttu-id="da950-117">[ **オンライン サービス] タブ** には、使用可能なすべての Marketplace SaaS オファーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="da950-117">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="da950-118">特定の種類のサブスクリプションのみを表示するには、使用可能なフィルターで選択を行います。</span><span class="sxs-lookup"><span data-stu-id="da950-118">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="da950-119">**[発行** 元 **]: [Microsoft]** を選択してMicrosoft のオファーのみを表示するか、ISV によって発行されたコマーシャル マーケットプレース製品を表示するパートナーを選択します。</span><span class="sxs-lookup"><span data-stu-id="da950-119">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="da950-120">**課金の種類**: 使用するサブスクリプションの課金の種類を選択します: [ **ライセンス] または** [使用状況 **]**。</span><span class="sxs-lookup"><span data-stu-id="da950-120">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="da950-121">月 [次請求頻度と年間請求](license-based-billing.md) 頻度の決定に役立つ情報については、ライセンスベースの課金に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="da950-121">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="da950-122">**カテゴリ**: [**エンタープライズ] 、 [\*\*\*\*小規模ビジネス] 、または**[試用版] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="da950-122">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="da950-123">試用版サブスクリプションについては、「[Microsoft 製品の試用版を顧客に提供する](offer-your-customers-trials-of-microsoft-products.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="da950-123">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="da950-124">顧客に対して購入する製品サブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="da950-124">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="da950-125">表示される製品は、顧客セグメントの種類 (教育、政府など) と適用したフィルターによって異なります。</span><span class="sxs-lookup"><span data-stu-id="da950-125">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="da950-126">Marketplace に表示されるプランによっては、特定の顧客または特定の CSP パートナーが常に利用できるとは限りません。</span><span class="sxs-lookup"><span data-stu-id="da950-126">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="da950-127">次の原因があります。</span><span class="sxs-lookup"><span data-stu-id="da950-127">This can be because:</span></span>

   - <span data-ttu-id="da950-128">お客様は既にその製品のサブスクリプションを持っているため、1つのみを使用できます</span><span class="sxs-lookup"><span data-stu-id="da950-128">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="da950-129">お客様のサブスクリプションが中断されている可能性があります (この場合は、新しいサブスクリプションを購入するのではなく、サブスクリプションを再アクティブ化することができます)。</span><span class="sxs-lookup"><span data-stu-id="da950-129">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="da950-130">ISV SaaS プランでは、プランを購入できない理由がいくつかあります。 ISV は、お客様の請求先の国または地域をサポートしていない可能性があります。ISV は、CSP プログラムを通じてプランを利用できるようにしないことを選択した可能性があります。または、ISV が特定の CSP パートナーのみ [に対してプランを](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 作成した可能性もあります。</span><span class="sxs-lookup"><span data-stu-id="da950-130">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="da950-131">ISV プランは、パートナーセンター (たとえば、コンテナーや使用量ベースのプランなど) によって不可能されない場合もあります。</span><span class="sxs-lookup"><span data-stu-id="da950-131">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="da950-132">追加するサブスクリプションごとに、必要に応じてライセンスの数を入力し、[ **カートに追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="da950-132">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="da950-133">サブスクリプションの追加が完了したら、[ **レビュー** ] を選択して注文を確認します。</span><span class="sxs-lookup"><span data-stu-id="da950-133">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="da950-134">注文を確認し、これらのサブスクリプションを購入する準備ができたら、[ **購入**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="da950-134">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="da950-135">顧客のサブスクリプションを購入すると、次のことが行われます。</span><span class="sxs-lookup"><span data-stu-id="da950-135">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="da950-136">サブスクリプションを確認または編集するには、その顧客の [ **サブスクリプション** ] ページからサブスクリプション名を選択します。</span><span class="sxs-lookup"><span data-stu-id="da950-136">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="da950-137">ここでは、使用可能な場合はアドオン ライセンスを選択したり、ライセンスの数を変更したり、サブスクリプションを中断したりできます。</span><span class="sxs-lookup"><span data-stu-id="da950-137">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="da950-138">**ISV SaaS (ライセンスベースおよび従量制課金) サブスクリプションの場合:**</span><span class="sxs-lookup"><span data-stu-id="da950-138">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="da950-139">ISV 発行元のサイトへのリンクが表示されます。</span><span class="sxs-lookup"><span data-stu-id="da950-139">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="da950-140">このリンクは、顧客のサブスクリプションのデプロイまたはアカウントの設定を完了するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="da950-140">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="da950-141">お客様やお客様には、この種類の ISV サブスクリプションのセットアップ/プロビジョニングを完了するための手順を記載した電子メールが届きません。)</span><span class="sxs-lookup"><span data-stu-id="da950-141">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="da950-142">サブスクリプションに30日間の無料試用版が付属している場合は、無料試用期間が自動的に適用されます。</span><span class="sxs-lookup"><span data-stu-id="da950-142">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="da950-143">CSP プログラムのパートナーとして、お客様に購入したプランの無料試用期間を免除することはできません。</span><span class="sxs-lookup"><span data-stu-id="da950-143">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="da950-144">無料試用期間が終了すると、サブスクリプション期間が開始され、サブスクリプションが有料ステータスに変換されます。</span><span class="sxs-lookup"><span data-stu-id="da950-144">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="da950-145">その後、サブスクリプションは同じスケジュールに従って自動更新されます。</span><span class="sxs-lookup"><span data-stu-id="da950-145">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="da950-146">アドオンでサブスクリプションを更新する</span><span class="sxs-lookup"><span data-stu-id="da950-146">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="da950-147">アドオンを購入するには、顧客が最初にアクティブなベース サブスクリプションを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="da950-147">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="da950-148">カタログを通じてアドオンを購入することはできません。</span><span class="sxs-lookup"><span data-stu-id="da950-148">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="da950-149">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="da950-149">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="da950-150">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="da950-150">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="da950-151">管理対象のサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="da950-151">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="da950-152">[状態 **] セクション** の下に、サブスクリプションで使用可能なアドオンの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="da950-152">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="da950-153">必要なアドオンごとにライセンスの数量を更新します。</span><span class="sxs-lookup"><span data-stu-id="da950-153">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="da950-154">次に、変更内容を **送信** します。</span><span class="sxs-lookup"><span data-stu-id="da950-154">Then **Submit** your changes.</span></span>

<span data-ttu-id="da950-155">サービスを通じてアドオンを購入する機能パートナー センター直接請求プロバイダーと間接プロバイダーでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="da950-155">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="da950-156">基本要件とリージョンの可用性に基づいて表示されるのは、対象となるアドオンのみです。</span><span class="sxs-lookup"><span data-stu-id="da950-156">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="da950-157">価格とオファーの詳細については、Cloud Reseller のオファー マトリックスを参照してください。</span><span class="sxs-lookup"><span data-stu-id="da950-157">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="da950-158">ベース サブスクリプションを中断すると、関連するすべてのアドオンも中断されます。</span><span class="sxs-lookup"><span data-stu-id="da950-158">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="da950-159">アドオンの開始日はベース サブスクリプションに合わせられ、料金は最初の請求書において請求開始日から請求終了日の対する比例配分で計算されます。</span><span class="sxs-lookup"><span data-stu-id="da950-159">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="da950-160">詳細については、「ライセンスベースの [課金」を参照してください](license-based-billing.md)。</span><span class="sxs-lookup"><span data-stu-id="da950-160">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="da950-161">サブスクリプションを中断または取り消す</span><span class="sxs-lookup"><span data-stu-id="da950-161">Suspend or cancel a subscription</span></span>

<span data-ttu-id="da950-162">顧客から要請があった場合、または未払いや詐欺が発生した場合、パートナーはサブスクリプションを中断するか取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="da950-162">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="da950-163">サブスクリプションの中断</span><span class="sxs-lookup"><span data-stu-id="da950-163">Suspend a subscription</span></span>

<span data-ttu-id="da950-164">サブスクリプションの状態を **[中断]** に変更すると、ユーザーはサインインしたり、サービスにアクセスしたりできなくなります。</span><span class="sxs-lookup"><span data-stu-id="da950-164">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="da950-165">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="da950-165">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="da950-166">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="da950-166">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="da950-167">管理対象のサブスクリプションを選びます。</span><span class="sxs-lookup"><span data-stu-id="da950-167">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="da950-168">**[状態]** セクションで **[保留]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="da950-168">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="da950-169">次に、変更内容を **送信** します。</span><span class="sxs-lookup"><span data-stu-id="da950-169">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="da950-170">90 日以内、または 90 日にアカウントが開かれた時点から最初の課金までの日数を加えた期間 (最大 120 日) 以内にサブスクリプションを再アクティブ化しない限り、すべてのデータは削除されます。</span><span class="sxs-lookup"><span data-stu-id="da950-170">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="da950-171">サブスクリプションを中断するときに、**[中断]** ボタンの下に表示される日付は、サブスクリプションを再アクティブ化しない場合に自動的に期限切れになる日付です。</span><span class="sxs-lookup"><span data-stu-id="da950-171">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="da950-172">CSP サブスクリプションには、サービスが引き続き機能している期間 (Web ダイレクト サブスクリプションの場合と同じ方法) が期限切れになるのではなく、サブスクリプションによって課金料金が生成されません。</span><span class="sxs-lookup"><span data-stu-id="da950-172">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="da950-173">CSP サブスクリプションは、アクティブまたは中断 (または完全に削除) されます。</span><span class="sxs-lookup"><span data-stu-id="da950-173">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="da950-174">サブスクリプションを取り消す</span><span class="sxs-lookup"><span data-stu-id="da950-174">Cancel a subscription</span></span>

<span data-ttu-id="da950-175">ライセンスベースの SaaS サブスクリプションは、コマーシャル マーケットプレース 内のサード パーティの ISV パートナー センター [取り消しできます](csp-commercial-marketplace-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="da950-175">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="da950-176">キャンセル期間中に取り消す限り、完全な払い戻しを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="da950-176">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="da950-177">ISV オファーの場合は、毎月請求されます。</span><span class="sxs-lookup"><span data-stu-id="da950-177">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="da950-178">注文後 24 時間以内にキャンセルした場合は、次の請求書に対して完全なクレジットを受け取る予定です。</span><span class="sxs-lookup"><span data-stu-id="da950-178">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="da950-179">注文後 24 時間より後にキャンセルした場合、キャンセルは更新時に行われる予定です。</span><span class="sxs-lookup"><span data-stu-id="da950-179">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="da950-180">年間請求されるオファーの場合:</span><span class="sxs-lookup"><span data-stu-id="da950-180">For offers billed annually:</span></span>

- <span data-ttu-id="da950-181">注文から 14 日未満でキャンセルした場合は、次の請求書に対して完全なクレジットを受け取ることになります。</span><span class="sxs-lookup"><span data-stu-id="da950-181">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="da950-182">注文後 14 日より後にキャンセルした場合、キャンセルは更新時に行われる予定です。</span><span class="sxs-lookup"><span data-stu-id="da950-182">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="da950-183">これらの期間が終了すると、サブスクリプションを取り消すオプションは表示されなくなりました。</span><span class="sxs-lookup"><span data-stu-id="da950-183">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="da950-184">使用量ベースおよび測定されたサード パーティの ISV サービス (仮想マシンやコンテナーを使用するサービスなど) は、返品の対象ではありません。</span><span class="sxs-lookup"><span data-stu-id="da950-184">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="da950-185">使用量ベースのサービスは、取り消し方法としてプロビジョニング解除できます。</span><span class="sxs-lookup"><span data-stu-id="da950-185">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="da950-186">料金は使用後に課金されます。このため、これらのサービスは返金の対象ではありません。</span><span class="sxs-lookup"><span data-stu-id="da950-186">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="da950-187">ISV 発行元から取得したライセンスベースの SaaS サブスクリプションを取り消すには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="da950-187">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="da950-188">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="da950-188">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="da950-189">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="da950-189">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="da950-190">取り消すサブスクリプションを見つける。</span><span class="sxs-lookup"><span data-stu-id="da950-190">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="da950-191">[状態] **列で** 、[キャンセル] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="da950-191">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="da950-192">次に、変更内容を **送信** します。</span><span class="sxs-lookup"><span data-stu-id="da950-192">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="da950-193">ダイアログ ボックスが表示されたら、関連する詳細を入力し、[送信] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="da950-193">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="da950-194">取り消しを確定するには、[はい、キャンセル **] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="da950-194">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="da950-195">また、API を使用してサブスクリプションのAzure Marketplaceを取り消す方法を選択できます。</span><span class="sxs-lookup"><span data-stu-id="da950-195">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="da950-196">これを行うには、「サブスクリプションのキャンセル [」をAzure Marketplaceしてください](/partner-center/develop/cancel-an-azure-marketplace-subscription)。</span><span class="sxs-lookup"><span data-stu-id="da950-196">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="da950-197">商用マーケットプレースのサブスクリプションを自動的に更新するかどうかを選択する</span><span class="sxs-lookup"><span data-stu-id="da950-197">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="da950-198">既定では、アクティブなサブスクリプションは、サブスクリプション期間の期限が切れると自動的に更新するように設定されます。</span><span class="sxs-lookup"><span data-stu-id="da950-198">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="da950-199">コマーシャル [マーケットプレース製品のサブスクリプションの](csp-commercial-marketplace-overview.md)場合は、必要に応じて、サブスクリプションを自動的に更新しない方法を選択できます。</span><span class="sxs-lookup"><span data-stu-id="da950-199">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="da950-200">アクティブなコマーシャル マーケットプレース サブスクリプションの自動更新を停止するには:</span><span class="sxs-lookup"><span data-stu-id="da950-200">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="da950-201">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="da950-201">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="da950-202">パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。</span><span class="sxs-lookup"><span data-stu-id="da950-202">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="da950-203">**[サブスクリプション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="da950-203">Select **Subscriptions**.</span></span> <span data-ttu-id="da950-204">これにより、顧客に対して購入したライセンス ベースのサブスクリプションが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="da950-204">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="da950-205">[サブスクリプション **]** 列で、変更するサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="da950-205">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="da950-206">サブスクリプションの詳細ページで、[状態] セクション **を見つけて** 、[ **自動更新] ボックスをオフ** にします。</span><span class="sxs-lookup"><span data-stu-id="da950-206">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="da950-207">**[Submit]\(送信\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="da950-207">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="da950-208">次のステップ</span><span class="sxs-lookup"><span data-stu-id="da950-208">Next steps</span></span>

- [<span data-ttu-id="da950-209">顧客のために商用マーケットプレースの製品を購入する</span><span class="sxs-lookup"><span data-stu-id="da950-209">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="da950-210">顧客向けコマーシャル マーケットプレース製品を管理する</span><span class="sxs-lookup"><span data-stu-id="da950-210">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="da950-211">商業マーケットプレースの概要</span><span class="sxs-lookup"><span data-stu-id="da950-211">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)