---
title: Azure Marketplace パートナーの統合
description: Azure 環境に統合された Azure Marketplace ソリューションについて説明し、Microsoft パートナーのデプロイガイドへのリンクを提供します。
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: b31486000e59f3d85ee30019ecea000252b297a8
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/21/2020
ms.locfileid: "95006907"
---
# <a name="azure-marketplace-partner-integrations"></a><span data-ttu-id="5bf46-103">Azure Marketplace パートナーの統合</span><span class="sxs-lookup"><span data-stu-id="5bf46-103">Azure Marketplace partner integrations</span></span>

<span data-ttu-id="5bf46-104">パートナーソリューションを Azure 環境に統合する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="5bf46-104">Learn how to integrate partner solutions into your Azure environment.</span></span> <span data-ttu-id="5bf46-105">この記事では、各ソリューションの概要と、詳細なデプロイガイドへのリンクを示します。</span><span class="sxs-lookup"><span data-stu-id="5bf46-105">This article gives an overview of each solution and links to detailed deployment guides.</span></span> <span data-ttu-id="5bf46-106">ソリューションはアルファベット順に一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="5bf46-106">Solutions are listed in alphabetical order.</span></span> 

## <a name="apache-kafka-on-confluent-cloud"></a><span data-ttu-id="5bf46-107">Confluent Cloud での Apache Kafka</span><span class="sxs-lookup"><span data-stu-id="5bf46-107">Apache Kafka on Confluent Cloud</span></span>

![Confluent Cloud](./media/partners/confluent-cloud.png)

<span data-ttu-id="5bf46-109">Azure では、クラウドアプリケーションに加えて Confluent Cloud と統合できます。</span><span class="sxs-lookup"><span data-stu-id="5bf46-109">Azure lets you integrate with Confluent Cloud in addition to your cloud applications.</span></span> <span data-ttu-id="5bf46-110">Confluent のお客様は、多くの場合、Azure portal と Confluent Cloud の間を移動します。</span><span class="sxs-lookup"><span data-stu-id="5bf46-110">Confluent customers often navigate between the Azure portal and Confluent Cloud.</span></span> <span data-ttu-id="5bf46-111">たとえば、ユーザーが Azure Marketplace で Confluent Cloud プランを購入すると、Confluent Cloud を使用してアカウントを設定することが求められます。</span><span class="sxs-lookup"><span data-stu-id="5bf46-111">For example, once a user purchases a Confluent Cloud offer in Azure Marketplace, they are then expected to set up an account with Confluent Cloud.</span></span> <span data-ttu-id="5bf46-112">このプロセスでは複雑さと時間が増加するため、ユーザーは2つのポータル間で構成とリソースを管理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5bf46-112">This process adds complexity and time, and requires users to manage configuration and resources between the two portals.</span></span> <span data-ttu-id="5bf46-113">Microsoft が Confluent Cloud と提携しているプラットフォームでの管理の負担を軽減するために、Azure から Confluent Cloud に統合されたプロビジョニングレイヤーを構築しています。</span><span class="sxs-lookup"><span data-stu-id="5bf46-113">To reduce the burden of managing across platforms, Microsoft, in partnership with Confluent Cloud, built an integrated provisioning layer from Azure to Confluent Cloud.</span></span> <span data-ttu-id="5bf46-114">このソリューションは Azure Marketplace で利用可能であり、Azure で Confluent Cloud オファリングを使用するためのシームレスなエクスペリエンスを提供します</span><span class="sxs-lookup"><span data-stu-id="5bf46-114">The solution is available in Azure Marketplace and  provides a seamless experience for using the Confluent Cloud offering on Azure</span></span>

<span data-ttu-id="5bf46-115">このソリューションでは、Azure で有効になっているリソースプロバイダーを使用して、Confluent クラウドリソースをプロビジョニングします。</span><span class="sxs-lookup"><span data-stu-id="5bf46-115">The solution uses a resource provider enabled in Azure to provision Confluent Cloud resources.</span></span> <span data-ttu-id="5bf46-116">これにより、ユーザーは Azure portal、Azure CLI、Azure Sdk を使用してリアルタイムのイベントストリーミングにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="5bf46-116">This allows users to access real-time event streaming via the Azure portal, Azure CLI, and Azure SDKs.</span></span> <span data-ttu-id="5bf46-117">Confluent Cloud は、環境、クラスター、トピック、API キー、およびマネージコネクタを含む SaaS アプリケーションを所有して実行します。</span><span class="sxs-lookup"><span data-stu-id="5bf46-117">Confluent Cloud owns and runs the SaaS application, which includes environments, clusters, topics, API keys, and managed connectors.</span></span>

<span data-ttu-id="5bf46-118">Confluent Cloud との緊密な統合により、次の機能が有効になります。</span><span class="sxs-lookup"><span data-stu-id="5bf46-118">The deep integration with Confluent Cloud enables the following capabilities:</span></span>

