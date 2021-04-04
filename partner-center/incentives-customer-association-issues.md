---
title: 顧客の関連付けのインセンティブに関する問題
description: 要求されたパートナーのレコード (CPOR) の顧客関連付けを使用して作業するときに発生する問題に対処する方法について説明します。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: 30639725c0a852046251e83c3791f56d788931c1
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/02/2021
ms.locfileid: "106179214"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a><span data-ttu-id="65ca3-103">要求されるパートナーのレコード (CPOR) 顧客の関連付けに関する問題</span><span class="sxs-lookup"><span data-stu-id="65ca3-103">Issues with Claimed Partner of Record (CPOR) customer associations</span></span>

<span data-ttu-id="65ca3-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="65ca3-104">**Appropriate roles**</span></span>

- <span data-ttu-id="65ca3-105">課金管理者</span><span class="sxs-lookup"><span data-stu-id="65ca3-105">Billing admin</span></span>
- <span data-ttu-id="65ca3-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="65ca3-106">Global admin</span></span>
- <span data-ttu-id="65ca3-107">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="65ca3-107">Incentives admin</span></span>

<span data-ttu-id="65ca3-108">以下の内容は、顧客の関連付けを操作するときに発生する可能性のある問題を解決するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="65ca3-108">The content below will help you solve issues that can come up when you work with customer associations.</span></span>

## <a name="domain-tenant-mismatch"></a><span data-ttu-id="65ca3-109">ドメインテナントの不一致</span><span class="sxs-lookup"><span data-stu-id="65ca3-109">Domain-tenant mismatch</span></span>

<span data-ttu-id="65ca3-110">要求されたパートナーのレコード (CPOR) アソシエーション要求フローで、顧客のテナント ID とサブドメインを入力するように求められます。</span><span class="sxs-lookup"><span data-stu-id="65ca3-110">In the Claimed Partner of Record (CPOR) association claim flow, you will be asked to provide the customer tenant ID and subdomain.</span></span> <span data-ttu-id="65ca3-111">一致しないというエラーが表示された場合は、お客様に適切な詳細情報があることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="65ca3-111">If you receive an error stating that they don’t match, contact your customer to ensure you have the correct details.</span></span>

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a><span data-ttu-id="65ca3-112">CPOR アソシエーション要求フローでのサブスクリプションエラー</span><span class="sxs-lookup"><span data-stu-id="65ca3-112">Subscription errors in the CPOR association claim flow</span></span>

<span data-ttu-id="65ca3-113">CPOR アソシエーション要求フローでは、Business Applications (Dynamics 365) を介して要求しようとしている製品のサブスクリプションを提供するように求められる場合があります。</span><span class="sxs-lookup"><span data-stu-id="65ca3-113">In the CPOR association claim flow, you may be asked to provide a subscription for a product that you're trying to claim via Business Applications (Dynamics 365).</span></span> <span data-ttu-id="65ca3-114">製品とサブスクリプションが要求されているテナントに属しているかどうかを動的に確認しているため、サブスクリプションを要求します。</span><span class="sxs-lookup"><span data-stu-id="65ca3-114">We ask for the subscription because we're dynamically checking that the product and subscription belong to the tenant being claimed for.</span></span> <span data-ttu-id="65ca3-115">また、サブスクリプションがアクティブであるか、または猶予状態になっていることを確認しています。</span><span class="sxs-lookup"><span data-stu-id="65ca3-115">We're also checking that the subscription is in active/in grace status.</span></span>

<span data-ttu-id="65ca3-116">エラーが発生した場合は、いくつかの理由が考えられます。</span><span class="sxs-lookup"><span data-stu-id="65ca3-116">If you receive the error, it could be for several reasons:</span></span>

- <span data-ttu-id="65ca3-117">選択された製品が顧客のテナントに存在しない</span><span class="sxs-lookup"><span data-stu-id="65ca3-117">The product selected doesn’t exist on the customer’s tenant</span></span>
- <span data-ttu-id="65ca3-118">指定されたサブスクリプションは Dynamics 向けではありません</span><span class="sxs-lookup"><span data-stu-id="65ca3-118">The subscription provided isn't for Dynamics</span></span>
- <span data-ttu-id="65ca3-119">指定されたサブスクリプションが CSP を対象としている</span><span class="sxs-lookup"><span data-stu-id="65ca3-119">The subscription provided is for CSP</span></span>
- <span data-ttu-id="65ca3-120">お客様は、そのサブスクリプションの製品をまだアクティブ化/プロビジョニングしていません</span><span class="sxs-lookup"><span data-stu-id="65ca3-120">The customer hasn't yet activated/provisioned the products for that subscription</span></span>
- <span data-ttu-id="65ca3-121">サブスクリプションが既に要求されている</span><span class="sxs-lookup"><span data-stu-id="65ca3-121">The subscription has already been claimed</span></span>
- <span data-ttu-id="65ca3-122">指定された識別子はサブスクリプション ID ではありません</span><span class="sxs-lookup"><span data-stu-id="65ca3-122">The identifier provided isn't a subscription ID</span></span>

