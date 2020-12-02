---
title: 顧客のアクティビティログで洞察を得る
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: アクティビティログを表示およびエクスポートして、顧客のアカウントトランザクションやその他の顧客関連のパートナー管理アクティビティに関する洞察を得る方法について説明します。
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1eaa7fee628015eb633cac3a2796e371f6046585
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474242"
---
# <a name="view-or-export-customer-activity-logs-for-more-insight-into-customer-transactions"></a><span data-ttu-id="3f7b8-103">顧客のアクティビティログを表示またはエクスポートして、顧客トランザクションの詳細を把握します</span><span class="sxs-lookup"><span data-stu-id="3f7b8-103">View or export customer activity logs for more insight into customer transactions</span></span>

<span data-ttu-id="3f7b8-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="3f7b8-104">**Appropriate roles**</span></span>

- <span data-ttu-id="3f7b8-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="3f7b8-105">Global admin</span></span>
- <span data-ttu-id="3f7b8-106">課金管理者</span><span class="sxs-lookup"><span data-stu-id="3f7b8-106">Billing admin</span></span>
- <span data-ttu-id="3f7b8-107">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="3f7b8-107">User management admin</span></span>
- <span data-ttu-id="3f7b8-108">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="3f7b8-108">Admin agent</span></span>
- <span data-ttu-id="3f7b8-109">販売代理店</span><span class="sxs-lookup"><span data-stu-id="3f7b8-109">Sales agent</span></span>
- <span data-ttu-id="3f7b8-110">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="3f7b8-110">Helpdesk agent</span></span>

<span data-ttu-id="3f7b8-111">アクティビティ ログは、顧客の取引やパートナーによる顧客の管理アクションに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-111">Activity logs provide information on transactions and Partner management actions for customers.</span></span> <span data-ttu-id="3f7b8-112">取引のログは、サブスクリプションの購入など、取引に関する詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-112">Logs for transactions provide detailed information about the transaction, including purchased subscriptions.</span></span> <span data-ttu-id="3f7b8-113">Excel 互換のコンマ区切り値ファイル形式 (.csv) でアクティビティ ログをエクスポートすることもできます。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-113">You can also export activity logs to an Excel-compatible comma-separated value file format (.csv).</span></span>

<span data-ttu-id="3f7b8-114">アクティビティ ログは、顧客アカウントや製品の取引に対するパートナーのアクションのレコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-114">Activity logs provide records for Partner actions on customer accounts and product transactions.</span></span> <span data-ttu-id="3f7b8-115">アクティビティ ログを .csv ファイルにエクスポートすることもできます。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-115">You can also export activity logs to a .csv file.</span></span>

## <a name="view-and-export-activity-logs"></a><span data-ttu-id="3f7b8-116">アクティビティ ログを表示およびエクスポートする</span><span class="sxs-lookup"><span data-stu-id="3f7b8-116">View and export activity logs</span></span>

1. <span data-ttu-id="3f7b8-117">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-117">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3f7b8-118">**[アカウント設定]** メニューの **[アクティビティ ログ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-118">From the **Account settings** menu, select **Activity Log**.</span></span>

3. <span data-ttu-id="3f7b8-119">**[開始]** フィールドと **[終了]** フィールドで、アクティビティ ログの期間を選びます。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-119">Select the activity log period in the **From** and **to** fields.</span></span> <span data-ttu-id="3f7b8-120">アクティビティ ログの既定の設定では、最近 1 か月間のログがエクスポートされます。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-120">The activity log export defaults to the most recent month.</span></span>

   <span data-ttu-id="3f7b8-121">各アクティビティ ログには、一覧に表示されている顧客の **[サブスクリプション]** ページへのリンクが示されます。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-121">Each activity log provides a link to the listed customer's **Subscriptions** page.</span></span>

   <span data-ttu-id="3f7b8-122">ログに記録されたアクションの詳細を表示するには、アクティビティ ログの下矢印を選びます。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-122">Select a down arrow for any activity log to view details about a logged action.</span></span> <span data-ttu-id="3f7b8-123">1 つのアクティビティ ログには、複数の製品の注文など、相当な量のデータが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-123">A single activity log can show a significant amount of data, such as the ordering of multiple products.</span></span>

4. <span data-ttu-id="3f7b8-124">ログのデータ列には、次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-124">The data columns of the log include the following:</span></span>
   - <span data-ttu-id="3f7b8-125">**[日時]**: アクションの日付と時刻です。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-125">**Date-Time**-the date and time of the action;</span></span>
   - <span data-ttu-id="3f7b8-126">**[影響を受けるユーザー]**: 顧客の会社名です。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-126">**Affected customer**—the customer's company name;</span></span>
   - <span data-ttu-id="3f7b8-127">**[アクション]**: "紹介を作成した" など、顧客によって実行されたアクションです。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-127">**Action**—the action taken by the customer such as "created a referral";</span></span>
   - <span data-ttu-id="3f7b8-128">**[パートナー ユーザー]**: アクティビティに関連付けられているパートナーです。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-128">**Partner user**—the partner associated with the activity.</span></span>

5. <span data-ttu-id="3f7b8-129">**[ログのエクスポート]** を選択し、顧客のサブスクリプション データを .csv ファイルにコピーして、お使いのコンピューター上の既定のダウンロード フォルダーにダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="3f7b8-129">Select **Export log** to copy the customer's subscription data into a .csv file and download it to the default download folder on your computer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3f7b8-130">次のステップ</span><span class="sxs-lookup"><span data-stu-id="3f7b8-130">Next steps</span></span>

- [<span data-ttu-id="3f7b8-131">サブスクリプションとライセンスを分析して、ビジネス上の意思決定を促進する</span><span class="sxs-lookup"><span data-stu-id="3f7b8-131">Analyze subscriptions and licenses to help drive business decisions</span></span>](analyze-subscriptions-licenses.md)
