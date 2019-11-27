---
title: CSP パートナー向けの Cloudyn 製 Azure Cost Management |パートナー センター
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Cloudyn web アプリを登録し、パートナーセンターで秘密キーを使用する方法について説明します。これにより、アプリを使用して、お客様の Azure の使用状況とコストを追跡することができます。
author: Janet
ms.author: janet
Keywords: Azure コスト管理アプリ, コストの管理, Web アプリ
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: b05f2085aad63f8a0e23fa44de97550d13053f86
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253296"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>Azure を販売する CSP パートナー様向けの Azure コスト管理アプリ  

**適用対象**

- パートナー センター
- クラウド ソリューション プロバイダー プログラム パートナー

**適切なロール**

- 全体管理者
- 管理エージェント

[Azure Cost Management の詳細情報](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>アンインストールの準備
Azure Cost Management を使用する前に、次の要件を満たしていることを確認してください。

- クラウド ソリューション プロバイダー プログラムのパートナー様であること。
- パートナー センター API Web アプリを作成できること。

## <a name="overview"></a>概要

Cloudyn は、お客様による Azure の使用量とその使用量に対するコストを追跡、管理できる Web アプリです。 このアプリは、パートナー センター API 経由で使用します。

## <a name="register-your-web-app-in-the-partner-center"></a>パートナー センターで Web アプリを登録する
パートナー センターで Azure Active Directory Web アプリを登録すると、アプリがパートナー センター API にアクセスできるようになります。 
1.  [全体管理者または管理エージェント アカウント](https://partnercenter.microsoft.com/pcv/dashboard/overview)を使って、[パートナー センター](create-user-accounts-and-set-permissions.md)にサインインします。
2.  **パートナー センター**から、 **[アカウント設定]** &gt; **[アプリ管理](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** を選択します。
3.  **[Web アプリ]** セクションで、 **[新しいアプリの追加]** をクリックします。
<br> **注**: 既にアプリを作成済みの場合は、手順 3 を省略することができます。
4.  登録する Web アプリの **商取引 ID** GUID と **アプリ ID** GUID をコピーして保存します。 Azure cost management アプリの 30 日間無料試用版を利用するには、両方の ID が必要です。

## <a name="add-a-secret-key-to-your-app"></a>アプリへの秘密鍵の追加
1. **[キーの追加]** ボタンの横のドロップ ダウンで、1 年間または 2 年間の期間を選択します。
2. **[キーの追加]** をクリックします。 
3. 秘密キーの値を書き留めて保存します。 この値は、30 日間無料試用版の利用に必要です。<br>
   > [!NOTE]  
   > アプリケーションの秘密キーは、有効期限の長いパスワードのようなものです。 後日使用できるように、安全な場所にキーの値を保存してください。

## <a name="next-steps"></a>次の手順
[30 日間無料試用版](https://go.microsoft.com/fwlink/?linkid=857895) をご利用ください。
試用を開始するには、次の情報が必要です。
- パートナー センターのログイン資格情報
- 商取引 ID GUID
- アプリ ID GUID
- アプリケーションの秘密キーの値
