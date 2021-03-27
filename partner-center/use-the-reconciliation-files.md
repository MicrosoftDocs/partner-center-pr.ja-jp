---
title: 調整ファイルを使用する
ms.topic: article
ms.date: 03/26/2021
description: パートナーセンターでの調整ファイルと、特定の請求サイクルにおける料金の詳細な行項目ビューを解釈する方法について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a6a1455304f12e364d71e666cbd548821f8be55
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633898"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="ba116-103">パートナーセンターの調整ファイルの品目を読み取る方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="ba116-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="ba116-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="ba116-104">**Appropriate roles**</span></span>

- <span data-ttu-id="ba116-105">課金管理者</span><span class="sxs-lookup"><span data-stu-id="ba116-105">Billing admin</span></span>
- <span data-ttu-id="ba116-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="ba116-106">Global admin</span></span>

<span data-ttu-id="ba116-107">パートナーセンターから調整ファイルをダウンロードして、請求サイクルの各料金の詳細な行項目ビューをダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="ba116-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="ba116-108">行項目の詳細には、各顧客のサブスクリプションの料金と詳細なイベント (サブスクリプションへのライセンスの長期追加など) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="ba116-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="ba116-109">**請求書** を読む方法の詳細については、「請求書の [読み取り](read-your-bill.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba116-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="ba116-110">調整ファイルのフィールドについて</span><span class="sxs-lookup"><span data-stu-id="ba116-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="ba116-111">ライセンス ベースの調整ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="ba116-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="ba116-112">使用量ベースの調整ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="ba116-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="ba116-113">毎日評価される使用状況調整ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="ba116-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="ba116-114">1回限りの購入 CSP 調整ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="ba116-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="ba116-115">調整ファイルの料金の種類について</span><span class="sxs-lookup"><span data-stu-id="ba116-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="ba116-116">調整ファイル ( **ChargeType** 列) の料金の種類については、「 [調整ファイルの料金の種類](recon-file-charge-types.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba116-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="ba116-117">書式設定の問題の修正</span><span class="sxs-lookup"><span data-stu-id="ba116-117">Fix formatting issues</span></span>

<span data-ttu-id="ba116-118">場合によっては、調整ファイルに書式設定の問題が含まれていることがあります。</span><span class="sxs-lookup"><span data-stu-id="ba116-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="ba116-119">たとえば、en-us ロケールが使用されていない場合に、この問題が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ba116-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="ba116-120">調整ファイルの書式設定に関する問題を修正するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="ba116-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="ba116-121">Microsoft Excel で調整ファイル (.csv 形式) を開きます。</span><span class="sxs-lookup"><span data-stu-id="ba116-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="ba116-122">ファイルの最初の列を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="ba116-123">**テキストを列に変換ウィザード** を開きます。</span><span class="sxs-lookup"><span data-stu-id="ba116-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="ba116-124">リボンで、[ **データ**] を選択し、[ **列のテキスト**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="ba116-125">ウィザードで、[区切られた **ファイルの種類**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="ba116-126">次に、 **[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="ba116-127">[ **区切り記号** ] ボックスで、[ **コンマ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="ba116-128">( **タブ** が既に選択されている場合は、このオプションを選択したままにしておくことができます)。次に、[ **次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="ba116-129">[ **列のデータ形式** ] フィールドで、[ **Date: MDY**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="ba116-130">次に、 **[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="ba116-131">[ **列のデータ形式** ] フィールドで、[すべての金額列] の **テキスト** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="ba116-132">次に、 **[Finish]\(完了\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="ba116-133">プログラムによる調整ファイルのダウンロード</span><span class="sxs-lookup"><span data-stu-id="ba116-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="ba116-134">調整ファイルは非常に大きくなる可能性があり、ダウンロードが困難な場合があります。</span><span class="sxs-lookup"><span data-stu-id="ba116-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="ba116-135">プログラムによって調整ファイルをダウンロードするには、「 [請求書の品目を取得](/partner-center/develop/get-invoiceline-items)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba116-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="ba116-136">ファイルが Excel の行の制限を超えている場合</span><span class="sxs-lookup"><span data-stu-id="ba116-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="ba116-137">調整ファイルをダウンロードできても Microsoft Excel で開くことができない場合は、Excel で許可されているよりも多くの行がファイルに含まれていることを意味します。</span><span class="sxs-lookup"><span data-stu-id="ba116-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="ba116-138">この問題が発生した場合は、次のいずれかの手順を使用してファイルを開くことができます。</span><span class="sxs-lookup"><span data-stu-id="ba116-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="ba116-139">Power BI で偵察ファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="ba116-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="ba116-140">通常どおりに調整ファイルをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="ba116-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="ba116-141">Power BI のインスタンスをダウンロード、インストール、および開く。</span><span class="sxs-lookup"><span data-stu-id="ba116-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="ba116-142">Power BI **ホーム** ] タブで、[ **データの取得**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="ba116-143">**共通データソース** の一覧で、[ **Text/CSV**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="ba116-144">メッセージが表示されたら、偵察ファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="ba116-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="ba116-145">Excel ピボットテーブルで偵察ファイルを開く</span><span class="sxs-lookup"><span data-stu-id="ba116-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="ba116-146">通常どおりに調整ファイルをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="ba116-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="ba116-147">Microsoft Excel で新しいファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="ba116-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="ba116-148">[ **データ** ] タブで [ **データの取得**] を選択し、[ **ファイルから**] を選択して、[ **Text/CSV**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="ba116-149">メッセージが表示されたら、偵察ファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="ba116-149">When prompted, open your recon file.</span></span> <span data-ttu-id="ba116-150">データが表示されます。</span><span class="sxs-lookup"><span data-stu-id="ba116-150">Your data will appear.</span></span>
5. <span data-ttu-id="ba116-151">[ **読み込み** ] ドロップダウンメニューで、[ **読み込み先**] を選択し、[ **OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ba116-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="ba116-152">[ **データのインポート** ] ダイアログボックスで、[ **PivotTable レポート** ] を選択してファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="ba116-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="ba116-153">税または VAT をマップする</span><span class="sxs-lookup"><span data-stu-id="ba116-153">Map taxes or VAT</span></span>

<span data-ttu-id="ba116-154">税金または付加価値税 (VAT) を請求書にマッピングするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="ba116-154">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="ba116-155">ライセンスベースのファイルから **税** 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="ba116-155">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="ba116-156">使用状況に基づくファイルから **taxationitem.taxamount** 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="ba116-156">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="ba116-157">パートナー別の調整ファイルの明細</span><span class="sxs-lookup"><span data-stu-id="ba116-157">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="ba116-158">**間接モデル** のパートナーは、これらの追加フィールドをライセンスベースと使用状況に基づく調整ファイルの両方で使用して、リセラーごとにファイルを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="ba116-158">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="ba116-159">MPN ID</span><span class="sxs-lookup"><span data-stu-id="ba116-159">MPN ID</span></span> | <span data-ttu-id="ba116-160">説明</span><span class="sxs-lookup"><span data-stu-id="ba116-160">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="ba116-161">MPN ID</span><span class="sxs-lookup"><span data-stu-id="ba116-161">MPN ID</span></span> | <span data-ttu-id="ba116-162">クラウドソリューションプロバイダー (CSP) パートナー (直接または間接) の Microsoft Partner Network (MPN) 識別子。</span><span class="sxs-lookup"><span data-stu-id="ba116-162">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="ba116-163">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="ba116-163">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="ba116-164">[サブスクリプションの販売店の MPN 識別子](#reseller-mpn-id)。</span><span class="sxs-lookup"><span data-stu-id="ba116-164">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="ba116-165">このフィールドは、パートナーセンターの特定のサブスクリプションについて一覧表示されているリセラー ID に対応しています。</span><span class="sxs-lookup"><span data-stu-id="ba116-165">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="ba116-166">インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="ba116-166">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="ba116-167">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="ba116-167">Reseller MPN ID</span></span>

<span data-ttu-id="ba116-168">CSP パートナーが顧客にサブスクリプションを直接販売した場合、 **MPN id** と **再販業者の MPN id** の両方として、 **MPN id** が2回表示されます。</span><span class="sxs-lookup"><span data-stu-id="ba116-168">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="ba116-169">CSP パートナーが **MPN id** のない再販業者を持っている場合、この値は代わりにパートナーの **MPN id** に設定されます。</span><span class="sxs-lookup"><span data-stu-id="ba116-169">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="ba116-170">CSP パートナーが **リセラーの MPN ID** を削除した場合、この値は *-1* に設定されます。</span><span class="sxs-lookup"><span data-stu-id="ba116-170">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="ba116-171">**リセラー MPN ID** を表示または更新するには:</span><span class="sxs-lookup"><span data-stu-id="ba116-171">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="ba116-172">パートナー センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="ba116-172">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="ba116-173">パートナー センター メニューで、**[顧客]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="ba116-173">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="ba116-174">一覧から顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-174">Choose the customer from the list.</span></span>
4. <span data-ttu-id="ba116-175">カスタマーメニューで、[ **サブスクリプション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-175">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="ba116-176">一覧からサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="ba116-176">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="ba116-177">**[更新]** を選んで、**[再販業者 (MPN ID)]** を変更します。</span><span class="sxs-lookup"><span data-stu-id="ba116-177">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ba116-178">次のステップ</span><span class="sxs-lookup"><span data-stu-id="ba116-178">Next steps</span></span>

- [<span data-ttu-id="ba116-179">請求書 & 偵察ファイルを読み取る方法</span><span class="sxs-lookup"><span data-stu-id="ba116-179">How to read your bill & recon file</span></span>](read-your-bill.md) 