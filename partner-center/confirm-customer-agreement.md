---
title: Microsoft 顧客契約に対する顧客の同意を確認する
description: Microsoft 顧客契約に対する顧客の同意を確認する方法について説明します。 クラウド ソリューション プロバイダー (CSP) プログラムの参加者が顧客のために Microsoft の製品とサービスを注文するには、これを行う必要があります。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 05/05/2020
ms.openlocfilehash: 45a34473ff63875af8bd07962ea836661bc948ee
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/19/2020
ms.locfileid: "92198058"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a><span data-ttu-id="f249b-104">CSP パートナー プログラムで Microsoft 顧客契約への顧客の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="f249b-104">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>

<span data-ttu-id="f249b-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="f249b-105">**Applies to**</span></span>

- <span data-ttu-id="f249b-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="f249b-106">Partner Center</span></span>
- <span data-ttu-id="f249b-107">Microsoft 365 管理センター</span><span class="sxs-lookup"><span data-stu-id="f249b-107">Microsoft 365 Admin Center</span></span>

<span data-ttu-id="f249b-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="f249b-108">**Appropriate roles**</span></span>

- <span data-ttu-id="f249b-109">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="f249b-109">Admin agent</span></span>
- <span data-ttu-id="f249b-110">販売代理店</span><span class="sxs-lookup"><span data-stu-id="f249b-110">Sales agent</span></span>

