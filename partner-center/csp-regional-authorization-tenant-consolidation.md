---
title: CSP の地域的承認によるテナント統合
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 別の国/地域のテナントを統合するには、次の手順を使用します。 これには、顧客アカウントと顧客のサブスクリプションを移行するための手順が含まれます。
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 2171e2b10101e99bdd8d415a936ba98af65c2a1b
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502572"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="43fe1-104">CSP の地域承認によるテナント統合の手順</span><span class="sxs-lookup"><span data-stu-id="43fe1-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="43fe1-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="43fe1-105">**Applies to**</span></span>

- <span data-ttu-id="43fe1-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="43fe1-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="43fe1-107">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="43fe1-107">**Appropriate roles**</span></span>

- <span data-ttu-id="43fe1-108">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="43fe1-108">Global admin</span></span>
- <span data-ttu-id="43fe1-109">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="43fe1-109">Admin agent</span></span>

<span data-ttu-id="43fe1-110">\[一部の情報はリリース前の製品に関する事項であり、正式版がリリースされるまでに大幅に変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="43fe1-110">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="43fe1-111">ここに記載された情報について、Microsoft は明示または黙示を問わずいかなる保証をするものでもありません。\]</span><span class="sxs-lookup"><span data-stu-id="43fe1-111">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="43fe1-112">テナントをビジネス向けに統合することができます。</span><span class="sxs-lookup"><span data-stu-id="43fe1-112">You can consolidate tenants for your business.</span></span> <span data-ttu-id="43fe1-113">別の国/地域のテナントを統合するには、次の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-113">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="43fe1-114">移行元のアカウントの各顧客について、プロビジョニングされたすべてのサブスクリプションとライセンス数を把握しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="43fe1-114">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="43fe1-115">移行プロセスの一部として、新しい中央 CSP アカウントで同じライセンス数を使用して、同じ完全なサブスクリプションを再プロビジョニングします。</span><span class="sxs-lookup"><span data-stu-id="43fe1-115">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="43fe1-116">エクスポート リスト機能を使用すると、一元化されたテナントに移動する顧客の一覧の作成に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="43fe1-116">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="43fe1-117">統合が完了すると、以前のテナントの状態に戻すことはできません。</span><span class="sxs-lookup"><span data-stu-id="43fe1-117">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="43fe1-118">また、顧客の操作が必要になる場合もあります。</span><span class="sxs-lookup"><span data-stu-id="43fe1-118">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="43fe1-119">移行を準備する</span><span class="sxs-lookup"><span data-stu-id="43fe1-119">Prepare for migration</span></span>

- <span data-ttu-id="43fe1-120">**移行** 中のアカウント (新しいアカウントに移行するアカウント) を使用して **パートナーセンター** にサインインし、すべての顧客と、それらの顧客に対してプロビジョニングされたすべてのサービスを確認します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-120">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="43fe1-121">このアカウントからサインアウトします。</span><span class="sxs-lookup"><span data-stu-id="43fe1-121">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="43fe1-122">顧客アカウントを移行する</span><span class="sxs-lookup"><span data-stu-id="43fe1-122">Migrate customer accounts</span></span>

