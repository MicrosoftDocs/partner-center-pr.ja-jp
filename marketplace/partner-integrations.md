---
title: Azure Marketplace パートナー統合
description: Azure 環境Azure Marketplaceするソリューションについて説明し、Microsoft パートナーからのデプロイ ガイドへのリンクを取得します。
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: 56e72af367cdcb264cc444446c5fcbedcd880451
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276486"
---
# <a name="azure-marketplace-partner-integrations"></a><span data-ttu-id="22dbf-103">Azure Marketplace パートナー統合</span><span class="sxs-lookup"><span data-stu-id="22dbf-103">Azure Marketplace partner integrations</span></span>

<span data-ttu-id="22dbf-104">パートナー ソリューションを Azure 環境に統合する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="22dbf-104">Learn how to integrate partner solutions into your Azure environment.</span></span> <span data-ttu-id="22dbf-105">この記事では、各ソリューションの概要と、詳細なデプロイ ガイドへのリンクを示します。</span><span class="sxs-lookup"><span data-stu-id="22dbf-105">This article gives an overview of each solution and links to detailed deployment guides.</span></span> <span data-ttu-id="22dbf-106">ソリューションはアルファベット順に一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="22dbf-106">Solutions are listed in alphabetical order.</span></span> 

## <a name="apache-kafka-on-confluent-cloud"></a><span data-ttu-id="22dbf-107">Confluent Cloud での Apache Kafka</span><span class="sxs-lookup"><span data-stu-id="22dbf-107">Apache Kafka on Confluent Cloud</span></span>

![Confluent Cloud。](./media/partners/confluent-cloud.png)

<span data-ttu-id="22dbf-109">Azure では、クラウド アプリケーションに加えて Confluent Cloud と統合できます。</span><span class="sxs-lookup"><span data-stu-id="22dbf-109">Azure lets you integrate with Confluent Cloud in addition to your cloud applications.</span></span> <span data-ttu-id="22dbf-110">Confluent のお客様は、多くの場合、Azure portal Confluent Cloud 間を移動します。</span><span class="sxs-lookup"><span data-stu-id="22dbf-110">Confluent customers often navigate between the Azure portal and Confluent Cloud.</span></span> <span data-ttu-id="22dbf-111">たとえば、ユーザーが Azure Marketplace で Confluent Cloud オファーを購入すると、Confluent Cloud でアカウントを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="22dbf-111">For example, once a user purchases a Confluent Cloud offer in Azure Marketplace, they are then expected to set up an account with Confluent Cloud.</span></span> <span data-ttu-id="22dbf-112">このプロセスにより複雑性と時間が追加され、ユーザーは 2 つのポータル間で構成とリソースを管理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="22dbf-112">This process adds complexity and time, and requires users to manage configuration and resources between the two portals.</span></span> <span data-ttu-id="22dbf-113">プラットフォーム間での管理の負担を軽減するために、Microsoft は Confluent Cloud と連携して、Azure から Confluent Cloud への統合プロビジョニング レイヤーを構築しました。</span><span class="sxs-lookup"><span data-stu-id="22dbf-113">To reduce the burden of managing across platforms, Microsoft, in partnership with Confluent Cloud, built an integrated provisioning layer from Azure to Confluent Cloud.</span></span> <span data-ttu-id="22dbf-114">このソリューションは、Azure Azure Marketplaceで Confluent Cloud オファリングを使用するシームレスなエクスペリエンスを提供します</span><span class="sxs-lookup"><span data-stu-id="22dbf-114">The solution is available in Azure Marketplace and  provides a seamless experience for using the Confluent Cloud offering on Azure</span></span>

<span data-ttu-id="22dbf-115">このソリューションでは、Azure で有効になっているリソース プロバイダーを使用して Confluent Cloud リソースをプロビジョニングします。</span><span class="sxs-lookup"><span data-stu-id="22dbf-115">The solution uses a resource provider enabled in Azure to provision Confluent Cloud resources.</span></span> <span data-ttu-id="22dbf-116">これにより、ユーザーは、Azure portal、Azure CLI、および Azure SDK を介してリアルタイム のイベント ストリーミングにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="22dbf-116">This allows users to access real-time event streaming via the Azure portal, Azure CLI, and Azure SDKs.</span></span> <span data-ttu-id="22dbf-117">Confluent Cloud は、環境、クラスター、トピック、API キー、マネージド コネクタを含む SaaS アプリケーションを所有して実行します。</span><span class="sxs-lookup"><span data-stu-id="22dbf-117">Confluent Cloud owns and runs the SaaS application, which includes environments, clusters, topics, API keys, and managed connectors.</span></span>

<span data-ttu-id="22dbf-118">Confluent Cloud との深い統合により、次の機能が可能です。</span><span class="sxs-lookup"><span data-stu-id="22dbf-118">The deep integration with Confluent Cloud enables the following capabilities:</span></span>