<span data-ttu-id="65ca3-123">サブスクリプションの精度に関する質問がある場合は、お客様と協力して、サブスクリプションが正しいこと、および正しいテナント ID を使用していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="65ca3-123">If you have a question about the accuracy of your subscription, work with your customer to ensure the subscription is correct and that you're using the correct tenant ID.</span></span>

<span data-ttu-id="65ca3-124">このルートが問題を解決していない場合は、 [サポート](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="65ca3-124">If this route hasn't resolved your issue, contact [support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).</span></span>

## <a name="when-subscriptions-will-be-available-to-claim"></a><span data-ttu-id="65ca3-125">サブスクリプションが要求に使用できるようになるタイミング</span><span class="sxs-lookup"><span data-stu-id="65ca3-125">When subscriptions will be available to claim</span></span>

<span data-ttu-id="65ca3-126">サブスクリプションを要求するときに、サブスクリプションがまだプロビジョニングされていない場合は、エラーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="65ca3-126">When claiming for a subscription, you will receive an error if the subscription hasn't been provisioned yet.</span></span> <span data-ttu-id="65ca3-127">お客様がサブスクリプションを取得して要求に使用できるようにするために、お客様がサブスクリプションを利用できるようにするには、いくつかの手順を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="65ca3-127">There are several steps the customer needs to take for the subscription to become available for the CPOR platform to pick it up and make it available to claim.</span></span> <span data-ttu-id="65ca3-128">サブスクリプションを要求しているときにエラーが発生した場合は、顧客に連絡して、サブスクリプションがプロビジョニングされていること、および要求されているサブスクリプションが正しいことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="65ca3-128">If you're receiving an error when trying to claim a subscription, contact your customer to ensure that it has been provisioned and the subscription you're claiming is correct.</span></span> <span data-ttu-id="65ca3-129">このルートを既に取得している場合は、 [サポート](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="65ca3-129">If you have taken this route already, contact [support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).</span></span>

## <a name="which-activity-do-i-choose"></a><span data-ttu-id="65ca3-130">どのアクティビティを選択しますか?</span><span class="sxs-lookup"><span data-stu-id="65ca3-130">Which activity do I choose?</span></span>

<span data-ttu-id="65ca3-131">CPOR が要求されているプラットフォームでは、Business Applications および Microsoft 365 ソリューション領域に関連する CPOR アソシエーション要求を使用できます。</span><span class="sxs-lookup"><span data-stu-id="65ca3-131">The CPOR claiming platform allows for CPOR association claims related to Business Applications and Microsoft 365 solution areas.</span></span> <span data-ttu-id="65ca3-132">各ソリューション領域に適用可能なアクティビティを以下に示します。</span><span class="sxs-lookup"><span data-stu-id="65ca3-132">The activities that are applicable to each solution area are below.</span></span> <span data-ttu-id="65ca3-133">後で再利用する必要がないように、説明に基づいて適切なアクティビティを選択します。</span><span class="sxs-lookup"><span data-stu-id="65ca3-133">Select the correct activity based on the descriptions to avoid having to reclaim in the future.</span></span> <span data-ttu-id="65ca3-134">不適切なアクティビティによって要求されると、適格性とインセンティブの利益が失われる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="65ca3-134">Claiming with an incorrect activity may result in missed eligibility and incentive earnings.</span></span>


| <span data-ttu-id="65ca3-135">ソリューション分野</span><span class="sxs-lookup"><span data-stu-id="65ca3-135">Solution area</span></span> | <span data-ttu-id="65ca3-136">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="65ca3-136">Activity</span></span> | <span data-ttu-id="65ca3-137">適用対象</span><span class="sxs-lookup"><span data-stu-id="65ca3-137">Applicable for</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="65ca3-138">ビジネス アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65ca3-138">Business applications</span></span>      | <span data-ttu-id="65ca3-139">プリセールス</span><span class="sxs-lookup"><span data-stu-id="65ca3-139">Presales</span></span>   | <span data-ttu-id="65ca3-140">対象となる製品の購入に影響を受けた場合に、販売前のインセンティブに適用するかどうかを選択します。</span><span class="sxs-lookup"><span data-stu-id="65ca3-140">Select if you influenced their purchase of an eligible product, and want to apply for pre-sale incentives.</span></span> <span data-ttu-id="65ca3-141">このオプションは、顧客がボリュームライセンス契約または Web ダイレクトを使用してこれらの製品を購入した場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="65ca3-141">This option is only applicable if the customer purchased these products via Volume Licensing agreement or Web-Direct.</span></span> |
|    |  <span data-ttu-id="65ca3-142">使用法</span><span class="sxs-lookup"><span data-stu-id="65ca3-142">Usage</span></span>  | <span data-ttu-id="65ca3-143">対象となるワークロードの導入と使用を推進し、使用量のインセンティブに適用する場合は、オンにします。</span><span class="sxs-lookup"><span data-stu-id="65ca3-143">Select if you drive their adoption and usage of an eligible workload, and want to apply for usage incentives.</span></span> <span data-ttu-id="65ca3-144">このオプションは、顧客がボリュームライセンス契約または Web ダイレクトを使用してこれらの製品を購入した場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="65ca3-144">This option is only applicable if the customer purchased these products via Volume Licensing agreement or Web-Direct.</span></span> |
|    | <span data-ttu-id="65ca3-145">収益の関連付け</span><span class="sxs-lookup"><span data-stu-id="65ca3-145">Revenue association</span></span>   | <span data-ttu-id="65ca3-146">ビジネスの有力者として、対象製品の選択が影響を受けた場合に選択します。</span><span class="sxs-lookup"><span data-stu-id="65ca3-146">Select if you influenced their selection of an eligible product as a Business Influencer.</span></span> <span data-ttu-id="65ca3-147">このオプションは、インセンティブ支払いではなく、収益の関連付けのみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="65ca3-147">This option is for revenue association only, not for incentive payments.</span></span> <span data-ttu-id="65ca3-148">このオプションは、顧客がボリュームライセンス契約または Web ダイレクトを使用してこれらの製品を購入した場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="65ca3-148">This option is only applicable if the customer purchased these products via Volume Licensing agreement or Web-Direct.</span></span>   |
| <span data-ttu-id="65ca3-149">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="65ca3-149">Microsoft 365</span></span>   | <span data-ttu-id="65ca3-150">使用法</span><span class="sxs-lookup"><span data-stu-id="65ca3-150">Usage</span></span>   | <span data-ttu-id="65ca3-151">対象となるワークロードの導入と使用を推進し、使用量のインセンティブに適用する場合は、オンにします。</span><span class="sxs-lookup"><span data-stu-id="65ca3-151">Select if you drive their adoption and usage of an eligible workload, and want to apply for usage incentives.</span></span> |

## <a name="which-mpn-do-i-choose"></a><span data-ttu-id="65ca3-152">どの MPN を選択しますか?</span><span class="sxs-lookup"><span data-stu-id="65ca3-152">Which MPN do I choose?</span></span>

<span data-ttu-id="65ca3-153">CPOR アソシエーション要求のフローでは、エンドユーザーが要求している作業に関連付ける必要のある会社の MPN を選択するよう求められます。</span><span class="sxs-lookup"><span data-stu-id="65ca3-153">In the CPOR association claim flow, you will be asked to choose a company MPN that should be associated to the work you're claiming for at the end customer.</span></span> <span data-ttu-id="65ca3-154">会社には多くの MPNs があり、その中にはインセンティブプログラムに登録されているものと、FRP FastTrack などのパートナータイプに関連付けられているものがあります。</span><span class="sxs-lookup"><span data-stu-id="65ca3-154">Your company may have many MPNs, some of which may be enrolled in incentive programs, and others associated with a partner type such as FRP FastTrack.</span></span> <span data-ttu-id="65ca3-155">CPOR アソシエーション要求フローでは、インセンティブプログラムに登録されている MPNs が識別されますが、特定のパートナータイプ MPN であるかどうかはわかりません。</span><span class="sxs-lookup"><span data-stu-id="65ca3-155">The CPOR association claim flow will identify which MPNs are enrolled in an incentive program, but it will not tell you if it is a specific partner type MPN.</span></span> <span data-ttu-id="65ca3-156">将来の再利用を避けるために、適切な MPN を選択することが重要です。</span><span class="sxs-lookup"><span data-stu-id="65ca3-156">It’s important to select the correct MPN, to avoid having to reclaim in the future.</span></span> <span data-ttu-id="65ca3-157">不適切な MPN を要求すると、適格性とインセンティブの利益が失われる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="65ca3-157">Claiming with an incorrect MPN may result in missed eligibility and incentive earnings.</span></span>

<span data-ttu-id="65ca3-158">使用する MPN がわからない場合は、全体管理者に問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="65ca3-158">If you do not know which MPN to use, contact your global admin.</span></span>

<span data-ttu-id="65ca3-159">使用しようとしている MPN が登録されていない場合は、[ [インセンティブの概要] タブ](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) で管理できます (必要なサインイン)。</span><span class="sxs-lookup"><span data-stu-id="65ca3-159">If the MPN you're wanting to use isn't enrolled, you can manage that in the [Incentives overview tab](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (sign-in required).</span></span>

## <a name="choosing-a-product-vs-entering-a-subscription"></a><span data-ttu-id="65ca3-160">製品の選択とサブスクリプションの入力</span><span class="sxs-lookup"><span data-stu-id="65ca3-160">Choosing a product vs entering a subscription</span></span>

<span data-ttu-id="65ca3-161">Dynamics 製品が要求され、承認されると、パートナーは CPOR アソシエーション要求自体でサブスクリプション ID を表示できます。</span><span class="sxs-lookup"><span data-stu-id="65ca3-161">When a Dynamics product is claimed and approved, the partner can view the subscription ID in the CPOR association claim itself.</span></span> <span data-ttu-id="65ca3-162">このサブスクリプションが要求されると、アクティブまたは猶予状態になりますが、サブスクリプションが終了し、新しいサブスクリプションが別の CPOR アソシエーション要求で要求される必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="65ca3-162">When this subscription is claimed, it is in active or in grace status, but there may be a time when the subscription ends, and the new subscriptions will need to be claimed in a separate CPOR association claim.</span></span>

## <a name="competing-claims"></a><span data-ttu-id="65ca3-163">競合している要求</span><span class="sxs-lookup"><span data-stu-id="65ca3-163">Competing claims</span></span>

<span data-ttu-id="65ca3-164">顧客と、既に別のパートナーに関連付けられている製品に対して CPOR アソシエーション要求を作成している場合は、次のように決定されます。</span><span class="sxs-lookup"><span data-stu-id="65ca3-164">If you're creating a CPOR association claim for a customer and their product(s) that is already associated with another partner, your claim will go through arbitration:</span></span>

1. <span data-ttu-id="65ca3-165">新しい顧客の関連付けの作成後、指定された関連付けおよび実行証明の詳細の検証が Microsoft によって行われ、その正確性が確保されます。</span><span class="sxs-lookup"><span data-stu-id="65ca3-165">After you create a new customer association, Microsoft will verify the details of the association and proof of execution provided to ensure its accuracy.</span></span>

2. <span data-ttu-id="65ca3-166">お客様と別のパートナーが同じ顧客と製品/ワークロードを要求した場合、Microsoft は各パートナーの実行に関するドキュメントをレビューして、承認するパートナーを決定します。</span><span class="sxs-lookup"><span data-stu-id="65ca3-166">If you and another partner claim the same customer and product/workload, Microsoft will review each partner's proof of execution documentation to determine which partner to approve.</span></span>

3. <span data-ttu-id="65ca3-167">両方のパートナーから追加情報が要求されている可能性があります。これにより、アソシエーション要求の処理に遅延が生じる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="65ca3-167">Additional information might be requested from both partners, which could cause delays in processing your association request.</span></span>

4. <span data-ttu-id="65ca3-168">お客様の CPOR はアソシエーションの要求は、5営業日以内に確認されますが、その状態は長期間にわたって _レビュー中_ のままになる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="65ca3-168">Your CPOR association claim will still be reviewed within five business days, although its status may stay as _Under Review_ for a longer period of time.</span></span> <span data-ttu-id="65ca3-169">このシナリオは、Microsoft が現在製品/ワークロードを所有しているパートナーと協力している場合に発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="65ca3-169">This scenario can happen when Microsoft works with the partner currently owning the product/workload.</span></span> <span data-ttu-id="65ca3-170">その場合は、要求のコメントセクション内で通知されます。</span><span class="sxs-lookup"><span data-stu-id="65ca3-170">You will be notified within the comments section of your claim if that is the case.</span></span> 

>[!IMPORTANT]
><span data-ttu-id="65ca3-171">CPOR 関連付けの実行 (PoE) を検証するために追加情報が必要な場合は、「CPOR アソシエーションの要求コメント」セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="65ca3-171">If we require additional information to verify your CPOR association proof of execution (PoE), we'll contact you via the CPOR association claim comments section.</span></span>

## <a name="next-steps"></a><span data-ttu-id="65ca3-172">次のステップ</span><span class="sxs-lookup"><span data-stu-id="65ca3-172">Next steps</span></span>

- [<span data-ttu-id="65ca3-173">インセンティブの概要</span><span class="sxs-lookup"><span data-stu-id="65ca3-173">Getting started with incentives</span></span>](incentives-get-started-intro.md)
