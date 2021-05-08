---
title: Azure Marketplace からのソフトウェアとソリューションの購入
description: Azure Marketplace でソフトウェアの購入と管理を簡略化し、合理化するツールについて説明します。
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 04/15/2021
ms.openlocfilehash: cfe37f26ad685ca723336d8559d15d4a64048f4b
ms.sourcegitcommit: 2ad9e61fa5b9941f927ebf44c459b6c1bd055b9d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/08/2021
ms.locfileid: "109630085"
---
# <a name="azure-marketplace-purchasing"></a><span data-ttu-id="0deb9-103">Azure Marketplace での購入</span><span class="sxs-lookup"><span data-stu-id="0deb9-103">Azure Marketplace purchasing</span></span>

<span data-ttu-id="0deb9-104">Azure Marketplace には多数のツールと機能があり、購入ポリシーの購入、請求、管理のプロセスを簡略化し、合理化することができます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-104">Azure Marketplace has numerous tools and features that simplify and streamline the process of purchasing, invoicing, and managing purchasing policy.</span></span>

## <a name="simplified-procurement"></a><span data-ttu-id="0deb9-105">簡素化された調達</span><span class="sxs-lookup"><span data-stu-id="0deb9-105">Simplified procurement</span></span>

<span data-ttu-id="0deb9-106">Azure Marketplace は、さまざまな購入オプションを通じて調達プロセスを簡素化するために役立ちます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-106">Azure Marketplace helps you simplify the procurement process through different purchasing options.</span></span> <span data-ttu-id="0deb9-107">Azure アカウントに関連付けられているクレジットカードを使用して製品を購入した場合、すべての購入は1つの請求書にまとめられ、選択したクレジットカードに請求されます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-107">If you purchase products using a credit card associated with your Azure account, all purchases will be consolidated on a single invoice and billed to the credit card of choice.</span></span> <span data-ttu-id="0deb9-108">大規模なお客様の場合は、Enterprise Agreement を使用して購入できます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-108">If you are a large customer, you can purchase using an Enterprise Agreement.</span></span> <span data-ttu-id="0deb9-109">EA を使用すると、すべてのソフトウェアの購入が Azure の請求書に自動的に含まれます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-109">With an EA, any software purchases are automatically included in your Azure invoice.</span></span> <span data-ttu-id="0deb9-110">請求書の項目は、Azure の使用量に応じた請求に、Azure Marketplace の請求が続く形になります。</span><span class="sxs-lookup"><span data-stu-id="0deb9-110">Your invoice will contain Azure usage charges first, followed by Azure Marketplace charges.</span></span>

<span data-ttu-id="0deb9-111">Azure Marketplace を通じて購入すると、個々のベンダーと請求書の管理の複雑さが解消されます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-111">When you purchase through Azure Marketplace, you eliminate the complexity of managing individual vendor relationships and invoices.</span></span> <span data-ttu-id="0deb9-112">Azure Marketplace での購入と Azure の料金の両方を含む、Microsoft からの1つの統合月単位請求書を取得できます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-112">You get a single, consolidated monthly bill from Microsoft that includes both your Azure Marketplace purchases and your Azure charges.</span></span>

## <a name="permission-to-purchase"></a><span data-ttu-id="0deb9-113">購入するためのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="0deb9-113">Permission to purchase</span></span>

<span data-ttu-id="0deb9-114">適切なソフトウェアアプリケーションが見つかったら、購入を完了するのは簡単です。</span><span class="sxs-lookup"><span data-stu-id="0deb9-114">After you've found the right software application, completing the purchase is simple.</span></span> <span data-ttu-id="0deb9-115">ただし、Azure サブスクリプション内で適切なアクセス許可が必要になります。</span><span class="sxs-lookup"><span data-stu-id="0deb9-115">You will, however, need suitable permissions within the Azure subscription.</span></span> <span data-ttu-id="0deb9-116">Azure は [ロールベースの Access Control](/azure/role-based-access-control/overview) (RBAC) モデルで動作するため、アカウントには購入を行うための **サブスクリプションの所有者** または **共同作成者** のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="0deb9-116">Since Azure operates on a [Role Based Access Control](/azure/role-based-access-control/overview) (RBAC) model, your account needs **subscription owner** or **contributor** permissions to make a purchase.</span></span>

<span data-ttu-id="0deb9-117">購入を完了する前に、ユーザーが Azure テナントで正しい構成を持っていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="0deb9-117">Before completing a purchase, make sure the user has the correct configuration in the Azure tenant.</span></span> <span data-ttu-id="0deb9-118">これは、購入時のエラーを防ぐのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-118">This will help prevent errors during purchase.</span></span>

