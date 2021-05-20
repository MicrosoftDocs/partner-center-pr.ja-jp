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
# <a name="assigning-azure-subscriptions-to-customers-in-partner-center"></a>パートナー センターで顧客に Azure サブスクリプションを割り当てる

**適切なロール**: グローバル管理者|セールス エージェント

## <a name="assign-azure-subscriptions-to-your-customers"></a>顧客に Azure サブスクリプションを割り当てる

1. **パートナー センター** メニューから **[顧客]** を選択し、管理対象の顧客を検索します。

2. 行の末尾にある下向き矢印を選択して顧客レコードを展開し、**[Microsoft Azure の管理ポータル]** を選択します。 顧客のサブスクリプションを [Azure portal](https://portal.azure.com/) 管理できるサブスクリプションが表示されます。

3. Azure Portal から、**[サブスクリプション]** を選択します。

4. 割り当てるサブスクリプションを選択し、**[アクセス制御]** を選択します。

5. **[追加]** を選択して、サブスクリプションにユーザーを追加します。 

6. ユーザーをサブスクリプションに追加したら、そのユーザーに対して、ロールと、そのユーザーからアクセスできるようにする特定のアカウントを割り当てることができます。

## <a name="enable-customers-to-manage-their-azure-subscriptions"></a>顧客が Azure サブスクリプションを管理できるようにする

顧客の Microsoft Azure サブスクリプションを作成すると、サブスクリプションを有効にして管理することができます。 これを行うには、顧客の管理ポータルにログオンMicrosoft Azureがあります。 

1. 顧客の顧客リストを開Azure portal顧客の一覧で顧客の一覧を展開するか、顧客の名前を選択し、[ ] を選択 **Microsoft Azure の管理ポータル。**

   > [!NOTE]  
   > サーバーにログオンするように求めるメッセージが表示Azure portal、委任された管理特権が付与されていない可能性があります。 **[関係を要求する]** を選択し、指名パートナーとして指定するよう顧客を招待します。 顧客が招待を受け入れると、代理管理者権限が自動的に付与されます。

2. [サブスクリプションAzure portal顧客のサブスクリプションの一覧を開き、顧客の Azure サブスクリプションを選択します。

3. サブスクリプションでリソースを作成および管理できるよう、顧客のユーザーにロールを割り当てる。

## <a name="next-steps"></a>次のステップ

- [CSP パートナーが顧客にサブスクリプションを販売する方法](customer-subscriptions.md)

- [顧客のサービスまたはサブスクリプションを管理するためのアクセス許可を取得する方法](customers-revoke-admin-privileges.md)
