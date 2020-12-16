---
title: Microsoft 顧客契約へのお客様の同意を確認する
description: Microsoft 顧客契約に対する顧客の同意を確認する方法について説明します。 これは、顧客のために Microsoft の製品やサービスを注文するのに必要になる場合があります。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: f2513213bff38a6296832253a13725ff2508f1f8
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354612"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="36ce8-104">Microsoft 顧客契約に対するお客様の同意を確認する方法 (更新版)</span><span class="sxs-lookup"><span data-stu-id="36ce8-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>


<span data-ttu-id="36ce8-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="36ce8-105">**Appropriate roles**</span></span>

- <span data-ttu-id="36ce8-106">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="36ce8-106">Admin agent</span></span>
- <span data-ttu-id="36ce8-107">販売代理店</span><span class="sxs-lookup"><span data-stu-id="36ce8-107">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="36ce8-108">契約リソースは、現在、Microsoft パブリック クラウドのパートナー センターでのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="36ce8-108">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="36ce8-109">以下には適用されません。</span><span class="sxs-lookup"><span data-stu-id="36ce8-109">It is not applicable to:</span></span>
> * <span data-ttu-id="36ce8-110">21Vianet が運営するパートナー センター</span><span class="sxs-lookup"><span data-stu-id="36ce8-110">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="36ce8-111">Microsoft Cloud ドイツのパートナー センター</span><span class="sxs-lookup"><span data-stu-id="36ce8-111">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="36ce8-112">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="36ce8-112">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="36ce8-113">2020 年 1 月 31 日の時点で、すべてのお客様 (既存および新規) は新しい Microsoft 顧客契約に署名する必要があります。</span><span class="sxs-lookup"><span data-stu-id="36ce8-113">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="36ce8-114">詳細については、「[Microsoft 顧客契約に対する顧客の同意を確認する](confirm-customer-agreement.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36ce8-114">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="36ce8-115">パートナーは、お客様のために Microsoft の製品やサービスを注文する前に、Microsoft 顧客契約へのそのお客様の同意を得る必要があります。</span><span class="sxs-lookup"><span data-stu-id="36ce8-115">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="36ce8-116">パートナーがコンプライアンス要件を満たすことができるように、マイクロソフトでは、パートナーに対して、契約に同意したユーザーに関する以下の詳細情報を提供することにより、同意を確認することを求めています。</span><span class="sxs-lookup"><span data-stu-id="36ce8-116">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="36ce8-117">名</span><span class="sxs-lookup"><span data-stu-id="36ce8-117">First name</span></span>

- <span data-ttu-id="36ce8-118">姓</span><span class="sxs-lookup"><span data-stu-id="36ce8-118">Last name</span></span>

- <span data-ttu-id="36ce8-119">電子メール アドレス</span><span class="sxs-lookup"><span data-stu-id="36ce8-119">Email address</span></span>

- <span data-ttu-id="36ce8-120">電話番号 (オプション)</span><span class="sxs-lookup"><span data-stu-id="36ce8-120">Phone number (optional)</span></span>

- <span data-ttu-id="36ce8-121">同意の日付</span><span class="sxs-lookup"><span data-stu-id="36ce8-121">Date of acceptance</span></span>

<span data-ttu-id="36ce8-122">直接請求パートナーと間接プロバイダーは、パートナー センターまたはパートナー センター API 経由で取引するときに、Microsoft 顧客契約へのお客様の同意を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="36ce8-122">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="36ce8-123">確認は *必須* です。</span><span class="sxs-lookup"><span data-stu-id="36ce8-123">Confirmation is *mandatory*.</span></span>

<span data-ttu-id="36ce8-124">特定のお客様について確認が提供されていない場合:</span><span class="sxs-lookup"><span data-stu-id="36ce8-124">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="36ce8-125">このお客様について新しい注文を作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="36ce8-125">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="36ce8-126">このお客様について既存のライセンス ベースのサブスクリプションのライセンス数を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="36ce8-126">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="36ce8-127">お客様の同意は、パートナー センターまたはパートナー センター API を使用して確認できます。</span><span class="sxs-lookup"><span data-stu-id="36ce8-127">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="36ce8-128">パートナー センター API でこれを行うには、以下のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="36ce8-128">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="36ce8-129">顧客の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="36ce8-129">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="36ce8-130">契約メタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="36ce8-130">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="36ce8-131">顧客の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="36ce8-131">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="36ce8-132">これは、運用環境とサンド ボックス環境の両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="36ce8-132">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="36ce8-133">新しいお客様についてお客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="36ce8-133">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="36ce8-134">パートナー センターで、新しいお客様のテナントを作成するときに、お客様の同意を確認するのには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="36ce8-134">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="36ce8-135">これを行うには、管理エージェントまたは販売エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="36ce8-135">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="36ce8-136">**[顧客]** 、 **[新しい顧客]** 、 **[アカウント情報]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-136">Select **Customers**, and then **New customer** and then select **Account info**.</span></span>

2. <span data-ttu-id="36ce8-137">**会社** と **主要連絡先** に関する情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-137">Enter the information about the **Company** and **Primary contact**.</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="会社情報":::

3. <span data-ttu-id="36ce8-139">**[Microsoft 顧客契約]** で、 **[The customer has accepted the latest Microsoft customer agreement] (お客様は最新の Microsoft 顧客契約に同意しました)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-139">Under **Microsoft customer agreement**, select **The customer has accepted the latest Microsoft customer agreement**.</span></span>

4. <span data-ttu-id="36ce8-140">**[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-140">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="36ce8-141">将来の日付に設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="36ce8-141">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="36ce8-142">同意しているユーザーの詳細を入力します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-142">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="同意の日付を追加する":::

   <span data-ttu-id="36ce8-144">既定では、第一連絡先担当者のユーザー情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="36ce8-144">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="36ce8-145">これが正しくない場合は、 **[更新]** を選択し、契約に同意したユーザーの **[名]** 、 **[姓]** 、 **[メール アドレス]** 、\* *[電話番号]* (省略可能) を入力します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-145">If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and \**Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="36ce8-146">**[次へ]** を選択して、お客様のテナントを作成する残りの手順を続行します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-146">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="36ce8-147">既存のお客様についてお客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="36ce8-147">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="36ce8-148">これを行うには、管理エージェントまたは販売エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="36ce8-148">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="36ce8-149">**[顧客]** を選択し、表示するお客様を検索して選択します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-149">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="36ce8-150">**[アカウント情報]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-150">Select **Account info**.</span></span>

3. <span data-ttu-id="36ce8-151">**[Microsoft 顧客契約]** で、 **[更新]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-151">Under **Microsoft customer agreement**, select **Update**.</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="アップデート":::

4. <span data-ttu-id="36ce8-153">契約に同意したユーザーの **名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-153">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="36ce8-154">**[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-154">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="36ce8-155">将来の日付に設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="36ce8-155">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="36ce8-156">**[Save and continue]** (保存して続行) を選択します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-156">Select **Save and continue**.</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="36ce8-157">既存のお客様について新しい注文の作成中にお客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="36ce8-157">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="36ce8-158">まだ確認していない既存のお客様について新しい注文を作成しようとすると、確認を完了するよう求めるプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="36ce8-158">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="36ce8-159">この場合、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-159">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="36ce8-160">契約に同意したユーザーの **名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-160">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="36ce8-161">**[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-161">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="36ce8-162">将来の日付に設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="36ce8-162">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="36ce8-163">**[Save and continue]** (保存して続行) を選択します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-163">Select **Save and continue**.</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="36ce8-164">既存のお客様についてお客様の同意の確認を取得する</span><span class="sxs-lookup"><span data-stu-id="36ce8-164">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="36ce8-165">以下の手順を使用して、既存のお客様について以前に提供したお客様の同意確認を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="36ce8-165">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="36ce8-166">これを行うには、管理エージェントまたは販売エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="36ce8-166">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="36ce8-167">**[顧客]** を選択し、表示するお客様を検索して選択します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-167">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="36ce8-168">**[アカウント情報]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="36ce8-168">Select **Account info**.</span></span>

3. <span data-ttu-id="36ce8-169">**[Microsoft 顧客契約]** に、このお客様について確認が得られているかどうかが表示されます。</span><span class="sxs-lookup"><span data-stu-id="36ce8-169">Under **Microsoft customer agreement**, you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="36ce8-170">次のステップ</span><span class="sxs-lookup"><span data-stu-id="36ce8-170">Next steps</span></span>

- [<span data-ttu-id="36ce8-171">CSP パートナー プログラムで Microsoft 顧客契約への顧客の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="36ce8-171">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="36ce8-172">顧客に代わって Microsoft 顧客契約の同意を証明する</span><span class="sxs-lookup"><span data-stu-id="36ce8-172">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)