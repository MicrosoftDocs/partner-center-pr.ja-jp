---
title: 支払いと収益の問題のトラブルシューティング
ms.topic: article
ms.date: 02/05/2021
description: 収益の不足や不適切な利益、適格性の問題、インセンティブ収益の調整方法などの問題を解決する方法について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: c6ff8915384f8c7ab98fa058f2e45e3d0b4f7214
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/02/2021
ms.locfileid: "106179515"
---
# <a name="troubleshooting-missing-payments-incorrect-earnings-and-other-issues"></a><span data-ttu-id="1ac8b-103">不足している支払い、不適切な収益、およびその他の問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="1ac8b-103">Troubleshooting missing payments, incorrect earnings, and other issues</span></span>

<span data-ttu-id="1ac8b-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="1ac8b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1ac8b-105">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="1ac8b-105">Incentives admin</span></span>

<span data-ttu-id="1ac8b-106">この記事は、インセンティブプログラムの利益や支払いの問題を解決するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-106">This article will help you resolve any earnings or payment issues in your incentives program.</span></span> <span data-ttu-id="1ac8b-107">対象となるのは、支払いのタイミング、収益の適格性の確認、および支払いと税金のプロファイルを適切に設定することの重要性です。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-107">Subjects covered include timing of payments, checking your earnings eligibility, and the importance of setting up your payout and tax profiles properly.</span></span>

## <a name="who-can-create-or-update-payout-and-tax-profiles-for-my-organization"></a><span data-ttu-id="1ac8b-108">組織の支払いと税金のプロファイルを作成または更新できるのはだれですか?</span><span class="sxs-lookup"><span data-stu-id="1ac8b-108">Who can create or update payout and tax profiles for my organization?</span></span>

<span data-ttu-id="1ac8b-109">パートナーセンターで、関連するインセンティブプログラムと MPN の場所のインセンティブ管理者ロールを持つユーザーは、組織の支払いと税金のプロファイルを更新して表示できます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-109">Users who have the incentive admin role in Partner Center for the relevant incentive program and MPN location can update and see the payout and tax profiles for the organization.</span></span>

## <a name="how-long-does-it-take-for-microsoft-to-approve-my-pending-payout-andor-tax-profiles"></a><span data-ttu-id="1ac8b-110">保留中の支払い/税務プロファイルの承認には、どのくらい時間がかかりますか?</span><span class="sxs-lookup"><span data-stu-id="1ac8b-110">How long does it take for Microsoft to approve my pending payout and/or tax profiles?</span></span>

<span data-ttu-id="1ac8b-111">検証には最大 48 時間かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-111">Validation can take up to 48 hours.</span></span> <span data-ttu-id="1ac8b-112">その間、[概要] ページのプロファイルの状態は "登録の検証中" になります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-112">During this time, your profile status on the Overview page will show as Validating enrollment.</span></span> <span data-ttu-id="1ac8b-113">プロセスが完了すると、状態は [成功した場合は **登録** 済み]、または必要に応じて [ **アクションが必要]** と表示されます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-113">Once the process is complete, the status will show as either **Enrolled** if successful, or **Action Required – Update Payment and/or tax details** if necessary.</span></span>

## <a name="how-do-i-know-if-i-have-completed-my-payout-and-tax-profile-correctly"></a><span data-ttu-id="1ac8b-114">支払いおよび税務プロファイルが正しく完了しているかどうかを確認するには、どうすればよいですか?</span><span class="sxs-lookup"><span data-stu-id="1ac8b-114">How do I know if I have completed my payout and tax profile correctly?</span></span>

<span data-ttu-id="1ac8b-115">登録の状態は [概要] ページに表示されます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-115">The status of your enrollment is displayed on the Overview page.</span></span> <span data-ttu-id="1ac8b-116">プロファイルの作成が完了すると、状態が [ **登録の検証** 中] になります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-116">When you’ve finished creating your profiles, your status will be **Validating enrollment**.</span></span> <span data-ttu-id="1ac8b-117">情報が検証されると、状態が [ **登録** 済み] に変わります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-117">Once we’ve validated your information, your status changes to **Enrolled**.</span></span> <span data-ttu-id="1ac8b-118">この状態は、支払いと税金のプロファイルおよび登録が正常に完了したことを示します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-118">This status indicates that your payout and tax profile and your enrollment have been successfully completed.</span></span>

