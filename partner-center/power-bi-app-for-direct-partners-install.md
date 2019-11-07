---
title: Power BI 用パートナー センター分析アプリをインストールしてプレビューする | パートナー センター
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Power BI 用パートナー センター分析アプリ (CSP の直接パートナー向け) をプレビューするには、次の手順に従います。
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: b7635e8d6fd9910123ac4113d467ae506e507793
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/06/2019
ms.locfileid: "73654179"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Power BI 用パートナー センター分析アプリをインストールしてプレビューする

**適用対象**

- パートナー センター

## <a name="before-you-begin"></a>始める前に

使用可能な Power BI アプリの次の一覧から、自分のビジネスに最も関係のあるアプリケーションを選択します。
- [直接パートナー](https://app.powerbi.com/groups/me/getdata/services/direct-providers-partner-analytics)

- [間接パートナー](https://app.powerbi.com/groups/me/getdata/services/indirect-providers-partner-analytics)

- [間接リセラー](https://app.powerbi.com/groups/me/getdata/services/indirect-seller-partner-analytics)

パートナー センター分析アプリのプレビュー バージョンをインストールする前に、次の要件を満たしていることを確認してください。

- 自分のビジネスに合った Power BI アプリを選択している。

- Microsoft Power BI Professional または Microsoft Power BI Premium のアクティブなサブスクリプションがある。

- Power BI にログインできる。

- [会社の Azure Active Directory (Azure AD) テナント](azure-active-directory-tenants-and-partner-center.md)に、グローバル管理者、管理エージェント、または課金管理者としてサインインできます。

## <a name="to-install-the-app"></a>アプリをインストールするには

1. [ここをクリック](https://app.powerbi.com/getdata/services/partneranalytics?cpcode=PartnerCenterAnalytics&getDataForceConnect=true&alwaysPromptForContentProviderCreds=true)して手順を開始します。

2. **[アカウントを既にお持ちの場合]** の下で **[サインイン]** を選びます。 

3. 次のページで Power BI のユーザー名とパスワードを入力し、 **[サインイン]** を選びます。 

4. **[Partner Center Analytics への接続]** ポップアップウィンドウで、 **[認証方法]** が **[oAuth2]** に設定されていることを確認するか、表示されていない場合は一覧から**oAuth2**を選択します。 

> [!NOTE]  
>  このウィンドウが表示されるまでに数分間かかることがあります。

5. **[Partner Center Analytics コネクタ]** ページで、会社の Azure AD テナントのグローバル管理者、管理エージェント、または課金管理者の資格情報を使用してサインインし、 **[サインイン]** を選択します。
 
6. アクセスするかどうかを尋ねられたら、 **[同意する]** を選びます。 

パートナー センターの分析サービスが Power BI に接続されると、データの読み込みが開始します。 データ量によっては、この読み込みに最大 10 分間かかります。 

データの読み込みが完了すると、Power BI でパートナー センターの分析アプリのダッシュボードとレポートを使用できるようになります。

## <a name="next-steps"></a>次のステップ

[Microsoft Power BI 用パートナー センター分析アプリでビジネス データを表示する](power-bi-app-for-direct-partners-use.md)
