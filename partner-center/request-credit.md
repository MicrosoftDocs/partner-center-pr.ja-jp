---
title: Microsoft から SLA クレジットを要求する
ms.topic: article
ms.date: 04/28/2020
description: 顧客がサービスの停止を経験している場合に Microsoft からサービスレベルアグリーメント (SLA) のクレジットを要求するための特典、制限、および手順について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: cb8f6b2280318427b2015403b528fc288ef64d97
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377756"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a><span data-ttu-id="78d55-103">Microsoft からサービスレベルアグリーメント (SLA) のクレジットを要求する方法とタイミング</span><span class="sxs-lookup"><span data-stu-id="78d55-103">How and when to request a service-level agreement (SLA) credit from Microsoft</span></span>

<span data-ttu-id="78d55-104">お客様に提供しているサービスで障害が発生した場合に、Microsoft から**サービスレベルアグリーメント (SLA) のクレジット**を要求することができます。</span><span class="sxs-lookup"><span data-stu-id="78d55-104">You're able to request **service-level agreement (SLA) credits** from Microsoft if a service that you're providing for your customers has an outage.</span></span>

## <a name="sla-credit-calculation"></a><span data-ttu-id="78d55-105">SLA クレジットの計算</span><span class="sxs-lookup"><span data-stu-id="78d55-105">SLA credit calculation</span></span>

<span data-ttu-id="78d55-106">Microsoft からの SLA クレジットは、影響を受けたサービスに基づいて決定されます。</span><span class="sxs-lookup"><span data-stu-id="78d55-106">SLA credits from Microsoft are determined based on which service(s) were impacted.</span></span> <span data-ttu-id="78d55-107">たとえば、顧客が Office 365 スイートを使用していても、SharePoint の停止しか経験していない場合は、顧客の計画全体ではなく、SharePoint に対してのみ SLA クレジットが承認されます。</span><span class="sxs-lookup"><span data-stu-id="78d55-107">For example, if your customer has an Office 365 suite but only experienced a SharePoint outage, the SLA credit is approved only for SharePoint and not the customer's entire plan.</span></span>

<span data-ttu-id="78d55-108">*クレジットは、影響を受けるサービスと停止の期間に基づいて、日割りで評価されます。*</span><span class="sxs-lookup"><span data-stu-id="78d55-108">*Credits are pro-rated based on the service affected and the duration of the outage.*</span></span> <span data-ttu-id="78d55-109">SLA クレジットに適合するシナリオの種類を確認するには、[オンラインサービスの統合](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)された sla に関するドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="78d55-109">To see the types of scenarios that qualify for SLA credits, see the [Online Services Consolidated SLA document](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37).</span></span> <span data-ttu-id="78d55-110">この情報は、クラウドソリューションプロバイダープログラムを通じて販売されたサービスにも適用されます。</span><span class="sxs-lookup"><span data-stu-id="78d55-110">This information applies to services sold through the Cloud Solution Provider program, too.</span></span>

## <a name="request-an-sla-credit"></a><span data-ttu-id="78d55-111">SLA のクレジットを要求する</span><span class="sxs-lookup"><span data-stu-id="78d55-111">Request an SLA credit</span></span>

<span data-ttu-id="78d55-112">*クラウドソリューションプロバイダー (CSP) パートナーは、請求書および必要なすべての情報を、インシデントが発生した月の後のカレンダー月の終わりまでに提出する必要があります。*</span><span class="sxs-lookup"><span data-stu-id="78d55-112">*The Cloud Solution Provider (CSP) partner must submit the claim and all required information by the end of the calendar month following the month in which the incident occurred.*</span></span> <span data-ttu-id="78d55-113">たとえば、インシデントが2月15日に発生した場合、マイクロソフトは、3月31日までに要求と必要なすべての情報を受け取る必要があります。</span><span class="sxs-lookup"><span data-stu-id="78d55-113">For example, if the incident occurred on February 15th, Microsoft must receive the claim and all required information by March 31st.</span></span> <span data-ttu-id="78d55-114">エンドカスタマーと間接リセラーは、SLA クレジット要求を送信できません。間接プロバイダーまたはダイレクト請求パートナーは、その代わりに要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="78d55-114">End customers and indirect resellers can't submit SLA credit claims; either the indirect provider or direct bill partner must submit claims on their behalf.</span></span>

