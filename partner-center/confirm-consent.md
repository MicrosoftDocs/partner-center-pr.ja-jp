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
ms.openlocfilehash: aacca72e9af45b2777364734c2b07dbe8101989d
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/19/2020
ms.locfileid: "92333920"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="e79ca-104">Microsoft 顧客契約に対するお客様の同意を確認する方法 (更新版)</span><span class="sxs-lookup"><span data-stu-id="e79ca-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>

<span data-ttu-id="e79ca-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="e79ca-105">**Applies to**</span></span>

-  <span data-ttu-id="e79ca-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="e79ca-106">Partner Center</span></span>

<span data-ttu-id="e79ca-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="e79ca-107">**Appropriate roles**</span></span>

- <span data-ttu-id="e79ca-108">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="e79ca-108">Admin agent</span></span>
- <span data-ttu-id="e79ca-109">販売代理店</span><span class="sxs-lookup"><span data-stu-id="e79ca-109">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="e79ca-110">契約リソースは、現在、Microsoft パブリック クラウドのパートナー センターでのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="e79ca-110">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="e79ca-111">以下には適用されません。</span><span class="sxs-lookup"><span data-stu-id="e79ca-111">It is not applicable to:</span></span>
> * <span data-ttu-id="e79ca-112">21Vianet が運営するパートナー センター</span><span class="sxs-lookup"><span data-stu-id="e79ca-112">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="e79ca-113">Microsoft Cloud ドイツのパートナー センター</span><span class="sxs-lookup"><span data-stu-id="e79ca-113">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="e79ca-114">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="e79ca-114">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="e79ca-115">2020 年 1 月 31 日の時点で、すべてのお客様 (既存および新規) は新しい Microsoft 顧客契約に署名する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e79ca-115">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="e79ca-116">詳細については、「[Microsoft 顧客契約に対する顧客の同意を確認する](confirm-customer-agreement.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e79ca-116">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="e79ca-117">パートナーは、お客様のために Microsoft の製品やサービスを注文する前に、Microsoft 顧客契約へのそのお客様の同意を得る必要があります。</span><span class="sxs-lookup"><span data-stu-id="e79ca-117">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="e79ca-118">パートナーがコンプライアンス要件を満たすことができるように、マイクロソフトでは、パートナーに対して、契約に同意したユーザーに関する以下の詳細情報を提供することにより、同意を確認することを求めています。</span><span class="sxs-lookup"><span data-stu-id="e79ca-118">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="e79ca-119">名</span><span class="sxs-lookup"><span data-stu-id="e79ca-119">First name</span></span>

- <span data-ttu-id="e79ca-120">姓</span><span class="sxs-lookup"><span data-stu-id="e79ca-120">Last name</span></span>

- <span data-ttu-id="e79ca-121">電子メール アドレス</span><span class="sxs-lookup"><span data-stu-id="e79ca-121">Email address</span></span>

- <span data-ttu-id="e79ca-122">電話番号 (オプション)</span><span class="sxs-lookup"><span data-stu-id="e79ca-122">Phone number (optional)</span></span>

- <span data-ttu-id="e79ca-123">同意の日付</span><span class="sxs-lookup"><span data-stu-id="e79ca-123">Date of acceptance</span></span>

<span data-ttu-id="e79ca-124">直接請求パートナーと間接プロバイダーは、パートナー センターまたはパートナー センター API 経由で取引するときに、Microsoft 顧客契約へのお客様の同意を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e79ca-124">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="e79ca-125">確認は *必須* です。</span><span class="sxs-lookup"><span data-stu-id="e79ca-125">Confirmation is *mandatory* .</span></span>

<span data-ttu-id="e79ca-126">特定のお客様について確認が提供されていない場合:</span><span class="sxs-lookup"><span data-stu-id="e79ca-126">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="e79ca-127">このお客様について新しい注文を作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="e79ca-127">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="e79ca-128">このお客様について既存のライセンス ベースのサブスクリプションのライセンス数を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="e79ca-128">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="e79ca-129">お客様の同意は、パートナー センターまたはパートナー センター API を使用して確認できます。</span><span class="sxs-lookup"><span data-stu-id="e79ca-129">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="e79ca-130">パートナー センター API でこれを行うには、以下のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e79ca-130">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="e79ca-131">顧客の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="e79ca-131">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="e79ca-132">契約メタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="e79ca-132">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="e79ca-133">顧客の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="e79ca-133">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="e79ca-134">これは、運用環境とサンド ボックス環境の両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e79ca-134">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="e79ca-135">新しいお客様についてお客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="e79ca-135">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="e79ca-136">パートナー センターで、新しいお客様のテナントを作成するときに、お客様の同意を確認するのには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="e79ca-136">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="e79ca-137">これを行うには、管理エージェントまたは販売エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="e79ca-137">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="e79ca-138">**[顧客]** 、 **[新しい顧客]** 、 **[アカウント情報]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-138">Select **Customers** , and then **New customer** and then select **Account info** .</span></span>

