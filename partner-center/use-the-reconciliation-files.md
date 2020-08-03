---
title: 調整ファイルを使用する
ms.topic: article
ms.date: 06/08/2020
description: パートナーセンターでの調整ファイルと、特定の請求サイクルにおける料金の詳細な行項目ビューを解釈する方法について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 05939dc5edaddeb2f74b3b75017e2062dff25e31
ms.sourcegitcommit: e243bc0ef337f5d92c5b208ce6bb9dc5f179b185
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2020
ms.locfileid: "87468333"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="fe755-103">パートナーセンターの調整ファイルの品目を読み取る方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="fe755-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="fe755-104">適用対象:</span><span class="sxs-lookup"><span data-stu-id="fe755-104">Applies to:</span></span>

- <span data-ttu-id="fe755-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="fe755-105">Partner Center</span></span>
- <span data-ttu-id="fe755-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="fe755-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="fe755-107">パートナーセンターから調整ファイルをダウンロードして、請求サイクルの各料金の詳細な行項目ビューをダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="fe755-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="fe755-108">行項目の詳細には、各顧客のサブスクリプションの料金と詳細なイベント (サブスクリプションへのライセンスの長期追加など) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="fe755-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="fe755-109">適切なロール:</span><span class="sxs-lookup"><span data-stu-id="fe755-109">Appropriate roles:</span></span>

- <span data-ttu-id="fe755-110">課金管理者</span><span class="sxs-lookup"><span data-stu-id="fe755-110">Billing admin</span></span>
- <span data-ttu-id="fe755-111">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="fe755-111">Global admin</span></span>

