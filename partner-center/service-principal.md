---
title: Azure AD サービス プリンシパル |パートナー センター
ms.topic: article
ms.date: 12/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure AD テナントにサービス プリンシパルを追加する
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, Azure プラン, サービス プリンシパル, Azure AD アプリケーション
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: bd74d09445d9a2f1745c518362b26f243f00a777
ms.sourcegitcommit: 780776ee32f20d03101a4ee39ee2dc985541d7c1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/07/2020
ms.locfileid: "75716893"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>パートナー センターで Azure AD アプリケーション (サービス プリンシパル) を追加する

パートナー センターのコマーシャル マーケットプレース プログラムでは、Azure AD アプリケーション (サービス プリンシパル) を パートナー センター アカウントのユーザーとして追加できるようになりました。 (これは、以前は Cloud パートナー ポータル (CPP) アカウントで実行できましたが、パートナー センターに移行したため、CPP アカウントは読み取り専用になりました。)サービス プリンシパルは Azure AD アプリケーションと同義であることに注意してください。

## <a name="add-an-azure-ad-application-service-principal"></a>Azure AD アプリケーション (サービス プリンシパル) を追加する

1. パートナー センター ダッシュボードで **[設定]** を選択し、 **[開発者向け設定]** を選択します。

2. **[ユーザー]** を選択し、 **[Azure AD アプリケーションの追加]** を選択します。

3. 既存の Azure AD アプリケーションを選択するか、新しいものを作成します。

4. 新しい Azure AD アプリケーションを作成する場合は、次の情報を含めます。  

  


**応答 URL**:これは、ユーザーが Azure AD アプリケーションを使用するためにサインインできる URL です。 

**アプリ ID の URI**:これは、Azure AD アプリケーションの論理識別子であり、シングル サインオン要求を Azure AD に送るときに提供されます。 

**セキュリティ ロール**:**マネージャー** (CPP の '所有者' ロールと同じ) と **開発者** (CPP の 'コントリビューター' ロールと同じ) のロールは、パートナー センターのコマーシャル マーケットプレース プログラムに適用され、この Azure AD アプリケーションに関連付けることができます。  

  
