---
title: 顧客の Azure 支出予算を設定する
ms.topic: how-to
ms.date: 03/17/2021
description: 顧客の毎月の Azure 支出予算を設定または削除する方法と、Azure の支出データを表示し、予算関連の通知を設定する方法について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855354"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="4ed39-103">顧客の月間 Azure 支出予算を設定、確認、または削除パートナー センター</span><span class="sxs-lookup"><span data-stu-id="4ed39-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="4ed39-104">**適切なロール**: 管理エージェント</span><span class="sxs-lookup"><span data-stu-id="4ed39-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="4ed39-105">顧客に [対して毎月の Azure 支出予算を](#set-azure-spending-budget) 設定するには、パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="4ed39-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="4ed39-106">これは、顧客が Azure の支出を管理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="4ed39-107">このオプションを使用すると、顧客の Azure 支出を月の予算と比較できます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="4ed39-108">また、月次請求が予想よりも高くないほど、顧客が Azure の支出を予算化するのにも役立ちます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="4ed39-109">この機能は、サンドボックスまたは Test in Production (TIP) アカウントでは使用できません。</span><span class="sxs-lookup"><span data-stu-id="4ed39-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="4ed39-110">顧客の [Azure 支出予算を](#set-azure-spending-budget)設定した後は、次の方法で顧客の使用状況を確認できます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="4ed39-111">これらのオプションは、正しく構成されていないサービスや、不正行為を示唆する可能性がある異常な傾向を見つけるのに役立つ場合があります。</span><span class="sxs-lookup"><span data-stu-id="4ed39-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="4ed39-112">その後、顧客と一緒に作業し、根本原因を特定し、コストを管理できます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="4ed39-113">必要に応じて、顧客 [の予算を高い](#set-azure-spending-budget) 金額に変更できます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="4ed39-114">Azure の現在の支出を確認する</span><span class="sxs-lookup"><span data-stu-id="4ed39-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="4ed39-115">顧客の支出が予算の上限に近い場合の電子メール通知を有効にする</span><span class="sxs-lookup"><span data-stu-id="4ed39-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="4ed39-116">使用量ベースのサブスクリプションのサービス別の項目別コストを表示する</span><span class="sxs-lookup"><span data-stu-id="4ed39-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="4ed39-117">顧客の [Azure 支出予算](#remove-azure-spending-budget) は、いつでも削除できます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="4ed39-118">Azure の支出データ</span><span class="sxs-lookup"><span data-stu-id="4ed39-118">Azure spending data</span></span>

<span data-ttu-id="4ed39-119">Azure の支出データは見積 *もりであり* 、 *実際の請求金額は異なる場合があります*。</span><span class="sxs-lookup"><span data-stu-id="4ed39-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="4ed39-120">データの値には *、税金* 、クレジット、調整、または適用される可能性があるその他の料金は反映されません。</span><span class="sxs-lookup"><span data-stu-id="4ed39-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="4ed39-121">支出データは *、1 日に 1 回更新されます*。</span><span class="sxs-lookup"><span data-stu-id="4ed39-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="4ed39-122">顧客は、Azure サービスとリソースのアカウント設定を変更しない限り、引き続き Azure サービスとリソースを使用Azure portal。</span><span class="sxs-lookup"><span data-stu-id="4ed39-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="4ed39-123">Azure の支出予算を設定する</span><span class="sxs-lookup"><span data-stu-id="4ed39-123">Set Azure spending budget</span></span>

<span data-ttu-id="4ed39-124">パートナーセンターでは、複数の顧客に対する *月単位の Azure 支出予算を設定* できます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="4ed39-125">[パートナー センター ダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="4ed39-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="4ed39-126">[ **CSP**] の左側のメニューで、[ **Azure の支出**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="4ed39-127">[ **Azure** の使用量] ページの [ **Microsoft Azure サブスクリプションを持つ顧客**] で、予算を設定する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="4ed39-128">**月単位の予算** の値を入力します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="4ed39-129">[ **適用** ] を選択して変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="4ed39-130">また、サブスクリプション設定で *個々の顧客の予算を設定* することもできます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="4ed39-131">パートナー センター ダッシュボードにサインインします。</span><span class="sxs-lookup"><span data-stu-id="4ed39-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="4ed39-132">[ **CSP**] の左側のメニューで、[ **Customers**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="4ed39-133">[ **顧客** ] ページで、顧客の **会社名** を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="4ed39-134">顧客の [ **サブスクリプション** ] ページの [ **使用量ベースのサブスクリプション**] で、[ **予算の変更**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="4ed39-135">予算の値を入力します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="4ed39-136">[ **適用** ] を選択して変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="4ed39-137">Azure の支出予算の削除</span><span class="sxs-lookup"><span data-stu-id="4ed39-137">Remove Azure spending budget</span></span>

<span data-ttu-id="4ed39-138">パートナーセンターでは、お客様の *月単位の Azure 支出予算を削除* できます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="4ed39-139">[パートナー センター ダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="4ed39-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="4ed39-140">[ **CSP**] の左側のメニューで、[ **Azure の支出**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="4ed39-141">[ **Azure** の使用量] ページの [ **Microsoft Azure サブスクリプションを持つ顧客**] で、予算を削除する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="4ed39-142">[ **予算の削除**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="4ed39-143">現在の Azure の支出を確認する</span><span class="sxs-lookup"><span data-stu-id="4ed39-143">Check current Azure spending</span></span>

<span data-ttu-id="4ed39-144">*お客様の現在の Azure の支出と月々の予算* をいつでも追跡できます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="4ed39-145">[パートナー センター ダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="4ed39-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="4ed39-146">[ **CSP**] の左側のメニューで、[ **Azure の支出**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="4ed39-147">**Azure** の支出ページの **[Microsoft Azure** サブスクリプションを持つ顧客] では、顧客の毎月の予算、現在の支出の見積もり、使用されている予算の割合の概要を確認できます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="4ed39-148">予算制限に関する通知</span><span class="sxs-lookup"><span data-stu-id="4ed39-148">Notifications for budget limits</span></span>

<span data-ttu-id="4ed39-149">顧客の *毎月の支出が* 予算の上限に近い場合の電子メール通知を有効にできます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="4ed39-150">このオプションを有効にすると、顧客が月次予算の 80% 以上を使用すると通知されます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="4ed39-151">このオプションは、Azure の請求書を見守るのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="4ed39-152">電子メール通知を構成するには:</span><span class="sxs-lookup"><span data-stu-id="4ed39-152">To configure email notifications:</span></span>

1. <span data-ttu-id="4ed39-153">パートナー センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="4ed39-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="4ed39-154">**[設定]** に移動します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="4ed39-155">[自分 **の設定] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="4ed39-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="4ed39-156">ない場合は、優先メール アドレスを構成します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="4ed39-157">通知の優先言語を構成します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="4ed39-158">[通知 **の基本設定** ] セクションの **[CSP] タブを** 選択します。</span><span class="sxs-lookup"><span data-stu-id="4ed39-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="4ed39-159">Azure 支出通知の [電子メール **] オプションをオン** にし、 を保存 **します**。</span><span class="sxs-lookup"><span data-stu-id="4ed39-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="4ed39-160">サービス別の明細化されたコスト</span><span class="sxs-lookup"><span data-stu-id="4ed39-160">Itemized costs by service</span></span>

<span data-ttu-id="4ed39-161">使用量ベース *のサブスクリプションのサービス別に*、項目化されたコスト (および推定使用量) を表示できます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="4ed39-162">パートナー センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="4ed39-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="4ed39-163">左側のメニューの **[CSP]** で、[顧客] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="4ed39-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="4ed39-164">[顧客 **] ページ** で、顧客の [会社名] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="4ed39-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="4ed39-165">顧客の [サブスクリプション] **ページの** [ **使用量ベースの** サブスクリプション] で、サブスクリプション の名前を選択 **します**。</span><span class="sxs-lookup"><span data-stu-id="4ed39-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="4ed39-166">サブスクリプションのページで、サービス別の項目化されたコストと、当月の推定使用量を確認できます。</span><span class="sxs-lookup"><span data-stu-id="4ed39-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="4ed39-167">次の手順</span><span class="sxs-lookup"><span data-stu-id="4ed39-167">Next steps</span></span>

- [<span data-ttu-id="4ed39-168">CSP の新しいコマース エクスペリエンス - Azure の請求</span><span class="sxs-lookup"><span data-stu-id="4ed39-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
