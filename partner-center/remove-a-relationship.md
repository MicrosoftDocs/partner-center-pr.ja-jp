---
title: リセラーと顧客との関係を削除する
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft direct パートナーが顧客を一覧から削除する方法、委任された管理者特権を削除する方法、顧客のサポートまたは購入を停止する方法について説明します。
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d6ff07d2c54d006478b290ad53c024a55dea4e18
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018103"
---
# <a name="how-to-remove-a-reseller-relationship-with-a-customer-in-partner-center"></a><span data-ttu-id="a324f-103">パートナー センターで顧客との再販業者関係を削除する方法</span><span class="sxs-lookup"><span data-stu-id="a324f-103">How to remove a reseller relationship with a customer in Partner Center</span></span>

<span data-ttu-id="a324f-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="a324f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a324f-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="a324f-105">Global admin</span></span>

<span data-ttu-id="a324f-106">この記事では、パートナーセンターで顧客との再販業者関係を削除する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="a324f-106">This article describes how to remove a reseller relationship with a customer in Partner Center.</span></span>

<span data-ttu-id="a324f-107">ダイレクトパートナーまたは間接プロバイダー: 顧客とのやり取りがなくなった場合は、パートナーセンターでリレーションシップを削除できます。</span><span class="sxs-lookup"><span data-stu-id="a324f-107">Direct partners or Indirect providers: if you're no longer transacting with a customer, you can remove the relationship in Partner Center.</span></span>

<span data-ttu-id="a324f-108">関係を削除すると、次のような結果になります。</span><span class="sxs-lookup"><span data-stu-id="a324f-108">Removing a relationship has the following consequences:</span></span>

- <span data-ttu-id="a324f-109">パートナー様のパートナー センターの顧客の一覧から顧客が削除されます。</span><span class="sxs-lookup"><span data-stu-id="a324f-109">Removes the customer from your list of customers in Partner Center</span></span>
- <span data-ttu-id="a324f-110">お客様の [利用可能なサポート連絡先の一覧](assign-support-contacts.md) から削除します。</span><span class="sxs-lookup"><span data-stu-id="a324f-110">Removes you from the [list of available support contacts](assign-support-contacts.md) for your customer</span></span>
- <span data-ttu-id="a324f-111">顧客に対するパートナー様の代理管理者権限が削除されます。</span><span class="sxs-lookup"><span data-stu-id="a324f-111">Removes your delegation admin privileges for the customer</span></span>
- <span data-ttu-id="a324f-112">その顧客に対してそれ以降購入を行うことができなくなります</span><span class="sxs-lookup"><span data-stu-id="a324f-112">Prevents you from making future purchases for the customer</span></span>

## <a name="how-to-remove-a-relationship"></a><span data-ttu-id="a324f-113">リレーションシップを削除する方法</span><span class="sxs-lookup"><span data-stu-id="a324f-113">How to remove a relationship</span></span>

<span data-ttu-id="a324f-114">リレーションシップを削除するには、Azure RI の予約をキャンセルし、ソフトウェアの購入を取り消し、残りのアクティブなサブスクリプションを最初に中断する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a324f-114">To remove the relationship, you'll need to cancel Azure RI reservations, cancel software purchases, and suspend any remaining active subscriptions first.</span></span>

1. <span data-ttu-id="a324f-115">**すべてのアクティブなサブスクリプションを中断します。**</span><span class="sxs-lookup"><span data-stu-id="a324f-115">**Suspend any active subscriptions.**</span></span>

   1. <span data-ttu-id="a324f-116">パートナーセンターから、[ **顧客** ] にアクセスして顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="a324f-116">From the Partner Center, go to **Customers** and select a customer</span></span>

   2. <span data-ttu-id="a324f-117">[ **サブスクリプション**] で、サブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="a324f-117">Under **Subscriptions**, select a subscription.</span></span>

   3. <span data-ttu-id="a324f-118">**中断** の選択</span><span class="sxs-lookup"><span data-stu-id="a324f-118">Select **Suspended**</span></span>

   4. <span data-ttu-id="a324f-119">アクティブなサブスクリプションごとに、これらの手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="a324f-119">Repeat these steps for each active subscription.</span></span>

2. <span data-ttu-id="a324f-120">**パートナー センターで関係を削除します。**</span><span class="sxs-lookup"><span data-stu-id="a324f-120">**Remove the relationship in Partner Center:**</span></span>

   <span data-ttu-id="a324f-121">a.</span><span class="sxs-lookup"><span data-stu-id="a324f-121">a.</span></span> <span data-ttu-id="a324f-122">パートナーセンターから、[ **顧客** ] にアクセスして顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="a324f-122">From the Partner Center, go to **Customers** and select a customer.</span></span>

   <span data-ttu-id="a324f-123">b.</span><span class="sxs-lookup"><span data-stu-id="a324f-123">b.</span></span> <span data-ttu-id="a324f-124">**[アカウント]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a324f-124">Select the **Account**.</span></span>

   <span data-ttu-id="a324f-125">c.</span><span class="sxs-lookup"><span data-stu-id="a324f-125">c.</span></span> <span data-ttu-id="a324f-126">[ **再販業者の関係を削除**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a324f-126">Select **Remove reseller relationship**.</span></span>

   > [!NOTE]
   > <span data-ttu-id="a324f-127">まだアクティブになっているサブスクリプションがある場合、[ **再販業者の関係を削除** する] リンクは非アクティブになります。</span><span class="sxs-lookup"><span data-stu-id="a324f-127">If any subscriptions are still active, the **Remove reseller relationship** link will be inactive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a324f-128">次のステップ</span><span class="sxs-lookup"><span data-stu-id="a324f-128">Next steps</span></span>

- [<span data-ttu-id="a324f-129">顧客との関係を要求または再確立する</span><span class="sxs-lookup"><span data-stu-id="a324f-129">Request or re-establish a relationship with a customer</span></span>](request-a-relationship-with-a-customer.md)
