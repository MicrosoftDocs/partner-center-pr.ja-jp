---
title: Microsoft から SLA クレジットを要求する
ms.topic: article
ms.date: 03/31/2021
description: 顧客がサービスの停止を経験している場合に Microsoft からサービスレベルアグリーメント (SLA) のクレジットを要求するための特典、制限、および手順について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 3a0bb85143efe3d4135b56985b9a04e2dbe5e4cc
ms.sourcegitcommit: 57442bbbef15a70bd9a042642140cbf2c8608b09
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/09/2021
ms.locfileid: "113519435"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a><span data-ttu-id="41e76-103">Microsoft からサービスレベルアグリーメント (SLA) のクレジットを要求する方法とタイミング</span><span class="sxs-lookup"><span data-stu-id="41e76-103">How and when to request a service-level agreement (SLA) credit from Microsoft</span></span>

<span data-ttu-id="41e76-104">**適切なロール**: 管理エージェント |全体管理者</span><span class="sxs-lookup"><span data-stu-id="41e76-104">**Appropriate roles**: Admin agent | Global admin</span></span>

<span data-ttu-id="41e76-105">お客様に提供しているサービスが停止している場合は、Microsoft からの **サービスレベルアグリーメント (SLA) クレジット** を要求できます。</span><span class="sxs-lookup"><span data-stu-id="41e76-105">You can request **service-level agreement (SLA) credits** from Microsoft if a service that you're providing for your customers has an outage.</span></span>

## <a name="sla-credit-calculation"></a><span data-ttu-id="41e76-106">SLA クレジットの計算</span><span class="sxs-lookup"><span data-stu-id="41e76-106">SLA credit calculation</span></span>

<span data-ttu-id="41e76-107">Microsoft からの SLA クレジットは、影響を受けたサービスに基づいて決定されます。</span><span class="sxs-lookup"><span data-stu-id="41e76-107">SLA credits from Microsoft are determined based on which service(s) were impacted.</span></span> <span data-ttu-id="41e76-108">たとえば、顧客が Office 365 スイートを使用していても、SharePoint の停止のみが発生した場合、SLA クレジットは SharePoint に対してのみ承認され、お客様のプラン全体では承認されません。</span><span class="sxs-lookup"><span data-stu-id="41e76-108">For example, if your customer has an Office 365 suite but only experienced a SharePoint outage, the SLA credit is approved only for SharePoint and not the customer's entire plan.</span></span>

<span data-ttu-id="41e76-109">*クレジットは、影響を受けるサービスと停止の期間に基づいて、日割りで評価されます。*</span><span class="sxs-lookup"><span data-stu-id="41e76-109">*Credits are pro-rated based on the service affected and the duration of the outage.*</span></span> <span data-ttu-id="41e76-110">SLA クレジットに適合するシナリオの種類を確認するには、 [オンラインサービスの統合](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)された sla に関するドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="41e76-110">To see the types of scenarios that qualify for SLA credits, see the [Online Services Consolidated SLA document](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37).</span></span> <span data-ttu-id="41e76-111">この情報は、クラウドソリューションプロバイダー (CSP) プログラムを通じて販売されたサービスにも適用されます。</span><span class="sxs-lookup"><span data-stu-id="41e76-111">This information applies to services sold through the Cloud Solution Provider (CSP) program, too.</span></span>


## <a name="request-an-sla-credit"></a><span data-ttu-id="41e76-112">SLA のクレジットを要求する</span><span class="sxs-lookup"><span data-stu-id="41e76-112">Request an SLA credit</span></span>

<span data-ttu-id="41e76-113">*CSP パートナーは、インシデントが発生した月の後のカレンダー月の終わりまでに要求と必要なすべての情報を送信する必要があります。*</span><span class="sxs-lookup"><span data-stu-id="41e76-113">*The CSP partner must submit the claim and all required information by the end of the calendar month following the month in which the incident occurred.*</span></span> <span data-ttu-id="41e76-114">たとえば、インシデントが2月15日に発生した場合、マイクロソフトは、3月31日までに要求と必要なすべての情報を受け取る必要があります。</span><span class="sxs-lookup"><span data-stu-id="41e76-114">For example, if the incident occurred on February 15, Microsoft must receive the claim and all required information by March 31.</span></span> <span data-ttu-id="41e76-115">エンドカスタマーと間接リセラーは、SLA クレジット要求を送信できません。間接プロバイダーまたはダイレクト請求パートナーは、その代わりに要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="41e76-115">End customers and indirect resellers can't submit SLA credit claims; either the indirect provider or direct bill partner must submit claims on their behalf.</span></span>

