---
title: Azure Marketplace からのソフトウェアとソリューションの購入
description: Azure Marketplace でソフトウェアの購入と管理を簡略化し、合理化するツールについて説明します。
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: ac20b3c0603f886104499ab8de6da1d3459bbd57
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412575"
---
# <a name="azure-marketplace-purchasing"></a><span data-ttu-id="a2c4b-103">Azure Marketplace での購入</span><span class="sxs-lookup"><span data-stu-id="a2c4b-103">Azure Marketplace purchasing</span></span>

<span data-ttu-id="a2c4b-104">Azure Marketplace には多数のツールと機能があり、購入ポリシーの購入、請求、管理のプロセスを簡略化し、合理化することができます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-104">Azure Marketplace has numerous tools and features that simplify and streamline the process of purchasing, invoicing, and managing purchasing policy.</span></span>

## <a name="simplified-procurement"></a><span data-ttu-id="a2c4b-105">簡素化された調達</span><span class="sxs-lookup"><span data-stu-id="a2c4b-105">Simplified procurement</span></span>

<span data-ttu-id="a2c4b-106">Azure Marketplace は、さまざまな購入オプションを通じて調達プロセスを簡素化するために役立ちます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-106">Azure Marketplace helps you simplify the procurement process through different purchasing options.</span></span> <span data-ttu-id="a2c4b-107">Azure アカウントに関連付けられているクレジットカードを使用して製品を購入した場合、すべての購入は1つの請求書にまとめられ、選択したクレジットカードに請求されます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-107">If you purchase products using a credit card associated with your Azure account, all purchases will be consolidated on a single invoice and billed to the credit card of choice.</span></span> <span data-ttu-id="a2c4b-108">大規模なお客様の場合は、Enterprise Agreement を使用して購入できます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-108">If you are a large customer, you can purchase using an Enterprise Agreement.</span></span> <span data-ttu-id="a2c4b-109">EA を使用すると、すべてのソフトウェアの購入が Azure の請求書に自動的に含まれます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-109">With an EA, any software purchases are automatically included in your Azure invoice.</span></span> <span data-ttu-id="a2c4b-110">請求書の項目は、Azure の使用量に応じた請求に、Azure Marketplace の請求が続く形になります。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-110">Your invoice will contain Azure usage charges first, followed by Azure Marketplace charges.</span></span>

<span data-ttu-id="a2c4b-111">Azure Marketplace を通じて購入すると、個々のベンダーと請求書の管理の複雑さが解消されます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-111">When you purchase through Azure Marketplace, you eliminate the complexity of managing individual vendor relationships and invoices.</span></span> <span data-ttu-id="a2c4b-112">Azure Marketplace での購入と Azure の料金の両方を含む、Microsoft からの1つの統合月単位請求書を取得できます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-112">You get a single, consolidated monthly bill from Microsoft that includes both your Azure Marketplace purchases and your Azure charges.</span></span>

## <a name="permission-to-purchase"></a><span data-ttu-id="a2c4b-113">購入するためのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="a2c4b-113">Permission to purchase</span></span>

<span data-ttu-id="a2c4b-114">適切なソフトウェアアプリケーションが見つかったら、購入を完了するのは簡単です。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-114">After you've found the right software application, completing the purchase is simple.</span></span> <span data-ttu-id="a2c4b-115">ただし、Azure サブスクリプション内で適切なアクセス許可が必要になります。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-115">You will, however, need suitable permissions within the Azure subscription.</span></span> <span data-ttu-id="a2c4b-116">Azure は [ロールベースの Access Control](/azure/role-based-access-control/overview) (RBAC) モデルで動作するため、アカウントには購入を行うための **サブスクリプションの所有者** または **共同作成者** のアクセス許可が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-116">Since Azure operates on a [Role Based Access Control](/azure/role-based-access-control/overview) (RBAC) model, your account needs **subscription owner** or **contributor** permissions to make a purchase.</span></span>

<span data-ttu-id="a2c4b-117">購入を完了する前に、ユーザーが Azure テナントで正しい構成を持っていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-117">Before completing a purchase, make sure the user has the correct configuration in the Azure tenant.</span></span> <span data-ttu-id="a2c4b-118">これは、購入時のエラーを防ぐのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-118">This will help prevent errors during purchase.</span></span>

