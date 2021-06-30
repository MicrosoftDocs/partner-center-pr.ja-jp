---
title: Microsoft から SLA クレジットを要求する
ms.topic: article
ms.date: 03/31/2021
description: 顧客にサービス停止が発生した場合に Microsoft にサービス レベル アグリーメント (SLA) クレジットを要求する利点、制限、および手順について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: f521e55869d60987fb46cd5d570bf206939e0782
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080641"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a><span data-ttu-id="f657f-103">Microsoft にサービス レベル アグリーメント (SLA) クレジットを要求する方法と条件</span><span class="sxs-lookup"><span data-stu-id="f657f-103">How and when to request a service-level agreement (SLA) credit from Microsoft</span></span>

<span data-ttu-id="f657f-104">**適切なロール**: 管理エージェント |グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="f657f-104">**Appropriate roles**: Admin agent | Global admin</span></span>

<span data-ttu-id="f657f-105">顧客に提供しているサービスが停止している場合は、Microsoft にサービス レベル アグリーメント **(SLA)** クレジットを要求できます。</span><span class="sxs-lookup"><span data-stu-id="f657f-105">You can request **service-level agreement (SLA) credits** from Microsoft if a service that you're providing for your customers has an outage.</span></span>

## <a name="sla-credit-calculation"></a><span data-ttu-id="f657f-106">SLA クレジットの計算</span><span class="sxs-lookup"><span data-stu-id="f657f-106">SLA credit calculation</span></span>

<span data-ttu-id="f657f-107">Microsoft の SLA クレジットは、影響を受け取ったサービスに基づいて決定されます。</span><span class="sxs-lookup"><span data-stu-id="f657f-107">SLA credits from Microsoft are determined based on which service(s) were impacted.</span></span> <span data-ttu-id="f657f-108">たとえば、顧客が Office 365 スイートを使用しているが、SharePoint の停止しか発生していない場合、SLA クレジットは顧客のプラン全体ではなく SharePoint に対してのみ承認されます。</span><span class="sxs-lookup"><span data-stu-id="f657f-108">For example, if your customer has an Office 365 suite but only experienced a SharePoint outage, the SLA credit is approved only for SharePoint and not the customer's entire plan.</span></span>

<span data-ttu-id="f657f-109">*クレジットは、影響を受けるサービスと停止の期間に基づいて日単位で評価されます。*</span><span class="sxs-lookup"><span data-stu-id="f657f-109">*Credits are pro-rated based on the service affected and the duration of the outage.*</span></span> <span data-ttu-id="f657f-110">SLA クレジットの対象となるシナリオの種類については、オンライン サービス統合 SLA に関するドキュメント [を参照してください](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)。</span><span class="sxs-lookup"><span data-stu-id="f657f-110">To see the types of scenarios that qualify for SLA credits, see the [Online Services Consolidated SLA document](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37).</span></span> <span data-ttu-id="f657f-111">この情報は、クラウド ソリューション プロバイダー (CSP) プログラムを通じて販売されたサービスにも適用されます。</span><span class="sxs-lookup"><span data-stu-id="f657f-111">This information applies to services sold through the Cloud Solution Provider (CSP) program, too.</span></span>


## <a name="request-an-sla-credit"></a><span data-ttu-id="f657f-112">SLA クレジットを要求する</span><span class="sxs-lookup"><span data-stu-id="f657f-112">Request an SLA credit</span></span>

<span data-ttu-id="f657f-113">*CSP パートナーは、インシデントが発生した月の次のカレンダー月の終わりまでに、要求と必要なすべての情報を送信する必要があります。*</span><span class="sxs-lookup"><span data-stu-id="f657f-113">*The CSP partner must submit the claim and all required information by the end of the calendar month following the month in which the incident occurred.*</span></span> <span data-ttu-id="f657f-114">たとえば、インシデントが 2 月 15 日に発生した場合、Microsoft は 3 月 31 日までに要求と必要なすべての情報を受け取る必要があります。</span><span class="sxs-lookup"><span data-stu-id="f657f-114">For example, if the incident occurred on February 15, Microsoft must receive the claim and all required information by March 31.</span></span> <span data-ttu-id="f657f-115">エンド カスタマーと間接リセラーは SLA クレジット要求を送信できない。間接プロバイダーまたは直接請求パートナーは、要求を代理で送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f657f-115">End customers and indirect resellers can't submit SLA credit claims; either the indirect provider or direct bill partner must submit claims on their behalf.</span></span>

