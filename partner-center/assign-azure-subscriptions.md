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
ms.openlocfilehash: 02bd7ca573be4b0b61da546f66c6102fbc752c2d
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527688"
---
# <a name="assigning-azure-subscriptions-to-customers-in-partner-center"></a><span data-ttu-id="b240b-103">パートナー センターで顧客に Azure サブスクリプションを割り当てる</span><span class="sxs-lookup"><span data-stu-id="b240b-103">Assigning Azure subscriptions to customers in Partner Center</span></span>

<span data-ttu-id="b240b-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="b240b-104">**Applies to**</span></span>

- <span data-ttu-id="b240b-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="b240b-105">Partner Center</span></span>

## <a name="assign-azure-subscriptions-to-your-customers"></a><span data-ttu-id="b240b-106">顧客に Azure サブスクリプションを割り当てる</span><span class="sxs-lookup"><span data-stu-id="b240b-106">Assign Azure subscriptions to your customers</span></span>

1. <span data-ttu-id="b240b-107">**パートナー センター** メニューから **[顧客]** を選択し、管理対象の顧客を検索します。</span><span class="sxs-lookup"><span data-stu-id="b240b-107">Select **Customers** from your **Partner Center** menu and locate the customer you want to manage.</span></span>

2. <span data-ttu-id="b240b-108">行の末尾にある下向き矢印を選択して顧客レコードを展開し、**[Microsoft Azure の管理ポータル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b240b-108">Select the down arrow at the end of the row to expand the customer's record and then select **Microsoft Azure Management Portal**.</span></span> <span data-ttu-id="b240b-109">顧客のサブスクリプションを管理できる[Azure portal](https://portal.azure.com/)が表示されます。</span><span class="sxs-lookup"><span data-stu-id="b240b-109">You will be directed to the [Azure portal](https://portal.azure.com/) where you can manage the customer's subscriptions.</span></span>

3. <span data-ttu-id="b240b-110">Azure Portal から、**[サブスクリプション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b240b-110">From the Azure portal, select **Subscriptions**.</span></span>

4. <span data-ttu-id="b240b-111">割り当てるサブスクリプションを選択し、**[アクセス制御]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b240b-111">Select the subscription you would like to assign, then select **Access Control**.</span></span>

5. <span data-ttu-id="b240b-112">**[追加]** を選択して、サブスクリプションにユーザーを追加します。</span><span class="sxs-lookup"><span data-stu-id="b240b-112">Select **Add** to add a user to the subscription.</span></span> 

6. <span data-ttu-id="b240b-113">ユーザーをサブスクリプションに追加したら、そのユーザーに対して、ロールと、そのユーザーからアクセスできるようにする特定のアカウントを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="b240b-113">After you add the user to the subscription, you can assign the user a role and the specific account that user will have access to.</span></span>

## <a name="enable-customers-to-manage-their-azure-subscriptions"></a><span data-ttu-id="b240b-114">顧客が Azure サブスクリプションを管理できるようにする</span><span class="sxs-lookup"><span data-stu-id="b240b-114">Enable customers to manage their Azure subscriptions</span></span>

<span data-ttu-id="b240b-115">顧客の Microsoft Azure サブスクリプションを作成すると、サブスクリプションを有効にして管理することができます。</span><span class="sxs-lookup"><span data-stu-id="b240b-115">After you create a Microsoft Azure subscription for a customer, you can enable them to manage the subscription.</span></span> <span data-ttu-id="b240b-116">これを行うには、顧客の Microsoft Azure 管理ポータルにログオンする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b240b-116">To do this, you'll need to log on to the customer's Microsoft Azure Management portal.</span></span> 

1. <span data-ttu-id="b240b-117">顧客の Azure portal を開くには、顧客リスト内の顧客の一覧を展開するか、顧客の名前を選択し、[ **Microsoft Azure の管理ポータル**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b240b-117">To open the customer's Azure portal, either expand the customer's listing in your customer list or select the customer's name and then select **Microsoft Azure Management Portal**.</span></span>

   > [!NOTE]  
   > <span data-ttu-id="b240b-118">Azure portal にログオンするように求められた場合は、管理者特権が委任されていない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b240b-118">If you are prompted to log onto the Azure portal, you may not have delegated administrative privileges.</span></span> <span data-ttu-id="b240b-119">**[関係を要求する]** を選択し、指名パートナーとして指定するよう顧客を招待します。</span><span class="sxs-lookup"><span data-stu-id="b240b-119">Select **Request a relationship** to invite the customer to identify you as their Partner of Record.</span></span> <span data-ttu-id="b240b-120">顧客が招待を受け入れると、代理管理者権限が自動的に付与されます。</span><span class="sxs-lookup"><span data-stu-id="b240b-120">After the customer accepts your invitation, you are automatically granted delegated administrative privileges.</span></span>

2. <span data-ttu-id="b240b-121">Azure portal で、顧客のサブスクリプション一覧を開き、顧客の Azure サブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="b240b-121">In the Azure portal, open the customer's subscriptions list and select the customer's Azure subscription.</span></span>

3. <span data-ttu-id="b240b-122">顧客のユーザーにロールを割り当てて、サブスクリプションのリソースを作成して管理できるようにします。</span><span class="sxs-lookup"><span data-stu-id="b240b-122">Assign a role to any of the customer's users so that they can create and manage resources under their subscription.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b240b-123">次の手順</span><span class="sxs-lookup"><span data-stu-id="b240b-123">Next steps</span></span>

- [<span data-ttu-id="b240b-124">CSP パートナーが顧客にサブスクリプションを販売する方法</span><span class="sxs-lookup"><span data-stu-id="b240b-124">How CSP partners can sell subscriptions to customers</span></span>](customer-subscriptions.md)

- [<span data-ttu-id="b240b-125">顧客のサービスまたはサブスクリプションを管理するためのアクセス許可を取得する方法</span><span class="sxs-lookup"><span data-stu-id="b240b-125">How to obtain permissions to manage a customer's service or subscriptions</span></span>](customers-revoke-admin-privileges.md)
