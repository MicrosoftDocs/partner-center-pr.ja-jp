---
title: Azure 予約 & サーバーサブスクリプション
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure の予約とサーバーサブスクリプションを取得、プロビジョニング、および管理するためのクラウドソリューションプロバイダーの機会について説明します。
author: rbars
ms.author: rbars
keywords: Azure, サブスクリプション, VM, 予約, 予約インスタンス
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dacab1c67a12be5143946c7ede33e647e1373cbb
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948267"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="ed1ea-104">Azure reserved VM instances (RI) と顧客向けのサーバーサブスクリプションの取得、プロビジョニング、& 管理</span><span class="sxs-lookup"><span data-stu-id="ed1ea-104">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="ed1ea-105">適用対象:</span><span class="sxs-lookup"><span data-stu-id="ed1ea-105">Applies to:</span></span>

- <span data-ttu-id="ed1ea-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="ed1ea-106">Partner Center</span></span>

<span data-ttu-id="ed1ea-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="ed1ea-107">**Appropriate roles**</span></span>

- <span data-ttu-id="ed1ea-108">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="ed1ea-108">Admin agent</span></span>
- <span data-ttu-id="ed1ea-109">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="ed1ea-109">Global admin</span></span>
- <span data-ttu-id="ed1ea-110">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="ed1ea-110">Helpdesk agent</span></span>
- <span data-ttu-id="ed1ea-111">販売代理店</span><span class="sxs-lookup"><span data-stu-id="ed1ea-111">Sales agent</span></span>
- <span data-ttu-id="ed1ea-112">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="ed1ea-112">User management admin</span></span>
 
## <a name="what-are-azure-reservations"></a><span data-ttu-id="ed1ea-113">Azure の予約とは</span><span class="sxs-lookup"><span data-stu-id="ed1ea-113">What are Azure Reservations?</span></span>

