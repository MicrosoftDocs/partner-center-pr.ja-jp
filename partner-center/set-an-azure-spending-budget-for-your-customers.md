---
title: 顧客の Azure 支出予算を設定する
ms.topic: how-to
ms.date: 06/03/2020
description: 顧客向けの月単位の Azure 支出予算を設定または削除する方法と、Azure の支出データを表示し、予算に関連する通知を設定する方法について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e311af31bbce65ed38c20df12243d325c7a63d04
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/01/2020
ms.locfileid: "96438976"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="da4c1-103">パートナーセンターのお客様に対する月単位の Azure 支出予算を設定、確認、または削除する</span><span class="sxs-lookup"><span data-stu-id="da4c1-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="da4c1-104">適用対象:</span><span class="sxs-lookup"><span data-stu-id="da4c1-104">Applies to:</span></span>

- <span data-ttu-id="da4c1-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="da4c1-105">Partner Center</span></span>
- <span data-ttu-id="da4c1-106">米国政府機関向け Microsoft Cloud のパートナー センター</span><span class="sxs-lookup"><span data-stu-id="da4c1-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="da4c1-107">パートナーセンターでは、 [顧客の Azure 支出予算を毎月設定](#set-azure-spending-budget) できます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="da4c1-108">これにより、お客様は Azure の支出を管理できます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="da4c1-109">このオプションを使用すると、顧客の Azure の支出を月の予算と比較できます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="da4c1-110">また、お客様が Azure の使用量を予算に費やして、月々の請求額が予想よりも高くならないようにすることもできます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-110">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="da4c1-111">この機能は、サンドボックスまたは Test in Production (TIP) アカウントでは使用できません。</span><span class="sxs-lookup"><span data-stu-id="da4c1-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="da4c1-112">[顧客の Azure 支出予算を設定](#set-azure-spending-budget)した後、次の方法で顧客の使用状況を確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="da4c1-113">これらのオプションを使用すると、正しく構成されていないサービスや、不正行為の可能性がある異常な傾向を特定できます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="da4c1-114">その後、顧客と協力して根本原因を特定し、コストを管理できます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="da4c1-115">必要に応じ [て、お客様の予算](#set-azure-spending-budget) をより高い金額に変更することもできます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="da4c1-116">現在の Azure の支出を確認する</span><span class="sxs-lookup"><span data-stu-id="da4c1-116">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="da4c1-117">顧客の支出が予算制限に近づいたときの電子メール通知を有効にする</span><span class="sxs-lookup"><span data-stu-id="da4c1-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="da4c1-118">使用量ベースのサブスクリプションのサービス別コストを表示する</span><span class="sxs-lookup"><span data-stu-id="da4c1-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="da4c1-119">また、お客様の [Azure 支出予算](#remove-azure-spending-budget) をいつでも削除することもできます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="da4c1-120">Azure の支出データ</span><span class="sxs-lookup"><span data-stu-id="da4c1-120">Azure spending data</span></span>

<span data-ttu-id="da4c1-121">Azure の支出データは *見積もり* で *あり、実際の請求金額は異なる場合があり* ます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="da4c1-122">データの値には、適用される可能性がある税金、クレジット、調整、またはその他の料金は反映され *ません* 。</span><span class="sxs-lookup"><span data-stu-id="da4c1-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="da4c1-123">支出データは 1 *日に1回更新* されます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="da4c1-124">Azure portal でアカウントの設定を変更しない限り、お客様は Azure のサービスとリソースを引き続き使用できます (料金が発生します)。</span><span class="sxs-lookup"><span data-stu-id="da4c1-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="da4c1-125">Azure の支出予算を設定する</span><span class="sxs-lookup"><span data-stu-id="da4c1-125">Set Azure spending budget</span></span>