- <span data-ttu-id="5bf46-119">完全に管理されたインフラストラクチャを使用して、Azure portal から新しい Confluent Cloud 組織のリソースをプロビジョニングします。</span><span class="sxs-lookup"><span data-stu-id="5bf46-119">Provision a new Confluent Cloud organization resource from the Azure portal with fully managed infrastructure.</span></span>
- <span data-ttu-id="5bf46-120">Azure Active Directory を使用した Azure から Confluent Cloud へのシングルサインオンを効率化します。Confluent Cloud ポータルでは、別個の認証は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="5bf46-120">Streamline single sign-on from Azure to Confluent Cloud with Azure Active Directory; no separate authentication needed from the Confluent Cloud portal.</span></span>
- <span data-ttu-id="5bf46-121">Azure サブスクリプションの請求書を通じて、Confluent クラウドの消費料金の統合課金を取得します。</span><span class="sxs-lookup"><span data-stu-id="5bf46-121">Get unified billing of Confluent Cloud consumption charges through Azure subscription invoicing.</span></span>
- <span data-ttu-id="5bf46-122">Azure portal から Confluent Cloud リソースを管理し、Azure リソースと共に [ **すべてのリソース** ] ページで追跡します。</span><span class="sxs-lookup"><span data-stu-id="5bf46-122">Manage Confluent Cloud resources from the Azure portal, and track them in the **All resources** page, alongside your Azure resources.</span></span>

[<span data-ttu-id="5bf46-123">Confluent クラウドデプロイガイド</span><span class="sxs-lookup"><span data-stu-id="5bf46-123">Confluent Cloud deployment guides</span></span>](https://docs.confluent.io/current/cloud/marketplace/index.html)

<span data-ttu-id="5bf46-124">Azure での Confluent に関する問題については、「」を参照 [https://support.confluent.io](https://support.confluent.io) してください。</span><span class="sxs-lookup"><span data-stu-id="5bf46-124">For issues related to Confluent on Azure, go to [https://support.confluent.io](https://support.confluent.io).</span></span> <span data-ttu-id="5bf46-125">初めてのユーザーの場合は、Confluent サポートポータルにサインインする前にパスワードをリセットしてください。</span><span class="sxs-lookup"><span data-stu-id="5bf46-125">If you are a first time user, reset your password before you sign in to the Confluent Support Portal.</span></span> <span data-ttu-id="5bf46-126">Confluent のアカウントをお持ちでない場合は、に電子メールをお送りください [cloud-support@confluent.io](mailto:cloud-support@confluent.io) 。</span><span class="sxs-lookup"><span data-stu-id="5bf46-126">If you do not have an account with Confluent, please send an email to [cloud-support@confluent.io](mailto:cloud-support@confluent.io).</span></span>

## <a name="datadog"></a><span data-ttu-id="5bf46-127">Datadog</span><span class="sxs-lookup"><span data-stu-id="5bf46-127">Datadog</span></span>

![DataDog のロゴ](./media/partners/datadog.png)

<span data-ttu-id="5bf46-129">Datadog は、ハイブリッド環境とマルチクラウド環境でのアプリケーションの正常性とパフォーマンスを理解するために、Azure ユーザー向けの可観測性およびセキュリティツールを提供します。</span><span class="sxs-lookup"><span data-stu-id="5bf46-129">Datadog provides observability and security tools for Azure users to understand the health and performance of their applications across hybrid and multi-cloud environments.</span></span> <span data-ttu-id="5bf46-130">ただし、必要な統合を構成するには、Azure portal と Datadog 間を頻繁に移動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5bf46-130">But configuring the necessary integrations often requires navigating between the Azure portal and Datadog.</span></span> <span data-ttu-id="5bf46-131">ポータルでの構成とリソースの管理を簡略化するために、Microsoft は Datadog と連携して Azure で統合 Datadog ソリューションを作成しました。</span><span class="sxs-lookup"><span data-stu-id="5bf46-131">To simplify configuration and resource management across portals, Microsoft worked with Datadog to create an integrated Datadog solution on Azure.</span></span> <span data-ttu-id="5bf46-132">Azure Marketplace を通じて提供されているこのソリューションでは、Azure のお客様が Datadog のクラウド監視ソリューションを使用するためのシームレスなエクスペリエンスを提供します。</span><span class="sxs-lookup"><span data-stu-id="5bf46-132">Available via the Azure Marketplace, this solution provides a seamless experience for Azure customers to use Datadog’s cloud monitoring solution.</span></span>

<span data-ttu-id="5bf46-133">このソリューションの詳細については、 [Azure Monitor のドキュメント](/azure/azure-monitor/platform/partners#datadog) を参照して、パブリックプレビューにサインアップしてください。</span><span class="sxs-lookup"><span data-stu-id="5bf46-133">See the [Azure Monitor documentation](/azure/azure-monitor/platform/partners#datadog) to learn more about this solution and sign up for the public preview.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5bf46-134">次の手順</span><span class="sxs-lookup"><span data-stu-id="5bf46-134">Next steps</span></span>

- [<span data-ttu-id="5bf46-135">Azure Marketplace オンラインストア</span><span class="sxs-lookup"><span data-stu-id="5bf46-135">Azure Marketplace online store</span></span>](https://azure.microsoft.com/marketplace/)
- [<span data-ttu-id="5bf46-136">Microsoft Learn: Azure アカウントを作成する</span><span class="sxs-lookup"><span data-stu-id="5bf46-136">Microsoft Learn: Create an Azure account</span></span>](/learn/modules/create-an-azure-account/)
