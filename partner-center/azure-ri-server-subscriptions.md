---
title: Azure 予約 & サーバーサブスクリプション
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure の予約とサーバーサブスクリプションを取得、プロビジョニング、および管理するためのクラウドソリューションプロバイダーの機会について説明します。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d5386dd4b2b19e641cc9d731d4a3d0f44ab5ad6
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182496"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="f7533-103">Azure reserved VM instances (RI) と顧客向けのサーバーサブスクリプションの取得、プロビジョニング、& 管理</span><span class="sxs-lookup"><span data-stu-id="f7533-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>


<span data-ttu-id="f7533-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="f7533-104">**Appropriate roles**</span></span>

- <span data-ttu-id="f7533-105">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="f7533-105">Admin agent</span></span>
- <span data-ttu-id="f7533-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="f7533-106">Global admin</span></span>
- <span data-ttu-id="f7533-107">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="f7533-107">Helpdesk agent</span></span>
- <span data-ttu-id="f7533-108">販売代理店</span><span class="sxs-lookup"><span data-stu-id="f7533-108">Sales agent</span></span>
- <span data-ttu-id="f7533-109">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="f7533-109">User management admin</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="f7533-110">Azure の予約とは</span><span class="sxs-lookup"><span data-stu-id="f7533-110">What are Azure Reservations?</span></span>

<span data-ttu-id="f7533-111">Azure Reservations では、1 年分または 3 年分の料金を前払いすることにより、仮想マシン、SQL Database の処理能力、Azure Cosmos DB スループット、その他の Azure リソースを割引価格で利用することができます。</span><span class="sxs-lookup"><span data-stu-id="f7533-111">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="f7533-112">前払いすると、使用するリソースの割り引きを受けることができます。</span><span class="sxs-lookup"><span data-stu-id="f7533-112">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="f7533-113">予約では、従量課金制の価格と比較して、仮想マシン、SQL Database の処理能力、Azure Cosmos DB、その他のリソースのコストを最大 72% も削減することができます。</span><span class="sxs-lookup"><span data-stu-id="f7533-113">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="f7533-114">予約は課金割引を提供するもので、リソースの実行時の状態には影響しません。</span><span class="sxs-lookup"><span data-stu-id="f7533-114">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="f7533-115">詳細について[は、「Azure Reservations とは](/azure/billing/billing-save-compute-costs-reservations)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f7533-115">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="f7533-116">顧客が予約を購入する必要がある理由</span><span class="sxs-lookup"><span data-stu-id="f7533-116">Why should customers buy a reservation?</span></span>

<span data-ttu-id="f7533-117">顧客が長期間実行する仮想マシン、Azure Cosmos DB、または SQL データベースを使用している場合、予約の購入は最もコスト効率に優れたオプションです。</span><span class="sxs-lookup"><span data-stu-id="f7533-117">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="f7533-118">たとえば、予約を使用しないでサービスの 4 つのインスタンスを連続的に実行している場合、従量課金制料金で課金されます。</span><span class="sxs-lookup"><span data-stu-id="f7533-118">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="f7533-119">これらのリソースについて予約を購入した場合は、すぐに予約割引が適用されます。</span><span class="sxs-lookup"><span data-stu-id="f7533-119">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="f7533-120">リソースには従量課金制の料金が適用されなくなります。</span><span class="sxs-lookup"><span data-stu-id="f7533-120">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="f7533-121">CSP での魅力的な新しい Azure プラン</span><span class="sxs-lookup"><span data-stu-id="f7533-121">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="f7533-122">今日、予測が十分可能で永続的なクラウド ワークロードはコスト効率の高いソリューションでサポートしたいという需要が急速に高まっています。Azure Reservations とサーバー サブスクリプションが CSP プログラムに含まれることで、Microsoft のパートナーはこのような顧客の需要に対応できます。</span><span class="sxs-lookup"><span data-stu-id="f7533-122">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="f7533-123">CSP プログラムを使用すると、パートナーは、Microsoft パートナーセンターと Azure portal を通じて、商用の顧客に代わって Azure Reservations とサーバーのサブスクリプションを取得、プロビジョニング、および管理できます。</span><span class="sxs-lookup"><span data-stu-id="f7533-123">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>
<span data-ttu-id="f7533-124">また、Azure の予約を購入する方法について、CSP プログラムの選択肢をパートナーに提供しています。</span><span class="sxs-lookup"><span data-stu-id="f7533-124">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="f7533-125">CSP パートナーは [、お客様の代わりに azure の予約を購入](azure-reservations-buying.md) できます。また、お客様は、パートナーが購入した以前の azure サブスクリプションから [独自の予約を購入する](give-customers-permission.md) こともできます。</span><span class="sxs-lookup"><span data-stu-id="f7533-125">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="f7533-126">Azure Reservations を利用すると、開発、テスト、アプリケーションの実行、データセンターの拡張を含む幅広いコンピューティング ソリューションに対して柔軟な仮想化を実現できます。</span><span class="sxs-lookup"><span data-stu-id="f7533-126">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="f7533-127">たとえば [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) では、商用のお客様は、1年間または3年間の仮想マシンを購入または "予約" するだけで、最大72% と従量課金制の Azure VM 料金を節約できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="f7533-127">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="f7533-128">ソフトウェア アシュアランスに含まれている Azure ハイブリッド特典を利用できる Windows Server 顧客は、従量課金制の価格と比較して最大 80% を節約できます。</span><span class="sxs-lookup"><span data-stu-id="f7533-128">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="f7533-129">説得力のある価格と比類のない展開の柔軟性の組み合わせにより、お客様は Azure Reservations を選択すると、全体的な価値が最も高くなります。</span><span class="sxs-lookup"><span data-stu-id="f7533-129">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations.</span></span>

