---
title: 2021 年 3 月のお知らせ
description: 2021 年 3 月の Microsoft パートナー センターのお知らせでは、新しい機能、販売促進、オファー、市場、既存のオファーに対する変更を紹介します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 3d91eb26f98005b92a48c6f242ea4439e42cde05
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702877"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="b75bf-103">2021 年 3 月のお知らせ</span><span class="sxs-lookup"><span data-stu-id="b75bf-103">March 2021 announcements</span></span>

<span data-ttu-id="b75bf-104">このページでは、2021 年 3 月の Microsoft パートナー センターのお知らせについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a><span data-ttu-id="b75bf-105">準備状況: クラウド ソリューション プロバイダー (CSP) 顧客アドレス検証 API に対する変更が 6 月に運用開始、現在テスト機能が利用可能</span><span class="sxs-lookup"><span data-stu-id="b75bf-105">Readiness: Changes to the Cloud Solution Provider (CSP) customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-106">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-106">Categories</span></span>

- <span data-ttu-id="b75bf-107">日付: 2021 年 3 月 30 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-107">Date: 2021-03-30</span></span>
- <span data-ttu-id="b75bf-108">準備</span><span class="sxs-lookup"><span data-stu-id="b75bf-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="b75bf-109">まとめ</span><span class="sxs-lookup"><span data-stu-id="b75bf-109">Summary</span></span>

<span data-ttu-id="b75bf-110">パートナーと顧客が信頼に基づいてビジネスを遂行できるようにするために、Microsoft はパートナーに対して世界中のすべての国の Validate Address API に対する変更をテストすることをお勧めしています。</span><span class="sxs-lookup"><span data-stu-id="b75bf-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-111">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-111">Impacted audience</span></span>

<span data-ttu-id="b75bf-112">顧客の住所の詳細を新規作成または既存のものを更新する、CSP 直接請求パートナーと間接プロバイダー。</span><span class="sxs-lookup"><span data-stu-id="b75bf-112">CSP direct bill partners and indirect providers who create new or update existing customers address details.</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-113">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-113">Details</span></span>

<span data-ttu-id="b75bf-114">Microsoft の基盤は信頼です。</span><span class="sxs-lookup"><span data-stu-id="b75bf-114">Microsoft runs on trust.</span></span> <span data-ttu-id="b75bf-115">Microsoft は、CSP プログラムで顧客サブスクリプションを処理するために、法令に準拠した安全な顧客住所の検証方法の提供に努めています。</span><span class="sxs-lookup"><span data-stu-id="b75bf-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="b75bf-116">2021 年 3 月 31 日の時点で、Validate Address API への変更が発表されています。2021 年 6 月にその変更を含む運用が開始される前にパートナーに対してこれをテストすることをお勧めしていました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-116">As of March 31, 2021, we’ve introduced changes to the Validate Address API that we invited partners to test, prior to going live with the changes in June 2021.</span></span>

<span data-ttu-id="b75bf-117">変更は、Validate Address API にのみ影響します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-117">Changes affect the Validate Address API only.</span></span> <span data-ttu-id="b75bf-118">Create Customer と Update Billing Profile の API には影響がありません。</span><span class="sxs-lookup"><span data-stu-id="b75bf-118">Create Customer and Update Billing Profile APIs aren’t impacted.</span></span>

<span data-ttu-id="b75bf-119">応答では、次のいずれかのステータス メッセージが返されます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="b75bf-120">状態</span><span class="sxs-lookup"><span data-stu-id="b75bf-120">Status</span></span>     | <span data-ttu-id="b75bf-121">説明</span><span class="sxs-lookup"><span data-stu-id="b75bf-121">Description</span></span> |    <span data-ttu-id="b75bf-122">返される住所候補の数</span><span class="sxs-lookup"><span data-stu-id="b75bf-122">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="b75bf-123">Verified shippable (検証済み出荷可能)</span><span class="sxs-lookup"><span data-stu-id="b75bf-123">Verified shippable</span></span> | <span data-ttu-id="b75bf-124">住所が確認され、出荷可能です。</span><span class="sxs-lookup"><span data-stu-id="b75bf-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="b75bf-125">Single</span><span class="sxs-lookup"><span data-stu-id="b75bf-125">Single</span></span> |
|<span data-ttu-id="b75bf-126">Verified</span><span class="sxs-lookup"><span data-stu-id="b75bf-126">Verified</span></span> | <span data-ttu-id="b75bf-127">住所が確認されました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-127">Address is verified.</span></span> | <span data-ttu-id="b75bf-128">Single</span><span class="sxs-lookup"><span data-stu-id="b75bf-128">Single</span></span> |
|<span data-ttu-id="b75bf-129">Interaction required (対話式操作が必要)</span><span class="sxs-lookup"><span data-stu-id="b75bf-129">Interaction required</span></span> | <span data-ttu-id="b75bf-130">提案された住所は大幅に変更されており、ユーザーの確認が必要です。</span><span class="sxs-lookup"><span data-stu-id="b75bf-130">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="b75bf-131">Single</span><span class="sxs-lookup"><span data-stu-id="b75bf-131">Single</span></span> |
|<span data-ttu-id="b75bf-132">Street partial (番地が不完全)</span><span class="sxs-lookup"><span data-stu-id="b75bf-132">Street partial</span></span> | <span data-ttu-id="b75bf-133">住所の番地が部分的であるため、さらに情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="b75bf-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="b75bf-134">複数 (最大 3)</span><span class="sxs-lookup"><span data-stu-id="b75bf-134">Multiple—maximum of three</span></span> |
|<span data-ttu-id="b75bf-135">Premises partial (建物が不完全)</span><span class="sxs-lookup"><span data-stu-id="b75bf-135">Premises partial</span></span> | <span data-ttu-id="b75bf-136">指定された建物 (ビル番号、部屋番号、その他) が不完全であるため、さらに情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="b75bf-136">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="b75bf-137">複数 (最大 3)</span><span class="sxs-lookup"><span data-stu-id="b75bf-137">Multiple—maximum of three</span></span> |
|<span data-ttu-id="b75bf-138">複数</span><span class="sxs-lookup"><span data-stu-id="b75bf-138">Multiple</span></span> | <span data-ttu-id="b75bf-139">住所の複数のフィールドが不完全です (street partial と premises partial も含む可能性があります)。</span><span class="sxs-lookup"><span data-stu-id="b75bf-139">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="b75bf-140">複数 (最大 3)</span><span class="sxs-lookup"><span data-stu-id="b75bf-140">Multiple—maximum of three</span></span> |
|<span data-ttu-id="b75bf-141">なし</span><span class="sxs-lookup"><span data-stu-id="b75bf-141">None</span></span> | <span data-ttu-id="b75bf-142">住所が正しくありません。</span><span class="sxs-lookup"><span data-stu-id="b75bf-142">Address is incorrect.</span></span> | <span data-ttu-id="b75bf-143">なし</span><span class="sxs-lookup"><span data-stu-id="b75bf-143">None</span></span> |
|<span data-ttu-id="b75bf-144">検証なし</span><span class="sxs-lookup"><span data-stu-id="b75bf-144">Not validated</span></span> | <span data-ttu-id="b75bf-145">住所は、検証プロセスを通じて送信できませんでした。</span><span class="sxs-lookup"><span data-stu-id="b75bf-145">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="b75bf-146">なし</span><span class="sxs-lookup"><span data-stu-id="b75bf-146">None</span></span> |

<span data-ttu-id="b75bf-147">米国の郵便番号は、ハイフン付きでさらに 4 桁が返されます (例: 12345-6789)。</span><span class="sxs-lookup"><span data-stu-id="b75bf-147">US post codes will return an additional 4 digits + hyphen - for example, 12345-6789.</span></span>

<span data-ttu-id="b75bf-148">住所が Validate Address API 経由で検証のために送信されると、次の応答スキーマが返されます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-148">Once an address is submitted for validation via the Validate Address API, the following response schema will be returned:</span></span>

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

<span data-ttu-id="b75bf-149">サンプルの応答をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-149">Take a look at this sample response.</span></span> <span data-ttu-id="b75bf-150">米国では、郵便番号に 5 桁の数字のみを入力した場合、応答では郵便番号の行に追加の 4 桁のサフィックスが返されることに注目してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-150">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp

"suggested_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Microsoft Way",
              "postal_Code": "98052-8300"
},
"original_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Micro Way",
              "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a><span data-ttu-id="b75bf-151">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b75bf-151">Next steps</span></span>

- <span data-ttu-id="b75bf-152">テスト フライトに含められるようにサンドボックスのテナント ID を領域の専門家 (Ali Khaki) に知らせます。これにより、更新の準備を開始できます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-152">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="b75bf-153">コントロール パネル ベンダー (CPV) ソリューションを使用している場合は、CPV とご相談ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-153">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="b75bf-154">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="b75bf-154">Questions?</span></span>

<span data-ttu-id="b75bf-155">Microsoft との連携でサポートが必要な場合は、パートナー サポートの Yammer グループにお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-155">If you need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

### <a name="change-log"></a><span data-ttu-id="b75bf-156">変更ログ:</span><span class="sxs-lookup"><span data-stu-id="b75bf-156">Change log:</span></span>

- <span data-ttu-id="b75bf-157">2020 年 3 月 31 日: 初版の発行</span><span class="sxs-lookup"><span data-stu-id="b75bf-157">March 31, 2020: Original publication</span></span>

- <span data-ttu-id="b75bf-158">2021 年 4 月 30 日: サンプルの応答と郵便番号の詳細について更新</span><span class="sxs-lookup"><span data-stu-id="b75bf-158">April 30, 2021: Updates for sample response and Zip code details</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="b75bf-159">新しい Exchange 管理センター (EAC) エクスペリエンス</span><span class="sxs-lookup"><span data-stu-id="b75bf-159">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-160">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-160">Categories</span></span>

