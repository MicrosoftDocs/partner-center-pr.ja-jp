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
ms.openlocfilehash: 20ce286814682277e375894e99f947d084206246
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172389"
---
# <a name="mobile-operator-billing"></a><span data-ttu-id="45710-104">携帯電話会社による課金</span><span class="sxs-lookup"><span data-stu-id="45710-104">Mobile operator billing</span></span>

<span data-ttu-id="45710-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="45710-105">**Appropriate roles**</span></span>

- <span data-ttu-id="45710-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="45710-106">Global admin</span></span>

> [!NOTE]
> <span data-ttu-id="45710-107">支払いに関するサポートが必要な場合 (支払いアカウントの構成、行われていない支払い、支払いの保留など) は、[こちら](https://developer.microsoft.com/windows/support)からサポートにお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="45710-107">If you're looking for support regarding payouts, including configuring payout accounts, missing payouts, putting payouts on hold, or anything else, contact support [here](https://developer.microsoft.com/windows/support).</span></span>

<span data-ttu-id="45710-108">Microsoft Store は、Windows 10 を実行するデバイスの支払い方法としての携帯電話の請求、Windows 10 Mobile を実行する電話、Xbox One のコンソールを提供します。</span><span class="sxs-lookup"><span data-stu-id="45710-108">The Microsoft Store offers mobile operator billing as a payment method for devices running Windows 10, phones running Windows 10 Mobile, and Xbox One consoles.</span></span> <span data-ttu-id="45710-109">お客様の携帯電話事業者がこの機能をサポートしている場合、お客様は、携帯電話の請求を支払い方法として追加し、それを使用して、モバイルアカウントを使用して店舗の購入を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="45710-109">If a customer’s mobile operator supports this capability, the customer can add mobile operator billing as a payment method and use it to make Store purchases using their mobile account.</span></span>

> [!TIP]
> <span data-ttu-id="45710-110">お客様の携帯電話会社が携帯電話の請求を提供していても、お客様のデバイスでこのオプションが見つからない場合は、次の [手順](https://support.microsoft.com/instantanswers/b25d6dd6-fb8b-3710-1e13-4d30eb01b51f)を確認してください。</span><span class="sxs-lookup"><span data-stu-id="45710-110">If a customer’s mobile operator offers mobile operator billing, but the customer can't find this option on their device, review these [steps](https://support.microsoft.com/instantanswers/b25d6dd6-fb8b-3710-1e13-4d30eb01b51f).</span></span>

<span data-ttu-id="45710-111">弊社は、定期的に携帯電話会社と協力して、この支払方法の機能を拡張しています。</span><span class="sxs-lookup"><span data-stu-id="45710-111">We are regularly working with mobile operators to expand the availability of this payment method.</span></span> <span data-ttu-id="45710-112">以下に記載されていない携帯電話会社を提案する場合は、その携帯電話会社に連絡して、この支払い方法を追加するように依頼してください。</span><span class="sxs-lookup"><span data-stu-id="45710-112">If you’d like to suggest a mobile operator that you don’t see listed below, contact that mobile operator and request that they add this payment method.</span></span>

## <a name="operators-that-support-mobile-operator-billing"></a><span data-ttu-id="45710-113">携帯電話会社の課金をサポートするオペレーター</span><span class="sxs-lookup"><span data-stu-id="45710-113">Operators that support mobile operator billing</span></span>

<span data-ttu-id="45710-114">次の携帯電話事業者は、現在、携帯電話の請求をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="45710-114">The following mobile operators currently support mobile operator billing.</span></span>

| <span data-ttu-id="45710-115">国/リージョン</span><span class="sxs-lookup"><span data-stu-id="45710-115">Country/region</span></span>       | <span data-ttu-id="45710-116">携帯電話会社</span><span class="sxs-lookup"><span data-stu-id="45710-116">Mobile operators</span></span>                                        |
|----------------------|---------------------------------------------------------|
| <span data-ttu-id="45710-117">オーストラリア</span><span class="sxs-lookup"><span data-stu-id="45710-117">Australia</span></span>            | <span data-ttu-id="45710-118">Optus</span><span class="sxs-lookup"><span data-stu-id="45710-118">Optus</span></span>                                                   |
| <span data-ttu-id="45710-119">オーストリア</span><span class="sxs-lookup"><span data-stu-id="45710-119">Austria</span></span>              | <span data-ttu-id="45710-120">A1 テレ、Hutchison 3G オーストリア、T-Mobile/テレ</span><span class="sxs-lookup"><span data-stu-id="45710-120">A1 Telekom, Hutchison 3G Austria, T-Mobile / tele.ring</span></span>  |
| <span data-ttu-id="45710-121">ベルギー</span><span class="sxs-lookup"><span data-stu-id="45710-121">Belgium</span></span>              | <span data-ttu-id="45710-122">Base、Proximus</span><span class="sxs-lookup"><span data-stu-id="45710-122">Base, Proximus</span></span>                                          |
| <span data-ttu-id="45710-123">カナダ</span><span class="sxs-lookup"><span data-stu-id="45710-123">Canada</span></span>               | <span data-ttu-id="45710-124">Telus</span><span class="sxs-lookup"><span data-stu-id="45710-124">Telus</span></span>                                                   |
| <span data-ttu-id="45710-125">チェコ</span><span class="sxs-lookup"><span data-stu-id="45710-125">Czechia</span></span>              | <span data-ttu-id="45710-126">T-Mobile、Vodafone、O2</span><span class="sxs-lookup"><span data-stu-id="45710-126">T-Mobile, Vodafone, O2</span></span>                                  |
| <span data-ttu-id="45710-127">デンマーク</span><span class="sxs-lookup"><span data-stu-id="45710-127">Denmark</span></span>              | <span data-ttu-id="45710-128">3、TDC / YouSee、Telenor、Telia</span><span class="sxs-lookup"><span data-stu-id="45710-128">3, TDC / YouSee, Telenor, Telia</span></span>                         |
| <span data-ttu-id="45710-129">フィンランド</span><span class="sxs-lookup"><span data-stu-id="45710-129">Finland</span></span>              | <span data-ttu-id="45710-130">DNA、Elisa</span><span class="sxs-lookup"><span data-stu-id="45710-130">DNA, Elisa</span></span>                                              |
| <span data-ttu-id="45710-131">フランス</span><span class="sxs-lookup"><span data-stu-id="45710-131">France</span></span>               | <span data-ttu-id="45710-132">オレンジ</span><span class="sxs-lookup"><span data-stu-id="45710-132">Orange</span></span>                                                  |
| <span data-ttu-id="45710-133">ドイツ</span><span class="sxs-lookup"><span data-stu-id="45710-133">Germany</span></span>              | <span data-ttu-id="45710-134">O2、テレ (Vodafone)、</span><span class="sxs-lookup"><span data-stu-id="45710-134">O2, Telekom Deutschland, Vodafone</span></span>                       |
| <span data-ttu-id="45710-135">ハンガリー</span><span class="sxs-lookup"><span data-stu-id="45710-135">Hungary</span></span>              | <span data-ttu-id="45710-136">Telenor</span><span class="sxs-lookup"><span data-stu-id="45710-136">Telenor</span></span>                                                 |
| <span data-ttu-id="45710-137">イタリア</span><span class="sxs-lookup"><span data-stu-id="45710-137">Italy</span></span>                | <span data-ttu-id="45710-138">Tre、風力、Vodafone</span><span class="sxs-lookup"><span data-stu-id="45710-138">Tre, Wind, Vodafone</span></span>                                     |
| <span data-ttu-id="45710-139">韓国</span><span class="sxs-lookup"><span data-stu-id="45710-139">Korea</span></span>                | <span data-ttu-id="45710-140">SK Telecom</span><span class="sxs-lookup"><span data-stu-id="45710-140">SK Telecom</span></span>                                              |
| <span data-ttu-id="45710-141">マレーシア</span><span class="sxs-lookup"><span data-stu-id="45710-141">Malaysia</span></span>             | <span data-ttu-id="45710-142">Digi</span><span class="sxs-lookup"><span data-stu-id="45710-142">Digi</span></span>                                                    |
| <span data-ttu-id="45710-143">オランダ</span><span class="sxs-lookup"><span data-stu-id="45710-143">Netherlands</span></span>          | <span data-ttu-id="45710-144">Vodafone n/Telfort、</span><span class="sxs-lookup"><span data-stu-id="45710-144">KPN / Telfort, Vodafone</span></span>                                 |
| <span data-ttu-id="45710-145">ノルウェー</span><span class="sxs-lookup"><span data-stu-id="45710-145">Norway</span></span>               | <span data-ttu-id="45710-146">Telenor/Talkmore、Telia/OneCall</span><span class="sxs-lookup"><span data-stu-id="45710-146">Telenor / Talkmore, Telia / OneCall</span></span>                     |
| <span data-ttu-id="45710-147">ポーランド</span><span class="sxs-lookup"><span data-stu-id="45710-147">Poland</span></span>               | <span data-ttu-id="45710-148">オレンジ色、再生、T-sql</span><span class="sxs-lookup"><span data-stu-id="45710-148">Orange, Play, T-Mobile</span></span>                                  |
| <span data-ttu-id="45710-149">サウジアラビア</span><span class="sxs-lookup"><span data-stu-id="45710-149">Saudi Arabia</span></span>         | <span data-ttu-id="45710-150">STC</span><span class="sxs-lookup"><span data-stu-id="45710-150">STC</span></span>                                                     |
| <span data-ttu-id="45710-151">シンガポール</span><span class="sxs-lookup"><span data-stu-id="45710-151">Singapore</span></span>            | <span data-ttu-id="45710-152">M1 限定、StarHub</span><span class="sxs-lookup"><span data-stu-id="45710-152">M1 Limited, StarHub</span></span>                                     |
| <span data-ttu-id="45710-153">スロバキア</span><span class="sxs-lookup"><span data-stu-id="45710-153">Slovakia</span></span>             | <span data-ttu-id="45710-154">Slovak Telekom</span><span class="sxs-lookup"><span data-stu-id="45710-154">Slovak Telekom</span></span>                                          |
| <span data-ttu-id="45710-155">南アフリカ</span><span class="sxs-lookup"><span data-stu-id="45710-155">South Africa</span></span>         | <span data-ttu-id="45710-156">Vodacom</span><span class="sxs-lookup"><span data-stu-id="45710-156">Vodacom</span></span>                                                 |
| <span data-ttu-id="45710-157">スペイン</span><span class="sxs-lookup"><span data-stu-id="45710-157">Spain</span></span>                | <span data-ttu-id="45710-158">オレンジ</span><span class="sxs-lookup"><span data-stu-id="45710-158">Orange</span></span>                                                  |
| <span data-ttu-id="45710-159">スウェーデン</span><span class="sxs-lookup"><span data-stu-id="45710-159">Sweden</span></span>               | <span data-ttu-id="45710-160">3、telenor</span><span class="sxs-lookup"><span data-stu-id="45710-160">3, Telenor</span></span>                                              |
| <span data-ttu-id="45710-161">スイス</span><span class="sxs-lookup"><span data-stu-id="45710-161">Switzerland</span></span>          | <span data-ttu-id="45710-162">Swisscom</span><span class="sxs-lookup"><span data-stu-id="45710-162">Sunrise, Swisscom</span></span>                                       |
| <span data-ttu-id="45710-163">台湾</span><span class="sxs-lookup"><span data-stu-id="45710-163">Taiwan</span></span>               | <span data-ttu-id="45710-164">FarEasTone</span><span class="sxs-lookup"><span data-stu-id="45710-164">FarEasTone</span></span>                                              |
| <span data-ttu-id="45710-165">トルコ</span><span class="sxs-lookup"><span data-stu-id="45710-165">Turkey</span></span>               | <span data-ttu-id="45710-166">Turkcell</span><span class="sxs-lookup"><span data-stu-id="45710-166">Turkcell</span></span>                                                |
| <span data-ttu-id="45710-167">アラブ首長国連邦</span><span class="sxs-lookup"><span data-stu-id="45710-167">United Arab Emirates</span></span> | <span data-ttu-id="45710-168">Etisalat</span><span class="sxs-lookup"><span data-stu-id="45710-168">Etisalat</span></span>                                                |
| <span data-ttu-id="45710-169">アメリカ合衆国</span><span class="sxs-lookup"><span data-stu-id="45710-169">United States</span></span>        | <span data-ttu-id="45710-170">Sprint、Verizon</span><span class="sxs-lookup"><span data-stu-id="45710-170">Sprint, Verizon</span></span>                                         |
| <span data-ttu-id="45710-171">イギリス</span><span class="sxs-lookup"><span data-stu-id="45710-171">United Kingdom</span></span>       | <span data-ttu-id="45710-172">3英国、EE、O2、Vodafone</span><span class="sxs-lookup"><span data-stu-id="45710-172">3 UK, EE, O2, Vodafone</span></span>                                 |
