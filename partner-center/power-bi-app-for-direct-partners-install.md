---
title: Power BI 用パートナー センター分析アプリをインストールしてプレビューする | パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: Power BI 用パートナー センター分析アプリ (CSP の直接パートナー向け) をプレビューするには、次の手順に従います。
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: ef641484ada5332a7129e13f8d7bbd8f1d269f96
ms.sourcegitcommit: 3871c82c1075206a33eae7cd395a5a36edb2d1fc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/08/2019
ms.locfileid: "8995556"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Power BI 用パートナー センター分析アプリをインストールしてプレビューする

**適用対象**

- パートナー センター

## <a name="before-you-begin"></a>開始する前に

次の Power BI の利用可能なアプリの一覧からお客様のビジネスに最も関連のあるアプリケーションを選択します。
- [直接パートナー](https://app.powerbi.com/groups/me/getdata/services/direct-providers-partner-analytics)

- [間接パートナー](https://app.powerbi.com/groups/me/getdata/services/indirect-providers-partner-analytics)

- [間接リセラー](https://app.powerbi.com/groups/me/getdata/services/indirect-seller-partner-analytics)

パートナー センター分析アプリのプレビュー バージョンをインストールする前に、次の要件を満たしていることを確認してください。

- ビジネス向けには、適切な Power BI アプリを選択します。

- Microsoft Power BI Professional または Microsoft Power BI Premium のアクティブなサブスクリプションがある。

- Power BI にログインできる。

- 全体管理者、管理エージェント、または課金管理者として[会社の Azure Active Directory (Azure AD) テナント](azure-active-directory-tenants-and-partner-center.md)にログインできる。

## <a name="to-install-the-app"></a>アプリをインストールするには

1. [ここをクリック](https://app.powerbi.com/getdata/services/partneranalytics?cpcode=PartnerCenterAnalytics&getDataForceConnect=true&alwaysPromptForContentProviderCreds=true)して手順を開始します。

2. **[アカウントを既にお持ちの場合]** の下で **[サインイン]** を選びます。 

3. 次のページで Power BI のユーザー名とパスワードを入力し、**[サインイン]** を選びます。 

4. **[Connect to Partner Center Analytics]** (パートナー センター分析に接続) ポップアップ ウィンドウで、**[認証方法]** が **[oAuth2]** に設定されていることを確認し、設定されていない場合は一覧から **[oAuth2]** を選びます。 

> [!NOTE]  
>  このウィンドウが表示されるまでに数分間かかることがあります。

5. **[Partner Center Analytics Connector]** (パートナー センターの分析コネクター) ページで、会社の Azure AD テナントの全体管理者、管理エージェント、または課金管理者の資格情報を使ってログインし、**[サインイン]** をクリックします。
 
6. アクセスするかどうかを尋ねられたら、**[同意する]** を選びます。 

パートナー センターの分析サービスが Power BI に接続されると、データの読み込みが開始します。 データ量によっては、この読み込みに最大 10 分間かかります。 

データの読み込みが完了すると、Power BI でパートナー センターの分析アプリのダッシュボードとレポートを使用できるようになります。

## <a name="next-steps"></a>次のステップ

[Microsoft Power BI 用パートナー センター分析アプリでビジネス データを表示する](power-bi-app-for-direct-partners-use.md)
