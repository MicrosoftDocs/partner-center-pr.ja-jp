---
title: Microsoft 顧客契約に対する顧客の同意を確認する
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Microsoft 顧客契約に対する顧客の同意を確認する方法について説明します。 これは、顧客のために Microsoft の製品やサービスを注文するのに必要になる場合があります。
author: LauraBrenner
ms.author: labrenne
keywords: 顧客, お客様, 同意, MCA, Microsoft 顧客契約, 顧客契約テンプレート
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9d45f04c8ee1a8d8715f5c6484598ecaca83b1f1
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908149"
---
# <a name="overview-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="d65fc-105">概要:Microsoft 顧客契約に対する顧客の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="d65fc-105">Overview: Confirm customer acceptance of the Microsoft Customer Agreement</span></span>

<span data-ttu-id="d65fc-106">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="d65fc-106">**Applies to**</span></span>
-  <span data-ttu-id="d65fc-107">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="d65fc-107">Partner Center</span></span>

<span data-ttu-id="d65fc-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="d65fc-108">**Appropriate roles**</span></span>

- <span data-ttu-id="d65fc-109">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="d65fc-109">Admin agent</span></span>
- <span data-ttu-id="d65fc-110">販売代理店</span><span class="sxs-lookup"><span data-stu-id="d65fc-110">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="d65fc-111">契約リソースは、現在、Microsoft パブリック クラウドのパートナー センターでのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="d65fc-111">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="d65fc-112">以下には適用されません。</span><span class="sxs-lookup"><span data-stu-id="d65fc-112">It is not applicable to:</span></span>
> * <span data-ttu-id="d65fc-113">21Vianet が運営するパートナー センター</span><span class="sxs-lookup"><span data-stu-id="d65fc-113">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="d65fc-114">Microsoft Cloud ドイツのパートナー センター</span><span class="sxs-lookup"><span data-stu-id="d65fc-114">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="d65fc-115">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="d65fc-115">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="d65fc-116">2020 年 1 月 31 日の時点で、すべてのお客様 (既存および新規) は新しい Microsoft 顧客契約に署名する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d65fc-116">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="d65fc-117">詳細については、「[Microsoft 顧客契約に対する顧客の同意を確認する](confirm-customer-agreement.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d65fc-117">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="d65fc-118">パートナーは、お客様のために Microsoft の製品やサービスを注文する前に、Microsoft 顧客契約へのそのお客様の同意を得る必要があります。</span><span class="sxs-lookup"><span data-stu-id="d65fc-118">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="d65fc-119">パートナーがコンプライアンス要件を満たすことができるように、マイクロソフトでは、パートナーに対して、契約に同意したユーザーに関する以下の詳細情報を提供することにより、同意を確認することを求めています。</span><span class="sxs-lookup"><span data-stu-id="d65fc-119">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="d65fc-120">名</span><span class="sxs-lookup"><span data-stu-id="d65fc-120">First name</span></span>

- <span data-ttu-id="d65fc-121">姓</span><span class="sxs-lookup"><span data-stu-id="d65fc-121">Last name</span></span>

- <span data-ttu-id="d65fc-122">電子メール アドレス</span><span class="sxs-lookup"><span data-stu-id="d65fc-122">Email address</span></span>

- <span data-ttu-id="d65fc-123">電話番号 (オプション)</span><span class="sxs-lookup"><span data-stu-id="d65fc-123">Phone number (optional)</span></span>

- <span data-ttu-id="d65fc-124">同意の日付</span><span class="sxs-lookup"><span data-stu-id="d65fc-124">Date of acceptance</span></span>

<span data-ttu-id="d65fc-125">直接請求パートナーと間接プロバイダーは、パートナー センターまたはパートナー センター API 経由で取引するときに、Microsoft 顧客契約へのお客様の同意を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d65fc-125">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="d65fc-126">確認は*必須*です。</span><span class="sxs-lookup"><span data-stu-id="d65fc-126">Confirmation is *mandatory*.</span></span>

<span data-ttu-id="d65fc-127">特定のお客様について確認が提供されていない場合:</span><span class="sxs-lookup"><span data-stu-id="d65fc-127">If confirmation is not provided for a given customer:</span></span>

-    <span data-ttu-id="d65fc-128">このお客様について新しい注文を作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="d65fc-128">You won't be able to create new orders for this customer.</span></span>

-    <span data-ttu-id="d65fc-129">このお客様について既存のシート ベースのサブスクリプションのシート数を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="d65fc-129">You won't be able to change the seat count of existing seat-based subscriptions for this customer.</span></span>

<span data-ttu-id="d65fc-130">お客様の同意は、パートナー センターまたはパートナー センター API を使用して確認できます。</span><span class="sxs-lookup"><span data-stu-id="d65fc-130">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="d65fc-131">パートナー センター API でこれを行うには、以下のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d65fc-131">To do this through the Partner Center API, see the following topics:</span></span> 