> [!NOTE]
> <span data-ttu-id="f657f-116">アドバイザリ インシデントは SLA クレジットの対象ではありません。</span><span class="sxs-lookup"><span data-stu-id="f657f-116">Advisory incidents are not eligible for SLA credits.</span></span> <span data-ttu-id="f657f-117">Service Health ダッシュボードに投稿されたインシデントは、テナントが影響を受け、発行時に Microsoft が持っている最適な情報を表します。</span><span class="sxs-lookup"><span data-stu-id="f657f-117">An incident posted to the Service Health Dashboard indicates that a tenant *may* be impacted and represents the best information Microsoft has at the time of publishing.</span></span> <span data-ttu-id="f657f-118">正常性ページ データは、サービスの一般提供を表します。</span><span class="sxs-lookup"><span data-stu-id="f657f-118">Health page data represents the general availability of a service.</span></span> <span data-ttu-id="f657f-119">個々のサービスへの影響、軽減策、および解決方法は異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="f657f-119">Individual service impact, mitigation, and resolution may vary.</span></span> <span data-ttu-id="f657f-120">詳細については、最終的なインシデント投稿とインシデント後のレビューを確認できます。</span><span class="sxs-lookup"><span data-stu-id="f657f-120">You can review the final Incident Post and Post Incident Review for more details.</span></span> <span data-ttu-id="f657f-121">詳細 [については、「サービスの正常性Microsoft 365する](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) 方法」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f657f-121">See [How to check Microsoft 365 service health](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) for more information.</span></span>

### <a name="required-information"></a><span data-ttu-id="f657f-122">必要な情報</span><span class="sxs-lookup"><span data-stu-id="f657f-122">Required information</span></span>

<span data-ttu-id="f657f-123">要求を処理するには、顧客名、テナント識別子、パートナー チケット#、チケット作成日/タイム スタンプでは十分ではありません。</span><span class="sxs-lookup"><span data-stu-id="f657f-123">Customer name, tenant identifier, partner ticket#, and ticket created date/time stamp are not sufficient for a claim to be processed.</span></span>