- <span data-ttu-id="b75bf-161">日付: 2021 年 3 月 29 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-161">Date: 2021-03-29</span></span>
- <span data-ttu-id="b75bf-162">機能</span><span class="sxs-lookup"><span data-stu-id="b75bf-162">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="b75bf-163">まとめ</span><span class="sxs-lookup"><span data-stu-id="b75bf-163">Summary</span></span>

<span data-ttu-id="b75bf-164">2021 年 4 月 27 日以降、Exchange 管理センター (EAC) では、ユーザーの日々の効率を向上させる新しいエクスペリエンスがロールアウトされます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-164">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-165">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-165">Impacted audience</span></span>

<span data-ttu-id="b75bf-166">パートナー センター経由で Exchange にアクセスする代理管理者</span><span class="sxs-lookup"><span data-stu-id="b75bf-166">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-167">説明</span><span class="sxs-lookup"><span data-stu-id="b75bf-167">Details</span></span>

<span data-ttu-id="b75bf-168">2021 年 4 月 27 日以降、パートナー センターを通じて Exchange に移動するパートナーは、新しい EAC にリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-168">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="b75bf-169">この新しいエクスペリエンスは現在、プレビューとして提供されており、管理者は従来の EAC で右上隅にあるトグルを選択すれば、このエクスペリエンスをアクティブにできます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-169">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="b75bf-170">また、すべてのページに表示される [今すぐ試す] バナーを選択して、新しい EAC に移動することもできます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-170">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="b75bf-171">新しい EAC には次のような利点があります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-171">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="b75bf-172">メール フロー関連の問題について、分析情報、レポート、アラートのメカニズムが追加されました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-172">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="b75bf-173">ダッシュボードをカスタマイズして、生産性を向上させることができます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-173">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="b75bf-174">新しいエクスペリエンスを簡単に確認するには、新しい EAC エクスペリエンスの「**トレーニングとガイド**」セクションでビデオを参照できます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-174">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="b75bf-175">新しいポータルを最適に使用する方法の概要について理解できます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-175">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="b75bf-176">この変更により、従来の EAC エクスペリエンスが非推奨になることはありません。</span><span class="sxs-lookup"><span data-stu-id="b75bf-176">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="b75bf-177">パートナーには、変更の実施に先立ち、十分前もって通知されます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-177">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="b75bf-178">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b75bf-178">Next steps</span></span>

- <span data-ttu-id="b75bf-179">[このトピックに関するリソース](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)を参照して、新しいエクスペリエンスのスクリーンショットを確認することができます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-179">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="b75bf-180">この情報を組織内の適切な関係者に共有してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-180">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="b75bf-181">疑問がある場合</span><span class="sxs-lookup"><span data-stu-id="b75bf-181">Questions?</span></span>

<span data-ttu-id="b75bf-182">これらの変更についてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-182">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="b75bf-183">Microsoft Operations: 製品発表予定表の概要</span><span class="sxs-lookup"><span data-stu-id="b75bf-183">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-184">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-184">Categories</span></span>

- <span data-ttu-id="b75bf-185">日付: 2021 年 3 月 25 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-185">Date: 2021-03-25</span></span>
- <span data-ttu-id="b75bf-186">製品サービス | モダン ワークプレース</span><span class="sxs-lookup"><span data-stu-id="b75bf-186">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="b75bf-187">まとめ</span><span class="sxs-lookup"><span data-stu-id="b75bf-187">Summary</span></span>

<span data-ttu-id="b75bf-188">パートナーからのフィードバックにお応えして、Microsoft Operations では製品発表に関するコミュニケーションを合理化します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-188">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-189">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-189">Impacted audience</span></span>

<span data-ttu-id="b75bf-190">クラウド ソリューション プロバイダー (CSP) パートナー様</span><span class="sxs-lookup"><span data-stu-id="b75bf-190">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-191">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-191">Details</span></span>

<span data-ttu-id="b75bf-192">Microsoft では、パートナー エクスペリエンスの継続的な改善に取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-192">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="b75bf-193">Microsoft からの情報が多すぎるというフィードバックが寄せられています。これには、製品の発表に関する重複したお知らせも含まれます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-193">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="b75bf-194">Microsoft では、皆様からのフィードバックにお応えして、新規および既存のオファーについて製品発表の準備エクスペリエンスを合理化しました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-194">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="b75bf-195">現在では、月に 1 回の製品発表ビューを Operations Readiness リソース ギャラリーに提供するようになりました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-195">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="b75bf-196">この月単位の[製品発表予定表ビュー](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)は、Operations Readiness リソース ギャラリーとパートナー センターのお知らせに含まれる個別の製品発表情報に置き換わるものとなります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-196">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="b75bf-197">また、[コミュニティ コレクション](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)、[予定表ビュー](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)、[CSP ニュースレター](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)から、この[製品発表予定表](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)にアクセスすることもできます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-197">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="b75bf-198">各月の製品発表予定表が公開されたら、Operations Readiness リソース ギャラリーのお知らせで皆様に通知します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-198">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="b75bf-199">新規および既存のオファーに関する情報は、今後も、価格一覧のプレビューと価格一覧の変更ログ、製品のブログ、ライセンス ガイド、製品マーケティング ページで確認できます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-199">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="b75bf-200">この変更は、次の製品に関する発表に適用されます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-200">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="b75bf-201">オンプレミスの Dynamics</span><span class="sxs-lookup"><span data-stu-id="b75bf-201">Dynamics on-premises</span></span>
- <span data-ttu-id="b75bf-202">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b75bf-202">Microsoft 365</span></span>
- <span data-ttu-id="b75bf-203">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="b75bf-203">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="b75bf-204">Windows</span><span class="sxs-lookup"><span data-stu-id="b75bf-204">Windows</span></span>
- <span data-ttu-id="b75bf-205">サーバー</span><span class="sxs-lookup"><span data-stu-id="b75bf-205">Server</span></span>  
- <span data-ttu-id="b75bf-206">ツール</span><span class="sxs-lookup"><span data-stu-id="b75bf-206">Tools</span></span>
- <span data-ttu-id="b75bf-207">Teams と Telco</span><span class="sxs-lookup"><span data-stu-id="b75bf-207">Teams and Telco</span></span>

<span data-ttu-id="b75bf-208">Operations Readiness の詳細を必要とする製品の発表については、引き続き特定のお知らせをお送りします。</span><span class="sxs-lookup"><span data-stu-id="b75bf-208">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="b75bf-209">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b75bf-209">Next steps</span></span>

<span data-ttu-id="b75bf-210">このトピックに関するリソースを確認し、この情報を組織内の該当する関係者と共有してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-210">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="b75bf-211">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="b75bf-211">Questions?</span></span>

<span data-ttu-id="b75bf-212">これらのオファーについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-212">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="b75bf-213">CSP のお客様のオンボード要件の変更</span><span class="sxs-lookup"><span data-stu-id="b75bf-213">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-214">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-214">Categories</span></span>

- <span data-ttu-id="b75bf-215">日付: 2021 年 3 月 25 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-215">Date: 2021-03-25</span></span>
- <span data-ttu-id="b75bf-216">機能</span><span class="sxs-lookup"><span data-stu-id="b75bf-216">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="b75bf-217">まとめ</span><span class="sxs-lookup"><span data-stu-id="b75bf-217">Summary</span></span>

<span data-ttu-id="b75bf-218">パートナーと顧客が信頼に基づいて取引できるように支援する責任の一環として、Microsoft では 2021 年 3 月 25 日から、追加の顧客情報を要求いたします。</span><span class="sxs-lookup"><span data-stu-id="b75bf-218">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-219">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-219">Impacted audience</span></span>

<span data-ttu-id="b75bf-220">次のセクションに記載されている国に新規または既存の顧客がいるクラウド ソリューション プロバイダー (CSP) 直接請求パートナーおよび間接プロバイダー</span><span class="sxs-lookup"><span data-stu-id="b75bf-220">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-221">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-221">Details</span></span>

<span data-ttu-id="b75bf-222">Microsoft の基盤は信頼です。</span><span class="sxs-lookup"><span data-stu-id="b75bf-222">Microsoft runs on trust.</span></span> <span data-ttu-id="b75bf-223">Microsoft は、CSP プログラムでの顧客サブスクリプションの取引について、顧客検証のための法令に準拠した安全な手段の提供に努めています。</span><span class="sxs-lookup"><span data-stu-id="b75bf-223">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="b75bf-224">2021 年 3 月 25 日に、パートナー センター API とユーザー インターフェイス (UI) の拡張機能を導入する予定です。これは、以下の条件の両方を満たすパートナーに影響します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-224">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="b75bf-225">Microsoft の間に直接請求関係があるパートナー (つまり、直接請求パートナーまたは間接プロバイダーのいずれかであるパートナー)</span><span class="sxs-lookup"><span data-stu-id="b75bf-225">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="b75bf-226">パートナーは、次の国の新規または既存の顧客と取引があります:</span><span class="sxs-lookup"><span data-stu-id="b75bf-226">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="b75bf-227">タイ</span><span class="sxs-lookup"><span data-stu-id="b75bf-227">Thailand</span></span>
    - <span data-ttu-id="b75bf-228">ベトナム</span><span class="sxs-lookup"><span data-stu-id="b75bf-228">Vietnam</span></span>
    - <span data-ttu-id="b75bf-229">トルコ</span><span class="sxs-lookup"><span data-stu-id="b75bf-229">Turkey</span></span>
    - <span data-ttu-id="b75bf-230">ポーランド</span><span class="sxs-lookup"><span data-stu-id="b75bf-230">Poland</span></span>
    - <span data-ttu-id="b75bf-231">南アフリカ</span><span class="sxs-lookup"><span data-stu-id="b75bf-231">South Africa</span></span>
    - <span data-ttu-id="b75bf-232">インド</span><span class="sxs-lookup"><span data-stu-id="b75bf-232">India</span></span>
    - <span data-ttu-id="b75bf-233">ブラジル</span><span class="sxs-lookup"><span data-stu-id="b75bf-233">Brazil</span></span>
    - <span data-ttu-id="b75bf-234">イラク</span><span class="sxs-lookup"><span data-stu-id="b75bf-234">Iraq</span></span>
    - <span data-ttu-id="b75bf-235">ミャンマー</span><span class="sxs-lookup"><span data-stu-id="b75bf-235">Myanmar</span></span>
    - <span data-ttu-id="b75bf-236">南スーダン</span><span class="sxs-lookup"><span data-stu-id="b75bf-236">South Sudan</span></span>
    - <span data-ttu-id="b75bf-237">サウジアラビア</span><span class="sxs-lookup"><span data-stu-id="b75bf-237">Saudi Arabia</span></span>
    - <span data-ttu-id="b75bf-238">アラブ首長国連邦</span><span class="sxs-lookup"><span data-stu-id="b75bf-238">United Arab Emirates</span></span>
    - <span data-ttu-id="b75bf-239">ベネズエラ</span><span class="sxs-lookup"><span data-stu-id="b75bf-239">Venezuela</span></span>

