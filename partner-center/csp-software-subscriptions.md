---
title: CSP によるソフトウェア サブスクリプションの販売 |パートナー センター
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: CSP プログラムのパートナーがパートナーセンターを使用して、Azure 予約インスタンスと顧客のサーバーサブスクリプションを購入、管理、販売、キャンセルする方法について説明します。
author: MaggiePucciEvans
ms.author: evansma
keywords: クラウド ソリューション プロバイダー, CSP, クラウド ベースのサービス, Azure, Azure RI, Windows Server, SQL Server, ソフトウェア サブスクリプション
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 0e2b735c1b67b49c18f2b83c042ec5a2bb0eefbd
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721337"
---
# <a name="sell-software-subscriptions-through-csp"></a><span data-ttu-id="a2ecd-104">CSP によるソフトウェア サブスクリプションの販売</span><span class="sxs-lookup"><span data-stu-id="a2ecd-104">Sell software subscriptions through CSP</span></span>

<span data-ttu-id="a2ecd-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="a2ecd-105">**Appropriate roles**</span></span>

- <span data-ttu-id="a2ecd-106">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="a2ecd-106">Admin agent</span></span>
- <span data-ttu-id="a2ecd-107">グローバル管理</span><span class="sxs-lookup"><span data-stu-id="a2ecd-107">Global admin</span></span>

<span data-ttu-id="a2ecd-108">Azure の予約とサーバーサブスクリプション (Windows Server および SQL Server サブスクリプション) を使用すると、CSP プログラムのパートナーは、高度な予測可能性と持続性をサポートするためのコスト効率に優れたソリューションを実現するために、急速に成長する顧客の需要に対応することができます。クラウドワークロード。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-108">With Azure reservations and Server subscriptions (Windows Server and SQL Server subscriptions), partners in the CSP program can better address the fast-growing customer demand for more cost-effective solutions to support highly predictable and persistent cloud workloads.</span></span> 

<span data-ttu-id="a2ecd-109">Azure ハイブリッド特典を利用して、パートナーセンターと Azure ポータルを使用して、商用顧客に代わって Azure 予約とサーバーサブスクリプションを取得、プロビジョニング、および管理できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-109">You can now acquire, provision, and manage Azure reservations and Server subscriptions on behalf of commercial customers through Partner Center and the Azure Portal by taking advantage of the Azure Hybrid Benefit.</span></span> 

<span data-ttu-id="a2ecd-110">Azure ハイブリッド特典を利用すると、Windows Server ライセンスから得られる価値を拡大し、仮想マシンのコストを最大で 40% 節約できます。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-110">The Azure Hybrid Benefit helps you get more value from your Windows Server licenses and save up to 40 percent on virtual machines.</span></span> <span data-ttu-id="a2ecd-111">この特典はソフトウェア アシュアランスに含まれており、Windows Server Datacenter および Standard エディションのライセンスで利用できます。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-111">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="a2ecd-112">エディションによっては、ライセンスを変換または再利用して、低いベース コンピューティング レート (Linux 仮想マシン レーなどト) で Windows Server 仮想マシンを Azure で実行できます。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-112">Depending on the edition, you can convert or re-use your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates, e.g.).</span></span>

