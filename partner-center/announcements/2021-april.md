---
title: 2021 年 4 月のお知らせ
description: 2021 年 4 月の Microsoft パートナー センターのお知らせでは、新しい機能、販売促進、オファー、市場、既存のオファーに対する変更を紹介します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 798dcb1570a0f6dfc94c7b45fc3c2e152f55cbe5
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702826"
---
# <a name="april-2021-announcements"></a><span data-ttu-id="329f6-103">2021 年 4 月のお知らせ</span><span class="sxs-lookup"><span data-stu-id="329f6-103">April 2021 announcements</span></span>

<span data-ttu-id="329f6-104">このページでは、2021 年 4 月の Microsoft パートナー センターのお知らせについて説明します。</span><span class="sxs-lookup"><span data-stu-id="329f6-104">This page provides the announcements for Microsoft Partner Center for April 2021.</span></span>

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a><span data-ttu-id="329f6-105">準備状況: 更新された CSP 顧客アドレス検証 API が 6 月に運用開始、テスト機能が現在利用可能</span><span class="sxs-lookup"><span data-stu-id="329f6-105">Readiness: Updated CSP customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="329f6-106">Categories</span><span class="sxs-lookup"><span data-stu-id="329f6-106">Categories</span></span>

- <span data-ttu-id="329f6-107">日付: 2021 年 4 月 30 日</span><span class="sxs-lookup"><span data-stu-id="329f6-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="329f6-108">準備</span><span class="sxs-lookup"><span data-stu-id="329f6-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="329f6-109">まとめ</span><span class="sxs-lookup"><span data-stu-id="329f6-109">Summary</span></span>

<span data-ttu-id="329f6-110">パートナーと顧客が信頼に基づいてビジネスを遂行できるようにするために、Microsoft はパートナーに対して世界中のすべての国の Validate Address API に対する変更をテストすることをお勧めしています。</span><span class="sxs-lookup"><span data-stu-id="329f6-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="329f6-111">対象</span><span class="sxs-lookup"><span data-stu-id="329f6-111">Impacted audience</span></span>

<span data-ttu-id="329f6-112">顧客の住所の詳細を新規作成または既存のものを更新する、CSP 直接請求パートナーと間接プロバイダー</span><span class="sxs-lookup"><span data-stu-id="329f6-112">CSP direct bill partners and indirect providers who create new or update existing customers’ address details</span></span>

### <a name="details"></a><span data-ttu-id="329f6-113">詳細</span><span class="sxs-lookup"><span data-stu-id="329f6-113">Details</span></span>

<span data-ttu-id="329f6-114">Microsoft の基盤は信頼です。</span><span class="sxs-lookup"><span data-stu-id="329f6-114">Microsoft runs on trust.</span></span> <span data-ttu-id="329f6-115">Microsoft は、CSP プログラムで顧客サブスクリプションを処理するために、法令に準拠した安全な顧客住所の検証方法の提供に努めています。</span><span class="sxs-lookup"><span data-stu-id="329f6-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="329f6-116">2021 年 3 月 31 日の時点で、Validate Address API に対する変更が発表されています。</span><span class="sxs-lookup"><span data-stu-id="329f6-116">As of March 31, 2021, we have introduced changes to the Validate Address API.</span></span> <span data-ttu-id="329f6-117">2021 年 6 月末の運用開始前にパートナーはこの API をテストすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="329f6-117">We invite partners to test the API prior to the  go-live at the end of June 2021.</span></span> 

<span data-ttu-id="329f6-118">これらの変更は、Validate Address API にのみ影響を与えることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="329f6-118">Note that these changes affect the Validate Address API only.</span></span> <span data-ttu-id="329f6-119">Create Customer と Update Billing Profile の API には影響がありません。</span><span class="sxs-lookup"><span data-stu-id="329f6-119">Create Customer and Update Billing Profile APIs aren’t affected.</span></span> <span data-ttu-id="329f6-120">提案された住所は現在、Create Customer API で使用する必要はありませんが、そうすることを強くお勧めします。</span><span class="sxs-lookup"><span data-stu-id="329f6-120">Although the suggested address doesn’t currently have to be used with the Create Customer API, it’s highly recommended.</span></span>

<span data-ttu-id="329f6-121">応答では、次のいずれかのステータス メッセージが返されます。</span><span class="sxs-lookup"><span data-stu-id="329f6-121">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="329f6-122">状態</span><span class="sxs-lookup"><span data-stu-id="329f6-122">Status</span></span>     | <span data-ttu-id="329f6-123">説明</span><span class="sxs-lookup"><span data-stu-id="329f6-123">Description</span></span> |    <span data-ttu-id="329f6-124">返される住所候補の数</span><span class="sxs-lookup"><span data-stu-id="329f6-124">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="329f6-125">Verified shippable (検証済み出荷可能)</span><span class="sxs-lookup"><span data-stu-id="329f6-125">Verified shippable</span></span> | <span data-ttu-id="329f6-126">住所が確認され、出荷可能です。</span><span class="sxs-lookup"><span data-stu-id="329f6-126">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="329f6-127">Single</span><span class="sxs-lookup"><span data-stu-id="329f6-127">Single</span></span> |
|<span data-ttu-id="329f6-128">Verified</span><span class="sxs-lookup"><span data-stu-id="329f6-128">Verified</span></span> | <span data-ttu-id="329f6-129">住所が確認されました。</span><span class="sxs-lookup"><span data-stu-id="329f6-129">Address is verified.</span></span> | <span data-ttu-id="329f6-130">Single</span><span class="sxs-lookup"><span data-stu-id="329f6-130">Single</span></span> |
|<span data-ttu-id="329f6-131">Interaction required (対話式操作が必要)</span><span class="sxs-lookup"><span data-stu-id="329f6-131">Interaction required</span></span> | <span data-ttu-id="329f6-132">提案された住所は大幅に変更されており、ユーザーの確認が必要です。</span><span class="sxs-lookup"><span data-stu-id="329f6-132">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="329f6-133">Single</span><span class="sxs-lookup"><span data-stu-id="329f6-133">Single</span></span> |
|<span data-ttu-id="329f6-134">Street partial (番地が不完全)</span><span class="sxs-lookup"><span data-stu-id="329f6-134">Street partial</span></span> | <span data-ttu-id="329f6-135">住所の番地が部分的であるため、さらに情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="329f6-135">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="329f6-136">複数 (最大 3)</span><span class="sxs-lookup"><span data-stu-id="329f6-136">Multiple—maximum of three</span></span> |
|<span data-ttu-id="329f6-137">Premises partial (建物が不完全)</span><span class="sxs-lookup"><span data-stu-id="329f6-137">Premises partial</span></span> | <span data-ttu-id="329f6-138">指定された建物 (ビル番号、部屋番号、その他) が不完全であるため、さらに情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="329f6-138">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="329f6-139">複数 (最大 3)</span><span class="sxs-lookup"><span data-stu-id="329f6-139">Multiple—maximum of three</span></span> |
|<span data-ttu-id="329f6-140">複数</span><span class="sxs-lookup"><span data-stu-id="329f6-140">Multiple</span></span> | <span data-ttu-id="329f6-141">住所の複数のフィールドが不完全です (street partial と premises partial も含む可能性があります)。</span><span class="sxs-lookup"><span data-stu-id="329f6-141">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="329f6-142">複数 (最大 3)</span><span class="sxs-lookup"><span data-stu-id="329f6-142">Multiple—maximum of three</span></span> |
|<span data-ttu-id="329f6-143">なし</span><span class="sxs-lookup"><span data-stu-id="329f6-143">None</span></span> | <span data-ttu-id="329f6-144">住所が正しくありません。</span><span class="sxs-lookup"><span data-stu-id="329f6-144">Address is incorrect.</span></span> | <span data-ttu-id="329f6-145">なし</span><span class="sxs-lookup"><span data-stu-id="329f6-145">None</span></span> |
|<span data-ttu-id="329f6-146">検証なし</span><span class="sxs-lookup"><span data-stu-id="329f6-146">Not validated</span></span> | <span data-ttu-id="329f6-147">住所は、検証プロセスを通じて送信できませんでした。</span><span class="sxs-lookup"><span data-stu-id="329f6-147">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="329f6-148">なし</span><span class="sxs-lookup"><span data-stu-id="329f6-148">None</span></span> |

<span data-ttu-id="329f6-149">米国の郵便番号は、ハイフン付きでさらに 4 桁が返されます (例: 12345-6789)。</span><span class="sxs-lookup"><span data-stu-id="329f6-149">US post codes will return an additional four digits + hyphen, for example, 12345-6789.</span></span>

### <a name="next-steps"></a><span data-ttu-id="329f6-150">次のステップ</span><span class="sxs-lookup"><span data-stu-id="329f6-150">Next steps</span></span>