<span data-ttu-id="b75bf-240">条件を満たすパートナーは、新しい顧客をオンボードするとき、または既存の顧客の詳細を変更するときに、顧客の **会社登録 ID** (顧客の **組織 INN** とも呼ばれます) と **電話番号** を提出する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-240">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="b75bf-241">また、これらのパートナーは、必要に応じて、顧客の **ミドル ネーム** を入力することができます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-241">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="b75bf-242">会社登録 ID を追加する場合は、顧客の個人 ID ではなく、業務用の税 ID を使用する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-242">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="b75bf-243">以下の国で新規または既存の顧客との取引を行っているパートナーは、先行する 2020 年 11 月のリリースで既にオンボードされています。</span><span class="sxs-lookup"><span data-stu-id="b75bf-243">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="b75bf-244">アルメニア</span><span class="sxs-lookup"><span data-stu-id="b75bf-244">Armenia</span></span>
- <span data-ttu-id="b75bf-245">アゼルバイジャン</span><span class="sxs-lookup"><span data-stu-id="b75bf-245">Azerbaijan</span></span>
- <span data-ttu-id="b75bf-246">ベラルーシ</span><span class="sxs-lookup"><span data-stu-id="b75bf-246">Belarus</span></span>
- <span data-ttu-id="b75bf-247">ハンガリー</span><span class="sxs-lookup"><span data-stu-id="b75bf-247">Hungary</span></span>
- <span data-ttu-id="b75bf-248">カザフスタン</span><span class="sxs-lookup"><span data-stu-id="b75bf-248">Kazakhstan</span></span>
- <span data-ttu-id="b75bf-249">キルギスタン</span><span class="sxs-lookup"><span data-stu-id="b75bf-249">Kyrgyzstan</span></span>
- <span data-ttu-id="b75bf-250">モルドバ</span><span class="sxs-lookup"><span data-stu-id="b75bf-250">Moldova</span></span>
- <span data-ttu-id="b75bf-251">ロシア</span><span class="sxs-lookup"><span data-stu-id="b75bf-251">Russia</span></span>
- <span data-ttu-id="b75bf-252">タジキスタン</span><span class="sxs-lookup"><span data-stu-id="b75bf-252">Tajikistan</span></span>
- <span data-ttu-id="b75bf-253">ウクライナ</span><span class="sxs-lookup"><span data-stu-id="b75bf-253">Ukraine</span></span>
- <span data-ttu-id="b75bf-254">ウズベキスタン</span><span class="sxs-lookup"><span data-stu-id="b75bf-254">Uzbekistan</span></span>

<span data-ttu-id="b75bf-255">その他の地域の顧客と提携しているパートナーは、2021 年 3 月 25 日に、顧客の **会社登録 ID**、**電話番号**、**ミドル ネーム** を詳細情報として必要に応じて入力できるようになります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-255">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="b75bf-256">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b75bf-256">Next steps</span></span>

- <span data-ttu-id="b75bf-257">詳細なガイダンスについては、[専用のパートナー コレクション](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)でテクニカル ドキュメントとよく寄せられる質問を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-257">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="b75bf-258">Partner Center API と Web ユーザー エクスペリエンスを使用して、変更を組み込む準備をしてください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-258">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="b75bf-259">API または SDK はテストに使用できます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-259">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="b75bf-260">新しい顧客をオンボードする場合や、既存の顧客の詳細情報を変更する場合は、必ず追加データを提出してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-260">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="b75bf-261">コントロール パネル ベンダー (CPV) ソリューションを使用している場合は、CPV とご相談ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-261">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="b75bf-262">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="b75bf-262">Questions?</span></span>

<span data-ttu-id="b75bf-263">有効な識別子 (INN または TIN とも呼ばれます) に関するご質問がある場合は、税務顧問または現地の税務署にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-263">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="b75bf-264">Microsoft では、税務に関するガイダンスを提供できません。</span><span class="sxs-lookup"><span data-stu-id="b75bf-264">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="b75bf-265">Microsoft との連携でサポートが必要な場合は、[サービス要求を開いてください](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)。</span><span class="sxs-lookup"><span data-stu-id="b75bf-265">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="b75bf-266">2021 年 3 月 1 日に永続的ソフトウェアの価格表に加えられた修正</span><span class="sxs-lookup"><span data-stu-id="b75bf-266">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-267">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-267">Categories</span></span>

- <span data-ttu-id="b75bf-268">日付: 2021 年 3 月 23 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-268">Date: 2021-03-23</span></span>
- <span data-ttu-id="b75bf-269">製品サービス/市場</span><span class="sxs-lookup"><span data-stu-id="b75bf-269">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-270">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-270">Impacted audience</span></span>

<span data-ttu-id="b75bf-271">クラウド ソリューション プロバイダー プログラムで永続的なソフトウェアの取引を行っている間接プロバイダーおよび直接請求パートナー</span><span class="sxs-lookup"><span data-stu-id="b75bf-271">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="b75bf-272">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-272">Details</span></span>

<span data-ttu-id="b75bf-273">2021 年 3 月 1 日に公開された永続的ソフトウェアの価格表には、掲載されるべきではなかった市場が含まれていました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-273">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="b75bf-274">修正内容を含めた永続的ソフトウェアの価格表が、2021 年 3 月 17 日に更新されました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-274">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="b75bf-275">これらの修正は、次の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-275">These corrections were only applicable to:</span></span>

- <span data-ttu-id="b75bf-276">製品 ID: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="b75bf-276">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="b75bf-277">製品名: Microsoft 365 Business の Windows 10 Home から Pro へのアップグレード</span><span class="sxs-lookup"><span data-stu-id="b75bf-277">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="b75bf-278">削除された、またはサポートされていない市場: AE、AF、AL、AM、AO、BA、BB、BD、BH、BM、BN、BO、BR、BS、BW、BY、BZ、CI、CL、CM、CO、CR、CW、DO、DZ、EC、EG、ET、FJ、FO、GE、GH、GT、HN、IL、IN、IQ、JM、JO、KE、KG、KN、KW、KY、KZ、LB、LK、LY、MA、MC、MD、ME、MN、MO、MU、NA、NG、NI、NP、OM、PA、PE、PH、PK、PR、PY、QA、RS、RU、RW、SG、SN、SV、TH、TJ、TM、TN、TT、TZ、UA、UG、UY、UZ、VE、VN、YE、ZM、ZW</span><span class="sxs-lookup"><span data-stu-id="b75bf-278">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="b75bf-279">これらの変更は、上記の製品にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-279">These changes only apply to the above product.</span></span> <span data-ttu-id="b75bf-280">他の製品には修正がありませんでした。</span><span class="sxs-lookup"><span data-stu-id="b75bf-280">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="b75bf-281">次の手順とリソース</span><span class="sxs-lookup"><span data-stu-id="b75bf-281">Next steps and resources</span></span>

- <span data-ttu-id="b75bf-282">永続的ソフトウェアの取引を行うパートナーは、最新の永続的ソフトウェアの価格表をダウンロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-282">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="b75bf-283">国を指す 2 文字の省略形のわかりやすいマッピングについては、[地域と国のコード](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-283">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><span data-ttu-id="b75bf-284"><a name="13">.NET Standard (v1.17.0) の SDK リリース</a></span><span class="sxs-lookup"><span data-stu-id="b75bf-284"><a name="13"></a> SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-285">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-285">Categories</span></span>

- <span data-ttu-id="b75bf-286">日付: 2021 年 3 月 23 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-286">Date: 2021-03-23</span></span>

- <span data-ttu-id="b75bf-287">機能</span><span class="sxs-lookup"><span data-stu-id="b75bf-287">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="b75bf-288">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-288">Impacted audience</span></span>

<span data-ttu-id="b75bf-289">パートナー センターの .NET SDK を使用している、CSP プログラムに参加している直接請求パートナーと間接プロバイダー。</span><span class="sxs-lookup"><span data-stu-id="b75bf-289">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-290">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-290">Details</span></span>

