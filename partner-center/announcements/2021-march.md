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
ms.openlocfilehash: 12954a5f7eafb138794de879a41026ef54c65da7
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374391"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="6f270-103">2021 年 3 月のお知らせ</span><span class="sxs-lookup"><span data-stu-id="6f270-103">March 2021 announcements</span></span>

<span data-ttu-id="6f270-104">このページでは、2021 年 3 月の Microsoft パートナー センターのお知らせについて説明します。</span><span class="sxs-lookup"><span data-stu-id="6f270-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a><span data-ttu-id="6f270-105">更新された CSP 顧客アドレス検証 API がテスト用に利用できるようになりました</span><span class="sxs-lookup"><span data-stu-id="6f270-105">Updated CSP customer address validation API now available for testing</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-106">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-106">Categories</span></span>

- <span data-ttu-id="6f270-107">日付 : 2021 年 3 月 31 日</span><span class="sxs-lookup"><span data-stu-id="6f270-107">Date: 2021-03-31</span></span>
- <span data-ttu-id="6f270-108">機能</span><span class="sxs-lookup"><span data-stu-id="6f270-108">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6f270-109">まとめ</span><span class="sxs-lookup"><span data-stu-id="6f270-109">Summary</span></span>

<span data-ttu-id="6f270-110">パートナーと顧客が信頼に基づいてビジネスを遂行できるようにするためのコミットメントの一環として、Microsoft では世界中のパートナーに対して ValidateAddress API への変更をテストすることをお勧めしています。</span><span class="sxs-lookup"><span data-stu-id="6f270-110">As part of our commitment to help partners and customers run their business based on trust, we will be inviting partners worldwide to test the changes to the ValidateAddress API.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-111">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-111">Impacted audience</span></span>

<span data-ttu-id="6f270-112">顧客の住所の詳細を新規作成または既存のものを更新する、すべての CSP 直接請求パートナーと間接プロバイダー</span><span class="sxs-lookup"><span data-stu-id="6f270-112">All CSP direct bill partners and indirect providers who create new or update existing customer address details</span></span>

### <a name="details"></a><span data-ttu-id="6f270-113">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-113">Details</span></span>

<span data-ttu-id="6f270-114">Microsoft の基盤は信頼です。</span><span class="sxs-lookup"><span data-stu-id="6f270-114">Microsoft runs on trust.</span></span> <span data-ttu-id="6f270-115">Microsoft は、CSP プログラムでの顧客サブスクリプションの取引について顧客の住所検証を送信する、法令に準拠した安全な手段の提供に努めています。</span><span class="sxs-lookup"><span data-stu-id="6f270-115">We’re committed to providing a compliant, safe, and secure method of submitting customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="6f270-116">2021 年 3 月 31 日現在、ValidateAddress API に変更が加えられており、2021 年 6 月に正式に変更される前にテストすることをお勧めしています。</span><span class="sxs-lookup"><span data-stu-id="6f270-116">Today, March 31, 2021, we have introduced changes to the ValidateAddress API that we’d like to invite you to test, prior to going live with the changes in June 2021.</span></span> 

<span data-ttu-id="6f270-117">これらの変更は、ValidateAddress API にのみ影響を与えることにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-117">Note that these changes affect the ValidateAddress API only.</span></span> <span data-ttu-id="6f270-118">CreateCustomer および UpdateBillingProfile API には影響がありません。</span><span class="sxs-lookup"><span data-stu-id="6f270-118">CreateCustomer and UpdateBillingProfile APIs are not affected.</span></span>

<span data-ttu-id="6f270-119">応答では、次のいずれかのステータス メッセージが返されます。</span><span class="sxs-lookup"><span data-stu-id="6f270-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="6f270-120">状態</span><span class="sxs-lookup"><span data-stu-id="6f270-120">Status</span></span> | <span data-ttu-id="6f270-121">説明</span><span class="sxs-lookup"><span data-stu-id="6f270-121">Description</span></span> | <span data-ttu-id="6f270-122">返される住所候補の数</span><span class="sxs-lookup"><span data-stu-id="6f270-122">Number of suggested addresses returned</span></span> |
|----------|-------------|-------------------|
| <span data-ttu-id="6f270-123">VerifiedShippable</span><span class="sxs-lookup"><span data-stu-id="6f270-123">VerifiedShippable</span></span> | <span data-ttu-id="6f270-124">住所が確認され、出荷可能です。</span><span class="sxs-lookup"><span data-stu-id="6f270-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="6f270-125">Single</span><span class="sxs-lookup"><span data-stu-id="6f270-125">Single</span></span> |
| <span data-ttu-id="6f270-126">Verified</span><span class="sxs-lookup"><span data-stu-id="6f270-126">Verified</span></span> | <span data-ttu-id="6f270-127">住所が確認されました。</span><span class="sxs-lookup"><span data-stu-id="6f270-127">Address is verified.</span></span> | <span data-ttu-id="6f270-128">Single</span><span class="sxs-lookup"><span data-stu-id="6f270-128">Single</span></span> |
| <span data-ttu-id="6f270-129">InteractionRequired</span><span class="sxs-lookup"><span data-stu-id="6f270-129">InteractionRequired</span></span> | <span data-ttu-id="6f270-130">住所候補は大幅に変更されており、ユーザーの確認が必要です。</span><span class="sxs-lookup"><span data-stu-id="6f270-130">Suggested address(es) has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="6f270-131">Single</span><span class="sxs-lookup"><span data-stu-id="6f270-131">Single</span></span> |
| <span data-ttu-id="6f270-132">StreetPartial</span><span class="sxs-lookup"><span data-stu-id="6f270-132">StreetPartial</span></span> | <span data-ttu-id="6f270-133">住所の番地が部分的であるため、さらに情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="6f270-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="6f270-134">複数 (最大 3)</span><span class="sxs-lookup"><span data-stu-id="6f270-134">Multiple—maximum of three</span></span>|
| <span data-ttu-id="6f270-135">PremisesPartial</span><span class="sxs-lookup"><span data-stu-id="6f270-135">PremisesPartial</span></span> | <span data-ttu-id="6f270-136">指定された建物 (ビル番号、部屋番号など) が部分的であるため、さらに情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="6f270-136">The given premises (building number, suite number, etc.) is partial and needs more info.</span></span> | <span data-ttu-id="6f270-137">複数 (最大 3)</span><span class="sxs-lookup"><span data-stu-id="6f270-137">Multiple—maximum of three</span></span> |
| <span data-ttu-id="6f270-138">複数</span><span class="sxs-lookup"><span data-stu-id="6f270-138">Multiple</span></span> | <span data-ttu-id="6f270-139">住所の複数の部分が部分的です (StreetPartial と PremisesPartial も含む可能性があります)。</span><span class="sxs-lookup"><span data-stu-id="6f270-139">There are multiple fields that are partial in the address (potentially also including StreetPartial and PremisesPartial).</span></span> | <span data-ttu-id="6f270-140">複数 (最大 3)</span><span class="sxs-lookup"><span data-stu-id="6f270-140">Multiple—maximum of three</span></span> |
| <span data-ttu-id="6f270-141">なし</span><span class="sxs-lookup"><span data-stu-id="6f270-141">None</span></span> | <span data-ttu-id="6f270-142">住所が正しくありません。</span><span class="sxs-lookup"><span data-stu-id="6f270-142">Address is incorrect.</span></span> | <span data-ttu-id="6f270-143">なし</span><span class="sxs-lookup"><span data-stu-id="6f270-143">None</span></span> |
| <span data-ttu-id="6f270-144">NotValidated</span><span class="sxs-lookup"><span data-stu-id="6f270-144">NotValidated</span></span> | <span data-ttu-id="6f270-145">住所は、検証プロセスを通じて送信できませんでした。</span><span class="sxs-lookup"><span data-stu-id="6f270-145">Address was not able to be sent through the validation process.</span></span>  | <span data-ttu-id="6f270-146">なし</span><span class="sxs-lookup"><span data-stu-id="6f270-146">None</span></span> |

<span data-ttu-id="6f270-147">住所を送信し、ValidateAddress API によって検証されると、次の応答スキーマが返されます。</span><span class="sxs-lookup"><span data-stu-id="6f270-147">Once an address has been submitted to be validated via the ValidateAddress API, the following response schema will be returned:</span></span>

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

<span data-ttu-id="6f270-148">サンプルの応答をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-148">Take a look at this sample response.</span></span> <span data-ttu-id="6f270-149">米国では、郵便番号に 5 桁の数字のみを入力した場合、応答では郵便番号の行に追加の 4 桁のサフィックスが返されることに注目してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-149">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

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

### <a name="next-steps"></a><span data-ttu-id="6f270-150">次のステップ</span><span class="sxs-lookup"><span data-stu-id="6f270-150">Next steps</span></span>

- <span data-ttu-id="6f270-151">テスト実行に参加して更新の準備を開始できるよう、サンドボックスのテナント ID を Microsoft の領域の専門家 (SME) Ali Khaki にお知らせください。</span><span class="sxs-lookup"><span data-stu-id="6f270-151">Share your sandbox tenant ID with our subject matter expert (SME), Ali Khaki, to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="6f270-152">コントロール パネル ベンダー (CPV) ソリューションを使用している場合は、CPV とご相談ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-152">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="6f270-153">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="6f270-153">Questions?</span></span>

<span data-ttu-id="6f270-154">ご質問がある場合や、Microsoft との連携でサポートが必要な場合は、パートナー サポートの Yammer グループにお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="6f270-154">If you have any questions or need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="6f270-155">新しい Exchange 管理センター (EAC) エクスペリエンス</span><span class="sxs-lookup"><span data-stu-id="6f270-155">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-156">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-156">Categories</span></span>

- <span data-ttu-id="6f270-157">日付: 2021 年 3 月 29 日</span><span class="sxs-lookup"><span data-stu-id="6f270-157">Date: 2021-03-29</span></span>
- <span data-ttu-id="6f270-158">機能</span><span class="sxs-lookup"><span data-stu-id="6f270-158">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6f270-159">まとめ</span><span class="sxs-lookup"><span data-stu-id="6f270-159">Summary</span></span>

<span data-ttu-id="6f270-160">2021 年 4 月 27 日以降、Exchange 管理センター (EAC) では、ユーザーの日々の効率を向上させる新しいエクスペリエンスがロールアウトされます。</span><span class="sxs-lookup"><span data-stu-id="6f270-160">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-161">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-161">Impacted audience</span></span>

