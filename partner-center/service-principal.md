---
title: Azure AD サービス プリンシパル
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: サービス プリンシパルを Azure AD テナント追加する方法を確認します。 そのようにすることによってパートナー センターで Azure AD アプリケーション (サービス プリンシパル) が追加されます。
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 9d0507b684b213e6da5f48a250e6e61f395fd52a
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436431"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>パートナー センターで Azure AD アプリケーション (サービス プリンシパル) を追加する

パートナー センターのコマーシャル マーケットプレース プログラムでは、Azure AD アプリケーション (サービス プリンシパル) を パートナー センター アカウントのユーザーとして追加できるようになりました。 (以前は、Cloud パートナー ポータルまたは CPP のアカウントでこれを行うことができました。 パートナーセンターに移行されたため、CPP アカウントは読み取り専用になります)。
 
>[!Note] 
>サービス プリンシパルは、Azure AD アプリケーションと同義です。

## <a name="add-an-azure-ad-application-service-principal"></a>Azure AD アプリケーション (サービス プリンシパル) を追加する

1. パートナー センター ダッシュボードで **[設定]** を選択し、 **[開発者向け設定]** を選択します。

2. **[ユーザー]** を選択し、 **[Azure AD アプリケーションの追加]** を選択します。

3. 既存の Azure AD アプリケーションを選択するか、新しいものを作成します。

4. 新しい Azure AD アプリケーションを作成する場合は、次の情報を含めます。  

   - **応答 URL**:ユーザーが Azure AD アプリケーションを使用するためにサインインできる URL です。

   - **アプリ ID の URI**:Azure AD アプリケーションの論理識別子であり、シングル サインオン要求を Azure AD に送るときに提供されます。

   - **セキュリティ ロール**:**マネージャー** (CPP の '所有者' ロールと同じ) と **開発者** (CPP の 'コントリビューター' ロールと同じ) のロールは、パートナー センターのコマーシャル マーケットプレース プログラムに適用され、この Azure AD アプリケーションに関連付けることができます。  
