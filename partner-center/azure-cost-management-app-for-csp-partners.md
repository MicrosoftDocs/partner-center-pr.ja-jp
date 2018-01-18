---
title: "CSP パートナー向けの Cloudyn 製 Azure Cost Management |パートナー センター"
description: "Cloudyn が提供する Azure Cost Management を使用するには、パートナー センター API へのアクセスをプロビジョニングする必要があります。"
author: Janet
Keywords: Azure cost management app, manage costs, web apps
robots: 
ms.openlocfilehash: 3d122e0f88867d16df3713f79e735126b7f40dd4
ms.sourcegitcommit: 628443b08dde9d2f02553b46e669504c620c3da4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/21/2017
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>Azure を販売する CSP パートナー様向けの Azure コスト管理アプリ  

**適用対象**

-  パートナー センター

[Azure Cost Management の詳細情報を取得する](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>前提条件
Azure Cost Management を使用する前に、次の要件を満たしていることを確認してください。
- クラウド ソリューション プロバイダー プログラムのパートナー様であること。
- パートナー センター API Web アプリを作成できること。

## <a name="overview"></a>概要

Cloudyn が提供する Azure cost management は、お客様による Azure の使用量とその使用量に対応するコストを追跡、管理できる Web アプリです。 このアプリは、パートナー センター API 経由で使用します。

## <a name="register-your-web-app-in-partner-center"></a>パートナー センターで Web アプリを登録する
パートナー センターで Azure Active Directory Web アプリを登録すると、アプリがパートナー センター API にアクセスできるようになります。 
1.  [グローバル管理者または管理エージェント アカウント](create-user-accounts-and-set-permissions.md)を使って、[パートナー センター](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview)にサインインします。
2.  **[ダッシュボード]** で、**[アカウント設定]** &gt; **[[アプリ管理]](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)** を選びます。
3.  **[Web アプリ]** セクションで、**[新しいアプリの追加]** をクリックします。
<br> **注**: 既にアプリを作成済みの場合は、手順 3 を省略することができます。
4.  登録する Web アプリの **商取引 ID** GUID と **アプリ ID** GUID をコピーして保存します。 Azure cost management アプリの 30 日間無料試用版を利用するには、両方の ID が必要です。

## <a name="add-a-secret-key-to-your-app"></a>アプリへの秘密鍵の追加
1.  **[キーの追加]** ボタンの横のドロップ ダウンで、1 年間または 2 年間の期間を選択します。
2.  **[キーの追加]** をクリックします。 
3.  秘密キーの値を書き留めて保存します。 この値は、30 日間無料試用版の利用に必要です。
<br>**注**: アプリケーションの秘密キーは、有効期限の長いパスワードのようなものです。 後日使用できるように、安全な場所にキーの値を保存してください。

## <a name="next-steps"></a>次のステップ
[30 日間無料試用版](https://go.microsoft.com/fwlink/?linkid=857895) をご利用ください。
試用を開始するには、次の情報が必要です。
- パートナー センターのログイン資格情報
- 商取引 ID GUID
- アプリ ID GUID
- アプリケーションの秘密キーの値