- <span data-ttu-id="f7533-130">Azure Portal での [購入予約](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f7533-130">See [Purchase Reservations](/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) on the Azure Portal.</span></span>

- <span data-ttu-id="f7533-131">ソフトウェアサブスクリプションと Linux ISV の年間サブスクリプションについては、パートナーセンターの [価格とプラン](https://partner.microsoft.com/dashboard/sell/pricingandoffers)に関するページの **Microsoft Azure 予約済みインスタンス**] カテゴリの下にある **Azure RI CSP の商用価格表** を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f7533-131">See the **Azure RI CSP Commercial Price List** under the **Microsoft Azure Reserved Instances** category on the [Pricing and Offers](https://partner.microsoft.com/dashboard/sell/pricingandoffers) page in Partner Center for software subscriptions and Linux ISV annual subscriptions.</span></span>


 
<span data-ttu-id="f7533-132">**Linux ISV 年間サブスクリプション**</span><span class="sxs-lookup"><span data-stu-id="f7533-132">**Linux ISV annual subscriptions**</span></span>

- <span data-ttu-id="f7533-133">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="f7533-133">SUSE Linux</span></span>
- <span data-ttu-id="f7533-134">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="f7533-134">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="f7533-135">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="f7533-135">Azure Red Hat OpenShift</span></span>

<span data-ttu-id="f7533-136">**ISV 年間サブスクリプション**</span><span class="sxs-lookup"><span data-stu-id="f7533-136">**ISV annual subscriptions**</span></span>

- <span data-ttu-id="f7533-137">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="f7533-137">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="f7533-138">作業の開始</span><span class="sxs-lookup"><span data-stu-id="f7533-138">Getting started</span></span>

<span data-ttu-id="f7533-139">Azure Reservations を顧客と共に配置し、可能な限り迅速に運用を開始する方法を理解するために、次の方法で準備資料を確認することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="f7533-139">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="f7533-140">[パートナーセンターの新しいコマース運用ガイド](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)を確認し、理解します。</span><span class="sxs-lookup"><span data-stu-id="f7533-140">Review and understand the [Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span></span>

2. <span data-ttu-id="f7533-141">[パートナーセンター api (api/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)での Azure Reservations とサーバーサブスクリプションの更新について説明します。</span><span class="sxs-lookup"><span data-stu-id="f7533-141">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances).</span></span>


### <a name="sales-readiness"></a><span data-ttu-id="f7533-142">販売の準備</span><span class="sxs-lookup"><span data-stu-id="f7533-142">Sales readiness</span></span>

- [<span data-ttu-id="f7533-143">リモートデスクトップサービス (RDS) クライアントアクセスライセンス (CAL) (アナウンス)</span><span class="sxs-lookup"><span data-stu-id="f7533-143">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [<span data-ttu-id="f7533-144">Azure Reserved VM Instances (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="f7533-144">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [<span data-ttu-id="f7533-145">サーバー サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="f7533-145">Server Subscriptions</span></span>](./csp-software-subscriptions.md)

- [<span data-ttu-id="f7533-146">SQL DB の予約 (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="f7533-146">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)

- [<span data-ttu-id="f7533-147">Azure Cosmos DB (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="f7533-147">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)

- [<span data-ttu-id="f7533-148">SQL Managed Instance (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="f7533-148">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)

- [<span data-ttu-id="f7533-149">SUSE および Red Hat Enterprise Linux (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="f7533-149">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)

- [<span data-ttu-id="f7533-150">Azure 上の Red Hat Linux</span><span class="sxs-lookup"><span data-stu-id="f7533-150">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)

- [<span data-ttu-id="f7533-151">Azure 上の SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="f7533-151">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [<span data-ttu-id="f7533-152">Linux on Azure</span><span class="sxs-lookup"><span data-stu-id="f7533-152">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)

- [<span data-ttu-id="f7533-153">Azure の料金概要</span><span class="sxs-lookup"><span data-stu-id="f7533-153">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)

- [<span data-ttu-id="f7533-154">Azure 料金計算ツール</span><span class="sxs-lookup"><span data-stu-id="f7533-154">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)

- [<span data-ttu-id="f7533-155">Azure Databricks ユニットの予約</span><span class="sxs-lookup"><span data-stu-id="f7533-155">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a><span data-ttu-id="f7533-156">トレーニング</span><span class="sxs-lookup"><span data-stu-id="f7533-156">Training</span></span>

<span data-ttu-id="f7533-157">登録して、 [商用ライセンス準備ウェビナー](https://commercial-licensing.eventbuilder.com/FY2019_ALL) およびオンデマンドイベントを表示します。</span><span class="sxs-lookup"><span data-stu-id="f7533-157">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>
<span data-ttu-id="f7533-158">以前に記録されたライセンス準備オンデマンドイベントには、次のようなトピックが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f7533-158">Previously recorded Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="f7533-159">CSP オンラインサービス、CSP Azure、一般的なライセンス更新 (Azure を含む) (2018 年11月)</span><span class="sxs-lookup"><span data-stu-id="f7533-159">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>

- <span data-ttu-id="f7533-160">SQL DB の予約容量 & インスタンスサイズの柔軟性 (8 月2018日)</span><span class="sxs-lookup"><span data-stu-id="f7533-160">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>

- <span data-ttu-id="f7533-161">CSP のサーバーサブスクリプション (2018 年7月)</span><span class="sxs-lookup"><span data-stu-id="f7533-161">Server Subscriptions in CSP (July 2018)</span></span>

- <span data-ttu-id="f7533-162">CSP での Azure Reservations の概要 (2018 年5月)</span><span class="sxs-lookup"><span data-stu-id="f7533-162">Azure Reservations Overview in CSP (May 2018)</span></span>

## <a name="operations"></a><span data-ttu-id="f7533-163">操作</span><span class="sxs-lookup"><span data-stu-id="f7533-163">Operations</span></span>

<span data-ttu-id="f7533-164">[パートナーセンターの新しいコマース運用ガイド](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf): 主要なポリシーと運用面 (契約、パートナーセンターからの注文、請求書、価格表の詳細、インセンティブ、調整ファイル、API/SDK、サンドボックス、Azure Partner Shared Services など) に関する包括的なガイドです。</span><span class="sxs-lookup"><span data-stu-id="f7533-164">[Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf):  Comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="f7533-165">Azure ハイブリッド特典</span><span class="sxs-lookup"><span data-stu-id="f7533-165">Azure Hybrid Benefit</span></span>

<span data-ttu-id="f7533-166">[Azure ハイブリッド特典](https://azure.microsoft.com/pricing/hybrid-benefit)は、ソフトウェアアシュアランス付きのライセンスを所有しているお客様にとっての価格特典です。これにより、既存のオンプレミスの Windows Server の価値を最大化したり、Azure への移行時にライセンスへの SQL Server を適用したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="f7533-166">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) is a pricing benefit for customers who have licenses with Software Assurance, which helps maximize the value of existing on-premises Windows Server and/or SQL Server license investments when migrating to Azure.</span></span> <span data-ttu-id="f7533-167">対象と80なるお客様は、Azure Virtual Machines (infrastructure as a service (IaaS)) で最大 40% \* を節約し、Azure SQL Database (プラットフォームとしてのプラットフォーム、または PaaS) に対して最大55% の節約を可能にし、Azure ハイブリッド特典を使用して Azure Virtual Machines (IaaS) に SQL Server します</span><span class="sxs-lookup"><span data-stu-id="f7533-167">Eligible customers can save up to 40%\* on Azure Virtual Machines (infrastructure as a service, or IaaS), and save up to 55% on Azure SQL Database (platform as a service, or PaaS) and SQL Server on Azure Virtual Machines (IaaS) with Azure Hybrid Benefit, which increases to up to 80% when combined with Azure Reserved Instances.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f7533-168">次のステップ</span><span class="sxs-lookup"><span data-stu-id="f7533-168">Next steps</span></span>

- [<span data-ttu-id="f7533-169">Azure ハイブリッド特典のよくあるご質問</span><span class="sxs-lookup"><span data-stu-id="f7533-169">Azure Hybrid Benefit FAQ</span></span>](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

<span data-ttu-id="f7533-170">\* 割引による実際の効果は、リージョン、インスタンスの種類、使用率によって異なります。</span><span class="sxs-lookup"><span data-stu-id="f7533-170">\*Actual savings may vary based on region, instance type, or usage.</span></span>