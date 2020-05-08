---
title: Csp の Cloudyn による Azure Cost Management
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Cloudyn web アプリを登録し、パートナーセンターで秘密キーを使用する方法について説明します。これにより、アプリを使用して、お客様の Azure の使用状況とコストを追跡することができます。
author: LauraBrenner
ms.author: labrenne
Keywords: Azure コスト管理アプリ, コストの管理, Web アプリ
robots: ''
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0d88f37e0fe653c679df5729fa283336e4c7e144
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908370"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a>CSP パートナー向けの Azure cost management アプリを使用して、お客様の Azure の使用状況とコストを追跡します  

**適用対象**

- パートナー センター
- クラウド ソリューション プロバイダー プログラム パートナー

**適切なロール**

- グローバル管理者
- 管理エージェント

[Azure Cost Management の詳細情報](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>開始する前に
Azure Cost Management を使用する前に、次の要件を満たしていることを確認してください。

- クラウド ソリューション プロバイダー プログラムのパートナー様であること。
- パートナー センター API Web アプリを作成できること。

## <a name="overview"></a>概要

Cloudyn は、お客様による Azure の使用量とその使用量に対するコストを追跡、管理できる Web アプリです。 このアプリは、パートナー センター API 経由で使用します。

## <a name="register-your-web-app-in-the-partner-center"></a>パートナー センターで Web アプリを登録する
パートナー センターで Azure Active Directory Web アプリを登録すると、アプリがパートナー センター API にアクセスできるようになります。 
1.  [全体管理者または管理エージェント アカウント](create-user-accounts-and-set-permissions.md)を使って、[パートナー センター](https://partnercenter.microsoft.com/pcv/dashboard/overview)にサインインします。
2.  **パートナー センター**から、**[アカウント設定]** &gt; **[アプリ管理](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** を選択します。
3.  **[Web アプリ]** セクションで、**[新しいアプリの追加]** をクリックします。
<br> **注**: 既にアプリを作成済みの場合は、手順 3 を省略することができます。
4.  登録する Web アプリの **商取引 ID** GUID と **アプリ ID** GUID をコピーして保存します。 Azure cost management アプリの 30 日間無料試用版を利用するには、両方の ID が必要です。

## <a name="add-a-secret-key-to-your-app"></a>アプリへの秘密鍵の追加
1. **[キーの追加]** ボタンの横のドロップ ダウンで、1 年間または 2 年間の期間を選択します。
2. [**キーの追加**] をクリックします。 
3. 秘密キーの値を書き留めて保存します。 この値は、30 日間無料試用版の利用に必要です。<br>
   > [!NOTE]  
   > アプリケーションの秘密キーは、有効期限の長いパスワードのようなものです。 後日使用できるように、安全な場所にキーの値を保存してください。

## <a name="next-steps"></a>次のステップ
[30 日間無料試用版](https://go.microsoft.com/fwlink/?linkid=857895) をご利用ください。
試用を開始するには、次の情報が必要です。
- パートナー センターのログイン資格情報
- 商取引 ID GUID
- アプリ ID GUID
- アプリケーションの秘密キーの値
