---
title: Power BI 用のパートナーセンター分析のインストール
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: この記事の手順に従って、Power BI 用のパートナーセンター分析アプリ (CSP のダイレクトパートナー向け) をインストールしてプレビューします。
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7e2a1d17a7520cca1a6e1da540cc58d2d365d8cb
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679309"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Power BI 用パートナー センター分析アプリをインストールしてプレビューする

**適用対象**

- パートナー センター

**適切なロール**
-   グローバル管理者
-   ユーザー管理者
-   販売代理店
-   管理エージェント

## <a name="before-you-begin"></a>開始する前に

使用可能な Power BI アプリの次の一覧から、自分のビジネスに最も関係のあるアプリケーションを選択します。
- [直接プロバイダー](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [間接プロバイダー](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [間接リセラー](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

パートナー センター分析アプリのプレビュー バージョンをインストールする前に、次の要件を満たしていることを確認してください。

- 自分のビジネスに合った Power BI アプリを選択している。

- Power BI pro ライセンスを持っている。

- テナントにテンプレートアプリをインストールするためのアクセス許可があります。

- Power BI にログインできる。

- [会社の Azure Active Directory (Azure AD) テナント](azure-active-directory-tenants-and-partner-center.md)に、グローバル管理者、管理エージェント、または課金管理者としてサインインできます。

## <a name="to-install-the-app"></a>アプリをインストールするには

1. 上記のセクションで、指定されたアプリソースリンク (Direct Provider/間接プロバイダ/間接リセラー) をクリックします。

2. [**今すぐ入手**する] をクリックします。 

3. [**続行**] をクリックして使用条件に同意します。

4. [アカウントを既にお持ちの場合] の下で **[サインイン]** を選びます。

5. 次のページで Power BI のユーザー名とパスワードを入力し、[サインイン]を選びます。

6. Workspacename を指定して、ワークスペースをインストールします。

7. インストールされているテンプレートアプリは、[アプリ] セクションで確認できます。

8. [アプリ] をクリックし、インストールされているアプリを選択します。

9. [新しいアプリの開始] 画面が開きます。

10. データに接続するには、[**接続**] をクリックします。

11. [ **Partner Center Analytics への接続**] ポップアップウィンドウで、[**認証方法**] が [ **oAuth2** ] に設定されていることを確認するか、表示されていない場合は一覧から**oAuth2**を選択します。 

> [!NOTE]  
>  このウィンドウが表示されるまでに数分間かかることがあります。

12. [ **Partner Center Analytics コネクタ**] ページで、会社の Azure AD テナントのグローバル管理者、管理エージェント、または課金管理者の資格情報を使用してサインインし、[**サインイン**] を選択します。
 
13. アクセスするかどうかを尋ねられたら、**[同意する]** を選びます。 

パートナー センターの分析サービスが Power BI に接続されると、データの読み込みが開始します。 データ量によっては、この読み込みに最大 10 分間かかります。 

データの読み込みが完了すると、Power BI でパートナー センターの分析アプリのダッシュボードとレポートを使用できるようになります。

## <a name="next-steps"></a>次の手順

[Microsoft Power BI 用パートナー センター分析アプリでビジネス データを表示する](power-bi-app-for-direct-partners-use.md)
