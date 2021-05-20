---
title: Azure サブスクリプションを顧客に割り当てる
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナー センター で Azure サブスクリプションを顧客に割り当てる方法と、顧客が独自のサブスクリプションを管理する方法について説明します。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: aba4f97ad6a385c2a9e36c95354a9d53e38ba9e3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149980"
---
# <a name="assigning-azure-subscriptions-to-customers-in-partner-center"></a><span data-ttu-id="321ac-103">パートナー センターで顧客に Azure サブスクリプションを割り当てる</span><span class="sxs-lookup"><span data-stu-id="321ac-103">Assigning Azure subscriptions to customers in Partner Center</span></span>

<span data-ttu-id="321ac-104">**適切なロール**: グローバル管理者|セールス エージェント</span><span class="sxs-lookup"><span data-stu-id="321ac-104">**Appropriate roles**: Global admin | Sales agent</span></span>

## <a name="assign-azure-subscriptions-to-your-customers"></a><span data-ttu-id="321ac-105">顧客に Azure サブスクリプションを割り当てる</span><span class="sxs-lookup"><span data-stu-id="321ac-105">Assign Azure subscriptions to your customers</span></span>

1. <span data-ttu-id="321ac-106">**パートナー センター** メニューから **[顧客]** を選択し、管理対象の顧客を検索します。</span><span class="sxs-lookup"><span data-stu-id="321ac-106">Select **Customers** from your **Partner Center** menu and locate the customer you want to manage.</span></span>

2. <span data-ttu-id="321ac-107">行の末尾にある下向き矢印を選択して顧客レコードを展開し、**[Microsoft Azure の管理ポータル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="321ac-107">Select the down arrow at the end of the row to expand the customer's record and then select **Microsoft Azure Management Portal**.</span></span> <span data-ttu-id="321ac-108">顧客のサブスクリプションを [Azure portal](https://portal.azure.com/) 管理できるサブスクリプションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="321ac-108">You will be directed to the [Azure portal](https://portal.azure.com/) where you can manage the customer's subscriptions.</span></span>

3. <span data-ttu-id="321ac-109">Azure Portal から、**[サブスクリプション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="321ac-109">From the Azure portal, select **Subscriptions**.</span></span>

4. <span data-ttu-id="321ac-110">割り当てるサブスクリプションを選択し、**[アクセス制御]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="321ac-110">Select the subscription you would like to assign, then select **Access Control**.</span></span>

5. <span data-ttu-id="321ac-111">**[追加]** を選択して、サブスクリプションにユーザーを追加します。</span><span class="sxs-lookup"><span data-stu-id="321ac-111">Select **Add** to add a user to the subscription.</span></span> 

6. <span data-ttu-id="321ac-112">ユーザーをサブスクリプションに追加したら、そのユーザーに対して、ロールと、そのユーザーからアクセスできるようにする特定のアカウントを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="321ac-112">After you add the user to the subscription, you can assign the user a role and the specific account that user will have access to.</span></span>

## <a name="enable-customers-to-manage-their-azure-subscriptions"></a><span data-ttu-id="321ac-113">顧客が Azure サブスクリプションを管理できるようにする</span><span class="sxs-lookup"><span data-stu-id="321ac-113">Enable customers to manage their Azure subscriptions</span></span>

<span data-ttu-id="321ac-114">顧客の Microsoft Azure サブスクリプションを作成すると、サブスクリプションを有効にして管理することができます。</span><span class="sxs-lookup"><span data-stu-id="321ac-114">After you create a Microsoft Azure subscription for a customer, you can enable them to manage the subscription.</span></span> <span data-ttu-id="321ac-115">これを行うには、顧客の管理ポータルにログオンMicrosoft Azureがあります。</span><span class="sxs-lookup"><span data-stu-id="321ac-115">To do this, you'll need to log on to the customer's Microsoft Azure Management portal.</span></span> 

1. <span data-ttu-id="321ac-116">顧客の顧客リストを開Azure portal顧客の一覧で顧客の一覧を展開するか、顧客の名前を選択し、[ ] を選択 **Microsoft Azure の管理ポータル。**</span><span class="sxs-lookup"><span data-stu-id="321ac-116">To open the customer's Azure portal, either expand the customer's listing in your customer list or select the customer's name and then select **Microsoft Azure Management Portal**.</span></span>

   > [!NOTE]  
   > <span data-ttu-id="321ac-117">サーバーにログオンするように求めるメッセージが表示Azure portal、委任された管理特権が付与されていない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="321ac-117">If you are prompted to log onto the Azure portal, you may not have delegated administrative privileges.</span></span> <span data-ttu-id="321ac-118">**[関係を要求する]** を選択し、指名パートナーとして指定するよう顧客を招待します。</span><span class="sxs-lookup"><span data-stu-id="321ac-118">Select **Request a relationship** to invite the customer to identify you as their Partner of Record.</span></span> <span data-ttu-id="321ac-119">顧客が招待を受け入れると、代理管理者権限が自動的に付与されます。</span><span class="sxs-lookup"><span data-stu-id="321ac-119">After the customer accepts your invitation, you are automatically granted delegated administrative privileges.</span></span>

2. <span data-ttu-id="321ac-120">[サブスクリプションAzure portal顧客のサブスクリプションの一覧を開き、顧客の Azure サブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="321ac-120">In the Azure portal, open the customer's subscriptions list and select the customer's Azure subscription.</span></span>

3. <span data-ttu-id="321ac-121">サブスクリプションでリソースを作成および管理できるよう、顧客のユーザーにロールを割り当てる。</span><span class="sxs-lookup"><span data-stu-id="321ac-121">Assign a role to any of the customer's users so that they can create and manage resources under their subscription.</span></span>

## <a name="next-steps"></a><span data-ttu-id="321ac-122">次のステップ</span><span class="sxs-lookup"><span data-stu-id="321ac-122">Next steps</span></span>

- [<span data-ttu-id="321ac-123">CSP パートナーが顧客にサブスクリプションを販売する方法</span><span class="sxs-lookup"><span data-stu-id="321ac-123">How CSP partners can sell subscriptions to customers</span></span>](customer-subscriptions.md)

- [<span data-ttu-id="321ac-124">顧客のサービスまたはサブスクリプションを管理するためのアクセス許可を取得する方法</span><span class="sxs-lookup"><span data-stu-id="321ac-124">How to obtain permissions to manage a customer's service or subscriptions</span></span>](customers-revoke-admin-privileges.md)
