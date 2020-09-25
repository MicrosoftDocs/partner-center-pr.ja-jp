---
title: 携帯電話会社の請求-Microsoft Store
description: Microsoft Store は、この機能をサポートするモバイルオペレーターの支払い方法として携帯電話の課金を提供します。
ms.date: 05/29/2020
ms.service: partner-dashboard
ms.topic: article
ms.author: hickeys
author: hickeys
keywords: windows 10, uwp, 携帯電話会社, 携帯電話への課金, 携帯電話会社による課金
ms.localizationpriority: medium
ms.openlocfilehash: 010451506df0d6115a8e1b4781e6fb40ab8853bb
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/25/2020
ms.locfileid: "91335693"
---
# <a name="mobile-operator-billing"></a><span data-ttu-id="7b32d-104">携帯電話会社による課金</span><span class="sxs-lookup"><span data-stu-id="7b32d-104">Mobile operator billing</span></span>

> [!NOTE]
> <span data-ttu-id="7b32d-105">支払いに関するサポートが必要な場合 (支払いアカウントの構成、行われていない支払い、支払いの保留など) は、[こちら](https://developer.microsoft.com/windows/support)からサポートにお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="7b32d-105">If you're looking for support regarding payouts, including configuring payout accounts, missing payouts, putting payouts on hold, or anything else, contact support [here](https://developer.microsoft.com/windows/support).</span></span>

<span data-ttu-id="7b32d-106">Microsoft Store では、Windows 10 を実行するデバイス、Windows 10 Mobile を実行するスマートフォン、Xbox One 本体用の支払い方法として、携帯電話会社による課金を提供しています。</span><span class="sxs-lookup"><span data-stu-id="7b32d-106">The Microsoft Store offers Mobile Operator Billing as a payment method for devices running Windows 10, phones running Windows 10 Mobile, and Xbox One consoles.</span></span> <span data-ttu-id="7b32d-107">ユーザーの携帯電話会社でこの機能がサポートされている場合、ユーザーは支払い方法として携帯電話会社による課金を追加し、この支払い方法を使用してモバイル アカウントによる Microsoft Store での購入を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="7b32d-107">If a customer’s mobile operator supports this capability, the customer can add Mobile Operator Billing as a payment method and use it to make Store purchases using their mobile account.</span></span>

> [!TIP]
>  <span data-ttu-id="7b32d-108">ユーザーの携帯電話会社が携帯電話会社による課金を提供していても、ユーザーのデバイスにこのオプションがない場合は、こちらの[手順](https://support.microsoft.com/instantanswers/b25d6dd6-fb8b-3710-1e13-4d30eb01b51f)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7b32d-108">If a customer’s mobile operator offers Mobile Operator Billing, but the customer can't find this option on their device, review these [steps](https://support.microsoft.com/instantanswers/b25d6dd6-fb8b-3710-1e13-4d30eb01b51f).</span></span>

<span data-ttu-id="7b32d-109">弊社は、定期的に携帯電話会社と協力して、この支払方法の機能を拡張しています。</span><span class="sxs-lookup"><span data-stu-id="7b32d-109">We are regularly working with mobile operators to expand the availability of this payment method.</span></span> <span data-ttu-id="7b32d-110">以下に記載されていない携帯電話会社を提案する場合は、その携帯電話会社に連絡して、この支払い方法を追加するように依頼してください。</span><span class="sxs-lookup"><span data-stu-id="7b32d-110">If you’d like to suggest a mobile operator that you don’t see listed below, contact that mobile operator and request that they add this payment method.</span></span>

<span data-ttu-id="7b32d-111">次の携帯電話事業者は、現在、携帯電話の請求をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="7b32d-111">The following mobile operators currently support Mobile Operator Billing.</span></span>

| <span data-ttu-id="7b32d-112">国/リージョン</span><span class="sxs-lookup"><span data-stu-id="7b32d-112">Country/region</span></span>       | <span data-ttu-id="7b32d-113">携帯電話会社</span><span class="sxs-lookup"><span data-stu-id="7b32d-113">Mobile operators</span></span>                                        |
|----------------------|---------------------------------------------------------|
| <span data-ttu-id="7b32d-114">オーストラリア</span><span class="sxs-lookup"><span data-stu-id="7b32d-114">Australia</span></span>            | <span data-ttu-id="7b32d-115">Optus</span><span class="sxs-lookup"><span data-stu-id="7b32d-115">Optus</span></span>                                                   |
| <span data-ttu-id="7b32d-116">オーストリア</span><span class="sxs-lookup"><span data-stu-id="7b32d-116">Austria</span></span>              | <span data-ttu-id="7b32d-117">A1 テレ、Hutchison 3G オーストリア、T-Mobile/テレ</span><span class="sxs-lookup"><span data-stu-id="7b32d-117">A1 Telekom, Hutchison 3G Austria, T-Mobile / tele.ring</span></span>  |
| <span data-ttu-id="7b32d-118">ベルギー</span><span class="sxs-lookup"><span data-stu-id="7b32d-118">Belgium</span></span>              | <span data-ttu-id="7b32d-119">Base、Proximus</span><span class="sxs-lookup"><span data-stu-id="7b32d-119">Base, Proximus</span></span>                                          |
| <span data-ttu-id="7b32d-120">Canada</span><span class="sxs-lookup"><span data-stu-id="7b32d-120">Canada</span></span>               | <span data-ttu-id="7b32d-121">Telus</span><span class="sxs-lookup"><span data-stu-id="7b32d-121">Telus</span></span>                                                   |
| <span data-ttu-id="7b32d-122">チェコ</span><span class="sxs-lookup"><span data-stu-id="7b32d-122">Czechia</span></span>              | <span data-ttu-id="7b32d-123">T-Mobile</span><span class="sxs-lookup"><span data-stu-id="7b32d-123">T-Mobile</span></span>                                                |
| <span data-ttu-id="7b32d-124">デンマーク</span><span class="sxs-lookup"><span data-stu-id="7b32d-124">Denmark</span></span>              | <span data-ttu-id="7b32d-125">3、TDC / YouSee、Telenor、Telia</span><span class="sxs-lookup"><span data-stu-id="7b32d-125">3, TDC / YouSee, Telenor, Telia</span></span>                         |
| <span data-ttu-id="7b32d-126">フィンランド</span><span class="sxs-lookup"><span data-stu-id="7b32d-126">Finland</span></span>              | <span data-ttu-id="7b32d-127">DNA、Elisa</span><span class="sxs-lookup"><span data-stu-id="7b32d-127">DNA, Elisa</span></span>                                              |
| <span data-ttu-id="7b32d-128">フランス</span><span class="sxs-lookup"><span data-stu-id="7b32d-128">France</span></span>               | <span data-ttu-id="7b32d-129">オレンジ</span><span class="sxs-lookup"><span data-stu-id="7b32d-129">Orange</span></span>                                                  |
| <span data-ttu-id="7b32d-130">ドイツ</span><span class="sxs-lookup"><span data-stu-id="7b32d-130">Germany</span></span>              | <span data-ttu-id="7b32d-131">O2、テレ (Vodafone)、</span><span class="sxs-lookup"><span data-stu-id="7b32d-131">O2, Telekom Deutschland, Vodafone</span></span>                       |
| <span data-ttu-id="7b32d-132">ハンガリー</span><span class="sxs-lookup"><span data-stu-id="7b32d-132">Hungary</span></span>              | <span data-ttu-id="7b32d-133">Telenor</span><span class="sxs-lookup"><span data-stu-id="7b32d-133">Telenor</span></span>                                                 |
| <span data-ttu-id="7b32d-134">イタリア</span><span class="sxs-lookup"><span data-stu-id="7b32d-134">Italy</span></span>                | <span data-ttu-id="7b32d-135">Tre、風力</span><span class="sxs-lookup"><span data-stu-id="7b32d-135">Tre, Wind</span></span>                                               |
| <span data-ttu-id="7b32d-136">マレーシア</span><span class="sxs-lookup"><span data-stu-id="7b32d-136">Malaysia</span></span>             | <span data-ttu-id="7b32d-137">Digi</span><span class="sxs-lookup"><span data-stu-id="7b32d-137">Digi</span></span>                                                    |
| <span data-ttu-id="7b32d-138">オランダ</span><span class="sxs-lookup"><span data-stu-id="7b32d-138">Netherlands</span></span>          | <span data-ttu-id="7b32d-139">/Telfort</span><span class="sxs-lookup"><span data-stu-id="7b32d-139">KPN / Telfort</span></span>                                           |
| <span data-ttu-id="7b32d-140">ノルウェー</span><span class="sxs-lookup"><span data-stu-id="7b32d-140">Norway</span></span>               | <span data-ttu-id="7b32d-141">Telenor/Talkmore、Telia/OneCall</span><span class="sxs-lookup"><span data-stu-id="7b32d-141">Telenor / Talkmore, Telia / OneCall</span></span>                     |
| <span data-ttu-id="7b32d-142">ポーランド</span><span class="sxs-lookup"><span data-stu-id="7b32d-142">Poland</span></span>               | <span data-ttu-id="7b32d-143">オレンジ、再生</span><span class="sxs-lookup"><span data-stu-id="7b32d-143">Orange, Play</span></span>                                            |
| <span data-ttu-id="7b32d-144">シンガポール</span><span class="sxs-lookup"><span data-stu-id="7b32d-144">Singapore</span></span>            | <span data-ttu-id="7b32d-145">M1 限定、StarHub</span><span class="sxs-lookup"><span data-stu-id="7b32d-145">M1 Limited, StarHub</span></span>                                     |
| <span data-ttu-id="7b32d-146">スロバキア</span><span class="sxs-lookup"><span data-stu-id="7b32d-146">Slovakia</span></span>             | <span data-ttu-id="7b32d-147">Slovak Telekom</span><span class="sxs-lookup"><span data-stu-id="7b32d-147">Slovak Telekom</span></span>                                          |
| <span data-ttu-id="7b32d-148">南アフリカ</span><span class="sxs-lookup"><span data-stu-id="7b32d-148">South Africa</span></span>         | <span data-ttu-id="7b32d-149">Vodacom</span><span class="sxs-lookup"><span data-stu-id="7b32d-149">Vodacom</span></span>                                                 |
| <span data-ttu-id="7b32d-150">スペイン</span><span class="sxs-lookup"><span data-stu-id="7b32d-150">Spain</span></span>                | <span data-ttu-id="7b32d-151">オレンジ</span><span class="sxs-lookup"><span data-stu-id="7b32d-151">Orange</span></span>                                                  |
| <span data-ttu-id="7b32d-152">スウェーデン</span><span class="sxs-lookup"><span data-stu-id="7b32d-152">Sweden</span></span>               | <span data-ttu-id="7b32d-153">3、telenor</span><span class="sxs-lookup"><span data-stu-id="7b32d-153">3, Telenor</span></span>                                              |
| <span data-ttu-id="7b32d-154">スイス</span><span class="sxs-lookup"><span data-stu-id="7b32d-154">Switzerland</span></span>          | <span data-ttu-id="7b32d-155">Swisscom</span><span class="sxs-lookup"><span data-stu-id="7b32d-155">Sunrise, Swisscom</span></span>                                       |
| <span data-ttu-id="7b32d-156">台湾</span><span class="sxs-lookup"><span data-stu-id="7b32d-156">Taiwan</span></span>               | <span data-ttu-id="7b32d-157">FarEasTone</span><span class="sxs-lookup"><span data-stu-id="7b32d-157">FarEasTone</span></span>                                              |
| <span data-ttu-id="7b32d-158">トルコ</span><span class="sxs-lookup"><span data-stu-id="7b32d-158">Turkey</span></span>               | <span data-ttu-id="7b32d-159">Turkcell</span><span class="sxs-lookup"><span data-stu-id="7b32d-159">Turkcell</span></span>                                                |
| <span data-ttu-id="7b32d-160">アラブ首長国連邦</span><span class="sxs-lookup"><span data-stu-id="7b32d-160">United Arab Emirates</span></span> | <span data-ttu-id="7b32d-161">Etisalat</span><span class="sxs-lookup"><span data-stu-id="7b32d-161">Etisalat</span></span>                                                |
| <span data-ttu-id="7b32d-162">United States</span><span class="sxs-lookup"><span data-stu-id="7b32d-162">United States</span></span>        | <span data-ttu-id="7b32d-163">Sprint、Verizon</span><span class="sxs-lookup"><span data-stu-id="7b32d-163">Sprint, Verizon</span></span>                                         |
| <span data-ttu-id="7b32d-164">イギリス</span><span class="sxs-lookup"><span data-stu-id="7b32d-164">United Kingdom</span></span>       | <span data-ttu-id="7b32d-165">3英国、EE、O2、Vodaphone</span><span class="sxs-lookup"><span data-stu-id="7b32d-165">3 UK, EE, O2, Vodaphone</span></span>                                 |
