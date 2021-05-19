---
title: 携帯電話会社の請求-Microsoft Store
description: Microsoft Store は、この機能をサポートするモバイルオペレーターの支払い方法として携帯電話の課金を提供します。
ms.date: 04/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.topic: article
ms.author: hickeys
author: hickeys
keywords: windows 10, uwp, 携帯電話会社, 携帯電話への課金, 携帯電話会社による課金
ms.localizationpriority: medium
ms.openlocfilehash: 70d1d05911c927832ae82a402b0c17be52e39cfa
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151544"
---
# <a name="mobile-operator-billing"></a><span data-ttu-id="5a292-104">携帯電話会社による課金</span><span class="sxs-lookup"><span data-stu-id="5a292-104">Mobile operator billing</span></span>

<span data-ttu-id="5a292-105">**適切なロール**: グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="5a292-105">**Appropriate roles**: Global admin</span></span>

> [!NOTE]
> <span data-ttu-id="5a292-106">支払いに関するサポートが必要な場合 (支払いアカウントの構成、行われていない支払い、支払いの保留など) は、[こちら](https://developer.microsoft.com/windows/support)からサポートにお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="5a292-106">If you're looking for support regarding payouts, including configuring payout accounts, missing payouts, putting payouts on hold, or anything else, contact support [here](https://developer.microsoft.com/windows/support).</span></span>

<span data-ttu-id="5a292-107">Microsoft Store は、Windows 10 を実行するデバイスの支払い方法としての携帯電話の請求、Windows 10 Mobile を実行する電話、Xbox One のコンソールを提供します。</span><span class="sxs-lookup"><span data-stu-id="5a292-107">The Microsoft Store offers mobile operator billing as a payment method for devices running Windows 10, phones running Windows 10 Mobile, and Xbox One consoles.</span></span> <span data-ttu-id="5a292-108">お客様の携帯電話事業者がこの機能をサポートしている場合、お客様は、携帯電話の請求を支払い方法として追加し、それを使用して、モバイルアカウントを使用して店舗の購入を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="5a292-108">If a customer’s mobile operator supports this capability, the customer can add mobile operator billing as a payment method and use it to make Store purchases using their mobile account.</span></span>

> [!TIP]
> <span data-ttu-id="5a292-109">お客様の携帯電話会社が携帯電話の請求を提供していても、お客様のデバイスでこのオプションが見つからない場合は、次の [手順](https://support.microsoft.com/instantanswers/b25d6dd6-fb8b-3710-1e13-4d30eb01b51f)を確認してください。</span><span class="sxs-lookup"><span data-stu-id="5a292-109">If a customer’s mobile operator offers mobile operator billing, but the customer can't find this option on their device, review these [steps](https://support.microsoft.com/instantanswers/b25d6dd6-fb8b-3710-1e13-4d30eb01b51f).</span></span>

<span data-ttu-id="5a292-110">弊社は、定期的に携帯電話会社と協力して、この支払方法の機能を拡張しています。</span><span class="sxs-lookup"><span data-stu-id="5a292-110">We are regularly working with mobile operators to expand the availability of this payment method.</span></span> <span data-ttu-id="5a292-111">以下に記載されていない携帯電話会社を提案する場合は、その携帯電話会社に連絡して、この支払い方法を追加するように依頼してください。</span><span class="sxs-lookup"><span data-stu-id="5a292-111">If you’d like to suggest a mobile operator that you don’t see listed below, contact that mobile operator and request that they add this payment method.</span></span>

## <a name="operators-that-support-mobile-operator-billing"></a><span data-ttu-id="5a292-112">携帯電話会社の課金をサポートするオペレーター</span><span class="sxs-lookup"><span data-stu-id="5a292-112">Operators that support mobile operator billing</span></span>

<span data-ttu-id="5a292-113">次の携帯電話事業者は、現在、携帯電話の請求をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="5a292-113">The following mobile operators currently support mobile operator billing.</span></span>

| <span data-ttu-id="5a292-114">国/リージョン</span><span class="sxs-lookup"><span data-stu-id="5a292-114">Country/region</span></span>       | <span data-ttu-id="5a292-115">携帯電話会社</span><span class="sxs-lookup"><span data-stu-id="5a292-115">Mobile operators</span></span>                                        |
|----------------------|---------------------------------------------------------|
| <span data-ttu-id="5a292-116">オーストラリア</span><span class="sxs-lookup"><span data-stu-id="5a292-116">Australia</span></span>            | <span data-ttu-id="5a292-117">Optus</span><span class="sxs-lookup"><span data-stu-id="5a292-117">Optus</span></span>                                                   |
| <span data-ttu-id="5a292-118">オーストリア</span><span class="sxs-lookup"><span data-stu-id="5a292-118">Austria</span></span>              | <span data-ttu-id="5a292-119">A1 テレ、Hutchison 3G オーストリア、T-Mobile/テレ</span><span class="sxs-lookup"><span data-stu-id="5a292-119">A1 Telekom, Hutchison 3G Austria, T-Mobile / tele.ring</span></span>  |
| <span data-ttu-id="5a292-120">ベルギー</span><span class="sxs-lookup"><span data-stu-id="5a292-120">Belgium</span></span>              | <span data-ttu-id="5a292-121">Base、Proximus</span><span class="sxs-lookup"><span data-stu-id="5a292-121">Base, Proximus</span></span>                                          |
| <span data-ttu-id="5a292-122">カナダ</span><span class="sxs-lookup"><span data-stu-id="5a292-122">Canada</span></span>               | <span data-ttu-id="5a292-123">Telus</span><span class="sxs-lookup"><span data-stu-id="5a292-123">Telus</span></span>                                                   |
| <span data-ttu-id="5a292-124">チェコ</span><span class="sxs-lookup"><span data-stu-id="5a292-124">Czechia</span></span>              | <span data-ttu-id="5a292-125">T-Mobile、Vodafone、O2</span><span class="sxs-lookup"><span data-stu-id="5a292-125">T-Mobile, Vodafone, O2</span></span>                                  |
| <span data-ttu-id="5a292-126">デンマーク</span><span class="sxs-lookup"><span data-stu-id="5a292-126">Denmark</span></span>              | <span data-ttu-id="5a292-127">3、TDC / YouSee、Telenor、Telia</span><span class="sxs-lookup"><span data-stu-id="5a292-127">3, TDC / YouSee, Telenor, Telia</span></span>                         |
| <span data-ttu-id="5a292-128">フィンランド</span><span class="sxs-lookup"><span data-stu-id="5a292-128">Finland</span></span>              | <span data-ttu-id="5a292-129">DNA、Elisa</span><span class="sxs-lookup"><span data-stu-id="5a292-129">DNA, Elisa</span></span>                                              |
| <span data-ttu-id="5a292-130">フランス</span><span class="sxs-lookup"><span data-stu-id="5a292-130">France</span></span>               | <span data-ttu-id="5a292-131">オレンジ</span><span class="sxs-lookup"><span data-stu-id="5a292-131">Orange</span></span>                                                  |
| <span data-ttu-id="5a292-132">ドイツ</span><span class="sxs-lookup"><span data-stu-id="5a292-132">Germany</span></span>              | <span data-ttu-id="5a292-133">O2、テレ (Vodafone)、</span><span class="sxs-lookup"><span data-stu-id="5a292-133">O2, Telekom Deutschland, Vodafone</span></span>                       |
| <span data-ttu-id="5a292-134">ハンガリー</span><span class="sxs-lookup"><span data-stu-id="5a292-134">Hungary</span></span>              | <span data-ttu-id="5a292-135">Telenor</span><span class="sxs-lookup"><span data-stu-id="5a292-135">Telenor</span></span>                                                 |
| <span data-ttu-id="5a292-136">イタリア</span><span class="sxs-lookup"><span data-stu-id="5a292-136">Italy</span></span>                | <span data-ttu-id="5a292-137">Tre、風力、Vodafone</span><span class="sxs-lookup"><span data-stu-id="5a292-137">Tre, Wind, Vodafone</span></span>                                     |
| <span data-ttu-id="5a292-138">韓国</span><span class="sxs-lookup"><span data-stu-id="5a292-138">Korea</span></span>                | <span data-ttu-id="5a292-139">SK Telecom</span><span class="sxs-lookup"><span data-stu-id="5a292-139">SK Telecom</span></span>                                              |
| <span data-ttu-id="5a292-140">マレーシア</span><span class="sxs-lookup"><span data-stu-id="5a292-140">Malaysia</span></span>             | <span data-ttu-id="5a292-141">Digi</span><span class="sxs-lookup"><span data-stu-id="5a292-141">Digi</span></span>                                                    |
| <span data-ttu-id="5a292-142">オランダ</span><span class="sxs-lookup"><span data-stu-id="5a292-142">Netherlands</span></span>          | <span data-ttu-id="5a292-143">Vodafone n/Telfort、</span><span class="sxs-lookup"><span data-stu-id="5a292-143">KPN / Telfort, Vodafone</span></span>                                 |
| <span data-ttu-id="5a292-144">ノルウェー</span><span class="sxs-lookup"><span data-stu-id="5a292-144">Norway</span></span>               | <span data-ttu-id="5a292-145">Telenor/Talkmore、Telia/OneCall</span><span class="sxs-lookup"><span data-stu-id="5a292-145">Telenor / Talkmore, Telia / OneCall</span></span>                     |
| <span data-ttu-id="5a292-146">ポーランド</span><span class="sxs-lookup"><span data-stu-id="5a292-146">Poland</span></span>               | <span data-ttu-id="5a292-147">オレンジ色、再生、T-sql</span><span class="sxs-lookup"><span data-stu-id="5a292-147">Orange, Play, T-Mobile</span></span>                                  |
| <span data-ttu-id="5a292-148">サウジアラビア</span><span class="sxs-lookup"><span data-stu-id="5a292-148">Saudi Arabia</span></span>         | <span data-ttu-id="5a292-149">STC</span><span class="sxs-lookup"><span data-stu-id="5a292-149">STC</span></span>                                                     |
| <span data-ttu-id="5a292-150">シンガポール</span><span class="sxs-lookup"><span data-stu-id="5a292-150">Singapore</span></span>            | <span data-ttu-id="5a292-151">M1 限定、StarHub</span><span class="sxs-lookup"><span data-stu-id="5a292-151">M1 Limited, StarHub</span></span>                                     |
| <span data-ttu-id="5a292-152">スロバキア</span><span class="sxs-lookup"><span data-stu-id="5a292-152">Slovakia</span></span>             | <span data-ttu-id="5a292-153">Slovak Telekom</span><span class="sxs-lookup"><span data-stu-id="5a292-153">Slovak Telekom</span></span>                                          |
| <span data-ttu-id="5a292-154">南アフリカ</span><span class="sxs-lookup"><span data-stu-id="5a292-154">South Africa</span></span>         | <span data-ttu-id="5a292-155">Vodacom</span><span class="sxs-lookup"><span data-stu-id="5a292-155">Vodacom</span></span>                                                 |
| <span data-ttu-id="5a292-156">スペイン</span><span class="sxs-lookup"><span data-stu-id="5a292-156">Spain</span></span>                | <span data-ttu-id="5a292-157">オレンジ</span><span class="sxs-lookup"><span data-stu-id="5a292-157">Orange</span></span>                                                  |
| <span data-ttu-id="5a292-158">スウェーデン</span><span class="sxs-lookup"><span data-stu-id="5a292-158">Sweden</span></span>               | <span data-ttu-id="5a292-159">3、telenor</span><span class="sxs-lookup"><span data-stu-id="5a292-159">3, Telenor</span></span>                                              |
| <span data-ttu-id="5a292-160">スイス</span><span class="sxs-lookup"><span data-stu-id="5a292-160">Switzerland</span></span>          | <span data-ttu-id="5a292-161">Swisscom</span><span class="sxs-lookup"><span data-stu-id="5a292-161">Sunrise, Swisscom</span></span>                                       |
| <span data-ttu-id="5a292-162">台湾</span><span class="sxs-lookup"><span data-stu-id="5a292-162">Taiwan</span></span>               | <span data-ttu-id="5a292-163">FarEasTone</span><span class="sxs-lookup"><span data-stu-id="5a292-163">FarEasTone</span></span>                                              |
| <span data-ttu-id="5a292-164">トルコ</span><span class="sxs-lookup"><span data-stu-id="5a292-164">Turkey</span></span>               | <span data-ttu-id="5a292-165">Turkcell</span><span class="sxs-lookup"><span data-stu-id="5a292-165">Turkcell</span></span>                                                |
| <span data-ttu-id="5a292-166">アラブ首長国連邦</span><span class="sxs-lookup"><span data-stu-id="5a292-166">United Arab Emirates</span></span> | <span data-ttu-id="5a292-167">Etisalat</span><span class="sxs-lookup"><span data-stu-id="5a292-167">Etisalat</span></span>                                                |
| <span data-ttu-id="5a292-168">アメリカ合衆国</span><span class="sxs-lookup"><span data-stu-id="5a292-168">United States</span></span>        | <span data-ttu-id="5a292-169">Sprint、Verizon</span><span class="sxs-lookup"><span data-stu-id="5a292-169">Sprint, Verizon</span></span>                                         |
| <span data-ttu-id="5a292-170">イギリス</span><span class="sxs-lookup"><span data-stu-id="5a292-170">United Kingdom</span></span>       | <span data-ttu-id="5a292-171">3英国、EE、O2、Vodafone</span><span class="sxs-lookup"><span data-stu-id="5a292-171">3 UK, EE, O2, Vodafone</span></span>                                 |