- <span data-ttu-id="22dbf-119">フル マネージド インフラストラクチャにより、Azure portal から新しい Confluent Cloud の組織リソースをプロビジョニング。</span><span class="sxs-lookup"><span data-stu-id="22dbf-119">Provision a new Confluent Cloud organization resource from the Azure portal with fully managed infrastructure.</span></span>
- <span data-ttu-id="22dbf-120">Azure から Confluent Cloud へのシングル サインオンを Azure Active Directory。Confluent Cloud ポータルから個別の認証を行う必要はありません。</span><span class="sxs-lookup"><span data-stu-id="22dbf-120">Streamline single sign-on from Azure to Confluent Cloud with Azure Active Directory; no separate authentication needed from the Confluent Cloud portal.</span></span>
- <span data-ttu-id="22dbf-121">Azure サブスクリプションの請求を通じて、Confluent Cloud の消費料金の統合請求を取得します。</span><span class="sxs-lookup"><span data-stu-id="22dbf-121">Get unified billing of Confluent Cloud consumption charges through Azure subscription invoicing.</span></span>
- <span data-ttu-id="22dbf-122">サーバーから Confluent Cloud リソースを管理Azure portal、Azure リソースと共に [すべてのリソース] ページでそれらを追跡します。</span><span class="sxs-lookup"><span data-stu-id="22dbf-122">Manage Confluent Cloud resources from the Azure portal, and track them in the **All resources** page, alongside your Azure resources.</span></span>

[<span data-ttu-id="22dbf-123">Confluent クラウドデプロイ ガイド</span><span class="sxs-lookup"><span data-stu-id="22dbf-123">Confluent Cloud deployment guides</span></span>](https://docs.confluent.io/current/cloud/marketplace/index.html)

<span data-ttu-id="22dbf-124">Azure 上の Confluent に関連する問題については、 にアクセスしてください [https://support.confluent.io](https://support.confluent.io) 。</span><span class="sxs-lookup"><span data-stu-id="22dbf-124">For issues related to Confluent on Azure, go to [https://support.confluent.io](https://support.confluent.io).</span></span> <span data-ttu-id="22dbf-125">初めて使用する場合は、Confluent サポート ポータルにサインインする前にパスワードをリセットしてください。</span><span class="sxs-lookup"><span data-stu-id="22dbf-125">If you are a first time user, reset your password before you sign in to the Confluent Support Portal.</span></span> <span data-ttu-id="22dbf-126">Confluent のアカウントをお持ちではない場合は、 にメールをお送りください [cloud-support@confluent.io](mailto:cloud-support@confluent.io) 。</span><span class="sxs-lookup"><span data-stu-id="22dbf-126">If you do not have an account with Confluent, please send an email to [cloud-support@confluent.io](mailto:cloud-support@confluent.io).</span></span>

## <a name="datadog"></a><span data-ttu-id="22dbf-127">Datadog</span><span class="sxs-lookup"><span data-stu-id="22dbf-127">Datadog</span></span>

![DataDog ロゴ。](./media/partners/datadog.png)

<span data-ttu-id="22dbf-129">Datadog は、Azure ユーザーがハイブリッドおよびマルチクラウド環境全体のアプリケーションの正常性とパフォーマンスを把握するための監視およびセキュリティ ツールを提供します。</span><span class="sxs-lookup"><span data-stu-id="22dbf-129">Datadog provides observability and security tools for Azure users to understand the health and performance of their applications across hybrid and multi-cloud environments.</span></span> <span data-ttu-id="22dbf-130">ただし、必要な統合を構成するには、Azure portal と Datadog 間を頻繁に移動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="22dbf-130">But configuring the necessary integrations often requires navigating between the Azure portal and Datadog.</span></span> <span data-ttu-id="22dbf-131">ポータル間の構成とリソース管理を簡素化するために、Microsoft は Datadog と一緒に Azure に統合 Datadog ソリューションを作成しました。</span><span class="sxs-lookup"><span data-stu-id="22dbf-131">To simplify configuration and resource management across portals, Microsoft worked with Datadog to create an integrated Datadog solution on Azure.</span></span> <span data-ttu-id="22dbf-132">このソリューションAzure Marketplace、Azure のお客様が Datadog のクラウド監視ソリューションを使用するシームレスなエクスペリエンスを提供します。</span><span class="sxs-lookup"><span data-stu-id="22dbf-132">Available via the Azure Marketplace, this solution provides a seamless experience for Azure customers to use Datadog’s cloud monitoring solution.</span></span>

<span data-ttu-id="22dbf-133">このソリューション [Azure Monitor詳細](/azure/azure-monitor/platform/partners#datadog) を確認し、パブリック プレビューにサインアップするには、次のドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="22dbf-133">See the [Azure Monitor documentation](/azure/azure-monitor/platform/partners#datadog) to learn more about this solution and sign up for the public preview.</span></span>

## <a name="next-steps"></a><span data-ttu-id="22dbf-134">次のステップ</span><span class="sxs-lookup"><span data-stu-id="22dbf-134">Next steps</span></span>

- [<span data-ttu-id="22dbf-135">Azure Marketplace オンライン ストア</span><span class="sxs-lookup"><span data-stu-id="22dbf-135">Azure Marketplace online store</span></span>](https://azure.microsoft.com/marketplace/)
- [<span data-ttu-id="22dbf-136">Microsoft Learn: Azure アカウントを作成する</span><span class="sxs-lookup"><span data-stu-id="22dbf-136">Microsoft Learn: Create an Azure account</span></span>](/learn/modules/create-an-azure-account/)