<span data-ttu-id="a2c4b-119">Azure portal の Azure Marketplace エクスペリエンスで、購入するアプリケーションを見つけ、[ **作成** ] または [セットアップ **+ サブスクライブ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-119">In the Azure Marketplace experience in the Azure portal, find the application you want to buy and select **Create** or **Set up + subscribe**.</span></span> <span data-ttu-id="a2c4b-120">新しいソリューションを使用する前に、いくつかの情報を入力するように求められます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-120">You'll be prompted to complete some information before being able to use your new solution.</span></span>

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="オファーの [作成] ボタン。":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="[セットアップ + サブスクライブ] ボタン。":::

<span data-ttu-id="a2c4b-123">Azure Marketplace オンラインストアからソリューションをデプロイする場合は、[製品の説明] ページで [ **今すぐ入手** する] を選択し、azure アカウントの資格情報でサインインします。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-123">If you want to deploy a solution from the Azure Marketplace online store, select **Get it now** on the product description page and then sign in with your Azure account credentials.</span></span>

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Azure Marketplace のサインインダイアログボックス。":::

<span data-ttu-id="a2c4b-125">サインインすると、Azure portal の製品にリダイレクトされ、購入が完了します。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-125">Once you sign in, you will be redirected to the product in the Azure portal to complete your purchase.</span></span>

## <a name="purchase-policy-management"></a><span data-ttu-id="a2c4b-126">ポリシー管理の購入</span><span class="sxs-lookup"><span data-stu-id="a2c4b-126">Purchase policy management</span></span>

<span data-ttu-id="a2c4b-127">Microsoft では、Azure サブスクリプション管理者として課金プロファイルを使用してユーザーの購入を管理できます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-127">Microsoft lets you manage user purchases through your billing profile as the Azure subscription administrator.</span></span> <span data-ttu-id="a2c4b-128">次の 3 つのオプションから選択できます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-128">Choose from three options:</span></span>

- <span data-ttu-id="a2c4b-129">**無料 + 有料** – Azure Marketplace ソフトウェアアプリケーションを取得することをユーザーに許可します。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-129">**Free + Paid** – Allows users to acquire any Azure Marketplace software application.</span></span>
- <span data-ttu-id="a2c4b-130">**Free** – Azure Marketplace から無料のソフトウェアのみをデプロイできます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-130">**Free** – Allows users to deploy only free software from Azure Marketplace.</span></span>
- <span data-ttu-id="a2c4b-131">[いいえ] –ユーザー **が** Azure Marketplace からソフトウェアをデプロイできないようにします。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-131">**No** – Prevents users from deploying any software from Azure Marketplace.</span></span>

<span data-ttu-id="a2c4b-132">これらの設定は、Azure サブスクリプションへのアクセス権を持つすべてのユーザーに適用されます。これにより、Azure portal を通じて IT 調達を制御できるようになります。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-132">These settings apply to all users with access to your Azure subscription, which gives you the capability to control IT procurement through the Azure portal.</span></span>

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Azure portal による IT 調達の制御":::

## <a name="cost-management"></a><span data-ttu-id="a2c4b-134">コスト管理</span><span class="sxs-lookup"><span data-stu-id="a2c4b-134">Cost management</span></span>

<span data-ttu-id="a2c4b-135">Azure Marketplace から製品を購入すると、コストの管理に役立つ洞察を得ることができます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-135">As you purchase products from Azure Marketplace, you want to get insights that help you manage costs.</span></span> <span data-ttu-id="a2c4b-136">Azure Cost Management は、購入した製品に関する情報を表示するための無料ツールです。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-136">Azure Cost Management is a free tool for viewing information on the products you've purchased.</span></span> <span data-ttu-id="a2c4b-137">Cost Management を使用すると、時間の経過と共に使用しているサービスの詳細と、設定した予算に対してそれらのコストがどのように追跡されるかを確認できます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-137">You can use Cost Management to see details of what services you're spending money on over time and how those costs track against the budgets you've set.</span></span> <span data-ttu-id="a2c4b-138">予算を設定するだけでなく、レポートのスケジュールを設定したり、サブスクリプションのコストを分析したりすることもできます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-138">In addition to setting budgets, you can schedule reports and analyze subscription costs.</span></span> <span data-ttu-id="a2c4b-139">Azure Cost Management の詳細については、「 [コストの分析」と「Azure Cost Management を使用した予算の作成](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)」の「Microsoft Learn」モジュールを参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-139">Learn more about Azure Cost Management by completing the Microsoft Learn module on [Analyze costs and create budgets with Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).</span></span>

<span data-ttu-id="a2c4b-140">Azure Marketplace の料金と請求書は、Azure Cost Management の費用分析ツールで確認できます。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-140">You can view your Azure Marketplace charges and invoices on the cost analysis tool under Azure Cost Management.</span></span>

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Azure Cost Management を使用すると、購入した製品に関する洞察を得ることができます。":::

## <a name="purchase-validation-checks"></a><span data-ttu-id="a2c4b-142">購入検証の確認</span><span class="sxs-lookup"><span data-stu-id="a2c4b-142">Purchase validation checks</span></span>

<span data-ttu-id="a2c4b-143">Azure Marketplace でプランを購入すると、さまざまな理由で失敗する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-143">Purchasing an offer through Azure Marketplace can fail for different reasons.</span></span> <span data-ttu-id="a2c4b-144">購入にコマンドラインインターフェイス (CLI) を使用すると、Azure Marketplace で使用できない、または表示できないプランを購入しようとしている場合があるため、エラーが発生する可能性が高くなります。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-144">Using the command-line interface (CLI) for a purchase is more likely to cause errors since you may be trying to purchase an offer that is not available or visible in Azure Marketplace.</span></span> <span data-ttu-id="a2c4b-145">次に、購入に失敗する可能性があるチェックを示します。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-145">Following are the checks that can cause a purchase to fail:</span></span>

1. <span data-ttu-id="a2c4b-146">サブスクリプションは、Enterprise Agreement (EA) に属し、EA 管理者によって無効化された Azure Marketplace の購入が無効になっています。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-146">The subscription belongs to an Enterprise Agreement (EA) and the EA admin disabled Azure Marketplace purchases.</span></span>
1. <span data-ttu-id="a2c4b-147">EA 管理者は無料プランでのみ購入が有効になっており、プランは有料プランです。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-147">The EA admin has enabled purchases only for free offers and the offer is a paid offer.</span></span>
1. <span data-ttu-id="a2c4b-148">プランが marketplace に見つかりません。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-148">The offer is not found in the marketplace.</span></span>
1. <span data-ttu-id="a2c4b-149">独立系ソフトウェアベンダー (ISV) は、少なくともお客様の地域でプランの販売を停止しました。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-149">The Independent Software Vendor (ISV) stopped selling the offer, at least in your region.</span></span>
1. <span data-ttu-id="a2c4b-150">使用しているサブスクリプションは、プランが使用できないリージョンの課金アカウントに属しています。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-150">The subscription you are using belongs to a billing account in a region where the offer is not available.</span></span>
1. <span data-ttu-id="a2c4b-151">サブスクリプション/請求アカウントが有効な支払い方法 (有効なクレジットカードなど) に関連付けられていません。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-151">The subscription/billing account is not associated with a valid payment instrument (such as a valid credit card).</span></span>
1. <span data-ttu-id="a2c4b-152">サブスクリプションはクラウドソリューションプロバイダー (CSP) に属し、ISV は CSP による販売を拒否しました。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-152">The subscription belongs to a Cloud Solution Provider (CSP) and the ISV declined to sell through a CSP.</span></span>
1. <span data-ttu-id="a2c4b-153">サブスクリプションに対してプライベートマーケットプレースが有効になっていますが、プランは許可されているプランの一覧に含まれていません。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-153">Private Marketplace is enabled for the subscription and the offer is not in the list of allowed offers.</span></span>
1. <span data-ttu-id="a2c4b-154">プランは特定の顧客のプライベート/プレビューであり、サブスクリプションは許可されている顧客の一覧に含まれていません。</span><span class="sxs-lookup"><span data-stu-id="a2c4b-154">The offer is Private/Preview for specific customers and the subscription is not in the list of allowed customers.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a2c4b-155">次の手順</span><span class="sxs-lookup"><span data-stu-id="a2c4b-155">Next steps</span></span>

- [<span data-ttu-id="a2c4b-156">請求と請求書作成</span><span class="sxs-lookup"><span data-stu-id="a2c4b-156">Billing and invoicing</span></span>](billing-invoicing.md)