> [!NOTE]  
> <span data-ttu-id="a2ecd-113">次の市場では Azure Reservations を利用できません。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-113">Azure reservations are not available in the following markets:</span></span>  
> * <span data-ttu-id="a2ecd-114">アルゼンチン</span><span class="sxs-lookup"><span data-stu-id="a2ecd-114">Argentina</span></span>
> * <span data-ttu-id="a2ecd-115">ブラジル</span><span class="sxs-lookup"><span data-stu-id="a2ecd-115">Brazil</span></span>
> * <span data-ttu-id="a2ecd-116">中国</span><span class="sxs-lookup"><span data-stu-id="a2ecd-116">China</span></span>
> * <span data-ttu-id="a2ecd-117">インドネシア</span><span class="sxs-lookup"><span data-stu-id="a2ecd-117">Indonesia</span></span>
> * <span data-ttu-id="a2ecd-118">リヒテンシュタイン</span><span class="sxs-lookup"><span data-stu-id="a2ecd-118">Liechtenstein</span></span>
> * <span data-ttu-id="a2ecd-119">ジャージー島</span><span class="sxs-lookup"><span data-stu-id="a2ecd-119">Jersey</span></span>
> * <span data-ttu-id="a2ecd-120">マレーシア</span><span class="sxs-lookup"><span data-stu-id="a2ecd-120">Malaysia</span></span>
> * <span data-ttu-id="a2ecd-121">メキシコ</span><span class="sxs-lookup"><span data-stu-id="a2ecd-121">Mexico</span></span>
> * <span data-ttu-id="a2ecd-122">ロシア連邦</span><span class="sxs-lookup"><span data-stu-id="a2ecd-122">Russia</span></span>
> * <span data-ttu-id="a2ecd-123">サウジアラビア</span><span class="sxs-lookup"><span data-stu-id="a2ecd-123">Saudi Arabia</span></span>
> * <span data-ttu-id="a2ecd-124">南アフリカ</span><span class="sxs-lookup"><span data-stu-id="a2ecd-124">South Africa</span></span>
> * <span data-ttu-id="a2ecd-125">トルコ</span><span class="sxs-lookup"><span data-stu-id="a2ecd-125">Turkey</span></span>

<!--March 20, 2019 - this list of countries was correct as of today. Maggie last updated the list according to FAREAST\v-pubobb in bug 20907186.
-->

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a><span data-ttu-id="a2ecd-126">顧客に代わってソフトウェア サブスクリプションを購入する</span><span class="sxs-lookup"><span data-stu-id="a2ecd-126">Buy software subscriptions on behalf of customers</span></span>

<span data-ttu-id="a2ecd-127">顧客の代わりにソフトウェア サブスクリプションを購入するには、顧客の詳細ページに移動し、 **[製品の追加]** を選択します。次に、画面の指示に従って注文を作成して支払います。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-127">To buy software subscriptions on behalf of a customer, go to the customer's detail page, select **Add products**, and then follow the on-screen instructions to create and pay for your order.</span></span> <span data-ttu-id="a2ecd-128">オーストラリアとブラジルを除き、すべての商用顧客向け価格には税は含まれません。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-128">All commercial pricing excludes tax with the exception of Australia and Brazil.</span></span> <span data-ttu-id="a2ecd-129">オーストラリアとブラジルの場合は、価格に税が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-129">For Australia and Brazil, the price includes tax.</span></span>

## <a name="activate-and-manage-software-subscriptions"></a><span data-ttu-id="a2ecd-130">ソフトウェア サブスクリプションのライセンス認証と管理</span><span class="sxs-lookup"><span data-stu-id="a2ecd-130">Activate and manage software subscriptions</span></span>

<span data-ttu-id="a2ecd-131">ソフトウェア サブスクリプションを購入した後は、次の手順に従ってダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-131">After you purchase the software subscription, follow the steps below to download it.</span></span>

>[!NOTE]
><span data-ttu-id="a2ecd-132">ソフトウェアをダウンロードしてライセンス認証キーを取得するには、管理エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-132">You must be an Admin agent to download software and get activation keys.</span></span>

1. <span data-ttu-id="a2ecd-133">顧客の詳細ページに移動し、 **[ソフトウェア]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-133">Go to your customer's detail page and then select **Software**.</span></span> <span data-ttu-id="a2ecd-134">お客様の代わりに購入したすべてのソフトウェアの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-134">You'll see a list of all the software you've purchased on behalf of the customer.</span></span> 
2.  <span data-ttu-id="a2ecd-135">ダウンロードする製品を展開します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-135">Expand the product you want to download.</span></span> <span data-ttu-id="a2ecd-136">**[製品の選択]** フィールドで、目的の **[バージョン]** 、 **[言語]** 、 **[ファイルの種類/OS]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-136">In the **Select product** field, select the **Version**, **Language**, and **File type/OS** that you want.</span></span> 
3.  <span data-ttu-id="a2ecd-137">**[送信]** 選択して特定の製品を表示します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-137">Select **Submit** to display the specific products.</span></span> 
4.  <span data-ttu-id="a2ecd-138">**[キーとダウンロードの取得]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-138">Select **Get keys and downloads**.</span></span> 
5.  <span data-ttu-id="a2ecd-139">**[ダウンロード]** を選択してダウンロードを開始するか、 **[リンクのコピー]** を選択してリンクをコピーし、顧客に送信します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-139">Select **Download** to begin downloading, or select **Copy link** to copy the link and send it to the customer.</span></span> 

