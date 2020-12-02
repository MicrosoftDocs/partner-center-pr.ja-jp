---
title: Azure サブスクリプションを顧客に割り当てる
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターで顧客に Azure サブスクリプションを割り当てる方法と、顧客が自分のサブスクリプションを管理できるようにする方法について説明します。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8cac2a6edc9199befeae940ed271c3236440c260
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/01/2020
ms.locfileid: "96473953"
---
# <a name="assigning-azure-subscriptions-to-customers-in-partner-center"></a><span data-ttu-id="51a1a-103">パートナー センターで顧客に Azure サブスクリプションを割り当てる</span><span class="sxs-lookup"><span data-stu-id="51a1a-103">Assigning Azure subscriptions to customers in Partner Center</span></span>

<span data-ttu-id="51a1a-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="51a1a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="51a1a-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="51a1a-105">Global admin</span></span>
- <span data-ttu-id="51a1a-106">販売代理店</span><span class="sxs-lookup"><span data-stu-id="51a1a-106">Sales agent</span></span>

## <a name="assign-azure-subscriptions-to-your-customers"></a><span data-ttu-id="51a1a-107">顧客に Azure サブスクリプションを割り当てる</span><span class="sxs-lookup"><span data-stu-id="51a1a-107">Assign Azure subscriptions to your customers</span></span>

1. <span data-ttu-id="51a1a-108">**パートナー センター** メニューから **[顧客]** を選択し、管理対象の顧客を検索します。</span><span class="sxs-lookup"><span data-stu-id="51a1a-108">Select **Customers** from your **Partner Center** menu and locate the customer you want to manage.</span></span>

2. <span data-ttu-id="51a1a-109">行の末尾にある下向き矢印を選択して顧客レコードを展開し、**[Microsoft Azure の管理ポータル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="51a1a-109">Select the down arrow at the end of the row to expand the customer's record and then select **Microsoft Azure Management Portal**.</span></span> <span data-ttu-id="51a1a-110">顧客のサブスクリプションを管理できる [Azure portal](https://portal.azure.com/) が表示されます。</span><span class="sxs-lookup"><span data-stu-id="51a1a-110">You will be directed to the [Azure portal](https://portal.azure.com/) where you can manage the customer's subscriptions.</span></span>

3. <span data-ttu-id="51a1a-111">Azure Portal から、**[サブスクリプション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="51a1a-111">From the Azure portal, select **Subscriptions**.</span></span>

4. <span data-ttu-id="51a1a-112">割り当てるサブスクリプションを選択し、**[アクセス制御]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="51a1a-112">Select the subscription you would like to assign, then select **Access Control**.</span></span>

5. <span data-ttu-id="51a1a-113">**[追加]** を選択して、サブスクリプションにユーザーを追加します。</span><span class="sxs-lookup"><span data-stu-id="51a1a-113">Select **Add** to add a user to the subscription.</span></span> 

6. <span data-ttu-id="51a1a-114">ユーザーをサブスクリプションに追加したら、そのユーザーに対して、ロールと、そのユーザーからアクセスできるようにする特定のアカウントを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="51a1a-114">After you add the user to the subscription, you can assign the user a role and the specific account that user will have access to.</span></span>

## <a name="enable-customers-to-manage-their-azure-subscriptions"></a><span data-ttu-id="51a1a-115">顧客が Azure サブスクリプションを管理できるようにする</span><span class="sxs-lookup"><span data-stu-id="51a1a-115">Enable customers to manage their Azure subscriptions</span></span>

<span data-ttu-id="51a1a-116">顧客の Microsoft Azure サブスクリプションを作成すると、サブスクリプションを有効にして管理することができます。</span><span class="sxs-lookup"><span data-stu-id="51a1a-116">After you create a Microsoft Azure subscription for a customer, you can enable them to manage the subscription.</span></span> <span data-ttu-id="51a1a-117">これを行うには、顧客の Microsoft Azure 管理ポータルにログオンする必要があります。</span><span class="sxs-lookup"><span data-stu-id="51a1a-117">To do this, you'll need to log on to the customer's Microsoft Azure Management portal.</span></span> 

1. <span data-ttu-id="51a1a-118">顧客の Azure portal を開くには、顧客リスト内の顧客の一覧を展開するか、顧客の名前を選択し、[ **Microsoft Azure の管理ポータル**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="51a1a-118">To open the customer's Azure portal, either expand the customer's listing in your customer list or select the customer's name and then select **Microsoft Azure Management Portal**.</span></span>

   > [!NOTE]  
   > <span data-ttu-id="51a1a-119">Azure portal にログオンするように求められた場合は、管理者特権が委任されていない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="51a1a-119">If you are prompted to log onto the Azure portal, you may not have delegated administrative privileges.</span></span> <span data-ttu-id="51a1a-120">**[関係を要求する]** を選択し、指名パートナーとして指定するよう顧客を招待します。</span><span class="sxs-lookup"><span data-stu-id="51a1a-120">Select **Request a relationship** to invite the customer to identify you as their Partner of Record.</span></span> <span data-ttu-id="51a1a-121">顧客が招待を受け入れると、代理管理者権限が自動的に付与されます。</span><span class="sxs-lookup"><span data-stu-id="51a1a-121">After the customer accepts your invitation, you are automatically granted delegated administrative privileges.</span></span>

2. <span data-ttu-id="51a1a-122">Azure portal で、顧客のサブスクリプション一覧を開き、顧客の Azure サブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="51a1a-122">In the Azure portal, open the customer's subscriptions list and select the customer's Azure subscription.</span></span>

3. <span data-ttu-id="51a1a-123">顧客のユーザーにロールを割り当てて、サブスクリプションのリソースを作成して管理できるようにします。</span><span class="sxs-lookup"><span data-stu-id="51a1a-123">Assign a role to any of the customer's users so that they can create and manage resources under their subscription.</span></span>

## <a name="next-steps"></a><span data-ttu-id="51a1a-124">次のステップ</span><span class="sxs-lookup"><span data-stu-id="51a1a-124">Next steps</span></span>

- [<span data-ttu-id="51a1a-125">CSP パートナーが顧客にサブスクリプションを販売する方法</span><span class="sxs-lookup"><span data-stu-id="51a1a-125">How CSP partners can sell subscriptions to customers</span></span>](customer-subscriptions.md)

- [<span data-ttu-id="51a1a-126">顧客のサービスまたはサブスクリプションを管理するためのアクセス許可を取得する方法</span><span class="sxs-lookup"><span data-stu-id="51a1a-126">How to obtain permissions to manage a customer's service or subscriptions</span></span>](customers-revoke-admin-privileges.md)
