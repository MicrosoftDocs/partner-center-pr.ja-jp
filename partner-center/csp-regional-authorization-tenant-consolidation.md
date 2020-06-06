---
title: CSP の地域的承認によるテナント統合
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 別の国/地域のテナントを統合するには、次の手順を使用します。 これには、顧客アカウントと顧客のサブスクリプションを移行するための手順が含まれます。
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: LauraBrenner
ms.author: labrenne
keywords: 顧客の移行, プロビジョニング, テナントのアカウント, テナントの統合
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: d361a220ce798863eaeec73e6ff093f135bc4ae1
ms.sourcegitcommit: ca6e0d4a9034120dd600c52ac67b9927dc63b7f5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2020
ms.locfileid: "84453229"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="8e5a3-105">CSP のリージョン承認テナント統合の手順</span><span class="sxs-lookup"><span data-stu-id="8e5a3-105">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="8e5a3-106">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="8e5a3-106">**Applies to**</span></span>

-  <span data-ttu-id="8e5a3-107">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="8e5a3-107">Partner Center</span></span>
-  <span data-ttu-id="8e5a3-108">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="8e5a3-108">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="8e5a3-109">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="8e5a3-109">**Appropriate roles**</span></span>

- <span data-ttu-id="8e5a3-110">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="8e5a3-110">Global admin</span></span>
- <span data-ttu-id="8e5a3-111">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="8e5a3-111">Admin agent</span></span>