- <span data-ttu-id="329f6-151">詳細なガイダンスについては、[専用のパートナー コレクション](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)でテクニカル ドキュメントとよく寄せられる質問を参照してください。</span><span class="sxs-lookup"><span data-stu-id="329f6-151">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="329f6-152">Partner Center API と Web ユーザー エクスペリエンスを使用して、変更を組み込む準備をしてください。</span><span class="sxs-lookup"><span data-stu-id="329f6-152">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> 
- <span data-ttu-id="329f6-153">テスト フライトに含められるようにサンドボックスのテナント ID を領域の専門家 (Ali Khaki) に知らせます。これにより、更新の準備を開始できます。</span><span class="sxs-lookup"><span data-stu-id="329f6-153">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span> 
- <span data-ttu-id="329f6-154">コントロール パネル ベンダー (CPV) ソリューションを使用している場合は、CPV とご相談ください。</span><span class="sxs-lookup"><span data-stu-id="329f6-154">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="329f6-155">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="329f6-155">Questions?</span></span>

<span data-ttu-id="329f6-156">Microsoft との連携でサポートが必要な場合は、パートナー サポートの Yammer グループに問い合わせるか、[サービス要求](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)を開いてください。</span><span class="sxs-lookup"><span data-stu-id="329f6-156">If you need support for your operations with Microsoft, reach out to your partner support Yammer group or open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a><span data-ttu-id="329f6-157">パートナー センター API の Swagger ドキュメントの新しい場所</span><span class="sxs-lookup"><span data-stu-id="329f6-157">New location for Partner Center API Swagger documentation</span></span>

### <a name="categories"></a><span data-ttu-id="329f6-158">Categories</span><span class="sxs-lookup"><span data-stu-id="329f6-158">Categories</span></span>

- <span data-ttu-id="329f6-159">日付: 2021 年 4 月 26 日</span><span class="sxs-lookup"><span data-stu-id="329f6-159">Date: 2021-04-26</span></span>
- <span data-ttu-id="329f6-160">機能</span><span class="sxs-lookup"><span data-stu-id="329f6-160">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="329f6-161">まとめ</span><span class="sxs-lookup"><span data-stu-id="329f6-161">Summary</span></span>