>[!NOTE]
><span data-ttu-id="a2ecd-140">このリンクは、2 週間後または 50 回のダウンロードのどちらか早い方のタイミングで期限切れになります。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-140">This link will expire after two weeks or 50 downloads, whichever comes first.</span></span> <span data-ttu-id="a2ecd-141">リンクが期限切れになった場合は、このページに戻り、 **[キーとダウンロードの取得]** をもう一度選択して、2 週間または 50 回のダウンロードを再び有効にします。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-141">Once the link expires, return to this page and select **Get keys and downloads** again to enable another two weeks or 50 downloads.</span></span> <span data-ttu-id="a2ecd-142">この操作は、必要な回数だけ行うことができます。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-142">You can do this as many times as you need to.</span></span> 

## <a name="view-activity-for-software-key-access-and-software-downloads"></a><span data-ttu-id="a2ecd-143">ソフトウェアキーのアクセスおよびソフトウェアのダウンロードの利用状況を表示する</span><span class="sxs-lookup"><span data-stu-id="a2ecd-143">View activity for software key access and software downloads</span></span>
<span data-ttu-id="a2ecd-144">監査またはコンプライアンスの目的で、サーバーサブスクリプションのソフトウェアキーまたはダウンロードされたサーバーサブスクリプションソフトウェアにアクセスしたユーザーの一覧を確認する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-144">For auditing or compliance purposes, you may need to check a list of users who have either accessed Server subscription software keys or downloaded Server subscription software.</span></span> <span data-ttu-id="a2ecd-145">この情報にアクセスするには、以下の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-145">Use the procedure below to access this information.</span></span> 

>[!NOTE]
><span data-ttu-id="a2ecd-146">これらのアクティビティログを表示するには、グローバル管理者、アカウント管理者、参照管理者、またはマーケティングコンテンツ管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-146">You must be a Global administrator, Account admin, Referral admin, or Marketing content admin to see these activity logs.</span></span> 

