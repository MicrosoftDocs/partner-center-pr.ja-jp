---
title: 顧客を Microsoft Azure 予約に販売する
description: クラウドソリューションプロバイダーとして、顧客向けの Azure 予約を購入、販売、管理することができます。 パートナーセンター、Azure portal、またはパートナーセンター API を使用します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 9dc92685503fd4b9b05e40337f72e810c1693779
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534898"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="d3b7a-104">パートナーセンター、Azure portal、Api を使用して Microsoft Azure の予約を顧客に販売する</span><span class="sxs-lookup"><span data-stu-id="d3b7a-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="d3b7a-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="d3b7a-105">**Appropriate roles**</span></span>

- <span data-ttu-id="d3b7a-106">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="d3b7a-106">Admin agent</span></span>
- <span data-ttu-id="d3b7a-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="d3b7a-107">Global admin</span></span>
- <span data-ttu-id="d3b7a-108">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="d3b7a-108">Helpdesk agent</span></span>
- <span data-ttu-id="d3b7a-109">販売代理店</span><span class="sxs-lookup"><span data-stu-id="d3b7a-109">Sales agent</span></span>
- <span data-ttu-id="d3b7a-110">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="d3b7a-110">User management admin</span></span>

<span data-ttu-id="d3b7a-111">クラウドソリューションプロバイダープログラム (CSP) のパートナーとして、顧客向けの Azure 予約を購入、販売、管理することができます。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-111">As a partner in the Cloud Solution Provider program (CSP), you can buy, sell, or manage Azure reservations for customers.</span></span> <span data-ttu-id="d3b7a-112">パートナーセンター、Azure portal、またはパートナーセンター API を使用します。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-112">Use Partner Center, the Azure portal, or the Partner Center API.</span></span>

> [!NOTE]
> <span data-ttu-id="d3b7a-113">この記事は、CSP のパートナーにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-113">This article applies only to partners in CSP.</span></span> <span data-ttu-id="d3b7a-114">他の種類のサブスクリプション (従量課金制、個人、Microsoft カスタマーアグリーメント、マイクロソフトエンタープライズ契約サブスクリプションなど) を使用しているお客様は、代わりに [この Azure 予約ドキュメント](/azure/cost-management-billing/reservations)を読む必要があります。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-114">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="d3b7a-115">CSP プログラムのパートナーは、お客様に Microsoft Azure 予約を提供できます。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-115">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="d3b7a-116">事前に予約した場合、顧客はコストを大幅に節約できます。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="d3b7a-117">Azure Reservations では顧客の皆様に、次のように簡単で柔軟にご利用いただけます。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="d3b7a-118">1 ～ 3 年の予約期間。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="d3b7a-119">簡単に使い始めることができます。セットアップは数秒で完了します。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="d3b7a-120">予約インスタンスはいつでも取り消しまたは交換でき、払い戻しが調整されます。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="d3b7a-121">組織レベルまたは個々の部署レベルで予約インスタンスの使用状況を管理できます。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-121">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="d3b7a-122">Azure Reservations は、次の点で顧客にとって魅力的です。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="d3b7a-123">予約では、従量課金制 (PAYG) の価格設定で大幅にコストを節約できます。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="d3b7a-124">1 年間または 3 年間の前払いにより、予算編成と支払い計画が容易になります。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="d3b7a-125">オフィスに近い Azure リージョンでコンピューティング処理能力を優先させることができます。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="d3b7a-126">Azure Reservations を Microsoft Windows Server や Azure SQL Database などのソフトウェアと組み合わせることで、エンドツーエンドのインフラストラクチャ ソリューション基盤が提供されます。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="d3b7a-127">Azure Reservations は、パートナー センター、Azure portal、およびパートナー センター API を使用して購入、販売、管理できます。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="d3b7a-128">購入した Azure サブスクリプションから独自の Azure 予約を購入するためのアクセス許可を顧客に付与することもできます。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="d3b7a-129">方法については、各リンク先をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="d3b7a-130">Azure Reservations に関するリソース</span><span class="sxs-lookup"><span data-stu-id="d3b7a-130">Azure reservations resources</span></span>

|<span data-ttu-id="d3b7a-131">**対象**</span><span class="sxs-lookup"><span data-stu-id="d3b7a-131">**For information about**</span></span>   |<span data-ttu-id="d3b7a-132">**参照先**</span><span class="sxs-lookup"><span data-stu-id="d3b7a-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="d3b7a-133">顧客向けの Azure Reservations に関するドキュメント</span><span class="sxs-lookup"><span data-stu-id="d3b7a-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="d3b7a-134">Azure の予約とは</span><span class="sxs-lookup"><span data-stu-id="d3b7a-134">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="d3b7a-135">パートナー センターで顧客の Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="d3b7a-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="d3b7a-136">Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="d3b7a-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="d3b7a-137">パートナー センターでの Azure Reservations の管理</span><span class="sxs-lookup"><span data-stu-id="d3b7a-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="d3b7a-138">パートナー センターでの Azure Reservations の管理</span><span class="sxs-lookup"><span data-stu-id="d3b7a-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="d3b7a-139">適切な VM サイズの判断と顧客による VM 使用状況の確認</span><span class="sxs-lookup"><span data-stu-id="d3b7a-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="d3b7a-140">Azure Reservation の最大使用量に対応する VM サイズ</span><span class="sxs-lookup"><span data-stu-id="d3b7a-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="d3b7a-141">パートナー センター API を使用して Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="d3b7a-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="d3b7a-142">[Azure Reserved VM Instances の購入](/partner-center/develop/purchase-azure-reservations) (パートナー センター開発者向けドキュメント)</span><span class="sxs-lookup"><span data-stu-id="d3b7a-142">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="d3b7a-143">CSP サブスクリプションから独自の Azure 予約を購入するためのアクセス許可を顧客に付与します。</span><span class="sxs-lookup"><span data-stu-id="d3b7a-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="d3b7a-144">独自の Azure 予約を購入するためのアクセス許可を顧客に付与する</span><span class="sxs-lookup"><span data-stu-id="d3b7a-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |