---
title: 未払い、詐欺、不正使用の管理
description: オンライントランザクションに関係するさまざまなリスクと、パートナーセンターでこれらのリスクを管理および軽減するためのベストプラクティスについて説明します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: ba5fe60234c002ad2696de348a1b3b9b1284c149
ms.sourcegitcommit: eef446698ed4e21afee7fe091fe9c2664767755c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/01/2020
ms.locfileid: "89280596"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a><span data-ttu-id="ca567-103">パートナー センターでの未払い、詐欺、不正使用の管理</span><span class="sxs-lookup"><span data-stu-id="ca567-103">Managing non-payment, fraud, or misuse in Partner Center</span></span>

<span data-ttu-id="ca567-104">適用対象:</span><span class="sxs-lookup"><span data-stu-id="ca567-104">Applies to:</span></span>

- <span data-ttu-id="ca567-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="ca567-105">Partner Center</span></span>
- <span data-ttu-id="ca567-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="ca567-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="ca567-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="ca567-107">**Appropriate roles**</span></span>
- <span data-ttu-id="ca567-108">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="ca567-108">Global admin</span></span>
- <span data-ttu-id="ca567-109">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="ca567-109">User admin</span></span>
- <span data-ttu-id="ca567-110">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="ca567-110">Admin agent</span></span>
- <span data-ttu-id="ca567-111">課金管理者</span><span class="sxs-lookup"><span data-stu-id="ca567-111">Billing admin</span></span>

<span data-ttu-id="ca567-112">パートナーは、顧客による不正購入や、購入サービスの料金未払いについて、金銭的な責任を負います。</span><span class="sxs-lookup"><span data-stu-id="ca567-112">You are financially responsible for fraudulent purchases by your customers and/or customers' non-payment of purchased services.</span></span> <span data-ttu-id="ca567-113">したがって、 *不正行為の防止と検出のリスク軽減のための制御*を行うことを強くお勧めします。</span><span class="sxs-lookup"><span data-stu-id="ca567-113">Therefore, *we strongly recommend that you put in place fraud prevention and detection risk mitigation controls*.</span></span>

<span data-ttu-id="ca567-114">不正行為や不正使用を回避したり、これらに対処するには、潜在的なリスクを理解して、リスクへの露出を軽減するためのポリシーとプラクティスを作成することが重要です。</span><span class="sxs-lookup"><span data-stu-id="ca567-114">To avoid and/or address fraudulent activity or misuse, it's important to understand potential risks and to develop policies and practices that can reduce your exposure.</span></span>

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a><span data-ttu-id="ca567-115">Microsoft による利用規約の適用</span><span class="sxs-lookup"><span data-stu-id="ca567-115">Enforcement of Microsoft Acceptable Use Policy</span></span>

<span data-ttu-id="ca567-116">許容される使用ポリシーに違反しているかどうかを確認するパートナーまたは顧客のアクティビティを Microsoft が検出した場合は、実施手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="ca567-116">If Microsoft detects partner or customer activity that we confirm or suspect violates the Acceptable Use Policy, we will take enforcement steps.</span></span> <span data-ttu-id="ca567-117">顧客はすぐに中断される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ca567-117">The customer could be immediately suspended.</span></span> <span data-ttu-id="ca567-118">Microsoft からの要求に対して、実施アクションまたは更新が通知されます。</span><span class="sxs-lookup"><span data-stu-id="ca567-118">You'll be notified of enforcement actions or updated on your requests by Microsoft.</span></span>

## <a name="abuse-of-service-risks"></a><span data-ttu-id="ca567-119">サービスリスクの悪用</span><span class="sxs-lookup"><span data-stu-id="ca567-119">Abuse of service risks</span></span>

<span data-ttu-id="ca567-120">**サービスのリスクを悪用** すると、クラウドサービスを使用するお客様は、マイクロソフトの利用規約に違反することになります。</span><span class="sxs-lookup"><span data-stu-id="ca567-120">**Abuse of service** risks means customers who use cloud services in violation of Microsoft's Acceptable Use Policy.</span></span>

