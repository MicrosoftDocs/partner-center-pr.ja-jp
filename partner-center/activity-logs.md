---
title: 顧客のアクティビティログで洞察を得る
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: アクティビティログを表示およびエクスポートして、顧客のアカウントトランザクションやその他の顧客関連のパートナー管理アクティビティに関する洞察を得る方法について説明します。
author: LauraBrenner
ms.author: labrenne
Keywords: アクティビティ ログ, サブスクリプション, サブスクリプション, 支払い, 課金, トランザクション
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cfef9a4e6c68496ffbe9e9f6abc25629e2d2eb73
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991156"
---
# <a name="view-or-export-customer-activity-logs-for-more-insight-into-customer-transactions"></a><span data-ttu-id="21940-104">顧客のアクティビティログを表示またはエクスポートして、顧客トランザクションの詳細を把握します</span><span class="sxs-lookup"><span data-stu-id="21940-104">View or export customer activity logs for more insight into customer transactions</span></span>

<span data-ttu-id="21940-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="21940-105">**Applies to**</span></span>

- <span data-ttu-id="21940-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="21940-106">Partner Center</span></span>
- <span data-ttu-id="21940-107">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="21940-107">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="21940-108">クラウド ソリューション プロバイダー プログラム パートナー</span><span class="sxs-lookup"><span data-stu-id="21940-108">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="21940-109">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="21940-109">**Appropriate roles**</span></span>

- <span data-ttu-id="21940-110">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="21940-110">Global admin</span></span>
- <span data-ttu-id="21940-111">課金管理者</span><span class="sxs-lookup"><span data-stu-id="21940-111">Billing admin</span></span>
- <span data-ttu-id="21940-112">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="21940-112">User management admin</span></span>
- <span data-ttu-id="21940-113">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="21940-113">Admin agent</span></span>
- <span data-ttu-id="21940-114">販売代理店</span><span class="sxs-lookup"><span data-stu-id="21940-114">Sales agent</span></span>
- <span data-ttu-id="21940-115">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="21940-115">Helpdesk agent</span></span>

<span data-ttu-id="21940-116">アクティビティ ログは、顧客の取引やパートナーによる顧客の管理アクションに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="21940-116">Activity logs provide information on transactions and Partner management actions for customers.</span></span> <span data-ttu-id="21940-117">取引のログは、サブスクリプションの購入など、取引に関する詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="21940-117">Logs for transactions provide detailed information about the transaction, including purchased subscriptions.</span></span> <span data-ttu-id="21940-118">Excel 互換のコンマ区切り値ファイル形式 (.csv) でアクティビティ ログをエクスポートすることもできます。</span><span class="sxs-lookup"><span data-stu-id="21940-118">You can also export activity logs to an Excel-compatible comma-separated value file format (.csv).</span></span>

<span data-ttu-id="21940-119">アクティビティ ログは、顧客アカウントや製品の取引に対するパートナーのアクションのレコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="21940-119">Activity logs provide records for Partner actions on customer accounts and product transactions.</span></span> <span data-ttu-id="21940-120">アクティビティ ログを .csv ファイルにエクスポートすることもできます。</span><span class="sxs-lookup"><span data-stu-id="21940-120">You can also export activity logs to a .csv file.</span></span>

<span data-ttu-id="21940-121">**アクティビティ ログを表示およびエクスポートする**</span><span class="sxs-lookup"><span data-stu-id="21940-121">**View and export activity logs**</span></span>

1. <span data-ttu-id="21940-122">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="21940-122">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="21940-123">**[アカウント設定]** メニューの **[アクティビティ ログ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="21940-123">From the **Account settings** menu, select **Activity Log**.</span></span>
2.  <span data-ttu-id="21940-124">**[開始]** フィールドと **[終了]** フィールドで、アクティビティ ログの期間を選びます。</span><span class="sxs-lookup"><span data-stu-id="21940-124">Select the activity log period in the **From** and **to** fields.</span></span> <span data-ttu-id="21940-125">アクティビティ ログの既定の設定では、最近 1 か月間のログがエクスポートされます。</span><span class="sxs-lookup"><span data-stu-id="21940-125">The activity log export defaults to the most recent month.</span></span>

    <span data-ttu-id="21940-126">各アクティビティ ログには、一覧に表示されている顧客の **[サブスクリプション]** ページへのリンクが示されます。</span><span class="sxs-lookup"><span data-stu-id="21940-126">Each activity log provides a link to the listed customer's **Subscriptions** page.</span></span>

    <span data-ttu-id="21940-127">ログに記録されたアクションの詳細を表示するには、アクティビティ ログの下矢印を選びます。</span><span class="sxs-lookup"><span data-stu-id="21940-127">Select a down arrow for any activity log to view details about a logged action.</span></span> <span data-ttu-id="21940-128">1 つのアクティビティ ログには、複数の製品の注文など、相当な量のデータが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="21940-128">A single activity log can show a significant amount of data, such as the ordering of multiple products.</span></span>

3.   <span data-ttu-id="21940-129">ログのデータ列には、次のものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="21940-129">The data columns of the log include the following:</span></span>
    -   <span data-ttu-id="21940-130">**[日時]**: アクションの日付と時刻です。</span><span class="sxs-lookup"><span data-stu-id="21940-130">**Date-Time**-the date and time of the action;</span></span>
    -   <span data-ttu-id="21940-131">**[影響を受けるユーザー]**: 顧客の会社名です。</span><span class="sxs-lookup"><span data-stu-id="21940-131">**Affected customer**—the customer's company name;</span></span>
    -   <span data-ttu-id="21940-132">**[アクション]**: "紹介を作成した" など、顧客によって実行されたアクションです。</span><span class="sxs-lookup"><span data-stu-id="21940-132">**Action**—the action taken by the customer such as "created a referral";</span></span>
    -   <span data-ttu-id="21940-133">**[パートナー ユーザー]**: アクティビティに関連付けられているパートナーです。</span><span class="sxs-lookup"><span data-stu-id="21940-133">**Partner user**—the partner associated with the activity.</span></span>

4.  <span data-ttu-id="21940-134">**[ログのエクスポート]** を選択し、顧客のサブスクリプション データを .csv ファイルにコピーして、お使いのコンピューター上の既定のダウンロード フォルダーにダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="21940-134">Select **Export log** to copy the customer's subscription data into a .csv file and download it to the default download folder on your computer.</span></span>
    
 

 



