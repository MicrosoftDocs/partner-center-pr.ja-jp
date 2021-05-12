---
title: 調整ファイルを使用する
ms.topic: article
ms.date: 03/26/2021
description: このページの調整ファイルパートナー センター、特定の請求サイクルの請求の詳細な明細ビューを解釈する方法について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 755881d0bd96b9d601346ebb6271bd524c31d0a3
ms.sourcegitcommit: 837d3c5b52ab056b2b761cd85eb2426f56b62614
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/12/2021
ms.locfileid: "109794957"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="cc644-103">調整ファイル内の品目を読み取パートナー センター説明します</span><span class="sxs-lookup"><span data-stu-id="cc644-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="cc644-104">**適切なロール**: 課金管理者|グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="cc644-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="cc644-105">調整ファイルを パートナー センター からダウンロードして、請求サイクル内の各料金の詳細な明細ビューを確認できます。</span><span class="sxs-lookup"><span data-stu-id="cc644-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="cc644-106">品目の詳細には、各顧客のサブスクリプションの料金と、詳細なイベント (サブスクリプションへのライセンスの中間追加など) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="cc644-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="cc644-107">請求書を読み取る方法 **については、「請求書** を読む [」を参照してください](read-your-bill.md)。</span><span class="sxs-lookup"><span data-stu-id="cc644-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="cc644-108">調整ファイルのフィールドについて</span><span class="sxs-lookup"><span data-stu-id="cc644-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="cc644-109">ライセンス ベースの調整ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="cc644-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="cc644-110">使用量ベースの調整ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="cc644-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="cc644-111">毎日評価される使用状況調整ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="cc644-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="cc644-112">1 回購入 CSP 調整ファイルのフィールド</span><span class="sxs-lookup"><span data-stu-id="cc644-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="cc644-113">調整ファイルの料金の種類について</span><span class="sxs-lookup"><span data-stu-id="cc644-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="cc644-114">調整ファイルの料金の種類 **(ChargeType** 列) については、「調整ファイルの料金の種類 [」を参照してください](recon-file-charge-types.md)。</span><span class="sxs-lookup"><span data-stu-id="cc644-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="cc644-115">書式設定の問題を修正する</span><span class="sxs-lookup"><span data-stu-id="cc644-115">Fix formatting issues</span></span>