1. <span data-ttu-id="43fe1-123">**移行**(新しい) アカウント (顧客を移行しているユーザー) で **パートナーセンター** にサインインします。</span><span class="sxs-lookup"><span data-stu-id="43fe1-123">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="43fe1-124">**[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-124">Select **Customers**.</span></span>

3. <span data-ttu-id="43fe1-125">[ **リセラーとの関係を要求する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-125">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="43fe1-126">顧客に送信する既定の電子メールメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="43fe1-126">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="43fe1-127">このメッセージには、新しいパートナー センター アカウントに対して一意の URL と組織 ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="43fe1-127">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="43fe1-128">**顧客のアクション:** 移行したいアクティブな各顧客がこの URL にアクセスしたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-128">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="43fe1-129">この URL を開くと、顧客は、Office 365 ポータルにサインインするよう求められます。</span><span class="sxs-lookup"><span data-stu-id="43fe1-129">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="43fe1-130">顧客は、Azure や Office 365 管理ポータルにアクセスするために使用する組織 ID と同じ組織 ID を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="43fe1-130">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="43fe1-131">サインインした後、 **顧客アカウント** のグローバル管理者は、新しい CSP アカウントに委任された管理者特権を付与する契約を提出するように求められます。</span><span class="sxs-lookup"><span data-stu-id="43fe1-131">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="43fe1-132">契約書に同意する場合、顧客はチェック ボックスをオンにして、関係を承認することに同意します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-132">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="43fe1-133">顧客は、契約を送信した後、パートナーの顧客一覧に表示されます (1 つずつ)。</span><span class="sxs-lookup"><span data-stu-id="43fe1-133">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="43fe1-134">Office 365 および Azure 以外の使用量ベースのサブスクリプションを移行する</span><span class="sxs-lookup"><span data-stu-id="43fe1-134">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="43fe1-135">顧客が契約書に署名すると、パートナーは、一元化されたパートナー テナントでサブスクリプションを再作成できます。</span><span class="sxs-lookup"><span data-stu-id="43fe1-135">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="43fe1-136">**パートナーセンター** から、[ **Customers**] \ (顧客 \) を選択します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-136">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="43fe1-137">移行する顧客の会社名を開きます。</span><span class="sxs-lookup"><span data-stu-id="43fe1-137">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="43fe1-138">**[サブスクリプションの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-138">Select **Add subscription**.</span></span>

5. <span data-ttu-id="43fe1-139">カタログから適切なサブスクリプションとライセンス数を追加します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-139">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="43fe1-140">**移行元** のパートナー アカウントに表示されている情報を確認します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-140">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="顧客の一覧":::

6. <span data-ttu-id="43fe1-142">[送信] を選択し **ます。**</span><span class="sxs-lookup"><span data-stu-id="43fe1-142">Select **Submit.**</span></span>

   <span data-ttu-id="43fe1-143">これでサービスは、**移行先** のパートナー アカウントから顧客に提供されるようになります。</span><span class="sxs-lookup"><span data-stu-id="43fe1-143">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="43fe1-144">その他のすべての顧客のサブスクリプションを移行するには、この手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-144">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="43fe1-145">次のセクションに進む前に、**移行元** のパートナー アカウントに存在しているすべての顧客のサブスクリプションが、**移行先** のパートナー アカウントで再プロビジョニングされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-145">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="43fe1-146">パートナーは、パートナーセンターのパートナーテナントアカウント **から** のサブスクリプションを中断し、パートナーセンターのパートナーテナントアカウント **に** 移行して、二重の課金が発生しないようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="43fe1-146">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="43fe1-147">サブスクリプション **からの移行** が正しく無効になっていないことが原因で、課金の重複によってクレジットのサポート要求が拒否されます。</span><span class="sxs-lookup"><span data-stu-id="43fe1-147">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="43fe1-148">移行元のパートナー アカウントで Office 365 のサブスクリプションを無効にする</span><span class="sxs-lookup"><span data-stu-id="43fe1-148">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="43fe1-149">**移行元** のパートナー アカウントで CSP サブスクリプションを無効にすると、それ以降の請求は停止されます。</span><span class="sxs-lookup"><span data-stu-id="43fe1-149">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="43fe1-150">Azure サブスクリプションは移行プロセス中に自動的に無効になるため、Azure サブスクリプションを手動で無効にする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="43fe1-150">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="43fe1-151">**移行元** の CSP アカウントで **パートナー センター** にサインインし、顧客の一覧に移動します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-151">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="43fe1-152">無効にするサブスクリプションが設定されている顧客を開き、無効にする最初のプランを選びます。</span><span class="sxs-lookup"><span data-stu-id="43fe1-152">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="43fe1-153">サブスクリプションを [ **一時停止**] に設定し、[ **送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-153">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="43fe1-154">サブスクリプションを中断すると、2つの課金が発生しなくなります。</span><span class="sxs-lookup"><span data-stu-id="43fe1-154">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="43fe1-155">サブスクリプションは、サブスクリプションの一覧で [ **中断** ] と表示されます。</span><span class="sxs-lookup"><span data-stu-id="43fe1-155">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="43fe1-156">顧客のすべてのサブスクリプションについて、この手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-156">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="43fe1-157">すべてが **[中断]** と表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-157">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="43fe1-158">一覧で次の顧客を選び、すべてのサブスクリプションを無効にするプロセスを繰り返します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-158">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="43fe1-159">Azure の使用量ベースのサブスクリプションを移行する</span><span class="sxs-lookup"><span data-stu-id="43fe1-159">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="43fe1-160">Office 365 CSP サブスクリプションとは異なり、Azure では、使用量ベースの CSP サブスクリプションを手動で移行する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="43fe1-160">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="43fe1-161">Microsoft Azure サポートは、Azure サブスクリプションと、すべてのデプロイ済みのサービスまたはリソースを、csp リセラーのアカウント **から** の移行 **から csp リセラーアカウントに移行** します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-161">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="43fe1-162">この移行中に、顧客へのサービスが中断されることはありません。</span><span class="sxs-lookup"><span data-stu-id="43fe1-162">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="43fe1-163">Azure サブスクリプション **を** 移行したお客様のアカウントが、新しい移行先の CSP アカウントに関連付けられている契約に同意していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-163">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="43fe1-164">移行の準備ができている顧客アカウントを Microsoft に通知し、その顧客の会社名を指定します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-164">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="43fe1-165">Microsoft は、Azure の使用量ベースのサブスクリプションを移行し、移行が完了したことを通知します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-165">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="43fe1-166">「CSP リセラーアカウント **からの移行** 」の Azure サブスクリプションが、パートナーセンターの [カスタマーサブスクリプション] セクションの [ **中断** 済み] とマークされていることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="43fe1-166">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="43fe1-167">[ **To** the CSP リセラー] アカウントの下にある Azure サブスクリプションの [customer subscription] \ (カスタマーサブスクリプション \) セクションの下に、パートナーセンターで [ **アクティブ** ] の状態が表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-167">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="43fe1-168">顧客のサブスクリプションを無効にしても、顧客の一覧に表示される顧客の外観は変わりません。</span><span class="sxs-lookup"><span data-stu-id="43fe1-168">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="43fe1-169">現在、一覧から顧客を削除するオプションはありません。</span><span class="sxs-lookup"><span data-stu-id="43fe1-169">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="43fe1-170">パートナーは、今後、**移行元** アカウントからこれらの顧客にサブスクリプションを追加しないでください。</span><span class="sxs-lookup"><span data-stu-id="43fe1-170">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="43fe1-171">今後、**移行元** アカウントでの課金を停止するために、すべての顧客のすべてのサブスクリプションについて、この手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-171">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="43fe1-172">パートナーは、取り消し日から課金期間の最終日までの未使用の日数のクレジットについて最終的な請求書を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="43fe1-172">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="43fe1-173">最後の課金期間以降、請求書は生成されません。</span><span class="sxs-lookup"><span data-stu-id="43fe1-173">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="43fe1-174">関連情報</span><span class="sxs-lookup"><span data-stu-id="43fe1-174">Additional information</span></span>

- <span data-ttu-id="43fe1-175">Csp アカウント **からの移行** からサブスクリプションを無効にしても、サブスクリプションを無効にする前に、サービスが "Csp **に移行** しています" アカウントからプロビジョニングされている限り、エンドカスタマーのサービスには影響しません。</span><span class="sxs-lookup"><span data-stu-id="43fe1-175">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="43fe1-176">サブスクリプションは、お客様が使用することはできません。また、保留中またはキャンセル時には請求を生成しません。</span><span class="sxs-lookup"><span data-stu-id="43fe1-176">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="43fe1-177">現在 **、顧客リストから** 顧客を完全に削除する方法はありません。</span><span class="sxs-lookup"><span data-stu-id="43fe1-177">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="43fe1-178">パートナーは、パートナーセンターのパートナーテナントアカウント **からの移行** 中に、2つの課金が発生しないように、それらのサブスクリプションが移行され、 **移行** 先アカウントで設定されている場合に、サブスクリプションを中断する必要があります。</span><span class="sxs-lookup"><span data-stu-id="43fe1-178">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="43fe1-179">Microsoft では、サブスクリプションから中断への **移行** を正しく設定していないことが原因で、課金の重複によってクレジットの要求がサポートされません。</span><span class="sxs-lookup"><span data-stu-id="43fe1-179">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="43fe1-180">エクスポートを使用して移行を簡素化する</span><span class="sxs-lookup"><span data-stu-id="43fe1-180">Simplify migration using Export</span></span>

<span data-ttu-id="43fe1-181">**エクスポート機能** を使用して、新しい統合後の構造で使用する必要があるサブスクリプションをキャプチャすることができます。</span><span class="sxs-lookup"><span data-stu-id="43fe1-181">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="43fe1-182">パートナーセンターで **顧客** を選択すると、顧客の一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="43fe1-182">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="43fe1-183">目的の顧客名を開きます。</span><span class="sxs-lookup"><span data-stu-id="43fe1-183">Open the desired customer name.</span></span>

3. <span data-ttu-id="43fe1-184">[ **サブスクリプション** ] ページで、[サブスクリプションの **エクスポート** ] を選択して、サブスクリプションの詳細を Excel ファイルにエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="43fe1-184">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="43fe1-185">この一覧を使用して、新しい統合テナント内でサブスクリプションを再作成します。</span><span class="sxs-lookup"><span data-stu-id="43fe1-185">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="43fe1-186">API 登録</span><span class="sxs-lookup"><span data-stu-id="43fe1-186">API registration</span></span>

<span data-ttu-id="43fe1-187">API 登録の詳細については、「 [パートナーセンターでの api アクセスの設定](/partner-center/develop/set-up-api-access-in-partner-center)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43fe1-187">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="43fe1-188">次の手順</span><span class="sxs-lookup"><span data-stu-id="43fe1-188">Next steps</span></span>

- [<span data-ttu-id="43fe1-189">クラウドソリューションプロバイダープログラムの地域市場と、CSP プランを販売できる通貨</span><span class="sxs-lookup"><span data-stu-id="43fe1-189">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