<span data-ttu-id="fe755-112">**請求書**を読む方法の詳細については、「請求書の[読み取り](read-your-bill.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe755-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="fe755-113">調整ファイルのフィールドについて</span><span class="sxs-lookup"><span data-stu-id="fe755-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="fe755-114">ライセンスベースの調整ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="fe755-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="fe755-115">使用法に基づく調整ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="fe755-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="fe755-116">日単位で評価した使用状況の調整ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="fe755-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="fe755-117">調整ファイルの料金の種類について</span><span class="sxs-lookup"><span data-stu-id="fe755-117">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="fe755-118">調整ファイル ( **ChargeType**列) の料金の種類については、「[調整ファイルの料金の種類](recon-file-charge-types.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe755-118">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="fe755-119">書式設定の問題の修正</span><span class="sxs-lookup"><span data-stu-id="fe755-119">Fix formatting issues</span></span>

<span data-ttu-id="fe755-120">場合によっては、調整ファイルに書式設定の問題が含まれていることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe755-120">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="fe755-121">たとえば、en-us ロケールが使用されていない場合に、この問題が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="fe755-121">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="fe755-122">調整ファイルの書式設定に関する問題を修正するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="fe755-122">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="fe755-123">Microsoft Excel で調整ファイル (.csv 形式) を開きます。</span><span class="sxs-lookup"><span data-stu-id="fe755-123">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="fe755-124">ファイルの最初の列を選択します。</span><span class="sxs-lookup"><span data-stu-id="fe755-124">Select the first column in the file.</span></span>
3. <span data-ttu-id="fe755-125">**テキストを列に変換ウィザード**を開きます。</span><span class="sxs-lookup"><span data-stu-id="fe755-125">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="fe755-126">リボンで、[**データ**] を選択し、[**列のテキスト**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="fe755-126">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="fe755-127">ウィザードで、[区切られた**ファイルの種類**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="fe755-127">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="fe755-128">次に、 **[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fe755-128">Then, select **Next**.</span></span>
5. <span data-ttu-id="fe755-129">[**区切り記号**] ボックスで、[**コンマ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="fe755-129">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="fe755-130">(**タブ**が既に選択されている場合は、このオプションを選択したままにしておくことができます)。次に、[**次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="fe755-130">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="fe755-131">[**列のデータ形式**] フィールドで、[ **Date: MDY**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="fe755-131">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="fe755-132">次に、 **[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fe755-132">Then, select **Next**.</span></span>
7. <span data-ttu-id="fe755-133">[**列のデータ形式**] フィールドで、[すべての金額列] の**テキスト**を選択します。</span><span class="sxs-lookup"><span data-stu-id="fe755-133">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="fe755-134">次に、 **[完了]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fe755-134">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="fe755-135">プログラムによる調整ファイルのダウンロード</span><span class="sxs-lookup"><span data-stu-id="fe755-135">Download reconciliation files programmatically</span></span>

<span data-ttu-id="fe755-136">調整ファイルは非常に大きくなる可能性があり、ダウンロードが困難な場合があります。</span><span class="sxs-lookup"><span data-stu-id="fe755-136">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="fe755-137">プログラムによって調整ファイルをダウンロードするには、「[請求書の品目を取得](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe755-137">To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="fe755-138">税または VAT をマップする</span><span class="sxs-lookup"><span data-stu-id="fe755-138">Map taxes or VAT</span></span>

<span data-ttu-id="fe755-139">税金または付加価値税 (VAT) を請求書にマッピングするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="fe755-139">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="fe755-140">ライセンスベースのファイルから**税**列を合計します。</span><span class="sxs-lookup"><span data-stu-id="fe755-140">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="fe755-141">使用状況に基づくファイルから**taxationitem.taxamount**列を合計します。</span><span class="sxs-lookup"><span data-stu-id="fe755-141">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="fe755-142">パートナー別の調整ファイルの明細</span><span class="sxs-lookup"><span data-stu-id="fe755-142">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="fe755-143">**間接モデル**のパートナーは、これらの追加フィールドをライセンスベースと使用状況に基づく調整ファイルの両方で使用して、リセラーごとにファイルを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="fe755-143">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="fe755-144">MPN ID</span><span class="sxs-lookup"><span data-stu-id="fe755-144">MPN ID</span></span> | <span data-ttu-id="fe755-145">Description</span><span class="sxs-lookup"><span data-stu-id="fe755-145">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="fe755-146">MPN ID</span><span class="sxs-lookup"><span data-stu-id="fe755-146">MPN ID</span></span> | <span data-ttu-id="fe755-147">クラウドソリューションプロバイダー (CSP) パートナー (直接または間接) の Microsoft Partner Network (MPN) 識別子。</span><span class="sxs-lookup"><span data-stu-id="fe755-147">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="fe755-148">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="fe755-148">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="fe755-149">[サブスクリプションの販売店の MPN 識別子](#reseller-mpn-id)。</span><span class="sxs-lookup"><span data-stu-id="fe755-149">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="fe755-150">このフィールドは、パートナーセンターの特定のサブスクリプションについて一覧表示されているリセラー ID に対応しています。</span><span class="sxs-lookup"><span data-stu-id="fe755-150">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="fe755-151">インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="fe755-151">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="fe755-152">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="fe755-152">Reseller MPN ID</span></span>

<span data-ttu-id="fe755-153">CSP パートナーが顧客にサブスクリプションを直接販売した場合、 **MPN id**と**再販業者の MPN id**の両方として、 **MPN id**が2回表示されます。</span><span class="sxs-lookup"><span data-stu-id="fe755-153">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="fe755-154">CSP パートナーが**MPN id**のない再販業者を持っている場合、この値は代わりにパートナーの**MPN id**に設定されます。</span><span class="sxs-lookup"><span data-stu-id="fe755-154">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="fe755-155">CSP パートナーが**リセラーの MPN ID**を削除した場合、この値は *-1*に設定されます。</span><span class="sxs-lookup"><span data-stu-id="fe755-155">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="fe755-156">**リセラー MPN ID**を表示または更新するには:</span><span class="sxs-lookup"><span data-stu-id="fe755-156">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="fe755-157">パートナー センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="fe755-157">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="fe755-158">パートナー センター メニューで、**[顧客]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="fe755-158">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="fe755-159">一覧から顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="fe755-159">Choose the customer from the list.</span></span>
4. <span data-ttu-id="fe755-160">カスタマーメニューで、[**サブスクリプション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="fe755-160">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="fe755-161">一覧からサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="fe755-161">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="fe755-162">**[更新]** を選んで、**[再販業者 (MPN ID)]** を変更します。</span><span class="sxs-lookup"><span data-stu-id="fe755-162">Select **update** to change the **Reseller (MPN ID)**.</span></span>
