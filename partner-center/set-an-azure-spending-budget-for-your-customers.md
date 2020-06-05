---
title: 顧客の Azure 支出予算を設定する
ms.topic: article
ms.date: 06/03/2020
description: 顧客向けの月単位の Azure 支出予算を設定または削除する方法と、Azure の支出データを表示し、予算に関連する通知を設定する方法について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17b6186d7e6cddaf598dc663c70841275c0db853
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/04/2020
ms.locfileid: "84425991"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="8f858-103">パートナーセンターのお客様に対する月単位の Azure 支出予算を設定、確認、または削除する</span><span class="sxs-lookup"><span data-stu-id="8f858-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="8f858-104">適用対象:</span><span class="sxs-lookup"><span data-stu-id="8f858-104">Applies to:</span></span>

- <span data-ttu-id="8f858-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="8f858-105">Partner Center</span></span>
- <span data-ttu-id="8f858-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="8f858-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="8f858-107">パートナーセンターでは、[顧客の Azure 支出予算を毎月設定](#set-azure-spending-budget)できます。</span><span class="sxs-lookup"><span data-stu-id="8f858-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="8f858-108">これにより、お客様は Azure の支出を管理できます。</span><span class="sxs-lookup"><span data-stu-id="8f858-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="8f858-109">このオプションを使用すると、顧客の Azure の支出を月の予算と比較できます。</span><span class="sxs-lookup"><span data-stu-id="8f858-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="8f858-110">また、お客様が Azure の使用量を予算に費やして、月々の請求額が予想よりも高くならないようにすることもできます。</span><span class="sxs-lookup"><span data-stu-id="8f858-110">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="8f858-111">この機能は、サンドボックスまたは Test in Production (TIP) アカウントでは使用できません。</span><span class="sxs-lookup"><span data-stu-id="8f858-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="8f858-112">[顧客の Azure 支出予算を設定](#set-azure-spending-budget)した後、次の方法で顧客の使用状況を確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="8f858-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="8f858-113">これらのオプションを使用すると、正しく構成されていないサービスや、不正行為の可能性がある異常な傾向を特定できます。</span><span class="sxs-lookup"><span data-stu-id="8f858-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="8f858-114">その後、顧客と協力して根本原因を特定し、コストを管理できます。</span><span class="sxs-lookup"><span data-stu-id="8f858-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="8f858-115">必要に応じ[て、お客様の予算](#set-azure-spending-budget)をより高い金額に変更することもできます。</span><span class="sxs-lookup"><span data-stu-id="8f858-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="8f858-116">現在の Azure の支出を確認する</span><span class="sxs-lookup"><span data-stu-id="8f858-116">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="8f858-117">顧客の支出が予算制限に近づいたときの電子メール通知を有効にする</span><span class="sxs-lookup"><span data-stu-id="8f858-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="8f858-118">使用量ベースのサブスクリプションのサービス別コストを表示する</span><span class="sxs-lookup"><span data-stu-id="8f858-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="8f858-119">また、お客様の[Azure 支出予算](#remove-azure-spending-budget)をいつでも削除することもできます。</span><span class="sxs-lookup"><span data-stu-id="8f858-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="8f858-120">Azure の支出データ</span><span class="sxs-lookup"><span data-stu-id="8f858-120">Azure spending data</span></span>

<span data-ttu-id="8f858-121">Azure の支出データは*見積もり*で*あり、実際の請求金額は異なる場合があり*ます。</span><span class="sxs-lookup"><span data-stu-id="8f858-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="8f858-122">データの値には、適用される可能性がある税金、クレジット、調整、またはその他の料金は反映され*ません*。</span><span class="sxs-lookup"><span data-stu-id="8f858-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="8f858-123">支出データは 1*日に1回更新*されます。</span><span class="sxs-lookup"><span data-stu-id="8f858-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="8f858-124">Azure portal でアカウントの設定を変更しない限り、お客様は Azure のサービスとリソースを引き続き使用できます (料金が発生します)。</span><span class="sxs-lookup"><span data-stu-id="8f858-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="8f858-125">Azure の支出予算を設定する</span><span class="sxs-lookup"><span data-stu-id="8f858-125">Set Azure spending budget</span></span>

<span data-ttu-id="8f858-126">パートナーセンターでは、複数の顧客に対する*月単位の Azure 支出予算を設定*できます。</span><span class="sxs-lookup"><span data-stu-id="8f858-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="8f858-127">[パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="8f858-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="8f858-128">[ **CSP**] の左側のメニューで、[ **Azure の支出**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f858-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="8f858-129">[ **Azure**の使用量] ページの [ **Microsoft Azure サブスクリプションを持つ顧客**] で、予算を設定する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f858-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="8f858-130">**月単位の予算**の値を入力します。</span><span class="sxs-lookup"><span data-stu-id="8f858-130">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="8f858-131">[**適用**] を選択して変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="8f858-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="8f858-132">また、サブスクリプション設定で*個々の顧客の予算を設定*することもできます。</span><span class="sxs-lookup"><span data-stu-id="8f858-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="8f858-133">パートナー センター ダッシュボードにサインインします。</span><span class="sxs-lookup"><span data-stu-id="8f858-133">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="8f858-134">[ **CSP**] の左側のメニューで、[ **Customers**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f858-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="8f858-135">[**顧客**] ページで、顧客の**会社名**を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f858-135">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="8f858-136">顧客の [**サブスクリプション**] ページの [**使用量ベースのサブスクリプション**] で、[**予算の変更**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f858-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="8f858-137">予算の値を入力します。</span><span class="sxs-lookup"><span data-stu-id="8f858-137">Enter a value for the budget.</span></span>

6. <span data-ttu-id="8f858-138">[**適用**] を選択して変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="8f858-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="8f858-139">Azure の支出予算の削除</span><span class="sxs-lookup"><span data-stu-id="8f858-139">Remove Azure spending budget</span></span>

<span data-ttu-id="8f858-140">パートナーセンターでは、お客様の*月単位の Azure 支出予算を削除*できます。</span><span class="sxs-lookup"><span data-stu-id="8f858-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="8f858-141">[パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="8f858-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="8f858-142">[ **CSP**] の左側のメニューで、[ **Azure の支出**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f858-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="8f858-143">[ **Azure**の使用量] ページの [ **Microsoft Azure サブスクリプションを持つ顧客**] で、予算を削除する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f858-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="8f858-144">[**予算の削除**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f858-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="8f858-145">現在の Azure の支出を確認する</span><span class="sxs-lookup"><span data-stu-id="8f858-145">Check current Azure spending</span></span>

<span data-ttu-id="8f858-146">*お客様の現在の Azure の支出と月々の予算*をいつでも追跡できます。</span><span class="sxs-lookup"><span data-stu-id="8f858-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="8f858-147">[パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="8f858-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="8f858-148">[ **CSP**] の左側のメニューで、[ **Azure の支出**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f858-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="8f858-149">[ **Azure**の使用量] ページで、[ **Microsoft Azure のサブスクリプションをお持ちのお客様**] の下に、顧客の月々の予算、現在の支出見積もり、使用された予算の割合の概要が表示されます。</span><span class="sxs-lookup"><span data-stu-id="8f858-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="8f858-150">予算制限の通知</span><span class="sxs-lookup"><span data-stu-id="8f858-150">Notifications for budget limits</span></span>

<span data-ttu-id="8f858-151">お客様の月々の支出が予算制限に近づいたときに、*電子メール通知を有効*にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8f858-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="8f858-152">このオプションをオンにすると、顧客が80% 以上の月間予算を使用した場合に通知が表示されます。</span><span class="sxs-lookup"><span data-stu-id="8f858-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="8f858-153">このオプションを使用すると、Azure の課金内容を監視できます。</span><span class="sxs-lookup"><span data-stu-id="8f858-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="8f858-154">電子メール通知を構成するには:</span><span class="sxs-lookup"><span data-stu-id="8f858-154">To configure email notifications:</span></span>

1. <span data-ttu-id="8f858-155">パートナー センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="8f858-155">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="8f858-156">[ **CSP**] の左側のメニューで、[ **Azure の支出**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f858-156">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="8f858-157">[ **Azure の支出**] ページの [**電子メール通知**] で、[**電子メールの取得**] 設定を **[オン**] に切り替えます。</span><span class="sxs-lookup"><span data-stu-id="8f858-157">On the **Azure spending** page, under **Email notifications**, toggle the **Get emails** setting to **On**.</span></span>

4. <span data-ttu-id="8f858-158">[**電子メールアドレスの変更**] を選択して、通知の電子メールアドレスを表示します。</span><span class="sxs-lookup"><span data-stu-id="8f858-158">Choose **Change email address** to see the email address for notifications.</span></span>

5. <span data-ttu-id="8f858-159">電子メールアドレスが*正しくない*場合は、正しい電子メールアドレスを入力し、[**更新**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f858-159">If the email address *isn't correct*, enter the correct email address and choose **Update**.</span></span> <span data-ttu-id="8f858-160">電子メールアドレス*が正しい*場合は、[**キャンセル**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f858-160">If the email address *is correct*, choose **Cancel**.</span></span>

## <a name="itemized-costs-by-service"></a><span data-ttu-id="8f858-161">サービス別コストの明細</span><span class="sxs-lookup"><span data-stu-id="8f858-161">Itemized costs by service</span></span>

<span data-ttu-id="8f858-162">*使用状況に基づいたサブスクリプションのサービスごとに、明細のコスト (および推定使用量) を表示*できます。</span><span class="sxs-lookup"><span data-stu-id="8f858-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="8f858-163">パートナー センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="8f858-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="8f858-164">[ **CSP**] の左側のメニューで、[ **Customers**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f858-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="8f858-165">[**顧客**] ページで、顧客の**会社名**を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f858-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="8f858-166">顧客の [**サブスクリプション**] ページの [**使用量ベースのサブスクリプション**] で、**サブスクリプション**の名前を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f858-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="8f858-167">サブスクリプションのページで、サービスごとの**明細コスト**と当月の**推定使用量**を確認できます。</span><span class="sxs-lookup"><span data-stu-id="8f858-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
