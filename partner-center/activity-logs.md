---
title: 顧客アクティビティ ログを使用して分析情報を取得する
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: アクティビティ ログを表示およびエクスポートして、顧客アカウントのトランザクションや他の顧客関連のパートナー管理アクティビティに関する分析情報を取得する方法について説明します。
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1bb98dd71c9e46914b90d5efbfe14404d08275f9
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150592"
---
# <a name="view-or-export-customer-activity-logs-for-more-insight-into-customer-transactions"></a><span data-ttu-id="983f0-103">顧客のトランザクションに関する詳細な分析情報を得る場合は、顧客アクティビティ ログを表示またはエクスポートします</span><span class="sxs-lookup"><span data-stu-id="983f0-103">View or export customer activity logs for more insight into customer transactions</span></span>

<span data-ttu-id="983f0-104">**適切なロール**: グローバル管理者|課金管理者|ユーザー管理管理者|管理エージェント |Sales Agent |ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="983f0-104">**Appropriate roles**: Global admin | Billing admin | User management admin | Admin agent | Sales agent | Helpdesk agent</span></span>

<span data-ttu-id="983f0-105">アクティビティ ログは、顧客の取引やパートナーによる顧客の管理アクションに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="983f0-105">Activity logs provide information on transactions and Partner management actions for customers.</span></span> <span data-ttu-id="983f0-106">取引のログは、サブスクリプションの購入など、取引に関する詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="983f0-106">Logs for transactions provide detailed information about the transaction, including purchased subscriptions.</span></span> <span data-ttu-id="983f0-107">Excel 互換のコンマ区切り値ファイル形式 (.csv) でアクティビティ ログをエクスポートすることもできます。</span><span class="sxs-lookup"><span data-stu-id="983f0-107">You can also export activity logs to an Excel-compatible comma-separated value file format (.csv).</span></span>

<span data-ttu-id="983f0-108">アクティビティ ログは、顧客アカウントや製品の取引に対するパートナーのアクションのレコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="983f0-108">Activity logs provide records for Partner actions on customer accounts and product transactions.</span></span> <span data-ttu-id="983f0-109">アクティビティ ログを .csv ファイルにエクスポートすることもできます。</span><span class="sxs-lookup"><span data-stu-id="983f0-109">You can also export activity logs to a .csv file.</span></span>

## <a name="view-and-export-activity-logs"></a><span data-ttu-id="983f0-110">アクティビティ ログを表示およびエクスポートする</span><span class="sxs-lookup"><span data-stu-id="983f0-110">View and export activity logs</span></span>

1. <span data-ttu-id="983f0-111">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="983f0-111">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="983f0-112">**[アカウント設定]** メニューの **[アクティビティ ログ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="983f0-112">From the **Account settings** menu, select **Activity Log**.</span></span>

3. <span data-ttu-id="983f0-113">**[開始]** フィールドと **[終了]** フィールドで、アクティビティ ログの期間を選びます。</span><span class="sxs-lookup"><span data-stu-id="983f0-113">Select the activity log period in the **From** and **to** fields.</span></span> <span data-ttu-id="983f0-114">アクティビティ ログの既定の設定では、最近 1 か月間のログがエクスポートされます。</span><span class="sxs-lookup"><span data-stu-id="983f0-114">The activity log export defaults to the most recent month.</span></span>

   <span data-ttu-id="983f0-115">各アクティビティ ログには、一覧に表示されている顧客の **[サブスクリプション]** ページへのリンクが示されます。</span><span class="sxs-lookup"><span data-stu-id="983f0-115">Each activity log provides a link to the listed customer's **Subscriptions** page.</span></span>

   <span data-ttu-id="983f0-116">ログに記録されたアクションの詳細を表示するには、アクティビティ ログの下矢印を選びます。</span><span class="sxs-lookup"><span data-stu-id="983f0-116">Select a down arrow for any activity log to view details about a logged action.</span></span> <span data-ttu-id="983f0-117">1 つのアクティビティ ログには、複数の製品の注文など、相当な量のデータが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="983f0-117">A single activity log can show a significant amount of data, such as the ordering of multiple products.</span></span>

4. <span data-ttu-id="983f0-118">ログのデータ列には、次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="983f0-118">The data columns of the log include the following:</span></span>
   - <span data-ttu-id="983f0-119">**[日時]**: アクションの日付と時刻です。</span><span class="sxs-lookup"><span data-stu-id="983f0-119">**Date-Time**-the date and time of the action;</span></span>
   - <span data-ttu-id="983f0-120">**[影響を受けるユーザー]**: 顧客の会社名です。</span><span class="sxs-lookup"><span data-stu-id="983f0-120">**Affected customer**—the customer's company name;</span></span>
   - <span data-ttu-id="983f0-121">**[アクション]**: "紹介を作成した" など、顧客によって実行されたアクションです。</span><span class="sxs-lookup"><span data-stu-id="983f0-121">**Action**—the action taken by the customer such as "created a referral";</span></span>
   - <span data-ttu-id="983f0-122">**[パートナー ユーザー]**: アクティビティに関連付けられているパートナーです。</span><span class="sxs-lookup"><span data-stu-id="983f0-122">**Partner user**—the partner associated with the activity.</span></span>

5. <span data-ttu-id="983f0-123">**[ログのエクスポート]** を選択し、顧客のサブスクリプション データを .csv ファイルにコピーして、お使いのコンピューター上の既定のダウンロード フォルダーにダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="983f0-123">Select **Export log** to copy the customer's subscription data into a .csv file and download it to the default download folder on your computer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="983f0-124">次のステップ</span><span class="sxs-lookup"><span data-stu-id="983f0-124">Next steps</span></span>

- [<span data-ttu-id="983f0-125">サブスクリプションとライセンスを分析してビジネス上の意思決定を支援する</span><span class="sxs-lookup"><span data-stu-id="983f0-125">Analyze subscriptions and licenses to help drive business decisions</span></span>](analyze-subscriptions-licenses.md)