<span data-ttu-id="ed1ea-114">Azure Reservations では、1 年分または 3 年分の料金を前払いすることにより、仮想マシン、SQL Database の処理能力、Azure Cosmos DB スループット、その他の Azure リソースを割引価格で利用することができます。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-114">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="ed1ea-115">前払いすると、使用するリソースの割り引きを受けることができます。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-115">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="ed1ea-116">予約では、従量課金制の価格と比較して、仮想マシン、SQL Database の処理能力、Azure Cosmos DB、その他のリソースのコストを最大 72% も削減することができます。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-116">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="ed1ea-117">予約は課金割引を提供するもので、リソースの実行時の状態には影響しません。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-117">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="ed1ea-118">詳細について[は、「Azure Reservations とは](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-118">For more information see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="ed1ea-119">顧客が予約を購入する必要がある理由</span><span class="sxs-lookup"><span data-stu-id="ed1ea-119">Why should customers buy a reservation?</span></span>

<span data-ttu-id="ed1ea-120">顧客が長期間実行する仮想マシン、Azure Cosmos DB、または SQL データベースを使用している場合、予約の購入は最もコスト効率に優れたオプションです。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-120">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="ed1ea-121">たとえば、予約を使用しないでサービスの 4 つのインスタンスを連続的に実行している場合、従量課金制料金で課金されます。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-121">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="ed1ea-122">これらのリソースについて予約を購入した場合は、すぐに予約割引が適用されます。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-122">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="ed1ea-123">リソースには従量課金制の料金が適用されなくなります。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-123">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="ed1ea-124">CSP での魅力的な新しい Azure プラン</span><span class="sxs-lookup"><span data-stu-id="ed1ea-124">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="ed1ea-125">今日、予測が十分可能で永続的なクラウド ワークロードはコスト効率の高いソリューションでサポートしたいという需要が急速に高まっています。Azure Reservations とサーバー サブスクリプションが CSP プログラムに含まれることで、Microsoft のパートナーはこのような顧客の需要に対応できます。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-125">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="ed1ea-126">CSP プログラムを使用すると、パートナーは、Microsoft パートナーセンターと Azure portal を通じて、商用の顧客に代わって Azure Reservations とサーバーのサブスクリプションを取得、プロビジョニング、および管理できます。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-126">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="ed1ea-127">また、Azure の予約を購入する方法について、CSP プログラムの選択肢をパートナーに提供しています。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-127">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="ed1ea-128">CSP パートナーは[、お客様の代わりに azure の予約を購入](azure-reservations-buying.md)できます。また、お客様は、パートナーが購入した以前の azure サブスクリプションから[独自の予約を購入する](give-customers-permission.md)こともできます。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-128">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="ed1ea-129">Azure Reservations を利用すると、開発、テスト、アプリケーションの実行、データセンターの拡張を含む幅広いコンピューティング ソリューションに対して柔軟な仮想化を実現できます。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-129">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="ed1ea-130">たとえば[Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/)では、商用のお客様は、1年間または3年間の仮想マシンを購入または "予約" するだけで、最大72% と従量課金制の Azure VM 料金を節約できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-130">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="ed1ea-131">ソフトウェア アシュアランスに含まれている Azure ハイブリッド特典を利用できる Windows Server 顧客は、従量課金制の価格と比較して最大 80% を節約できます。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-131">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="ed1ea-132">訴求力のある価格設定と驚くべき展開柔軟性という無比の組み合わせで、Azure Reservations を選んだ顧客には、すべてにおいて最大の価値が提供されます。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-132">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="ed1ea-133">Azure の予約</span><span class="sxs-lookup"><span data-stu-id="ed1ea-133">Azure reservations</span></span>

- <span data-ttu-id="ed1ea-134">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="ed1ea-134">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="ed1ea-135">SQL DB 予約</span><span class="sxs-lookup"><span data-stu-id="ed1ea-135">SQL DB Reservations</span></span>
- <span data-ttu-id="ed1ea-136">SQL Managed Instance</span><span class="sxs-lookup"><span data-stu-id="ed1ea-136">SQL Managed Instance</span></span>
- <span data-ttu-id="ed1ea-137">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ed1ea-137">Azure Cosmos DB</span></span>
- <span data-ttu-id="ed1ea-138">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="ed1ea-138">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="ed1ea-139">アプリケーション サービス</span><span class="sxs-lookup"><span data-stu-id="ed1ea-139">App Services</span></span>
- <span data-ttu-id="ed1ea-140">Azure Databricks ユニットの予約</span><span class="sxs-lookup"><span data-stu-id="ed1ea-140">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="ed1ea-141">マネージド ディスク</span><span class="sxs-lookup"><span data-stu-id="ed1ea-141">Managed Disk</span></span>
- <span data-ttu-id="ed1ea-142">ブロック BLOB</span><span class="sxs-lookup"><span data-stu-id="ed1ea-142">Block blob</span></span>
- <span data-ttu-id="ed1ea-143">MySQL</span><span class="sxs-lookup"><span data-stu-id="ed1ea-143">MySQL</span></span>
- <span data-ttu-id="ed1ea-144">Azure データエクスプローラー</span><span class="sxs-lookup"><span data-stu-id="ed1ea-144">Azure Data explorer</span></span>
- <span data-ttu-id="ed1ea-145">MariaDB</span><span class="sxs-lookup"><span data-stu-id="ed1ea-145">MariaDB</span></span>
- <span data-ttu-id="ed1ea-146">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="ed1ea-146">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="ed1ea-147">サーバーサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="ed1ea-147">Server subscriptions</span></span>

- <span data-ttu-id="ed1ea-148">Windows Server</span><span class="sxs-lookup"><span data-stu-id="ed1ea-148">Windows Server</span></span>
- <span data-ttu-id="ed1ea-149">リモートデスクトップサービス (RDS) Cal</span><span class="sxs-lookup"><span data-stu-id="ed1ea-149">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="ed1ea-150">SQL Server</span><span class="sxs-lookup"><span data-stu-id="ed1ea-150">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="ed1ea-151">Linux ISV 年間サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="ed1ea-151">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="ed1ea-152">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="ed1ea-152">SUSE Linux</span></span>
- <span data-ttu-id="ed1ea-153">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="ed1ea-153">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="ed1ea-154">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="ed1ea-154">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="ed1ea-155">ISV 年間サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="ed1ea-155">ISV annual subscriptions</span></span>

- <span data-ttu-id="ed1ea-156">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="ed1ea-156">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="ed1ea-157">作業の開始</span><span class="sxs-lookup"><span data-stu-id="ed1ea-157">Getting started</span></span>

<span data-ttu-id="ed1ea-158">Azure Reservations を顧客と共に配置し、可能な限り迅速に運用を開始する方法を理解するために、次の方法で準備資料を確認することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-158">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="ed1ea-159">概要プレゼンテーションおよび関連するウェビナーで、顧客価値提案と位置付けを確認する</span><span class="sxs-lookup"><span data-stu-id="ed1ea-159">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="ed1ea-160">Modern Commerce Operating Guide を確認し、内容を理解する</span><span class="sxs-lookup"><span data-stu-id="ed1ea-160">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="ed1ea-161">Azure RI と Server Subscriptions のよく寄せられる質問を確認する</span><span class="sxs-lookup"><span data-stu-id="ed1ea-161">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="ed1ea-162">[パートナー センター API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) での Azure Reservations と Server Subscriptions に関する更新内容を理解する</span><span class="sxs-lookup"><span data-stu-id="ed1ea-162">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="ed1ea-163">リソース</span><span class="sxs-lookup"><span data-stu-id="ed1ea-163">Resources</span></span>

<span data-ttu-id="ed1ea-164">Azure Reservations パートナー センターで Azure Reservations の業務を早く開始するために役立つリソースを以下にまとめました。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-164">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="ed1ea-165">販売の準備</span><span class="sxs-lookup"><span data-stu-id="ed1ea-165">Sales readiness</span></span>

- [<span data-ttu-id="ed1ea-166">Azure ハイブリッド特典概要を使用した Azure Reservations およびサーバーサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="ed1ea-166">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="ed1ea-167">販売シート</span><span class="sxs-lookup"><span data-stu-id="ed1ea-167">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="ed1ea-168">Azure Reservations のパートナー FAQ</span><span class="sxs-lookup"><span data-stu-id="ed1ea-168">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="ed1ea-169">Azure Reservations と SQL DB に関するパートナー向け FAQ</span><span class="sxs-lookup"><span data-stu-id="ed1ea-169">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="ed1ea-170">リモートデスクトップサービス (RDS) クライアントアクセスライセンス (CAL) (アナウンス)</span><span class="sxs-lookup"><span data-stu-id="ed1ea-170">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="ed1ea-171">Azure Reserved VM Instances (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="ed1ea-171">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="ed1ea-172">サーバー サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="ed1ea-172">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)
- [<span data-ttu-id="ed1ea-173">Azure の SQL DB の概要</span><span class="sxs-lookup"><span data-stu-id="ed1ea-173">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="ed1ea-174">SQL DB の予約 (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="ed1ea-174">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="ed1ea-175">Azure Cosmos DB (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="ed1ea-175">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="ed1ea-176">SQL Managed Instance (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="ed1ea-176">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="ed1ea-177">SUSE および Red Hat Enterprise Linux (Azure portal)</span><span class="sxs-lookup"><span data-stu-id="ed1ea-177">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="ed1ea-178">Azure 上の Red Hat Linux</span><span class="sxs-lookup"><span data-stu-id="ed1ea-178">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="ed1ea-179">Azure 上の SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="ed1ea-179">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="ed1ea-180">Azure での Linux</span><span class="sxs-lookup"><span data-stu-id="ed1ea-180">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="ed1ea-181">Azure の料金概要</span><span class="sxs-lookup"><span data-stu-id="ed1ea-181">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="ed1ea-182">Azure 料金計算ツール</span><span class="sxs-lookup"><span data-stu-id="ed1ea-182">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="ed1ea-183">Azure Databricks ユニットの予約</span><span class="sxs-lookup"><span data-stu-id="ed1ea-183">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="ed1ea-184">CSP の価格表: **Microsoft Azure 予約インスタンス**と**ソフトウェアサブスクリプション**の価格表は両方とも、パートナーセンターの価格[&](https://partner.microsoft.com/pcv/sales)のページに掲載されています。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-184">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="ed1ea-185">トレーニング</span><span class="sxs-lookup"><span data-stu-id="ed1ea-185">Training</span></span>

<span data-ttu-id="ed1ea-186">登録して、[商用ライセンス準備ウェビナー](https://commercial-licensing.eventbuilder.com/FY2019_ALL)およびオンデマンドイベントを表示します。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-186">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="ed1ea-187">ライセンス準備オンデマンドイベントには、次のようなトピックが含まれます。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-187">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="ed1ea-188">CSP オンラインサービス、CSP Azure、一般的なライセンス更新 (Azure を含む) (2018 年11月)</span><span class="sxs-lookup"><span data-stu-id="ed1ea-188">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="ed1ea-189">SQL DB の予約容量 & インスタンスサイズの柔軟性 (8 月2018日)</span><span class="sxs-lookup"><span data-stu-id="ed1ea-189">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="ed1ea-190">CSP のサーバーサブスクリプション (2018 年7月)</span><span class="sxs-lookup"><span data-stu-id="ed1ea-190">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="ed1ea-191">CSP での Azure Reservations の概要 (2018 年5月)</span><span class="sxs-lookup"><span data-stu-id="ed1ea-191">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="ed1ea-192">その他の便利なトレーニングには、[パートナー大学の Azure ライセンスモジュール](https://aka.ms/azure_partner_licensing)が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-192">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="ed1ea-193">Operations</span><span class="sxs-lookup"><span data-stu-id="ed1ea-193">Operations</span></span>

- <span data-ttu-id="ed1ea-194">[最新のコマース運用ガイド](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx)(更新済み): 契約書、パートナーセンターからの注文、請求書、価格表の詳細、インセンティブ、調整ファイル、API/SDK、サンドボックス、Azure Partner Shared Services などの主要なポリシーと運用面を網羅した包括的なガイドです。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-194">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="ed1ea-195">モダン オファーの提供国と顧客の通貨の対応表</span><span class="sxs-lookup"><span data-stu-id="ed1ea-195">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="ed1ea-196">Microsoft Azure Reserved Instances の販売</span><span class="sxs-lookup"><span data-stu-id="ed1ea-196">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="ed1ea-197">顧客に代わって Microsoft Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="ed1ea-197">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="ed1ea-198">顧客に代わって Azure Reservations を管理する</span><span class="sxs-lookup"><span data-stu-id="ed1ea-198">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="ed1ea-199">Azure Reservations の請求</span><span class="sxs-lookup"><span data-stu-id="ed1ea-199">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="ed1ea-200">最大限の予約使用に備えた VM サイズ</span><span class="sxs-lookup"><span data-stu-id="ed1ea-200">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="ed1ea-201">パートナー センター API (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="ed1ea-201">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="ed1ea-202">リモート デスクトップ サービス</span><span class="sxs-lookup"><span data-stu-id="ed1ea-202">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="ed1ea-203">Azure ハイブリッド特典</span><span class="sxs-lookup"><span data-stu-id="ed1ea-203">Azure Hybrid Benefit</span></span>

<span data-ttu-id="ed1ea-204">[Azure ハイブリッド特典](https://azure.microsoft.com/pricing/hybrid-benefit)を利用すると、Windows Server ライセンスから得られる価値を拡大し、仮想マシンのコストを最大で \*47% 節約できます。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-204">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="ed1ea-205">この特典はソフトウェア アシュアランスに含まれており、Windows Server Datacenter および Standard エディションのライセンスで利用できます。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-205">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="ed1ea-206">エディションによっては、ライセンスを変換または再利用して、Azure で Windows Server 仮想マシンを実行し、基本コンピューティング料金 (Linux 仮想マシンの料金) を下げることができます。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-206">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="ed1ea-207">関連項目: [Azure ハイブリッド特典についてよく寄せられる質問](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="ed1ea-207">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="ed1ea-208">\* 割引による実際の効果は、リージョン、インスタンスの種類、使用率によって異なります。</span><span class="sxs-lookup"><span data-stu-id="ed1ea-208">\*Actual savings may vary based on region, instance type, or usage.</span></span>
