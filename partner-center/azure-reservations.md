---
title: 顧客を Microsoft Azure 予約に販売する
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: クラウドソリューションプロバイダーとして、顧客向けの Azure 予約を購入、販売、管理することができます。 パートナーセンター、Azure portal、またはパートナーセンター API を使用します。
author: LauraBrenner
ms.author: labrenne
keywords: Azure, 予約, 管理, 請求, 購入, Azure RI, Azure Reserved Instances
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5393e757b209de5a7df22b35a0cee0703419bef4
ms.sourcegitcommit: 595b7de03963a4a78cad8344bd4b5d4f5cff9802
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2020
ms.locfileid: "85198640"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="cf07c-105">パートナーセンター、Azure portal、Api を使用して Microsoft Azure の予約を顧客に販売する</span><span class="sxs-lookup"><span data-stu-id="cf07c-105">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="cf07c-106">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="cf07c-106">**Applies to**</span></span>

- <span data-ttu-id="cf07c-107">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="cf07c-107">Partner Center</span></span>
- <span data-ttu-id="cf07c-108">Microsoft Azure portal</span><span class="sxs-lookup"><span data-stu-id="cf07c-108">Microsoft Azure portal</span></span>
- <span data-ttu-id="cf07c-109">CSP のパートナー</span><span class="sxs-lookup"><span data-stu-id="cf07c-109">Partners in CSP</span></span>

<span data-ttu-id="cf07c-110">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="cf07c-110">**Appropriate roles**</span></span>

- <span data-ttu-id="cf07c-111">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="cf07c-111">Admin agent</span></span>
- <span data-ttu-id="cf07c-112">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="cf07c-112">Global admin</span></span>
- <span data-ttu-id="cf07c-113">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="cf07c-113">Helpdesk agent</span></span>
- <span data-ttu-id="cf07c-114">販売代理店</span><span class="sxs-lookup"><span data-stu-id="cf07c-114">Sales agent</span></span>
- <span data-ttu-id="cf07c-115">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="cf07c-115">User management admin</span></span>

<span data-ttu-id="cf07c-116">クラウド ソリューション プロバイダー プログラム (CSP) のパートナーは、Microsoft Azure Reservations を顧客に提供できます。</span><span class="sxs-lookup"><span data-stu-id="cf07c-116">Partners in the Cloud Solution Provider program (CSP) can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="cf07c-117">事前に予約した場合、顧客はコストを大幅に節約できます。</span><span class="sxs-lookup"><span data-stu-id="cf07c-117">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="cf07c-118">Azure Reservations では顧客の皆様に、次のように簡単で柔軟にご利用いただけます。</span><span class="sxs-lookup"><span data-stu-id="cf07c-118">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="cf07c-119">1 ～ 3 年の予約期間。</span><span class="sxs-lookup"><span data-stu-id="cf07c-119">One or three-year reservation terms</span></span>
- <span data-ttu-id="cf07c-120">簡単に使い始めることができます。セットアップは数秒で完了します。</span><span class="sxs-lookup"><span data-stu-id="cf07c-120">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="cf07c-121">予約インスタンスはいつでも取り消しまたは交換でき、払い戻しが調整されます。</span><span class="sxs-lookup"><span data-stu-id="cf07c-121">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="cf07c-122">組織レベルまたは個々の部署レベルで予約インスタンスの使用状況を管理できます。</span><span class="sxs-lookup"><span data-stu-id="cf07c-122">Manage reserved instances usage at the organizational or individual department level</span></span> 

<span data-ttu-id="cf07c-123">Azure Reservations は、次の点で顧客にとって魅力的です。</span><span class="sxs-lookup"><span data-stu-id="cf07c-123">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="cf07c-124">予約では、従量課金制 (PAYG) の価格設定で大幅にコストを節約できます。</span><span class="sxs-lookup"><span data-stu-id="cf07c-124">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="cf07c-125">1 年間または 3 年間の前払いにより、予算編成と支払い計画が容易になります。</span><span class="sxs-lookup"><span data-stu-id="cf07c-125">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="cf07c-126">オフィスに近い Azure リージョンでコンピューティング処理能力を優先させることができます。</span><span class="sxs-lookup"><span data-stu-id="cf07c-126">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="cf07c-127">Azure Reservations を Microsoft Windows Server や Azure SQL Database などのソフトウェアと組み合わせることで、エンドツーエンドのインフラストラクチャ ソリューション基盤が提供されます。</span><span class="sxs-lookup"><span data-stu-id="cf07c-127">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="cf07c-128">Azure Reservations は、パートナー センター、Azure portal、およびパートナー センター API を使用して購入、販売、管理できます。</span><span class="sxs-lookup"><span data-stu-id="cf07c-128">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="cf07c-129">購入した Azure サブスクリプションから独自の Azure 予約を購入するためのアクセス許可を顧客に付与することもできます。</span><span class="sxs-lookup"><span data-stu-id="cf07c-129">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="cf07c-130">方法については、各リンク先をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="cf07c-130">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="cf07c-131">Azure Reservations に関するリソース</span><span class="sxs-lookup"><span data-stu-id="cf07c-131">Azure reservations resources</span></span>

|<span data-ttu-id="cf07c-132">**対象**</span><span class="sxs-lookup"><span data-stu-id="cf07c-132">**For information about**</span></span>   |<span data-ttu-id="cf07c-133">**参照先**</span><span class="sxs-lookup"><span data-stu-id="cf07c-133">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="cf07c-134">顧客向けの Azure Reservations に関するドキュメント</span><span class="sxs-lookup"><span data-stu-id="cf07c-134">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="cf07c-135">Azure の予約とは</span><span class="sxs-lookup"><span data-stu-id="cf07c-135">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="cf07c-136">パートナー センターで顧客の Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="cf07c-136">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="cf07c-137">Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="cf07c-137">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="cf07c-138">パートナー センターでの Azure Reservations の管理</span><span class="sxs-lookup"><span data-stu-id="cf07c-138">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="cf07c-139">パートナー センターでの Azure Reservations の管理</span><span class="sxs-lookup"><span data-stu-id="cf07c-139">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="cf07c-140">適切な VM サイズの判断と顧客による VM 使用状況の確認</span><span class="sxs-lookup"><span data-stu-id="cf07c-140">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="cf07c-141">Azure Reservation の最大使用量に対応する VM サイズ</span><span class="sxs-lookup"><span data-stu-id="cf07c-141">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="cf07c-142">パートナー センター API を使用して Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="cf07c-142">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="cf07c-143">[Azure Reserved VM Instances の購入](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) (パートナー センター開発者向けドキュメント)</span><span class="sxs-lookup"><span data-stu-id="cf07c-143">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="cf07c-144">CSP サブスクリプションから独自の Azure 予約を購入するためのアクセス許可を顧客に付与します。</span><span class="sxs-lookup"><span data-stu-id="cf07c-144">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="cf07c-145">独自の Azure 予約を購入するためのアクセス許可を顧客に付与する</span><span class="sxs-lookup"><span data-stu-id="cf07c-145">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