<span data-ttu-id="da4c1-126">パートナーセンターでは、複数の顧客に対する *月単位の Azure 支出予算を設定* できます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="da4c1-127">[パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="da4c1-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="da4c1-128">[ **CSP**] の左側のメニューで、[ **Azure の支出**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="da4c1-129">[ **Azure** の使用量] ページの [ **Microsoft Azure サブスクリプションを持つ顧客**] で、予算を設定する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="da4c1-130">**月単位の予算** の値を入力します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-130">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="da4c1-131">[ **適用** ] を選択して変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="da4c1-132">また、サブスクリプション設定で *個々の顧客の予算を設定* することもできます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="da4c1-133">パートナー センター ダッシュボードにサインインします。</span><span class="sxs-lookup"><span data-stu-id="da4c1-133">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="da4c1-134">[ **CSP**] の左側のメニューで、[ **Customers**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="da4c1-135">[ **顧客** ] ページで、顧客の **会社名** を選択します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-135">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="da4c1-136">顧客の [ **サブスクリプション** ] ページの [ **使用量ベースのサブスクリプション**] で、[ **予算の変更**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="da4c1-137">予算の値を入力します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-137">Enter a value for the budget.</span></span>

6. <span data-ttu-id="da4c1-138">[ **適用** ] を選択して変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="da4c1-139">Azure の支出予算の削除</span><span class="sxs-lookup"><span data-stu-id="da4c1-139">Remove Azure spending budget</span></span>

<span data-ttu-id="da4c1-140">パートナーセンターでは、お客様の *月単位の Azure 支出予算を削除* できます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="da4c1-141">[パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="da4c1-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="da4c1-142">[ **CSP**] の左側のメニューで、[ **Azure の支出**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="da4c1-143">[ **Azure** の使用量] ページの [ **Microsoft Azure サブスクリプションを持つ顧客**] で、予算を削除する顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="da4c1-144">[ **予算の削除**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="da4c1-145">現在の Azure の支出を確認する</span><span class="sxs-lookup"><span data-stu-id="da4c1-145">Check current Azure spending</span></span>

<span data-ttu-id="da4c1-146">*お客様の現在の Azure の支出と月々の予算* をいつでも追跡できます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="da4c1-147">[パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="da4c1-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="da4c1-148">[ **CSP**] の左側のメニューで、[ **Azure の支出**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="da4c1-149">[ **Azure** の使用量] ページで、[ **Microsoft Azure のサブスクリプションをお持ちのお客様**] の下に、顧客の月々の予算、現在の支出見積もり、使用された予算の割合の概要が表示されます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="da4c1-150">予算制限の通知</span><span class="sxs-lookup"><span data-stu-id="da4c1-150">Notifications for budget limits</span></span>

<span data-ttu-id="da4c1-151">お客様の月々の支出が予算制限に近づいたときに、 *電子メール通知を有効* にすることができます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="da4c1-152">このオプションをオンにすると、顧客が80% 以上の月間予算を使用した場合に通知が表示されます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="da4c1-153">このオプションを使用すると、Azure の課金内容を監視できます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="da4c1-154">電子メール通知を構成するには:</span><span class="sxs-lookup"><span data-stu-id="da4c1-154">To configure email notifications:</span></span>

1. <span data-ttu-id="da4c1-155">パートナー センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="da4c1-155">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="da4c1-156">**[設定]** に移動します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-156">Go to **Settings**.</span></span>

3. <span data-ttu-id="da4c1-157">[ **個人用設定**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-157">Select **My preferences**.</span></span>

4. <span data-ttu-id="da4c1-158">お持ちでない場合は、優先する電子メールアドレスを構成します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-158">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="da4c1-159">通知の優先言語を構成します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-159">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="da4c1-160">[**通知の設定**] セクションの [ **CSP** ] タブを選択します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-160">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="da4c1-161">**Azure** の使用量に関する通知の電子メールオプションを確認し、**保存** します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-161">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="da4c1-162">サービス別コストの明細</span><span class="sxs-lookup"><span data-stu-id="da4c1-162">Itemized costs by service</span></span>

<span data-ttu-id="da4c1-163">*使用状況に基づいたサブスクリプションのサービスごとに、明細のコスト (および推定使用量) を表示* できます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-163">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="da4c1-164">パートナー センターにサインインします。</span><span class="sxs-lookup"><span data-stu-id="da4c1-164">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="da4c1-165">[ **CSP**] の左側のメニューで、[ **Customers**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-165">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="da4c1-166">[ **顧客** ] ページで、顧客の **会社名** を選択します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-166">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="da4c1-167">顧客の [ **サブスクリプション** ] ページの [ **使用量ベースのサブスクリプション**] で、 **サブスクリプション** の名前を選択します。</span><span class="sxs-lookup"><span data-stu-id="da4c1-167">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="da4c1-168">サブスクリプションのページで、サービスごとの **明細コスト** と当月の **推定使用量** を確認できます。</span><span class="sxs-lookup"><span data-stu-id="da4c1-168">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