### <a name="examples-of-abuse-of-service"></a><span data-ttu-id="ca567-121">サービスの悪用の例</span><span class="sxs-lookup"><span data-stu-id="ca567-121">Examples of abuse of service</span></span>

<span data-ttu-id="ca567-122">Microsoft の利用規約に違反する例として、次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="ca567-122">Examples of these violations of Microsoft's acceptable use policy can include:</span></span>

- <span data-ttu-id="ca567-123">スパム</span><span class="sxs-lookup"><span data-stu-id="ca567-123">Spamming</span></span>
- <span data-ttu-id="ca567-124">ハッキング</span><span class="sxs-lookup"><span data-stu-id="ca567-124">Hacking</span></span>
- <span data-ttu-id="ca567-125">分散型サービス拒否 (DDoS) 攻撃</span><span class="sxs-lookup"><span data-stu-id="ca567-125">Distributed denial-of-service (DDoS) attacks</span></span>
- <span data-ttu-id="ca567-126">ビットコイン マイニング</span><span class="sxs-lookup"><span data-stu-id="ca567-126">Bitcoin mining</span></span>
- <span data-ttu-id="ca567-127">マルウェアの配布</span><span class="sxs-lookup"><span data-stu-id="ca567-127">Malware distribution</span></span>
- <span data-ttu-id="ca567-128">偽造されたサブスクリプションの再販</span><span class="sxs-lookup"><span data-stu-id="ca567-128">Resale of pirated subscriptions</span></span>

## <a name="theft-of-service-risks"></a><span data-ttu-id="ca567-129">サービスリスクの盗難</span><span class="sxs-lookup"><span data-stu-id="ca567-129">Theft of service risks</span></span>

<span data-ttu-id="ca567-130">**サービスリスクの盗難** は、消費されたサービスに対して支払いを行うことがないお客様を意味します。</span><span class="sxs-lookup"><span data-stu-id="ca567-130">**Theft of service** risks means customers who have no intention of paying for consumed services.</span></span> <span data-ttu-id="ca567-131">この盗難には、盗まれた支払い方法の使用、誤請求情報の提供、または未払い残高の既定値の使用が含まれる場合があります。</span><span class="sxs-lookup"><span data-stu-id="ca567-131">This theft may involve using stolen payment instruments, providing false billing information, and/or defaulting on outstanding balances.</span></span>

### <a name="examples-of-service-theft"></a><span data-ttu-id="ca567-132">サービスの盗難の例</span><span class="sxs-lookup"><span data-stu-id="ca567-132">Examples of service theft</span></span>

<span data-ttu-id="ca567-133">オンライントランザクションのリスクの例としては、次のようなものがあります。</span><span class="sxs-lookup"><span data-stu-id="ca567-133">Examples of these online transaction risks can include:</span></span>

- <span data-ttu-id="ca567-134">担当者では発生しないトランザクション ("クレジットカードが存在しません" トランザクション)</span><span class="sxs-lookup"><span data-stu-id="ca567-134">Transactions that don't occur in person ("credit card not present" transactions)</span></span>
- <span data-ttu-id="ca567-135">ID の不正使用</span><span class="sxs-lookup"><span data-stu-id="ca567-135">Misrepresented identities</span></span>
- <span data-ttu-id="ca567-136">初回の支払い前にプロビジョニングおよび使用されたサービス</span><span class="sxs-lookup"><span data-stu-id="ca567-136">Services provisioned and used before initial payment is received</span></span>
- <span data-ttu-id="ca567-137">オンライン不正アクセスのための新たな市場や危険度の高いリージョン</span><span class="sxs-lookup"><span data-stu-id="ca567-137">Emerging markets and/or high-risk regions for online fraud</span></span>
- <span data-ttu-id="ca567-138">不正なアクターによるアカウントの作成と購入を自動化する</span><span class="sxs-lookup"><span data-stu-id="ca567-138">Automate account creation and purchasing by bad actors</span></span>

