---
title: 調整ファイルを使用する
ms.topic: article
ms.date: 03/10/2021
description: パートナーセンターでの調整ファイルと、特定の請求サイクルにおける料金の詳細な行項目ビューを解釈する方法について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6b9e466402d71c988729052bd72ba2346a9d977
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022776"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="f133d-103">パートナーセンターの調整ファイルの品目を読み取る方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="f133d-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="f133d-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="f133d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="f133d-105">課金管理者</span><span class="sxs-lookup"><span data-stu-id="f133d-105">Billing admin</span></span>
- <span data-ttu-id="f133d-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="f133d-106">Global admin</span></span>

<span data-ttu-id="f133d-107">パートナーセンターから調整ファイルをダウンロードして、請求サイクルの各料金の詳細な行項目ビューをダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="f133d-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="f133d-108">行項目の詳細には、各顧客のサブスクリプションの料金と詳細なイベント (サブスクリプションへのライセンスの長期追加など) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="f133d-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="f133d-109">**請求書** を読む方法の詳細については、「請求書の [読み取り](read-your-bill.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f133d-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="f133d-110">調整ファイルのフィールドについて</span><span class="sxs-lookup"><span data-stu-id="f133d-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="f133d-111">ライセンス ベースの調整ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="f133d-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="f133d-112">使用量ベースの調整ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="f133d-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="f133d-113">毎日評価される使用状況調整ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="f133d-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="f133d-114">1回限りの購入 CSP 調整ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="f133d-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="f133d-115">調整ファイルの料金の種類について</span><span class="sxs-lookup"><span data-stu-id="f133d-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="f133d-116">調整ファイル ( **ChargeType** 列) の料金の種類については、「 [調整ファイルの料金の種類](recon-file-charge-types.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f133d-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="f133d-117">書式設定の問題の修正</span><span class="sxs-lookup"><span data-stu-id="f133d-117">Fix formatting issues</span></span>

<span data-ttu-id="f133d-118">場合によっては、調整ファイルに書式設定の問題が含まれていることがあります。</span><span class="sxs-lookup"><span data-stu-id="f133d-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="f133d-119">たとえば、en-us ロケールが使用されていない場合に、この問題が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f133d-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="f133d-120">調整ファイルの書式設定に関する問題を修正するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="f133d-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="f133d-121">Microsoft Excel で調整ファイル (.csv 形式) を開きます。</span><span class="sxs-lookup"><span data-stu-id="f133d-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="f133d-122">ファイルの最初の列を選択します。</span><span class="sxs-lookup"><span data-stu-id="f133d-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="f133d-123">**テキストを列に変換ウィザード** を開きます。</span><span class="sxs-lookup"><span data-stu-id="f133d-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="f133d-124">リボンで、[ **データ**] を選択し、[ **列のテキスト**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="f133d-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="f133d-125">ウィザードで、[区切られた **ファイルの種類**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="f133d-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="f133d-126">次に、 **[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="f133d-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="f133d-127">[ **区切り記号** ] ボックスで、[ **コンマ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="f133d-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="f133d-128">( **タブ** が既に選択されている場合は、このオプションを選択したままにしておくことができます)。次に、[ **次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="f133d-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="f133d-129">[ **列のデータ形式** ] フィールドで、[ **Date: MDY**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="f133d-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="f133d-130">次に、 **[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="f133d-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="f133d-131">[ **列のデータ形式** ] フィールドで、[すべての金額列] の **テキスト** を選択します。</span><span class="sxs-lookup"><span data-stu-id="f133d-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="f133d-132">次に、 **[Finish]\(完了\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="f133d-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="f133d-133">プログラムによる調整ファイルのダウンロード</span><span class="sxs-lookup"><span data-stu-id="f133d-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="f133d-134">調整ファイルは非常に大きくなる可能性があり、ダウンロードが困難な場合があります。</span><span class="sxs-lookup"><span data-stu-id="f133d-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="f133d-135">プログラムによって調整ファイルをダウンロードするには、「 [請求書の品目を取得](/partner-center/develop/get-invoiceline-items)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f133d-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="f133d-136">税または VAT をマップする</span><span class="sxs-lookup"><span data-stu-id="f133d-136">Map taxes or VAT</span></span>

<span data-ttu-id="f133d-137">税金または付加価値税 (VAT) を請求書にマッピングするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="f133d-137">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="f133d-138">ライセンスベースのファイルから **税** 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="f133d-138">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="f133d-139">使用状況に基づくファイルから **taxationitem.taxamount** 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="f133d-139">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="f133d-140">パートナー別の調整ファイルの明細</span><span class="sxs-lookup"><span data-stu-id="f133d-140">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="f133d-141">**間接モデル** のパートナーは、これらの追加フィールドをライセンスベースと使用状況に基づく調整ファイルの両方で使用して、リセラーごとにファイルを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="f133d-141">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="f133d-142">MPN ID</span><span class="sxs-lookup"><span data-stu-id="f133d-142">MPN ID</span></span> | <span data-ttu-id="f133d-143">説明</span><span class="sxs-lookup"><span data-stu-id="f133d-143">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="f133d-144">MPN ID</span><span class="sxs-lookup"><span data-stu-id="f133d-144">MPN ID</span></span> | <span data-ttu-id="f133d-145">クラウドソリューションプロバイダー (CSP) パートナー (直接または間接) の Microsoft Partner Network (MPN) 識別子。</span><span class="sxs-lookup"><span data-stu-id="f133d-145">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="f133d-146">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="f133d-146">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="f133d-147">[サブスクリプションの販売店の MPN 識別子](#reseller-mpn-id)。</span><span class="sxs-lookup"><span data-stu-id="f133d-147">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="f133d-148">このフィールドは、パートナーセンターの特定のサブスクリプションについて一覧表示されているリセラー ID に対応しています。</span><span class="sxs-lookup"><span data-stu-id="f133d-148">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="f133d-149">インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="f133d-149">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="f133d-150">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="f133d-150">Reseller MPN ID</span></span>

<span data-ttu-id="f133d-151">CSP パートナーが顧客にサブスクリプションを直接販売した場合、 **MPN id** と **再販業者の MPN id** の両方として、 **MPN id** が2回表示されます。</span><span class="sxs-lookup"><span data-stu-id="f133d-151">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="f133d-152">CSP パートナーが **MPN id** のない再販業者を持っている場合、この値は代わりにパートナーの **MPN id** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="f133d-152">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="f133d-153">CSP パートナーが **リセラーの MPN ID** を削除した場合、この値は *-1* に設定されます。</span><span class="sxs-lookup"><span data-stu-id="f133d-153">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="f133d-154">**リセラー MPN ID** を表示または更新するには:</span><span class="sxs-lookup"><span data-stu-id="f133d-154">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="f133d-155">パートナー センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="f133d-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="f133d-156">パートナー センター メニューで、**[顧客]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="f133d-156">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="f133d-157">一覧から顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="f133d-157">Choose the customer from the list.</span></span>
4. <span data-ttu-id="f133d-158">カスタマーメニューで、[ **サブスクリプション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="f133d-158">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="f133d-159">一覧からサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="f133d-159">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="f133d-160">**[更新]** を選んで、**[再販業者 (MPN ID)]** を変更します。</span><span class="sxs-lookup"><span data-stu-id="f133d-160">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f133d-161">次のステップ</span><span class="sxs-lookup"><span data-stu-id="f133d-161">Next steps</span></span>

- [<span data-ttu-id="f133d-162">請求書 & 偵察ファイルを読み取る方法</span><span class="sxs-lookup"><span data-stu-id="f133d-162">How to read your bill & recon file</span></span>](read-your-bill.md) 