<span data-ttu-id="b75bf-291">2020 年 3 月 23 日より、パートナーは、更新されたパートナー センター SDK [GitHub の一般向けサンプル](https://github.com/Microsoft/Partner-Center-DotNet-Samples)と共に、[MicrosoftPartnerCenter.NETSDK (NuGet ギャラリー | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0) バージョンのダウンロードを開始できます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-291">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="b75bf-292">このバージョンには、以下のメソッドに対する更新が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b75bf-292">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="b75bf-293">更新された監査: 新しい操作の種類</span><span class="sxs-lookup"><span data-stu-id="b75bf-293">Audit Updated: New operation types</span></span>

<span data-ttu-id="b75bf-294">顧客が DAP を承認および終了した日時を把握するための、新しい[操作の種類](https://docs.microsoft.com/partner-center/develop/auditing-resources)が追加されました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-294">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="b75bf-295">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="b75bf-295">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="b75bf-296">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="b75bf-296">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="b75bf-297">更新された監査: 新しいリソースと操作の種類</span><span class="sxs-lookup"><span data-stu-id="b75bf-297">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="b75bf-298">顧客ディレクトリ ロールのシナリオをサポートするための、新しい[リソースと操作の種類](https://docs.microsoft.com/partner-center/develop/auditing-resources)が追加されました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-298">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="b75bf-299">新しいリソースの種類 "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="b75bf-299">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="b75bf-300">操作の種類 "AddUserMember" と "RemoveUserMember"</span><span class="sxs-lookup"><span data-stu-id="b75bf-300">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="b75bf-301">顧客アカウントに対する SDK の更新</span><span class="sxs-lookup"><span data-stu-id="b75bf-301">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="b75bf-302">GET のサポート /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span><span class="sxs-lookup"><span data-stu-id="b75bf-302">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="b75bf-303">GET /customers/{customer-tenant-id}/qualifications</span><span class="sxs-lookup"><span data-stu-id="b75bf-303">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="b75bf-304">POST /customers/{customer_id}/qualifications?code={validationCode}</span><span class="sxs-lookup"><span data-stu-id="b75bf-304">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="b75bf-305">追加の変更</span><span class="sxs-lookup"><span data-stu-id="b75bf-305">Additional changes</span></span>

<span data-ttu-id="b75bf-306">新しいコマースの一部として導入された次の変更は、現在、M365 または D365 の新しいコマース エクスペリエンスのテクニカル プレビューに含まれているパートナーのみが、招待に基づいて利用できます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-306">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="b75bf-307">新しいコマースのテクニカル プレビューに含まれていないパートナーは、影響を受けないようにして、下位互換性を確保する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-307">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="b75bf-308">カタログの変更:</span><span class="sxs-lookup"><span data-stu-id="b75bf-308">Catalog Changes:</span></span>

  - <span data-ttu-id="b75bf-309">GET /products/{product-id}/skus/{sku-id}</span><span class="sxs-lookup"><span data-stu-id="b75bf-309">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="b75bf-310">購入および管理:</span><span class="sxs-lookup"><span data-stu-id="b75bf-310">Purchase and Manage:</span></span>
  - <span data-ttu-id="b75bf-311">GET /customers/{customerId}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="b75bf-311">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="b75bf-312">GET /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="b75bf-312">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="b75bf-313">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="b75bf-313">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="b75bf-314">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="b75bf-314">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="b75bf-315">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="b75bf-315">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="b75bf-316">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="b75bf-316">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="b75bf-317">次の手順</span><span class="sxs-lookup"><span data-stu-id="b75bf-317">Next Steps</span></span>

- <span data-ttu-id="b75bf-318">最新バージョン [MicrosoftPartnerCenter.NETSDK (NuGet ギャラリー | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0) をダウンロードする</span><span class="sxs-lookup"><span data-stu-id="b75bf-318">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="b75bf-319">[GitHub サンプル](https://github.com/Microsoft/Partner-Center-DotNet-Samples)をダウンロードして確認する</span><span class="sxs-lookup"><span data-stu-id="b75bf-319">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="b75bf-320">CSP コマーシャル マーケットプレース プランと、対象となるプランの FY21 CSP インセンティブ</span><span class="sxs-lookup"><span data-stu-id="b75bf-320">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-321">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-321">Categories</span></span>

- <span data-ttu-id="b75bf-322">日付: 2021 年 3 月 18 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-322">Date: 2021-03-18</span></span>
- <span data-ttu-id="b75bf-323">機能</span><span class="sxs-lookup"><span data-stu-id="b75bf-323">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-324">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-324">Impacted audience</span></span>

<span data-ttu-id="b75bf-325">クラウド ソリューション プロバイダー プログラムにおける間接プロバイダーと直接請求パートナー</span><span class="sxs-lookup"><span data-stu-id="b75bf-325">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="b75bf-326">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-326">Details</span></span>

<span data-ttu-id="b75bf-327">クラウド ソリューション プロバイダー プログラムにおける間接プロバイダーおよび直接請求パートナーは、サードパーティのプランを販売できます。また、パートナー センターまたは Azure portal でトランザクションが実行された、対象となるサードパーティのプランごとにリベート インセンティブを獲得することができます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-327">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="b75bf-328">インセンティブは、対象となるプランの請求済み売上に対するリベートの形式であり、**2021 年 6 月 30 日まで利用可能** です。</span><span class="sxs-lookup"><span data-stu-id="b75bf-328">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="b75bf-329">この CSP コマーシャル マーケットプレース プランのインセンティブについて、以下で引き続き学習してください。顧客に今すぐ連絡して、継続的な成功とデジタル変革を実現するための適切なプランを特定してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-329">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="b75bf-330">Microsoft では、独立系ソフトウェア ベンダー (ISV) と提携して、Microsoft 顧客向けの最新の IaaS および SaaS ソリューションを市場に投入しています。</span><span class="sxs-lookup"><span data-stu-id="b75bf-330">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="b75bf-331">ISV 発行者は、Microsoft パートナー チャネルを通じたプランの販売を有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-331">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="b75bf-332">インセンティブの対象となるプランは、次の 2 つのカテゴリに分類されます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-332">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="b75bf-333">Azure IP 共同販売インセンティブ対象ステータスを持つ、SaaS と IaaS のサードパーティ プランを選択する。</span><span class="sxs-lookup"><span data-stu-id="b75bf-333">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="b75bf-334">Teams、または少なくとも 2 つの Microsoft 365 生産性向上アプリ (PowerPoint、Word、Excel、Outlook、SharePoint など) で統合された SaaS アプリケーション。</span><span class="sxs-lookup"><span data-stu-id="b75bf-334">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="b75bf-335">次の手順とリソース</span><span class="sxs-lookup"><span data-stu-id="b75bf-335">Next steps and resources</span></span>

- <span data-ttu-id="b75bf-336">対象となるマーケットプレース アプリやインセンティブ対象アプリを販売する場合の[パートナー インセンティブ](https://partner.microsoft.com/membership/partner-incentives)の獲得について確認してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-336">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="b75bf-337">新しいプランは毎月追加されます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-337">New offers are added monthly.</span></span>  
- [<span data-ttu-id="b75bf-338">クラウド ソリューション プロバイダーの直接請求パートナー インセンティブ リソース</span><span class="sxs-lookup"><span data-stu-id="b75bf-338">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="b75bf-339">クラウド ソリューション プロバイダーの間接プロバイダー インセンティブ リソース</span><span class="sxs-lookup"><span data-stu-id="b75bf-339">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="b75bf-340">この[プレゼンテーション](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf)を確認して、コマーシャル マーケットプレース アプリの販売に関する詳細を確認してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-340">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="b75bf-341">その他のリソースについては、[こちら](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-341">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="b75bf-342">[パートナー センター](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover)または [Azure portal](https://ms.portal.azure.com/#home) でコマーシャル マーケットプレース カタログを探索する</span><span class="sxs-lookup"><span data-stu-id="b75bf-342">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="b75bf-343">[API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) 使用して、会社のマーケットプレースにアプリを統合する</span><span class="sxs-lookup"><span data-stu-id="b75bf-343">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="b75bf-344">取引を行いたい ISV に連絡する</span><span class="sxs-lookup"><span data-stu-id="b75bf-344">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="b75bf-345">間接プロバイダーは API を使用して統合し、販売するアプリについてリセラーに指示する必要があります</span><span class="sxs-lookup"><span data-stu-id="b75bf-345">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="b75bf-346">疑問がある場合</span><span class="sxs-lookup"><span data-stu-id="b75bf-346">Questions?</span></span>  

<span data-ttu-id="b75bf-347">パートナー センターのコマーシャル マーケットプレースの概要については、[この記事](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-347">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="b75bf-348">さらにサポートが必要な場合は、パートナー センターでサポート リクエストを作成できます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-348">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="b75bf-349">詳細については、[https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-349">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="b75bf-350">Power BI Premium プランの名前と前提条件の更新</span><span class="sxs-lookup"><span data-stu-id="b75bf-350">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-351">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-351">Categories</span></span>

- <span data-ttu-id="b75bf-352">日付: 2021 年 3 月 18 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-352">Date: 2021-03-18</span></span>
- <span data-ttu-id="b75bf-353">機能</span><span class="sxs-lookup"><span data-stu-id="b75bf-353">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="b75bf-354">まとめ</span><span class="sxs-lookup"><span data-stu-id="b75bf-354">Summary</span></span>

<span data-ttu-id="b75bf-355">2021 年 4 月 1 日の最終的な価格表は、Power BI Premium Per User の名前や前提条件の情報を明確にするために更新されます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-356">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-356">Impacted audience</span></span>

<span data-ttu-id="b75bf-357">クラウド ソリューション プロバイダー (CSP) の直接および間接のパートナー</span><span class="sxs-lookup"><span data-stu-id="b75bf-357">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-358">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-358">Details</span></span>

<span data-ttu-id="b75bf-359">2021 年 4 月 1 日の最終的な価格表は、Power BI Premium Per User の名前や前提条件の情報を明確にするために更新されます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-359">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="b75bf-360">最終的な価格表が更新されるまで、このセクションの情報を使用して、正しい製品が注文されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-360">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="b75bf-361">次の詳細は、影響を受ける SKU と前提条件の詳細を示しています。</span><span class="sxs-lookup"><span data-stu-id="b75bf-361">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="b75bf-362">3 月 1 日の価格表プレビューでのプラン表示名</span><span class="sxs-lookup"><span data-stu-id="b75bf-362">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="b75bf-363">4 月 1 日の最終的な価格表での更新されたプラン表示名</span><span class="sxs-lookup"><span data-stu-id="b75bf-363">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="b75bf-364">プラン ID</span><span class="sxs-lookup"><span data-stu-id="b75bf-364">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="b75bf-365">Power BI Premium Per User アドオン (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="b75bf-365">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="b75bf-366">Power BI Premium Per User アドオン **(Office)** (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="b75bf-366">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="b75bf-367">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="b75bf-367">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="b75bf-368">このプランを購入するには、次のいずれかの前提条件が満たされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-368">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="b75bf-369">プラン表示名</span><span class="sxs-lookup"><span data-stu-id="b75bf-369">Offer display name</span></span> | <span data-ttu-id="b75bf-370">プラン ID</span><span class="sxs-lookup"><span data-stu-id="b75bf-370">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="b75bf-371">Microsoft 365 E5 (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="b75bf-371">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="b75bf-372">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="b75bf-372">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="b75bf-373">オーディオ会議なしの Microsoft 365 E5 (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="b75bf-373">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="b75bf-374">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="b75bf-374">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="b75bf-375">Office 365 E5 (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="b75bf-375">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="b75bf-376">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="b75bf-376">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="b75bf-377">Office 365 E5 (非営利団体職員向けの価格) 試用版</span><span class="sxs-lookup"><span data-stu-id="b75bf-377">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="b75bf-378">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="b75bf-378">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="b75bf-379">オーディオ会議なしの Office 365 E5 (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="b75bf-379">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="b75bf-380">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="b75bf-380">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="b75bf-381">次の Power BI Premium プランには、購入に必要な前提条件があります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-381">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="b75bf-382">プラン表示名</span><span class="sxs-lookup"><span data-stu-id="b75bf-382">Offer display name</span></span> | <span data-ttu-id="b75bf-383">プラン ID</span><span class="sxs-lookup"><span data-stu-id="b75bf-383">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="b75bf-384">Power BI Premium Per User アドオン (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="b75bf-384">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="b75bf-385">ef0b895b-681b-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="b75bf-385">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="b75bf-386">このプランを購入するには、この前提条件が必要です。</span><span class="sxs-lookup"><span data-stu-id="b75bf-386">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="b75bf-387">プラン表示名</span><span class="sxs-lookup"><span data-stu-id="b75bf-387">Offer display name</span></span> | <span data-ttu-id="b75bf-388">プラン ID</span><span class="sxs-lookup"><span data-stu-id="b75bf-388">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="b75bf-389">Power BI Pro (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="b75bf-389">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="b75bf-390">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="b75bf-390">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="b75bf-391">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b75bf-391">Next steps</span></span>

<span data-ttu-id="b75bf-392">このトピックに関するリソースを確認し、この情報を組織内の該当する関係者と共有してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-392">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="b75bf-393">疑問がある場合</span><span class="sxs-lookup"><span data-stu-id="b75bf-393">Questions?</span></span>

<span data-ttu-id="b75bf-394">これらのプランについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-394">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a><span data-ttu-id="b75bf-395">Microsoft 365 F3 の 3 月の価格更新</span><span class="sxs-lookup"><span data-stu-id="b75bf-395">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-396">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-396">Categories</span></span>

- <span data-ttu-id="b75bf-397">日付: 2021 年 3 月 16 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-397">Date: 2021-03-16</span></span>
- <span data-ttu-id="b75bf-398">製品サービス/市場</span><span class="sxs-lookup"><span data-stu-id="b75bf-398">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="b75bf-399">まとめ</span><span class="sxs-lookup"><span data-stu-id="b75bf-399">Summary</span></span>

<span data-ttu-id="b75bf-400">Microsoft 365 F3 のイギリス ポンド (GBP) とユーロ (EUR) では、2021 年 3 月の正しくない価格が修正されました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-400">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-401">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-401">Impacted audience</span></span>

<span data-ttu-id="b75bf-402">クラウド ソリューション プロバイダー (CSP) プログラムを通して、2021 年 3 月 1 日から 3 月 17 日までの間に Microsoft 365 F3 を GBP または EUR で購入したパートナー。</span><span class="sxs-lookup"><span data-stu-id="b75bf-402">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-403">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-403">Details</span></span>

<span data-ttu-id="b75bf-404">Microsoft は Microsoft 365 F3 の価格が正しくなかった問題を解決しました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-404">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="b75bf-405">GBP と EUR の価格が正しくありませんでした。2021 年 3 月 1 日から 3 月 17 日の間に購入したプランのみが対象となります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-405">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="b75bf-406">影響を受けるプランと通貨は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="b75bf-406">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="b75bf-407">プラン名</span><span class="sxs-lookup"><span data-stu-id="b75bf-407">Offer name</span></span> | <span data-ttu-id="b75bf-408">Currency</span><span class="sxs-lookup"><span data-stu-id="b75bf-408">Currency</span></span> | <span data-ttu-id="b75bf-409">プラン ID</span><span class="sxs-lookup"><span data-stu-id="b75bf-409">Offer ID</span></span> | <span data-ttu-id="b75bf-410">マテリアル ID</span><span class="sxs-lookup"><span data-stu-id="b75bf-410">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="b75bf-411">Microsoft 365 F3 (非営利団体)</span><span class="sxs-lookup"><span data-stu-id="b75bf-411">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="b75bf-412">GBP</span><span class="sxs-lookup"><span data-stu-id="b75bf-412">GBP</span></span> | <span data-ttu-id="b75bf-413">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="b75bf-413">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="b75bf-414">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="b75bf-414">AAD-11626</span></span> |
| <span data-ttu-id="b75bf-415">Microsoft 365 F3 (商用)</span><span class="sxs-lookup"><span data-stu-id="b75bf-415">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="b75bf-416">EUR</span><span class="sxs-lookup"><span data-stu-id="b75bf-416">EUR</span></span>| <span data-ttu-id="b75bf-417">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="b75bf-417">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="b75bf-418">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="b75bf-418">AAA-89898</span></span> |
 
<span data-ttu-id="b75bf-419">3 月および 4 月のプレビューのライセンスベースの価格表は、3 月 16 日午後 5 時 (太平洋標準時) に更新されました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-419">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="b75bf-420">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b75bf-420">Next steps</span></span>

- <span data-ttu-id="b75bf-421">パートナーは、3 月と 4 月のプレビューの両方の現在のライセンスベースの価格表をもう一度ダウンロードし、該当する場合はこれらの価格を修正する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-421">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="b75bf-422">Microsoft は、今後数週間にわたって影響を受けたパートナーにメールで連絡し、影響を受けるトランザクションの修正に関連する今後の手順について通知します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-422">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="b75bf-423">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="b75bf-423">Questions?</span></span>

<span data-ttu-id="b75bf-424">さらにご質問がある場合は、関連する CSP Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-424">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a><span data-ttu-id="b75bf-425">パートナー センターでの会社正式名称の更新</span><span class="sxs-lookup"><span data-stu-id="b75bf-425">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-426">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-426">Categories</span></span>

- <span data-ttu-id="b75bf-427">日付: 2021 年 3 月 16 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-427">Date: 2021-03-16</span></span>
- <span data-ttu-id="b75bf-428">効率とスケールの向上</span><span class="sxs-lookup"><span data-stu-id="b75bf-428">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="b75bf-429">まとめ</span><span class="sxs-lookup"><span data-stu-id="b75bf-429">Summary</span></span>

<span data-ttu-id="b75bf-430">2021 年 3 月から、Microsoft Partner Network (MPN) パートナーとクラウド ソリューション プロバイダー (CSP) 間接リセラーは、パートナー センターで会社の正式名称を更新できます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-430">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-431">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-431">Impacted audience</span></span>

<span data-ttu-id="b75bf-432">MPN パートナーと CSP 間接リセラー (CSP 直接請求パートナーは対象外です)</span><span class="sxs-lookup"><span data-stu-id="b75bf-432">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-433">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-433">Details</span></span>

<span data-ttu-id="b75bf-434">2021 年 3 月から MPN パートナーと CSP 間接リセラーは、パートナー センターで、規則に従って、セルフ サービス方式で、会社の正式名称を更新できます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-434">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="b75bf-435">この新機能により、パートナーは社名を更新するためにパートナー センター サポート チケットを提出する必要がなくなります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-435">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="b75bf-436">これにより、パートナーはこれらの操作を行う際の時間をかなり節約することができます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-436">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="b75bf-437">詳細については、「[法的ビジネスプロファイルを更新する](../update-your-partner-profile.md#update-your-legal-business-profile)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-437">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="b75bf-438">企業の公式プロファイルの社名に誤字や略式表記がないこと、会社の正式な登録情報と完全に一致していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-438">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="b75bf-439">組織プロファイル更新の詳細は[組織プロファイルの有効性を確認する](../update-your-partner-profile.md#update-your-legal-business-profile)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-439">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="b75bf-440">次の手順</span><span class="sxs-lookup"><span data-stu-id="b75bf-440">Next steps</span></span>

<span data-ttu-id="b75bf-441">担当チームが手続きの見直し、更新を実施できるよう、この情報を組織で共有してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-441">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="b75bf-442">ご質問がある場合は、</span><span class="sxs-lookup"><span data-stu-id="b75bf-442">Questions?</span></span>

<span data-ttu-id="b75bf-443">さらにご質問がある場合は、関連する CSP Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-443">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a><span data-ttu-id="b75bf-444">クラウド ソリューション プロバイダー (CSP) プログラムの進歩とオープン ライセンス プログラムの変更に関する最新情報</span><span class="sxs-lookup"><span data-stu-id="b75bf-444">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-445">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-445">Categories</span></span>

- <span data-ttu-id="b75bf-446">日付: 2021 年 3 月 15 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-446">Date: 2021-03-15</span></span>
- <span data-ttu-id="b75bf-447">機能</span><span class="sxs-lookup"><span data-stu-id="b75bf-447">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="b75bf-448">まとめ</span><span class="sxs-lookup"><span data-stu-id="b75bf-448">Summary</span></span>

<span data-ttu-id="b75bf-449">オープン ライセンス プログラムの変更に伴い、商用および公的機関向けの新しい永続ライセンス ソフトウェア商品を、クラウド ソリューション プロバイダー (CSP) プログラムに追加します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-449">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-450">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-450">Impacted audience</span></span>

<span data-ttu-id="b75bf-451">オープン ライセンス プログラムを通じて販売を行っている商業ディストリビューターと管理下のリセラー、および、永続ライセンス ソフトウェアの取引を行っているすべての CSP パートナー</span><span class="sxs-lookup"><span data-stu-id="b75bf-451">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-452">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-452">Details</span></span>

<span data-ttu-id="b75bf-453">2020 年 9 月、Microsoft はデジタル化推進の一環として、CSP プログラムのパートナーにビジネス機会を提供するための一連の方策を[発表しました](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/)。一例として、パートナーはオンプレミスのソフトウェアを使用できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-453">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="b75bf-454">これらの変更により、パートナーは CSP のソフトウェア ライセンスを利用してビジネスを成長させ、リーチを広げることができ、クラウド ファーストである現環境での成功を期待できます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-454">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="b75bf-455">これはまた、顧客のクラウド移行をサポートし、顧客のハイブリッド クラウド環境の運用に求められる柔軟性をパートナーに与えます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-455">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="b75bf-456">こうしてデジタル化を推し進める中で、Microsoft は次の変更を発表しました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-456">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="b75bf-457">2021 年 7 月 1 日: 新たな SKU、製品、販促物をオープン ライセンス プログラムの価格表に追加することを中止します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-457">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="b75bf-458">2021 年 7 月 7 日: Get Genuine Windows と Visual Studio Professional の 2 商品、および公的機関 (政府、教育機関、NPO。[発表](./2020-december.md#9)をご確認ください) 向けオファーを CSP 永続ライセンス ソフトウェアの価格表に追加します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-458">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="b75bf-459">価格表はパートナー センターの [[Sell]\(販売\) > [Pricing & Offers]\(価格とオファー\)](https://partnercenter.microsoft.com/pcv/sales) ページの [ソフトウェア] セクションで閲覧できます。この価格表はこの日に改定する予定です。</span><span class="sxs-lookup"><span data-stu-id="b75bf-459">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="b75bf-460">CSP プログラムの進歩とオープン ライセンス プログラムの変更の詳細は、下の「**次のステップ**」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-460">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="b75bf-461">次のステップ:</span><span class="sxs-lookup"><span data-stu-id="b75bf-461">Next Steps:</span></span>

- <span data-ttu-id="b75bf-462">CSP プログラムの進歩: 準備資料[クラウド ソリューション プロバイダー プログラムの永続ライセンス ソフトウェア](https://partner.microsoft.com/resources/collection/software-in-csp#/)をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-462">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="b75bf-463">こちらの[レディネス マップ](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf)を利用すると、ロールに適した情報をすばやく見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-463">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="b75bf-464">オープン ライセンス プログラムの変更: 準備資料[ CSP プログラムの進歩とオープン ライセンス プログラムの変更](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-464">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="b75bf-465">こちらの[レディネス マップ](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf)を利用すると、ロールに適した情報をすばやく見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-465">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="b75bf-466">質問</span><span class="sxs-lookup"><span data-stu-id="b75bf-466">Questions</span></span>

<span data-ttu-id="b75bf-467">さらにご質問がある場合は、関連する CSP Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-467">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="b75bf-468">以前の発表に関する最新情報: Compliance Manager のプレミアム評価アドオン</span><span class="sxs-lookup"><span data-stu-id="b75bf-468">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-469">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-469">Categories</span></span>

- <span data-ttu-id="b75bf-470">日付: 2021 年 3 月 15 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-470">Date: 2021-03-15</span></span>
- <span data-ttu-id="b75bf-471">ビジネスを拡大する</span><span class="sxs-lookup"><span data-stu-id="b75bf-471">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="b75bf-472">まとめ</span><span class="sxs-lookup"><span data-stu-id="b75bf-472">Summary</span></span>

<span data-ttu-id="b75bf-473">オファーの試用版は価格表に掲載しないことになっており、今後削除する予定です。</span><span class="sxs-lookup"><span data-stu-id="b75bf-473">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-474">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-474">Impacted audience</span></span>

<span data-ttu-id="b75bf-475">クラウド ソリューション プロバイダー プログラムで取引を行うパートナー</span><span class="sxs-lookup"><span data-stu-id="b75bf-475">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-476">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-476">Details</span></span>

<span data-ttu-id="b75bf-477">オファーの試用版は価格表に掲載しないことになっています。</span><span class="sxs-lookup"><span data-stu-id="b75bf-477">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="b75bf-478">これらは 2021 年 5 月 1 日の価格表から削除します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-478">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="b75bf-479">元の発表は[こちら](./2021-february.md#4)でご覧いただけます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-479">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="b75bf-480">その他のリソース</span><span class="sxs-lookup"><span data-stu-id="b75bf-480">Additional resources</span></span>

- [<span data-ttu-id="b75bf-481">Microsoft 365 E5 のセキュリティとコンプライアンス</span><span class="sxs-lookup"><span data-stu-id="b75bf-481">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="b75bf-482">Microsoft コンプライアンス マネージャーでの評価の作成と管理 - Microsoft 365 コンプライアンス</span><span class="sxs-lookup"><span data-stu-id="b75bf-482">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="b75bf-483">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b75bf-483">Next steps</span></span>

<span data-ttu-id="b75bf-484">このトピックに関するリソースを確認し、この情報を組織内の該当する関係者と共有してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-484">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="b75bf-485">疑問がある場合</span><span class="sxs-lookup"><span data-stu-id="b75bf-485">Questions?</span></span>

<span data-ttu-id="b75bf-486">これらのオファーに関するご質問については、Yammer の関連コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-486">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="b75bf-487">One Commercial Partner (OCP) Go-to-Market (GTM) から Microsoft コマーシャル マーケットプレースにソリューションを移動する</span><span class="sxs-lookup"><span data-stu-id="b75bf-487">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-488">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-488">Categories</span></span>

- <span data-ttu-id="b75bf-489">日付: 2021 年 3 月 12 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-489">Date: 2021-03-12</span></span>
- <span data-ttu-id="b75bf-490">機能</span><span class="sxs-lookup"><span data-stu-id="b75bf-490">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="b75bf-491">まとめ</span><span class="sxs-lookup"><span data-stu-id="b75bf-491">Summary</span></span>

<span data-ttu-id="b75bf-492">2021 年 3 月 29 日から One Commercial Partner (OCP) Go-to-Market (GTM) の機能を制限します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-492">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="b75bf-493">パートナー センターのコマーシャル マーケットプレースにソリューションを移動することを推奨します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-493">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-494">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-494">Impacted audience</span></span>

<span data-ttu-id="b75bf-495">OCP GTM のソリューションを使用して共同販売を行っている組織</span><span class="sxs-lookup"><span data-stu-id="b75bf-495">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-496">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-496">Details</span></span>

<span data-ttu-id="b75bf-497">Microsoft は 2020 年 12 月に、Microsoft OCP GTM ツールからパートナー センターの Microsoft コマーシャル マーケットプレースへの移行を開始しました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-497">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="b75bf-498">この移行によってコマーシャル マーケットプレースの機能を拡張します。これは、皆様のソリューションを何百万もの顧客に紹介し、Microsoft や他のパートナー販売者と相互にビジネス機会を共有し、革新的なソリューションを共同販売できるプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="b75bf-498">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="b75bf-499">移行の次のステップは 2021 年 3 月 29 日に実施します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-499">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="b75bf-500">そのときに、OCP GTM の機能の制限を開始し、一部のサービスは閲覧しかできなくなります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-500">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="b75bf-501">現在 OCP GTM のソリューションを使用して共同販売を行っている場合、ソリューションをコマーシャル マーケットプレースに移動することを推奨します。それによって、この機能を利用できるようになり、公開作業も単純化できます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-501">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="b75bf-502">コマーシャル マーケットプレースに移行すると、共同販売する商品は主としてパートナー センターで公開することになります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-502">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="b75bf-503">そこでは、Microsoft が採用している共通の販路と製品内部の仕組みを通じて皆様のソリューションを共通の顧客に紹介することで、引き続きビジネスを成長させることができます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-503">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="b75bf-504">[コマーシャル マーケットプレースの詳細](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/)。</span><span class="sxs-lookup"><span data-stu-id="b75bf-504">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="b75bf-505">次の手順</span><span class="sxs-lookup"><span data-stu-id="b75bf-505">Next steps</span></span>

- <span data-ttu-id="b75bf-506">まだソリューションを移動させていない場合、[移行ガイド](/azure/marketplace/co-sell-solution-migration)に詳述された手順に従うか、[ステップ バイ ステップの動画チュートリアル](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4)を見て移動作業を完了し、コマーシャル マーケットプレースでソリューションの公開を始めてください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-506">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="b75bf-507">OCP GTM の機能の制限に関するご質問については [Microsoft コマーシャル マーケットプレース共同販売公開要件 FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf) に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-507">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="b75bf-508">(2021 年 3 月 29 日に始まる OCP GTM の機能の制限に関するセクションをお読みください。)</span><span class="sxs-lookup"><span data-stu-id="b75bf-508">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="b75bf-509">疑問がある場合</span><span class="sxs-lookup"><span data-stu-id="b75bf-509">Questions?</span></span>

<span data-ttu-id="b75bf-510">ご質問がある場合、詳しく知りたい場合は[サポート](https://partner.microsoft.com/support/?stage=1)にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-510">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="b75bf-511">クラウド ソリューション プロバイダー (CSP) プログラムの Azure 取引新サービスをロシアに拡大</span><span class="sxs-lookup"><span data-stu-id="b75bf-511">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-512">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-512">Categories</span></span>

- <span data-ttu-id="b75bf-513">日付: 2021 年 3 月 10 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-513">Date: 2021-03-10</span></span>
- <span data-ttu-id="b75bf-514">機能</span><span class="sxs-lookup"><span data-stu-id="b75bf-514">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-515">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-515">Impacted audience</span></span>

<span data-ttu-id="b75bf-516">クラウド ソリューション プロバイダー (CSP) プログラムを通じてロシアで取引を行うすべてのパートナー。</span><span class="sxs-lookup"><span data-stu-id="b75bf-516">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-517">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-517">Details</span></span>

<span data-ttu-id="b75bf-518">2021 年 3 月 10 日から **CSP の Azure 取引新サービスをロシアで利用** できるようになります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-518">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="b75bf-519">このサービスにより、顧客が Azure のサービスを購入、使用する方法を効率化し、改善します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-519">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="b75bf-520">また、CSP プログラムのパートナーは、さまざまな販売状況を通じて Azure の料金を安定的に見通し、国際的目安として米ドルでの料金を把握し、請求日をそろえ、Azure Cost Management にアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-520">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="b75bf-521">次の手順</span><span class="sxs-lookup"><span data-stu-id="b75bf-521">Next steps</span></span>

<span data-ttu-id="b75bf-522">Azure の新しい取引サービスを紹介し、追加的な情報を提供する資料をいくつか用意しています。</span><span class="sxs-lookup"><span data-stu-id="b75bf-522">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="b75bf-523">最新の FAQ、プレゼン資料、動画、その他の資料を [CSP プログラム最新情報資料ギャラリー](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)で見付けてください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-523">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="b75bf-524">パートナー センター ソフトウェア ライセンス キーとダウンロード フルフィルメント</span><span class="sxs-lookup"><span data-stu-id="b75bf-524">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-525">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-525">Categories</span></span>

- <span data-ttu-id="b75bf-526">日付: 2021 年 3 月 4 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-526">Date: 2021-03-04</span></span>
- <span data-ttu-id="b75bf-527">機能</span><span class="sxs-lookup"><span data-stu-id="b75bf-527">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="b75bf-528">まとめ</span><span class="sxs-lookup"><span data-stu-id="b75bf-528">Summary</span></span>

<span data-ttu-id="b75bf-529">パートナー センターのソフトウェア ダウンロードおよびライセンス キー フルフィルメント機能が復元されました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-529">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-530">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-530">Impacted audience</span></span>

<span data-ttu-id="b75bf-531">パートナー センターを通じて永続的およびサーバーのサブスクリプション ソフトウェアの注文を処理しているすべてのクラウド ソリューション プロバイダー (CSP) パートナー</span><span class="sxs-lookup"><span data-stu-id="b75bf-531">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-532">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-532">Details</span></span>

<span data-ttu-id="b75bf-533">パートナーからのフィードバックに応えて、永続的およびサーバーのサブスクリプション ソフトウェアの注文に対してソフトウェアとライセンス キーを取得するパートナー センターのフルフィルメント機能を復元しています。</span><span class="sxs-lookup"><span data-stu-id="b75bf-533">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="b75bf-534">2021 年 1 月 19 日に削除される前の状態に復元されます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-534">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="b75bf-535">([お知らせ](2020-september.md#17)を参照してください。)</span><span class="sxs-lookup"><span data-stu-id="b75bf-535">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="b75bf-536">ソフトウェア ライセンス キーとダウンロード リンクは、価値ある重要な知財資産であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-536">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="b75bf-537">リークが生じると、それらのライセンス認証制限がすぐに枯渇し、顧客エクスペリエンスやパートナー エクスペリエンスに悪影響を及ぼす恐れがあります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-537">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="b75bf-538">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b75bf-538">Next steps</span></span>

<span data-ttu-id="b75bf-539">ソフトウェアキーの配布に関する使用方法と重要なガイダンスについては、次のリソースを参照してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-539">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="b75bf-540">CSP プログラムによるオンプレミス ソフトウェアの販売</span><span class="sxs-lookup"><span data-stu-id="b75bf-540">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="b75bf-541">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (**ソフトウェア キーの配布に関するガイダンス** に関するセクションを参照してください)。</span><span class="sxs-lookup"><span data-stu-id="b75bf-541">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="b75bf-542">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="b75bf-542">Questions?</span></span>

<span data-ttu-id="b75bf-543">この通知についてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-543">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="b75bf-544">Partner Sales Connect (PSC) からパートナー センターに取引を移行</span><span class="sxs-lookup"><span data-stu-id="b75bf-544">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-545">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-545">Categories</span></span>

- <span data-ttu-id="b75bf-546">日付: 2021 年 3 月 4 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-546">Date: 2021-03-04</span></span>
- <span data-ttu-id="b75bf-547">機能</span><span class="sxs-lookup"><span data-stu-id="b75bf-547">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="b75bf-548">まとめ</span><span class="sxs-lookup"><span data-stu-id="b75bf-548">Summary</span></span>

<span data-ttu-id="b75bf-549">Partner Sales Connect (PSC) は、2021 年 3 月 31 日から読み取り専用アクセスに移行するので、PSC からパートナー センターに取引を移行し始めることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="b75bf-549">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-550">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-550">Impacted audience</span></span>

<span data-ttu-id="b75bf-551">PSC での取引があるパートナー</span><span class="sxs-lookup"><span data-stu-id="b75bf-551">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-552">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-552">Details</span></span>

<span data-ttu-id="b75bf-553">成長に対する共有コミットメントの一環として、**Microsoft との共同販売** は、お客様が **認識され、専門知識を提供し、顧客フットプリントを拡大して**、良好な顧客アウトカムを得るための手段です。</span><span class="sxs-lookup"><span data-stu-id="b75bf-553">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="b75bf-554">パートナー センターで共同販売エクスペリエンスを管理すれば、平均的な処理が通常より **3.5 倍高速** になり、顧客への直接販売や、パートナー、Microsoft の販売者チャネルなどに対する販売ができ、1 か所でパイプライン全体を管理できます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-554">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="b75bf-555">**PSC** は **2021 年 3 月 31 日** から **読み取り専用アクセス** に移行するため、パートナー センターへの移行を開始し、以下のような機能改善にアクセスすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="b75bf-555">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="b75bf-556">お客様が必要とするサポートの種類に基づいて、Microsoft と共有する取引を適切な販売者に **ルーティングする際の正確さの向上**。</span><span class="sxs-lookup"><span data-stu-id="b75bf-556">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="b75bf-557">インセンティブの対象となるソリューションに対する適格性があるか、および ISV コネクト プログラムの基準を満たしているかについての **前払い取引の検証**。このため、承認プロセスと最終的な実行証明 (POE) の立証が簡略化されます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-557">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="b75bf-558">すべての共同販売機会とセールス見込み客を 1 か所で管理するための **シームレスなユーザー エクスペリエンス**。</span><span class="sxs-lookup"><span data-stu-id="b75bf-558">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="b75bf-559">また、お客様の移行を支援するために、最近パートナー センターに次のような新しい機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-559">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="b75bf-560">共同販売機会の一括操作</span><span class="sxs-lookup"><span data-stu-id="b75bf-560">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="b75bf-561">[取引移行機能](../psc-to-pc.md) (**PSC 取引の移行** に関するセクションを参照してください)。</span><span class="sxs-lookup"><span data-stu-id="b75bf-561">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="b75bf-562">パートナー センターの共同販売エクスペリエンスを利用することで、販売チームは、見込み客や機会の促進、契約の締結、顧客との長期的な関係の形成に集中する時間が増えます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-562">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="b75bf-563">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b75bf-563">Next steps</span></span>

<span data-ttu-id="b75bf-564">パートナー センターへの[移行ガイド](../psc-to-pc.md)を使用して、PSC からパートナー センターに取引を移行する手順について説明します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-564">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="b75bf-565">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="b75bf-565">Questions?</span></span>

<span data-ttu-id="b75bf-566">その他の質問については、[サポート](https://partner.microsoft.com/support/?stage=1)にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-566">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="b75bf-567">新しい Microsoft Dynamics 365 製品およびオファーが 2021 年 4 月 1 日に利用できるようになります</span><span class="sxs-lookup"><span data-stu-id="b75bf-567">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-568">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-568">Categories</span></span>

- <span data-ttu-id="b75bf-569">日付: 2021 年 3 月 4 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-569">Date: 2021-03-04</span></span>
- <span data-ttu-id="b75bf-570">機能</span><span class="sxs-lookup"><span data-stu-id="b75bf-570">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="b75bf-571">まとめ</span><span class="sxs-lookup"><span data-stu-id="b75bf-571">Summary</span></span>

<span data-ttu-id="b75bf-572">2021 年 4 月 1 日、Microsoft は、クラウド ソリューション プロバイダー (CSP) プログラム用のいくつかの新しい製品およびプランを開始します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-572">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-573">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-573">Impacted audience</span></span>

<span data-ttu-id="b75bf-574">クラウド ソリューション プロバイダー (CSP) プログラムを通じて取引を行う、すべてのパートナー様</span><span class="sxs-lookup"><span data-stu-id="b75bf-574">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-575">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-575">Details</span></span>

<span data-ttu-id="b75bf-576">2021 年 4 月 1 日に、Microsoft は、次のような新しい製品およびプランを開始します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-576">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="b75bf-577">Power BI Premium Per User</span><span class="sxs-lookup"><span data-stu-id="b75bf-577">Power BI Premium Per User</span></span>
- <span data-ttu-id="b75bf-578">Customer Voice および Marketing USL の地域およびセグメントの拡張</span><span class="sxs-lookup"><span data-stu-id="b75bf-578">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="b75bf-579">**Power BI Premium Per User**</span><span class="sxs-lookup"><span data-stu-id="b75bf-579">**Power BI Premium Per User**</span></span>

<span data-ttu-id="b75bf-580">Microsoft は、最初のユーザーごとの Power BI Premium プランを導入します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-580">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="b75bf-581">Power BI Premium は現在、容量構成でのみ販売されています。</span><span class="sxs-lookup"><span data-stu-id="b75bf-581">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="b75bf-582">Power BI Premium Per User は、ユーザーごとに、エンタープライズ ビジネス インテリジェンス (BI) および分析機能へのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-582">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="b75bf-583">その柔軟な個別のシート ライセンスで、中小規模の企業の要求に応えます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-583">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="b75bf-584">このプランについて詳しくは、[Power BI リリースの詳細](/power-platform-release-plan/2020wave2/power-bi/planned-features)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-584">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="b75bf-585">**特典の詳細**</span><span class="sxs-lookup"><span data-stu-id="b75bf-585">**Offer details**</span></span>

<span data-ttu-id="b75bf-586">プラン名は、価格表プレビューとは若干異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-586">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="b75bf-587">プラン名</span><span class="sxs-lookup"><span data-stu-id="b75bf-587">Offer name</span></span> | <span data-ttu-id="b75bf-588">プラン ID</span><span class="sxs-lookup"><span data-stu-id="b75bf-588">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="b75bf-589">Power BI Premium Per User</span><span class="sxs-lookup"><span data-stu-id="b75bf-589">Power BI Premium Per User</span></span> | <span data-ttu-id="b75bf-590">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="b75bf-590">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="b75bf-591">教職員用 Power BI Premium Per User</span><span class="sxs-lookup"><span data-stu-id="b75bf-591">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="b75bf-592">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="b75bf-592">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="b75bf-593">学生用 Power BI Premium Per User</span><span class="sxs-lookup"><span data-stu-id="b75bf-593">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="b75bf-594">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="b75bf-594">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="b75bf-595">Power BI Premium Per User (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="b75bf-595">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="b75bf-596">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="b75bf-596">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="b75bf-597">Power BI Premium Per User アドオン</span><span class="sxs-lookup"><span data-stu-id="b75bf-597">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="b75bf-598">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="b75bf-598">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="b75bf-599">教職員用 Power BI Premium Per User アドオン</span><span class="sxs-lookup"><span data-stu-id="b75bf-599">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="b75bf-600">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="b75bf-600">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="b75bf-601">学生用 Power BI Premium Per User アドオン</span><span class="sxs-lookup"><span data-stu-id="b75bf-601">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="b75bf-602">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="b75bf-602">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="b75bf-603">Power BI Premium Per User アドオン (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="b75bf-603">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="b75bf-604">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="b75bf-604">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="b75bf-605">**Customer Voice および Marketing USL の地域およびセグメントの拡張**</span><span class="sxs-lookup"><span data-stu-id="b75bf-605">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="b75bf-606">2020 年 12 月の発売後のフォローアップとして、Dynamics 365 Customer Voice および Marketing USL プランは、新しい国やより多くの非営利団体および教育機関向けの SKU を追加するように変更されてきました。</span><span class="sxs-lookup"><span data-stu-id="b75bf-606">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="b75bf-607">プラン名</span><span class="sxs-lookup"><span data-stu-id="b75bf-607">Offer name</span></span> | <span data-ttu-id="b75bf-608">プラン ID</span><span class="sxs-lookup"><span data-stu-id="b75bf-608">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="b75bf-609">Dynamics 365 Customer Voice USL (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="b75bf-609">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="b75bf-610">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="b75bf-610">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="b75bf-611">教職員用 Dynamics 365 Customer Voice USL</span><span class="sxs-lookup"><span data-stu-id="b75bf-611">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="b75bf-612">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="b75bf-612">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="b75bf-613">これらのプランについて詳しくは、次のページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-613">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="b75bf-614">Dynamics 365 Customer Service Voice ホーム ページ</span><span class="sxs-lookup"><span data-stu-id="b75bf-614">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="b75bf-615">Dynamics 365 Marketing ホーム ページ</span><span class="sxs-lookup"><span data-stu-id="b75bf-615">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="b75bf-616">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b75bf-616">Next steps</span></span>

<span data-ttu-id="b75bf-617">このトピックに関するリソースを確認し、この情報を組織内の該当する関係者と共有します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-617">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="b75bf-618">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="b75bf-618">Questions?</span></span>

<span data-ttu-id="b75bf-619">これらのプランについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-619">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a><span data-ttu-id="b75bf-620">Microsoft Universal Print が一部のスイートで利用できるようになりました</span><span class="sxs-lookup"><span data-stu-id="b75bf-620">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="b75bf-621">Categories</span><span class="sxs-lookup"><span data-stu-id="b75bf-621">Categories</span></span>

- <span data-ttu-id="b75bf-622">日付: 2021 年 3 月 3 日</span><span class="sxs-lookup"><span data-stu-id="b75bf-622">Date: 2021-03-03</span></span>
- <span data-ttu-id="b75bf-623">機能</span><span class="sxs-lookup"><span data-stu-id="b75bf-623">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="b75bf-624">まとめ</span><span class="sxs-lookup"><span data-stu-id="b75bf-624">Summary</span></span>

<span data-ttu-id="b75bf-625">Microsoft Universal Print は、2021 年 3 月 1 日から、選択された Microsoft 365 スイート内での取引に利用したり、スタンドアロン アドオンとして利用したりできるようになります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-625">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="b75bf-626">対象</span><span class="sxs-lookup"><span data-stu-id="b75bf-626">Impacted audience</span></span>

<span data-ttu-id="b75bf-627">クラウド ソリューション プロバイダー (CSP) プログラムを通じて取引を行う、すべてのパートナー様</span><span class="sxs-lookup"><span data-stu-id="b75bf-627">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="b75bf-628">詳細</span><span class="sxs-lookup"><span data-stu-id="b75bf-628">Details</span></span>

<span data-ttu-id="b75bf-629">[Universal Print](https://aka.ms/universalprint) は、オンプレミスのプリント サーバーを不要にし、Windows デバイスから Azure 登録済みプリンターに出力できるようにする Microsoft 365 プリント サービスです。</span><span class="sxs-lookup"><span data-stu-id="b75bf-629">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="b75bf-630">2021 年 3 月 1 日から取引に利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="b75bf-630">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="b75bf-631">ワーカーは、ドライバー不要の印刷、合理化されたロケーションベースのプリンター検出、学習曲線不要の直感的な印刷操作などの利点が得られます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-631">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="b75bf-632">Azure Active Directory (Azure AD) に参加しているデバイスは、既存の Azure AD 資格情報を使用して安全に印刷します。</span><span class="sxs-lookup"><span data-stu-id="b75bf-632">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="b75bf-633">管理者は Azure portal を使用して印刷を管理し、Universal Print のネイティブ サポートを使用してプリンターを簡単に接続できます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-633">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="b75bf-634">Universal Print は、Universal Print コネクタ ソフトウェアを使用して、互換性のないプリンターで展開できます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-634">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="b75bf-635">Universal Print はサービス開始時に、Windows E3、A3、E5、A5 と Microsoft 365 BP、F3、E3、A3、E5、A5 に追加されます。</span><span class="sxs-lookup"><span data-stu-id="b75bf-635">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="b75bf-636">**特典の詳細**</span><span class="sxs-lookup"><span data-stu-id="b75bf-636">**Offer details**</span></span>

<span data-ttu-id="b75bf-637">プラン名は、価格表プレビューとは若干異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-637">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="b75bf-638">プラン名</span><span class="sxs-lookup"><span data-stu-id="b75bf-638">Offer name</span></span> | <span data-ttu-id="b75bf-639">プラン ID</span><span class="sxs-lookup"><span data-stu-id="b75bf-639">Offer ID</span></span> | <span data-ttu-id="b75bf-640">マテリアル ID</span><span class="sxs-lookup"><span data-stu-id="b75bf-640">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="b75bf-641">Universal Print ボリューム アドオン (500 ジョブ) - Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b75bf-641">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="b75bf-642">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="b75bf-642">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="b75bf-643">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="b75bf-643">9BI-00004</span></span>   |
| <span data-ttu-id="b75bf-644">教職員用 Universal Print ボリューム アドオン (500 ジョブ) - Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b75bf-644">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="b75bf-645">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="b75bf-645">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="b75bf-646">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="b75bf-646">9BK-00004</span></span>   |
| <span data-ttu-id="b75bf-647">Universal Print ボリューム アドオン (500 ジョブ) - Windows</span><span class="sxs-lookup"><span data-stu-id="b75bf-647">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="b75bf-648">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="b75bf-648">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="b75bf-649">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="b75bf-649">9BI-00002</span></span>   |
| <span data-ttu-id="b75bf-650">教職員用 Universal Print ボリューム アドオン (500 ジョブ) - Windows</span><span class="sxs-lookup"><span data-stu-id="b75bf-650">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="b75bf-651">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="b75bf-651">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="b75bf-652">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="b75bf-652">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="b75bf-653">次のステップ</span><span class="sxs-lookup"><span data-stu-id="b75bf-653">Next steps</span></span>

<span data-ttu-id="b75bf-654">価格表と [Universal Print の概要](/universal-print/fundamentals/universal-print-whatis)についてご確認ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-654">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="b75bf-655">この情報を組織内の適切なすべての担当者に共有してください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-655">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="b75bf-656">ご質問がある場合は、</span><span class="sxs-lookup"><span data-stu-id="b75bf-656">Questions?</span></span>

<span data-ttu-id="b75bf-657">これらのプランについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="b75bf-657">For any questions about these offers, check your relevant Yammer communities.</span></span>