<span data-ttu-id="6f270-162">パートナー センター経由で Exchange にアクセスする代理管理者</span><span class="sxs-lookup"><span data-stu-id="6f270-162">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="6f270-163">説明</span><span class="sxs-lookup"><span data-stu-id="6f270-163">Details</span></span>

<span data-ttu-id="6f270-164">2021 年 4 月 27 日以降、パートナー センターを通じて Exchange に移動するパートナーは、新しい EAC にリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="6f270-164">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="6f270-165">この新しいエクスペリエンスは現在、プレビューとして提供されており、管理者は従来の EAC で右上隅にあるトグルを選択すれば、このエクスペリエンスをアクティブにできます。</span><span class="sxs-lookup"><span data-stu-id="6f270-165">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="6f270-166">また、すべてのページに表示される [今すぐ試す] バナーを選択して、新しい EAC に移動することもできます。</span><span class="sxs-lookup"><span data-stu-id="6f270-166">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="6f270-167">新しい EAC には次のような利点があります。</span><span class="sxs-lookup"><span data-stu-id="6f270-167">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="6f270-168">メール フロー関連の問題について、分析情報、レポート、アラートのメカニズムが追加されました。</span><span class="sxs-lookup"><span data-stu-id="6f270-168">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="6f270-169">ダッシュボードをカスタマイズして、生産性を向上させることができます。</span><span class="sxs-lookup"><span data-stu-id="6f270-169">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="6f270-170">新しいエクスペリエンスを簡単に確認するには、新しい EAC エクスペリエンスの「**トレーニングとガイド**」セクションでビデオを参照できます。</span><span class="sxs-lookup"><span data-stu-id="6f270-170">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="6f270-171">新しいポータルを最適に使用する方法の概要について理解できます。</span><span class="sxs-lookup"><span data-stu-id="6f270-171">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="6f270-172">この変更により、従来の EAC エクスペリエンスが非推奨になることはありません。</span><span class="sxs-lookup"><span data-stu-id="6f270-172">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="6f270-173">パートナーには、変更の実施に先立ち、十分前もって通知されます。</span><span class="sxs-lookup"><span data-stu-id="6f270-173">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6f270-174">次のステップ</span><span class="sxs-lookup"><span data-stu-id="6f270-174">Next steps</span></span>

- <span data-ttu-id="6f270-175">[このトピックに関するリソース](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)を参照して、新しいエクスペリエンスのスクリーンショットを確認することができます。</span><span class="sxs-lookup"><span data-stu-id="6f270-175">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="6f270-176">この情報を組織内の適切な関係者に共有してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-176">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="6f270-177">疑問がある場合</span><span class="sxs-lookup"><span data-stu-id="6f270-177">Questions?</span></span>

<span data-ttu-id="6f270-178">これらの変更についてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-178">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="6f270-179">Microsoft Operations: 製品発表予定表の概要</span><span class="sxs-lookup"><span data-stu-id="6f270-179">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-180">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-180">Categories</span></span>

- <span data-ttu-id="6f270-181">日付: 2021 年 3 月 25 日</span><span class="sxs-lookup"><span data-stu-id="6f270-181">Date: 2021-03-25</span></span>
- <span data-ttu-id="6f270-182">製品サービス | モダン ワークプレース</span><span class="sxs-lookup"><span data-stu-id="6f270-182">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="6f270-183">まとめ</span><span class="sxs-lookup"><span data-stu-id="6f270-183">Summary</span></span>

<span data-ttu-id="6f270-184">パートナーからのフィードバックにお応えして、Microsoft Operations では製品発表に関するコミュニケーションを合理化します。</span><span class="sxs-lookup"><span data-stu-id="6f270-184">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-185">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-185">Impacted audience</span></span>

<span data-ttu-id="6f270-186">クラウド ソリューション プロバイダー (CSP) パートナー様</span><span class="sxs-lookup"><span data-stu-id="6f270-186">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="6f270-187">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-187">Details</span></span>

<span data-ttu-id="6f270-188">Microsoft では、パートナー エクスペリエンスの継続的な改善に取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="6f270-188">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="6f270-189">Microsoft からの情報が多すぎるというフィードバックが寄せられています。これには、製品の発表に関する重複したお知らせも含まれます。</span><span class="sxs-lookup"><span data-stu-id="6f270-189">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="6f270-190">Microsoft では、皆様からのフィードバックにお応えして、新規および既存のオファーについて製品発表の準備エクスペリエンスを合理化しました。</span><span class="sxs-lookup"><span data-stu-id="6f270-190">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="6f270-191">現在では、月に 1 回の製品発表ビューを Operations Readiness リソース ギャラリーに提供するようになりました。</span><span class="sxs-lookup"><span data-stu-id="6f270-191">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="6f270-192">この月単位の[製品発表予定表ビュー](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)は、Operations Readiness リソース ギャラリーとパートナー センターのお知らせに含まれる個別の製品発表情報に置き換わるものとなります。</span><span class="sxs-lookup"><span data-stu-id="6f270-192">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="6f270-193">また、[コミュニティ コレクション](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)、[予定表ビュー](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)、[CSP ニュースレター](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)から、この[製品発表予定表](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)にアクセスすることもできます。</span><span class="sxs-lookup"><span data-stu-id="6f270-193">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="6f270-194">各月の製品発表予定表が公開されたら、Operations Readiness リソース ギャラリーのお知らせで皆様に通知します。</span><span class="sxs-lookup"><span data-stu-id="6f270-194">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="6f270-195">新規および既存のオファーに関する情報は、今後も、価格一覧のプレビューと価格一覧の変更ログ、製品のブログ、ライセンス ガイド、製品マーケティング ページで確認できます。</span><span class="sxs-lookup"><span data-stu-id="6f270-195">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="6f270-196">この変更は、次の製品に関する発表に適用されます。</span><span class="sxs-lookup"><span data-stu-id="6f270-196">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="6f270-197">オンプレミスの Dynamics</span><span class="sxs-lookup"><span data-stu-id="6f270-197">Dynamics on-premises</span></span>
- <span data-ttu-id="6f270-198">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6f270-198">Microsoft 365</span></span>
- <span data-ttu-id="6f270-199">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="6f270-199">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="6f270-200">Windows</span><span class="sxs-lookup"><span data-stu-id="6f270-200">Windows</span></span>
- <span data-ttu-id="6f270-201">サーバー</span><span class="sxs-lookup"><span data-stu-id="6f270-201">Server</span></span>  
- <span data-ttu-id="6f270-202">ツール</span><span class="sxs-lookup"><span data-stu-id="6f270-202">Tools</span></span>
- <span data-ttu-id="6f270-203">Teams と Telco</span><span class="sxs-lookup"><span data-stu-id="6f270-203">Teams and Telco</span></span>

<span data-ttu-id="6f270-204">Operations Readiness の詳細を必要とする製品の発表については、引き続き特定のお知らせをお送りします。</span><span class="sxs-lookup"><span data-stu-id="6f270-204">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6f270-205">次のステップ</span><span class="sxs-lookup"><span data-stu-id="6f270-205">Next steps</span></span>

<span data-ttu-id="6f270-206">このトピックに関するリソースを確認し、この情報を組織内の該当する関係者と共有してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-206">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="6f270-207">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="6f270-207">Questions?</span></span>

<span data-ttu-id="6f270-208">これらのオファーについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-208">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="6f270-209">CSP のお客様のオンボード要件の変更</span><span class="sxs-lookup"><span data-stu-id="6f270-209">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-210">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-210">Categories</span></span>

- <span data-ttu-id="6f270-211">日付: 2021 年 3 月 25 日</span><span class="sxs-lookup"><span data-stu-id="6f270-211">Date: 2021-03-25</span></span>
- <span data-ttu-id="6f270-212">機能</span><span class="sxs-lookup"><span data-stu-id="6f270-212">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6f270-213">まとめ</span><span class="sxs-lookup"><span data-stu-id="6f270-213">Summary</span></span>

<span data-ttu-id="6f270-214">パートナーと顧客が信頼に基づいて取引できるように支援する責任の一環として、Microsoft では 2021 年 3 月 25 日から、追加の顧客情報を要求いたします。</span><span class="sxs-lookup"><span data-stu-id="6f270-214">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-215">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-215">Impacted audience</span></span>

<span data-ttu-id="6f270-216">次のセクションに記載されている国に新規または既存の顧客がいるクラウド ソリューション プロバイダー (CSP) 直接請求パートナーおよび間接プロバイダー</span><span class="sxs-lookup"><span data-stu-id="6f270-216">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="6f270-217">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-217">Details</span></span>

<span data-ttu-id="6f270-218">Microsoft の基盤は信頼です。</span><span class="sxs-lookup"><span data-stu-id="6f270-218">Microsoft runs on trust.</span></span> <span data-ttu-id="6f270-219">Microsoft は、CSP プログラムでの顧客サブスクリプションの取引について、顧客検証のための法令に準拠した安全な手段の提供に努めています。</span><span class="sxs-lookup"><span data-stu-id="6f270-219">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="6f270-220">2021 年 3 月 25 日に、パートナー センター API とユーザー インターフェイス (UI) の拡張機能を導入する予定です。これは、以下の条件の両方を満たすパートナーに影響します。</span><span class="sxs-lookup"><span data-stu-id="6f270-220">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="6f270-221">Microsoft の間に直接請求関係があるパートナー (つまり、直接請求パートナーまたは間接プロバイダーのいずれかであるパートナー)</span><span class="sxs-lookup"><span data-stu-id="6f270-221">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="6f270-222">パートナーは、次の国の新規または既存の顧客と取引があります:</span><span class="sxs-lookup"><span data-stu-id="6f270-222">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="6f270-223">タイ</span><span class="sxs-lookup"><span data-stu-id="6f270-223">Thailand</span></span>
    - <span data-ttu-id="6f270-224">ベトナム</span><span class="sxs-lookup"><span data-stu-id="6f270-224">Vietnam</span></span>
    - <span data-ttu-id="6f270-225">トルコ</span><span class="sxs-lookup"><span data-stu-id="6f270-225">Turkey</span></span>
    - <span data-ttu-id="6f270-226">ポーランド</span><span class="sxs-lookup"><span data-stu-id="6f270-226">Poland</span></span>
    - <span data-ttu-id="6f270-227">南アフリカ</span><span class="sxs-lookup"><span data-stu-id="6f270-227">South Africa</span></span>
    - <span data-ttu-id="6f270-228">インド</span><span class="sxs-lookup"><span data-stu-id="6f270-228">India</span></span>
    - <span data-ttu-id="6f270-229">ブラジル</span><span class="sxs-lookup"><span data-stu-id="6f270-229">Brazil</span></span>
    - <span data-ttu-id="6f270-230">イラク</span><span class="sxs-lookup"><span data-stu-id="6f270-230">Iraq</span></span>
    - <span data-ttu-id="6f270-231">ミャンマー</span><span class="sxs-lookup"><span data-stu-id="6f270-231">Myanmar</span></span>
    - <span data-ttu-id="6f270-232">南スーダン</span><span class="sxs-lookup"><span data-stu-id="6f270-232">South Sudan</span></span>
    - <span data-ttu-id="6f270-233">サウジアラビア</span><span class="sxs-lookup"><span data-stu-id="6f270-233">Saudi Arabia</span></span>
    - <span data-ttu-id="6f270-234">アラブ首長国連邦</span><span class="sxs-lookup"><span data-stu-id="6f270-234">United Arab Emirates</span></span>
    - <span data-ttu-id="6f270-235">ベネズエラ</span><span class="sxs-lookup"><span data-stu-id="6f270-235">Venezuela</span></span>