### <a name="required-information"></a><span data-ttu-id="78d55-115">必要な情報</span><span class="sxs-lookup"><span data-stu-id="78d55-115">Required information</span></span>

<span data-ttu-id="78d55-116">マイクロソフトに[SLA クレジット要求を送信](#submit-sla-credit-request)する前に、次の情報を収集してサポートチケットに含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="78d55-116">Before you [submit an SLA credit request](#submit-sla-credit-request) to Microsoft, you must gather the following information to include in your support ticket:</span></span>

- <span data-ttu-id="78d55-117">顧客テナントの GUID</span><span class="sxs-lookup"><span data-stu-id="78d55-117">The customer tenant's GUID</span></span>
- <span data-ttu-id="78d55-118">[停止インシデント識別子](#outage-incident-identifier)</span><span class="sxs-lookup"><span data-stu-id="78d55-118">The [outage incident identifier](#outage-incident-identifier)?</span></span>
- <span data-ttu-id="78d55-119">影響を受けたサブスクリプションは CSP を通じて購入されましたか?</span><span class="sxs-lookup"><span data-stu-id="78d55-119">Were the impacted subscriptions purchased through CSP?</span></span> <span data-ttu-id="78d55-120">(*yes*または*no*)</span><span class="sxs-lookup"><span data-stu-id="78d55-120">(*yes* or *no*)</span></span>

#### <a name="outage-incident-identifier"></a><span data-ttu-id="78d55-121">停止インシデント識別子</span><span class="sxs-lookup"><span data-stu-id="78d55-121">Outage incident identifier</span></span>

<span data-ttu-id="78d55-122">停止インシデントの識別子は、Microsoft 365 管理センターの [ **Service Health** ] ページで確認できます。</span><span class="sxs-lookup"><span data-stu-id="78d55-122">You can find the identifier for the outage incident on the **Service Health** page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="78d55-123">**停止インシデント ID**は、影響を受けるサービスを示す2文字の省略形 (Exchange Online が停止した場合の*EX25194*など) を表す数字です。</span><span class="sxs-lookup"><span data-stu-id="78d55-123">The **Outage Incident ID** is a number preceded by a two-letter abbreviation that indicates the affected service (for example, *EX25194* for an Exchange Online outage).</span></span> <span data-ttu-id="78d55-124">次の表では、一般的なサービスの省略形について説明します。</span><span class="sxs-lookup"><span data-stu-id="78d55-124">The follow table describes common service abbreviations:</span></span>

| <span data-ttu-id="78d55-125">2文字の省略形</span><span class="sxs-lookup"><span data-stu-id="78d55-125">Two-letter abbreviation</span></span> | <span data-ttu-id="78d55-126">Microsoft サービス</span><span class="sxs-lookup"><span data-stu-id="78d55-126">Microsoft service</span></span> |
| ----------------------- | ----------------- |
| <span data-ttu-id="78d55-127">EX</span><span class="sxs-lookup"><span data-stu-id="78d55-127">EX</span></span> | <span data-ttu-id="78d55-128">Exchange Online</span><span class="sxs-lookup"><span data-stu-id="78d55-128">Exchange Online</span></span> |
| <span data-ttu-id="78d55-129">FO</span><span class="sxs-lookup"><span data-stu-id="78d55-129">FO</span></span> | <span data-ttu-id="78d55-130">Exchange Online の保護</span><span class="sxs-lookup"><span data-stu-id="78d55-130">Exchange Online Protection</span></span> |
| <span data-ttu-id="78d55-131">SB</span><span class="sxs-lookup"><span data-stu-id="78d55-131">SB</span></span> | <span data-ttu-id="78d55-132">Skype for Business Online (以前の Lync Online)</span><span class="sxs-lookup"><span data-stu-id="78d55-132">Skype for Business Online (formerly Lync Online)</span></span> |
| <span data-ttu-id="78d55-133">OS</span><span class="sxs-lookup"><span data-stu-id="78d55-133">OS</span></span> | <span data-ttu-id="78d55-134">Office サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="78d55-134">Office Subscription</span></span> |
| <span data-ttu-id="78d55-135"> PB</span><span class="sxs-lookup"><span data-stu-id="78d55-135">PB</span></span> | <span data-ttu-id="78d55-136">Office 365 用 BI 機能</span><span class="sxs-lookup"><span data-stu-id="78d55-136">Power BI for Office 365</span></span> |
| <span data-ttu-id="78d55-137">SP</span><span class="sxs-lookup"><span data-stu-id="78d55-137">SP</span></span> | <span data-ttu-id="78d55-138">SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="78d55-138">SharePoint Online</span></span> |
| <span data-ttu-id="78d55-139">YA</span><span class="sxs-lookup"><span data-stu-id="78d55-139">YA</span></span> | <span data-ttu-id="78d55-140">Yammer Enterprise</span><span class="sxs-lookup"><span data-stu-id="78d55-140">Yammer Enterprise</span></span> |
| <span data-ttu-id="78d55-141">MO</span><span class="sxs-lookup"><span data-stu-id="78d55-141">MO</span></span> | <span data-ttu-id="78d55-142">ポータルエラー</span><span class="sxs-lookup"><span data-stu-id="78d55-142">Portal error</span></span> |

### <a name="submit-sla-credit-request"></a><span data-ttu-id="78d55-143">SLA クレジット要求の送信</span><span class="sxs-lookup"><span data-stu-id="78d55-143">Submit SLA credit request</span></span>

<span data-ttu-id="78d55-144">パートナーセンターのダッシュボードを使用して SLA クレジット要求を Microsoft に送信するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="78d55-144">To submit your SLA credit request to Microsoft through the Partner Center dashboard:</span></span>

1. <span data-ttu-id="78d55-145">パートナー センター ダッシュボードにサインインします。</span><span class="sxs-lookup"><span data-stu-id="78d55-145">Sign in to the Partner Center dashboard.</span></span>
2. <span data-ttu-id="78d55-146">左側のメニューで、[**サービス要求**] を選択し、[**パートナーサポート要求**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="78d55-146">In the left-hand menu, choose **Service requests**, then select **Partner support requests**.</span></span>
3. <span data-ttu-id="78d55-147">[**パートナーの要求**] ページで、[**新しい要求**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="78d55-147">On the **Partner request** page, choose **New request**.</span></span>
4. <span data-ttu-id="78d55-148">[**要求の開始**] ページで、 **CSP-customers、orders、およびサブスクリプション**を検索します。</span><span class="sxs-lookup"><span data-stu-id="78d55-148">On the **Start the request** page, find the section **CSP - customers, orders and subscriptions**.</span></span> <span data-ttu-id="78d55-149">このセクションで、[**問題の種類を選択**] を選択し、[**カスタマーサービスのクレジット要求**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="78d55-149">In this section, choose **Select an issue type**, then select **Customer services credit requests**.</span></span>
5. <span data-ttu-id="78d55-150">[**推奨されるソリューション**] ページで、[**追加のヘルプが必要ですか?**] の [**はい]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="78d55-150">On the **Recommended solutions** page, under **Do you need more help?**, choose **Yes**.</span></span>
6. <span data-ttu-id="78d55-151">[**詳細**] ページで、[**問題の詳細**] セクションに入力します。</span><span class="sxs-lookup"><span data-stu-id="78d55-151">On the **Details** page, fill out the **Issue details** section.</span></span> <span data-ttu-id="78d55-152">[**詳細**] テキストボックスに、前に収集した[必要な情報](#required-information)を入力します。</span><span class="sxs-lookup"><span data-stu-id="78d55-152">In the **Details** text box, be sure to enter the [required information](#required-information) that you gathered earlier.</span></span>
7. <span data-ttu-id="78d55-153">[**送信**] を選択して、SLA クレジット要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="78d55-153">Choose **Submit** to send in your SLA credit request.</span></span>