> [!NOTE]
> <span data-ttu-id="41e76-116">アドバイザリインシデントは、通常、SLA クレジットの対象にはなりません。</span><span class="sxs-lookup"><span data-stu-id="41e76-116">Advisory incidents are generally not eligible for SLA credits.</span></span> <span data-ttu-id="41e76-117">Service Health ダッシュボードに送信されたインシデントは、テナントが影響を受けている *可能性が* あることを示し、発行時に Microsoft が持っている最適な情報を表します。</span><span class="sxs-lookup"><span data-stu-id="41e76-117">An incident posted to the Service Health Dashboard indicates that a tenant *may* be impacted and represents the best information Microsoft has at the time of publishing.</span></span> <span data-ttu-id="41e76-118">正常性ページデータは、サービスの一般提供を表します。</span><span class="sxs-lookup"><span data-stu-id="41e76-118">Health page data represents the general availability of a service.</span></span> <span data-ttu-id="41e76-119">個々のサービスの影響、軽減策、解決策は異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="41e76-119">Individual service impact, mitigation, and resolution may vary.</span></span> <span data-ttu-id="41e76-120">詳細については、インシデントの最終投稿とインシデントレビューの投稿を確認してください。</span><span class="sxs-lookup"><span data-stu-id="41e76-120">You can review the final Incident Post and Post Incident Review for more details.</span></span> <span data-ttu-id="41e76-121">詳細については、「 [How to check Microsoft 365 service health](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) 」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41e76-121">See [How to check Microsoft 365 service health](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) for more information.</span></span>

### <a name="required-information"></a><span data-ttu-id="41e76-122">必要な情報</span><span class="sxs-lookup"><span data-stu-id="41e76-122">Required information</span></span>

<span data-ttu-id="41e76-123">顧客名、テナント識別子、パートナーチケット番号、チケットが作成された日付/時刻スタンプは、要求を処理するのに十分ではありません。</span><span class="sxs-lookup"><span data-stu-id="41e76-123">Customer name, tenant identifier, partner ticket#, and ticket created date/time stamp are not sufficient for a claim to be processed.</span></span>

