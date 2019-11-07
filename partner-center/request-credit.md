---
title: Microsoft からの SLA クレジットを要求する |パートナーセンター
ms.topic: article
ms.date: 06/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: サービスで障害が発生した場合は、顧客の SLA クレジットを要求できます。
ms.assetid: E7F1F68D-25E5-46C5-9C98-1D0A9FAB7993
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6a04d8e179f48f60c71b2e0e5c723c9d821de797
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/06/2019
ms.locfileid: "73651696"
---
# <a name="request-an-sla-credit-from-microsoft"></a><span data-ttu-id="c0999-103">Microsoft からの SLA クレジットを要求する</span><span class="sxs-lookup"><span data-stu-id="c0999-103">Request an SLA credit from Microsoft</span></span> 

<span data-ttu-id="c0999-104">お客様に提供しているサービスで障害が発生した場合は、Microsoft にクレジットを申請することができます。</span><span class="sxs-lookup"><span data-stu-id="c0999-104">If a service you are providing for your customers has an outage, you are able to request a credit from Microsoft.</span></span> <span data-ttu-id="c0999-105">サービスレベルアグリーメント (SLA) クレジットは、影響を受けたサービスに基づいて決定されます (つまり、顧客が O365 スイートを持ち、SharePoint のみがダウンしている場合は、プラン全体ではなく、SharePoint に対してのみ SLA クレジットが承認されます)。</span><span class="sxs-lookup"><span data-stu-id="c0999-105">Service Level Agreement (SLA) credits are determined based on which service was impacted (i.e. if the customer has an O365 suite and only SharePoint was down, the SLA credit is approved for SharePoint only, not for the entire plan).</span></span>

<span data-ttu-id="c0999-106">クレジットは、影響を受けるサービスと停止の期間に基づいて、日割りで評価されます。</span><span class="sxs-lookup"><span data-stu-id="c0999-106">Credits are pro-rated based on the service affected and the duration of the outage.</span></span> <span data-ttu-id="c0999-107">SLA クレジットの対象となるシナリオの種類を確認するには、[オンラインサービスの統合](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)された sla に関するドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0999-107">To see the types of scenarios that qualify for SLA credits, read the [Online Services Consolidated SLA document](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37).</span></span> <span data-ttu-id="c0999-108">この情報は、クラウドソリューションプロバイダープログラムを通じて販売されたサービスにも適用されます。</span><span class="sxs-lookup"><span data-stu-id="c0999-108">This information applies to services sold through the Cloud Solution Provider program, too.</span></span>

>[!Note]
><span data-ttu-id="c0999-109">**とても重要です！**</span><span class="sxs-lookup"><span data-stu-id="c0999-109">**VERY IMPORTANT!**</span></span> <span data-ttu-id="c0999-110">CSP パートナーは、間接プロバイダーまたはダイレクト請求パートナー (エンドカスタマーまたは間接リセラーではない) のいずれかで、インシデントが発生した月の後のカレンダー月の終わりまでに要求とすべての必要な情報を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0999-110">The CSP partner, either the indirect provider or the direct bill partner, (not the end customer or the indirect reseller) must submit a claim and all required information by the end of the calendar month following the month in which the incident occurred.</span></span> <span data-ttu-id="c0999-111">たとえば、インシデントが2月15日に発生した場合、請求書と必要なすべての情報を3月31日まで受け取る必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0999-111">For example, if the incident occurred on February 15, we must receive the claim and all required information by March 31.</span></span> 

## <a name="required-information"></a><span data-ttu-id="c0999-112">必要な情報</span><span class="sxs-lookup"><span data-stu-id="c0999-112">Required information</span></span>


<span data-ttu-id="c0999-113">SLA のクレジットを要求するには、次の情報を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0999-113">To request an SLA credit, you need to provide the following information:</span></span> 

- <span data-ttu-id="c0999-114">顧客テナントの GUID:</span><span class="sxs-lookup"><span data-stu-id="c0999-114">Customer tenant GUID:</span></span> 

- <span data-ttu-id="c0999-115">停止インシデント #: (下記を参照)</span><span class="sxs-lookup"><span data-stu-id="c0999-115">Outage Incident#: (see below)</span></span>

- <span data-ttu-id="c0999-116">影響を受けたサブスクリプションは CSP を通じて購入されましたか?</span><span class="sxs-lookup"><span data-stu-id="c0999-116">Were the impacted subscriptions purchased via CSP?</span></span> <span data-ttu-id="c0999-117">はい/いいえ</span><span class="sxs-lookup"><span data-stu-id="c0999-117">Yes/No</span></span>

<span data-ttu-id="c0999-118">停止インシデント ID (EX25194 など) は、Microsoft 365 管理センターの [Service Health] ページにあります。</span><span class="sxs-lookup"><span data-stu-id="c0999-118">The Outage Incident ID (such as EX25194) is found on the Service Health page in the Microsoft 365 admin center.</span></span> <span data-ttu-id="c0999-119">インシデント番号の前には、次のような、影響を受けるサービスを示す2文字の省略形が付きます。</span><span class="sxs-lookup"><span data-stu-id="c0999-119">Incident numbers are preceded with a 2-letter abbreviation that indicates the service affected, such as:</span></span>

<span data-ttu-id="c0999-120">例-Exchange Online</span><span class="sxs-lookup"><span data-stu-id="c0999-120">EX - Exchange Online</span></span>

<span data-ttu-id="c0999-121">Exchange Online の保護</span><span class="sxs-lookup"><span data-stu-id="c0999-121">FO - Exchange Online Protection</span></span>

<span data-ttu-id="c0999-122">SB-Skype for Business Online (正式な Lync Online)</span><span class="sxs-lookup"><span data-stu-id="c0999-122">SB - Skype for Business Online (formally Lync Online)</span></span>

<span data-ttu-id="c0999-123">OS-Office サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="c0999-123">OS - Office Subscription</span></span>

<span data-ttu-id="c0999-124">PB-Power BI for Office 365</span><span class="sxs-lookup"><span data-stu-id="c0999-124">PB -Power BI for Office 365</span></span>

<span data-ttu-id="c0999-125">SP-SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="c0999-125">SP - SharePoint Online</span></span>

<span data-ttu-id="c0999-126">YA-Yammer Enterprise</span><span class="sxs-lookup"><span data-stu-id="c0999-126">YA - Yammer Enterprise</span></span>

<span data-ttu-id="c0999-127">MO-ポータルエラー</span><span class="sxs-lookup"><span data-stu-id="c0999-127">MO - Portal Error</span></span>

## <a name="submit-a-request"></a><span data-ttu-id="c0999-128">要求を送信する</span><span class="sxs-lookup"><span data-stu-id="c0999-128">Submit a request</span></span>

<span data-ttu-id="c0999-129">パートナーセンターでクレジット要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="c0999-129">Submit your credit request on Partner Center.</span></span>

1. <span data-ttu-id="c0999-130">パートナーセンターのダッシュボードで、左側のナビゲーションから **[サポート]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c0999-130">From your Partner Center dashboard, select **Support** from the left nav.</span></span>

2. <span data-ttu-id="c0999-131">**[パートナーサポート要求]** を選択し、[ **CSP-customers]、[orders]、[サブスクリプション]、[カスタマーサービスクレジット要求**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="c0999-131">Select **Partner support requests** and then select **CSP - customers, orders, and subscriptions/Customer services credit requests**.</span></span>

3. <span data-ttu-id="c0999-132">SLA のクレジット要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="c0999-132">Submit your SLA credit request.</span></span>