## <a name="why-do-i-need-to-update-my-tax-profile-to-use-it-with-a-new-incentive-program"></a><span data-ttu-id="1ac8b-119">税務プロファイルを更新しないと、そのプロファイルを新しいインセンティブ プログラムで使用できないのはなぜですか?</span><span class="sxs-lookup"><span data-stu-id="1ac8b-119">Why do I need to update my tax profile to use it with a new incentive program?</span></span>

<span data-ttu-id="1ac8b-120">インセンティブの支払いは、インセンティブの種類に応じて、さまざまな場所から行われます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-120">We pay out incentives from different locations depending on the incentive type.</span></span> <span data-ttu-id="1ac8b-121">適切な処理を実行するには、場所によってはインセンティブ プログラム ルールに基づいて、追加の税務情報が必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-121">These differing locations may require additional tax information, based on the incentive program rules, to process correctly.</span></span>

## <a name="how-can-i-delete-a-payment-andor-tax-profile"></a><span data-ttu-id="1ac8b-122">支払い/税務プロファイルを削除するには、どうすればよいですか?</span><span class="sxs-lookup"><span data-stu-id="1ac8b-122">How can I delete a payment and/or tax profile?</span></span>

<span data-ttu-id="1ac8b-123">現在、既存の支払いおよび税務プロファイルを削除するオプションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-123">Microsoft currently does not support the option of deleting existing payout and tax profiles.</span></span>

## <a name="my-payment-is-missing-or-incorrect"></a><span data-ttu-id="1ac8b-124">支払いが不足しているか、正しくありません</span><span class="sxs-lookup"><span data-stu-id="1ac8b-124">My payment is missing or incorrect</span></span>

<span data-ttu-id="1ac8b-125">支払いが見つからないか正しくない場合、次のいずれかが原因であることがよくあります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-125">Missing or incorrect payments are often due to one of the following:</span></span>