<span data-ttu-id="41e76-124">マイクロソフトに [SLA クレジット要求を送信](#submit-sla-credit-request) する前に、サポートチケットに含まれる次の情報を **すべて** 収集する必要があります。</span><span class="sxs-lookup"><span data-stu-id="41e76-124">Before you [submit an SLA credit request](#submit-sla-credit-request) to Microsoft, you must gather **all** the following information to include in your support ticket:</span></span>

- <span data-ttu-id="41e76-125">顧客テナントの GUID</span><span class="sxs-lookup"><span data-stu-id="41e76-125">The customer tenant's GUID</span></span>
- <span data-ttu-id="41e76-126">[停止インシデント識別子](#outage-incident-identifier)</span><span class="sxs-lookup"><span data-stu-id="41e76-126">The [outage incident identifier](#outage-incident-identifier)?</span></span>
- <span data-ttu-id="41e76-127">顧客が停止によって影響を受け、SLA クレジットを要求したことを示す証拠。</span><span class="sxs-lookup"><span data-stu-id="41e76-127">Evidence that the customer was impacted by the outage and has requested an SLA credit.</span></span>
- <span data-ttu-id="41e76-128">影響を受けたサブスクリプションは CSP を通じて購入されましたか?</span><span class="sxs-lookup"><span data-stu-id="41e76-128">Were the impacted subscriptions purchased through CSP?</span></span> <span data-ttu-id="41e76-129">(*yes* または *no*)</span><span class="sxs-lookup"><span data-stu-id="41e76-129">(*yes* or *no*)</span></span>

#### <a name="evidence-that-proves-customer-impact"></a><span data-ttu-id="41e76-130">顧客への影響を証明する証拠</span><span class="sxs-lookup"><span data-stu-id="41e76-130">Evidence that proves customer impact</span></span>

- <span data-ttu-id="41e76-131">ダウンタイムの時間と期間に関する情報</span><span class="sxs-lookup"><span data-stu-id="41e76-131">Information regarding the time and duration of the downtime</span></span>
- <span data-ttu-id="41e76-132">影響を受けるユーザーの数と場所 (該当する場合)</span><span class="sxs-lookup"><span data-stu-id="41e76-132">The number and location(s) of affected users (if applicable)</span></span>
- <span data-ttu-id="41e76-133">発生時のインシデントの解決試行の説明</span><span class="sxs-lookup"><span data-stu-id="41e76-133">Descriptions of your attempts to resolve the incident at the time of occurrence</span></span>
- <span data-ttu-id="41e76-134">影響を受ける顧客からのサポートを要求する電子メール</span><span class="sxs-lookup"><span data-stu-id="41e76-134">An email from the impacted customer requesting support and subsequently credit</span></span>
- <span data-ttu-id="41e76-135">サービスへの影響の解決に関するサポートチケット番号と顧客連絡先の詳細</span><span class="sxs-lookup"><span data-stu-id="41e76-135">The support ticket number and details of customer contact in regard to resolving service impact</span></span>


#### <a name="outage-incident-identifier"></a><span data-ttu-id="41e76-136">停止インシデント識別子</span><span class="sxs-lookup"><span data-stu-id="41e76-136">Outage incident identifier</span></span>

<span data-ttu-id="41e76-137">停止インシデントの識別子は、Microsoft 365 管理センターの [ **Service Health** ] ページで確認できます。</span><span class="sxs-lookup"><span data-stu-id="41e76-137">You can find the identifier for the outage incident on the **Service Health** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="41e76-138">**停止インシデント ID** は、影響を受けるサービスを示す2文字の省略形で始まる番号です (たとえば、Exchange Online の停止の場合は *EX25194* )。</span><span class="sxs-lookup"><span data-stu-id="41e76-138">The **Outage Incident ID** is a number preceded by a two-letter abbreviation that indicates the affected service (for example, *EX25194* for an Exchange Online outage).</span></span> <span data-ttu-id="41e76-139">次の表では、一般的なサービスの省略形について説明します。</span><span class="sxs-lookup"><span data-stu-id="41e76-139">The follow table describes common service abbreviations:</span></span>

| <span data-ttu-id="41e76-140">2文字の省略形</span><span class="sxs-lookup"><span data-stu-id="41e76-140">Two-letter abbreviation</span></span> | <span data-ttu-id="41e76-141">Microsoft サービス</span><span class="sxs-lookup"><span data-stu-id="41e76-141">Microsoft service</span></span> |
| ----------------------- | ----------------- |
| <span data-ttu-id="41e76-142">EX</span><span class="sxs-lookup"><span data-stu-id="41e76-142">EX</span></span> | <span data-ttu-id="41e76-143">Exchange Online</span><span class="sxs-lookup"><span data-stu-id="41e76-143">Exchange Online</span></span> |
| <span data-ttu-id="41e76-144">FO</span><span class="sxs-lookup"><span data-stu-id="41e76-144">FO</span></span> | <span data-ttu-id="41e76-145">Exchange Online Protection</span><span class="sxs-lookup"><span data-stu-id="41e76-145">Exchange Online Protection</span></span> |
| <span data-ttu-id="41e76-146">SB</span><span class="sxs-lookup"><span data-stu-id="41e76-146">SB</span></span> | <span data-ttu-id="41e76-147">Skype for Businessオンライン (以前の Lync Online)</span><span class="sxs-lookup"><span data-stu-id="41e76-147">Skype for Business Online (formerly Lync Online)</span></span> |
| <span data-ttu-id="41e76-148">OS</span><span class="sxs-lookup"><span data-stu-id="41e76-148">OS</span></span> | <span data-ttu-id="41e76-149">Office サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="41e76-149">Office Subscription</span></span> |
| <span data-ttu-id="41e76-150"> PB</span><span class="sxs-lookup"><span data-stu-id="41e76-150">PB</span></span> | <span data-ttu-id="41e76-151">Office 365 用 BI 機能</span><span class="sxs-lookup"><span data-stu-id="41e76-151">Power BI for Office 365</span></span> |
| <span data-ttu-id="41e76-152">SP</span><span class="sxs-lookup"><span data-stu-id="41e76-152">SP</span></span> | <span data-ttu-id="41e76-153">SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="41e76-153">SharePoint Online</span></span> |
| <span data-ttu-id="41e76-154">YA</span><span class="sxs-lookup"><span data-stu-id="41e76-154">YA</span></span> | <span data-ttu-id="41e76-155">Yammer Enterprise</span><span class="sxs-lookup"><span data-stu-id="41e76-155">Yammer Enterprise</span></span> |
| <span data-ttu-id="41e76-156">MO</span><span class="sxs-lookup"><span data-stu-id="41e76-156">MO</span></span> | <span data-ttu-id="41e76-157">ポータルエラー</span><span class="sxs-lookup"><span data-stu-id="41e76-157">Portal error</span></span> |

### <a name="submit-sla-credit-request"></a><span data-ttu-id="41e76-158">SLA クレジット要求の送信</span><span class="sxs-lookup"><span data-stu-id="41e76-158">Submit SLA credit request</span></span>

<span data-ttu-id="41e76-159">パートナーセンターのダッシュボードを使用して SLA クレジット要求を Microsoft に送信するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="41e76-159">To submit your SLA credit request to Microsoft through the Partner Center dashboard:</span></span>

1. <span data-ttu-id="41e76-160">パートナー センター ダッシュボードにサインインします。</span><span class="sxs-lookup"><span data-stu-id="41e76-160">Sign in to the Partner Center dashboard.</span></span>
2. <span data-ttu-id="41e76-161">左側のメニューで、[ **サービス要求**] を選択し、[ **パートナーサポート要求**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="41e76-161">In the left-hand menu, choose **Service requests**, then select **Partner support requests**.</span></span>
3. <span data-ttu-id="41e76-162">[ **パートナーの要求** ] ページで、[ **新しい要求**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="41e76-162">On the **Partner request** page, choose **New request**.</span></span>
4. <span data-ttu-id="41e76-163">[ **要求の開始** ] ページで、 **CSP-customers、orders、およびサブスクリプション** を検索します。</span><span class="sxs-lookup"><span data-stu-id="41e76-163">On the **Start the request** page, find the section **CSP - customers, orders and subscriptions**.</span></span> <span data-ttu-id="41e76-164">このセクションで、[ **問題の種類を選択**] を選択し、[ **カスタマーサービスのクレジット要求**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="41e76-164">In this section, choose **Select an issue type**, then select **Customer services credit requests**.</span></span>
5. <span data-ttu-id="41e76-165">[ **推奨されるソリューション** ] ページで、[ **追加のヘルプが必要ですか?**] の [ **はい]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="41e76-165">On the **Recommended solutions** page, under **Do you need more help?**, choose **Yes**.</span></span>
6. <span data-ttu-id="41e76-166">[ **詳細** ] ページで、[ **問題の詳細** ] セクションに入力します。</span><span class="sxs-lookup"><span data-stu-id="41e76-166">On the **Details** page, fill out the **Issue details** section.</span></span> <span data-ttu-id="41e76-167">[ **詳細** ] テキストボックスに、前に収集した [必要な情報](#required-information) を入力します。</span><span class="sxs-lookup"><span data-stu-id="41e76-167">In the **Details** text box, be sure to enter the [required information](#required-information) that you gathered earlier.</span></span>
7. <span data-ttu-id="41e76-168">[ **送信** ] を選択して、SLA クレジット要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="41e76-168">Choose **Submit** to send in your SLA credit request.</span></span>

## <a name="next-steps"></a><span data-ttu-id="41e76-169">次のステップ</span><span class="sxs-lookup"><span data-stu-id="41e76-169">Next steps</span></span>

- [<span data-ttu-id="41e76-170">顧客に代わって問題を報告する</span><span class="sxs-lookup"><span data-stu-id="41e76-170">Report problems on behalf of your customer</span></span>](report-problems-on-behalf-of-a-customer.md)