<span data-ttu-id="f249b-111">2019 年 10 月 1 日に、Microsoft Cloud 契約に置き換わるものとして、CSP プログラムに **Microsoft 顧客契約**が導入されました。</span><span class="sxs-lookup"><span data-stu-id="f249b-111">On October 1, 2019, Microsoft introduced the **Microsoft Customer Agreement** to the CSP program to replace the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="f249b-112">間接リセラー向けの追加の[ガイダンス](indirect-reseller-tasks-in-partner-center.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f249b-112">Read additional [guidance](indirect-reseller-tasks-in-partner-center.md) for indirect resellers.</span></span> <span data-ttu-id="f249b-113">新しい契約へのパートナーの移行を促進するために、2020 年 1 月 31 までは両方の契約が CSP プログラムで共存していました。</span><span class="sxs-lookup"><span data-stu-id="f249b-113">To facilitate partners' migration to the new agreement, both agreements coexisted in the CSP program until January 31, 2020.</span></span> <span data-ttu-id="f249b-114">2020 年 2 月 1 日に、Microsoft Cloud 契約は Microsoft 顧客契約に置き換わりました。</span><span class="sxs-lookup"><span data-stu-id="f249b-114">Starting February 1, 2020, the Microsoft Customer Agreement replaced the Microsoft Cloud Agreement.</span></span>

<span data-ttu-id="f249b-115">顧客が Microsoft 顧客契約に同意するには、次の 2 つのオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="f249b-115">Customers have two options for accepting the Microsoft Customer Agreement.</span></span> 

<span data-ttu-id="f249b-116">**オプション 1**:顧客の同意に対するパートナー証明 - パートナーは、パートナー センター API/SDK を使用するか、パートナー センター ダッシュボードを使用して、顧客の同意を確認できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-116">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="f249b-117">**オプション 2**:顧客の直接同意 - パートナーは、URL を使用して、Microsoft 365 管理センターで契約を確認し、同意するように顧客に要請できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-117">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="f249b-118">Microsoft 顧客契約テンプレートへのアクセス</span><span class="sxs-lookup"><span data-stu-id="f249b-118">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="f249b-119">最新バージョンの Microsoft 顧客契約テンプレートは、[こちら](https://aka.ms/customeragreement)から手動でダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="f249b-119">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="f249b-120">Microsoft 顧客契約は国によって異なります。</span><span class="sxs-lookup"><span data-stu-id="f249b-120">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="f249b-121">Microsoft 顧客契約テンプレートを要求するときは、顧客の所在地に応じて正しい国を選択してください。</span><span class="sxs-lookup"><span data-stu-id="f249b-121">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="f249b-122">オプション 1:パートナー センターを使用してお客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="f249b-122">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="f249b-123">パートナーは、新規の顧客と既存の顧客について、パートナー センターで Microsoft 顧客契約に対する顧客の同意を確認できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-123">Partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="f249b-124">リセラーは顧客に代わって証明を行うことができません。間接プロバイダーと協力して、証明を完了する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f249b-124">Resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="f249b-125">新しいお客様について、お客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="f249b-125">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="f249b-126">パートナー センターで新しい顧客テナントを作成するときに、次の手順を使用して、Microsoft 顧客契約へのお客様の同意を確認します。</span><span class="sxs-lookup"><span data-stu-id="f249b-126">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="f249b-127">この手順を実行するには、管理エージェントまたは販売エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="f249b-127">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="f249b-128">**[顧客]** を選択し、 **[新しい顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="f249b-128">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="f249b-129">**[アカウント情報]** で、会社と主要連絡先の情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="f249b-129">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="f249b-130">**[Microsoft agreement]\(Microsoft 契約\)** で、ボックスをオンにして、顧客が Microsoft 顧客契約に同意していることを証明します。</span><span class="sxs-lookup"><span data-stu-id="f249b-130">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="f249b-131">**[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。</span><span class="sxs-lookup"><span data-stu-id="f249b-131">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="f249b-132">将来の日付に設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="f249b-132">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="f249b-133">表示されたユーザーの主要連絡先情報が正しいことを確認します。</span><span class="sxs-lookup"><span data-stu-id="f249b-133">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="f249b-134">正しくない場合は、 **[更新]** を選択し、契約に同意した人の正確な情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="f249b-134">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="f249b-135">**[次へ]** を選択して、顧客のテナントの作成を続行します。</span><span class="sxs-lookup"><span data-stu-id="f249b-135">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="新しい顧客":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="f249b-137">既存のお客様について、お客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="f249b-137">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="f249b-138">これを行うには、管理エージェントまたは販売エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="f249b-138">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="f249b-139">**[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="f249b-139">Select **Customers**.</span></span> <span data-ttu-id="f249b-140">顧客を検索して選択します。</span><span class="sxs-lookup"><span data-stu-id="f249b-140">Find and select the customer.</span></span>

2. <span data-ttu-id="f249b-141">**[アカウント情報]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="f249b-141">Select **Account info**.</span></span>

3. <span data-ttu-id="f249b-142">**[Microsoft 顧客契約]** で **[更新]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="f249b-142">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="f249b-143">契約に同意したユーザーの**名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。</span><span class="sxs-lookup"><span data-stu-id="f249b-143">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="f249b-144">**[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。</span><span class="sxs-lookup"><span data-stu-id="f249b-144">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="f249b-145">将来の日付に設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="f249b-145">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="f249b-146">**[保存]** を選択して続行します。</span><span class="sxs-lookup"><span data-stu-id="f249b-146">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="新しい顧客":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="f249b-148">お客様の同意の確認を取得する</span><span class="sxs-lookup"><span data-stu-id="f249b-148">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="f249b-149">次の手順に従って、既存のお客様が Microsoft 顧客契約に同意したことを示す確認を取得できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-149">You can retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement using the following steps.</span></span> <span data-ttu-id="f249b-150">これを行うには、管理エージェントまたは販売エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="f249b-150">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="f249b-151">**[顧客]** を選択し、表示するお客様を検索して選択します。</span><span class="sxs-lookup"><span data-stu-id="f249b-151">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="f249b-152">**[アカウント情報]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="f249b-152">Select **Account info**.</span></span>

3. <span data-ttu-id="f249b-153">**Microsoft 顧客契約** で、この顧客による確認の提供の有無を表示します。</span><span class="sxs-lookup"><span data-stu-id="f249b-153">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="f249b-154">パートナー センター API/SDK を使用して顧客の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="f249b-154">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="f249b-155">パートナー センター API/SDK を使用して、Microsoft 顧客契約に対する顧客の同意を確認できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-155">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="f249b-156">API/SDK について詳しくは、以下をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f249b-156">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="f249b-157">Microsoft 顧客契約の契約メタデータを取得する</span><span class="sxs-lookup"><span data-stu-id="f249b-157">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="f249b-158">Microsoft 顧客契約へのお客様の同意を確認する</span><span class="sxs-lookup"><span data-stu-id="f249b-158">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="f249b-159">Microsoft 顧客契約に関する顧客の同意の確認を取得する </span><span class="sxs-lookup"><span data-stu-id="f249b-159">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="f249b-160">Microsoft 顧客契約テンプレートのダウンロード リンクを取得する</span><span class="sxs-lookup"><span data-stu-id="f249b-160">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="f249b-161">オプション 2:Microsoft 365 管理センターでの顧客の同意</span><span class="sxs-lookup"><span data-stu-id="f249b-161">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="f249b-162">パートナーは、URL を使用して、Microsoft 365 管理センターで契約を確認し、同意するように新規および既存の顧客に要請できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-162">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="f249b-163">次のいくつかのセクションでその方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="f249b-163">The next few sections show you how to:</span></span>

- <span data-ttu-id="f249b-164">新規の顧客を作成し、契約を確認して同意するよう顧客に要請します。</span><span class="sxs-lookup"><span data-stu-id="f249b-164">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="f249b-165">リセラー関係とリセラー契約を確認して同意するよう新規の顧客に要請します。</span><span class="sxs-lookup"><span data-stu-id="f249b-165">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="f249b-166">契約を確認して同意するよう既存の顧客に要請します。</span><span class="sxs-lookup"><span data-stu-id="f249b-166">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="f249b-167">[パートナー センター API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) を使用して、Microsoft 顧客契約の顧客の直接同意の状況を確認できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-167">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="f249b-168">新規の顧客を作成し、契約を確認して同意するよう顧客に要請する</span><span class="sxs-lookup"><span data-stu-id="f249b-168">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="f249b-169">パートナー センターで新規の顧客を作成し、Microsoft 365 管理センターで Microsoft 顧客契約を確認して同意するように要請するには、次の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="f249b-169">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="f249b-170">パートナー センターの **[顧客]** タブから、 **[顧客の追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="f249b-170">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="f249b-171">**[アカウント情報]** で、顧客の会社名や主要連絡先など、すべての必須フィールドに新しい顧客に関する情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="f249b-171">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="f249b-172">**[顧客契約]** で、最初のオプション **[Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center]\(顧客は Microsoft 365 管理センターで Microsoft 顧客契約に同意するように求められます\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="f249b-172">Under **Customer Agreement**, select the first option, **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="f249b-173">ページの他の必須フィールドをすべて入力します。</span><span class="sxs-lookup"><span data-stu-id="f249b-173">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="f249b-174">**[次へ: 確認]** を選択し、顧客のテナントを作成する手順を続行します。</span><span class="sxs-lookup"><span data-stu-id="f249b-174">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="f249b-175">新規の顧客は、Microsoft 顧客契約に同意するまで新しい購入を行うことはできません。</span><span class="sxs-lookup"><span data-stu-id="f249b-175">New customers cannot make a new purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="新しい顧客":::

5. <span data-ttu-id="f249b-177">新規顧客のワークフローで **[確認]** 画面が表示されたら、顧客の資格情報を保存します。</span><span class="sxs-lookup"><span data-stu-id="f249b-177">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="f249b-178">これらの資格情報は、後で顧客に提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f249b-178">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="f249b-179">パートナー センターの外部で、Microsoft 365 管理センターで Microsoft 顧客契約に同意するよう顧客に要請するメールを作成して送信します。</span><span class="sxs-lookup"><span data-stu-id="f249b-179">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="f249b-180">メールには次の点を必ず含めるようにします。</span><span class="sxs-lookup"><span data-stu-id="f249b-180">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="f249b-181">この [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) へのリンク (サインインが必要)</span><span class="sxs-lookup"><span data-stu-id="f249b-181">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="f249b-182">手順 5 で保存した顧客の資格情報</span><span class="sxs-lookup"><span data-stu-id="f249b-182">The customer's credentials you saved in Step 5.</span></span>

7. <span data-ttu-id="f249b-183">顧客がパートナーから要請メールを受け取り、[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) を選択します。</span><span class="sxs-lookup"><span data-stu-id="f249b-183">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="f249b-184">顧客が、パートナーから受信した顧客の資格情報を使用して Microsoft 365 管理センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="f249b-184">The customer signs into Microsoft 365 Admin Center using the customer credentials previously received from the partner.</span></span>

9. <span data-ttu-id="f249b-185">顧客が、Microsoft 顧客契約に同意するボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="f249b-185">The customer then checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="f249b-186">リセラー関係と Microsoft 顧客契約を確認して同意するよう新規の顧客に要請する</span><span class="sxs-lookup"><span data-stu-id="f249b-186">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="f249b-187">リセラー関係と Microsoft 顧客契約を確認して同意するよう新規の顧客に要請するには、次の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="f249b-187">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="f249b-188">パートナー センターの **[顧客]** タブから、 **[リセラーの関係を要求する]** リンクを選択します。</span><span class="sxs-lookup"><span data-stu-id="f249b-188">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="f249b-189">テキストとパラメーター化された URL を含む自動メール テンプレートが生成されます。この URL により、顧客は Microsoft 365 管理センターに誘導されます。</span><span class="sxs-lookup"><span data-stu-id="f249b-189">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="f249b-190">自動的に生成されるメール テンプレートをカスタマイズして、 **[クリップボードにコピー]** か **[電子メールで開く]** を選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="f249b-190">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="f249b-191">このメール テンプレートを使用して、 **[reseller relationship]\(リセラー関係\)** の要求と **[Microsoft 顧客契約]** に同意するよう顧客に要請します。</span><span class="sxs-lookup"><span data-stu-id="f249b-191">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="f249b-192">(注:パートナーは、この要請メールに、自動的に作成された URL と、先ほど作成された顧客の資格情報も含めてください。)</span><span class="sxs-lookup"><span data-stu-id="f249b-192">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="新しい顧客":::

5. <span data-ttu-id="f249b-194">顧客がメールで要請を受け取り、パラメーター化された URL をクリックします。</span><span class="sxs-lookup"><span data-stu-id="f249b-194">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="f249b-195">顧客が、メールでパートナーによって提供された資格情報を使用して、Microsoft 365 管理センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="f249b-195">Customer uses credentials provided by partner within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="f249b-196">顧客が、 **[reseller relationship]\(リセラー関係\)** と **[Microsoft 顧客契約]** に同意するボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="f249b-196">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="f249b-197">同じ URL 内で、顧客は、協力関係にあるさまざまなパートナーの一覧を統合して表示できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-197">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="f249b-198">パートナーを選択すると、詳細を表示できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-198">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="新しい顧客":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="f249b-200">契約を確認して同意するよう既存の顧客に要請する</span><span class="sxs-lookup"><span data-stu-id="f249b-200">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="f249b-201">Microsoft 顧客契約を確認して同意するよう既存の顧客に要請するには、次の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="f249b-201">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="f249b-202">Microsoft 顧客契約に同意するよう同意するよう顧客に要請する URL が埋め込まれた顧客宛のメールを作成します。</span><span class="sxs-lookup"><span data-stu-id="f249b-202">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="f249b-203">顧客がメールで招待状を受け取り、[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) をクリックします。</span><span class="sxs-lookup"><span data-stu-id="f249b-203">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="f249b-204">顧客が Microsoft 365 管理センターに資格情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="f249b-204">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="f249b-205">顧客が、Microsoft 顧客契約に同意するボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="f249b-205">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="f249b-206">同じ URL 内で、顧客は、協力関係にあるさまざまなパートナーの一覧を統合して表示できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-206">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="f249b-207">パートナーを選択すると、詳細を表示できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-207">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="新しい顧客":::

>[!NOTE]
><span data-ttu-id="f249b-209">特定のシナリオでは、Microsoft 顧客契約に顧客が直接同意できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="f249b-209">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="f249b-210">そのようなシナリオについて詳しくは、「[顧客の代わりに証明する必要がある 2 つのシナリオ](attest-acceptance-customer-agreement.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f249b-210">To learn more about these situations, see [Two scenarios where you need to attest on behalf of your customer](attest-acceptance-customer-agreement.md).</span></span>

### <a name="historical-timeline-details"></a><span data-ttu-id="f249b-211">履歴タイムラインの詳細</span><span class="sxs-lookup"><span data-stu-id="f249b-211">Historical timeline details</span></span>

| <span data-ttu-id="f249b-212">日付</span><span class="sxs-lookup"><span data-stu-id="f249b-212">Date</span></span> | <span data-ttu-id="f249b-213">マイルストーン</span><span class="sxs-lookup"><span data-stu-id="f249b-213">Milestone</span></span> | <span data-ttu-id="f249b-214">詳細情報</span><span class="sxs-lookup"><span data-stu-id="f249b-214">Details</span></span> |
|------------|------------|--------------------------------|
|<span data-ttu-id="f249b-215">2019 年 8 月 1 日</span><span class="sxs-lookup"><span data-stu-id="f249b-215">August 01, 2019</span></span>| <span data-ttu-id="f249b-216">サンドボックスで UX プレビューの提供開始</span><span class="sxs-lookup"><span data-stu-id="f249b-216">UX preview available in sandbox</span></span>| <span data-ttu-id="f249b-217">パートナーは、CSP サンドボックス環境でパートナー センター ダッシュボードを使用して、Microsoft 顧客契約へのお客様の同意を確認できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-217">Partners can confirm customer acceptance of the Microsoft Customer Agreement using the Partner Center dashboard in the CSP sandbox environment.</span></span> <span data-ttu-id="f249b-218">CSP サンドボックス環境へのアクセス権を持つパートナーは、ユーザー エクスペリエンスの変更をプレビューできます。</span><span class="sxs-lookup"><span data-stu-id="f249b-218">Partners with access to the CSP sandbox environment preview the user experience changes.</span></span> <span data-ttu-id="f249b-219">サンドボックス環境へのアクセス権を持たないパートナーは、その変更をこのトピックで確認できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-219">Partners without sandbox access can learn about the changes in this topic.</span></span>|
|<span data-ttu-id="f249b-220">2019 年 9 月 3 日</span><span class="sxs-lookup"><span data-stu-id="f249b-220">September 03, 2019</span></span>|<span data-ttu-id="f249b-221">サンドボックスで API プレビューの提供開始。</span><span class="sxs-lookup"><span data-stu-id="f249b-221">API preview is available in sandbox.</span></span>|<span data-ttu-id="f249b-222">パートナーは、CSP サンドボックス環境でパートナー センター API を使用して、Microsoft 顧客契約へのお客様の同意を確認できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-222">Partner can confirm customer acceptance of the Microsoft Customer Agreement using Partner Center API in CSP sandbox environment.</span></span> <span data-ttu-id="f249b-223">API パートナーは、この機会を利用して API の変更をプレビューし、新しい契約をサポートするために API の統合作業を開始できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-223">API partners can use this opportunity to preview the API changes and start working on API integration to support the new agreement.</span></span>|
|<span data-ttu-id="f249b-224">2019 年 9 月 20 日</span><span class="sxs-lookup"><span data-stu-id="f249b-224">September 20, 2019</span></span>|<span data-ttu-id="f249b-225">サンドボックスで .NET SDK プレビューの提供開始。</span><span class="sxs-lookup"><span data-stu-id="f249b-225">.NET SDK preview is available in sandbox.</span></span>|<span data-ttu-id="f249b-226">パートナーは、CSP サンドボックス環境内でパートナー センター .NET SDK を使用して、Microsoft 顧客契約へのお客様の同意を確認できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-226">Partner can confirm customer acceptance of the Microsoft Customer Agreement using Partner Center .NET SDK in CSP sandbox environment.</span></span> <span data-ttu-id="f249b-227">API パートナーは、この機会を利用して .NET SDK の変更のプレビューを表示し、新しい契約をサポートするために API の統合作業を開始できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-227">API partners can use this opportunity to preview the .NET SDK changes and start working on API integration to support the new agreement.</span></span>|
|<span data-ttu-id="f249b-228">2019 年 10 月 1 日</span><span class="sxs-lookup"><span data-stu-id="f249b-228">October 01, 2019</span></span>|<span data-ttu-id="f249b-229">Microsoft 顧客契約が運用環境で使用可能</span><span class="sxs-lookup"><span data-stu-id="f249b-229">Microsoft Customer Agreement available in production</span></span>|<span data-ttu-id="f249b-230">Microsoft では、Microsoft 顧客契約を CSP プログラムに導入します。これは、Microsoft Cloud 契約に置き換わるものです。</span><span class="sxs-lookup"><span data-stu-id="f249b-230">Microsoft introduces the Microsoft Customer Agreement to the CSP program to replace the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="f249b-231">パートナーは、運用環境でパートナー センター ダッシュボードと API を使用して、Microsoft 顧客契約へのお客様の同意を確認できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-231">Partners can confirm customer acceptance of the Microsoft Customer Agreement using the Partner Center dashboard and API in production.</span></span> <span data-ttu-id="f249b-232">Microsoft Cloud 契約は、CSP パートナー プログラムで引き続きサポートされます。</span><span class="sxs-lookup"><span data-stu-id="f249b-232">The Microsoft Cloud Agreement remains supported within the CSP partner program.</span></span> <span data-ttu-id="f249b-233">ただし、パートナーは、Microsoft 顧客契約への移行を開始することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="f249b-233">However, partners are advised to start migrating to the Microsoft Customer Agreement.</span></span> <span data-ttu-id="f249b-234">新しい購入および既存のサブスクリプションに対するライセンス数の変更を行う場合、パートナーによる Microsoft 顧客契約または Microsoft Cloud 契約の確認が必要になります。</span><span class="sxs-lookup"><span data-stu-id="f249b-234">New purchases and license count changes to existing subscriptions will require partner confirmation of either the Microsoft Customer Agreement or the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="f249b-235">特定の新しいオファー (新しい Azure プランなど) では、Microsoft 顧客契約への同意の確認が求められます。</span><span class="sxs-lookup"><span data-stu-id="f249b-235">Certain new offers (for example, the new Azure plan) will require confirmation of the Microsoft Customer Agreement.</span></span>|
|<span data-ttu-id="f249b-236">2020 年 1 月 31 日</span><span class="sxs-lookup"><span data-stu-id="f249b-236">January 31, 2020</span></span>|<span data-ttu-id="f249b-237">Microsoft クラウド契約が運用環境から削除</span><span class="sxs-lookup"><span data-stu-id="f249b-237">Microsoft Cloud Agreement removed from production</span></span>|<span data-ttu-id="f249b-238">Microsoft Cloud 契約は CSP パートナー プログラムでは受け入れられなくなりました。</span><span class="sxs-lookup"><span data-stu-id="f249b-238">The Microsoft Cloud Agreement is no longer accepted within the CSP partner program.</span></span> <span data-ttu-id="f249b-239">新しい購入および既存のサブスクリプションに対するライセンス数の変更を行う場合、パートナーは、Microsoft 顧客契約の確認を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f249b-239">New purchases and license count changes to existing subscriptions will require the partner to provide confirmation of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="f249b-240">この要件は、以前に Microsoft Cloud 契約に同意した場合でも、新しいお客様および既存のお客様に適用されます。</span><span class="sxs-lookup"><span data-stu-id="f249b-240">This requirement applies to new customers and existing customers who may have previously accepted the Microsoft Cloud Agreement.</span></span>|
|<span data-ttu-id="f249b-241">2020 年 2 月 3 日</span><span class="sxs-lookup"><span data-stu-id="f249b-241">February 3, 2020</span></span>|<span data-ttu-id="f249b-242">パートナーは、URL を使用して、認証された Microsoft 365 管理センターで契約を確認し、同意するように顧客に要請するオプションを利用できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="f249b-242">Partner now has the option to invite the customer via a URL to review and accept the agreement in authenticated Microsoft 365 Admin Center.</span></span> | <span data-ttu-id="f249b-243">顧客は、Microsoft 365 管理センターで Microsoft 顧客契約に同意できます。</span><span class="sxs-lookup"><span data-stu-id="f249b-243">Customer can accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="f249b-244">顧客が Microsoft 365 管理センターで契約に直接同意することにより、条件を承認したことが確認されます。</span><span class="sxs-lookup"><span data-stu-id="f249b-244">Customer's direct acceptance of the agreement in Microsoft 365 Admin Center confirms approval of terms.</span></span> 