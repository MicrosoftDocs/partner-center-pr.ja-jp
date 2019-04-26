---
title: Power BI 用パートナー センター分析アプリをインストールしてプレビューする | パートナー センター
ms.topic: article
ms.date: 03/15/2019
description: Power BI 用パートナー センター分析アプリ (CSP の直接パートナー向け) をプレビューするには、次の手順に従います。
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 10a47f22fb3716e8ff162e7b936770a2ca8a8ffc
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134652"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Power BI 用パートナー センター分析アプリをインストールしてプレビューする

**適用対象**

- パートナー センター

## <a name="before-you-begin"></a>始める前に

次の使用可能な Power BI アプリの一覧から、ビジネスに関係のあるアプリケーションを選択します。
- [パートナーの直接](https://app.powerbi.com/groups/me/getdata/services/direct-providers-partner-analytics)

- [間接的なパートナー](https://app.powerbi.com/groups/me/getdata/services/indirect-providers-partner-analytics)

- [間接リセラー](https://app.powerbi.com/groups/me/getdata/services/indirect-seller-partner-analytics)

パートナー センター分析アプリのプレビュー バージョンをインストールする前に、次の要件を満たしていることを確認してください。

- お客様のビジネスには、正しい Power BI アプリを選択します。

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

[Microsoft Power BI 用のパートナー センターの Analytics のアプリで、ビジネス データを表示します。](power-bi-app-for-direct-partners-use.md)
