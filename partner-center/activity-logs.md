---
title: 顧客のアクティビティ ログを表示する | パートナー センター
ms.topic: article
ms.date: 08/23/2019
description: アクティビティ ログは、顧客の取引やパートナーによる顧客の管理アクションに関する情報を提供します。
ms.assetid: 2e8ea634-9f76-4005-9274-e104170c2ed5
author: MaggiePucciEvans
ms.author: evansma
Keywords: アクティビティ ログ, サブスクリプション, サブスクリプション, 支払い, 課金, トランザクション
ms.localizationpriority: medium
ms.openlocfilehash: 4cfbbf48122de87d5e3b650862ab83d0ee27ff04
ms.sourcegitcommit: c14db60f552f6e8349170b6ca825dbd073965c03
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/23/2019
ms.locfileid: "69993956"
---
# <a name="view-customer-activity-logs"></a><span data-ttu-id="cdc0e-104">顧客のアクティビティ ログの表示</span><span class="sxs-lookup"><span data-stu-id="cdc0e-104">View customer activity logs</span></span>

<span data-ttu-id="cdc0e-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="cdc0e-105">**Applies to**</span></span>

-  <span data-ttu-id="cdc0e-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="cdc0e-106">Partner Center</span></span>
-  <span data-ttu-id="cdc0e-107">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="cdc0e-107">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="cdc0e-108">アクティビティ ログは、顧客の取引やパートナーによる顧客の管理アクションに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-108">Activity logs provide information on transactions and Partner management actions for customers.</span></span> <span data-ttu-id="cdc0e-109">取引のログは、サブスクリプションの購入など、取引に関する詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-109">Logs for transactions provide detailed information about the transaction, including purchased subscriptions.</span></span> <span data-ttu-id="cdc0e-110">Excel 互換のコンマ区切り値ファイル形式 (.csv) でアクティビティ ログをエクスポートすることもできます。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-110">You can also export activity logs to an Excel-compatible comma-separated value file format (.csv).</span></span>

<span data-ttu-id="cdc0e-111">アクティビティ ログは、顧客アカウントや製品の取引に対するパートナーのアクションのレコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-111">Activity logs provide records for Partner actions on customer accounts and product transactions.</span></span> <span data-ttu-id="cdc0e-112">アクティビティ ログを .csv ファイルにエクスポートすることもできます。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-112">You can also export activity logs to a .csv file.</span></span>

<span data-ttu-id="cdc0e-113">**アクティビティ ログを表示およびエクスポートする**</span><span class="sxs-lookup"><span data-stu-id="cdc0e-113">**View and export activity logs**</span></span>

1.  <span data-ttu-id="cdc0e-114">**[アカウント設定]** メニューの **[アクティビティ ログ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-114">From the **Account settings** menu, select **Activity Log**.</span></span>
2.  <span data-ttu-id="cdc0e-115">**[開始]** フィールドと **[終了]** フィールドで、アクティビティ ログの期間を選びます。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-115">Select the activity log period in the **From** and **to** fields.</span></span> <span data-ttu-id="cdc0e-116">アクティビティ ログの既定の設定では、最近 1 か月間のログがエクスポートされます。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-116">The activity log export defaults to the most recent month.</span></span>

    <span data-ttu-id="cdc0e-117">各アクティビティ ログには、一覧に表示されている顧客の **[サブスクリプション]** ページへのリンクが示されます。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-117">Each activity log provides a link to the listed customer's **Subscriptions** page.</span></span>

    <span data-ttu-id="cdc0e-118">ログに記録されたアクションの詳細を表示するには、アクティビティ ログの下矢印を選びます。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-118">Select a down arrow for any activity log to view details about a logged action.</span></span> <span data-ttu-id="cdc0e-119">1 つのアクティビティ ログには、複数の製品の注文など、相当な量のデータが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-119">A single activity log can show a significant amount of data, such as the ordering of multiple products.</span></span>

3.   <span data-ttu-id="cdc0e-120">ログのデータ列には、次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-120">The data columns of the log include the following:</span></span>
    -   <span data-ttu-id="cdc0e-121">**[日時]** : アクションの日付と時刻です。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-121">**Date-Time**-the date and time of the action;</span></span>
    -   <span data-ttu-id="cdc0e-122">**[影響を受けるユーザー]** : 顧客の会社名です。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-122">**Affected customer**—the customer's company name;</span></span>
    -   <span data-ttu-id="cdc0e-123">**[アクション]** : "紹介を作成した" など、顧客によって実行されたアクションです。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-123">**Action**—the action taken by the customer such as "created a referral";</span></span>
    -   <span data-ttu-id="cdc0e-124">**[パートナー ユーザー]** : アクティビティに関連付けられているパートナーです。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-124">**Partner user**—the partner associated with the activity.</span></span>

4.  <span data-ttu-id="cdc0e-125">**[ログのエクスポート]** を選択し、顧客のサブスクリプション データを .csv ファイルにコピーして、お使いのコンピューター上の既定のダウンロード フォルダーにダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="cdc0e-125">Select **Export log** to copy the customer's subscription data into a .csv file and download it to the default download folder on your computer.</span></span>
    
 

 