2. <span data-ttu-id="e79ca-139">**会社** と **主要連絡先** に関する情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-139">Enter the information about the **Company** and **Primary contact** .</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="会社情報":::

3. <span data-ttu-id="e79ca-141">**[Microsoft 顧客契約]** で、 **[The customer has accepted the latest Microsoft customer agreement] (お客様は最新の Microsoft 顧客契約に同意しました)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-141">Under **Microsoft customer agreement** , select **The customer has accepted the latest Microsoft customer agreement** .</span></span>

4. <span data-ttu-id="e79ca-142">**[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-142">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="e79ca-143">将来の日付に設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="e79ca-143">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="e79ca-144">同意しているユーザーの詳細を入力します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-144">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="同意の日付を追加する":::

   <span data-ttu-id="e79ca-146">既定では、第一連絡先担当者のユーザー情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="e79ca-146">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="e79ca-147">これが正しくない場合は、 **[更新]** を選択し、契約に同意したユーザーの **[名]** 、 **[姓]** 、 **[メール アドレス]** 、\* *[電話番号]* (省略可能) を入力します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-147">If this isn't correct, select **Update** and then enter the **First name** , **Last name** , **Email address** , and \* *Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="e79ca-148">**[次へ]** を選択して、お客様のテナントを作成する残りの手順を続行します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-148">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="e79ca-149">既存のお客様についてお客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="e79ca-149">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="e79ca-150">これを行うには、管理エージェントまたは販売エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="e79ca-150">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="e79ca-151">**[顧客]** を選択し、表示するお客様を検索して選択します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-151">Select **Customers** , and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="e79ca-152">**[アカウント情報]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-152">Select **Account info** .</span></span>

3. <span data-ttu-id="e79ca-153">**[Microsoft 顧客契約]** で、 **[更新]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-153">Under **Microsoft customer agreement** , select **Update** .</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="アップデート":::

4. <span data-ttu-id="e79ca-155">契約に同意したユーザーの **名** 、 **姓** 、 **メール アドレス** 、 **電話番号** (省略可能) を入力します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-155">Enter the **First name** , **Last name** , **Email address** , and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="e79ca-156">**[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-156">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="e79ca-157">将来の日付に設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="e79ca-157">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="e79ca-158">**[Save and continue]** (保存して続行) を選択します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-158">Select **Save and continue** .</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="e79ca-159">既存のお客様について新しい注文の作成中にお客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="e79ca-159">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="e79ca-160">まだ確認していない既存のお客様について新しい注文を作成しようとすると、確認を完了するよう求めるプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="e79ca-160">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="e79ca-161">この場合、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-161">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="e79ca-162">契約に同意したユーザーの **名** 、 **姓** 、 **メール アドレス** 、 **電話番号** (省略可能) を入力します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-162">Enter the **First name** , **Last name** , **Email address** , and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="e79ca-163">**[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-163">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="e79ca-164">将来の日付に設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="e79ca-164">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="e79ca-165">**[Save and continue]** (保存して続行) を選択します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-165">Select **Save and continue** .</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="e79ca-166">既存のお客様についてお客様の同意の確認を取得する</span><span class="sxs-lookup"><span data-stu-id="e79ca-166">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="e79ca-167">以下の手順を使用して、既存のお客様について以前に提供したお客様の同意確認を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="e79ca-167">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="e79ca-168">これを行うには、管理エージェントまたは販売エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="e79ca-168">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="e79ca-169">**[顧客]** を選択し、表示するお客様を検索して選択します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-169">Select **Customers** , and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="e79ca-170">**[アカウント情報]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e79ca-170">Select **Account info** .</span></span>

3. <span data-ttu-id="e79ca-171">**[Microsoft 顧客契約]** に、このお客様について確認が得られているかどうかが表示されます。</span><span class="sxs-lookup"><span data-stu-id="e79ca-171">Under **Microsoft customer agreement** , you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e79ca-172">次のステップ</span><span class="sxs-lookup"><span data-stu-id="e79ca-172">Next steps</span></span>

- [<span data-ttu-id="e79ca-173">CSP パートナー プログラムで Microsoft 顧客契約への顧客の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="e79ca-173">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="e79ca-174">顧客に代わって Microsoft 顧客契約の同意を証明する</span><span class="sxs-lookup"><span data-stu-id="e79ca-174">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)