<span data-ttu-id="329f6-162">パートナー センター API の Swagger ドキュメントは、[前の Swagger ドキュメント サイト](https://apidocs.microsoft.com/services/partnercenter)から[新しい Swagger ドキュメント サイト](https://docs.microsoft.com/rest/api/partner-center-rest/)に移行されました。</span><span class="sxs-lookup"><span data-stu-id="329f6-162">Partner Center API Swagger documents have been migrated from the [previous Swagger Documentation site](https://apidocs.microsoft.com/services/partnercenter) to a [new Swagger Documentation site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="329f6-163">対象</span><span class="sxs-lookup"><span data-stu-id="329f6-163">Impacted audience</span></span>

<span data-ttu-id="329f6-164">パートナー センター API を使用し、クラウド ソリューション プロバイダー (CSP) プログラムに参加している直接請求パートナーと間接プロバイダー</span><span class="sxs-lookup"><span data-stu-id="329f6-164">Direct bill partners and Indirect Providers participating in the Cloud Solution Provider (CSP) program who are using the Partner Center APIs</span></span>

### <a name="details"></a><span data-ttu-id="329f6-165">詳細</span><span class="sxs-lookup"><span data-stu-id="329f6-165">Details</span></span>

<span data-ttu-id="329f6-166">2021 年 4 月 26 日の時点で、パートナー センター API の Swagger ドキュメント (Rest API コンテンツを含む) は[新しいサイト](https://docs.microsoft.com/rest/api/partner-center-rest/)に配置されています。</span><span class="sxs-lookup"><span data-stu-id="329f6-166">As of April 26, 2021 the Partner Center API Swagger documentation, including Rest API content, is located on a [new site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span> <span data-ttu-id="329f6-167">古いサイトは数週間後にアクセスできなくなります。</span><span class="sxs-lookup"><span data-stu-id="329f6-167">The old site will be inaccessible after several weeks.</span></span>

### <a name="benefits"></a><span data-ttu-id="329f6-168">メリット</span><span class="sxs-lookup"><span data-stu-id="329f6-168">Benefits</span></span>

<span data-ttu-id="329f6-169">パートナー センター API の Swagger ドキュメントには、**Try It** (試用) 機能があります。</span><span class="sxs-lookup"><span data-stu-id="329f6-169">The Partner Center API Swagger documentation will provide a **Try It** function.</span></span> <span data-ttu-id="329f6-170">この機能を使用するには、ベアラー トークンが必要です。これは、[パートナー センターの認証](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication)に関する記事に記載されている手順に従って生成できます。</span><span class="sxs-lookup"><span data-stu-id="329f6-170">To use this function, you’ll need to have a Bearer Token, which you can generate by following the steps listed in [Partner Center Authentication](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication).</span></span>

### <a name="next-steps"></a><span data-ttu-id="329f6-171">次の手順</span><span class="sxs-lookup"><span data-stu-id="329f6-171">Next steps</span></span>

<span data-ttu-id="329f6-172">担当チームが手続きの見直し、更新を実施できるよう、この情報を組織で共有してください。</span><span class="sxs-lookup"><span data-stu-id="329f6-172">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="329f6-173">疑問がある場合</span><span class="sxs-lookup"><span data-stu-id="329f6-173">Questions?</span></span>

<span data-ttu-id="329f6-174">これらのオファーに関するご質問については、Yammer の関連コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="329f6-174">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a><span data-ttu-id="329f6-175">クラウド ソリューション プロバイダー (CSP) ソフトウェア返品期間ポリシーとダウンロード リンクの有効期限に関する通知</span><span class="sxs-lookup"><span data-stu-id="329f6-175">Cloud Solution Provider (CSP) software return period policy and download link expiry notice</span></span>

### <a name="categories"></a><span data-ttu-id="329f6-176">Categories</span><span class="sxs-lookup"><span data-stu-id="329f6-176">Categories</span></span>

- <span data-ttu-id="329f6-177">日付: 2021-04-21</span><span class="sxs-lookup"><span data-stu-id="329f6-177">Date: 2021-04-21</span></span>
- <span data-ttu-id="329f6-178">機能</span><span class="sxs-lookup"><span data-stu-id="329f6-178">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="329f6-179">まとめ</span><span class="sxs-lookup"><span data-stu-id="329f6-179">Summary</span></span>

<span data-ttu-id="329f6-180">CSP ソフトウェア返品期間ポリシーとダウンロード リンクの有効期限に変更点があります。</span><span class="sxs-lookup"><span data-stu-id="329f6-180">There are changes to the CSP software return period policy and download link expiry.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="329f6-181">対象</span><span class="sxs-lookup"><span data-stu-id="329f6-181">Impacted audience</span></span>

<span data-ttu-id="329f6-182">CSP で永続的ソフトウェアまたはソフトウェア サブスクリプション プランの取引を行っているパートナー</span><span class="sxs-lookup"><span data-stu-id="329f6-182">Partners transacting perpetual software or software subscription offers in CSP</span></span>

### <a name="details"></a><span data-ttu-id="329f6-183">詳細</span><span class="sxs-lookup"><span data-stu-id="329f6-183">Details</span></span>

<span data-ttu-id="329f6-184">パートナー センターを介した永続的ソフトウェアまたはソフトウェア サブスクリプションの購入に関して次の重要な通知にご注意ください。</span><span class="sxs-lookup"><span data-stu-id="329f6-184">Note the following important notifications regarding perpetual software and software subscription purchases through Partner Center:</span></span>

#### <a name="software-return-period-policy"></a><span data-ttu-id="329f6-185">ソフトウェアの返品期間ポリシー</span><span class="sxs-lookup"><span data-stu-id="329f6-185">Software return period policy</span></span>

<span data-ttu-id="329f6-186">2021 年 6 月 1 日から、Microsoft Partner Agreement (MPA) に記載されているように、CSP のソフトウェア プランの返品期間が、注文日から 60 日間から 30 日間に変更されます。</span><span class="sxs-lookup"><span data-stu-id="329f6-186">From June 1, 2021, the return period for software offers in CSP, as stated in the Microsoft Partner Agreement (MPA), will change from 60 days from order date to 30 days from order date.</span></span>

<span data-ttu-id="329f6-187">ソフトウェア プランの注文が送信されると、パートナーは注文日から 30 日以内であれば、そのような注文への変更を送信できます。</span><span class="sxs-lookup"><span data-stu-id="329f6-187">After an order for a software offer is submitted, partners will have 30 days from the order date to submit any revisions to such order:</span></span>

- <span data-ttu-id="329f6-188">30 日間の返品期間内に返されたすべての永続的なソフトウェア ライセンスには、支払済み購入価格のフル クレジットが付与されます。</span><span class="sxs-lookup"><span data-stu-id="329f6-188">Any perpetual software license returned within the 30-day return period will receive a full credit of the paid purchase price.</span></span>

- <span data-ttu-id="329f6-189">30 日間の返品期間内に返されたすべてのソフトウェア サブスクリプション製品には、支払済み購入価格の日割り計算のクレジットが付与されます。</span><span class="sxs-lookup"><span data-stu-id="329f6-189">Any software subscription product returned within the 30-day return period will receive a prorated credit of the paid purchase price.</span></span>

<span data-ttu-id="329f6-190">このメッセージは、2020 年 12 月と 2021 年 4 月に、返品期間や MPS へのその他の更新に関してすべての CSP パートナーに送信された電子メール通信の補足情報です。</span><span class="sxs-lookup"><span data-stu-id="329f6-190">This message is a follow-up to our email communications sent on December 2020 and April 2021 to all CSP partners regarding the return period and other updates to the MPA.</span></span> <span data-ttu-id="329f6-191">MPA に影響する変更に関する詳細については、これらの通知を参照してください。</span><span class="sxs-lookup"><span data-stu-id="329f6-191">Refer to those notices for full details regarding changes affecting the MPA.</span></span>

#### <a name="software-download-link-expiry"></a><span data-ttu-id="329f6-192">ソフトウェアのダウンロード リンクの有効期限</span><span class="sxs-lookup"><span data-stu-id="329f6-192">Software download link expiry</span></span>

<span data-ttu-id="329f6-193">2021 年 6 月 3 日以降、パートナー センターを通じた永続的ソフトウェアおよびソフトウェア サブスクリプション製品の購入におけるソフトウェアのダウンロード リンクについて、最初のダウンロードから 5 日間の有効期限が設けられます。</span><span class="sxs-lookup"><span data-stu-id="329f6-193">From June 3, 2021, the software download links for perpetual software and software subscription product purchases through Partner Center will have an expiration date of five days from the initial download.</span></span> <span data-ttu-id="329f6-194">有効期限は、2021 年 6 月 3 日より前と 2021 年 6 月 3 日以降のすべての購入に適用されます。</span><span class="sxs-lookup"><span data-stu-id="329f6-194">The expiry period will apply to all purchases before June 3, 2021, as well as on or after June 3, 2021.</span></span>

### <a name="next-steps"></a><span data-ttu-id="329f6-195">次のステップ</span><span class="sxs-lookup"><span data-stu-id="329f6-195">Next steps</span></span>

<span data-ttu-id="329f6-196">[CSP の返品期間とダウンロード リンクの有効期限に関する FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf) を確認し、これらの変更を組織内のすべての適切なチームに通知しましょう。</span><span class="sxs-lookup"><span data-stu-id="329f6-196">Review the [CSP return period and download link expiry FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), and inform all appropriate teams within your organization of these changes:</span></span>

### <a name="questions"></a><span data-ttu-id="329f6-197">疑問がある場合</span><span class="sxs-lookup"><span data-stu-id="329f6-197">Questions?</span></span>

<span data-ttu-id="329f6-198">これらのオファーに関するご質問については、Yammer の関連コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="329f6-198">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a><span data-ttu-id="329f6-199">オープン ライセンス プログラム: クラウド ソリューション プロバイダー (CSP) プログラムへのリセラーの移行</span><span class="sxs-lookup"><span data-stu-id="329f6-199">Open Licensing program: Transitioning resellers to the Cloud Solution Provider (CSP) program</span></span>

### <a name="categories"></a><span data-ttu-id="329f6-200">Categories</span><span class="sxs-lookup"><span data-stu-id="329f6-200">Categories</span></span>

- <span data-ttu-id="329f6-201">日付 : 2021 年 4 月 19 日</span><span class="sxs-lookup"><span data-stu-id="329f6-201">Date: 2021-04-19</span></span>
- <span data-ttu-id="329f6-202">ビジネスの拡大</span><span class="sxs-lookup"><span data-stu-id="329f6-202">Grow Your Business</span></span>

### <a name="summary"></a><span data-ttu-id="329f6-203">まとめ</span><span class="sxs-lookup"><span data-stu-id="329f6-203">Summary</span></span>

<span data-ttu-id="329f6-204">この通信では、オープン ライセンス プログラムに近日行われる変更に備える方法を記載しています。</span><span class="sxs-lookup"><span data-stu-id="329f6-204">This communication details how to prepare for the changes that are coming soon to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="329f6-205">対象</span><span class="sxs-lookup"><span data-stu-id="329f6-205">Impacted audience</span></span>

<span data-ttu-id="329f6-206">CSP と Open License パートナー</span><span class="sxs-lookup"><span data-stu-id="329f6-206">CSP and Open License partners</span></span>

### <a name="details"></a><span data-ttu-id="329f6-207">詳細</span><span class="sxs-lookup"><span data-stu-id="329f6-207">Details</span></span>

<span data-ttu-id="329f6-208">2020 年、Microsoft は、クラウド ソリューション プロバイダー (CSP) プログラムを通じてパートナーとお客様が永続的ソフトウェア ライセンスを幅広くご利用いただけるようになることを[発表](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/)しました。</span><span class="sxs-lookup"><span data-stu-id="329f6-208">In 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) that perpetual software licenses will be broadly available to partners and customers through the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="329f6-209">最初のマイルストーンには、商用の永続的ソフトウェア プランが利用可能になった 2021 年 1 月時点で到達しました。</span><span class="sxs-lookup"><span data-stu-id="329f6-209">The first milestone was reached in January 2021, when commercial perpetual software offers became available.</span></span> <span data-ttu-id="329f6-210">次の主要なマイルストーンは、[公的機関](https://aka.ms/openlicensepublicsector)のプランが利用可能になる 2021 年 7 月に発生します。</span><span class="sxs-lookup"><span data-stu-id="329f6-210">The next key milestone will happen in July 2021, when [public sector](https://aka.ms/openlicensepublicsector) offers become available.</span></span> <span data-ttu-id="329f6-211">2022 年 1 月 1 日より、Open License プログラムを通じてソフトウェア アシュアランスまたはオンライン サービスの新しいソフトウェア ライセンスの購入または更新を行えなくなる旨も[お伝えしました](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/)。</span><span class="sxs-lookup"><span data-stu-id="329f6-211">We also [communicated](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) that effective January 1, 2022, no new software license purchases or renewals of Software Assurance or online services can be made through the Open License program.</span></span>

<span data-ttu-id="329f6-212">新しいコマース エクスペリエンスで永続的ソフトウェアを CSP プログラムに移行することで、パートナーはさまざまなソリューションやマネージド サービスを提供する機会を広げることができます。</span><span class="sxs-lookup"><span data-stu-id="329f6-212">The transition of perpetual software to the CSP program in the new commerce experience will help partners to expand the opportunities to offer diverse solutions and managed services.</span></span> <span data-ttu-id="329f6-213">これにより、お客様のクラウドへの移行も促進されます。</span><span class="sxs-lookup"><span data-stu-id="329f6-213">This will also accelerate customers’ transition to the cloud.</span></span>  <span data-ttu-id="329f6-214">パートナーとお客様両方の円滑な移行を実現するために、こうした調整を行い、このデジタル変革を促進するための資料をご用意しました。</span><span class="sxs-lookup"><span data-stu-id="329f6-214">To help ensure a smooth transition for both our partners and customers, we’ve made these adjustments and materials to accelerate this digital transformation:</span></span>

#### <a name="april-2021"></a><span data-ttu-id="329f6-215">2021 年 4 月</span><span class="sxs-lookup"><span data-stu-id="329f6-215">April 2021</span></span>

<span data-ttu-id="329f6-216">[提供中](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): リセラー向けの Open License から CSP への移行に関する資料</span><span class="sxs-lookup"><span data-stu-id="329f6-216">[Now available](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Open License-to-CSP transition materials for resellers</span></span>

#### <a name="july-2021"></a><span data-ttu-id="329f6-217">2021 年 7 月</span><span class="sxs-lookup"><span data-stu-id="329f6-217">July 2021</span></span>

##### <a name="csp"></a><span data-ttu-id="329f6-218">CSP</span><span class="sxs-lookup"><span data-stu-id="329f6-218">CSP</span></span>

- <span data-ttu-id="329f6-219">7 月 1 日: 永続的ソフトウェア ライセンスを公的機関のお客様が利用可能に</span><span class="sxs-lookup"><span data-stu-id="329f6-219">July 1: Perpetual software licenses available to public sector customers</span></span>

- <span data-ttu-id="329f6-220">7 月 7 日: Visual Studio Pro および Get Genuine Windows Agreement の永続的なソフトウェア ライセンスがすべてのセグメントで利用可能に</span><span class="sxs-lookup"><span data-stu-id="329f6-220">July 7: Visual Studio Pro and Get Genuine Windows Agreement  perpetual software licenses available to all segments</span></span>

##### <a name="open-value"></a><span data-ttu-id="329f6-221">オープン バリュー</span><span class="sxs-lookup"><span data-stu-id="329f6-221">Open Value</span></span>

- <span data-ttu-id="329f6-222">7 月 1 日: 追加の SKU が教育および非営利向けの Open Value プログラムで利用可能に。Open License プログラムに似たプランを提供します。</span><span class="sxs-lookup"><span data-stu-id="329f6-222">July 1: Additional SKUs available in the Open Value program for education and nonprofit, providing similar offers to the Open License program</span></span>

##### <a name="open-license"></a><span data-ttu-id="329f6-223">オープン ライセンス</span><span class="sxs-lookup"><span data-stu-id="329f6-223">Open License</span></span>

- <span data-ttu-id="329f6-224">7 月 1 日: Microsoft による Open License プログラムでの新しいプランの発表はなくなります。</span><span class="sxs-lookup"><span data-stu-id="329f6-224">July 1: Microsoft will no longer launch new offers in the Open License program.</span></span>

#### <a name="january-2022"></a><span data-ttu-id="329f6-225">2022 年 1 月</span><span class="sxs-lookup"><span data-stu-id="329f6-225">January 2022</span></span>

- <span data-ttu-id="329f6-226">1 月 1 日: Open License プログラムで新しい購入や更新を行うことはできなくなります。</span><span class="sxs-lookup"><span data-stu-id="329f6-226">January 1: No new purchases or renewals can be made through the Open License program</span></span>

### <a name="next-steps"></a><span data-ttu-id="329f6-227">次のステップ</span><span class="sxs-lookup"><span data-stu-id="329f6-227">Next steps</span></span>

#### <a name="csp-indirect-providers"></a><span data-ttu-id="329f6-228">CSP 間接プロバイダー</span><span class="sxs-lookup"><span data-stu-id="329f6-228">CSP indirect providers</span></span>

<span data-ttu-id="329f6-229">今後数か月間で、パートナー コミュニティのイベントに参加し、リセラー向けの Open License から CSP への移行に関する資料を使用して、Open License リセラーの CSP プログラムへの移行を進めます。</span><span class="sxs-lookup"><span data-stu-id="329f6-229">Use the coming months to help Open License resellers orient into the CSP program by attending partner community events and using the Open License-to-CSP transition materials for resellers:</span></span>

- <span data-ttu-id="329f6-230">[リセラー向けの Open License から CSP への移行に関する資料](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—カスタマイズ可能な概要プレゼンテーション、電子メール テンプレート、CSP 間接リセラー オンボード ガイドなどを利用して、大規模なリセラーの導入を促進することができます。</span><span class="sxs-lookup"><span data-stu-id="329f6-230">[Open License-to-CSP transition materials for resellers](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—Customizable overview presentation, email template, CSP indirect reseller onboarding guide, and more to help you drive the adoption for your resellers at scale.</span></span>

- <span data-ttu-id="329f6-231">Microsoft Business Operations 主催の [CSP パートナー コミュニティ イベント](https://globalpbocomm.eventbuilder.com/GlobalCSP)。</span><span class="sxs-lookup"><span data-stu-id="329f6-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) hosted by Microsoft Business Operations.</span></span>  <span data-ttu-id="329f6-232">さまざまなセッションに参加して、CSP の基本 (CSP の基礎) を確認したり、最新の情報を入手したり、Software in CSP に関する質問をしたり (Q&A セッション) することができます。</span><span class="sxs-lookup"><span data-stu-id="329f6-232">Join the various sessions to learn CSP basics (CSP Fundamentals) or stay up to date, and ask questions regarding Software in CSP (Q&A Sessions).</span></span>

- <span data-ttu-id="329f6-233">(近日公開予定) Microsoft Business Operations 主催の CSP 間接リセラー向けトレーニング セッション。</span><span class="sxs-lookup"><span data-stu-id="329f6-233">(Coming soon) CSP indirect reseller–focused training session hosted by Microsoft Business Operations.</span></span>

#### <a name="open-license-resellers"></a><span data-ttu-id="329f6-234">Open License リセラー</span><span class="sxs-lookup"><span data-stu-id="329f6-234">Open License resellers</span></span>

- <span data-ttu-id="329f6-235">組織が現在 CSP プログラムに登録されていない場合は、開始方法について、ディストリビューターにお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="329f6-235">If your organization isn’t currently enrolled in the CSP program, contact your distributor for information on how to get started.</span></span> <span data-ttu-id="329f6-236">間接プロバイダーと[こちら](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider)から連携できます。</span><span class="sxs-lookup"><span data-stu-id="329f6-236">Connect with an indirect provider [here](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span></span>

- <span data-ttu-id="329f6-237">組織が既に CSP プログラムに登録されている場合は、CSP の永続的ソフトウェアの詳細について、[こちら](https://partner.microsoft.com/resources/collection/software-in-csp)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="329f6-237">If your organization is already enrolled in the CSP program, learn more about perpetual software in CSP [here](https://partner.microsoft.com/resources/collection/software-in-csp).</span></span>

### <a name="questions"></a><span data-ttu-id="329f6-238">疑問がある場合</span><span class="sxs-lookup"><span data-stu-id="329f6-238">Questions?</span></span>

<span data-ttu-id="329f6-239">これらのオファーについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="329f6-239">For further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a><span data-ttu-id="329f6-240">公開中: グローバル プロモーション準備ガイド</span><span class="sxs-lookup"><span data-stu-id="329f6-240">Now live: Global promo readiness guide</span></span>

### <a name="categories"></a><span data-ttu-id="329f6-241">Categories</span><span class="sxs-lookup"><span data-stu-id="329f6-241">Categories</span></span>

- <span data-ttu-id="329f6-242">日付: 2021 年 4 月 16 日</span><span class="sxs-lookup"><span data-stu-id="329f6-242">Date: 2021-04-16</span></span>
- <span data-ttu-id="329f6-243">機能</span><span class="sxs-lookup"><span data-stu-id="329f6-243">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="329f6-244">まとめ</span><span class="sxs-lookup"><span data-stu-id="329f6-244">Summary</span></span>

<span data-ttu-id="329f6-245">Launch Readiness が、Operations Readiness リソース ギャラリーに[グローバル プロモーション準備ガイド](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf)を公開しました。</span><span class="sxs-lookup"><span data-stu-id="329f6-245">Launch Readiness has published a new [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) on the Operations Readiness resource gallery.</span></span> <span data-ttu-id="329f6-246">このガイドは、すべてのアクティブな[グローバル販売促進](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)を統合的に表示します。</span><span class="sxs-lookup"><span data-stu-id="329f6-246">This guide provides a consolidated view of all active [global promotions](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="329f6-247">対象</span><span class="sxs-lookup"><span data-stu-id="329f6-247">Impacted audience</span></span>

<span data-ttu-id="329f6-248">すべてのボリューム ライセンス (VL)、Dynamics Price List (DPL)、およびクラウド ソリューション プロバイダー (CSP) パートナー</span><span class="sxs-lookup"><span data-stu-id="329f6-248">All Volume Licensing (VL), Dynamics Price List (DPL), and Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="329f6-249">詳細</span><span class="sxs-lookup"><span data-stu-id="329f6-249">Details</span></span>

<span data-ttu-id="329f6-250">Microsoft パートナーから、すべてのグローバル プロモーションとその詳細について統合されたビューを提供してほしいという要望がありました。</span><span class="sxs-lookup"><span data-stu-id="329f6-250">Microsoft partners have shared with us the need to provide a consolidated view of all global promotions with supporting details.</span></span> <span data-ttu-id="329f6-251">この統合ガイドを使用すると、利用可能なすべての情報に一元的かつ便利な場所で簡単にアクセスできるという安心感の中、プロモーションを利用できます。</span><span class="sxs-lookup"><span data-stu-id="329f6-251">You wanted this consolidated guide to help you use promotions with the confidence that all the available information will be readily accessible in a central and convenient location.</span></span>

<span data-ttu-id="329f6-252">2021 年 4 月から、Microsoft はこのガイドを毎月更新し、ガイドは Operations Readiness リソース ギャラリーの専用グローバル プロモーション準備ガイド コレクションで利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="329f6-252">Beginning in April 2021, Microsoft will update this guide on a monthly basis, and it will be available in a dedicated Global Promo Readiness Guide collection in the Operations Readiness resource gallery.</span></span>

<span data-ttu-id="329f6-253">このガイドへのリンクは、次のコレクションにも含まれます。</span><span class="sxs-lookup"><span data-stu-id="329f6-253">Links to this guide will also be included in the following collections:</span></span>

- <span data-ttu-id="329f6-254">[製品発表予定表コレクション](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/)。今後の変更や発表を一元的に表示できます。</span><span class="sxs-lookup"><span data-stu-id="329f6-254">[Launch calendar collection](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), which provides a centralized view of upcoming changes and launches.</span></span>

- <span data-ttu-id="329f6-255">[コミュニティ コレクション](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)。月次パートナー コールのサポート資料が含まれ、今後の変更や、運用上興味深いタイムリーなトピックを中心に扱います。</span><span class="sxs-lookup"><span data-stu-id="329f6-255">[Community collections](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), which contain supporting materials for our monthly partner calls, highlighting upcoming changes and timely topics of operational interest.</span></span>

- <span data-ttu-id="329f6-256">[パートナー ニュースレター](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)。CSP の月ごとの更新ニュースレター</span><span class="sxs-lookup"><span data-stu-id="329f6-256">[Partner newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), such as CSP Monthly Update</span></span>

<span data-ttu-id="329f6-257">毎月のリマインダーとして、グローバル プロモーション準備ガイドの最新刊と共に、パートナー センターのお知らせも公開されます。</span><span class="sxs-lookup"><span data-stu-id="329f6-257">As a monthly reminder, we will also publish a Partner Center announcement with each new issue of the global promo readiness guide.</span></span>

### <a name="next-steps"></a><span data-ttu-id="329f6-258">次のステップ</span><span class="sxs-lookup"><span data-stu-id="329f6-258">Next steps</span></span>

<span data-ttu-id="329f6-259">各月の開始時に、[Operations Readiness リソースギャラリー](https://partner.microsoft.com/resources)に最新の[グローバル プロモーション準備ガイド](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf)が掲載されます。</span><span class="sxs-lookup"><span data-stu-id="329f6-259">At the start of each month, you will find the latest [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources).</span></span>

<span data-ttu-id="329f6-260">この情報を組織内の適切な担当者と共有し、各ページの最後の「このページは役に立ちましたか?」</span><span class="sxs-lookup"><span data-stu-id="329f6-260">Share this information with the appropriate contacts in your organizations and let us know how helpful the guide is through the “Was this page helpful?”</span></span> <span data-ttu-id="329f6-261">ボタンを押して、ガイドがどのくらい役立ったかをお聞かせください。</span><span class="sxs-lookup"><span data-stu-id="329f6-261">button at the end of each page.</span></span>

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a><span data-ttu-id="329f6-262">4 月のクラウド ソリューション プロバイダー (CSP) コミュニティの更新とリマインダー</span><span class="sxs-lookup"><span data-stu-id="329f6-262">April Cloud Solution Provider (CSP) community update and reminders</span></span>

### <a name="categories"></a><span data-ttu-id="329f6-263">Categories</span><span class="sxs-lookup"><span data-stu-id="329f6-263">Categories</span></span>

- <span data-ttu-id="329f6-264">日付: 2021 年 4 月 16 日</span><span class="sxs-lookup"><span data-stu-id="329f6-264">Date: 2021-04-16</span></span>
- <span data-ttu-id="329f6-265">コミュニティ | 招待とリマインダー</span><span class="sxs-lookup"><span data-stu-id="329f6-265">Community | Invites and reminders</span></span>

### <a name="summary"></a><span data-ttu-id="329f6-266">まとめ</span><span class="sxs-lookup"><span data-stu-id="329f6-266">Summary</span></span>

<span data-ttu-id="329f6-267">オンデマンドで利用できる CSP コミュニティ リソースは毎月更新されるため、常に最新情報を入手し、CSP プログラムの変更に備えることができます。</span><span class="sxs-lookup"><span data-stu-id="329f6-267">CSP community resources are available on demand and updated monthly to keep you informed and prepared for change in the CSP program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="329f6-268">対象</span><span class="sxs-lookup"><span data-stu-id="329f6-268">Impacted audience</span></span>

<span data-ttu-id="329f6-269">CSP 直接請求パートナーおよび間接プロバイダー</span><span class="sxs-lookup"><span data-stu-id="329f6-269">CSP direct bill partners and indirect providers</span></span>

### <a name="details"></a><span data-ttu-id="329f6-270">詳細</span><span class="sxs-lookup"><span data-stu-id="329f6-270">Details</span></span>

<span data-ttu-id="329f6-271">今月、リソースには、次の主要なトピックが含まれています。</span><span class="sxs-lookup"><span data-stu-id="329f6-271">This month, the resources include the following key topics:</span></span>

- [<span data-ttu-id="329f6-272">CSP プログラムの進化の更新と Open License プログラムの変更</span><span class="sxs-lookup"><span data-stu-id="329f6-272">Update to CSP program evolution and Open License program changes</span></span>](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [<span data-ttu-id="329f6-273">特定の地域での CSP のお客様のオンボード要件の変更</span><span class="sxs-lookup"><span data-stu-id="329f6-273">Changes to CSP customer onboarding requirements in certain regions</span></span>](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [<span data-ttu-id="329f6-274">CSP プログラムでの新しいコマース PDF 請求書の新しい形式</span><span class="sxs-lookup"><span data-stu-id="329f6-274">New format for the new commerce PDF invoice in the CSP program</span></span>](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

<span data-ttu-id="329f6-275">[CSP コミュニティ コレクション](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)には、以下が見つかります。</span><span class="sxs-lookup"><span data-stu-id="329f6-275">Within the [CSP community collection](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), you’ll find:</span></span>

- <span data-ttu-id="329f6-276">ダウンロード可能な [CSP の月ごとの更新ニュースレター](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)。最近の CSP のお知らせ、更新プログラム、イベント、リマインダーを、読みやすいドキュメントに集計します。</span><span class="sxs-lookup"><span data-stu-id="329f6-276">The downloadable [CSP Monthly Update newsletter](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), which aggregates recent CSP announcements, updates, events, and reminders in an easy-to-read document.</span></span>

- <span data-ttu-id="329f6-277">[CSP のお知らせカレンダー](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)。プログラムに影響を与える今後の変更のタイムライン ビューを提供します。</span><span class="sxs-lookup"><span data-stu-id="329f6-277">The [CSP Announcement Calendar](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), which provides a timeline view of upcoming changes affecting the program.</span></span>

- <span data-ttu-id="329f6-278">新しい[製品の発売予定表](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)。今後の製品の発表とプランをご覧いただけます。</span><span class="sxs-lookup"><span data-stu-id="329f6-278">The new [product launch calendar](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), where you can view upcoming product launches and offers.</span></span>

- <span data-ttu-id="329f6-279">[CSP 製品発表更新リソース](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/)には、主要な運用上の変更に関する簡単に使用できるコンテンツが含まれています。</span><span class="sxs-lookup"><span data-stu-id="329f6-279">[CSP launch update resources](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) with easy-to-consume content on key operational changes.</span></span>

- <span data-ttu-id="329f6-280">関心や質問を受け付ける CSP の主要なトピックに関する[リフレッシャーとリマインダー](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf)。</span><span class="sxs-lookup"><span data-stu-id="329f6-280">[Refreshers and reminders](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) on key CSP topics receiving interest and queries.</span></span>

#### <a name="csp-community-call-qas"></a><span data-ttu-id="329f6-281">CSP コミュニティ コールに関する Q&A</span><span class="sxs-lookup"><span data-stu-id="329f6-281">CSP Community Call Q&As</span></span>

<span data-ttu-id="329f6-282">コミュニティ コールの Q&A は、今後の変更に関する質問がある場合に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="329f6-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span></span> <span data-ttu-id="329f6-283">4 月、5 月、6 月に開催される CSP コミュニティ コールの Q&A に今すぐ登録しましょう。</span><span class="sxs-lookup"><span data-stu-id="329f6-283">Register now for CSP Community Call Q&As that are taking place in April, May, and June.</span></span> <span data-ttu-id="329f6-284">ここでは、最新の発表、重要なリフレッシャー、リマインダーにフォーカスが置かれます。</span><span class="sxs-lookup"><span data-stu-id="329f6-284">These will focus on the latest launches, important refreshers, and reminders.</span></span>

<span data-ttu-id="329f6-285">[こちらからご登録ください](https://globalpbocomm.eventbuilder.com/GlobalCSP)。</span><span class="sxs-lookup"><span data-stu-id="329f6-285">[Register here](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span></span>

### <a name="next-steps"></a><span data-ttu-id="329f6-286">次のステップ</span><span class="sxs-lookup"><span data-stu-id="329f6-286">Next steps</span></span>

<span data-ttu-id="329f6-287">コミュニティのリソースを確認し、コミュニティ コールの Q&A に登録しましょう。</span><span class="sxs-lookup"><span data-stu-id="329f6-287">Review the community resources and register for the Community Call Q&A.</span></span>

<span data-ttu-id="329f6-288">コミュニティ コールの Q&A を最大限に活用するには、オンデマンド コミュニティ コンテンツを確認し、電話の少なくとも 48 時間前までに質問をお送りください。</span><span class="sxs-lookup"><span data-stu-id="329f6-288">To ensure that you get the most from the Community Call Q&A, review the on-demand community content and submit your questions up to 48 hours before the call.</span></span>

### <a name="questions"></a><span data-ttu-id="329f6-289">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="329f6-289">Questions?</span></span>

<span data-ttu-id="329f6-290">月次の CSP コミュニティ コール Q&A は、CSP プログラムの変更に関する質問がある場合に最適です。</span><span class="sxs-lookup"><span data-stu-id="329f6-290">The monthly CSP Community Call Q&A is the best place for questions related to changes in the CSP program.</span></span> <span data-ttu-id="329f6-291">毎月、お客様にとって最も重要なトピックにセッションを費やせるよう、資料を確認し、事前に質問をお送りください。</span><span class="sxs-lookup"><span data-stu-id="329f6-291">Each month, review the material and submit your questions in advance so that we can spend the session on the topics that are most important to you.</span></span>

<span data-ttu-id="329f6-292">詳細については、[サポート](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="329f6-292">For more information, contact [Support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span></span>

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a><span data-ttu-id="329f6-293">最後のリマインダー: 2021 年 5 月 6 日に GET 認定が非推奨化</span><span class="sxs-lookup"><span data-stu-id="329f6-293">Final reminder: Deprecation of GET qualification on May 6, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="329f6-294">Categories</span><span class="sxs-lookup"><span data-stu-id="329f6-294">Categories</span></span>

- <span data-ttu-id="329f6-295">日付: 2021 年 5 月 4 日</span><span class="sxs-lookup"><span data-stu-id="329f6-295">Date: 2021-05-04</span></span>

- <span data-ttu-id="329f6-296">機能</span><span class="sxs-lookup"><span data-stu-id="329f6-296">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="329f6-297">対象</span><span class="sxs-lookup"><span data-stu-id="329f6-297">Impacted audience</span></span>

<span data-ttu-id="329f6-298">パートナー センター API を使用してクラウド ソリューション プロバイダー プログラムを通じて教育、非営利、Government Community Cloud (GCC) 向けのプランを販売しているパートナー様</span><span class="sxs-lookup"><span data-stu-id="329f6-298">Partners selling Academic, Nonprofit, and Government Community Cloud (GCC) offers through the Cloud Solution Provider program using the Partner Center API</span></span>

### <a name="details"></a><span data-ttu-id="329f6-299">詳細</span><span class="sxs-lookup"><span data-stu-id="329f6-299">Details</span></span>

<span data-ttu-id="329f6-300">この発表は、[12 月にリリースされたパートナー センター の機能強化](https://docs.microsoft.com/partner-center/announcements/2020-december#1)に関する補足です。</span><span class="sxs-lookup"><span data-stu-id="329f6-300">This announcement is a follow-up to the Partner Center [enhancements released in December](https://docs.microsoft.com/partner-center/announcements/2020-december#1).</span></span> <span data-ttu-id="329f6-301">そのリリースの一部として、新しい GET および POST 認定 API が展開されました。その結果、**既存の GET 認定は 2021 年 5 月 6 日に廃止される予定です**。</span><span class="sxs-lookup"><span data-stu-id="329f6-301">As part of that release, new GET and POST Qualifications APIs were deployed and, as a result, **the existing GET qualification will be retired on May 6, 2021**.</span></span> <span data-ttu-id="329f6-302">その時点までに、新しい POST パートナー センター API を使用するように移行しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="329f6-302">By that time, you will need to have transitioned to using the new POST Partner Center APIs.</span></span> <span data-ttu-id="329f6-303">新しい POST API を使用すると、教育機関向けプランを購入できます。一方、新しい GET API を使用すると、事前に資格要件が確認された非営利および GCC 向けプランを購入できます。</span><span class="sxs-lookup"><span data-stu-id="329f6-303">The new POST APIs will enable you to purchase Education offers, while the new GET APIs will enable you to purchase pre-qualified Nonprofit and GCC offers.</span></span>

### <a name="next-steps"></a><span data-ttu-id="329f6-304">次のステップ</span><span class="sxs-lookup"><span data-stu-id="329f6-304">Next steps</span></span>

- <span data-ttu-id="329f6-305">適切かつタイムリーに移行できるよう、**新しい API に更新** してください。</span><span class="sxs-lookup"><span data-stu-id="329f6-305">**Update to the new APIs** for a successful and timely transition.</span></span>

- <span data-ttu-id="329f6-306">オペレーション レディネス リソースで、**新しいパートナー センター API に関する変更点とガイド** を確認してください: [パートナー センターの教育機関顧客検証プロセスの機能強化](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)。</span><span class="sxs-lookup"><span data-stu-id="329f6-306">**Review the new Partner Center API changes and Guide** in the Operations Readiness resources: [Partner Center Education customer validation process enhancements](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span></span>

- <span data-ttu-id="329f6-307">この情報を組織内の該当するチームと、およびリセラーと共有し、彼らがこれらの変更内容に対して準備できるようにしてください。</span><span class="sxs-lookup"><span data-stu-id="329f6-307">Share this information with the appropriate teams within your organization and with your resellers to help them prepare for these changes.</span></span>

### <a name="questions"></a><span data-ttu-id="329f6-308">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="329f6-308">Questions?</span></span>

<span data-ttu-id="329f6-309">このお知らせに関してご質問がある場合は、[パートナー センター サポート](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="329f6-309">For any questions related to this notification, contact [Partner Center support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span></span>

### <a name="change-log"></a><span data-ttu-id="329f6-310">ログの変更</span><span class="sxs-lookup"><span data-stu-id="329f6-310">Change log</span></span>

- <span data-ttu-id="329f6-311">2021 年 5 月 4 日: GET 認定の予定されている非推奨に関する最後のご案内</span><span class="sxs-lookup"><span data-stu-id="329f6-311">May 4, 2021: Final reminder of upcoming deprecation of GET qualification</span></span>

- <span data-ttu-id="329f6-312">2021 年 4 月 9 日: GET 認定の予定されている非推奨に関するご案内</span><span class="sxs-lookup"><span data-stu-id="329f6-312">April 9, 2021: Reminder of upcoming deprecation of GET qualification</span></span> 

- <span data-ttu-id="329f6-313">2 月: GET と PUT の認定の非推奨に関するタイムラインを更新しました</span><span class="sxs-lookup"><span data-stu-id="329f6-313">February: Updated timelines for deprecation of GET & PUT qualifications</span></span>

- <span data-ttu-id="329f6-314">1 月: GET と PUT の認定の予定されている非推奨に関するご案内</span><span class="sxs-lookup"><span data-stu-id="329f6-314">January: Reminder of upcoming deprecations of GET & PUT qualifications</span></span>

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a><span data-ttu-id="329f6-315">CSP での新しいコマース PDF 請求書の新しい形式</span><span class="sxs-lookup"><span data-stu-id="329f6-315">New format for the new commerce PDF invoice in CSP</span></span>

### <a name="categories"></a><span data-ttu-id="329f6-316">Categories</span><span class="sxs-lookup"><span data-stu-id="329f6-316">Categories</span></span>

- <span data-ttu-id="329f6-317">日付: 2021 年 4 月 5 日</span><span class="sxs-lookup"><span data-stu-id="329f6-317">Date: 2021-04-05</span></span>
- <span data-ttu-id="329f6-318">機能</span><span class="sxs-lookup"><span data-stu-id="329f6-318">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="329f6-319">まとめ</span><span class="sxs-lookup"><span data-stu-id="329f6-319">Summary</span></span>

<span data-ttu-id="329f6-320">Microsoft では、クラウド ソリューション プロバイダー (CSP) プログラムに新しいコマース PDF 請求書の新しい形式を導入中であり、SKU の説明ではなく製品の詳細ごとに請求の詳細を表示するようになります。</span><span class="sxs-lookup"><span data-stu-id="329f6-320">Microsoft is introducing a new format for the new commerce PDF invoice in the Cloud Solution Provider (CSP) program to display billing details by product detail instead of SKU description.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="329f6-321">対象</span><span class="sxs-lookup"><span data-stu-id="329f6-321">Impacted audience</span></span>

<span data-ttu-id="329f6-322">CSP プログラム経由で取引のあるパートナー様</span><span class="sxs-lookup"><span data-stu-id="329f6-322">Partners transacting through the CSP program</span></span>

### <a name="details"></a><span data-ttu-id="329f6-323">詳細</span><span class="sxs-lookup"><span data-stu-id="329f6-323">Details</span></span>

<span data-ttu-id="329f6-324">2021 年 5 月以降、Microsoft では、CSP プログラムに新しいコマース PDF 請求書の新しい形式を導入し、SKU の説明ではなく製品の詳細ごとに請求の詳細を表示するようになります。</span><span class="sxs-lookup"><span data-stu-id="329f6-324">Starting May 2021, Microsoft is introducing a new format for the new commerce PDF invoice in the CSP program to display billing details by product detail instead of SKU description.</span></span> <span data-ttu-id="329f6-325">この新しい更新により、製品の種類ごとに品目が集計され、すべての製品が個別の行に表示されます。</span><span class="sxs-lookup"><span data-stu-id="329f6-325">With this new update, we will be aggregating the line items by product type while displaying every product on an individual line.</span></span>

<span data-ttu-id="329f6-326">パートナー様は、2021 年 4 月 1 日から 2021 年 4 月 30 日までの請求期間に対する 5 月の請求書でこの変更を目にすることになります。</span><span class="sxs-lookup"><span data-stu-id="329f6-326">Partners will notice this change coming into effect in their May invoice for the billing period between April 1, 2021 and April 30, 2021.</span></span> <span data-ttu-id="329f6-327">影響を受けるオファーは、Microsoft Azure 予約インスタンス、Azure サブスクリプション (Azure プラン)、Marketplace です。</span><span class="sxs-lookup"><span data-stu-id="329f6-327">The affected offers are Microsoft Azure Reserved Instance, Azure subscriptions (Azure plan), and Marketplace.</span></span>

<span data-ttu-id="329f6-328">請求書の形式が更新された後に行われるクレジット再請求の要求は、新しい形式で生成されます。</span><span class="sxs-lookup"><span data-stu-id="329f6-328">Any credit-rebill requests made after the invoice format has been updated will be generated in the new format.</span></span>

#### <a name="partner-benefits"></a><span data-ttu-id="329f6-329">パートナーの特典</span><span class="sxs-lookup"><span data-stu-id="329f6-329">Partner benefits</span></span>

<span data-ttu-id="329f6-330">この更新では、パートナー様への請求エクスペリエンスに関して次の点が改善されます。</span><span class="sxs-lookup"><span data-stu-id="329f6-330">This update will offer the following improvements to the invoicing experience for partners:</span></span>

- <span data-ttu-id="329f6-331">重要なデータを保持したまま、請求書のサイズが削減されます</span><span class="sxs-lookup"><span data-stu-id="329f6-331">Reduced invoice size while retaining critical data</span></span>

- <span data-ttu-id="329f6-332">簡潔でユーザー フレンドリな請求書の業界標準の形式に従います</span><span class="sxs-lookup"><span data-stu-id="329f6-332">Alignment of the format to the industry standards for compact and user-friendly invoices</span></span> 

<span data-ttu-id="329f6-333">次の要素は影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="329f6-333">The following elements will not be affected:</span></span>

- <span data-ttu-id="329f6-334">請求書 PDF の請求の概要ページ</span><span class="sxs-lookup"><span data-stu-id="329f6-334">Billing summary page on the invoice PDF</span></span>

- <span data-ttu-id="329f6-335">既存の請求 API</span><span class="sxs-lookup"><span data-stu-id="329f6-335">Existing invoicing APIs</span></span>

- <span data-ttu-id="329f6-336">調整ファイル (調整ファイルは詳細データを取得するために使用できます)</span><span class="sxs-lookup"><span data-stu-id="329f6-336">Reconciliation files (Recon files can be used for retrieving granular data.)</span></span> 

- <span data-ttu-id="329f6-337">使用量とライセンス ベースの料金の請求書</span><span class="sxs-lookup"><span data-stu-id="329f6-337">Usage and license-based charges invoices</span></span>

### <a name="next-steps"></a><span data-ttu-id="329f6-338">次のステップ</span><span class="sxs-lookup"><span data-stu-id="329f6-338">Next steps</span></span>

<span data-ttu-id="329f6-339">このトピックの情報について、Microsoft パートナー Web サイトの [Operations Readiness リソース ギャラリー](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="329f6-339">Review the information about this topic in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) on the Microsoft partner website.</span></span> <span data-ttu-id="329f6-340">請求リソース、請求書、CSP 請求、税金など、請求と税金のトピックに関する詳細は、パートナー センターの[請求セクション](https://docs.microsoft.com/partner-center/billing)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="329f6-340">For more information about billing and tax topics including billing resources, invoices, CSP billing, and taxes, visit the [Billing section](https://docs.microsoft.com/partner-center/billing) in Partner Center.</span></span>

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a><span data-ttu-id="329f6-341">クラウド ソリューション プロバイダー (CSP) のお客様のオンボード要件の変更</span><span class="sxs-lookup"><span data-stu-id="329f6-341">Changes to the Cloud Solution Provider (CSP) customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="329f6-342">Categories</span><span class="sxs-lookup"><span data-stu-id="329f6-342">Categories</span></span>

- <span data-ttu-id="329f6-343">日付: 2021 年 4 月 2 日</span><span class="sxs-lookup"><span data-stu-id="329f6-343">Date: 2021-04-02</span></span>
- <span data-ttu-id="329f6-344">製品サービス/市場</span><span class="sxs-lookup"><span data-stu-id="329f6-344">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="329f6-345">まとめ</span><span class="sxs-lookup"><span data-stu-id="329f6-345">Summary</span></span>

<span data-ttu-id="329f6-346">パートナーと顧客が信頼に基づいて取引できるように支援する責任の一環として、Microsoft では 2021 年 3 月 25 日から、追加の顧客情報を要求いたします。</span><span class="sxs-lookup"><span data-stu-id="329f6-346">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="329f6-347">対象</span><span class="sxs-lookup"><span data-stu-id="329f6-347">Impacted audience</span></span>

<span data-ttu-id="329f6-348">次のセクションに記載されている国に新規または既存の顧客がいる CSP 直接請求パートナーおよび間接プロバイダー</span><span class="sxs-lookup"><span data-stu-id="329f6-348">CSP direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="329f6-349">詳細</span><span class="sxs-lookup"><span data-stu-id="329f6-349">Details</span></span>

<span data-ttu-id="329f6-350">Microsoft の基盤は信頼です。</span><span class="sxs-lookup"><span data-stu-id="329f6-350">Microsoft runs on trust.</span></span> <span data-ttu-id="329f6-351">Microsoft は、CSP プログラムでの顧客サブスクリプションの取引について、顧客検証のための法令に準拠した安全な手段の提供に努めています。</span><span class="sxs-lookup"><span data-stu-id="329f6-351">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="329f6-352">2021 年 3 月 25 日に、パートナー センター API とユーザー インターフェイス (UI) の拡張機能を導入する予定です。これは、以下の条件の両方を満たすパートナーに影響します。</span><span class="sxs-lookup"><span data-stu-id="329f6-352">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

- <span data-ttu-id="329f6-353">Microsoft の間に直接請求関係があるパートナー (つまり、直接請求パートナーまたは間接プロバイダーのいずれかであるパートナー)</span><span class="sxs-lookup"><span data-stu-id="329f6-353">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

- <span data-ttu-id="329f6-354">パートナーは、次の国の新規または既存の顧客と取引があります:</span><span class="sxs-lookup"><span data-stu-id="329f6-354">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="329f6-355">タイ</span><span class="sxs-lookup"><span data-stu-id="329f6-355">Thailand</span></span>
    - <span data-ttu-id="329f6-356">ベトナム</span><span class="sxs-lookup"><span data-stu-id="329f6-356">Vietnam</span></span>
    - <span data-ttu-id="329f6-357">トルコ</span><span class="sxs-lookup"><span data-stu-id="329f6-357">Turkey</span></span>
    - <span data-ttu-id="329f6-358">ポーランド</span><span class="sxs-lookup"><span data-stu-id="329f6-358">Poland</span></span>
    - <span data-ttu-id="329f6-359">南アフリカ</span><span class="sxs-lookup"><span data-stu-id="329f6-359">South Africa</span></span>
    - <span data-ttu-id="329f6-360">インド</span><span class="sxs-lookup"><span data-stu-id="329f6-360">India</span></span>
    - <span data-ttu-id="329f6-361">ブラジル</span><span class="sxs-lookup"><span data-stu-id="329f6-361">Brazil</span></span>
    - <span data-ttu-id="329f6-362">イラク</span><span class="sxs-lookup"><span data-stu-id="329f6-362">Iraq</span></span>
    - <span data-ttu-id="329f6-363">ミャンマー</span><span class="sxs-lookup"><span data-stu-id="329f6-363">Myanmar</span></span>
    - <span data-ttu-id="329f6-364">南スーダン</span><span class="sxs-lookup"><span data-stu-id="329f6-364">South Sudan</span></span>
    - <span data-ttu-id="329f6-365">サウジアラビア</span><span class="sxs-lookup"><span data-stu-id="329f6-365">Saudi Arabia</span></span>
    - <span data-ttu-id="329f6-366">アラブ首長国連邦</span><span class="sxs-lookup"><span data-stu-id="329f6-366">United Arab Emirates</span></span>
    - <span data-ttu-id="329f6-367">ベネズエラ</span><span class="sxs-lookup"><span data-stu-id="329f6-367">Venezuela</span></span>

<span data-ttu-id="329f6-368">条件を満たすパートナーは、次にその顧客のサブスクリプションを更新または作成するときに、顧客の会社登録 ID (顧客の組織 INN とも呼ばれます) と電話番号を提出する必要があります。</span><span class="sxs-lookup"><span data-stu-id="329f6-368">Partners who meet the criteria will have to submit a customer's company registration ID (also known as the customer's organization INN) and phone number when they next update or create a subscription for that customer.</span></span> <span data-ttu-id="329f6-369">また、これらのパートナーは、必要に応じて、顧客のミドル ネームを入力することができます。</span><span class="sxs-lookup"><span data-stu-id="329f6-369">These partners can also enter an optional middle name for the customer.</span></span>

<span data-ttu-id="329f6-370">会社登録 ID を追加する場合は、顧客の個人 ID ではなく、業務用の税 ID を使用する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="329f6-370">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="329f6-371">以下の国で新規または既存の顧客との取引を行っているパートナーは、先行する 2020 年 11 月のリリースで既にオンボードされています。</span><span class="sxs-lookup"><span data-stu-id="329f6-371">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="329f6-372">アルメニア</span><span class="sxs-lookup"><span data-stu-id="329f6-372">Armenia</span></span>
- <span data-ttu-id="329f6-373">アゼルバイジャン</span><span class="sxs-lookup"><span data-stu-id="329f6-373">Azerbaijan</span></span>
- <span data-ttu-id="329f6-374">ベラルーシ</span><span class="sxs-lookup"><span data-stu-id="329f6-374">Belarus</span></span>
- <span data-ttu-id="329f6-375">ハンガリー</span><span class="sxs-lookup"><span data-stu-id="329f6-375">Hungary</span></span>
- <span data-ttu-id="329f6-376">カザフスタン</span><span class="sxs-lookup"><span data-stu-id="329f6-376">Kazakhstan</span></span>
- <span data-ttu-id="329f6-377">キルギスタン</span><span class="sxs-lookup"><span data-stu-id="329f6-377">Kyrgyzstan</span></span>
- <span data-ttu-id="329f6-378">モルドバ</span><span class="sxs-lookup"><span data-stu-id="329f6-378">Moldova</span></span>
- <span data-ttu-id="329f6-379">ロシア</span><span class="sxs-lookup"><span data-stu-id="329f6-379">Russia</span></span>
- <span data-ttu-id="329f6-380">タジキスタン</span><span class="sxs-lookup"><span data-stu-id="329f6-380">Tajikistan</span></span>
- <span data-ttu-id="329f6-381">ウクライナ</span><span class="sxs-lookup"><span data-stu-id="329f6-381">Ukraine</span></span>
- <span data-ttu-id="329f6-382">ウズベキスタン</span><span class="sxs-lookup"><span data-stu-id="329f6-382">Uzbekistan</span></span>

<span data-ttu-id="329f6-383">その他の地域の顧客と提携しているパートナーは、2021 年 3 月の終わりに、顧客の会社登録 ID、電話番号、ミドル ネームを詳細情報として必要に応じて入力できるようになります。</span><span class="sxs-lookup"><span data-stu-id="329f6-383">Partners with customers in the rest of the world will have the ability at the end of March 2021 to enter the company registration ID, phone number, and middle name for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="329f6-384">次のステップ</span><span class="sxs-lookup"><span data-stu-id="329f6-384">Next steps</span></span>

- <span data-ttu-id="329f6-385">詳細なガイダンスについては、専用の[パートナー コレクション](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)でテクニカル ドキュメントとよく寄せられる質問を参照してください。</span><span class="sxs-lookup"><span data-stu-id="329f6-385">Review the technical documentation and frequently asked questions in the dedicated [partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="329f6-386">パートナー センター API と Web ユーザー エクスペリエンスを使用して、変更を組み込む準備をしてください。</span><span class="sxs-lookup"><span data-stu-id="329f6-386">Prepare to incorporate the changes using Partner Center API and web user experience.</span></span> <span data-ttu-id="329f6-387">API または SDK はテストに使用できます。</span><span class="sxs-lookup"><span data-stu-id="329f6-387">API/SDKs will be available for testing.</span></span>
- <span data-ttu-id="329f6-388">新しい顧客をオンボードする場合や、既存の顧客の詳細情報を変更する場合は、必ず追加データを提出してください。</span><span class="sxs-lookup"><span data-stu-id="329f6-388">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>
- <span data-ttu-id="329f6-389">コントロール パネル ベンダー (CPV) ソリューションを使用している場合は、CPV とご相談ください。</span><span class="sxs-lookup"><span data-stu-id="329f6-389">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="329f6-390">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="329f6-390">Questions?</span></span>

<span data-ttu-id="329f6-391">会社登録 ID (INN または TIN とも呼ばれます) に関するご質問がある場合は、税務顧問または現地の税務署にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="329f6-391">Contact your tax advisor or local tax office if you have any questions related to the company registration ID (also called INN or TIN).</span></span> <span data-ttu-id="329f6-392">Microsoft では、税務に関するガイダンスを提供できません。</span><span class="sxs-lookup"><span data-stu-id="329f6-392">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="329f6-393">Microsoft との連携でサポートが必要な場合は、[サービス要求](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)を開いてください。</span><span class="sxs-lookup"><span data-stu-id="329f6-393">If you need support with your operations with Microsoft, open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a><span data-ttu-id="329f6-394">今月の製品の発表とオファーを見る</span><span class="sxs-lookup"><span data-stu-id="329f6-394">View this month’s product launches and offers</span></span>

### <a name="categories"></a><span data-ttu-id="329f6-395">Categories</span><span class="sxs-lookup"><span data-stu-id="329f6-395">Categories</span></span>

- <span data-ttu-id="329f6-396">日付: 2021 年 4 月 1 日</span><span class="sxs-lookup"><span data-stu-id="329f6-396">Date: 2021-04-01</span></span>
- <span data-ttu-id="329f6-397">機能</span><span class="sxs-lookup"><span data-stu-id="329f6-397">Capabilities</span></span>
 
### <a name="summary"></a><span data-ttu-id="329f6-398">まとめ</span><span class="sxs-lookup"><span data-stu-id="329f6-398">Summary</span></span>

<span data-ttu-id="329f6-399">2021 年 4 月の製品発表予定表が公開されました。</span><span class="sxs-lookup"><span data-stu-id="329f6-399">The April 2021 product launch calendar is now published.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="329f6-400">対象</span><span class="sxs-lookup"><span data-stu-id="329f6-400">Impacted audience</span></span>

<span data-ttu-id="329f6-401">クラウド ソリューション プロバイダー (CSP) プログラムを通じて取引を行う、すべてのパートナー様</span><span class="sxs-lookup"><span data-stu-id="329f6-401">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="329f6-402">詳細</span><span class="sxs-lookup"><span data-stu-id="329f6-402">Details</span></span>

<span data-ttu-id="329f6-403">2021 年 4 月の[製品発表予定表](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) が、Operations Readiness リソース ギャラリーで入手できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="329f6-403">The April 2021 [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) is now available in the Operations readiness resource gallery.</span></span> <span data-ttu-id="329f6-404">こちらで今後予定されている製品の発表とオファーをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="329f6-404">View the upcoming product launches and offers here.</span></span>

### <a name="next-steps"></a><span data-ttu-id="329f6-405">次のステップ</span><span class="sxs-lookup"><span data-stu-id="329f6-405">Next steps</span></span>

<span data-ttu-id="329f6-406">[製品発表予定表](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)を確認し、この情報を組織内の該当する関係者と共有します。</span><span class="sxs-lookup"><span data-stu-id="329f6-406">Review the [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), and share the information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="329f6-407">わからないことがある場合は、</span><span class="sxs-lookup"><span data-stu-id="329f6-407">Questions?</span></span>

<span data-ttu-id="329f6-408">これらのオファーについてさらにご質問がある場合は、関連する Yammer コミュニティをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="329f6-408">For any further questions about these offers, check your relevant Yammer communities.</span></span>
