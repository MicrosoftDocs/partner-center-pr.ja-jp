---
title: 未払い、詐欺、不正使用の管理
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: オンライントランザクションに関連するさまざまなリスクと、それらのリスクを管理して軽減するためのベストプラクティスについて理解することが重要です。
keywords: 詐欺, 不正使用, 使用条件, 利用規約, 未払い, 顧客が料金を支払わない, オンライン リスク, サービスの盗用, サービスの不正使用, サブスクリプションの一時停止,
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0b08fc6a94f91be978802a6bf850b46189ea740f
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377806"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a><span data-ttu-id="90c79-104">パートナー センターでの未払い、詐欺、不正使用の管理</span><span class="sxs-lookup"><span data-stu-id="90c79-104">Managing non-payment, fraud, or misuse in Partner Center</span></span>

<span data-ttu-id="90c79-105">適用対象:</span><span class="sxs-lookup"><span data-stu-id="90c79-105">Applies to:</span></span>

- <span data-ttu-id="90c79-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="90c79-106">Partner Center</span></span>
- <span data-ttu-id="90c79-107">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="90c79-107">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="90c79-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="90c79-108">**Appropriate roles**</span></span>
- <span data-ttu-id="90c79-109">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="90c79-109">Global admin</span></span>
- <span data-ttu-id="90c79-110">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="90c79-110">User admin</span></span>
- <span data-ttu-id="90c79-111">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="90c79-111">Admin agent</span></span>
- <span data-ttu-id="90c79-112">課金管理者</span><span class="sxs-lookup"><span data-stu-id="90c79-112">Billing admin</span></span>

<span data-ttu-id="90c79-113">パートナーは、顧客による不正購入や、購入サービスの料金未払いについて、金銭的な責任を負います。</span><span class="sxs-lookup"><span data-stu-id="90c79-113">You are financially responsible for fraudulent purchases by your customers and/or customers' non-payment of purchased services.</span></span> <span data-ttu-id="90c79-114">したがって、*不正行為の防止と検出のリスク軽減のための制御*を行うことを強くお勧めします。</span><span class="sxs-lookup"><span data-stu-id="90c79-114">Therefore, *we strongly recommend that you put in place fraud prevention and detection risk mitigation controls*.</span></span>

<span data-ttu-id="90c79-115">不正行為や不正使用を回避したり、これらに対処するには、潜在的なリスクを理解して、リスクへの露出を軽減するためのポリシーとプラクティスを作成することが重要です。</span><span class="sxs-lookup"><span data-stu-id="90c79-115">To avoid and/or address fraudulent activity or misuse, it's important to understand potential risks and to develop policies and practices that can reduce your exposure.</span></span>

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a><span data-ttu-id="90c79-116">Microsoft による利用規約の適用</span><span class="sxs-lookup"><span data-stu-id="90c79-116">Enforcement of Microsoft Acceptable Use Policy</span></span>

<span data-ttu-id="90c79-117">許容される使用ポリシーに違反しているかどうかを確認するパートナーまたは顧客のアクティビティを Microsoft が検出した場合は、実施手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="90c79-117">If Microsoft detects partner or customer activity that we confirm or suspect violates the Acceptable Use Policy, we will take enforcement steps.</span></span> <span data-ttu-id="90c79-118">顧客はすぐに中断される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="90c79-118">The customer could be immediately suspended.</span></span> <span data-ttu-id="90c79-119">Microsoft からの要求に対して、実施アクションまたは更新が通知されます。</span><span class="sxs-lookup"><span data-stu-id="90c79-119">You'll be notified of enforcement actions or updated on your requests by Microsoft.</span></span>

## <a name="abuse-of-service-risks"></a><span data-ttu-id="90c79-120">サービスリスクの悪用</span><span class="sxs-lookup"><span data-stu-id="90c79-120">Abuse of service risks</span></span>

<span data-ttu-id="90c79-121">**サービスのリスクを悪用**すると、クラウドサービスを使用するお客様は、マイクロソフトの利用規約に違反することになります。</span><span class="sxs-lookup"><span data-stu-id="90c79-121">**Abuse of service** risks means customers who use cloud services in violation of Microsoft's Acceptable Use Policy.</span></span>

