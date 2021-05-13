---
title: パートナー センター Analytics for Power BI のインストール
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: この記事の手順に従って、(CSP の直接パートナー向け) Power BI 用パートナー センター分析アプリをインストールしてプレビューします。
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 15ee391d6b748b6499700aee321ff4abd85e75d2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854487"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Power BI 用パートナー センター分析アプリをインストールしてプレビューする


**適切なロール**: グローバル管理者|ユーザー管理管理者|Sales Agent |管理エージェント

## <a name="before-you-begin"></a>開始する前に

使用可能な Power BI アプリの次の一覧から、自分のビジネスに最も関係のあるアプリケーションを選択します。

- [ダイレクト プロバイダー](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [間接プロバイダー](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [間接リセラー](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

パートナー センター分析アプリのプレビュー バージョンをインストールする前に、次の要件を満たしていることを確認してください。

- 自分のビジネスに合った Power BI アプリを選択している。

- お持ちPower BI Pro ライセンスをお持ちです。

- テナントにテンプレート アプリをインストールするアクセス許可があります。

- Power BI にログインできる。

- グローバル管理者、管理者エージェント、または課金管理者として、会社の Azure Active Directory [(Azure AD)](azure-active-directory-tenants-and-partner-center.md)テナント にサインインできます。

## <a name="to-install-the-app"></a>アプリをインストールするには

1. 上記のセクションで指定したアプリ ソース リンク (ダイレクト プロバイダー/間接プロバイダー/間接リセラー) を選択します。

2. **[今すぐ入手する]** を選択します。 

3. [続行] を選択して使用条件に **同意します**。

4. [アカウントを既にお持ちの場合] の下で **[サインイン]** を選びます。

5. 次のページで Power BI のユーザー名とパスワードを入力し、**[サインイン]** を選びます。

6. ワークスペース名を指定して、ワークスペースをインストールします。

7. インストールされているテンプレート アプリは、[アプリ] セクションで確認できます。

8. [アプリ **] を** 選択し、インストールされているアプリを選択します。

9. 開始するアプリの画面が開きます。

10. データに接続するには、 [接続] を **選択します**。

11. [パートナー センター **Analytics** に接続する] ポップアップ ウィンドウで、[認証方法] が **[oAuth2]** に設定されているのを確認するか、一覧から **[oAuth2]** を選択します (設定されていない場合)。 

> [!NOTE]  
>  このウィンドウが表示されるまでに数分間かかることがあります。

12. **[パートナー センター Analytics Connector]** ページで、会社の Azure AD テナントのグローバル管理者、管理者エージェント、または課金管理者の資格情報でサインインし、[サインイン]**を選択します**。
 
13. アクセスするかどうかを尋ねられたら、**[同意する]** を選びます。 

パートナー センターの分析サービスが Power BI に接続されると、データの読み込みが開始します。 データ量によっては、この読み込みに最大 10 分間かかります。 

データの読み込みが完了すると、Power BI でパートナー センターの分析アプリのダッシュボードとレポートを使用できるようになります。

## <a name="next-steps"></a>次の手順

[Microsoft Power BI 用パートナー センター分析アプリでビジネス データを表示する](power-bi-app-for-direct-partners-use.md)