<span data-ttu-id="6f270-236">条件を満たすパートナーは、新しい顧客をオンボードするとき、または既存の顧客の詳細を変更するときに、顧客の **会社登録 ID** (顧客の **組織 INN** とも呼ばれます) と **電話番号** を提出する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6f270-236">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="6f270-237">また、これらのパートナーは、必要に応じて、顧客の **ミドル ネーム** を入力することができます。</span><span class="sxs-lookup"><span data-stu-id="6f270-237">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="6f270-238">会社登録 ID を追加する場合は、顧客の個人 ID ではなく、業務用の税 ID を使用する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-238">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="6f270-239">以下の国で新規または既存の顧客との取引を行っているパートナーは、先行する 2020 年 11 月のリリースで既にオンボードされています。</span><span class="sxs-lookup"><span data-stu-id="6f270-239">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="6f270-240">アルメニア</span><span class="sxs-lookup"><span data-stu-id="6f270-240">Armenia</span></span>
- <span data-ttu-id="6f270-241">アゼルバイジャン</span><span class="sxs-lookup"><span data-stu-id="6f270-241">Azerbaijan</span></span>
- <span data-ttu-id="6f270-242">ベラルーシ</span><span class="sxs-lookup"><span data-stu-id="6f270-242">Belarus</span></span>
- <span data-ttu-id="6f270-243">ハンガリー</span><span class="sxs-lookup"><span data-stu-id="6f270-243">Hungary</span></span>
- <span data-ttu-id="6f270-244">カザフスタン</span><span class="sxs-lookup"><span data-stu-id="6f270-244">Kazakhstan</span></span>
- <span data-ttu-id="6f270-245">キルギスタン</span><span class="sxs-lookup"><span data-stu-id="6f270-245">Kyrgyzstan</span></span>
- <span data-ttu-id="6f270-246">モルドバ</span><span class="sxs-lookup"><span data-stu-id="6f270-246">Moldova</span></span>
- <span data-ttu-id="6f270-247">ロシア</span><span class="sxs-lookup"><span data-stu-id="6f270-247">Russia</span></span>
- <span data-ttu-id="6f270-248">タジキスタン</span><span class="sxs-lookup"><span data-stu-id="6f270-248">Tajikistan</span></span>
- <span data-ttu-id="6f270-249">ウクライナ</span><span class="sxs-lookup"><span data-stu-id="6f270-249">Ukraine</span></span>
- <span data-ttu-id="6f270-250">ウズベキスタン</span><span class="sxs-lookup"><span data-stu-id="6f270-250">Uzbekistan</span></span>

<span data-ttu-id="6f270-251">その他の地域の顧客と提携しているパートナーは、2021 年 3 月 25 日に、顧客の **会社登録 ID**、**電話番号**、**ミドル ネーム** を詳細情報として必要に応じて入力できるようになります。</span><span class="sxs-lookup"><span data-stu-id="6f270-251">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6f270-252">次のステップ</span><span class="sxs-lookup"><span data-stu-id="6f270-252">Next steps</span></span>

- <span data-ttu-id="6f270-253">詳細なガイダンスについては、[専用のパートナー コレクション](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)でテクニカル ドキュメントとよく寄せられる質問を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-253">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="6f270-254">Partner Center API と Web ユーザー エクスペリエンスを使用して、変更を組み込む準備をしてください。</span><span class="sxs-lookup"><span data-stu-id="6f270-254">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="6f270-255">API または SDK はテストに使用できます。</span><span class="sxs-lookup"><span data-stu-id="6f270-255">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="6f270-256">新しい顧客をオンボードする場合や、既存の顧客の詳細情報を変更する場合は、必ず追加データを提出してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-256">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="6f270-257">コントロール パネル ベンダー (CPV) ソリューションを使用している場合は、CPV とご相談ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-257">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="6f270-258">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="6f270-258">Questions?</span></span>

<span data-ttu-id="6f270-259">有効な識別子 (INN または TIN とも呼ばれます) に関するご質問がある場合は、税務顧問または現地の税務署にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="6f270-259">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="6f270-260">Microsoft では、税務に関するガイダンスを提供できません。</span><span class="sxs-lookup"><span data-stu-id="6f270-260">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="6f270-261">Microsoft との連携でサポートが必要な場合は、[サービス要求を開いてください](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)。</span><span class="sxs-lookup"><span data-stu-id="6f270-261">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="6f270-262">2021 年 3 月 1 日に永続的ソフトウェアの価格表に加えられた修正</span><span class="sxs-lookup"><span data-stu-id="6f270-262">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-263">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-263">Categories</span></span>

- <span data-ttu-id="6f270-264">日付: 2021 年 3 月 23 日</span><span class="sxs-lookup"><span data-stu-id="6f270-264">Date: 2021-03-23</span></span>
- <span data-ttu-id="6f270-265">製品サービス/市場</span><span class="sxs-lookup"><span data-stu-id="6f270-265">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-266">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-266">Impacted audience</span></span>

<span data-ttu-id="6f270-267">クラウド ソリューション プロバイダー プログラムで永続的なソフトウェアの取引を行っている間接プロバイダーおよび直接請求パートナー</span><span class="sxs-lookup"><span data-stu-id="6f270-267">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="6f270-268">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-268">Details</span></span>

<span data-ttu-id="6f270-269">2021 年 3 月 1 日に公開された永続的ソフトウェアの価格表には、掲載されるべきではなかった市場が含まれていました。</span><span class="sxs-lookup"><span data-stu-id="6f270-269">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="6f270-270">修正内容を含めた永続的ソフトウェアの価格表が、2021 年 3 月 17 日に更新されました。</span><span class="sxs-lookup"><span data-stu-id="6f270-270">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="6f270-271">これらの修正は、次の場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="6f270-271">These corrections were only applicable to:</span></span>

- <span data-ttu-id="6f270-272">製品 ID: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="6f270-272">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="6f270-273">製品名: Microsoft 365 Business の Windows 10 Home から Pro へのアップグレード</span><span class="sxs-lookup"><span data-stu-id="6f270-273">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="6f270-274">削除された、またはサポートされていない市場: AE、AF、AL、AM、AO、BA、BB、BD、BH、BM、BN、BO、BR、BS、BW、BY、BZ、CI、CL、CM、CO、CR、CW、DO、DZ、EC、EG、ET、FJ、FO、GE、GH、GT、HN、IL、IN、IQ、JM、JO、KE、KG、KN、KW、KY、KZ、LB、LK、LY、MA、MC、MD、ME、MN、MO、MU、NA、NG、NI、NP、OM、PA、PE、PH、PK、PR、PY、QA、RS、RU、RW、SG、SN、SV、TH、TJ、TM、TN、TT、TZ、UA、UG、UY、UZ、VE、VN、YE、ZM、ZW</span><span class="sxs-lookup"><span data-stu-id="6f270-274">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="6f270-275">これらの変更は、上記の製品にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="6f270-275">These changes only apply to the above product.</span></span> <span data-ttu-id="6f270-276">他の製品には修正がありませんでした。</span><span class="sxs-lookup"><span data-stu-id="6f270-276">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="6f270-277">次の手順とリソース</span><span class="sxs-lookup"><span data-stu-id="6f270-277">Next steps and resources</span></span>

