---
title: Power BI 用のパートナーセンター分析のインストール
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: この記事の手順に従って、Power BI 用のパートナーセンター分析アプリ (CSP のダイレクトパートナー向け) をインストールしてプレビューします。
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ad0c2f3ee7d130c49dea6ba354e6794e29fd9e9f
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633694"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Power BI 用パートナー センター分析アプリをインストールしてプレビューする


**適切なロール**

- グローバル管理者
- ユーザー管理の管理者
- 販売代理店
- 管理エージェント

## <a name="before-you-begin"></a>開始する前に

使用可能な Power BI アプリの次の一覧から、自分のビジネスに最も関係のあるアプリケーションを選択します。

- [直接プロバイダー](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [間接プロバイダー](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [間接リセラー](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

パートナー センター分析アプリのプレビュー バージョンをインストールする前に、次の要件を満たしていることを確認してください。

- 自分のビジネスに合った Power BI アプリを選択している。

- Power BI pro ライセンスを持っている。

- テナントにテンプレートアプリをインストールするためのアクセス許可があります。

- Power BI にログインできる。

- [会社の Azure Active Directory (Azure AD) テナント](azure-active-directory-tenants-and-partner-center.md)に、グローバル管理者、管理エージェント、または課金管理者としてサインインできます。

## <a name="to-install-the-app"></a>アプリをインストールするには

1. 上記のセクションで、指定されたアプリソースリンク (Direct Provider/間接プロバイダ/間接リセラー) を選択します。

2. **[今すぐ入手する]** を選択します。 

3. [ **続行**] を選択して、使用条件に同意します。

4. [アカウントを既にお持ちの場合] の下で **[サインイン]** を選びます。

5. 次のページで Power BI のユーザー名とパスワードを入力し、**[サインイン]** を選びます。

6. ワークスペース名を指定して、ワークスペースをインストールします。

7. インストールされているテンプレートアプリは、[アプリ] セクションで確認できます。

8. [ **アプリ** ] を選択し、インストールされているアプリを選択します。

9. [新しいアプリの開始] 画面が開きます。

10. データに接続するには、[ **接続**] を選択します。

11. [ **Partner Center Analytics への接続** ] ポップアップウィンドウで、[ **認証方法** ] が [ **oAuth2** ] に設定されていることを確認するか、表示されていない場合は一覧から **oAuth2** を選択します。 

> [!NOTE]  
>  このウィンドウが表示されるまでに数分間かかることがあります。

12. [ **Partner Center Analytics コネクタ** ] ページで、会社の Azure AD テナントのグローバル管理者、管理エージェント、または課金管理者の資格情報を使用してサインインし、[ **サインイン**] を選択します。
 
13. アクセスするかどうかを尋ねられたら、**[同意する]** を選びます。 

パートナー センターの分析サービスが Power BI に接続されると、データの読み込みが開始します。 データ量によっては、この読み込みに最大 10 分間かかります。 

データの読み込みが完了すると、Power BI でパートナー センターの分析アプリのダッシュボードとレポートを使用できるようになります。

## <a name="next-steps"></a>次のステップ

[Microsoft Power BI 用パートナー センター分析アプリでビジネス データを表示する](power-bi-app-for-direct-partners-use.md)
