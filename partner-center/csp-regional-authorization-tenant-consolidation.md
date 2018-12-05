---
title: CSP の地域的承認によるテナント統合 | パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: 別の国/地域のテナントを統合するには、次の手順を使用します。
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.author: evansma
keywords: 顧客の移行, プロビジョニング, テナントのアカウント, テナントの統合
ms.localizationpriority: medium
ms.openlocfilehash: 83b5040f1562ef44c5cb17b5a2676387237b2794
ms.sourcegitcommit: d3613d23bd177a53381ebf32b4f1075201f8f7f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/05/2018
ms.locfileid: "8683801"
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="a5986-104">CSP の地域的承認によるテナント統合</span><span class="sxs-lookup"><span data-stu-id="a5986-104">CSP regional authorization tenant consolidation</span></span>

**<span data-ttu-id="a5986-105">適用対象</span><span class="sxs-lookup"><span data-stu-id="a5986-105">Applies to</span></span>**

-  <span data-ttu-id="a5986-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="a5986-106">Partner Center</span></span>
-  <span data-ttu-id="a5986-107">Microsoft Cloud for US Government のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="a5986-107">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="a5986-108">\[一部の情報はリリース前の製品に関することであり、正式版がリリースされるまでに大幅に変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a5986-108">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="a5986-109">ここに記載された情報について、Microsoft は明示または黙示を問わずいかなる保証をするものでもありません。\]</span><span class="sxs-lookup"><span data-stu-id="a5986-109">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="a5986-110">別の国/地域のテナントを統合するには、次の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="a5986-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="a5986-111">**注:** すべてのサブスクリプションを認識する必要があり、切り替えアカウントからプロビジョニングされた顧客用のシート数します。</span><span class="sxs-lookup"><span data-stu-id="a5986-111">**Note**You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="a5986-112">移行プロセスの一環として、新しい一元化された CSP アカウントで、まったく同じサブスクリプションを同じシート数で再プロビジョニングします。</span><span class="sxs-lookup"><span data-stu-id="a5986-112">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="a5986-113">エクスポート リスト機能を使用すると、一元化されたテナントに移動する顧客の一覧の作成に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="a5986-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="a5986-114">パートナーは、テナントを統合することを選択します。</span><span class="sxs-lookup"><span data-stu-id="a5986-114">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="a5986-115">統合が完了すると、パートナーは、以前の状態に戻すことはできません。</span><span class="sxs-lookup"><span data-stu-id="a5986-115">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="a5986-116">顧客のアクションも必要になる可能性があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="a5986-116">Note that customer action may also be required.</span></span>

 

## <a name="prepare-for-migration"></a><span data-ttu-id="a5986-117">移行を準備する</span><span class="sxs-lookup"><span data-stu-id="a5986-117">Prepare for migration</span></span>


-   <span data-ttu-id="a5986-118">**移行元**(既存の) アカウント (移行は 1 つ) を使用して、**パートナー センター**にサインインし、すべての顧客とのすべてのそれらのユーザー用にプロビジョニング サービスを書き留めます。</span><span class="sxs-lookup"><span data-stu-id="a5986-118">Sign in to your **Partner Center**  with the **Transitioning** (existing) account (the one you will transition)  and take note of all customers and all of the services provisioned for those customers.</span></span>

![地域の顧客の一覧](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="a5986-120">顧客アカウントを移行する</span><span class="sxs-lookup"><span data-stu-id="a5986-120">Migrate customer accounts</span></span>


1.  <span data-ttu-id="a5986-121">**移行元**(新規) アカウント (先もの) を使用して、**パートナー センター**にサインインし、**お客様**から、顧客の一覧に移動します。</span><span class="sxs-lookup"><span data-stu-id="a5986-121">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2.  <span data-ttu-id="a5986-122">[顧客] を選びます。</span><span class="sxs-lookup"><span data-stu-id="a5986-122">Select Customers.</span></span>

3.  <span data-ttu-id="a5986-123">**[再販業者関係の要求]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a5986-123">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="a5986-124">顧客に表示する既定のメール メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="a5986-124">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="a5986-125">このメッセージには、新しいパートナー センター アカウントに対して一意の URL と組織 ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a5986-125">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="a5986-126">**顧客のアクション:** 移行したいアクティブな各顧客がこの URL にアクセスしたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="a5986-126">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="a5986-127">この URL を開くと、顧客は、Office 365 ポータルにサインインするよう求められます。</span><span class="sxs-lookup"><span data-stu-id="a5986-127">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="a5986-128">顧客は、Azure や Office 365 管理ポータルにアクセスするために使用する組織 ID と同じ組織 ID を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="a5986-128">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="a5986-129">サインインした後、顧客アカウントのグローバル管理者は、新しい CSP アカウントに委任された管理者特権を与えるという契約を提出するよう求められます。</span><span class="sxs-lookup"><span data-stu-id="a5986-129">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="a5986-130">契約書に同意する場合、顧客はチェック ボックスをオンにして、関係を承認することに同意します。</span><span class="sxs-lookup"><span data-stu-id="a5986-130">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="a5986-131">顧客が契約書を送信すると、パートナーの顧客の一覧に、1 つずつ表示されます。</span><span class="sxs-lookup"><span data-stu-id="a5986-131">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="a5986-132">Office 365 および Azure 以外の使用量ベースのサブスクリプションを移行する</span><span class="sxs-lookup"><span data-stu-id="a5986-132">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="a5986-133">顧客が契約書に署名すると、パートナーは、一元化されたパートナー テナントでサブスクリプションを再作成できます。</span><span class="sxs-lookup"><span data-stu-id="a5986-133">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="a5986-134">**パートナー センター**から**顧客**を選びます。</span><span class="sxs-lookup"><span data-stu-id="a5986-134">From the **Partner Center** select **Customers**.</span></span>

3.  <span data-ttu-id="a5986-135">移行する顧客の会社名を開きます。</span><span class="sxs-lookup"><span data-stu-id="a5986-135">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="a5986-136">**[サブスクリプションの追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a5986-136">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="a5986-137">カタログから適切なサブスクリプションとシート数を追加します。</span><span class="sxs-lookup"><span data-stu-id="a5986-137">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="a5986-138">**移行元**のパートナー アカウントに表示されている情報を確認します。</span><span class="sxs-lookup"><span data-stu-id="a5986-138">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

    ![顧客一覧のスクリーンショット](images/regionalcustomer2.png)

6.  <span data-ttu-id="a5986-140">**[送信]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a5986-140">Click **Submit.**</span></span>

<span data-ttu-id="a5986-141">これでサービスは、**移行先**のパートナー アカウントから顧客に提供されるようになります。</span><span class="sxs-lookup"><span data-stu-id="a5986-141">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="a5986-142">その他のすべての顧客のサブスクリプションを移行するには、この手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="a5986-142">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="a5986-143">次のセクションに進む前に、**移行元**のパートナー アカウントに存在しているすべての顧客のサブスクリプションが、**移行先**のパートナー アカウントで再プロビジョニングされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a5986-143">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="a5986-144">**注:** パートナーする必要がありますサブスクリプションを中断パートナー センターで**移行元**のパートナー テナント アカウントでそれらのサブスクリプションを移行してで**移行先**パートナー テナント アカウントで設定した同じ日パートナー センターを二重請求は発生しません。</span><span class="sxs-lookup"><span data-stu-id="a5986-144">**Note**Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="a5986-145">**移行元**のサブスクリプションが正しく無効に設定されていない場合、請求の重複のために、クレジットのサポート要求が拒否されます。</span><span class="sxs-lookup"><span data-stu-id="a5986-145">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="a5986-146">移行元のパートナー アカウントで Office 365 のサブスクリプションを無効にする</span><span class="sxs-lookup"><span data-stu-id="a5986-146">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="a5986-147">**移行元**のパートナー アカウントで CSP サブスクリプションを無効にすると、それ以降の請求は停止されます。</span><span class="sxs-lookup"><span data-stu-id="a5986-147">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="a5986-148">Azure サブスクリプションを手動で無効にする必要はありません。移行処理中に、Azure サブスクリプションは自動的に無効になっているためです。</span><span class="sxs-lookup"><span data-stu-id="a5986-148">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="a5986-149">**移行元**の CSP アカウントと**パートナー センター**にサインインし、顧客一覧に移動します。</span><span class="sxs-lookup"><span data-stu-id="a5986-149">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="a5986-150">無効にするサブスクリプションが設定されている顧客を開き、無効にする最初のプランを選びます。</span><span class="sxs-lookup"><span data-stu-id="a5986-150">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="a5986-151">サブスクリプションを **[中断]** に設定し、**[送信]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a5986-151">Set the subscription to **suspended**, and then click **submit**.</span></span>

    <span data-ttu-id="a5986-152">**注:** 二重請求が発生しないようにサブスクリプションを中断します。</span><span class="sxs-lookup"><span data-stu-id="a5986-152">**Note**Suspending the subscription ensures double billing does not occur.</span></span>

     

    <span data-ttu-id="a5986-153">サブスクリプションの一覧で、サブスクリプションに **[中断]** と表示されます。</span><span class="sxs-lookup"><span data-stu-id="a5986-153">The Subscription shows **suspended** on the subscriptions list.</span></span>

4.  <span data-ttu-id="a5986-154">顧客のすべてのサブスクリプションについて、この手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="a5986-154">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="a5986-155">すべてが **[中断]** と表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a5986-155">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="a5986-156">一覧で次の顧客を選び、すべてのサブスクリプションを無効にするプロセスを繰り返します。</span><span class="sxs-lookup"><span data-stu-id="a5986-156">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="a5986-157">Azure の使用量ベースのサブスクリプションを移行する</span><span class="sxs-lookup"><span data-stu-id="a5986-157">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="a5986-158">Azure の使用量ベースの CSP サブスクリプションは、Office 365 の CSP サブスクリプションの場合とは異なり、手動で移行する必要がないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="a5986-158">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="a5986-159">Microsoft Azure サポートは、Azureサブスクリプションと展開されたすべてのサービスやリソースを、**移行元**の CSP リセラー アカウントから**移行先**の CSP リセラー アカウントに移行できます。</span><span class="sxs-lookup"><span data-stu-id="a5986-159">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="a5986-160">この移行中に、顧客へのサービスが中断されることはありません。</span><span class="sxs-lookup"><span data-stu-id="a5986-160">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="a5986-161">Azure サブスクリプションの移行を必要とする顧客のアカウントが、新しい**移行先**の CSP アカウントに関連付けられる契約に同意していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a5986-161">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="a5986-162">パートナーは、Azure サブスクリプションの移行の準備ができている顧客アカウントを Microsoft に通知し、それらの顧客の会社名を提供します。</span><span class="sxs-lookup"><span data-stu-id="a5986-162">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span></span>
3.  <span data-ttu-id="a5986-163">Microsoft は、Azure の使用量ベースのサブスクリプションを移行し、移行が完了したらパートナーに通知します。</span><span class="sxs-lookup"><span data-stu-id="a5986-163">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="a5986-164">パートナーは、パートナー センターの顧客のサブスクリプション セクションで、**移行元**の CSP リセラー アカウントの Azure サブスクリプションが中断されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a5986-164">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="a5986-165">パートナーは、パートナー センターの顧客のサブスクリプション セクションで、**移行先**の CSP リセラー アカウントの Azure サブスクリプションの状態が **[アクティブ]** になっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a5986-165">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

    <span data-ttu-id="a5986-166">**注:**、顧客のサブスクリプションを無効にしても、顧客一覧で、顧客の外観は変わりません。</span><span class="sxs-lookup"><span data-stu-id="a5986-166">**Note**Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="a5986-167">現在、一覧から顧客を削除するオプションはありません。</span><span class="sxs-lookup"><span data-stu-id="a5986-167">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="a5986-168">パートナーは、今後、**移行元**アカウントからこれらの顧客にサブスクリプションを追加しないでください。</span><span class="sxs-lookup"><span data-stu-id="a5986-168">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

     

6.  <span data-ttu-id="a5986-169">今後、**移行元**アカウントでの課金を停止するために、すべての顧客のすべてのサブスクリプションについて、この手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="a5986-169">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="a5986-170">パートナーは、取り消し日から課金期間の最終日までの未使用の日数のクレジットについて最終的な請求書を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="a5986-170">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="a5986-171">最後の課金期間以降、請求書は生成されません。</span><span class="sxs-lookup"><span data-stu-id="a5986-171">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="a5986-172">注意事項</span><span class="sxs-lookup"><span data-stu-id="a5986-172">Notes</span></span>

-   <span data-ttu-id="a5986-173">サービスを無効にする前に**移行先**の CSP アカウントからサービスがプロビジョニングされている場合、**移行元**の CSP アカウントからのサブスクリプションを無効にしても、顧客のサービスには影響しません。</span><span class="sxs-lookup"><span data-stu-id="a5986-173">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="a5986-174">サブスクリプションが中断または取り消しされている場合、顧客はサブスクリプションを利用することはできず、課金は発生しません。</span><span class="sxs-lookup"><span data-stu-id="a5986-174">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="a5986-175">現在、顧客の一覧から顧客を完全に削除する方法はありません。</span><span class="sxs-lookup"><span data-stu-id="a5986-175">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="a5986-176">**注:** パートナーは、パートナー センターそれらのサブスクリプションに移行して、**移行先**パートナー テナント アカウントで設定した同じ日に**移行元**のパートナー テナント アカウントでサブスクリプションを中断する必要があります確認するパートナー センターでは、二重請求は発生しません。</span><span class="sxs-lookup"><span data-stu-id="a5986-176">**Note**Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="a5986-177">**移行元**のサブスクリプションが正しく中断されていない場合、請求の重複のために、Microsoft はクレジットの要求をサポートしません。</span><span class="sxs-lookup"><span data-stu-id="a5986-177">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

     

### <a name="simplify-migration-using-export"></a><span data-ttu-id="a5986-178">エクスポートを使用して移行を簡素化する</span><span class="sxs-lookup"><span data-stu-id="a5986-178">Simplify migration using Export</span></span>

<span data-ttu-id="a5986-179">**エクスポート機能**を使用して、新しい統合後の構造で使用する必要があるサブスクリプションをキャプチャすることができます。</span><span class="sxs-lookup"><span data-stu-id="a5986-179">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="a5986-180">既存の構造内の顧客の一覧を表示するパートナー センターで**顧客**をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a5986-180">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="a5986-181">目的の顧客名を開きます。</span><span class="sxs-lookup"><span data-stu-id="a5986-181">Open the desired customer name.</span></span>

3.  <span data-ttu-id="a5986-182">**[サブスクリプション]** ページで、**[サブスクリプションのエクスポート]** をクリックしてサブスクリプションの詳細を Excel ファイルにエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="a5986-182">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="a5986-183">この一覧を使用して、新しい統合テナント内でサブスクリプションを再作成します。</span><span class="sxs-lookup"><span data-stu-id="a5986-183">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="a5986-184">API 登録</span><span class="sxs-lookup"><span data-stu-id="a5986-184">API registration</span></span>

<span data-ttu-id="a5986-185">この API 登録について詳しくは、[このページ](https://go.microsoft.com/fwlink/?linkid=847990)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a5986-185">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>


 

 



