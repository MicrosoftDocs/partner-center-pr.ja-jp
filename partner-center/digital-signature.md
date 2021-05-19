---
title: デジタル署名機能
ms.topic: how-to
ms.date: 07/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: インドのパートナーセンターパートナーがデジタル署名された請求書を表示し、パートナーセンターで作成された注文の請求書のデジタルコピーを受信する方法について説明します。
author: keramp
ms.author: keramp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4253c59a85c8353856b16f60957761f4f2245da3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147192"
---
# <a name="view-digitally-signed-invoices"></a><span data-ttu-id="71f13-103">デジタル署名された請求書の表示</span><span class="sxs-lookup"><span data-stu-id="71f13-103">View digitally signed invoices</span></span>

<span data-ttu-id="71f13-104">**適用対象**: パートナーセンター |インドのパートナーセンター</span><span class="sxs-lookup"><span data-stu-id="71f13-104">**Applies to**: Partner Center | Partner Center India</span></span>

<span data-ttu-id="71f13-105">**適切なロール**: Account admin |課金エージェント |営業担当者</span><span class="sxs-lookup"><span data-stu-id="71f13-105">**Appropriate roles**: Account admin | Billing agent | Sales agent</span></span>

<span data-ttu-id="71f13-106">インドのパートナーは、Microsoft がデジタル署名した請求書を持っていることがわかりました。</span><span class="sxs-lookup"><span data-stu-id="71f13-106">Partners in India now see that Microsoft has digitally signed invoices.</span></span> <span data-ttu-id="71f13-107">署名を表示するには、Adobe Acrobat Reader ドキュメントクラウド (DC) を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="71f13-107">You must use Adobe Acrobat Reader Document Cloud (DC) to view a signature.</span></span>

## <a name="how-to-view-and-insure-a-valid-digital-signature"></a><span data-ttu-id="71f13-108">有効なデジタル署名を表示して保証する方法</span><span class="sxs-lookup"><span data-stu-id="71f13-108">How to view and insure a valid digital signature</span></span>


1. <span data-ttu-id="71f13-109">パートナーセンターで注文を作成した場合は、電子メールで請求書のデジタルコピーを受け取ることになります。</span><span class="sxs-lookup"><span data-stu-id="71f13-109">If you created the order in Partner Center, you will receive a digital copy of an invoice in email.</span></span> <span data-ttu-id="71f13-110">Adobe Acrobat Reader DC 内から開く請求書を選択します。</span><span class="sxs-lookup"><span data-stu-id="71f13-110">Select the invoice, which will open from within Adobe Acrobat Reader DC.</span></span>


2. <span data-ttu-id="71f13-111">請求書の上部には、署名されていて、 **すべての署名が有効** であることが必要です。</span><span class="sxs-lookup"><span data-stu-id="71f13-111">At the top of the invoice, you should see **Signed and all signatures are valid**.</span></span>
 
 :::image type="content" source="images/digitalsig/digital1.png" alt-text="有効な署名通知バナー付きのサンプル請求書。緑色のチェックマークと語句、署名済み、すべての署名が有効です。":::

3. <span data-ttu-id="71f13-113">署名を選択します。</span><span class="sxs-lookup"><span data-stu-id="71f13-113">Select the signature.</span></span> <span data-ttu-id="71f13-114">有効性を示す証明書が表示されます。</span><span class="sxs-lookup"><span data-stu-id="71f13-114">The certificate stating validity will appear.</span></span>

:::image type="content" source="images/digitalsig/digital2.png" alt-text="[承認された署名者] フィールドと [署名検証の状態] ダイアログボックスの [詳細]、[署名のプロパティ] オプション、[キャンセル] オプションを使用した署名付き請求書。"::: 

4. <span data-ttu-id="71f13-116">署名の **プロパティ** を選択すると、署名の有効性に関する詳細が表示されます。</span><span class="sxs-lookup"><span data-stu-id="71f13-116">Select **Signature Properties** to view more details on signature validity.</span></span>

:::image type="content" source="images/digitalsig/digital4.png" alt-text="署名プロパティの詳細ビューには、だれが、ドキュメントが署名された日時、検証プロセス、署名者の証明書に関する情報が表示されます。"::: 

4. <span data-ttu-id="71f13-118">また、証明書のパスが正しいことと、証明書が信頼されていることを確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="71f13-118">You can also ensure that the certification paths are correct and that the certificate is trusted.</span></span>

 :::image type="content" source="images/digitalsig/digital3.png" alt-text="[証明書ビューアー] ダイアログボックスには、証明書とその発行チェーン全体に関する詳細情報を含むタブがいくつか表示されます。":::

### <a name="additional-information-on-invoices-and-digital-signatures"></a><span data-ttu-id="71f13-120">請求書とデジタル署名に関する追加情報</span><span class="sxs-lookup"><span data-stu-id="71f13-120">Additional information on invoices and digital signatures</span></span>

<span data-ttu-id="71f13-121">デジタル コピーは、注文を作成したユーザーにパートナー センター。</span><span class="sxs-lookup"><span data-stu-id="71f13-121">A digital copy will be mailed to the person who created the order in Partner Center.</span></span> <span data-ttu-id="71f13-122">2020 年 7 月 17 日より前に発行された請求書に対してデジタル署名された請求書を取得できない。</span><span class="sxs-lookup"><span data-stu-id="71f13-122">You can't get digitally signed invoices for any invoices that were issued before July 17, 2020.</span></span> <span data-ttu-id="71f13-123">また、手動で署名された請求書は使用できません。</span><span class="sxs-lookup"><span data-stu-id="71f13-123">Also, manually signed invoices will not be available.</span></span>

## <a name="next-steps"></a><span data-ttu-id="71f13-124">次のステップ</span><span class="sxs-lookup"><span data-stu-id="71f13-124">Next steps</span></span>

- [<span data-ttu-id="71f13-125">一般的な課金シナリオ</span><span class="sxs-lookup"><span data-stu-id="71f13-125">Common billing scenarios</span></span>](common-billing-scenarios.md)