---
title: Power BI 用パートナー センター分析アプリをインストールしてプレビューする | パートナー センター
description: Power BI 用パートナー センター分析アプリ (CSP の直接パートナー向け) をプレビューするには、次の手順に従います。
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 8dd91d16ffe5e49271dd3c5fe50e8910299f1a1c
ms.sourcegitcommit: 5b720c2ad126ec52564ad5264596ca1cf6a12489
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/05/2018
ms.locfileid: "4377514"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Power BI 用パートナー センター分析アプリをインストールしてプレビューする

**適用対象**

-   パートナー センター

## <a name="before-you-begin"></a>開始する前に

パートナー センター分析アプリのプレビュー バージョンをインストールする前に、次の要件を満たしていることを確認してください。

-   クラウド ソリューション プロバイダー プログラムの直接パートナーであり、パートナーセンターを使用している。 直接パートナーとは、マイクロソフトおよび顧客と直接取引するパートナーを指します。

-   Microsoft Power BI Professional または Microsoft Power BI Premium のアクティブなサブスクリプションがある。

-   Power BI にログインできる。

-   全体管理者、管理エージェント、または課金管理者として[会社の Azure Active Directory (Azure AD) テナント](azure-active-directory-tenants-and-partner-center.md)にログインできる。

## <a name="to-install-the-app"></a>アプリをインストールするには

1. [ここをクリック](https://app.powerbi.com/getdata/services/partneranalytics?cpcode=PartnerCenterAnalytics&getDataForceConnect=true&alwaysPromptForContentProviderCreds=true)して手順を開始します。

2. **[アカウントを既にお持ちの場合]** の下で **[サインイン]** を選びます。 

3.  次のページで Power BI のユーザー名とパスワードを入力し、**[サインイン]** を選びます。 

4.  **[Connect to Partner Center Analytics]** (パートナー センター分析に接続) ポップアップ ウィンドウで、**[認証方法]** が **[oAuth2]** に設定されていることを確認し、設定されていない場合は一覧から **[oAuth2]** を選びます。 

    > [!NOTE]  
>  このウィンドウが表示されるまでに数分間かかることがあります。

5.  **[Partner Center Analytics Connector]** (パートナー センターの分析コネクター) ページで、会社の Azure AD テナントの全体管理者、管理エージェント、または課金管理者の資格情報を使ってログインし、**[サインイン]** をクリックします。
 
6.  アクセスするかどうかを尋ねられたら、**[同意する]** を選びます。 

パートナー センターの分析サービスが Power BI に接続されると、データの読み込みが開始します。 データ量によっては、この読み込みに最大 10 分間かかります。 

データの読み込みが完了すると、Power BI でパートナー センターの分析アプリのダッシュボードとレポートを使用できるようになります。

## <a name="next-steps"></a>次のステップ

[Microsoft Power BI 用パートナー センター分析アプリでビジネス データを表示する](power-bi-app-for-direct-partners-use.md)