### <a name="examples-of-abuse-of-service"></a><span data-ttu-id="90c79-122">サービスの悪用の例</span><span class="sxs-lookup"><span data-stu-id="90c79-122">Examples of abuse of service</span></span>

<span data-ttu-id="90c79-123">Microsoft の利用規約に違反する例として、次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="90c79-123">Examples of these violations of Microsoft's acceptable use policy can include:</span></span>

- <span data-ttu-id="90c79-124">スパム</span><span class="sxs-lookup"><span data-stu-id="90c79-124">Spamming</span></span>
- <span data-ttu-id="90c79-125">ハッキング</span><span class="sxs-lookup"><span data-stu-id="90c79-125">Hacking</span></span>
- <span data-ttu-id="90c79-126">分散型サービス拒否 (DDoS) 攻撃</span><span class="sxs-lookup"><span data-stu-id="90c79-126">Distributed denial-of-service (DDoS) attacks</span></span>
- <span data-ttu-id="90c79-127">ビットコイン マイニング</span><span class="sxs-lookup"><span data-stu-id="90c79-127">Bitcoin mining</span></span>
- <span data-ttu-id="90c79-128">マルウェアの配布</span><span class="sxs-lookup"><span data-stu-id="90c79-128">Malware distribution</span></span>
- <span data-ttu-id="90c79-129">偽造されたサブスクリプションの再販</span><span class="sxs-lookup"><span data-stu-id="90c79-129">Resale of pirated subscriptions</span></span>

## <a name="theft-of-service-risks"></a><span data-ttu-id="90c79-130">サービスリスクの盗難</span><span class="sxs-lookup"><span data-stu-id="90c79-130">Theft of service risks</span></span>

<span data-ttu-id="90c79-131">**サービスリスクの盗難**は、消費されたサービスに対して支払いを行うことがないお客様を意味します。</span><span class="sxs-lookup"><span data-stu-id="90c79-131">**Theft of service** risks means customers who have no intention of paying for consumed services.</span></span> <span data-ttu-id="90c79-132">この盗難には、盗まれた支払い方法の使用、誤請求情報の提供、または未払い残高の既定値の使用が含まれる場合があります。</span><span class="sxs-lookup"><span data-stu-id="90c79-132">This theft may involve using stolen payment instruments, providing false billing information, and/or defaulting on outstanding balances.</span></span>

### <a name="examples-of-service-theft"></a><span data-ttu-id="90c79-133">サービスの盗難の例</span><span class="sxs-lookup"><span data-stu-id="90c79-133">Examples of service theft</span></span>

<span data-ttu-id="90c79-134">オンライントランザクションのリスクの例としては、次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="90c79-134">Examples of these online transaction risks can include:</span></span>

- <span data-ttu-id="90c79-135">担当者では発生しないトランザクション ("クレジットカードが存在しません" トランザクション)</span><span class="sxs-lookup"><span data-stu-id="90c79-135">Transactions that don't occur in person ("credit card not present" transactions)</span></span>
- <span data-ttu-id="90c79-136">ID の不正使用</span><span class="sxs-lookup"><span data-stu-id="90c79-136">Misrepresented identities</span></span>
- <span data-ttu-id="90c79-137">初回の支払い前にプロビジョニングおよび使用されたサービス</span><span class="sxs-lookup"><span data-stu-id="90c79-137">Services provisioned and used before initial payment is received</span></span>
- <span data-ttu-id="90c79-138">オンライン不正アクセスのための新たな市場や危険度の高いリージョン</span><span class="sxs-lookup"><span data-stu-id="90c79-138">Emerging markets and/or high-risk regions for online fraud</span></span>
- <span data-ttu-id="90c79-139">不正なアクターによるアカウントの作成と購入を自動化する</span><span class="sxs-lookup"><span data-stu-id="90c79-139">Automate account creation and purchasing by bad actors</span></span>