<span data-ttu-id="0deb9-119">Azure portal の Azure Marketplace エクスペリエンスで、購入するアプリケーションを見つけ、[ **作成** ] または [セットアップ **+ サブスクライブ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="0deb9-119">In the Azure Marketplace experience in the Azure portal, find the application you want to buy and select **Create** or **Set up + subscribe**.</span></span> <span data-ttu-id="0deb9-120">新しいソリューションを使用する前に、いくつかの情報を入力するように求められます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-120">You'll be prompted to complete some information before being able to use your new solution.</span></span>

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="オファーの [作成] ボタン。":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="[セットアップ + サブスクライブ] ボタン。":::

<span data-ttu-id="0deb9-123">Azure Marketplace オンライン ストアからソリューションをデプロイする場合は、製品の説明ページで [今すぐ取得] を選択し、Azure アカウントの資格情報でサインインします。</span><span class="sxs-lookup"><span data-stu-id="0deb9-123">If you want to deploy a solution from the Azure Marketplace online store, select **Get it now** on the product description page and then sign in with your Azure account credentials.</span></span>

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="[Azure Marketplace] ダイアログ ボックス。":::

<span data-ttu-id="0deb9-125">サインインすると、購入を完了するために、Azure portal製品にリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-125">Once you sign in, you will be redirected to the product in the Azure portal to complete your purchase.</span></span>

## <a name="purchase-policy-management"></a><span data-ttu-id="0deb9-126">購入ポリシー管理</span><span class="sxs-lookup"><span data-stu-id="0deb9-126">Purchase policy management</span></span>

<span data-ttu-id="0deb9-127">Microsoft では、Azure サブスクリプション管理者として課金プロファイルを使用してユーザーの購入を管理できます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-127">Microsoft lets you manage user purchases through your billing profile as the Azure subscription administrator.</span></span> <span data-ttu-id="0deb9-128">次の 3 つのオプションから選択できます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-128">Choose from three options:</span></span>

- <span data-ttu-id="0deb9-129">**無料 + 有料** – ユーザーは、任意のソフトウェア アプリケーションAzure Marketplace取得できます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-129">**Free + Paid** – Allows users to acquire any Azure Marketplace software application.</span></span>
- <span data-ttu-id="0deb9-130">**[無料** ] – ユーザーが無料のソフトウェアのみを展開Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="0deb9-130">**Free** – Allows users to deploy only free software from Azure Marketplace.</span></span>
- <span data-ttu-id="0deb9-131">**[いいえ** ] – ユーザーがソフトウェアを展開Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="0deb9-131">**No** – Prevents users from deploying any software from Azure Marketplace.</span></span>

<span data-ttu-id="0deb9-132">これらの設定は、Azure サブスクリプションにアクセスできるすべてのユーザーに適用されます。これにより、Azure サブスクリプションを通じて IT 調達を制御Azure portal。</span><span class="sxs-lookup"><span data-stu-id="0deb9-132">These settings apply to all users with access to your Azure subscription, which gives you the capability to control IT procurement through the Azure portal.</span></span>

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="サービスを通じた IT 調達のAzure portal":::

## <a name="cost-management"></a><span data-ttu-id="0deb9-134">コスト管理</span><span class="sxs-lookup"><span data-stu-id="0deb9-134">Cost management</span></span>

<span data-ttu-id="0deb9-135">顧客から製品を購入するAzure Marketplace、コストの管理に役立つ分析情報を得る必要があります。</span><span class="sxs-lookup"><span data-stu-id="0deb9-135">As you purchase products from Azure Marketplace, you want to get insights that help you manage costs.</span></span> <span data-ttu-id="0deb9-136">Azure Cost Managementは、購入した製品に関する情報を表示する無料のツールです。</span><span class="sxs-lookup"><span data-stu-id="0deb9-136">Azure Cost Management is a free tool for viewing information on the products you've purchased.</span></span> <span data-ttu-id="0deb9-137">Cost Managementを使用して、時間の費やしているサービスの詳細と、設定した予算に対してそれらのコストがどのように追跡されるのかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-137">You can use Cost Management to see details of what services you're spending money on over time and how those costs track against the budgets you've set.</span></span> <span data-ttu-id="0deb9-138">予算の設定に加えて、レポートをスケジュールし、サブスクリプションのコストを分析できます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-138">In addition to setting budgets, you can schedule reports and analyze subscription costs.</span></span> <span data-ttu-id="0deb9-139">コストの分析とAzure Cost Managementの作成に関するMicrosoft Learnモジュールを完了して、コストの詳細を[確認Azure Cost Management。](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)</span><span class="sxs-lookup"><span data-stu-id="0deb9-139">Learn more about Azure Cost Management by completing the Microsoft Learn module on [Analyze costs and create budgets with Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).</span></span>

<span data-ttu-id="0deb9-140">Azure Marketplace の料金と請求書は、Azure Cost Management の費用分析ツールで確認できます。</span><span class="sxs-lookup"><span data-stu-id="0deb9-140">You can view your Azure Marketplace charges and invoices on the cost analysis tool under Azure Cost Management.</span></span>

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="購入Azure Cost Managementに関する分析情報を取得するには、次のコマンドを使用します。":::

## <a name="purchase-validation-checks"></a><span data-ttu-id="0deb9-142">購入の検証チェック</span><span class="sxs-lookup"><span data-stu-id="0deb9-142">Purchase validation checks</span></span>

<span data-ttu-id="0deb9-143">サービスを通じてオファー Azure Marketplace、さまざまな理由で失敗する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0deb9-143">Purchasing an offer through Azure Marketplace can fail for different reasons.</span></span> <span data-ttu-id="0deb9-144">購入にコマンド ライン インターフェイス (CLI) を使用すると、Azure Marketplace で使用できないオファーを購入しようとしている可能性が高く、エラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0deb9-144">Using the command-line interface (CLI) for a purchase is more likely to cause errors since you may be trying to purchase an offer that is not available or visible in Azure Marketplace.</span></span> <span data-ttu-id="0deb9-145">購入が失敗する可能性があるチェックを次に示します。</span><span class="sxs-lookup"><span data-stu-id="0deb9-145">Following are the checks that can cause a purchase to fail:</span></span>

1. <span data-ttu-id="0deb9-146">サブスクリプションは、Enterprise Agreement (EA) に属し、EA 管理者によって無効化された Azure Marketplace の購入が無効になっています。</span><span class="sxs-lookup"><span data-stu-id="0deb9-146">The subscription belongs to an Enterprise Agreement (EA) and the EA admin disabled Azure Marketplace purchases.</span></span>
1. <span data-ttu-id="0deb9-147">EA 管理者は無料プランでのみ購入が有効になっており、プランは有料プランです。</span><span class="sxs-lookup"><span data-stu-id="0deb9-147">The EA admin has enabled purchases only for free offers and the offer is a paid offer.</span></span>
1. <span data-ttu-id="0deb9-148">プランが marketplace に見つかりません。</span><span class="sxs-lookup"><span data-stu-id="0deb9-148">The offer is not found in the marketplace.</span></span>
1. <span data-ttu-id="0deb9-149">独立系ソフトウェアベンダー (ISV) は、少なくともお客様の地域で提供されているプランを非推奨としました。</span><span class="sxs-lookup"><span data-stu-id="0deb9-149">The Independent Software Vendor (ISV) deprecated (formerly stop sell) the offer, at least in your region.</span></span>
1. <span data-ttu-id="0deb9-150">使用しているサブスクリプションは、プランが使用できないリージョンの課金アカウントに属しています。</span><span class="sxs-lookup"><span data-stu-id="0deb9-150">The subscription you are using belongs to a billing account in a region where the offer is not available.</span></span>
1. <span data-ttu-id="0deb9-151">サブスクリプション/請求アカウントが有効な支払い方法 (有効なクレジットカードなど) に関連付けられていません。</span><span class="sxs-lookup"><span data-stu-id="0deb9-151">The subscription/billing account is not associated with a valid payment instrument (such as a valid credit card).</span></span>
1. <span data-ttu-id="0deb9-152">サブスクリプションはクラウドソリューションプロバイダー (CSP) に属し、ISV は CSP による販売を拒否しました。</span><span class="sxs-lookup"><span data-stu-id="0deb9-152">The subscription belongs to a Cloud Solution Provider (CSP) and the ISV declined to sell through a CSP.</span></span>
1. <span data-ttu-id="0deb9-153">サブスクリプションに対してプライベートマーケットプレースが有効になっていますが、プランは許可されているプランの一覧に含まれていません。</span><span class="sxs-lookup"><span data-stu-id="0deb9-153">Private Marketplace is enabled for the subscription and the offer is not in the list of allowed offers.</span></span>
1. <span data-ttu-id="0deb9-154">プランは特定の顧客のプライベート/プレビューであり、サブスクリプションは許可されている顧客の一覧に含まれていません。</span><span class="sxs-lookup"><span data-stu-id="0deb9-154">The offer is Private/Preview for specific customers and the subscription is not in the list of allowed customers.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0deb9-155">次のステップ</span><span class="sxs-lookup"><span data-stu-id="0deb9-155">Next steps</span></span>

- [<span data-ttu-id="0deb9-156">請求と請求書作成</span><span class="sxs-lookup"><span data-stu-id="0deb9-156">Billing and invoicing</span></span>](billing-invoicing.md)