-   [<span data-ttu-id="d65fc-132">顧客の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="d65fc-132">Get confirmation of customer consent</span></span>](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [<span data-ttu-id="d65fc-133">契約メタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="d65fc-133">Get agreement metadata</span></span>](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [<span data-ttu-id="d65fc-134">顧客の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="d65fc-134">Confirm customer consent</span></span>](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


<span data-ttu-id="d65fc-135">これは、運用環境とサンド ボックス環境の両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d65fc-135">This applies to both production and sandbox environments.</span></span>

## <a name="confirming-customer-acceptance-in-partner-center"></a><span data-ttu-id="d65fc-136">パートナー センターを使用してお客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="d65fc-136">Confirming customer acceptance in Partner Center</span></span>

### <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="d65fc-137">新しいお客様についてお客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="d65fc-137">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="d65fc-138">パートナー センターで、新しいお客様のテナントを作成するときに、お客様の同意を確認するのには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="d65fc-138">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="d65fc-139">これを行うには、管理エージェントまたは販売エージェントである必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="d65fc-139">Note that you must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="d65fc-140">**[顧客]** 、 **[新しい顧客]** 、 **[アカウント情報]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-140">Select **Customers**, and then **New customer** and then select **Account info**.</span></span>
2. <span data-ttu-id="d65fc-141">**会社**と**主要連絡先**に関する情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-141">Enter the information about the **Company** and **Primary contact**.</span></span>

![会社情報](images/mca/mca1.png)

3. <span data-ttu-id="d65fc-143">**[Microsoft 顧客契約]** で、 **[The customer has accepted the latest Microsoft customer agreement] (お客様は最新の Microsoft 顧客契約に同意しました)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-143">Under **Microsoft customer agreement**, select **The customer has accepted the latest Microsoft customer agreement**.</span></span>
4. <span data-ttu-id="d65fc-144">**[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-144">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="d65fc-145">将来の日付に設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="d65fc-145">You cannot set this to a future date.</span></span>
5. <span data-ttu-id="d65fc-146">同意しているユーザーの詳細を入力します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-146">Enter the details of the user who provided the acceptance.</span></span>

![同意の日付を追加する](images/mca/MCA3.png)

<span data-ttu-id="d65fc-148">既定では、第一連絡先担当者のユーザー情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="d65fc-148">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="d65fc-149">これが正しくない場合は、 **[更新]** を選択し、契約に同意したユーザーの **[名]** 、 **[姓]** 、 **[メール アドレス]** 、\* *[電話番号]* (省略可能) を入力します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-149">If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and \**Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="d65fc-150">**[次へ]** を選択して、お客様のテナントを作成する残りの手順を続行します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-150">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="d65fc-151">既存のお客様についてお客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="d65fc-151">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="d65fc-152">これを行うには、管理エージェントまたは販売エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="d65fc-152">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="d65fc-153">**[顧客]** を選択し、表示するお客様を検索して選択します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-153">Select **Customers**, and then find and select the customer you want to see.</span></span>
2. <span data-ttu-id="d65fc-154">**[アカウント情報]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-154">Select **Account info**.</span></span>
3. <span data-ttu-id="d65fc-155">**[Microsoft 顧客契約]** で、 **[更新]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-155">Under **Microsoft customer agreement**, select **Update**.</span></span>

![更新プログラム、更新](images/mca/mca4.png)

4. <span data-ttu-id="d65fc-157">契約に同意したユーザーの**名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-157">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>
5. <span data-ttu-id="d65fc-158">**[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-158">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="d65fc-159">将来の日付に設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="d65fc-159">You cannot set this to a future date.</span></span>
6. <span data-ttu-id="d65fc-160">**[Save and continue]** (保存して続行) を選択します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-160">Select **Save and continue**.</span></span>

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="d65fc-161">既存のお客様について新しい注文の作成中にお客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="d65fc-161">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="d65fc-162">まだ確認していない既存のお客様について新しい注文を作成しようとすると、確認を完了するよう求めるプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="d65fc-162">If you try to create a new order for an existing customer which you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="d65fc-163">この場合、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-163">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="d65fc-164">契約に同意したユーザーの**名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-164">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>
2. <span data-ttu-id="d65fc-165">**[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-165">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="d65fc-166">将来の日付に設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="d65fc-166">You cannot set this to a future date.</span></span>
3. <span data-ttu-id="d65fc-167">**[Save and continue]** (保存して続行) を選択します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-167">Select **Save and continue**.</span></span>

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="d65fc-168">既存のお客様についてお客様の同意の確認を取得する</span><span class="sxs-lookup"><span data-stu-id="d65fc-168">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="d65fc-169">以下の手順を使用して、既存のお客様について以前に提供したお客様の同意確認を取得することができます。</span><span class="sxs-lookup"><span data-stu-id="d65fc-169">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="d65fc-170">これを行うには、管理エージェントまたは販売エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="d65fc-170">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="d65fc-171">**[顧客]** を選択し、表示するお客様を検索して選択します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-171">Select **Customers**, and then find and select the customer you want to see.</span></span>
2. <span data-ttu-id="d65fc-172">**[アカウント情報]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="d65fc-172">Select **Account info**.</span></span>
3. <span data-ttu-id="d65fc-173">**[Microsoft 顧客契約]** に、このお客様について確認が得られているかどうかが表示されます。</span><span class="sxs-lookup"><span data-stu-id="d65fc-173">Under **Microsoft customer agreement**, you'll see whether or not confirmation has been provided for this customer.</span></span>