## <a name="managing-online-risk"></a><span data-ttu-id="90c79-140">オンラインリスクの管理</span><span class="sxs-lookup"><span data-stu-id="90c79-140">Managing online risk</span></span>

<span data-ttu-id="90c79-141">次の推奨事項を使用すると、顧客関係のライフサイクルにおいてオンライントランザクションのリスクにさらされるリスクを軽減するためのポリシーとプラクティスを開発できます。</span><span class="sxs-lookup"><span data-stu-id="90c79-141">You can use the following recommendations to help you develop policies and practices to reduce your exposure to online transaction risks in the lifecycle of your customer relationships.</span></span>

### <a name="onboarding-new-customers"></a><span data-ttu-id="90c79-142">新しい顧客をオンボードする</span><span class="sxs-lookup"><span data-stu-id="90c79-142">Onboarding new customers</span></span>

<span data-ttu-id="90c79-143">新しい顧客をオンボードするときにオンラインリスクを軽減するための推奨事項は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="90c79-143">Suggestions for reducing online risks when onboarding new customers include:</span></span>

- <span data-ttu-id="90c79-144">可能な場合は、顧客との個人関係を確立します (たとえば、電話で顧客に連絡します)。</span><span class="sxs-lookup"><span data-stu-id="90c79-144">Establish personal relationships with customers when possible (for example, contacting customers by phone).</span></span>
- <span data-ttu-id="90c79-145">お客様の資格情報とバックグラウンドをより適切な方法 (クレジット機関やビジネスコマーシャルレポート機関を使用するなど) で検証します。</span><span class="sxs-lookup"><span data-stu-id="90c79-145">Verify customers' credentials and background through better methods (such as using credit bureaus or business commercial report agencies).</span></span>
- <span data-ttu-id="90c79-146">サインアップ時に multi-factor authentication (SMS の検証など) を使用して、ロボットアカウントの作成と購入の危険性を最小限に抑えます。</span><span class="sxs-lookup"><span data-stu-id="90c79-146">Use multi-factor authentication (such as SMS verification) during sign-up to minimize exposure to robotic account creation and purchasing.</span></span>
- <span data-ttu-id="90c79-147">サービス (デジタル id サービスなど) を使用して id を管理および追跡します。</span><span class="sxs-lookup"><span data-stu-id="90c79-147">Manage and track identities using services (such as digital identity services).</span></span>
- <span data-ttu-id="90c79-148">クレジットカード詐欺検出システムを使用して、顧客の財務力を評価します。</span><span class="sxs-lookup"><span data-stu-id="90c79-148">Assess customer financial strength through rigorous credit card fraud detection systems.</span></span>
- <span data-ttu-id="90c79-149">コレクションのクリアポリシーを確立します。</span><span class="sxs-lookup"><span data-stu-id="90c79-149">Establish a clear collections policy.</span></span> <span data-ttu-id="90c79-150">コレクションのプロセスを詳しく説明します。サブスクリプションへのアクセスは、支払いが行われないことによって影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="90c79-150">Detail your collections process and when access to subscriptions will be impacted by non-payment.</span></span> <span data-ttu-id="90c79-151">(アクセスを無効にしたり[、顧客のサブスクリプション](suspend-a-subscription.md)の支払いを中断したりすることができます)。</span><span class="sxs-lookup"><span data-stu-id="90c79-151">(You can disable access or [suspend a customer's subscriptions](suspend-a-subscription.md) for non-payment.)</span></span>

### <a name="managing-customer-accounts"></a><span data-ttu-id="90c79-152">顧客アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="90c79-152">Managing customer accounts</span></span>

<span data-ttu-id="90c79-153">購入後に顧客アカウントを管理するための推奨事項は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="90c79-153">Suggestions for managing customer accounts post-purchase include:</span></span>

- <span data-ttu-id="90c79-154">Microsoft 通知を迅速に受信、確認、操作、および対応するプロセスを実装します。</span><span class="sxs-lookup"><span data-stu-id="90c79-154">Implement a process to quickly receive, review, act on, and respond to Microsoft notifications.</span></span>
- <span data-ttu-id="90c79-155">お客様と協力して、クラウドの使用状況に関するビジネスニーズを把握し、設定に適切な監視しきい値を設定します。</span><span class="sxs-lookup"><span data-stu-id="90c79-155">Work with customers to understand their cloud usage business needs while settings appropriate monitoring thresholds.</span></span> <span data-ttu-id="90c79-156">(たとえば、パートナーセンターで[月単位の Azure 支出予算を設定](set-an-azure-spending-budget-for-your-customers.md)できます。</span><span class="sxs-lookup"><span data-stu-id="90c79-156">(For example, you can [set a monthly Azure spending budget](set-an-azure-spending-budget-for-your-customers.md) in Partner Center.</span></span> <span data-ttu-id="90c79-157">これにより、1か月の間に顧客の使用状況を監視し、顧客が予算に近づいたときに通知を受けることができます。)</span><span class="sxs-lookup"><span data-stu-id="90c79-157">This allows you to monitor customer usage during the month and be notified when customers are close to their budget.)</span></span>
- <span data-ttu-id="90c79-158">[顧客のアクティビティログ](activity-logs.md)を定期的に監視して、不正行為を早期に検出できるようにします。</span><span class="sxs-lookup"><span data-stu-id="90c79-158">Monitor [customer activity logs](activity-logs.md) regularly to help detect fraud early.</span></span>
- <span data-ttu-id="90c79-159">疑わしいアクティビティが検出されたときにクイックアクションを実行します。</span><span class="sxs-lookup"><span data-stu-id="90c79-159">Take quick action when suspicious activities are detected.</span></span>
- <span data-ttu-id="90c79-160">最初にリスク軽減制御を実装することなく、サブスクリプションへの完全な管理アクセス権を顧客に付与しないようにします。</span><span class="sxs-lookup"><span data-stu-id="90c79-160">Avoid giving customers full administrative access to subscriptions without first implementing risk mitigation controls.</span></span>

### <a name="managing-customer-billing"></a><span data-ttu-id="90c79-161">顧客の請求の管理</span><span class="sxs-lookup"><span data-stu-id="90c79-161">Managing customer billing</span></span>

<span data-ttu-id="90c79-162">購入後のお客様の課金を管理するための推奨事項は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="90c79-162">Suggestions for managing customer billing post-purchase include:</span></span>

- <span data-ttu-id="90c79-163">初期のトランザクションと課金の前に、前払いを要求します。</span><span class="sxs-lookup"><span data-stu-id="90c79-163">Request prepayments prior to initial transactions and billing .</span></span>
- <span data-ttu-id="90c79-164">高リスクの支払い方法 (プリペイドカードや格納済みの値のカードなど) は受け入れないでください。</span><span class="sxs-lookup"><span data-stu-id="90c79-164">Don't accept high-risk payment instruments (such as pre-paid cards or stored-value cards).</span></span>
- <span data-ttu-id="90c79-165">顧客の支払いと経時勘定科目の売掛金を監視します。</span><span class="sxs-lookup"><span data-stu-id="90c79-165">Monitor customer payments and aging accounts receivables.</span></span> <span data-ttu-id="90c79-166">遅延支払いまたは非支払いのために標準化された催促プロセスを積極的に適用します。</span><span class="sxs-lookup"><span data-stu-id="90c79-166">Aggressively enforce standardized dunning processes for late payments or non-payment.</span></span>

<span data-ttu-id="90c79-167">オンライン リスクを軽減するための詳しい方法については、[オンライン トランザクション リスクの管理ガイド](https://assets.windowsphone.com/7d885238-e13b-4f10-a682-3d5adacd2859/CSP-PartnerRiskGuide-APSFinal_InvariantCulture_Default.zip)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="90c79-167">For more detailed strategies for mitigating online risk, see the [Online transaction risk management guide.](https://assets.windowsphone.com/7d885238-e13b-4f10-a682-3d5adacd2859/CSP-PartnerRiskGuide-APSFinal_InvariantCulture_Default.zip)</span></span>