<span data-ttu-id="cc644-116">調整ファイルに書式設定の問題が含まれる場合があります。</span><span class="sxs-lookup"><span data-stu-id="cc644-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="cc644-117">たとえば、en-US ロケールが使用されていない場合、この問題が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="cc644-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="cc644-118">調整ファイルの書式設定の問題を解決するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="cc644-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="cc644-119">Microsoft Excel で調整ファイル (.csv 形式) を開きます。</span><span class="sxs-lookup"><span data-stu-id="cc644-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="cc644-120">ファイル内の最初の列を選択します。</span><span class="sxs-lookup"><span data-stu-id="cc644-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="cc644-121">[テキスト **を列に変換] ウィザードを開きます**。</span><span class="sxs-lookup"><span data-stu-id="cc644-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="cc644-122">リボンで [データ] を **選択し、[** 列にテキスト] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="cc644-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="cc644-123">ウィザードで、 [区切りファイル **の種類] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="cc644-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="cc644-124">次に、 **[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="cc644-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="cc644-125">[ **区切り記号** ] ボックスで、[ **コンマ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="cc644-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="cc644-126">( **タブ** が既に選択されている場合は、このオプションを選択したままにしておくことができます)。次に、[ **次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="cc644-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="cc644-127">[ **列のデータ形式** ] フィールドで、[ **Date: MDY**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="cc644-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="cc644-128">次に、 **[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="cc644-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="cc644-129">[ **列のデータ形式** ] フィールドで、[すべての金額列] の **テキスト** を選択します。</span><span class="sxs-lookup"><span data-stu-id="cc644-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="cc644-130">次に、 **[Finish]\(完了\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="cc644-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="cc644-131">プログラムによる調整ファイルのダウンロード</span><span class="sxs-lookup"><span data-stu-id="cc644-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="cc644-132">調整ファイルは非常に大きくなる可能性があり、ダウンロードが困難な場合があります。</span><span class="sxs-lookup"><span data-stu-id="cc644-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="cc644-133">プログラムによって調整ファイルをダウンロードするには、「 [請求書の品目を取得](/partner-center/develop/get-invoiceline-items)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc644-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="cc644-134">ファイルが Excel の行の制限を超えている場合</span><span class="sxs-lookup"><span data-stu-id="cc644-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="cc644-135">調整ファイルをダウンロードできても Microsoft Excel で開くことができない場合は、Excel で許可されているよりも多くの行がファイルに含まれていることを意味します。</span><span class="sxs-lookup"><span data-stu-id="cc644-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="cc644-136">この問題が発生した場合は、次のいずれかの手順を使用してファイルを開くことができます。</span><span class="sxs-lookup"><span data-stu-id="cc644-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="cc644-137">Power BI で偵察ファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="cc644-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="cc644-138">通常どおりに調整ファイルをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="cc644-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="cc644-139">Power BI のインスタンスをダウンロード、インストール、および開く。</span><span class="sxs-lookup"><span data-stu-id="cc644-139">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="cc644-140">Power BI **ホーム** ] タブで、[ **データの取得**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="cc644-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="cc644-141">**共通データソース** の一覧で、[ **Text/CSV**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="cc644-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="cc644-142">メッセージが表示されたら、偵察ファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="cc644-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="cc644-143">Excel ピボットテーブルで偵察ファイルを開く</span><span class="sxs-lookup"><span data-stu-id="cc644-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="cc644-144">通常どおりに調整ファイルをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="cc644-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="cc644-145">Microsoft Excel で新しいファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="cc644-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="cc644-146">[ **データ** ] タブで [ **データの取得**] を選択し、[ **ファイルから**] を選択して、[ **Text/CSV**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="cc644-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="cc644-147">メッセージが表示されたら、recon ファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="cc644-147">When prompted, open your recon file.</span></span> <span data-ttu-id="cc644-148">データが表示されます。</span><span class="sxs-lookup"><span data-stu-id="cc644-148">Your data will appear.</span></span>
5. <span data-ttu-id="cc644-149">[読み **込み]** ドロップダウン メニューで、[ に読み込む] **を選択** し、 **[OK] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="cc644-149">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="cc644-150">[データ **のインポート] ダイアログ** ボックスで、[ピボットテーブル レポート **] を選択して** ファイルを開きます。</span><span class="sxs-lookup"><span data-stu-id="cc644-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="cc644-151">表示される負の金額</span><span class="sxs-lookup"><span data-stu-id="cc644-151">Negative amount displayed</span></span>

<span data-ttu-id="cc644-152">調整ファイルに負の金額が表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="cc644-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="cc644-153">おそらく、これは次のいずれかが原因で起こります。</span><span class="sxs-lookup"><span data-stu-id="cc644-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="cc644-154">ライセンス数を最近取り消した、または減らした</span><span class="sxs-lookup"><span data-stu-id="cc644-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="cc644-155">サービス ライセンス契約 (SLA) または Azure の使用に対してクレジットを受け取った</span><span class="sxs-lookup"><span data-stu-id="cc644-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="cc644-156">このトランザクションの詳細情報を取得するには、調整ファイルでその料金の種類の属性を確認します。</span><span class="sxs-lookup"><span data-stu-id="cc644-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="cc644-157">税金または VAT をマップする</span><span class="sxs-lookup"><span data-stu-id="cc644-157">Map taxes or VAT</span></span>

<span data-ttu-id="cc644-158">税または付加価値税 (VAT) を請求書にマップするには:</span><span class="sxs-lookup"><span data-stu-id="cc644-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="cc644-159">ライセンス ベース **のファイル** の Tax 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="cc644-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="cc644-160">使用状況ベース **のファイルから TaxAmount** 列を合計します。</span><span class="sxs-lookup"><span data-stu-id="cc644-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="cc644-161">パートナー別に調整ファイルを項目化する</span><span class="sxs-lookup"><span data-stu-id="cc644-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="cc644-162">間接モデルの **パートナーは、** ライセンス ベースの調整ファイルと使用状況ベースの調整ファイルの両方でこれらの追加フィールドを使用して、リセラー別にファイルを明細化できます。</span><span class="sxs-lookup"><span data-stu-id="cc644-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="cc644-163">MPN ID</span><span class="sxs-lookup"><span data-stu-id="cc644-163">MPN ID</span></span> | <span data-ttu-id="cc644-164">説明</span><span class="sxs-lookup"><span data-stu-id="cc644-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="cc644-165">MPN ID</span><span class="sxs-lookup"><span data-stu-id="cc644-165">MPN ID</span></span> | <span data-ttu-id="cc644-166">CSP Microsoft Partner Network (直接または間接) クラウド ソリューション プロバイダー (MPN) 識別子。</span><span class="sxs-lookup"><span data-stu-id="cc644-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="cc644-167">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="cc644-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="cc644-168">サブスクリプション [のレコードのリセラーの MPN 識別子](#reseller-mpn-id)。</span><span class="sxs-lookup"><span data-stu-id="cc644-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="cc644-169">このフィールドは、サブスクリプション内の特定のサブスクリプションに対して一覧表示されているリセラー ID にパートナー センター。</span><span class="sxs-lookup"><span data-stu-id="cc644-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="cc644-170">インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="cc644-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="cc644-171">リセラーの MPN ID</span><span class="sxs-lookup"><span data-stu-id="cc644-171">Reseller MPN ID</span></span>

<span data-ttu-id="cc644-172">CSP パートナーがサブスクリプションを顧客に直接販売した場合 **、MPN ID** は MPN ID と Reseller **MPN ID** の両方として 2 回 **表示されます**。</span><span class="sxs-lookup"><span data-stu-id="cc644-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="cc644-173">CSP パートナーに **MPN ID** がないリセラーがある場合、この値は代わりにパートナーの **MPN ID に** 設定されます。</span><span class="sxs-lookup"><span data-stu-id="cc644-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="cc644-174">CSP パートナーが Reseller **MPN ID** を削除した場合、この値は *-1 に設定されます*。</span><span class="sxs-lookup"><span data-stu-id="cc644-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="cc644-175">**リセラー MPN ID** を表示または更新するには:</span><span class="sxs-lookup"><span data-stu-id="cc644-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="cc644-176">パートナー センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="cc644-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="cc644-177">パートナー センター メニューで、**[顧客]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="cc644-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="cc644-178">一覧から顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="cc644-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="cc644-179">カスタマーメニューで、[ **サブスクリプション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="cc644-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="cc644-180">一覧からサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="cc644-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="cc644-181">**[更新]** を選んで、**[再販業者 (MPN ID)]** を変更します。</span><span class="sxs-lookup"><span data-stu-id="cc644-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="cc644-182">次の手順</span><span class="sxs-lookup"><span data-stu-id="cc644-182">Next steps</span></span>

- [<span data-ttu-id="cc644-183">請求書 & 偵察ファイルを読み取る方法</span><span class="sxs-lookup"><span data-stu-id="cc644-183">How to read your bill & recon file</span></span>](read-your-bill.md) 