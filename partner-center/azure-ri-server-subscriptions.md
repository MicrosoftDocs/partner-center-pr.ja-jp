---
title: Azure Reserved VM Instances (RI) + Server Subscriptions for Azure | パートナー センター
ms.topic: article
ms.date: 12/02/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: クラウドソリューションプロバイダーが顧客の Azure の予約とサーバーサブスクリプションを取得、プロビジョニング、および管理する機会について説明します。
author: LauraBrenner
ms.author: labrenne
keywords: Azure, サブスクリプション, VM, 予約, 予約インスタンス
ms.localizationpriority: medium
ms.openlocfilehash: 22ba6af523bf73d9d7778940ef7495e6581a0730
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722254"
---
<!-- Mike Aasen wrote and owns this topic -->

# <a name="azure-reserved-vm-instances-ri--server-subscriptions-for-azure"></a><span data-ttu-id="c0d68-104">Azure Reserved VM Instances (RI) + Server Subscriptions for Azure</span><span class="sxs-lookup"><span data-stu-id="c0d68-104">Azure reserved VM instances (RI) + server subscriptions for Azure</span></span>

<span data-ttu-id="c0d68-105">適用対象:</span><span class="sxs-lookup"><span data-stu-id="c0d68-105">Applies to:</span></span>

- <span data-ttu-id="c0d68-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="c0d68-106">Partner Center</span></span>

<span data-ttu-id="c0d68-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="c0d68-107">**Appropriate roles**</span></span>

- <span data-ttu-id="c0d68-108">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="c0d68-108">Admin agent</span></span>
- <span data-ttu-id="c0d68-109">グローバル管理</span><span class="sxs-lookup"><span data-stu-id="c0d68-109">Global admin</span></span>
- <span data-ttu-id="c0d68-110">ヘルプデスク エージェント</span><span class="sxs-lookup"><span data-stu-id="c0d68-110">Helpdesk agent</span></span>
- <span data-ttu-id="c0d68-111">販売代理店</span><span class="sxs-lookup"><span data-stu-id="c0d68-111">Sales agent</span></span>
- <span data-ttu-id="c0d68-112">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="c0d68-112">User management admin</span></span>
 
## <a name="what-are-azure-reservations"></a><span data-ttu-id="c0d68-113">Azure Reservations とは</span><span class="sxs-lookup"><span data-stu-id="c0d68-113">What are Azure Reservations?</span></span>