- <span data-ttu-id="6f270-278">永続的ソフトウェアの取引を行うパートナーは、最新の永続的ソフトウェアの価格表をダウンロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="6f270-278">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="6f270-279">国を指す 2 文字の省略形のわかりやすいマッピングについては、[地域と国のコード](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-279">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><span data-ttu-id="6f270-280"><a name="13">.NET Standard (v1.17.0) の SDK リリース</a></span><span class="sxs-lookup"><span data-stu-id="6f270-280"><a name="13"></a> SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-281">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-281">Categories</span></span>

- <span data-ttu-id="6f270-282">日付: 2021 年 3 月 23 日</span><span class="sxs-lookup"><span data-stu-id="6f270-282">Date: 2021-03-23</span></span>

- <span data-ttu-id="6f270-283">機能</span><span class="sxs-lookup"><span data-stu-id="6f270-283">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="6f270-284">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-284">Impacted audience</span></span>

<span data-ttu-id="6f270-285">パートナー センターの .NET SDK を使用している、CSP プログラムに参加している直接請求パートナーと間接プロバイダー。</span><span class="sxs-lookup"><span data-stu-id="6f270-285">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="6f270-286">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-286">Details</span></span>

<span data-ttu-id="6f270-287">2020 年 3 月 23 日より、パートナーは、更新されたパートナー センター SDK [GitHub の一般向けサンプル](https://github.com/Microsoft/Partner-Center-DotNet-Samples)と共に、[MicrosoftPartnerCenter.NETSDK (NuGet ギャラリー | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0) バージョンのダウンロードを開始できます。</span><span class="sxs-lookup"><span data-stu-id="6f270-287">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="6f270-288">このバージョンには、以下のメソッドに対する更新が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6f270-288">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="6f270-289">更新された監査: 新しい操作の種類</span><span class="sxs-lookup"><span data-stu-id="6f270-289">Audit Updated: New operation types</span></span>

<span data-ttu-id="6f270-290">顧客が DAP を承認および終了した日時を把握するための、新しい[操作の種類](https://docs.microsoft.com/partner-center/develop/auditing-resources)が追加されました。</span><span class="sxs-lookup"><span data-stu-id="6f270-290">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="6f270-291">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="6f270-291">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="6f270-292">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="6f270-292">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="6f270-293">更新された監査: 新しいリソースと操作の種類</span><span class="sxs-lookup"><span data-stu-id="6f270-293">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="6f270-294">顧客ディレクトリ ロールのシナリオをサポートするための、新しい[リソースと操作の種類](https://docs.microsoft.com/partner-center/develop/auditing-resources)が追加されました。</span><span class="sxs-lookup"><span data-stu-id="6f270-294">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="6f270-295">新しいリソースの種類 "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="6f270-295">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="6f270-296">操作の種類 "AddUserMember" と "RemoveUserMember"</span><span class="sxs-lookup"><span data-stu-id="6f270-296">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="6f270-297">顧客アカウントに対する SDK の更新</span><span class="sxs-lookup"><span data-stu-id="6f270-297">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="6f270-298">GET のサポート /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span><span class="sxs-lookup"><span data-stu-id="6f270-298">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="6f270-299">GET /customers/{customer-tenant-id}/qualifications</span><span class="sxs-lookup"><span data-stu-id="6f270-299">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="6f270-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span><span class="sxs-lookup"><span data-stu-id="6f270-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="6f270-301">追加の変更</span><span class="sxs-lookup"><span data-stu-id="6f270-301">Additional changes</span></span>

<span data-ttu-id="6f270-302">新しいコマースの一部として導入された次の変更は、現在、M365 または D365 の新しいコマース エクスペリエンスのテクニカル プレビューに含まれているパートナーのみが、招待に基づいて利用できます。</span><span class="sxs-lookup"><span data-stu-id="6f270-302">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="6f270-303">新しいコマースのテクニカル プレビューに含まれていないパートナーは、影響を受けないようにして、下位互換性を確保する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6f270-303">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="6f270-304">カタログの変更:</span><span class="sxs-lookup"><span data-stu-id="6f270-304">Catalog Changes:</span></span>

  - <span data-ttu-id="6f270-305">GET /products/{product-id}/skus/{sku-id}</span><span class="sxs-lookup"><span data-stu-id="6f270-305">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="6f270-306">購入および管理:</span><span class="sxs-lookup"><span data-stu-id="6f270-306">Purchase and Manage:</span></span>
  - <span data-ttu-id="6f270-307">GET /customers/{customerId}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="6f270-307">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="6f270-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="6f270-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="6f270-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="6f270-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="6f270-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="6f270-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="6f270-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="6f270-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="6f270-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="6f270-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="6f270-313">次の手順</span><span class="sxs-lookup"><span data-stu-id="6f270-313">Next Steps</span></span>

- <span data-ttu-id="6f270-314">最新バージョン [MicrosoftPartnerCenter.NETSDK (NuGet ギャラリー | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0) をダウンロードする</span><span class="sxs-lookup"><span data-stu-id="6f270-314">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="6f270-315">[GitHub サンプル](https://github.com/Microsoft/Partner-Center-DotNet-Samples)をダウンロードして確認する</span><span class="sxs-lookup"><span data-stu-id="6f270-315">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="6f270-316">CSP コマーシャル マーケットプレース プランと、対象となるプランの FY21 CSP インセンティブ</span><span class="sxs-lookup"><span data-stu-id="6f270-316">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-317">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-317">Categories</span></span>

- <span data-ttu-id="6f270-318">日付: 2021 年 3 月 18 日</span><span class="sxs-lookup"><span data-stu-id="6f270-318">Date: 2021-03-18</span></span>
- <span data-ttu-id="6f270-319">機能</span><span class="sxs-lookup"><span data-stu-id="6f270-319">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-320">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-320">Impacted audience</span></span>

<span data-ttu-id="6f270-321">クラウド ソリューション プロバイダー プログラムにおける間接プロバイダーと直接請求パートナー</span><span class="sxs-lookup"><span data-stu-id="6f270-321">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="6f270-322">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-322">Details</span></span>

<span data-ttu-id="6f270-323">クラウド ソリューション プロバイダー プログラムにおける間接プロバイダーおよび直接請求パートナーは、サードパーティのプランを販売できます。また、パートナー センターまたは Azure portal でトランザクションが実行された、対象となるサードパーティのプランごとにリベート インセンティブを獲得することができます。</span><span class="sxs-lookup"><span data-stu-id="6f270-323">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="6f270-324">インセンティブは、対象となるプランの請求済み売上に対するリベートの形式であり、**2021 年 6 月 30 日まで利用可能** です。</span><span class="sxs-lookup"><span data-stu-id="6f270-324">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="6f270-325">この CSP コマーシャル マーケットプレース プランのインセンティブについて、以下で引き続き学習してください。顧客に今すぐ連絡して、継続的な成功とデジタル変革を実現するための適切なプランを特定してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-325">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="6f270-326">Microsoft では、独立系ソフトウェア ベンダー (ISV) と提携して、Microsoft 顧客向けの最新の IaaS および SaaS ソリューションを市場に投入しています。</span><span class="sxs-lookup"><span data-stu-id="6f270-326">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="6f270-327">ISV 発行者は、Microsoft パートナー チャネルを通じたプランの販売を有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6f270-327">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="6f270-328">インセンティブの対象となるプランは、次の 2 つのカテゴリに分類されます。</span><span class="sxs-lookup"><span data-stu-id="6f270-328">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="6f270-329">Azure IP 共同販売インセンティブ対象ステータスを持つ、SaaS と IaaS のサードパーティ プランを選択する。</span><span class="sxs-lookup"><span data-stu-id="6f270-329">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="6f270-330">Teams、または少なくとも 2 つの Microsoft 365 生産性向上アプリ (PowerPoint、Word、Excel、Outlook、SharePoint など) で統合された SaaS アプリケーション。</span><span class="sxs-lookup"><span data-stu-id="6f270-330">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="6f270-331">次の手順とリソース</span><span class="sxs-lookup"><span data-stu-id="6f270-331">Next steps and resources</span></span>

- <span data-ttu-id="6f270-332">対象となるマーケットプレース アプリやインセンティブ対象アプリを販売する場合の[パートナー インセンティブ](https://partner.microsoft.com/membership/partner-incentives)の獲得について確認してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-332">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="6f270-333">新しいプランは毎月追加されます。</span><span class="sxs-lookup"><span data-stu-id="6f270-333">New offers are added monthly.</span></span>  
- [<span data-ttu-id="6f270-334">クラウド ソリューション プロバイダーの直接請求パートナー インセンティブ リソース</span><span class="sxs-lookup"><span data-stu-id="6f270-334">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="6f270-335">クラウド ソリューション プロバイダーの間接プロバイダー インセンティブ リソース</span><span class="sxs-lookup"><span data-stu-id="6f270-335">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="6f270-336">この[プレゼンテーション](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf)を確認して、コマーシャル マーケットプレース アプリの販売に関する詳細を確認してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-336">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="6f270-337">その他のリソースについては、[こちら](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-337">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="6f270-338">[パートナー センター](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover)または [Azure portal](https://ms.portal.azure.com/#home) でコマーシャル マーケットプレース カタログを探索する</span><span class="sxs-lookup"><span data-stu-id="6f270-338">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="6f270-339">[API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) 使用して、会社のマーケットプレースにアプリを統合する</span><span class="sxs-lookup"><span data-stu-id="6f270-339">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="6f270-340">取引を行いたい ISV に連絡する</span><span class="sxs-lookup"><span data-stu-id="6f270-340">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="6f270-341">間接プロバイダーは API を使用して統合し、販売するアプリについてリセラーに指示する必要があります</span><span class="sxs-lookup"><span data-stu-id="6f270-341">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="6f270-342">疑問がある場合</span><span class="sxs-lookup"><span data-stu-id="6f270-342">Questions?</span></span>  

<span data-ttu-id="6f270-343">パートナー センターのコマーシャル マーケットプレースの概要については、[この記事](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-343">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="6f270-344">さらにサポートが必要な場合は、パートナー センターでサポート リクエストを作成できます。</span><span class="sxs-lookup"><span data-stu-id="6f270-344">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="6f270-345">詳細については、[https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-345">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="6f270-346">Power BI Premium プランの名前と前提条件の更新</span><span class="sxs-lookup"><span data-stu-id="6f270-346">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-347">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-347">Categories</span></span>

- <span data-ttu-id="6f270-348">日付: 2021 年 3 月 18 日</span><span class="sxs-lookup"><span data-stu-id="6f270-348">Date: 2021-03-18</span></span>
- <span data-ttu-id="6f270-349">機能</span><span class="sxs-lookup"><span data-stu-id="6f270-349">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6f270-350">まとめ</span><span class="sxs-lookup"><span data-stu-id="6f270-350">Summary</span></span>

<span data-ttu-id="6f270-351">2021 年 4 月 1 日の最終的な価格表は、Power BI Premium Per User の名前や前提条件の情報を明確にするために更新されます。</span><span class="sxs-lookup"><span data-stu-id="6f270-351">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-352">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-352">Impacted audience</span></span>

<span data-ttu-id="6f270-353">クラウド ソリューション プロバイダー (CSP) の直接および間接のパートナー</span><span class="sxs-lookup"><span data-stu-id="6f270-353">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="6f270-354">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-354">Details</span></span>

<span data-ttu-id="6f270-355">2021 年 4 月 1 日の最終的な価格表は、Power BI Premium Per User の名前や前提条件の情報を明確にするために更新されます。</span><span class="sxs-lookup"><span data-stu-id="6f270-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="6f270-356">最終的な価格表が更新されるまで、このセクションの情報を使用して、正しい製品が注文されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-356">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="6f270-357">次の詳細は、影響を受ける SKU と前提条件の詳細を示しています。</span><span class="sxs-lookup"><span data-stu-id="6f270-357">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="6f270-358">3 月 1 日の価格表プレビューでのプラン表示名</span><span class="sxs-lookup"><span data-stu-id="6f270-358">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="6f270-359">4 月 1 日の最終的な価格表での更新されたプラン表示名</span><span class="sxs-lookup"><span data-stu-id="6f270-359">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="6f270-360">プラン ID</span><span class="sxs-lookup"><span data-stu-id="6f270-360">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="6f270-361">Power BI Premium Per User アドオン (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="6f270-361">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="6f270-362">Power BI Premium Per User アドオン **(Office)** (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="6f270-362">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="6f270-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="6f270-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="6f270-364">このプランを購入するには、次のいずれかの前提条件が満たされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6f270-364">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="6f270-365">プラン表示名</span><span class="sxs-lookup"><span data-stu-id="6f270-365">Offer display name</span></span> | <span data-ttu-id="6f270-366">プラン ID</span><span class="sxs-lookup"><span data-stu-id="6f270-366">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="6f270-367">Microsoft 365 E5 (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="6f270-367">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="6f270-368">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="6f270-368">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="6f270-369">オーディオ会議なしの Microsoft 365 E5 (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="6f270-369">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="6f270-370">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="6f270-370">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="6f270-371">Office 365 E5 (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="6f270-371">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="6f270-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="6f270-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="6f270-373">Office 365 E5 (非営利団体職員向けの価格) 試用版</span><span class="sxs-lookup"><span data-stu-id="6f270-373">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="6f270-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="6f270-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="6f270-375">オーディオ会議なしの Office 365 E5 (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="6f270-375">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="6f270-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="6f270-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="6f270-377">次の Power BI Premium プランには、購入に必要な前提条件があります。</span><span class="sxs-lookup"><span data-stu-id="6f270-377">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="6f270-378">プラン表示名</span><span class="sxs-lookup"><span data-stu-id="6f270-378">Offer display name</span></span> | <span data-ttu-id="6f270-379">プラン ID</span><span class="sxs-lookup"><span data-stu-id="6f270-379">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="6f270-380">Power BI Premium Per User アドオン (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="6f270-380">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="6f270-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="6f270-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="6f270-382">このプランを購入するには、この前提条件が必要です。</span><span class="sxs-lookup"><span data-stu-id="6f270-382">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="6f270-383">プラン表示名</span><span class="sxs-lookup"><span data-stu-id="6f270-383">Offer display name</span></span> | <span data-ttu-id="6f270-384">プラン ID</span><span class="sxs-lookup"><span data-stu-id="6f270-384">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="6f270-385">Power BI Pro (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="6f270-385">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="6f270-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="6f270-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="6f270-387">次のステップ</span><span class="sxs-lookup"><span data-stu-id="6f270-387">Next steps</span></span>

<span data-ttu-id="6f270-388">このトピックに関するリソースを確認し、この情報を組織内の該当する関係者と共有してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-388">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="6f270-389">疑問がある場合</span><span class="sxs-lookup"><span data-stu-id="6f270-389">Questions?</span></span>

<span data-ttu-id="6f270-390">これらのプランについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-390">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a><span data-ttu-id="6f270-391">Microsoft 365 F3 の 3 月の価格更新</span><span class="sxs-lookup"><span data-stu-id="6f270-391">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-392">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-392">Categories</span></span>

- <span data-ttu-id="6f270-393">日付: 2021 年 3 月 16 日</span><span class="sxs-lookup"><span data-stu-id="6f270-393">Date: 2021-03-16</span></span>
- <span data-ttu-id="6f270-394">製品サービス/市場</span><span class="sxs-lookup"><span data-stu-id="6f270-394">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="6f270-395">まとめ</span><span class="sxs-lookup"><span data-stu-id="6f270-395">Summary</span></span>

<span data-ttu-id="6f270-396">Microsoft 365 F3 のイギリス ポンド (GBP) とユーロ (EUR) では、2021 年 3 月の正しくない価格が修正されました。</span><span class="sxs-lookup"><span data-stu-id="6f270-396">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-397">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-397">Impacted audience</span></span>

<span data-ttu-id="6f270-398">クラウド ソリューション プロバイダー (CSP) プログラムを通して、2021 年 3 月 1 日から 3 月 17 日までの間に Microsoft 365 F3 を GBP または EUR で購入したパートナー。</span><span class="sxs-lookup"><span data-stu-id="6f270-398">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="6f270-399">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-399">Details</span></span>

<span data-ttu-id="6f270-400">Microsoft は Microsoft 365 F3 の価格が正しくなかった問題を解決しました。</span><span class="sxs-lookup"><span data-stu-id="6f270-400">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="6f270-401">GBP と EUR の価格が正しくありませんでした。2021 年 3 月 1 日から 3 月 17 日の間に購入したプランのみが対象となります。</span><span class="sxs-lookup"><span data-stu-id="6f270-401">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="6f270-402">影響を受けるプランと通貨は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="6f270-402">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="6f270-403">プラン名</span><span class="sxs-lookup"><span data-stu-id="6f270-403">Offer name</span></span> | <span data-ttu-id="6f270-404">Currency</span><span class="sxs-lookup"><span data-stu-id="6f270-404">Currency</span></span> | <span data-ttu-id="6f270-405">プラン ID</span><span class="sxs-lookup"><span data-stu-id="6f270-405">Offer ID</span></span> | <span data-ttu-id="6f270-406">マテリアル ID</span><span class="sxs-lookup"><span data-stu-id="6f270-406">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="6f270-407">Microsoft 365 F3 (非営利団体)</span><span class="sxs-lookup"><span data-stu-id="6f270-407">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="6f270-408">GBP</span><span class="sxs-lookup"><span data-stu-id="6f270-408">GBP</span></span> | <span data-ttu-id="6f270-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="6f270-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="6f270-410">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="6f270-410">AAD-11626</span></span> |
| <span data-ttu-id="6f270-411">Microsoft 365 F3 (商用)</span><span class="sxs-lookup"><span data-stu-id="6f270-411">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="6f270-412">EUR</span><span class="sxs-lookup"><span data-stu-id="6f270-412">EUR</span></span>| <span data-ttu-id="6f270-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="6f270-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="6f270-414">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="6f270-414">AAA-89898</span></span> |
 
<span data-ttu-id="6f270-415">3 月および 4 月のプレビューのライセンスベースの価格表は、3 月 16 日午後 5 時 (太平洋標準時) に更新されました。</span><span class="sxs-lookup"><span data-stu-id="6f270-415">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6f270-416">次のステップ</span><span class="sxs-lookup"><span data-stu-id="6f270-416">Next steps</span></span>

- <span data-ttu-id="6f270-417">パートナーは、3 月と 4 月のプレビューの両方の現在のライセンスベースの価格表をもう一度ダウンロードし、該当する場合はこれらの価格を修正する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6f270-417">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="6f270-418">Microsoft は、今後数週間にわたって影響を受けたパートナーにメールで連絡し、影響を受けるトランザクションの修正に関連する今後の手順について通知します。</span><span class="sxs-lookup"><span data-stu-id="6f270-418">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="6f270-419">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="6f270-419">Questions?</span></span>

<span data-ttu-id="6f270-420">さらにご質問がある場合は、関連する CSP Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-420">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a><span data-ttu-id="6f270-421">パートナー センターでの会社正式名称の更新</span><span class="sxs-lookup"><span data-stu-id="6f270-421">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-422">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-422">Categories</span></span>

- <span data-ttu-id="6f270-423">日付: 2021 年 3 月 16 日</span><span class="sxs-lookup"><span data-stu-id="6f270-423">Date: 2021-03-16</span></span>
- <span data-ttu-id="6f270-424">効率とスケールの向上</span><span class="sxs-lookup"><span data-stu-id="6f270-424">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="6f270-425">まとめ</span><span class="sxs-lookup"><span data-stu-id="6f270-425">Summary</span></span>

<span data-ttu-id="6f270-426">2021 年 3 月から、Microsoft Partner Network (MPN) パートナーとクラウド ソリューション プロバイダー (CSP) 間接リセラーは、パートナー センターで会社の正式名称を更新できます。</span><span class="sxs-lookup"><span data-stu-id="6f270-426">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-427">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-427">Impacted audience</span></span>

<span data-ttu-id="6f270-428">MPN パートナーと CSP 間接リセラー (CSP 直接請求パートナーは対象外です)</span><span class="sxs-lookup"><span data-stu-id="6f270-428">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="6f270-429">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-429">Details</span></span>

<span data-ttu-id="6f270-430">2021 年 3 月から MPN パートナーと CSP 間接リセラーは、パートナー センターで、規則に従って、セルフ サービス方式で、会社の正式名称を更新できます。</span><span class="sxs-lookup"><span data-stu-id="6f270-430">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="6f270-431">この新機能により、パートナーは社名を更新するためにパートナー センター サポート チケットを提出する必要がなくなります。</span><span class="sxs-lookup"><span data-stu-id="6f270-431">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="6f270-432">これにより、パートナーはこれらの操作を行う際の時間をかなり節約することができます。</span><span class="sxs-lookup"><span data-stu-id="6f270-432">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="6f270-433">詳細については、「[法的ビジネスプロファイルを更新する](../update-your-partner-profile.md#update-your-legal-business-profile)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-433">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="6f270-434">企業の公式プロファイルの社名に誤字や略式表記がないこと、会社の正式な登録情報と完全に一致していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-434">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="6f270-435">組織プロファイル更新の詳細は[組織プロファイルの有効性を確認する](../update-your-partner-profile.md#update-your-legal-business-profile)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-435">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="6f270-436">次の手順</span><span class="sxs-lookup"><span data-stu-id="6f270-436">Next steps</span></span>

<span data-ttu-id="6f270-437">担当チームが手続きの見直し、更新を実施できるよう、この情報を組織で共有してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-437">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="6f270-438">ご質問がある場合は、</span><span class="sxs-lookup"><span data-stu-id="6f270-438">Questions?</span></span>

<span data-ttu-id="6f270-439">さらにご質問がある場合は、関連する CSP Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-439">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a><span data-ttu-id="6f270-440">クラウド ソリューション プロバイダー (CSP) プログラムの進歩とオープン ライセンス プログラムの変更に関する最新情報</span><span class="sxs-lookup"><span data-stu-id="6f270-440">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-441">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-441">Categories</span></span>

- <span data-ttu-id="6f270-442">日付: 2021 年 3 月 15 日</span><span class="sxs-lookup"><span data-stu-id="6f270-442">Date: 2021-03-15</span></span>
- <span data-ttu-id="6f270-443">機能</span><span class="sxs-lookup"><span data-stu-id="6f270-443">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6f270-444">まとめ</span><span class="sxs-lookup"><span data-stu-id="6f270-444">Summary</span></span>

<span data-ttu-id="6f270-445">オープン ライセンス プログラムの変更に伴い、商用および公的機関向けの新しい永続ライセンス ソフトウェア商品を、クラウド ソリューション プロバイダー (CSP) プログラムに追加します。</span><span class="sxs-lookup"><span data-stu-id="6f270-445">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-446">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-446">Impacted audience</span></span>

<span data-ttu-id="6f270-447">オープン ライセンス プログラムを通じて販売を行っている商業ディストリビューターと管理下のリセラー、および、永続ライセンス ソフトウェアの取引を行っているすべての CSP パートナー</span><span class="sxs-lookup"><span data-stu-id="6f270-447">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="6f270-448">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-448">Details</span></span>

<span data-ttu-id="6f270-449">2020 年 9 月、Microsoft はデジタル化推進の一環として、CSP プログラムのパートナーにビジネス機会を提供するための一連の方策を[発表しました](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/)。一例として、パートナーはオンプレミスのソフトウェアを使用できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="6f270-449">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="6f270-450">これらの変更により、パートナーは CSP のソフトウェア ライセンスを利用してビジネスを成長させ、リーチを広げることができ、クラウド ファーストである現環境での成功を期待できます。</span><span class="sxs-lookup"><span data-stu-id="6f270-450">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="6f270-451">これはまた、顧客のクラウド移行をサポートし、顧客のハイブリッド クラウド環境の運用に求められる柔軟性をパートナーに与えます。</span><span class="sxs-lookup"><span data-stu-id="6f270-451">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="6f270-452">こうしてデジタル化を推し進める中で、Microsoft は次の変更を発表しました。</span><span class="sxs-lookup"><span data-stu-id="6f270-452">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="6f270-453">2021 年 7 月 1 日: 新たな SKU、製品、販促物をオープン ライセンス プログラムの価格表に追加することを中止します。</span><span class="sxs-lookup"><span data-stu-id="6f270-453">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="6f270-454">2021 年 7 月 7 日: Get Genuine Windows と Visual Studio Professional の 2 商品、および公的機関 (政府、教育機関、NPO。[発表](./2020-december.md#9)をご確認ください) 向けオファーを CSP 永続ライセンス ソフトウェアの価格表に追加します。</span><span class="sxs-lookup"><span data-stu-id="6f270-454">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="6f270-455">価格表はパートナー センターの [[Sell]\(販売\) > [Pricing & Offers]\(価格とオファー\)](https://partnercenter.microsoft.com/pcv/sales) ページの [ソフトウェア] セクションで閲覧できます。この価格表はこの日に改定する予定です。</span><span class="sxs-lookup"><span data-stu-id="6f270-455">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="6f270-456">CSP プログラムの進歩とオープン ライセンス プログラムの変更の詳細は、下の「**次のステップ**」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-456">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6f270-457">次のステップ:</span><span class="sxs-lookup"><span data-stu-id="6f270-457">Next Steps:</span></span>

- <span data-ttu-id="6f270-458">CSP プログラムの進歩: 準備資料[クラウド ソリューション プロバイダー プログラムの永続ライセンス ソフトウェア](https://partner.microsoft.com/resources/collection/software-in-csp#/)をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-458">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="6f270-459">こちらの[レディネス マップ](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf)を利用すると、ロールに適した情報をすばやく見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="6f270-459">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="6f270-460">オープン ライセンス プログラムの変更: 準備資料[ CSP プログラムの進歩とオープン ライセンス プログラムの変更](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-460">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="6f270-461">こちらの[レディネス マップ](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf)を利用すると、ロールに適した情報をすばやく見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="6f270-461">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="6f270-462">質問</span><span class="sxs-lookup"><span data-stu-id="6f270-462">Questions</span></span>

<span data-ttu-id="6f270-463">さらにご質問がある場合は、関連する CSP Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-463">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="6f270-464">以前の発表に関する最新情報: Compliance Manager のプレミアム評価アドオン</span><span class="sxs-lookup"><span data-stu-id="6f270-464">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-465">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-465">Categories</span></span>

- <span data-ttu-id="6f270-466">日付: 2021 年 3 月 15 日</span><span class="sxs-lookup"><span data-stu-id="6f270-466">Date: 2021-03-15</span></span>
- <span data-ttu-id="6f270-467">ビジネスを拡大する</span><span class="sxs-lookup"><span data-stu-id="6f270-467">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="6f270-468">まとめ</span><span class="sxs-lookup"><span data-stu-id="6f270-468">Summary</span></span>

<span data-ttu-id="6f270-469">オファーの試用版は価格表に掲載しないことになっており、今後削除する予定です。</span><span class="sxs-lookup"><span data-stu-id="6f270-469">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-470">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-470">Impacted audience</span></span>

<span data-ttu-id="6f270-471">クラウド ソリューション プロバイダー プログラムで取引を行うパートナー</span><span class="sxs-lookup"><span data-stu-id="6f270-471">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="6f270-472">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-472">Details</span></span>

<span data-ttu-id="6f270-473">オファーの試用版は価格表に掲載しないことになっています。</span><span class="sxs-lookup"><span data-stu-id="6f270-473">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="6f270-474">これらは 2021 年 5 月 1 日の価格表から削除します。</span><span class="sxs-lookup"><span data-stu-id="6f270-474">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="6f270-475">元の発表は[こちら](./2021-february.md#4)でご覧いただけます。</span><span class="sxs-lookup"><span data-stu-id="6f270-475">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="6f270-476">その他のリソース</span><span class="sxs-lookup"><span data-stu-id="6f270-476">Additional resources</span></span>

- [<span data-ttu-id="6f270-477">Microsoft 365 E5 のセキュリティとコンプライアンス</span><span class="sxs-lookup"><span data-stu-id="6f270-477">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="6f270-478">Microsoft コンプライアンス マネージャーでの評価の作成と管理 - Microsoft 365 コンプライアンス</span><span class="sxs-lookup"><span data-stu-id="6f270-478">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="6f270-479">次のステップ</span><span class="sxs-lookup"><span data-stu-id="6f270-479">Next steps</span></span>

<span data-ttu-id="6f270-480">このトピックに関するリソースを確認し、この情報を組織内の該当する関係者と共有してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-480">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="6f270-481">疑問がある場合</span><span class="sxs-lookup"><span data-stu-id="6f270-481">Questions?</span></span>

<span data-ttu-id="6f270-482">これらのオファーに関するご質問については、Yammer の関連コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-482">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="6f270-483">One Commercial Partner (OCP) Go-to-Market (GTM) から Microsoft コマーシャル マーケットプレースにソリューションを移動する</span><span class="sxs-lookup"><span data-stu-id="6f270-483">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-484">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-484">Categories</span></span>

- <span data-ttu-id="6f270-485">日付: 2021 年 3 月 12 日</span><span class="sxs-lookup"><span data-stu-id="6f270-485">Date: 2021-03-12</span></span>
- <span data-ttu-id="6f270-486">機能</span><span class="sxs-lookup"><span data-stu-id="6f270-486">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6f270-487">まとめ</span><span class="sxs-lookup"><span data-stu-id="6f270-487">Summary</span></span>

<span data-ttu-id="6f270-488">2021 年 3 月 29 日から One Commercial Partner (OCP) Go-to-Market (GTM) の機能を制限します。</span><span class="sxs-lookup"><span data-stu-id="6f270-488">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="6f270-489">パートナー センターのコマーシャル マーケットプレースにソリューションを移動することを推奨します。</span><span class="sxs-lookup"><span data-stu-id="6f270-489">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-490">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-490">Impacted audience</span></span>

<span data-ttu-id="6f270-491">OCP GTM のソリューションを使用して共同販売を行っている組織</span><span class="sxs-lookup"><span data-stu-id="6f270-491">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="6f270-492">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-492">Details</span></span>

<span data-ttu-id="6f270-493">Microsoft は 2020 年 12 月に、Microsoft OCP GTM ツールからパートナー センターの Microsoft コマーシャル マーケットプレースへの移行を開始しました。</span><span class="sxs-lookup"><span data-stu-id="6f270-493">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="6f270-494">この移行によってコマーシャル マーケットプレースの機能を拡張します。これは、皆様のソリューションを何百万もの顧客に紹介し、Microsoft や他のパートナー販売者と相互にビジネス機会を共有し、革新的なソリューションを共同販売できるプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="6f270-494">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="6f270-495">移行の次のステップは 2021 年 3 月 29 日に実施します。</span><span class="sxs-lookup"><span data-stu-id="6f270-495">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="6f270-496">そのときに、OCP GTM の機能の制限を開始し、一部のサービスは閲覧しかできなくなります。</span><span class="sxs-lookup"><span data-stu-id="6f270-496">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="6f270-497">現在 OCP GTM のソリューションを使用して共同販売を行っている場合、ソリューションをコマーシャル マーケットプレースに移動することを推奨します。それによって、この機能を利用できるようになり、公開作業も単純化できます。</span><span class="sxs-lookup"><span data-stu-id="6f270-497">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="6f270-498">コマーシャル マーケットプレースに移行すると、共同販売する商品は主としてパートナー センターで公開することになります。</span><span class="sxs-lookup"><span data-stu-id="6f270-498">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="6f270-499">そこでは、Microsoft が採用している共通の販路と製品内部の仕組みを通じて皆様のソリューションを共通の顧客に紹介することで、引き続きビジネスを成長させることができます。</span><span class="sxs-lookup"><span data-stu-id="6f270-499">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="6f270-500">[コマーシャル マーケットプレースの詳細](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/)。</span><span class="sxs-lookup"><span data-stu-id="6f270-500">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="6f270-501">次の手順</span><span class="sxs-lookup"><span data-stu-id="6f270-501">Next steps</span></span>

- <span data-ttu-id="6f270-502">まだソリューションを移動させていない場合、[移行ガイド](/azure/marketplace/co-sell-solution-migration)に詳述された手順に従うか、[ステップ バイ ステップの動画チュートリアル](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4)を見て移動作業を完了し、コマーシャル マーケットプレースでソリューションの公開を始めてください。</span><span class="sxs-lookup"><span data-stu-id="6f270-502">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="6f270-503">OCP GTM の機能の制限に関するご質問については [Microsoft コマーシャル マーケットプレース共同販売公開要件 FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf) に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-503">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="6f270-504">(2021 年 3 月 29 日に始まる OCP GTM の機能の制限に関するセクションをお読みください。)</span><span class="sxs-lookup"><span data-stu-id="6f270-504">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="6f270-505">疑問がある場合</span><span class="sxs-lookup"><span data-stu-id="6f270-505">Questions?</span></span>

<span data-ttu-id="6f270-506">ご質問がある場合、詳しく知りたい場合は[サポート](https://partner.microsoft.com/support/?stage=1)にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="6f270-506">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="6f270-507">クラウド ソリューション プロバイダー (CSP) プログラムの Azure 取引新サービスをロシアに拡大</span><span class="sxs-lookup"><span data-stu-id="6f270-507">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-508">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-508">Categories</span></span>

- <span data-ttu-id="6f270-509">日付: 2021 年 3 月 10 日</span><span class="sxs-lookup"><span data-stu-id="6f270-509">Date: 2021-03-10</span></span>
- <span data-ttu-id="6f270-510">機能</span><span class="sxs-lookup"><span data-stu-id="6f270-510">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-511">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-511">Impacted audience</span></span>

<span data-ttu-id="6f270-512">クラウド ソリューション プロバイダー (CSP) プログラムを通じてロシアで取引を行うすべてのパートナー。</span><span class="sxs-lookup"><span data-stu-id="6f270-512">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="6f270-513">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-513">Details</span></span>

<span data-ttu-id="6f270-514">2021 年 3 月 10 日から **CSP の Azure 取引新サービスをロシアで利用** できるようになります。</span><span class="sxs-lookup"><span data-stu-id="6f270-514">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="6f270-515">このサービスにより、顧客が Azure のサービスを購入、使用する方法を効率化し、改善します。</span><span class="sxs-lookup"><span data-stu-id="6f270-515">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="6f270-516">また、CSP プログラムのパートナーは、さまざまな販売状況を通じて Azure の料金を安定的に見通し、国際的目安として米ドルでの料金を把握し、請求日をそろえ、Azure Cost Management にアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="6f270-516">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6f270-517">次の手順</span><span class="sxs-lookup"><span data-stu-id="6f270-517">Next steps</span></span>

<span data-ttu-id="6f270-518">Azure の新しい取引サービスを紹介し、追加的な情報を提供する資料をいくつか用意しています。</span><span class="sxs-lookup"><span data-stu-id="6f270-518">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="6f270-519">最新の FAQ、プレゼン資料、動画、その他の資料を [CSP プログラム最新情報資料ギャラリー](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)で見付けてください。</span><span class="sxs-lookup"><span data-stu-id="6f270-519">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="6f270-520">パートナー センター ソフトウェア ライセンス キーとダウンロード フルフィルメント</span><span class="sxs-lookup"><span data-stu-id="6f270-520">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-521">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-521">Categories</span></span>

- <span data-ttu-id="6f270-522">日付: 2021 年 3 月 4 日</span><span class="sxs-lookup"><span data-stu-id="6f270-522">Date: 2021-03-04</span></span>
- <span data-ttu-id="6f270-523">機能</span><span class="sxs-lookup"><span data-stu-id="6f270-523">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6f270-524">まとめ</span><span class="sxs-lookup"><span data-stu-id="6f270-524">Summary</span></span>

<span data-ttu-id="6f270-525">パートナー センターのソフトウェア ダウンロードおよびライセンス キー フルフィルメント機能が復元されました。</span><span class="sxs-lookup"><span data-stu-id="6f270-525">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-526">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-526">Impacted audience</span></span>

<span data-ttu-id="6f270-527">パートナー センターを通じて永続的およびサーバーのサブスクリプション ソフトウェアの注文を処理しているすべてのクラウド ソリューション プロバイダー (CSP) パートナー</span><span class="sxs-lookup"><span data-stu-id="6f270-527">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="6f270-528">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-528">Details</span></span>

<span data-ttu-id="6f270-529">パートナーからのフィードバックに応えて、永続的およびサーバーのサブスクリプション ソフトウェアの注文に対してソフトウェアとライセンス キーを取得するパートナー センターのフルフィルメント機能を復元しています。</span><span class="sxs-lookup"><span data-stu-id="6f270-529">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="6f270-530">2021 年 1 月 19 日に削除される前の状態に復元されます。</span><span class="sxs-lookup"><span data-stu-id="6f270-530">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="6f270-531">([お知らせ](2020-september.md#17)を参照してください。)</span><span class="sxs-lookup"><span data-stu-id="6f270-531">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="6f270-532">ソフトウェア ライセンス キーとダウンロード リンクは、価値ある重要な知財資産であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-532">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="6f270-533">リークが生じると、それらのライセンス認証制限がすぐに枯渇し、顧客エクスペリエンスやパートナー エクスペリエンスに悪影響を及ぼす恐れがあります。</span><span class="sxs-lookup"><span data-stu-id="6f270-533">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6f270-534">次のステップ</span><span class="sxs-lookup"><span data-stu-id="6f270-534">Next steps</span></span>

<span data-ttu-id="6f270-535">ソフトウェアキーの配布に関する使用方法と重要なガイダンスについては、次のリソースを参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-535">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="6f270-536">CSP プログラムによるオンプレミス ソフトウェアの販売</span><span class="sxs-lookup"><span data-stu-id="6f270-536">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="6f270-537">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (**ソフトウェア キーの配布に関するガイダンス** に関するセクションを参照してください)。</span><span class="sxs-lookup"><span data-stu-id="6f270-537">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="6f270-538">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="6f270-538">Questions?</span></span>

<span data-ttu-id="6f270-539">この通知についてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-539">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="6f270-540">Partner Sales Connect (PSC) からパートナー センターに取引を移行</span><span class="sxs-lookup"><span data-stu-id="6f270-540">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-541">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-541">Categories</span></span>

- <span data-ttu-id="6f270-542">日付: 2021 年 3 月 4 日</span><span class="sxs-lookup"><span data-stu-id="6f270-542">Date: 2021-03-04</span></span>
- <span data-ttu-id="6f270-543">機能</span><span class="sxs-lookup"><span data-stu-id="6f270-543">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6f270-544">まとめ</span><span class="sxs-lookup"><span data-stu-id="6f270-544">Summary</span></span>

<span data-ttu-id="6f270-545">Partner Sales Connect (PSC) は、2021 年 3 月 31 日から読み取り専用アクセスに移行するので、PSC からパートナー センターに取引を移行し始めることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="6f270-545">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-546">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-546">Impacted audience</span></span>

<span data-ttu-id="6f270-547">PSC での取引があるパートナー</span><span class="sxs-lookup"><span data-stu-id="6f270-547">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="6f270-548">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-548">Details</span></span>

<span data-ttu-id="6f270-549">成長に対する共有コミットメントの一環として、**Microsoft との共同販売** は、お客様が **認識され、専門知識を提供し、顧客フットプリントを拡大して**、良好な顧客アウトカムを得るための手段です。</span><span class="sxs-lookup"><span data-stu-id="6f270-549">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="6f270-550">パートナー センターで共同販売エクスペリエンスを管理すれば、平均的な処理が通常より **3.5 倍高速** になり、顧客への直接販売や、パートナー、Microsoft の販売者チャネルなどに対する販売ができ、1 か所でパイプライン全体を管理できます。</span><span class="sxs-lookup"><span data-stu-id="6f270-550">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="6f270-551">**PSC** は **2021 年 3 月 31 日** から **読み取り専用アクセス** に移行するため、パートナー センターへの移行を開始し、以下のような機能改善にアクセスすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="6f270-551">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="6f270-552">お客様が必要とするサポートの種類に基づいて、Microsoft と共有する取引を適切な販売者に **ルーティングする際の正確さの向上**。</span><span class="sxs-lookup"><span data-stu-id="6f270-552">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="6f270-553">インセンティブの対象となるソリューションに対する適格性があるか、および ISV コネクト プログラムの基準を満たしているかについての **前払い取引の検証**。このため、承認プロセスと最終的な実行証明 (POE) の立証が簡略化されます。</span><span class="sxs-lookup"><span data-stu-id="6f270-553">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="6f270-554">すべての共同販売機会とセールス見込み客を 1 か所で管理するための **シームレスなユーザー エクスペリエンス**。</span><span class="sxs-lookup"><span data-stu-id="6f270-554">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="6f270-555">また、お客様の移行を支援するために、最近パートナー センターに次のような新しい機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="6f270-555">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="6f270-556">共同販売機会の一括操作</span><span class="sxs-lookup"><span data-stu-id="6f270-556">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="6f270-557">[取引移行機能](../psc-to-pc.md) (**PSC 取引の移行** に関するセクションを参照してください)。</span><span class="sxs-lookup"><span data-stu-id="6f270-557">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="6f270-558">パートナー センターの共同販売エクスペリエンスを利用することで、販売チームは、見込み客や機会の促進、契約の締結、顧客との長期的な関係の形成に集中する時間が増えます。</span><span class="sxs-lookup"><span data-stu-id="6f270-558">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="6f270-559">次のステップ</span><span class="sxs-lookup"><span data-stu-id="6f270-559">Next steps</span></span>

<span data-ttu-id="6f270-560">パートナー センターへの[移行ガイド](../psc-to-pc.md)を使用して、PSC からパートナー センターに取引を移行する手順について説明します。</span><span class="sxs-lookup"><span data-stu-id="6f270-560">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="6f270-561">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="6f270-561">Questions?</span></span>

<span data-ttu-id="6f270-562">その他の質問については、[サポート](https://partner.microsoft.com/support/?stage=1)にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="6f270-562">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="6f270-563">新しい Microsoft Dynamics 365 製品およびオファーが 2021 年 4 月 1 日に利用できるようになります</span><span class="sxs-lookup"><span data-stu-id="6f270-563">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-564">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-564">Categories</span></span>

- <span data-ttu-id="6f270-565">日付: 2021 年 3 月 4 日</span><span class="sxs-lookup"><span data-stu-id="6f270-565">Date: 2021-03-04</span></span>
- <span data-ttu-id="6f270-566">機能</span><span class="sxs-lookup"><span data-stu-id="6f270-566">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6f270-567">まとめ</span><span class="sxs-lookup"><span data-stu-id="6f270-567">Summary</span></span>

<span data-ttu-id="6f270-568">2021 年 4 月 1 日、Microsoft は、クラウド ソリューション プロバイダー (CSP) プログラム用のいくつかの新しい製品およびプランを開始します。</span><span class="sxs-lookup"><span data-stu-id="6f270-568">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-569">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-569">Impacted audience</span></span>

<span data-ttu-id="6f270-570">クラウド ソリューション プロバイダー (CSP) プログラムを通じて取引を行う、すべてのパートナー様</span><span class="sxs-lookup"><span data-stu-id="6f270-570">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="6f270-571">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-571">Details</span></span>

<span data-ttu-id="6f270-572">2021 年 4 月 1 日に、Microsoft は、次のような新しい製品およびプランを開始します。</span><span class="sxs-lookup"><span data-stu-id="6f270-572">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="6f270-573">Power BI Premium Per User</span><span class="sxs-lookup"><span data-stu-id="6f270-573">Power BI Premium Per User</span></span>
- <span data-ttu-id="6f270-574">Customer Voice および Marketing USL の地域およびセグメントの拡張</span><span class="sxs-lookup"><span data-stu-id="6f270-574">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="6f270-575">**Power BI Premium Per User**</span><span class="sxs-lookup"><span data-stu-id="6f270-575">**Power BI Premium Per User**</span></span>

<span data-ttu-id="6f270-576">Microsoft は、最初のユーザーごとの Power BI Premium プランを導入します。</span><span class="sxs-lookup"><span data-stu-id="6f270-576">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="6f270-577">Power BI Premium は現在、容量構成でのみ販売されています。</span><span class="sxs-lookup"><span data-stu-id="6f270-577">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="6f270-578">Power BI Premium Per User は、ユーザーごとに、エンタープライズ ビジネス インテリジェンス (BI) および分析機能へのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="6f270-578">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="6f270-579">その柔軟な個別のシート ライセンスで、中小規模の企業の要求に応えます。</span><span class="sxs-lookup"><span data-stu-id="6f270-579">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="6f270-580">このプランについて詳しくは、[Power BI リリースの詳細](/power-platform-release-plan/2020wave2/power-bi/planned-features)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-580">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="6f270-581">**特典の詳細**</span><span class="sxs-lookup"><span data-stu-id="6f270-581">**Offer details**</span></span>

<span data-ttu-id="6f270-582">プラン名は、価格表プレビューとは若干異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-582">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="6f270-583">プラン名</span><span class="sxs-lookup"><span data-stu-id="6f270-583">Offer name</span></span> | <span data-ttu-id="6f270-584">プラン ID</span><span class="sxs-lookup"><span data-stu-id="6f270-584">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="6f270-585">Power BI Premium Per User</span><span class="sxs-lookup"><span data-stu-id="6f270-585">Power BI Premium Per User</span></span> | <span data-ttu-id="6f270-586">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="6f270-586">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="6f270-587">教職員用 Power BI Premium Per User</span><span class="sxs-lookup"><span data-stu-id="6f270-587">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="6f270-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="6f270-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="6f270-589">学生用 Power BI Premium Per User</span><span class="sxs-lookup"><span data-stu-id="6f270-589">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="6f270-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="6f270-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="6f270-591">Power BI Premium Per User (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="6f270-591">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="6f270-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="6f270-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="6f270-593">Power BI Premium Per User アドオン</span><span class="sxs-lookup"><span data-stu-id="6f270-593">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="6f270-594">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="6f270-594">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="6f270-595">教職員用 Power BI Premium Per User アドオン</span><span class="sxs-lookup"><span data-stu-id="6f270-595">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="6f270-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="6f270-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="6f270-597">学生用 Power BI Premium Per User アドオン</span><span class="sxs-lookup"><span data-stu-id="6f270-597">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="6f270-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="6f270-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="6f270-599">Power BI Premium Per User アドオン (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="6f270-599">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="6f270-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="6f270-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="6f270-601">**Customer Voice および Marketing USL の地域およびセグメントの拡張**</span><span class="sxs-lookup"><span data-stu-id="6f270-601">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="6f270-602">2020 年 12 月の発売後のフォローアップとして、Dynamics 365 Customer Voice および Marketing USL プランは、新しい国やより多くの非営利団体および教育機関向けの SKU を追加するように変更されてきました。</span><span class="sxs-lookup"><span data-stu-id="6f270-602">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="6f270-603">プラン名</span><span class="sxs-lookup"><span data-stu-id="6f270-603">Offer name</span></span> | <span data-ttu-id="6f270-604">プラン ID</span><span class="sxs-lookup"><span data-stu-id="6f270-604">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="6f270-605">Dynamics 365 Customer Voice USL (非営利団体職員向けの価格)</span><span class="sxs-lookup"><span data-stu-id="6f270-605">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="6f270-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="6f270-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="6f270-607">教職員用 Dynamics 365 Customer Voice USL</span><span class="sxs-lookup"><span data-stu-id="6f270-607">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="6f270-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="6f270-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="6f270-609">これらのプランについて詳しくは、次のページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-609">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="6f270-610">Dynamics 365 Customer Service Voice ホーム ページ</span><span class="sxs-lookup"><span data-stu-id="6f270-610">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="6f270-611">Dynamics 365 Marketing ホーム ページ</span><span class="sxs-lookup"><span data-stu-id="6f270-611">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="6f270-612">次のステップ</span><span class="sxs-lookup"><span data-stu-id="6f270-612">Next steps</span></span>

<span data-ttu-id="6f270-613">このトピックに関するリソースを確認し、この情報を組織内の該当する関係者と共有します。</span><span class="sxs-lookup"><span data-stu-id="6f270-613">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="6f270-614">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="6f270-614">Questions?</span></span>

<span data-ttu-id="6f270-615">これらのプランについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-615">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a><span data-ttu-id="6f270-616">Microsoft Universal Print が一部のスイートで利用できるようになりました</span><span class="sxs-lookup"><span data-stu-id="6f270-616">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="6f270-617">Categories</span><span class="sxs-lookup"><span data-stu-id="6f270-617">Categories</span></span>

- <span data-ttu-id="6f270-618">日付: 2021 年 3 月 3 日</span><span class="sxs-lookup"><span data-stu-id="6f270-618">Date: 2021-03-33</span></span>
- <span data-ttu-id="6f270-619">機能</span><span class="sxs-lookup"><span data-stu-id="6f270-619">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="6f270-620">まとめ</span><span class="sxs-lookup"><span data-stu-id="6f270-620">Summary</span></span>

<span data-ttu-id="6f270-621">Microsoft Universal Print は、2021 年 3 月 1 日から、選択された Microsoft 365 スイート内での取引に利用したり、スタンドアロン アドオンとして利用したりできるようになります。</span><span class="sxs-lookup"><span data-stu-id="6f270-621">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="6f270-622">対象</span><span class="sxs-lookup"><span data-stu-id="6f270-622">Impacted audience</span></span>

<span data-ttu-id="6f270-623">クラウド ソリューション プロバイダー (CSP) プログラムを通じて取引を行う、すべてのパートナー様</span><span class="sxs-lookup"><span data-stu-id="6f270-623">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="6f270-624">詳細</span><span class="sxs-lookup"><span data-stu-id="6f270-624">Details</span></span>

<span data-ttu-id="6f270-625">[Universal Print](https://aka.ms/universalprint) は、オンプレミスのプリント サーバーを不要にし、Windows デバイスから Azure 登録済みプリンターに出力できるようにする Microsoft 365 プリント サービスです。</span><span class="sxs-lookup"><span data-stu-id="6f270-625">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="6f270-626">2021 年 3 月 1 日から取引に利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="6f270-626">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="6f270-627">ワーカーは、ドライバー不要の印刷、合理化されたロケーションベースのプリンター検出、学習曲線不要の直感的な印刷操作などの利点が得られます。</span><span class="sxs-lookup"><span data-stu-id="6f270-627">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="6f270-628">Azure Active Directory (Azure AD) に参加しているデバイスは、既存の Azure AD 資格情報を使用して安全に印刷します。</span><span class="sxs-lookup"><span data-stu-id="6f270-628">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="6f270-629">管理者は Azure portal を使用して印刷を管理し、Universal Print のネイティブ サポートを使用してプリンターを簡単に接続できます。</span><span class="sxs-lookup"><span data-stu-id="6f270-629">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="6f270-630">Universal Print は、Universal Print コネクタ ソフトウェアを使用して、互換性のないプリンターで展開できます。</span><span class="sxs-lookup"><span data-stu-id="6f270-630">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="6f270-631">Universal Print はサービス開始時に、Windows E3、A3、E5、A5 と Microsoft 365 BP、F3、E3、A3、E5、A5 に追加されます。</span><span class="sxs-lookup"><span data-stu-id="6f270-631">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="6f270-632">**特典の詳細**</span><span class="sxs-lookup"><span data-stu-id="6f270-632">**Offer details**</span></span>

<span data-ttu-id="6f270-633">プラン名は、価格表プレビューとは若干異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-633">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="6f270-634">プラン名</span><span class="sxs-lookup"><span data-stu-id="6f270-634">Offer name</span></span> | <span data-ttu-id="6f270-635">プラン ID</span><span class="sxs-lookup"><span data-stu-id="6f270-635">Offer ID</span></span> | <span data-ttu-id="6f270-636">マテリアル ID</span><span class="sxs-lookup"><span data-stu-id="6f270-636">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="6f270-637">Universal Print ボリューム アドオン (500 ジョブ) - Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6f270-637">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="6f270-638">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="6f270-638">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="6f270-639">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="6f270-639">9BI-00004</span></span>   |
| <span data-ttu-id="6f270-640">教職員用 Universal Print ボリューム アドオン (500 ジョブ) - Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6f270-640">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="6f270-641">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="6f270-641">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="6f270-642">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="6f270-642">9BK-00004</span></span>   |
| <span data-ttu-id="6f270-643">Universal Print ボリューム アドオン (500 ジョブ) - Windows</span><span class="sxs-lookup"><span data-stu-id="6f270-643">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="6f270-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="6f270-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="6f270-645">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="6f270-645">9BI-00002</span></span>   |
| <span data-ttu-id="6f270-646">教職員用 Universal Print ボリューム アドオン (500 ジョブ) - Windows</span><span class="sxs-lookup"><span data-stu-id="6f270-646">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="6f270-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="6f270-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="6f270-648">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="6f270-648">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="6f270-649">次のステップ</span><span class="sxs-lookup"><span data-stu-id="6f270-649">Next steps</span></span>

<span data-ttu-id="6f270-650">価格表と [Universal Print の概要](/universal-print/fundamentals/universal-print-whatis)についてご確認ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-650">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="6f270-651">この情報を組織内の適切なすべての担当者に共有してください。</span><span class="sxs-lookup"><span data-stu-id="6f270-651">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="6f270-652">ご質問がある場合は、</span><span class="sxs-lookup"><span data-stu-id="6f270-652">Questions?</span></span>

<span data-ttu-id="6f270-653">これらのプランについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="6f270-653">For any questions about these offers, check your relevant Yammer communities.</span></span>
