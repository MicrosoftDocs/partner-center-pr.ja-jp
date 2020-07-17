---
title: 顧客のアクティビティログで洞察を得る
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: アクティビティログを表示およびエクスポートして、顧客のアカウントトランザクションやその他の顧客関連のパートナー管理アクティビティに関する洞察を得る方法について説明します。
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 06cc76ee5689bbce5e8017f6bc5a664ff130c1ec
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436401"
---
# <a name="view-or-export-customer-activity-logs-for-more-insight-into-customer-transactions"></a><span data-ttu-id="28714-103">顧客のアクティビティログを表示またはエクスポートして、顧客トランザクションの詳細を把握します</span><span class="sxs-lookup"><span data-stu-id="28714-103">View or export customer activity logs for more insight into customer transactions</span></span>

<span data-ttu-id="28714-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="28714-104">**Applies to**</span></span>

- <span data-ttu-id="28714-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="28714-105">Partner Center</span></span>
- <span data-ttu-id="28714-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="28714-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="28714-107">クラウド ソリューション プロバイダー プログラム パートナー</span><span class="sxs-lookup"><span data-stu-id="28714-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="28714-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="28714-108">**Appropriate roles**</span></span>

- <span data-ttu-id="28714-109">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="28714-109">Global admin</span></span>
- <span data-ttu-id="28714-110">課金管理者</span><span class="sxs-lookup"><span data-stu-id="28714-110">Billing admin</span></span>
- <span data-ttu-id="28714-111">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="28714-111">User management admin</span></span>
- <span data-ttu-id="28714-112">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="28714-112">Admin agent</span></span>
- <span data-ttu-id="28714-113">販売代理店</span><span class="sxs-lookup"><span data-stu-id="28714-113">Sales agent</span></span>
- <span data-ttu-id="28714-114">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="28714-114">Helpdesk agent</span></span>

<span data-ttu-id="28714-115">アクティビティ ログは、顧客の取引やパートナーによる顧客の管理アクションに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="28714-115">Activity logs provide information on transactions and Partner management actions for customers.</span></span> <span data-ttu-id="28714-116">取引のログは、サブスクリプションの購入など、取引に関する詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="28714-116">Logs for transactions provide detailed information about the transaction, including purchased subscriptions.</span></span> <span data-ttu-id="28714-117">Excel 互換のコンマ区切り値ファイル形式 (.csv) でアクティビティ ログをエクスポートすることもできます。</span><span class="sxs-lookup"><span data-stu-id="28714-117">You can also export activity logs to an Excel-compatible comma-separated value file format (.csv).</span></span>

<span data-ttu-id="28714-118">アクティビティ ログは、顧客アカウントや製品の取引に対するパートナーのアクションのレコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="28714-118">Activity logs provide records for Partner actions on customer accounts and product transactions.</span></span> <span data-ttu-id="28714-119">アクティビティ ログを .csv ファイルにエクスポートすることもできます。</span><span class="sxs-lookup"><span data-stu-id="28714-119">You can also export activity logs to a .csv file.</span></span>

## <a name="view-and-export-activity-logs"></a><span data-ttu-id="28714-120">アクティビティ ログを表示およびエクスポートする</span><span class="sxs-lookup"><span data-stu-id="28714-120">View and export activity logs</span></span>

1. <span data-ttu-id="28714-121">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="28714-121">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="28714-122">**[アカウント設定]** メニューの **[アクティビティ ログ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="28714-122">From the **Account settings** menu, select **Activity Log**.</span></span>

3. <span data-ttu-id="28714-123">**[開始]** フィールドと **[終了]** フィールドで、アクティビティ ログの期間を選びます。</span><span class="sxs-lookup"><span data-stu-id="28714-123">Select the activity log period in the **From** and **to** fields.</span></span> <span data-ttu-id="28714-124">アクティビティ ログの既定の設定では、最近 1 か月間のログがエクスポートされます。</span><span class="sxs-lookup"><span data-stu-id="28714-124">The activity log export defaults to the most recent month.</span></span>

   <span data-ttu-id="28714-125">各アクティビティ ログには、一覧に表示されている顧客の **[サブスクリプション]** ページへのリンクが示されます。</span><span class="sxs-lookup"><span data-stu-id="28714-125">Each activity log provides a link to the listed customer's **Subscriptions** page.</span></span>

   <span data-ttu-id="28714-126">ログに記録されたアクションの詳細を表示するには、アクティビティ ログの下矢印を選びます。</span><span class="sxs-lookup"><span data-stu-id="28714-126">Select a down arrow for any activity log to view details about a logged action.</span></span> <span data-ttu-id="28714-127">1 つのアクティビティ ログには、複数の製品の注文など、相当な量のデータが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="28714-127">A single activity log can show a significant amount of data, such as the ordering of multiple products.</span></span>

4. <span data-ttu-id="28714-128">ログのデータ列には、次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="28714-128">The data columns of the log include the following:</span></span>
   - <span data-ttu-id="28714-129">**[日時]**: アクションの日付と時刻です。</span><span class="sxs-lookup"><span data-stu-id="28714-129">**Date-Time**-the date and time of the action;</span></span>
   - <span data-ttu-id="28714-130">**[影響を受けるユーザー]**: 顧客の会社名です。</span><span class="sxs-lookup"><span data-stu-id="28714-130">**Affected customer**—the customer's company name;</span></span>
   - <span data-ttu-id="28714-131">**[アクション]**: "紹介を作成した" など、顧客によって実行されたアクションです。</span><span class="sxs-lookup"><span data-stu-id="28714-131">**Action**—the action taken by the customer such as "created a referral";</span></span>
   - <span data-ttu-id="28714-132">**[パートナー ユーザー]**: アクティビティに関連付けられているパートナーです。</span><span class="sxs-lookup"><span data-stu-id="28714-132">**Partner user**—the partner associated with the activity.</span></span>

5. <span data-ttu-id="28714-133">**[ログのエクスポート]** を選択し、顧客のサブスクリプション データを .csv ファイルにコピーして、お使いのコンピューター上の既定のダウンロード フォルダーにダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="28714-133">Select **Export log** to copy the customer's subscription data into a .csv file and download it to the default download folder on your computer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="28714-134">次のステップ</span><span class="sxs-lookup"><span data-stu-id="28714-134">Next steps</span></span>

- [<span data-ttu-id="28714-135">サブスクリプションとライセンスを分析して、ビジネス上の意思決定を促進する</span><span class="sxs-lookup"><span data-stu-id="28714-135">Analyze subscriptions and licenses to help drive business decisions</span></span>](analyze-subscriptions-licenses.md)