<span data-ttu-id="8e5a3-112">\[一部の情報はリリース前の製品に関する事項であり、正式版がリリースされるまでに大幅に変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-112">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="8e5a3-113">ここに記載された情報について、Microsoft は明示または黙示を問わずいかなる保証をするものでもありません。\]</span><span class="sxs-lookup"><span data-stu-id="8e5a3-113">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="8e5a3-114">別の国/地域のテナントを統合するには、次の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="8e5a3-115">**注**  切り替えアカウントからプロビジョニングされた顧客のすべてのサブスクリプションとシート数を把握しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-115">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="8e5a3-116">移行プロセスの一環として、新しい一元化された CSP アカウントで、まったく同じサブスクリプションを同じシート数で再プロビジョニングします。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-116">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="8e5a3-117">エクスポート リスト機能を使用すると、一元化されたテナントに移動する顧客の一覧の作成に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="8e5a3-118">パートナーは、テナントを統合することを選びます。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-118">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="8e5a3-119">統合が完了すると、パートナーは、以前の状態に戻すことはできません。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-119">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="8e5a3-120">顧客のアクションも必要になる可能性があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-120">Note that customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="8e5a3-121">移行を準備する</span><span class="sxs-lookup"><span data-stu-id="8e5a3-121">Prepare for migration</span></span>

- <span data-ttu-id="8e5a3-122">**移行元** (既存の) アカウントで**パートナー センター**にサインインし、すべての顧客と、それらの顧客にプロビジョニングされているすべてのサービスをメモします。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-122">Sign in to your **Partner Center**  with the **Transitioning** (existing) account (the one you will transition)  and take note of all customers and all of the services provisioned for those customers.</span></span>

   :::image type="content" source="images/regionalcustomer1.png" alt-text="地域の顧客の一覧":::

## <a name="migrate-customer-accounts"></a><span data-ttu-id="8e5a3-124">顧客アカウントを移行する</span><span class="sxs-lookup"><span data-stu-id="8e5a3-124">Migrate customer accounts</span></span>

1. <span data-ttu-id="8e5a3-125">**移行先** (新しい) アカウントで**パートナー センター**にサインインし、**[顧客]** から顧客の一覧に移動します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-125">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2. <span data-ttu-id="8e5a3-126">[顧客] を選びます。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-126">Select Customers.</span></span>

3. <span data-ttu-id="8e5a3-127">**[再販業者関係の要求]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-127">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="8e5a3-128">顧客に表示する既定のメール メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-128">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="8e5a3-129">このメッセージには、新しいパートナー センター アカウントに対して一意の URL と組織 ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-129">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="8e5a3-130">**顧客のアクション:** 移行したいアクティブな各顧客がこの URL にアクセスしたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-130">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="8e5a3-131">この URL を開くと、顧客は、Office 365 ポータルにサインインするよう求められます。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-131">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="8e5a3-132">顧客は、Azure や Office 365 管理ポータルにアクセスするために使用する組織 ID と同じ組織 ID を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-132">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="8e5a3-133">サインインした後、顧客アカウントのグローバル管理者は、新しい CSP アカウントに委任された管理者特権を与えるという契約を提出するよう求められます。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-133">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="8e5a3-134">契約書に同意する場合、顧客はチェック ボックスをオンにして、関係を承認することに同意します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-134">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="8e5a3-135">顧客は、契約を送信した後、パートナーの顧客一覧に表示されます (1 つずつ)。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-135">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="8e5a3-136">Office 365 および Azure 以外の使用量ベースのサブスクリプションを移行する</span><span class="sxs-lookup"><span data-stu-id="8e5a3-136">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="8e5a3-137">顧客が契約書に署名すると、パートナーは、一元化されたパートナー テナントでサブスクリプションを再作成できます。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-137">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="8e5a3-138">**パートナー センター**で **[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-138">From the **Partner Center** select **Customers**.</span></span>

3. <span data-ttu-id="8e5a3-139">移行する顧客の会社名を開きます。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-139">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="8e5a3-140">[**サブスクリプションの追加**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-140">Click **Add subscription**.</span></span>

5. <span data-ttu-id="8e5a3-141">カタログから適切なサブスクリプションとシート数を追加します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-141">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="8e5a3-142">**移行元**のパートナー アカウントに表示されている情報を確認します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-142">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="顧客の一覧":::

6. <span data-ttu-id="8e5a3-144">[**送信] をクリックします。**</span><span class="sxs-lookup"><span data-stu-id="8e5a3-144">Click **Submit.**</span></span>

   <span data-ttu-id="8e5a3-145">これでサービスは、**移行先**のパートナー アカウントから顧客に提供されるようになります。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-145">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="8e5a3-146">その他のすべての顧客のサブスクリプションを移行するには、この手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-146">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="8e5a3-147">次のセクションに進む前に、**移行元**のパートナー アカウントに存在しているすべての顧客のサブスクリプションが、**移行先**のパートナー アカウントで再プロビジョニングされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-147">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="8e5a3-148">パートナーは、パートナーセンターのパートナーテナントアカウント**から**のサブスクリプションを中断し、パートナーセンターのパートナーテナントアカウント**に**移行して、二重の課金が発生しないようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-148">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="8e5a3-149">**移行元**のサブスクリプションが正しく無効に設定されていない場合、請求の重複のために、クレジットのサポート要求が拒否されます。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-149">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="8e5a3-150">移行元のパートナー アカウントで Office 365 のサブスクリプションを無効にする</span><span class="sxs-lookup"><span data-stu-id="8e5a3-150">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="8e5a3-151">**移行元**のパートナー アカウントで CSP サブスクリプションを無効にすると、それ以降の請求は停止されます。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-151">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="8e5a3-152">Azure サブスクリプションを手動で無効にする必要はありません。移行処理中に、Azure サブスクリプションは自動的に無効になっているためです。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-152">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="8e5a3-153">**移行元**の CSP アカウントで**パートナー センター**にサインインし、顧客の一覧に移動します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-153">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="8e5a3-154">無効にするサブスクリプションが設定されている顧客を開き、無効にする最初のプランを選びます。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-154">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="8e5a3-155">サブスクリプションを **[中断]** に設定し、**[送信]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-155">Set the subscription to **suspended**, and then click **submit**.</span></span>

   >[!Note]
   >  <span data-ttu-id="8e5a3-156">サブスクリプションを中断すると、2つの課金が発生しなくなります。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-156">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="8e5a3-157">サブスクリプションの一覧で、サブスクリプションに **[中断]** と表示されます。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-157">The Subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="8e5a3-158">顧客のすべてのサブスクリプションについて、この手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-158">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="8e5a3-159">すべてが **[中断]** と表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-159">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="8e5a3-160">一覧で次の顧客を選び、すべてのサブスクリプションを無効にするプロセスを繰り返します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-160">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="8e5a3-161">Azure の使用量ベースのサブスクリプションを移行する</span><span class="sxs-lookup"><span data-stu-id="8e5a3-161">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="8e5a3-162">Azure では、Office 365 CSP サブスクリプションの場合と同様に、使用量ベースの CSP サブスクリプションを手動で移行する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-162">Azure, usage-based CSP subscriptions do not need to be migrated manually as is the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="8e5a3-163">Microsoft Azure サポートは、Azureサブスクリプションと展開されたすべてのサービスやリソースを、**移行元**の CSP リセラー アカウントから**移行先**の CSP リセラー アカウントに移行できます。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-163">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="8e5a3-164">この移行中に、顧客へのサービスが中断されることはありません。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-164">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="8e5a3-165">Azure サブスクリプションの移行を必要とする顧客のアカウントが、新しい**移行先**の CSP アカウントに関連付けられる契約に同意していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-165">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="8e5a3-166">パートナーは、Azure サブスクリプションを所有しているお客様のアカウントを移行する準備ができていることを Microsoft に通知し、その顧客の会社名を提供します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-166">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer's company names.</span></span>

3. <span data-ttu-id="8e5a3-167">Microsoft は、Azure の使用量ベースのサブスクリプションを移行し、移行が完了したらパートナーに通知します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-167">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>

4. <span data-ttu-id="8e5a3-168">パートナーは、パートナー センターの顧客のサブスクリプション セクションで、**移行元**の CSP リセラー アカウントの Azure サブスクリプションが中断されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-168">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="8e5a3-169">パートナーは、パートナー センターの顧客のサブスクリプション セクションで、**移行先**の CSP リセラー アカウントの Azure サブスクリプションの状態が **[アクティブ]** になっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-169">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="8e5a3-170">顧客のサブスクリプションを無効にしても、顧客の一覧に表示される顧客の外観は変わりません。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-170">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="8e5a3-171">現在、一覧から顧客を削除するオプションはありません。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-171">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="8e5a3-172">パートナーは、今後、**移行元**アカウントからこれらの顧客にサブスクリプションを追加しないでください。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-172">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="8e5a3-173">今後、**移行元**アカウントでの課金を停止するために、すべての顧客のすべてのサブスクリプションについて、この手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-173">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="8e5a3-174">パートナーは、取り消し日から課金期間の最終日までの未使用の日数のクレジットについて最終的な請求書を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-174">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="8e5a3-175">最後の課金期間以降、請求書は生成されません。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-175">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="8e5a3-176">Notes</span><span class="sxs-lookup"><span data-stu-id="8e5a3-176">Notes</span></span>

- <span data-ttu-id="8e5a3-177">Csp アカウント**からの移行**からサブスクリプションを無効にしても、サブスクリプションを無効にする前に、サービスが "Csp**に移行**しています" アカウントからプロビジョニングされている限り、エンドカスタマーのサービスには影響しません。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-177">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="8e5a3-178">サブスクリプションは、お客様が使用することはできません。また、保留中またはキャンセル時には請求を生成しません。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-178">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="8e5a3-179">現在、顧客の一覧から顧客を完全に削除する方法はありません。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-179">There is currently no way to remove a customer from the Customers list completely.</span></span>

>[!Note]
> <span data-ttu-id="8e5a3-180">パートナーは、パートナーセンターのパートナーテナントアカウントからのサブスクリプションを中断して、パートナーセンターのパートナーテナントアカウント**から\*\*\*\*の移行**と設定を行い、二重の課金が発生しないようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-180">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="8e5a3-181">Microsoft では、サブスクリプションから中断への**移行**を正しく設定していないことが原因で、課金の重複によってクレジットの要求がサポートされません。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-181">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="8e5a3-182">エクスポートを使用して移行を簡素化する</span><span class="sxs-lookup"><span data-stu-id="8e5a3-182">Simplify migration using Export</span></span>

<span data-ttu-id="8e5a3-183">**エクスポート機能**を使用して、新しい統合後の構造で使用する必要があるサブスクリプションをキャプチャすることができます。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-183">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="8e5a3-184">パートナー センターで **[顧客]** をクリックして、既存の構造内の顧客の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-184">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2. <span data-ttu-id="8e5a3-185">目的の顧客名を開きます。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-185">Open the desired customer name.</span></span>

3. <span data-ttu-id="8e5a3-186">**[サブスクリプション]** ページで、**[サブスクリプションのエクスポート]** をクリックしてサブスクリプションの詳細を Excel ファイルにエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-186">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="8e5a3-187">この一覧を使用して、新しい統合テナント内でサブスクリプションを再作成します。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-187">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="8e5a3-188">API 登録</span><span class="sxs-lookup"><span data-stu-id="8e5a3-188">API registration</span></span>

<span data-ttu-id="8e5a3-189">API 登録の詳細については、「[パートナーセンターでの api アクセスの設定](https://go.microsoft.com/fwlink/?linkid=847990)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e5a3-189">For more information about API registration, see [Set up API access in Partner Center](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>
