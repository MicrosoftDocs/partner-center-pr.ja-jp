---
title: 顧客が CSP プログラムの Microsoft 顧客契約に同意していることを確認する方法
description: クラウド ソリューション プロバイダー (CSP) パートナーは、顧客に代わって Microsoft サービスを注文する前に、Microsoft 顧客契約への顧客の同意を確認する必要があります。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633780"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="dba82-103">顧客が CSP プログラムの Microsoft 顧客契約に同意していることを確認する方法</span><span class="sxs-lookup"><span data-stu-id="dba82-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="dba82-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="dba82-104">**Appropriate roles**</span></span>

- <span data-ttu-id="dba82-105">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="dba82-105">Admin agent</span></span>
- <span data-ttu-id="dba82-106">販売代理店</span><span class="sxs-lookup"><span data-stu-id="dba82-106">Sales agent</span></span>


<span data-ttu-id="dba82-107">顧客が Microsoft 顧客契約に同意するには、次の 2 つのオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="dba82-107">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="dba82-108">**オプション 1**:顧客の同意に対するパートナー証明 - パートナーは、パートナー センター API/SDK を使用するか、パートナー センター ダッシュボードを使用して、顧客の同意を確認できます。</span><span class="sxs-lookup"><span data-stu-id="dba82-108">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="dba82-109">**オプション 2**:顧客の直接同意 - パートナーは、URL を使用して、Microsoft 365 管理センターで契約を確認し、同意するように顧客に要請できます。</span><span class="sxs-lookup"><span data-stu-id="dba82-109">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="dba82-110">Microsoft 顧客契約テンプレートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="dba82-110">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="dba82-111">最新バージョンの Microsoft 顧客契約テンプレートは、[こちら](https://aka.ms/customeragreement)から手動でダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="dba82-111">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="dba82-112">Microsoft 顧客契約は国によって異なります。</span><span class="sxs-lookup"><span data-stu-id="dba82-112">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="dba82-113">Microsoft 顧客契約テンプレートを要求するときは、顧客の所在地に応じて正しい国を選択してください。</span><span class="sxs-lookup"><span data-stu-id="dba82-113">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="dba82-114">オプション 1:パートナー センターを使用してお客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="dba82-114">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="dba82-115">直接請求パートナーは、新規の顧客と既存の顧客について、パートナー センターで Microsoft 顧客契約に対する顧客の同意を確認できます。</span><span class="sxs-lookup"><span data-stu-id="dba82-115">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="dba82-116">間接リセラーは顧客に代わって証明を行うことができません。間接プロバイダーと協力して、証明を完了する必要があります。</span><span class="sxs-lookup"><span data-stu-id="dba82-116">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="dba82-117">新しいお客様について、お客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="dba82-117">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="dba82-118">パートナー センターで新しい顧客テナントを作成するときに、次の手順を使用して、Microsoft 顧客契約へのお客様の同意を確認します。</span><span class="sxs-lookup"><span data-stu-id="dba82-118">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="dba82-119">この手順を実行するには、管理エージェントまたは販売エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="dba82-119">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="dba82-120">**[顧客]** を選択し、 **[新しい顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="dba82-120">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="dba82-121">**[アカウント情報]** で、会社と主要連絡先の情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="dba82-121">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="dba82-122">**[Microsoft agreement]\(Microsoft 契約\)** で、ボックスをオンにして、顧客が Microsoft 顧客契約に同意していることを証明します。</span><span class="sxs-lookup"><span data-stu-id="dba82-122">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="dba82-123">**[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。</span><span class="sxs-lookup"><span data-stu-id="dba82-123">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="dba82-124">将来の日付に設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="dba82-124">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="dba82-125">表示されたユーザーの主要連絡先情報が正しいことを確認します。</span><span class="sxs-lookup"><span data-stu-id="dba82-125">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="dba82-126">正しくない場合は、 **[更新]** を選択し、契約に同意した人の正確な情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="dba82-126">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="dba82-127">**[次へ]** を選択して、顧客のテナントの作成を続行します。</span><span class="sxs-lookup"><span data-stu-id="dba82-127">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="新しい顧客":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="dba82-129">既存のお客様について、お客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="dba82-129">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="dba82-130">これを行うには、管理エージェントまたは販売エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="dba82-130">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="dba82-131">**[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="dba82-131">Select **Customers**.</span></span> <span data-ttu-id="dba82-132">顧客を検索して選択します。</span><span class="sxs-lookup"><span data-stu-id="dba82-132">Find and select the customer.</span></span>

2. <span data-ttu-id="dba82-133">**[アカウント情報]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="dba82-133">Select **Account info**.</span></span>

3. <span data-ttu-id="dba82-134">**[Microsoft 顧客契約]** で **[更新]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="dba82-134">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="dba82-135">契約に同意したユーザーの **名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。</span><span class="sxs-lookup"><span data-stu-id="dba82-135">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="dba82-136">**[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。</span><span class="sxs-lookup"><span data-stu-id="dba82-136">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="dba82-137">将来の日付に設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="dba82-137">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="dba82-138">**[保存]** を選択して続行します。</span><span class="sxs-lookup"><span data-stu-id="dba82-138">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="既存の顧客":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="dba82-140">お客様の同意の確認を取得する</span><span class="sxs-lookup"><span data-stu-id="dba82-140">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="dba82-141">既存の顧客が Microsoft 顧客契約に同意したことを示す確認を取得するには、次の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="dba82-141">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="dba82-142">これを行うには、管理エージェントまたは販売エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="dba82-142">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="dba82-143">**[顧客]** を選択し、表示するお客様を検索して選択します。</span><span class="sxs-lookup"><span data-stu-id="dba82-143">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="dba82-144">**[アカウント情報]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="dba82-144">Select **Account info**.</span></span>

3. <span data-ttu-id="dba82-145">**Microsoft 顧客契約** で、この顧客による確認の提供の有無を表示します。</span><span class="sxs-lookup"><span data-stu-id="dba82-145">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="dba82-146">パートナー センター API/SDK を使用して顧客の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="dba82-146">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="dba82-147">パートナー センター API/SDK を使用して、Microsoft 顧客契約に対する顧客の同意を確認できます。</span><span class="sxs-lookup"><span data-stu-id="dba82-147">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="dba82-148">API/SDK について詳しくは、以下をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="dba82-148">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="dba82-149">Microsoft 顧客契約の契約メタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="dba82-149">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="dba82-150">Microsoft 顧客契約へのお客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="dba82-150">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="dba82-151">Microsoft 顧客契約に関する顧客の同意の確認を取得する </span><span class="sxs-lookup"><span data-stu-id="dba82-151">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="dba82-152">Microsoft 顧客契約テンプレートのダウンロード リンクを取得する</span><span class="sxs-lookup"><span data-stu-id="dba82-152">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="dba82-153">オプション 2:Microsoft 365 管理センターでの顧客の同意</span><span class="sxs-lookup"><span data-stu-id="dba82-153">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="dba82-154">パートナーは、URL を使用して、Microsoft 365 管理センターで契約を確認し、同意するように新規および既存の顧客に要請できます。</span><span class="sxs-lookup"><span data-stu-id="dba82-154">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="dba82-155">次のいくつかのセクションでその方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="dba82-155">The next few sections show you how to:</span></span>

- <span data-ttu-id="dba82-156">新規の顧客を作成し、契約を確認して同意するよう顧客に要請します。</span><span class="sxs-lookup"><span data-stu-id="dba82-156">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="dba82-157">リセラー関係とリセラー契約を確認して同意するよう新規の顧客に要請します。</span><span class="sxs-lookup"><span data-stu-id="dba82-157">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="dba82-158">契約を確認して同意するよう既存の顧客に要請します。</span><span class="sxs-lookup"><span data-stu-id="dba82-158">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="dba82-159">[パートナー センター API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) を使用して、Microsoft 顧客契約の顧客の直接同意の状況を確認できます。</span><span class="sxs-lookup"><span data-stu-id="dba82-159">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="dba82-160">新規の顧客を作成し、契約を確認して同意するよう顧客に要請する</span><span class="sxs-lookup"><span data-stu-id="dba82-160">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="dba82-161">パートナー センターで新規の顧客を作成し、Microsoft 365 管理センターで Microsoft 顧客契約を確認して同意するように要請するには、次の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="dba82-161">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="dba82-162">パートナー センターの **[顧客]** タブから、 **[顧客の追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="dba82-162">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="dba82-163">**[アカウント情報]** で、顧客の会社名や主要連絡先など、すべての必須フィールドに新しい顧客に関する情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="dba82-163">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="dba82-164">**[顧客契約]** で、 **[Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center]\(顧客は Microsoft 365 管理センターで Microsoft 顧客契約に同意するように求められます\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="dba82-164">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="dba82-165">ページの他の必須フィールドをすべて入力します。</span><span class="sxs-lookup"><span data-stu-id="dba82-165">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="dba82-166">**[次へ: 確認]** を選択し、顧客のテナントを作成する手順を続行します。</span><span class="sxs-lookup"><span data-stu-id="dba82-166">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="dba82-167">新規の顧客は、Microsoft 顧客契約に同意するまで購入を行うことはできません。</span><span class="sxs-lookup"><span data-stu-id="dba82-167">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="新規の顧客を作成する":::

5. <span data-ttu-id="dba82-169">新規顧客のワークフローで **[確認]** 画面が表示されたら、顧客の資格情報を保存します。</span><span class="sxs-lookup"><span data-stu-id="dba82-169">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="dba82-170">これらの資格情報は、後で顧客に提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="dba82-170">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="dba82-171">パートナー センターの外部で、Microsoft 365 管理センターで Microsoft 顧客契約に同意するよう顧客に要請するメールを作成して送信します。</span><span class="sxs-lookup"><span data-stu-id="dba82-171">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="dba82-172">メールには次の点を必ず含めるようにします。</span><span class="sxs-lookup"><span data-stu-id="dba82-172">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="dba82-173">この [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) へのリンク (サインインが必要)</span><span class="sxs-lookup"><span data-stu-id="dba82-173">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="dba82-174">手順 5 で保存した顧客の資格情報</span><span class="sxs-lookup"><span data-stu-id="dba82-174">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="dba82-175">顧客がパートナーから要請メールを受け取り、[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) を選択します。</span><span class="sxs-lookup"><span data-stu-id="dba82-175">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="dba82-176">顧客は、提供された顧客の資格情報を使用して Microsoft 365 管理センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="dba82-176">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="dba82-177">顧客は、Microsoft 顧客契約に同意するためのチェック ボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="dba82-177">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="dba82-178">リセラー関係と Microsoft 顧客契約を確認して同意するよう新規の顧客に要請する</span><span class="sxs-lookup"><span data-stu-id="dba82-178">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="dba82-179">リセラー関係と Microsoft 顧客契約を確認して同意するよう新規の顧客に要請するには、次の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="dba82-179">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="dba82-180">パートナー センターの **[顧客]** タブから、 **[リセラーの関係を要求する]** リンクを選択します。</span><span class="sxs-lookup"><span data-stu-id="dba82-180">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="dba82-181">テキストとパラメーター化された URL を含む自動メール テンプレートが生成されます。この URL により、顧客は Microsoft 365 管理センターに誘導されます。</span><span class="sxs-lookup"><span data-stu-id="dba82-181">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="dba82-182">自動的に生成されるメール テンプレートをカスタマイズして、 **[クリップボードにコピー]** か **[電子メールで開く]** を選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="dba82-182">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="dba82-183">このメール テンプレートを使用して、 **[reseller relationship]\(リセラー関係\)** の要求と **[Microsoft 顧客契約]** に同意するよう顧客に要請します。</span><span class="sxs-lookup"><span data-stu-id="dba82-183">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="dba82-184">(注:パートナーは、この要請メールに、自動的に作成された URL と、先ほど作成された顧客の資格情報も含めてください。)</span><span class="sxs-lookup"><span data-stu-id="dba82-184">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="関係を作成する":::

5. <span data-ttu-id="dba82-186">顧客がメールで要請を受け取り、パラメーター化された URL をクリックします。</span><span class="sxs-lookup"><span data-stu-id="dba82-186">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="dba82-187">顧客は、メールで提供された資格情報を使用して、Microsoft 365 管理センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="dba82-187">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="dba82-188">顧客が、 **[reseller relationship]\(リセラー関係\)** と **[Microsoft 顧客契約]** に同意するボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="dba82-188">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="dba82-189">同じ URL 内で、顧客は、協力関係にあるさまざまなパートナーの一覧を統合して表示できます。</span><span class="sxs-lookup"><span data-stu-id="dba82-189">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="dba82-190">パートナーを選択すると、詳細を表示できます。</span><span class="sxs-lookup"><span data-stu-id="dba82-190">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="契約に同意する":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="dba82-192">契約を確認して同意するよう既存の顧客に要請する</span><span class="sxs-lookup"><span data-stu-id="dba82-192">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="dba82-193">Microsoft 顧客契約を確認して同意するよう既存の顧客に要請するには、次の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="dba82-193">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="dba82-194">Microsoft 顧客契約に同意するよう同意するよう顧客に要請する URL が埋め込まれた顧客宛のメールを作成します。</span><span class="sxs-lookup"><span data-stu-id="dba82-194">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="dba82-195">顧客がメールで招待状を受け取り、[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) をクリックします。</span><span class="sxs-lookup"><span data-stu-id="dba82-195">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="dba82-196">顧客が Microsoft 365 管理センターに資格情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="dba82-196">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="dba82-197">顧客が、Microsoft 顧客契約に同意するボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="dba82-197">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="dba82-198">同じ URL 内で、顧客は、協力関係にあるさまざまなパートナーの一覧を統合して表示できます。</span><span class="sxs-lookup"><span data-stu-id="dba82-198">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="dba82-199">パートナーを選択すると、詳細を表示できます。</span><span class="sxs-lookup"><span data-stu-id="dba82-199">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="顧客":::

>[!NOTE]
><span data-ttu-id="dba82-201">特定のシナリオでは、Microsoft 顧客契約に顧客が直接同意できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="dba82-201">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="dba82-202">そのようなシナリオについて詳しくは、以下の「顧客の代わりに証明する必要がある 2 つのシナリオ」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="dba82-202">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="dba82-203">顧客の代わりに証明する必要がある 2 つのシナリオ</span><span class="sxs-lookup"><span data-stu-id="dba82-203">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="dba82-204">顧客が Microsoft 365 管理センター内で Microsoft 顧客契約に直接同意することができない可能性のあるシナリオが 2 つあります。</span><span class="sxs-lookup"><span data-stu-id="dba82-204">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="dba82-205">**シナリオ 1**: 既存の顧客が、既存のパートナー関係を通じて次のうちのいずれかを購入したことがある: プラン、ソフトウェアまたはソフトウェア サブスクリプション、予約インスタンス、Azure プラン。</span><span class="sxs-lookup"><span data-stu-id="dba82-205">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="dba82-206">顧客が新たな購入を行おうとしている (自動更新を除く)。</span><span class="sxs-lookup"><span data-stu-id="dba82-206">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="dba82-207">その顧客が URL をクリックすると、"Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement"(Microsoft 顧客契約に同意したことを確認するために、パートナーに連絡してください) というメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="dba82-207">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="dba82-208">**解決策**:パートナーが顧客に代わって証明する必要があります。</span><span class="sxs-lookup"><span data-stu-id="dba82-208">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Microsoft 365 管理センターのページのスクリーンショット。Microsoft 顧客契約への同意を確認するためにパートナーに連絡するよう求められています。":::

<span data-ttu-id="dba82-210">**シナリオ 2**:既存の顧客が、次のうちいずれかを購入したことがある: プラン、ソフトウェアまたはソフトウェア サブスクリプション、予約インスタンス、Azure プラン。</span><span class="sxs-lookup"><span data-stu-id="dba82-210">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="dba82-211">顧客が新しいパートナーを通じて新たな購入を行おうとしている。</span><span class="sxs-lookup"><span data-stu-id="dba82-211">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="dba82-212">その顧客が Microsoft 365 管理センターへの URL をクリックして、新しいパートナー関係と契約に同意すると、"Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement"(Microsoft 顧客契約に同意したことを確認するために、パートナーに連絡してください) というメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="dba82-212">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="dba82-213">**解決策**:パートナーが顧客に代わって証明する必要があります。</span><span class="sxs-lookup"><span data-stu-id="dba82-213">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="dba82-214">顧客が契約に同意したことを確認する</span><span class="sxs-lookup"><span data-stu-id="dba82-214">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="dba82-215">まだ確認していない既存のお客様について新しい注文を作成しようとすると、確認を完了するよう求めるプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="dba82-215">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="dba82-216">この場合、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="dba82-216">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="dba82-217">契約に同意したユーザーの **名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。</span><span class="sxs-lookup"><span data-stu-id="dba82-217">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="dba82-218">**[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。</span><span class="sxs-lookup"><span data-stu-id="dba82-218">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="dba82-219">将来の日付に設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="dba82-219">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="dba82-220">**[Save and continue]** (保存して続行) を選択します。</span><span class="sxs-lookup"><span data-stu-id="dba82-220">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="dba82-221">次のステップ</span><span class="sxs-lookup"><span data-stu-id="dba82-221">Next steps</span></span>

- [<span data-ttu-id="dba82-222">会社のプロファイルの情報を確認または更新する</span><span class="sxs-lookup"><span data-stu-id="dba82-222">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="dba82-223">Microsoft 顧客契約 (地域、言語別)</span><span class="sxs-lookup"><span data-stu-id="dba82-223">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
