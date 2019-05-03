---
title: Azure 利用状況分析 | パートナー センター
ms.date: 07/12/2018
Description: パートナー センターを使用して、顧客の Azure サブスクリプションの利用状況に関するデータを取得します。
Author: Xansky
ms.author: mhopkins
ms.assetid: E7081190-C1FA-47C1-963B-6EBA1B33703B
ms.topic: article
keywords: ビジネス データ
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 9bd76a51664b18a8b3cea1e4163415480186fd86
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "62131873"
---
# <a name="get-data-about-the-usage-of-your-customers-azure-subscriptions"></a><span data-ttu-id="9a534-104">顧客の Azure サブスクリプションの利用状況に関するデータの取得</span><span class="sxs-lookup"><span data-stu-id="9a534-104">Get data about the usage of your customers' Azure subscriptions</span></span> 

<span data-ttu-id="9a534-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="9a534-105">**Applies to**</span></span>
- <span data-ttu-id="9a534-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="9a534-106">Partner Center</span></span>

<span data-ttu-id="9a534-107">データはビジネス上の意思決定を促進します。</span><span class="sxs-lookup"><span data-stu-id="9a534-107">Data drives business decisions.</span></span> <span data-ttu-id="9a534-108">**Azure 利用状況**のページのメトリックを使用して、パートナーの成功度や注意が必要な分野を把握します。</span><span class="sxs-lookup"><span data-stu-id="9a534-108">Use the metrics in the **Azure usage** page to identify your successes and areas that need more attention.</span></span> <span data-ttu-id="9a534-109">新しいビジネス目標を計画するときに、この情報を使用できます。</span><span class="sxs-lookup"><span data-stu-id="9a534-109">Use this information as you plan new business goals.</span></span>

> [!NOTE]
> <span data-ttu-id="9a534-110">Azure 利用状況分析は、クラウド ソリューション プロバイダー プログラムに参加しているパートナーのみが利用できます。</span><span class="sxs-lookup"><span data-stu-id="9a534-110">Azure usage  analytics is available only for partners in the Cloud Solution Provider program.</span></span>

<span data-ttu-id="9a534-111">次のメトリックを追跡しています。</span><span class="sxs-lookup"><span data-stu-id="9a534-111">We are tracking the following metrics:</span></span>

<span data-ttu-id="9a534-112">**要約**</span><span class="sxs-lookup"><span data-stu-id="9a534-112">**Summary**</span></span>  
 - <span data-ttu-id="9a534-113">**Total Azure subscriptions sold** (Azure サブスクリプションの合計販売数):指定した期間に販売されたサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="9a534-113">**Total Azure subscriptions sold**: Number of subscriptions sold in the specified time period</span></span>  
 - <span data-ttu-id="9a534-114">**Customers with usage** (利用状況のある顧客数):指定した期間に Azure の利用状況がある顧客の数</span><span class="sxs-lookup"><span data-stu-id="9a534-114">**Customers with usage**: Number of customers with Azure usage in the specified time period</span></span>  
 - <span data-ttu-id="9a534-115">**Customers with usage** (利用状況のない顧客数):指定した期間に Azure の利用状況がない顧客の数</span><span class="sxs-lookup"><span data-stu-id="9a534-115">**Customers without usage**: Number of customers without Azure usage in the specified time period</span></span>  

<span data-ttu-id="9a534-116">**Top 5 customers in category** (カテゴリ内の上位 5 件の顧客)</span><span class="sxs-lookup"><span data-stu-id="9a534-116">**Top 5 customers in category**</span></span>  
 -  <span data-ttu-id="9a534-117">指定したカテゴリの上位 5 件の顧客</span><span class="sxs-lookup"><span data-stu-id="9a534-117">The top 5 customers for the specified category</span></span>  

<span data-ttu-id="9a534-118">**Subscriptions without usage** (利用状況のないサブスクリプション)</span><span class="sxs-lookup"><span data-stu-id="9a534-118">**Subscriptions without usage**</span></span>  
 -  <span data-ttu-id="9a534-119">指定した期間に Azure の利用状況がないサブスクリプションの一覧</span><span class="sxs-lookup"><span data-stu-id="9a534-119">List of sepcific subscriptions without Azure usage in the specified time period</span></span>  

<span data-ttu-id="9a534-120">**Azure subscription churn** (Azure サブスクリプションのチャーン)</span><span class="sxs-lookup"><span data-stu-id="9a534-120">**Azure subscription churn**</span></span>  
 - <span data-ttu-id="9a534-121">**Active subscriptions** (アクティブなサブスクリプション数):日付ごとのアクティブなサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="9a534-121">**Active subscriptions**: Count of active subscriptions by date</span></span>  
 - <span data-ttu-id="9a534-122">**Deprovisioned subscriptions** (プロビジョニング解除されたサブスクリプション数):日付ごとのプロビジョニング解除または中断されたサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="9a534-122">**Deprovisioned subscriptions**: Count of subscriptions deprovisioned or suspended by date</span></span>  

<span data-ttu-id="9a534-123">**Customer count** (顧客数)</span><span class="sxs-lookup"><span data-stu-id="9a534-123">**Customer count**</span></span>
 - <span data-ttu-id="9a534-124">指定した期間中に獲得した新規顧客数</span><span class="sxs-lookup"><span data-stu-id="9a534-124">New customers acquired during the specified time period</span></span>  

<span data-ttu-id="9a534-125">**Azure subscription retention** (Azure サブスクリプションの維持)</span><span class="sxs-lookup"><span data-stu-id="9a534-125">**Azure subscription retention**</span></span>  
 - <span data-ttu-id="9a534-126">更新されたサブスクリプションの数。</span><span class="sxs-lookup"><span data-stu-id="9a534-126">The number of subscriptions that were renewed.</span></span>   
  