<span data-ttu-id="c0d68-114">Azure Reservations では、1 年分または 3 年分の料金を前払いすることにより、仮想マシン、SQL Database の処理能力、Azure Cosmos DB スループット、その他の Azure リソースを割引価格で利用することができます。</span><span class="sxs-lookup"><span data-stu-id="c0d68-114">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="c0d68-115">前払いの場合は、使用するリソースに割引価格で適用されます。</span><span class="sxs-lookup"><span data-stu-id="c0d68-115">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="c0d68-116">予約では、従量課金制の価格と比較して、仮想マシン、SQL Database の処理能力、Azure Cosmos DB、その他のリソースのコストを最大 72% も削減することができます。</span><span class="sxs-lookup"><span data-stu-id="c0d68-116">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="c0d68-117">Reservations では請求の割引が提供され、リソースの実行時の状態には影響しません。詳しくは、「[Azure の予約とは](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="c0d68-117">Reservations provide a billing discount and don't affect the runtime state of your resources.For more information see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="c0d68-118">顧客が予約を購入する必要がある理由</span><span class="sxs-lookup"><span data-stu-id="c0d68-118">Why should customers buy a reservation?</span></span>

<span data-ttu-id="c0d68-119">顧客が長期間実行する仮想マシン、Azure Cosmos DB、または SQL データベースを使用している場合、予約の購入は最もコスト効率に優れたオプションです。</span><span class="sxs-lookup"><span data-stu-id="c0d68-119">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="c0d68-120">たとえば、予約を使用しないでサービスの 4 つのインスタンスを連続的に実行している場合、従量課金制料金で課金されます。</span><span class="sxs-lookup"><span data-stu-id="c0d68-120">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="c0d68-121">これらのリソースについて予約を購入した場合は、すぐに予約割引が適用されます。</span><span class="sxs-lookup"><span data-stu-id="c0d68-121">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="c0d68-122">リソースは、従量課金制料金では課金されなくなります。</span><span class="sxs-lookup"><span data-stu-id="c0d68-122">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="c0d68-123">CSP での魅力的な新しい Azure プラン</span><span class="sxs-lookup"><span data-stu-id="c0d68-123">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="c0d68-124">今日、予測が十分可能で永続的なクラウド ワークロードはコスト効率の高いソリューションでサポートしたいという需要が急速に高まっています。Azure Reservations とサーバー サブスクリプションが CSP プログラムに含まれることで、Microsoft のパートナーはこのような顧客の需要に対応できます。</span><span class="sxs-lookup"><span data-stu-id="c0d68-124">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="c0d68-125">CSP プログラムでは、パートナーが企業顧客に代わり、Microsoft パートナー センターと Azure portal を通じて Azure Reservations とサーバー サブスクリプションの取得、プロビジョニング、管理を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="c0d68-125">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure Portal.</span></span>

<span data-ttu-id="c0d68-126">Azure Reservations を利用すると、開発、テスト、アプリケーションの実行、データセンターの拡張を含む幅広いコンピューティング ソリューションに対して柔軟な仮想化を実現できます。</span><span class="sxs-lookup"><span data-stu-id="c0d68-126">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="c0d68-127">たとえば[Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/)では、商用のお客様は、1年間または3年間の仮想マシンを購入または "予約" するだけで、最大72% と従量課金制の Azure VM 料金を節約できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="c0d68-127">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or “reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="c0d68-128">ソフトウェア アシュアランスに含まれている Azure ハイブリッド特典を利用できる Windows Server 顧客は、従量課金制の価格と比較して最大 80% を節約できます。</span><span class="sxs-lookup"><span data-stu-id="c0d68-128">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="c0d68-129">訴求力のある価格設定と驚くべき展開柔軟性という無比の組み合わせで、Azure Reservations を選んだ顧客には、すべてにおいて最大の価値が提供されます。</span><span class="sxs-lookup"><span data-stu-id="c0d68-129">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="c0d68-130">Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="c0d68-130">Azure reservations</span></span>

- <span data-ttu-id="c0d68-131">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="c0d68-131">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="c0d68-132">SQL DB の予約</span><span class="sxs-lookup"><span data-stu-id="c0d68-132">SQL DB Reservations</span></span>
- <span data-ttu-id="c0d68-133">SQL Managed Instance</span><span class="sxs-lookup"><span data-stu-id="c0d68-133">SQL Managed Instance</span></span>
- <span data-ttu-id="c0d68-134">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="c0d68-134">Azure Cosmos DB</span></span>
- <span data-ttu-id="c0d68-135">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="c0d68-135">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="c0d68-136">App Services</span><span class="sxs-lookup"><span data-stu-id="c0d68-136">App Services</span></span>
- <span data-ttu-id="c0d68-137">Azure Databricks ユニットの予約</span><span class="sxs-lookup"><span data-stu-id="c0d68-137">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="c0d68-138">管理ディスク</span><span class="sxs-lookup"><span data-stu-id="c0d68-138">Managed Disk</span></span>
- <span data-ttu-id="c0d68-139">Blockblob</span><span class="sxs-lookup"><span data-stu-id="c0d68-139">Blockblob</span></span>
- <span data-ttu-id="c0d68-140">MySQL</span><span class="sxs-lookup"><span data-stu-id="c0d68-140">MySQL</span></span>
- <span data-ttu-id="c0d68-141">Azure データエクスプローラー</span><span class="sxs-lookup"><span data-stu-id="c0d68-141">Azure Data explorer</span></span>
- <span data-ttu-id="c0d68-142">MariaDB</span><span class="sxs-lookup"><span data-stu-id="c0d68-142">MariaDB</span></span>
- <span data-ttu-id="c0d68-143">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="c0d68-143">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="c0d68-144">サーバー サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="c0d68-144">Server subscriptions</span></span>

- <span data-ttu-id="c0d68-145">Windows Server</span><span class="sxs-lookup"><span data-stu-id="c0d68-145">Windows Server</span></span>
- <span data-ttu-id="c0d68-146">リモートデスクトップサービス (RDS) Cal</span><span class="sxs-lookup"><span data-stu-id="c0d68-146">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="c0d68-147">SQL Server</span><span class="sxs-lookup"><span data-stu-id="c0d68-147">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="c0d68-148">Linux ISV 年間サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="c0d68-148">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="c0d68-149">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="c0d68-149">SUSE Linux</span></span>
- <span data-ttu-id="c0d68-150">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="c0d68-150">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="c0d68-151">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="c0d68-151">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="c0d68-152">ISV 年間サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="c0d68-152">ISV annual subscriptions</span></span>

- <span data-ttu-id="c0d68-153">CloudSimple での Azure VMware ソリューション</span><span class="sxs-lookup"><span data-stu-id="c0d68-153">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="c0d68-154">開始するには</span><span class="sxs-lookup"><span data-stu-id="c0d68-154">Getting started</span></span>

<span data-ttu-id="c0d68-155">顧客に対する Azure Reservations の位置付けを理解し、できる限り早く営業活動を開始するには、次に示すアプローチで準備資料を確認することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="c0d68-155">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible we recommend the following approach for reviewing the readiness materials:</span></span>

1. <span data-ttu-id="c0d68-156">概要プレゼンテーションおよび関連するウェビナーで、顧客価値提案と位置付けを確認する</span><span class="sxs-lookup"><span data-stu-id="c0d68-156">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="c0d68-157">Modern Commerce Operating Guide を確認し、内容を理解する</span><span class="sxs-lookup"><span data-stu-id="c0d68-157">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="c0d68-158">Azure RI と Server Subscriptions のよく寄せられる質問を確認する</span><span class="sxs-lookup"><span data-stu-id="c0d68-158">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="c0d68-159">[パートナー センター API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) での Azure Reservations と Server Subscriptions に関する更新内容を理解する</span><span class="sxs-lookup"><span data-stu-id="c0d68-159">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="c0d68-160">参考資料</span><span class="sxs-lookup"><span data-stu-id="c0d68-160">Resources</span></span>

<span data-ttu-id="c0d68-161">Azure Reservations パートナー センターで Azure Reservations の業務を早く開始するために役立つリソースを以下にまとめました。</span><span class="sxs-lookup"><span data-stu-id="c0d68-161">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="c0d68-162">販売準備</span><span class="sxs-lookup"><span data-stu-id="c0d68-162">Sales readiness</span></span>

- [<span data-ttu-id="c0d68-163">Azure ハイブリッド特典概要を使用した Azure Reservations およびサーバーサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="c0d68-163">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="c0d68-164">販売シート</span><span class="sxs-lookup"><span data-stu-id="c0d68-164">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="c0d68-165">Azure Reservations のパートナー FAQ</span><span class="sxs-lookup"><span data-stu-id="c0d68-165">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="c0d68-166">Azure Reservations と SQL DB に関するパートナー向け FAQ</span><span class="sxs-lookup"><span data-stu-id="c0d68-166">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="c0d68-167">リモートデスクトップサービス (RDS) Cal (アナウンス)</span><span class="sxs-lookup"><span data-stu-id="c0d68-167">Remote Desktop Services (RDS) CALs (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="c0d68-168">Azure Reserved VM Instances (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="c0d68-168">Azure Reserved VM Instances (Azure Portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="c0d68-169">サーバー サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="c0d68-169">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)
- [<span data-ttu-id="c0d68-170">Azure の SQL DB の概要</span><span class="sxs-lookup"><span data-stu-id="c0d68-170">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="c0d68-171">SQL DB の予約 (Azure ポータル)</span><span class="sxs-lookup"><span data-stu-id="c0d68-171">SQL DB Reservations (Azure Portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="c0d68-172">Azure Cosmos DB (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="c0d68-172">Azure Cosmos DB (Azure Portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="c0d68-173">SQL Managed Instance (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="c0d68-173">SQL Managed Instance (Azure Portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="c0d68-174">SUSE と Red Hat Enterprise Linux (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="c0d68-174">SUSE and Red Hat Enterprise Linux (Azure Portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="c0d68-175">Azure 上の Red Hat Linux</span><span class="sxs-lookup"><span data-stu-id="c0d68-175">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="c0d68-176">Azure 上の SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="c0d68-176">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="c0d68-177">Azure 上の Linux</span><span class="sxs-lookup"><span data-stu-id="c0d68-177">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="c0d68-178">Azure の料金概要</span><span class="sxs-lookup"><span data-stu-id="c0d68-178">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="c0d68-179">Azure 料金計算ツール</span><span class="sxs-lookup"><span data-stu-id="c0d68-179">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="c0d68-180">Azure Databricks ユニットの予約</span><span class="sxs-lookup"><span data-stu-id="c0d68-180">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="c0d68-181">CSP の価格表: **Microsoft Azure 予約インスタンス**と**ソフトウェアサブスクリプション**の価格表は両方とも、パートナーセンターの価格[&](https://partner.microsoft.com/pcv/sales)のページに掲載されています。</span><span class="sxs-lookup"><span data-stu-id="c0d68-181">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="c0d68-182">トレーニング</span><span class="sxs-lookup"><span data-stu-id="c0d68-182">Training</span></span>

- <span data-ttu-id="c0d68-183">CSP オンライン サービス、CSP Azure、および一般的なライセンス更新について説明されている [2018 年 11 月の商用ライセンス準備ウェビナー](https://na01.safelinks.protection.outlook.com/?url=https%3A%2F%2Fcommercial-licensing.eventbuilder.com%2F%3Flandingpageid%3DV0Bx6L&data=02%7C01%7Cv-oumaki%40microsoft.com%7C96e24687952242e1ff0c08d62ada13f3%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636743513471330495&sdata=DjPAKnW%2BpVekRS3Zngy2uwAkTpU4z1O%2Fh56NuTOmCzM%3D&reserved=0) (Azure を含む)</span><span class="sxs-lookup"><span data-stu-id="c0d68-183">[November 2018 Commercial Licensing Readiness Webinars](https://na01.safelinks.protection.outlook.com/?url=https%3A%2F%2Fcommercial-licensing.eventbuilder.com%2F%3Flandingpageid%3DV0Bx6L&data=02%7C01%7Cv-oumaki%40microsoft.com%7C96e24687952242e1ff0c08d62ada13f3%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636743513471330495&sdata=DjPAKnW%2BpVekRS3Zngy2uwAkTpU4z1O%2Fh56NuTOmCzM%3D&reserved=0) covering CSP Online Services, CSP Azure and a general licensing update (including Azure)</span></span>
- [<span data-ttu-id="c0d68-184">8 月の SQL DB の予約容量およびインスタンス サイズ柔軟性 - ライセンス ウェビナー</span><span class="sxs-lookup"><span data-stu-id="c0d68-184">August SQL DB Reserved Capacity & Instance Size Flexibility - Licensing Webinar</span></span>](https://commercial-licensing.eventbuilder.com/view?eventid=d0t9g4)
- [<span data-ttu-id="c0d68-185">2018 年 7 月の CSP でのサーバー サブスクリプション ウェビナー</span><span class="sxs-lookup"><span data-stu-id="c0d68-185">July 2018 Server Subscriptions in CSP Webinar</span></span>](https://commercial-licensing.eventbuilder.com/Server_Subscriptions_in_CSP_P2_July)
- [<span data-ttu-id="c0d68-186">2018 年 5 月の Azure Reservations 概要ウェビナー</span><span class="sxs-lookup"><span data-stu-id="c0d68-186">May 2018 Azure Reservations Overview Webinar</span></span>](https://commercial-licensing.eventbuilder.com/Reserved_Instances_in_CSP_May_Option_1)
- [<span data-ttu-id="c0d68-187">Azure ライセンス モジュール (Partner University)</span><span class="sxs-lookup"><span data-stu-id="c0d68-187">Azure Licensing Module on Partner University</span></span>](https://aka.ms/azure_partner_licensing)

### <a name="operations"></a><span data-ttu-id="c0d68-188">運用</span><span class="sxs-lookup"><span data-stu-id="c0d68-188">Operations</span></span>

- <span data-ttu-id="c0d68-189">[最新のコマース運用ガイド](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx)(更新): 契約書、パートナーセンターからの注文、請求書、価格表の詳細、インセンティブ、調整ファイル、API/SDK、サンドボックスなどの主要なポリシーと運用面を網羅した包括的なガイドです。Azure Partner Shared Services。</span><span class="sxs-lookup"><span data-stu-id="c0d68-189">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="c0d68-190">モダン オファーの提供国と顧客の通貨の対応表</span><span class="sxs-lookup"><span data-stu-id="c0d68-190">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="c0d68-191">Microsoft Azure Reserved Instances の販売</span><span class="sxs-lookup"><span data-stu-id="c0d68-191">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="c0d68-192">顧客に代わって Microsoft Azure Reservations を購入する</span><span class="sxs-lookup"><span data-stu-id="c0d68-192">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="c0d68-193">顧客に代わって Azure Reservations を管理する</span><span class="sxs-lookup"><span data-stu-id="c0d68-193">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="c0d68-194">Azure Reservations の請求</span><span class="sxs-lookup"><span data-stu-id="c0d68-194">Billing for Azure reservations</span></span>](https://go.microsoft.com/fwlink/?linkid=872809)
- [<span data-ttu-id="c0d68-195">最大限の予約使用に備えた VM サイズ</span><span class="sxs-lookup"><span data-stu-id="c0d68-195">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="c0d68-196">パートナー センター API (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="c0d68-196">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="c0d68-197">リモート デスクトップ サービス</span><span class="sxs-lookup"><span data-stu-id="c0d68-197">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="c0d68-198">Azure ハイブリッド特典</span><span class="sxs-lookup"><span data-stu-id="c0d68-198">Azure Hybrid Benefit</span></span>

<span data-ttu-id="c0d68-199">[Azure ハイブリッド特典](https://azure.microsoft.com/pricing/hybrid-benefit)を利用すると、Windows Server ライセンスから得られる価値を拡大し、仮想マシンのコストを最大で \*47% 節約できます。</span><span class="sxs-lookup"><span data-stu-id="c0d68-199">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="c0d68-200">この特典はソフトウェア アシュアランスに含まれており、Windows Server Datacenter および Standard エディションのライセンスで利用できます。</span><span class="sxs-lookup"><span data-stu-id="c0d68-200">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="c0d68-201">エディションによっては、ライセンスを変換または再利用して、低いベース コンピューティング レート (Linux 仮想マシン レート) で Windows Server 仮想マシンを Azure で実行できます。</span><span class="sxs-lookup"><span data-stu-id="c0d68-201">Depending on the edition, you can convert or re-use your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="c0d68-202">関連項目: [Azure ハイブリッド特典についてよく寄せられる質問](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="c0d68-202">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="c0d68-203">\* 割引による実際の効果は、リージョン、インスタンスの種類、使用率によって異なります。</span><span class="sxs-lookup"><span data-stu-id="c0d68-203">\*Actual savings may vary based on region, instance type, or usage.</span></span>