1.  <span data-ttu-id="a2ecd-147">パートナーセンターで、右上隅にある歯車アイコンを選択します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-147">In Partner Center, select the gear icon from the upper right corner.</span></span> 
2.  <span data-ttu-id="a2ecd-148">メニューで **[アクティビティログ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-148">In the menu, select **Activity log**.</span></span>
3.  <span data-ttu-id="a2ecd-149">表示する活動の日付範囲を入力します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-149">Enter the date range for the activity you want to see.</span></span> <span data-ttu-id="a2ecd-150">[アクティビティログ] には、指定した期間にソフトウェアキーまたはダウンロードしたソフトウェアにアクセスしたユーザーの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-150">The activity log will display a list of users who have either accessed software keys or downloaded software during the time you specified.</span></span> 

## <a name="cancel-a-purchase"></a><span data-ttu-id="a2ecd-151">購入を取り消す</span><span class="sxs-lookup"><span data-stu-id="a2ecd-151">Cancel a purchase</span></span>

<span data-ttu-id="a2ecd-152">購入日から 60 日以内であればソフトウェア購入を取り消すことができます。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-152">You can cancel a software purchase within 60 days of the purchase date.</span></span> <span data-ttu-id="a2ecd-153">中途解約料金は発生しませんが、購入日から 60 日を過ぎた後は購入をキャンセルできません。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-153">Microsoft does not charge an early termination fee, however, you can't cancel a purchase after 60 days from the purchase date.</span></span>

<span data-ttu-id="a2ecd-154">購入をキャンセルした後は、ソフトウェア キーが取り消されます。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-154">After you cancel the purchase, the software key will be revoked.</span></span> 

<span data-ttu-id="a2ecd-155">購入をキャンセルするには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-155">Follow the steps below to cancel a purchase:</span></span>

>[!NOTE]
><span data-ttu-id="a2ecd-156">購入を取り消すには、管理エージェントである必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-156">You must be an Admin agent to cancel a purchase.</span></span> 

1.  <span data-ttu-id="a2ecd-157">プロセスを開始する前に、次の情報がそろっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-157">Before beginning the process, make sure you have the following:</span></span>
    -   <span data-ttu-id="a2ecd-158">顧客のテナント GUID またはドメイン名</span><span class="sxs-lookup"><span data-stu-id="a2ecd-158">The customer tenant GUID or domain name</span></span>
    -   <span data-ttu-id="a2ecd-159">注文 ID またはサブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="a2ecd-159">Order ID or Subscription ID</span></span>
    -   <span data-ttu-id="a2ecd-160">払い戻し理由</span><span class="sxs-lookup"><span data-stu-id="a2ecd-160">Refund reason</span></span>
    -   <span data-ttu-id="a2ecd-161">要求された数量</span><span class="sxs-lookup"><span data-stu-id="a2ecd-161">Amount requested</span></span>

2.  <span data-ttu-id="a2ecd-162">顧客の詳細ページで、 **[ソフトウェア]** を選択して、顧客用に購入したすべてのソフトウェアの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-162">On the customer's details page, select **Software** to see the list of all the software you've purchased for the customer.</span></span> 

3.  <span data-ttu-id="a2ecd-163">取り消すソフトウェアを検索し、 **[キャンセル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-163">Locate the software you want to cancel, and then select **Cancel**.</span></span> <span data-ttu-id="a2ecd-164">**[パートナー センターに関する問題を報告する]** ページが開きます。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-164">The **Report a problem with Partner Center** page opens.</span></span> 

4.  <span data-ttu-id="a2ecd-165">**[詳細]** の **[問題の種類]** の一覧で、 **[お客様に代わって CSP を購入/払い戻し]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-165">Under **Details**, in the **Type of problem** list, select **CSP Purchase/Refund on behalf of customers**.</span></span>

5.  <span data-ttu-id="a2ecd-166">**[影響]** と **[タイトル]** フィールドに入力します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-166">Fill in the **Impact** and **Title** fields.</span></span> 

6.  <span data-ttu-id="a2ecd-167">**[説明]** フィールドに、以下の情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-167">In the **Description** field, provide the following:</span></span> 
    -   <span data-ttu-id="a2ecd-168">顧客のテナント GUID またはドメイン名</span><span class="sxs-lookup"><span data-stu-id="a2ecd-168">The customer tenant GUID or domain name</span></span>
    -   <span data-ttu-id="a2ecd-169">注文 ID またはサブスクリプション ID</span><span class="sxs-lookup"><span data-stu-id="a2ecd-169">Order ID or Subscription ID</span></span>
    -   <span data-ttu-id="a2ecd-170">払い戻し理由</span><span class="sxs-lookup"><span data-stu-id="a2ecd-170">Refund reason</span></span>
    -   <span data-ttu-id="a2ecd-171">要求された数量</span><span class="sxs-lookup"><span data-stu-id="a2ecd-171">Amount requested</span></span>

7.  <span data-ttu-id="a2ecd-172">**[連絡先]** フィールドに、パートナーの名前、メール アドレス、電話番号を入力します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-172">In the **Contact** field, enter your name, email address, and phone number.</span></span> 

8.  <span data-ttu-id="a2ecd-173">何らかの理由でファイルを添付する必要がある場合は、 **[ファイルの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-173">If you need to attach a file for any reason, select **Add files**.</span></span> <span data-ttu-id="a2ecd-174">この手順は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-174">This step is optional.</span></span> 

9.  <span data-ttu-id="a2ecd-175">終了したら、 **[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a2ecd-175">When you're finished, select **Submit**.</span></span>