- <span data-ttu-id="1ac8b-126">**資格がない可能性があります。**</span><span class="sxs-lookup"><span data-stu-id="1ac8b-126">**You may not be eligible.**</span></span>  <span data-ttu-id="1ac8b-127">収益を受け取ることができるのは、運用の適格性の要件を満たしている場合、つまり、各プログラムの収益期間にご自身が登録されている場合だけです。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-127">Earnings will be available only if you meet Operational Eligibility Requirements, that is, enrolled to the respective program earning period.</span></span>
- <span data-ttu-id="1ac8b-128">**要件を満たしていない可能性があります。**</span><span class="sxs-lookup"><span data-stu-id="1ac8b-128">**You may not have met the requirements.**</span></span>  <span data-ttu-id="1ac8b-129">探しているインセンティブの適格性および対象となる収益のルールを満たしているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-129">Check to see whether you have met the eligibility and eligible revenue rules for the incentive you’re looking for.</span></span>

  <span data-ttu-id="1ac8b-130">**資格を確認するには**</span><span class="sxs-lookup"><span data-stu-id="1ac8b-130">**To check your eligibility**</span></span>

  1. <span data-ttu-id="1ac8b-131">[パートナーインセンティブ](https://partner.microsoft.com/membership/partner-incentives)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-131">Sign into [Partner incentives](https://partner.microsoft.com/membership/partner-incentives).</span></span>

  2. <span data-ttu-id="1ac8b-132">プログラムのドキュメントまで下にスクロールします。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-132">Scroll down to the documents for your program.</span></span>
  
  3. <span data-ttu-id="1ac8b-133">目的のドキュメントリンクを選択し、次のセクションを確認します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-133">Select the document link you want, and then review the sections</span></span> 

<span data-ttu-id="1ac8b-134">**パートナーの資格** と **適格な収益ルール**。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-134">**Partner eligibility** and **Eligible revenue rules**.</span></span>

- <span data-ttu-id="1ac8b-135">**支払いプロファイルが不完全である可能性があります。**</span><span class="sxs-lookup"><span data-stu-id="1ac8b-135">**Your payment profile may be incomplete.**</span></span> <span data-ttu-id="1ac8b-136">インセンティブの収益の開始日は、すべての適格性の要件 (支払いと税金でのオンボードの詳細を含む) を完了した月の最初の日になります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-136">Your incentive earnings start date will be the first day of the month in which you’ve completed all of the eligibility requirements, including onboarding with payout and tax details.</span></span> <span data-ttu-id="1ac8b-137">支払いおよび税務プロファイルが完了する前の数か月は収益を利用できません。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-137">Earnings will not be available for the months prior to payout and tax completion.</span></span> <span data-ttu-id="1ac8b-138">たとえば、2020 年 4 月にすべての要件を満たした場合、収益の開始日は 2020 年 4 月 1 日になります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-138">For example, if you complete all of the requirements during the month of April 2020, your earnings start date will be April 1, 2020.</span></span>
- <span data-ttu-id="1ac8b-139">**未処理のアクションがある可能性があり** ます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-139">**You may have an outstanding action**.</span></span>  <span data-ttu-id="1ac8b-140">未処理のアクションが保留中になっているため、インセンティブが処理されていない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-140">It could be that your incentives are not being processed because there’s an outstanding action pending from you.</span></span>

  <span data-ttu-id="1ac8b-141">**未処理のアクションを表示するには**</span><span class="sxs-lookup"><span data-stu-id="1ac8b-141">**To view your outstanding actions**</span></span>

  1. <span data-ttu-id="1ac8b-142">[パートナーインセンティブ](https://partner.microsoft.com/membership/partner-incentives)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-142">Sign into [Partner incentives](https://partner.microsoft.com/membership/partner-incentives).</span></span>
  2. <span data-ttu-id="1ac8b-143">[ **トランザクションの履歴** ] ページを開きます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-143">Open the **Transaction history** page.</span></span> <span data-ttu-id="1ac8b-144">このページのフィールドを確認して、 **保留中の税プロファイル**、 **保留中の支払いプロファイル**、または **保留中の税金請求書の送信** など、未処理のアクションを実行します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-144">Review the fields in this page for any outstanding actions to be completed, such as **Pending Tax profile**, **Pending payment profile**, or **Pending tax invoice submission**.</span></span>

<span data-ttu-id="1ac8b-145">これらのアクションが役に立ちませんが、支払いがまだ見つからないか間違っている場合は、 [サポート](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-145">If these actions don’t help and your payments are still missing or incorrect, contact [support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).</span></span>

## <a name="how-can-i-reconcile-my-adjustments"></a><span data-ttu-id="1ac8b-146">調整を調整するにはどうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-146">How can I reconcile my adjustments?</span></span>

<span data-ttu-id="1ac8b-147">調整を見つけて調整するには、詳細情報とトランザクションの詳細をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-147">You can locate and reconcile your adjustments by downloading your earning and transaction details.</span></span>

1. <span data-ttu-id="1ac8b-148">[パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-148">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="1ac8b-149">上部のナビゲーションバーで、money アイコンを選択し、[ **トランザクション履歴**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-149">On the top navigation bar, select the money icon, and then select **Transaction history**.</span></span>
3. <span data-ttu-id="1ac8b-150">適切なフィルターを適用します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-150">Apply the appropriate filters.</span></span> <span data-ttu-id="1ac8b-151">(以下の **重要な** 注意事項を参照してください)。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-151">(See the **Important** note below.)</span></span>
4. <span data-ttu-id="1ac8b-152">データをフィルター処理したら、[ **ダウンロードの開始**] を選択し、[ **データのエクスポート**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-152">Once you’ve filtered your data, select **Start download**, and then select **Export data**.</span></span> <span data-ttu-id="1ac8b-153">データが CSV ファイルで開かれます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-153">Your data will open in a CSV file.</span></span>
5. <span data-ttu-id="1ac8b-154">CSV ファイルで、[列 P]、[操作の **種類**] の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-154">In the CSV file, navigate to Column P, **Earning type**.</span></span>
6. <span data-ttu-id="1ac8b-155">この列に対して **調整-リベート** をフィルター処理します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-155">Filter this column for **Adjustment-Rebate**.</span></span> <span data-ttu-id="1ac8b-156">各調整の月は列 S で確認できます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-156">You can see the month of each adjustment in Column S.</span></span>

>[!IMPORTANT]
><span data-ttu-id="1ac8b-157">以前の収益期間に適用された調整は、調整が適用された月の利益には表示されません。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-157">Adjustments applied to prior earnings periods will not be visible in the earnings for the month in which the adjustment was applied.</span></span> <span data-ttu-id="1ac8b-158">調整は、調整が適用された月の収益レポートに常に反映されます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-158">Adjustments will always reflect in the earnings report for the month that the adjustment was applied to.</span></span>
>
><span data-ttu-id="1ac8b-159">たとえば、2019年9月に処理された2019年1月の収益の調整は、9月の2019の利益額に反映されません。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-159">For example, an adjustment for January 2019 earnings that was processed in September 2019 will not reflect in the earnings amount for September 2019.</span></span> <span data-ttu-id="1ac8b-160">ただし、2019年9月の支払いを受け取ると、9月に適用された1月2019の調整が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-160">However, when the payment for September 2019 is received, it will include the adjustment for January 2019 that was applied in September.</span></span> <span data-ttu-id="1ac8b-161">このシナリオでは、2019年1月のトランザクション詳細をダウンロードして、適用された調整を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-161">In this scenario, you would need to download the transaction details for January 2019 to see the adjustment that was applied.</span></span>
>
><span data-ttu-id="1ac8b-162">日付フィルターを設定するときは、この点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-162">Keep this in mind when you set your date filters.</span></span> <span data-ttu-id="1ac8b-163">前述のように、以前の期間の調整は、調整が適用された月にのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-163">As mentioned above, adjustments for previous periods will only be visible in the month the adjustment was applied to.</span></span> <span data-ttu-id="1ac8b-164">選択した日付範囲が、検索しようとしている調整の月と一致することを再確認します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-164">Double check that the date range selected corresponds with the month of the adjustment you’re attempting to locate.</span></span> <span data-ttu-id="1ac8b-165">フィルターを削除して新しいフィルターを適用するには、[ **すべてクリア** ] を選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-165">You may need to select **Clear all** to remove your filters, and then apply new ones.</span></span>

## <a name="why-are-my-co-op-claim-payments-made-in-two-different-currencies"></a><span data-ttu-id="1ac8b-166">協力申請の支払いが 2 つの異なる通貨で行われるのはなぜですか?</span><span class="sxs-lookup"><span data-stu-id="1ac8b-166">Why are my co-op claim payments made in two different currencies?</span></span>

<span data-ttu-id="1ac8b-167">さまざまな Microsoft エンティティから協力ファンドが取得されるとき、エンティティごとに現地通貨で支払いが行われます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-167">When co-op funds are earned from different Microsoft entities, payments are made in the local currency of each respective entity.</span></span>  

## <a name="why-was-i-paid-in-a-currency-other-than-my-co-op-claim-currency"></a><span data-ttu-id="1ac8b-168">協力申請の通貨以外で支払いが行われたのはなぜですか?</span><span class="sxs-lookup"><span data-stu-id="1ac8b-168">Why was I paid in a currency other than my co-op claim currency?</span></span>

<span data-ttu-id="1ac8b-169">すべてのインセンティブ プログラムに、セットアップ中に作成された銀行プロファイルがあります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-169">Every incentive program has a bank profile that was created during setup.</span></span> <span data-ttu-id="1ac8b-170">そのプロファイルで指定された通貨は、支払いが行われる通貨です。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-170">The currency specified in that profile is the currency in which you’ll be paid.</span></span>

## <a name="i-dont-see-earnings-for-a-certain-period"></a><span data-ttu-id="1ac8b-171">特定の期間の収益が表示されない</span><span class="sxs-lookup"><span data-stu-id="1ac8b-171">I don’t see earnings for a certain period</span></span>

<span data-ttu-id="1ac8b-172">予想される期間の収益が表示されない場合は、通常、次のいずれかの問題が原因です。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-172">When you don’t see earnings for a period in which they’re expected, it’s usually due to one of the following issues:</span></span>

- <span data-ttu-id="1ac8b-173">**資格がない可能性があります。**</span><span class="sxs-lookup"><span data-stu-id="1ac8b-173">**You may not be eligible.**</span></span>  <span data-ttu-id="1ac8b-174">収益を受け取ることができるのは、運用の適格性の要件を満たしている場合、つまり、各プログラムの収益期間にご自身が登録されている場合だけです。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-174">Earnings will be available only if you meet Operational Eligibility Requirements, that is, enrolled to the respective program earning period.</span></span>

- <span data-ttu-id="1ac8b-175">**支払いプロファイルが不完全である可能性があります。**</span><span class="sxs-lookup"><span data-stu-id="1ac8b-175">**Your payment profile may be incomplete.**</span></span>  <span data-ttu-id="1ac8b-176">インセンティブの収益の開始日は、すべての適格性の要件 (支払いと税金でのオンボードの詳細を含む) を完了した月の最初の日になります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-176">Your incentive earnings start date will be the first day of the month in which you’ve completed all of the eligibility requirements, including onboarding with payout and tax details.</span></span> <span data-ttu-id="1ac8b-177">支払いおよび税務プロファイルが完了する前の数か月は収益を利用できません。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-177">Earnings will not be available for the months prior to payout and tax completion.</span></span> <span data-ttu-id="1ac8b-178">たとえば、2020 年 4 月にすべての要件を満たした場合、収益の開始日は 2020 年 4 月 1 日になります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-178">For example, if you complete all of the requirements during the month of April 2020, your earnings start date will be April 1, 2020.</span></span>

<span data-ttu-id="1ac8b-179">支払いと税金の詳細を使用したオンボードなどの有資格要件を満たしていても、収益がまだない場合は、 [サポート](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-179">If you have completed eligibility requirements including onboarding with payout and tax details on time, and earnings are still missing, contact [support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).</span></span>

## <a name="my-earnings-are-missing-or-incorrect"></a><span data-ttu-id="1ac8b-180">収益が不足しているか、正しくありません</span><span class="sxs-lookup"><span data-stu-id="1ac8b-180">My earnings are missing or incorrect</span></span>

<span data-ttu-id="1ac8b-181">収益の欠落または誤りは、次のいずれかの問題が原因である可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-181">Missing or incorrect earnings may be caused by one of the following issues:</span></span>

- <span data-ttu-id="1ac8b-182">**要件を満たしていない可能性があります。**</span><span class="sxs-lookup"><span data-stu-id="1ac8b-182">**You may not have met the requirements.**</span></span>  <span data-ttu-id="1ac8b-183">探しているインセンティブの[適格性](#my-payment-is-missing-or-incorrect)および対象となる収益のルールを満たしているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-183">Check to see whether you have met the [eligibility](#my-payment-is-missing-or-incorrect) and eligible revenue rules for the incentive you’re looking for.</span></span>

- <span data-ttu-id="1ac8b-184">**不一致が存在する可能性があります。**</span><span class="sxs-lookup"><span data-stu-id="1ac8b-184">**There may be a discrepancy.**</span></span>  <span data-ttu-id="1ac8b-185">[プログラムの適格性](incentives-determined-your-program-eligibility.md)と[利益](incentives-confirm-your-earnings-eligibility.md)の両方の要件を満たしていても、収益が誤って表示される場合は、次の情報を参考にしてデータを取得してください。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-185">If you meet both [program eligibility](incentives-determined-your-program-eligibility.md) and [earnings eligibility](incentives-confirm-your-earnings-eligibility.md) requirements and your earnings still appear to be incorrect, the following information may help you retrieve your data.</span></span>

<span data-ttu-id="1ac8b-186">収益は、[ **トランザクション履歴** ] ページと [ **支払い** ] ページの両方に表示されます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-186">Earnings are displayed on both the **Transaction history** page and the **Payments** page.</span></span> <span data-ttu-id="1ac8b-187">パートナーセンターのナビゲーションバーで [ **支払い** ] アイコンを選択すると、両方のページにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-187">You can access both pages by selecting the **Payout** icon on the navigation bar in Partner Center.</span></span>

:::image type="content" source="images/incentives/paymenticon.png" alt-text="トランザクション情報":::

<span data-ttu-id="1ac8b-189">トランザクション履歴ビューの月単位の数量は、特定の月に受信した支払額と一致しない場合があります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-189">Monthly earning amounts in the Transaction history view may not align with the payment amount received for a specific month.</span></span> <span data-ttu-id="1ac8b-190">これは、将来の支払いに適用される前の計算期間の再計算と調整に起因します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-190">This is due to recalculations and adjustments for prior earning periods that are applied to future payments.</span></span>

<span data-ttu-id="1ac8b-191">たとえば、2019年9月に処理された2019年1月の収益の調整は、9月の2019の利益には反映されません。ただし、2019年9月の支払いを受け取ると、9月に適用された1月2019の調整が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-191">For example, an adjustment for January 2019 earnings that was processed in September 2019 will not be reflected in the earnings amount for September 2019; however, when the payment for September 2019 is received, it will include the adjustment for January 2019 that was applied in September.</span></span>

<span data-ttu-id="1ac8b-192">このシナリオでは、支払いに含まれるすべての利益の完全なビューを取得するために、トランザクションの詳細をダウンロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-192">In this scenario, you would need to download the transaction details to get a complete view of all earnings included in your payment.</span></span>  <span data-ttu-id="1ac8b-193">また、[支払い] ビューに移動して、各支払いのトランザクションをダウンロードすることもできます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-193">Additionally, you can navigate to the Payments view to download transactions for each payment.</span></span>

### <a name="transaction-history"></a><span data-ttu-id="1ac8b-194">取引履歴</span><span class="sxs-lookup"><span data-stu-id="1ac8b-194">Transaction history</span></span>

<span data-ttu-id="1ac8b-195">このビューには、月ごとの収入と支払いの傾向、状態ごとの収益、およびトランザクションの詳細と、各トランザクションの支払いの状態が表示されます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-195">This view shows earning and payment trends by month, earnings by status, and transaction details along with the payment status for each transaction.</span></span> <span data-ttu-id="1ac8b-196">データは、ユーザーまたは管理者がインセンティブを持っているプログラムと MPN の Id に対してのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-196">Data is only visible for the programs and MPN IDs for which you're an incentive user or admin.</span></span>

### <a name="payments"></a><span data-ttu-id="1ac8b-197">支払い</span><span class="sxs-lookup"><span data-stu-id="1ac8b-197">Payments</span></span>

<span data-ttu-id="1ac8b-198">このビューでは、すべてのプログラムと MPN Id の支払いを表示できます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-198">This view allows you to view payments for all programs and MPN IDs.</span></span> <span data-ttu-id="1ac8b-199">データは、ユーザーまたは管理者がインセンティブを持っているプログラムと MPN の Id に対してのみ表示されます。このビューでは、送金をダウンロードしたり、支払い別にトランザクションの詳細を表示したりできます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-199">Data is only visible for the programs and MPN IDs for which you're an incentive user or admin. From this view, you can download remittance or view transaction details by payment.</span></span>

| <span data-ttu-id="1ac8b-200">目的</span><span class="sxs-lookup"><span data-stu-id="1ac8b-200">To do this</span></span> | <span data-ttu-id="1ac8b-201">参照先</span><span class="sxs-lookup"><span data-stu-id="1ac8b-201">Go here</span></span> |
| ------ | :----------- | 
| <span data-ttu-id="1ac8b-202">支払い情報を1行ずつ表示する (現地通貨での数量と支払額を含む)</span><span class="sxs-lookup"><span data-stu-id="1ac8b-202">View your payment information by line, including earning and payment amounts in local currency</span></span>  | <span data-ttu-id="1ac8b-203">支払いフィールド **の一覧** を参照する</span><span class="sxs-lookup"><span data-stu-id="1ac8b-203">See the **List of Payments** field</span></span>   |
| <span data-ttu-id="1ac8b-204">送金レターをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="1ac8b-204">Download a remittance letter</span></span>   |  <span data-ttu-id="1ac8b-205">**支払い送金** の選択</span><span class="sxs-lookup"><span data-stu-id="1ac8b-205">Select **Payment remittance**</span></span>  |
| <span data-ttu-id="1ac8b-206">特定の支払いのトランザクションレベルの詳細を表示する</span><span class="sxs-lookup"><span data-stu-id="1ac8b-206">View transaction level details for a specific payment</span></span> |  <span data-ttu-id="1ac8b-207">**ビュー** の選択</span><span class="sxs-lookup"><span data-stu-id="1ac8b-207">Select **View**</span></span>  |
| <span data-ttu-id="1ac8b-208">トランザクションの詳細を Excel にエクスポートする</span><span class="sxs-lookup"><span data-stu-id="1ac8b-208">Export transaction details to Excel</span></span>  |  <span data-ttu-id="1ac8b-209">[ **ダウンロードの開始**] を選択し、[ **データのエクスポート**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-209">Select **Start download**, and then select **Export data**.</span></span> <span data-ttu-id="1ac8b-210">選択したすべてのフィルターが、エクスポートされたデータに適用されます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-210">All selected filters will be applied to the exported data.</span></span> <span data-ttu-id="1ac8b-211">状態が [完了] に変わったら、[ **ダウンロード** ] を選択し、画面の指示に従って詳細なトランザクションレポートをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-211">Once the status has changed to Completed, select **Download** and follow the prompts to export the detailed transactions report.</span></span> <span data-ttu-id="1ac8b-212">5分以内に状態が更新されない場合は、ページを更新します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-212">Refresh the page if the status is not updated within five minutes.</span></span>  |

### <a name="missing-or-incorrect-earnings-and-payments"></a><span data-ttu-id="1ac8b-213">収益と支払いの欠如または誤検出</span><span class="sxs-lookup"><span data-stu-id="1ac8b-213">Missing or incorrect earnings and payments</span></span>

<span data-ttu-id="1ac8b-214">支払いまたはトランザクションの詳細が見つからない場合は、適切なフィルターが適用されているかどうかを確認してください。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-214">If you’re unable to locate a payment or transaction details, check to see whether you’ve applied the correct filters.</span></span> <span data-ttu-id="1ac8b-215">一部のプログラム名は変更されているため (たとえば、CSP 1T Direct Partner は CSP Direct Bill パートナーになります)、複数の選択肢を使用することが必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-215">Since some program names have changed (for example, CSP 1T Direct Partner is now CSP Direct Bill Partner), you may need to use multiple selections.</span></span>

<span data-ttu-id="1ac8b-216">それでも利益が得られない場合や、表示される収益が間違っていると思われる場合は、 [サポート](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-216">If you still can’t find your earnings or believe the earnings shown are incorrect, contact [Support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).</span></span>

## <a name="how-do-i-reconcile-my-earnings"></a><span data-ttu-id="1ac8b-217">収益を調整操作方法</span><span class="sxs-lookup"><span data-stu-id="1ac8b-217">How do I reconcile my earnings?</span></span>

<span data-ttu-id="1ac8b-218">収益に不一致がある場合は、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-218">If there’s a discrepancy in your earnings, complete the following steps:</span></span>

1. <span data-ttu-id="1ac8b-219">**収益を受け取る資格を持っていることを確認します。**</span><span class="sxs-lookup"><span data-stu-id="1ac8b-219">**Verify that you’re eligible for earnings.**</span></span>  <span data-ttu-id="1ac8b-220">利益は、 [プログラムの適格性](incentives-determined-your-program-eligibility.md) と利益の両方の [適格性](incentives-confirm-your-earnings-eligibility.md)を満たしている場合にのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-220">Earnings will be available only if you meet both [program eligibility](incentives-determined-your-program-eligibility.md) and [earnings eligibility](incentives-confirm-your-earnings-eligibility.md).</span></span>

2. <span data-ttu-id="1ac8b-221">**支払いプロファイルが完了していることを確認します。**</span><span class="sxs-lookup"><span data-stu-id="1ac8b-221">**Verify that your payment profile is complete.**</span></span>  <span data-ttu-id="1ac8b-222">インセンティブの収益の開始日は、すべての適格性の要件 (支払いと税金でのオンボードの詳細を含む) を完了した月の最初の日になります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-222">Your incentive earnings start date will be the first day of the month in which you’ve completed all of the eligibility requirements, including onboarding with payout and tax details.</span></span> <span data-ttu-id="1ac8b-223">支払いおよび税務プロファイルが完了する前の数か月は収益を利用できません。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-223">Earnings will not be available for the months prior to payout and tax completion.</span></span> <span data-ttu-id="1ac8b-224">たとえば、2020 年 4 月にすべての要件を満たした場合、収益の開始日は 2020 年 4 月 1 日になります。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-224">For example, if you complete all of the requirements during the month of April 2020, your earnings start date will be April 1, 2020.</span></span> 

3. <span data-ttu-id="1ac8b-225">**要件を満たしていることを確認します。**</span><span class="sxs-lookup"><span data-stu-id="1ac8b-225">**Verify that you’ve met the requirements.**</span></span>  <span data-ttu-id="1ac8b-226">インセンティブプログラムの [資格](#my-payment-is-missing-or-incorrect) と適格な収益ルールが満たされているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-226">Check to see whether you have met the [eligibility](#my-payment-is-missing-or-incorrect) and eligible revenue rules for your incentive program.</span></span>

<span data-ttu-id="1ac8b-227">これらのアクションが役に立ちませんが、収益がまだ調整されていない場合は、 [サポート](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-227">If these actions don’t help and your earnings are still not reconciled, contact [Support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).</span></span>

## <a name="where-can-i-find-my-rates"></a><span data-ttu-id="1ac8b-228">料金はどこで確認できますか。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-228">Where can I find my rates?</span></span>

1. <span data-ttu-id="1ac8b-229">[パートナーインセンティブ](https://partner.microsoft.com/membership/partner-incentives)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-229">Sign into [Partner incentives](https://partner.microsoft.com/membership/partner-incentives).</span></span>

2. <span data-ttu-id="1ac8b-230">下にスクロールして、プログラムのドキュメントにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-230">Scroll down to access the documents for your program.</span></span>

3. <span data-ttu-id="1ac8b-231">各プログラムの [ドキュメント] リンクを選択します。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-231">Select the document link for the respective program.</span></span>

4. <span data-ttu-id="1ac8b-232">このドキュメントでは、「プログラムの **構造と料金**」セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ac8b-232">In the document, refer to the section **Program structure and Rates**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1ac8b-233">次の手順</span><span class="sxs-lookup"><span data-stu-id="1ac8b-233">Next steps</span></span>

- [<span data-ttu-id="1ac8b-234">協力申請の管理</span><span class="sxs-lookup"><span data-stu-id="1ac8b-234">Manage co-op claims</span></span>](incentives-managing-co-op-claims.md)