## <a name="managing-online-risk"></a><span data-ttu-id="ca567-139">オンラインリスクの管理</span><span class="sxs-lookup"><span data-stu-id="ca567-139">Managing online risk</span></span>

<span data-ttu-id="ca567-140">次の推奨事項を使用すると、顧客関係のライフサイクルにおいてオンライントランザクションのリスクにさらされるリスクを軽減するためのポリシーとプラクティスを開発できます。</span><span class="sxs-lookup"><span data-stu-id="ca567-140">You can use the following recommendations to help you develop policies and practices to reduce your exposure to online transaction risks in the lifecycle of your customer relationships.</span></span>

### <a name="onboarding-new-customers"></a><span data-ttu-id="ca567-141">新しい顧客をオンボードする</span><span class="sxs-lookup"><span data-stu-id="ca567-141">Onboarding new customers</span></span>

<span data-ttu-id="ca567-142">新しい顧客をオンボードするときにオンラインリスクを軽減するための推奨事項は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ca567-142">Suggestions for reducing online risks when onboarding new customers include:</span></span>

- <span data-ttu-id="ca567-143">可能な場合は、顧客との個人関係を確立します (たとえば、電話で顧客に連絡します)。</span><span class="sxs-lookup"><span data-stu-id="ca567-143">Establish personal relationships with customers when possible (for example, contacting customers by phone).</span></span>
- <span data-ttu-id="ca567-144">お客様の資格情報とバックグラウンドをより適切な方法 (クレジット機関やビジネスコマーシャルレポート機関を使用するなど) で検証します。</span><span class="sxs-lookup"><span data-stu-id="ca567-144">Verify customers' credentials and background through better methods (such as using credit bureaus or business commercial report agencies).</span></span>
- <span data-ttu-id="ca567-145">サインアップ時に multi-factor authentication (SMS の検証など) を使用して、ロボットアカウントの作成と購入の危険性を最小限に抑えます。</span><span class="sxs-lookup"><span data-stu-id="ca567-145">Use multi-factor authentication (such as SMS verification) during sign-up to minimize exposure to robotic account creation and purchasing.</span></span>
- <span data-ttu-id="ca567-146">サービス (デジタル id サービスなど) を使用して id を管理および追跡します。</span><span class="sxs-lookup"><span data-stu-id="ca567-146">Manage and track identities using services (such as digital identity services).</span></span>
- <span data-ttu-id="ca567-147">クレジットカード詐欺検出システムを使用して、顧客の財務力を評価します。</span><span class="sxs-lookup"><span data-stu-id="ca567-147">Assess customer financial strength through rigorous credit card fraud detection systems.</span></span>
- <span data-ttu-id="ca567-148">コレクションのクリアポリシーを確立します。</span><span class="sxs-lookup"><span data-stu-id="ca567-148">Establish a clear collections policy.</span></span> <span data-ttu-id="ca567-149">コレクションのプロセスを詳しく説明します。サブスクリプションへのアクセスは、支払いが行われないことによって影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="ca567-149">Detail your collections process and when access to subscriptions will be impacted by non-payment.</span></span> <span data-ttu-id="ca567-150">(アクセスを無効にしたり [、顧客のサブスクリプション](suspend-a-subscription.md) の支払いを中断したりすることができます)。</span><span class="sxs-lookup"><span data-stu-id="ca567-150">(You can disable access or [suspend a customer's subscriptions](suspend-a-subscription.md) for non-payment.)</span></span>

### <a name="managing-customer-accounts"></a><span data-ttu-id="ca567-151">顧客アカウントの管理</span><span class="sxs-lookup"><span data-stu-id="ca567-151">Managing customer accounts</span></span>

<span data-ttu-id="ca567-152">購入後に顧客アカウントを管理するための推奨事項は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ca567-152">Suggestions for managing customer accounts post-purchase include:</span></span>

- <span data-ttu-id="ca567-153">Microsoft 通知を迅速に受信、確認、操作、および対応するプロセスを実装します。</span><span class="sxs-lookup"><span data-stu-id="ca567-153">Implement a process to quickly receive, review, act on, and respond to Microsoft notifications.</span></span>
- <span data-ttu-id="ca567-154">お客様と協力して、クラウドの使用状況に関するビジネスニーズを把握し、設定に適切な監視しきい値を設定します。</span><span class="sxs-lookup"><span data-stu-id="ca567-154">Work with customers to understand their cloud usage business needs while settings appropriate monitoring thresholds.</span></span> <span data-ttu-id="ca567-155">(たとえば、パートナーセンターで [月単位の Azure 支出予算を設定](set-an-azure-spending-budget-for-your-customers.md) できます。</span><span class="sxs-lookup"><span data-stu-id="ca567-155">(For example, you can [set a monthly Azure spending budget](set-an-azure-spending-budget-for-your-customers.md) in Partner Center.</span></span> <span data-ttu-id="ca567-156">このことを理解することで、1か月の間に顧客の使用状況を監視し、顧客が予算に近づいたときに通知を受けることができます。)</span><span class="sxs-lookup"><span data-stu-id="ca567-156">This understanding allows you to monitor customer usage during the month and be notified when customers are close to their budget.)</span></span>
- <span data-ttu-id="ca567-157">[顧客のアクティビティログ](activity-logs.md)を定期的に監視して、不正行為を早期に検出できるようにします。</span><span class="sxs-lookup"><span data-stu-id="ca567-157">Monitor [customer activity logs](activity-logs.md) regularly to help detect fraud early.</span></span>
- <span data-ttu-id="ca567-158">疑わしいアクティビティが検出されたときにクイックアクションを実行します。</span><span class="sxs-lookup"><span data-stu-id="ca567-158">Take quick action when suspicious activities are detected.</span></span>
- <span data-ttu-id="ca567-159">最初にリスク軽減制御を実装することなく、サブスクリプションへの完全な管理アクセス権を顧客に付与しないようにします。</span><span class="sxs-lookup"><span data-stu-id="ca567-159">Avoid giving customers full administrative access to subscriptions without first implementing risk mitigation controls.</span></span>

### <a name="managing-customer-billing"></a><span data-ttu-id="ca567-160">顧客の請求の管理</span><span class="sxs-lookup"><span data-stu-id="ca567-160">Managing customer billing</span></span>

<span data-ttu-id="ca567-161">購入後のお客様の課金を管理するための推奨事項は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ca567-161">Suggestions for managing customer billing post-purchase include:</span></span>

- <span data-ttu-id="ca567-162">初期のトランザクションと課金の前に、前払いを要求します。</span><span class="sxs-lookup"><span data-stu-id="ca567-162">Request prepayments prior to initial transactions and billing.</span></span>
- <span data-ttu-id="ca567-163">高リスクの支払い方法 (プリペイドカードや格納済みの値のカードなど) は受け入れないでください。</span><span class="sxs-lookup"><span data-stu-id="ca567-163">Don't accept high-risk payment instruments (such as pre-paid cards or stored-value cards).</span></span>
- <span data-ttu-id="ca567-164">顧客の支払いと経時勘定科目の売掛金を監視します。</span><span class="sxs-lookup"><span data-stu-id="ca567-164">Monitor customer payments and aging accounts receivables.</span></span> <span data-ttu-id="ca567-165">遅延支払いまたは非支払いのために標準化された催促プロセスを積極的に適用します。</span><span class="sxs-lookup"><span data-stu-id="ca567-165">Aggressively enforce standardized dunning processes for late payments or non-payment.</span></span>

<span data-ttu-id="ca567-166">オンライン リスクを軽減するための詳しい方法については、[オンライン トランザクション リスクの管理ガイド](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="ca567-166">For more detailed strategies for mitigating online risk, see the [Online transaction risk management guide.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)</span></span>