<span data-ttu-id="f657f-124">SLA クレジット要求を Microsoft に[送信する前](#submit-sla-credit-request)に、サポート チケットに含める次のすべての情報を収集する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f657f-124">Before you [submit an SLA credit request](#submit-sla-credit-request) to Microsoft, you must gather **all** the following information to include in your support ticket:</span></span>

- <span data-ttu-id="f657f-125">顧客テナントの GUID</span><span class="sxs-lookup"><span data-stu-id="f657f-125">The customer tenant's GUID</span></span>
- <span data-ttu-id="f657f-126">障害 [インシデント識別子](#outage-incident-identifier)?</span><span class="sxs-lookup"><span data-stu-id="f657f-126">The [outage incident identifier](#outage-incident-identifier)?</span></span>
- <span data-ttu-id="f657f-127">顧客が停止の影響を受け、SLA クレジットを要求した証拠。</span><span class="sxs-lookup"><span data-stu-id="f657f-127">Evidence that the customer was impacted by the outage and has requested an SLA credit.</span></span>
- <span data-ttu-id="f657f-128">影響を受け取ったサブスクリプションは CSP を通じて購入されましたか?</span><span class="sxs-lookup"><span data-stu-id="f657f-128">Were the impacted subscriptions purchased through CSP?</span></span> <span data-ttu-id="f657f-129">(*はい\*\*またはいいえ*)</span><span class="sxs-lookup"><span data-stu-id="f657f-129">(*yes* or *no*)</span></span>

#### <a name="evidence-that-proves-customer-impact"></a><span data-ttu-id="f657f-130">顧客への影響を証明する証拠</span><span class="sxs-lookup"><span data-stu-id="f657f-130">Evidence that proves customer impact</span></span>

- <span data-ttu-id="f657f-131">ダウンタイムの時間と期間に関する情報</span><span class="sxs-lookup"><span data-stu-id="f657f-131">Information regarding the time and duration of the downtime</span></span>
- <span data-ttu-id="f657f-132">影響を受けるユーザーの数と場所 (該当する場合)</span><span class="sxs-lookup"><span data-stu-id="f657f-132">The number and location(s) of affected users (if applicable)</span></span>
- <span data-ttu-id="f657f-133">発生時にインシデントを解決しようとする試みについて説明します</span><span class="sxs-lookup"><span data-stu-id="f657f-133">Descriptions of your attempts to resolve the incident at the time of occurrence</span></span>
- <span data-ttu-id="f657f-134">影響を受け、サポートを要求している顧客からの電子メールと、その後のクレジット</span><span class="sxs-lookup"><span data-stu-id="f657f-134">An email from the impacted customer requesting support and subsequently credit</span></span>
- <span data-ttu-id="f657f-135">サービスへの影響の解決に関するサポート チケット番号と顧客の連絡先の詳細</span><span class="sxs-lookup"><span data-stu-id="f657f-135">The support ticket number and details of customer contact in regard to resolving service impact</span></span>


#### <a name="outage-incident-identifier"></a><span data-ttu-id="f657f-136">停止インシデント識別子</span><span class="sxs-lookup"><span data-stu-id="f657f-136">Outage incident identifier</span></span>

<span data-ttu-id="f657f-137">停止インシデントの識別子は、次のページのService Healthで確認Microsoft 365 管理センター。</span><span class="sxs-lookup"><span data-stu-id="f657f-137">You can find the identifier for the outage incident on the **Service Health** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="f657f-138">停止 **インシデント ID は**、影響を受けるサービスを示す 2 文字の省略形が付いた数値です (たとえば、Exchange Online の停止の場合は *EX25194)。*</span><span class="sxs-lookup"><span data-stu-id="f657f-138">The **Outage Incident ID** is a number preceded by a two-letter abbreviation that indicates the affected service (for example, *EX25194* for an Exchange Online outage).</span></span> <span data-ttu-id="f657f-139">次の表では、一般的なサービスの省略形について説明します。</span><span class="sxs-lookup"><span data-stu-id="f657f-139">The follow table describes common service abbreviations:</span></span>

| <span data-ttu-id="f657f-140">2 文字の省略形</span><span class="sxs-lookup"><span data-stu-id="f657f-140">Two-letter abbreviation</span></span> | <span data-ttu-id="f657f-141">Microsoft サービス</span><span class="sxs-lookup"><span data-stu-id="f657f-141">Microsoft service</span></span> |
| ----------------------- | ----------------- |
| <span data-ttu-id="f657f-142">EX</span><span class="sxs-lookup"><span data-stu-id="f657f-142">EX</span></span> | <span data-ttu-id="f657f-143">Exchange Online</span><span class="sxs-lookup"><span data-stu-id="f657f-143">Exchange Online</span></span> |
| <span data-ttu-id="f657f-144">FO</span><span class="sxs-lookup"><span data-stu-id="f657f-144">FO</span></span> | <span data-ttu-id="f657f-145">Exchange Online Protection</span><span class="sxs-lookup"><span data-stu-id="f657f-145">Exchange Online Protection</span></span> |
| <span data-ttu-id="f657f-146">SB</span><span class="sxs-lookup"><span data-stu-id="f657f-146">SB</span></span> | <span data-ttu-id="f657f-147">Skype for Business Online (旧 Lync Online)</span><span class="sxs-lookup"><span data-stu-id="f657f-147">Skype for Business Online (formerly Lync Online)</span></span> |
| <span data-ttu-id="f657f-148">OS</span><span class="sxs-lookup"><span data-stu-id="f657f-148">OS</span></span> | <span data-ttu-id="f657f-149">Office サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="f657f-149">Office Subscription</span></span> |
| <span data-ttu-id="f657f-150"> PB</span><span class="sxs-lookup"><span data-stu-id="f657f-150">PB</span></span> | <span data-ttu-id="f657f-151">Office 365 用 BI 機能</span><span class="sxs-lookup"><span data-stu-id="f657f-151">Power BI for Office 365</span></span> |
| <span data-ttu-id="f657f-152">SP</span><span class="sxs-lookup"><span data-stu-id="f657f-152">SP</span></span> | <span data-ttu-id="f657f-153">SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f657f-153">SharePoint Online</span></span> |
| <span data-ttu-id="f657f-154">屋</span><span class="sxs-lookup"><span data-stu-id="f657f-154">YA</span></span> | <span data-ttu-id="f657f-155">Yammer Enterprise</span><span class="sxs-lookup"><span data-stu-id="f657f-155">Yammer Enterprise</span></span> |
| <span data-ttu-id="f657f-156">MO</span><span class="sxs-lookup"><span data-stu-id="f657f-156">MO</span></span> | <span data-ttu-id="f657f-157">ポータル エラー</span><span class="sxs-lookup"><span data-stu-id="f657f-157">Portal error</span></span> |

### <a name="submit-sla-credit-request"></a><span data-ttu-id="f657f-158">SLA クレジット要求を送信する</span><span class="sxs-lookup"><span data-stu-id="f657f-158">Submit SLA credit request</span></span>

<span data-ttu-id="f657f-159">SLA クレジット要求を Microsoft に送信するには、次のパートナー センターします。</span><span class="sxs-lookup"><span data-stu-id="f657f-159">To submit your SLA credit request to Microsoft through the Partner Center dashboard:</span></span>

1. <span data-ttu-id="f657f-160">パートナー センター ダッシュボードにサインインします。</span><span class="sxs-lookup"><span data-stu-id="f657f-160">Sign in to the Partner Center dashboard.</span></span>
2. <span data-ttu-id="f657f-161">左側のメニューで、[サービス要求] **を選択** し、[パートナー サポート要求 **] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="f657f-161">In the left-hand menu, choose **Service requests**, then select **Partner support requests**.</span></span>
3. <span data-ttu-id="f657f-162">[パートナー要求 **] ページで** 、[新しい要求] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="f657f-162">On the **Partner request** page, choose **New request**.</span></span>
4. <span data-ttu-id="f657f-163">[要求 **の開始] ページ** で、「CSP - 顧客、注文、サブスクリプション」 **セクションを探します**。</span><span class="sxs-lookup"><span data-stu-id="f657f-163">On the **Start the request** page, find the section **CSP - customers, orders and subscriptions**.</span></span> <span data-ttu-id="f657f-164">このセクションで、[問題の **種類の選択] を選択し**、[顧客サービスのクレジット要求 **] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="f657f-164">In this section, choose **Select an issue type**, then select **Customer services credit requests**.</span></span>
5. <span data-ttu-id="f657f-165">[推奨される **ソリューション] ページの** [さらにヘルプが必要ですか **?]** で、[はい] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="f657f-165">On the **Recommended solutions** page, under **Do you need more help?**, choose **Yes**.</span></span>
6. <span data-ttu-id="f657f-166">[詳細 **] ページ** で、[問題の詳細] **セクションに入力** します。</span><span class="sxs-lookup"><span data-stu-id="f657f-166">On the **Details** page, fill out the **Issue details** section.</span></span> <span data-ttu-id="f657f-167">[詳細 **]** テキスト ボックスに、前に収集した [必要](#required-information) な情報を入力してください。</span><span class="sxs-lookup"><span data-stu-id="f657f-167">In the **Details** text box, be sure to enter the [required information](#required-information) that you gathered earlier.</span></span>
7. <span data-ttu-id="f657f-168">[ **送信] を** 選択して、SLA クレジット要求で送信します。</span><span class="sxs-lookup"><span data-stu-id="f657f-168">Choose **Submit** to send in your SLA credit request.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f657f-169">次のステップ</span><span class="sxs-lookup"><span data-stu-id="f657f-169">Next steps</span></span>

- [<span data-ttu-id="f657f-170">顧客に代わって問題を報告する</span><span class="sxs-lookup"><span data-stu-id="f657f-170">Report problems on behalf of your customer</span></span>](report-problems-on-behalf-of-a-customer.md)
