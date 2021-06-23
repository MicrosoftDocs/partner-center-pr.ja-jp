---
title: 顧客とのリセラー関係を削除する
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft の直接パートナーがリストから顧客を削除し、委任された管理者特権を削除し、顧客のサポートや購入を停止する方法について説明します。
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 83259f2f895be9ef34c55db5613ccfe6891a4424
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551471"
---
# <a name="how-to-remove-a-reseller-relationship-with-a-customer-in-partner-center"></a><span data-ttu-id="a093e-103">パートナー センターで顧客との再販業者関係を削除する方法</span><span class="sxs-lookup"><span data-stu-id="a093e-103">How to remove a reseller relationship with a customer in Partner Center</span></span>

<span data-ttu-id="a093e-104">**適切なロール**: グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="a093e-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="a093e-105">この記事では、顧客とのリセラー関係を削除する方法について説明パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="a093e-105">This article describes how to remove a reseller relationship with a customer in Partner Center.</span></span>

<span data-ttu-id="a093e-106">直接パートナーまたは間接プロバイダー: 顧客と取引しなくなった場合は、顧客との関係を削除パートナー センター。</span><span class="sxs-lookup"><span data-stu-id="a093e-106">Direct partners or Indirect providers: if you're no longer transacting with a customer, you can remove the relationship in Partner Center.</span></span>

<span data-ttu-id="a093e-107">関係を削除すると、次のような結果になります。</span><span class="sxs-lookup"><span data-stu-id="a093e-107">Removing a relationship has the following consequences:</span></span>

- <span data-ttu-id="a093e-108">パートナー様のパートナー センターの顧客の一覧から顧客が削除されます。</span><span class="sxs-lookup"><span data-stu-id="a093e-108">Removes the customer from your list of customers in Partner Center</span></span>
- <span data-ttu-id="a093e-109">顧客に対して利用可能 [なサポート連絡先の一覧から](assign-support-contacts.md) ユーザーを削除します</span><span class="sxs-lookup"><span data-stu-id="a093e-109">Removes you from the [list of available support contacts](assign-support-contacts.md) for your customer</span></span>
- <span data-ttu-id="a093e-110">顧客に対するパートナー様の代理管理者権限が削除されます。</span><span class="sxs-lookup"><span data-stu-id="a093e-110">Removes your delegation admin privileges for the customer</span></span>
- <span data-ttu-id="a093e-111">その顧客に対してそれ以降購入を行うことができなくなります</span><span class="sxs-lookup"><span data-stu-id="a093e-111">Prevents you from making future purchases for the customer</span></span>

## <a name="how-to-remove-a-relationship"></a><span data-ttu-id="a093e-112">リレーションシップを削除する方法</span><span class="sxs-lookup"><span data-stu-id="a093e-112">How to remove a relationship</span></span>

<span data-ttu-id="a093e-113">リレーションシップを削除するには、Azure 予約インスタンス (RI) の予約を取り消し、ソフトウェアの購入を取り消し、残りのアクティブなサブスクリプションを最初に中断する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a093e-113">To remove the relationship, you'll need to cancel Azure reserved instance (RI) reservations, cancel software purchases, and suspend any remaining active subscriptions first.</span></span>

1. <span data-ttu-id="a093e-114">**すべてのアクティブなサブスクリプションを中断します。**</span><span class="sxs-lookup"><span data-stu-id="a093e-114">**Suspend any active subscriptions.**</span></span>

   1. <span data-ttu-id="a093e-115">[顧客] パートナー センター[顧客] に **移動し** 、顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="a093e-115">From the Partner Center, go to **Customers** and select a customer</span></span>

   2. <span data-ttu-id="a093e-116">[ **サブスクリプション] で**、サブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="a093e-116">Under **Subscriptions**, select a subscription.</span></span>

   3. <span data-ttu-id="a093e-117">[ **中断] を選択します**</span><span class="sxs-lookup"><span data-stu-id="a093e-117">Select **Suspended**</span></span>

   4. <span data-ttu-id="a093e-118">アクティブなサブスクリプションごとにこれらの手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="a093e-118">Repeat these steps for each active subscription.</span></span>

2. <span data-ttu-id="a093e-119">**パートナー センターで関係を削除します。**</span><span class="sxs-lookup"><span data-stu-id="a093e-119">**Remove the relationship in Partner Center:**</span></span>

   <span data-ttu-id="a093e-120">a.</span><span class="sxs-lookup"><span data-stu-id="a093e-120">a.</span></span> <span data-ttu-id="a093e-121">[顧客] パートナー センター[顧客] に **移動し** 、顧客を選択します。</span><span class="sxs-lookup"><span data-stu-id="a093e-121">From the Partner Center, go to **Customers** and select a customer.</span></span>

   <span data-ttu-id="a093e-122">b.</span><span class="sxs-lookup"><span data-stu-id="a093e-122">b.</span></span> <span data-ttu-id="a093e-123">**[アカウント]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a093e-123">Select the **Account**.</span></span>

   <span data-ttu-id="a093e-124">c.</span><span class="sxs-lookup"><span data-stu-id="a093e-124">c.</span></span> <span data-ttu-id="a093e-125">[リセラー **リレーションシップの削除] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="a093e-125">Select **Remove reseller relationship**.</span></span>

   > [!NOTE]
   > <span data-ttu-id="a093e-126">サブスクリプションがまだアクティブな場合、[リセラーリレーションシップの **削除] リンク** は非アクティブになります。</span><span class="sxs-lookup"><span data-stu-id="a093e-126">If any subscriptions are still active, the **Remove reseller relationship** link will be inactive.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a093e-127">次の手順</span><span class="sxs-lookup"><span data-stu-id="a093e-127">Next steps</span></span>

- [<span data-ttu-id="a093e-128">顧客との関係を要求または再確立する</span><span class="sxs-lookup"><span data-stu-id="a093e-128">Request or re-establish a relationship with a customer</span></span>](request-a-relationship-with-a-customer.md)
