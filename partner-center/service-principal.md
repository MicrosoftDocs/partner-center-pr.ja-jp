---
title: Azure AD サービス プリンシパル
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: サービス プリンシパルを Azure AD テナント追加する方法を確認します。 そのようにすることによってパートナー センターで Azure AD アプリケーション (サービス プリンシパル) が追加されます。
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ef5373fd9a606cd25345cbe80a55f28fc1f753f
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028470"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>パートナー センターで Azure AD アプリケーション (サービス プリンシパル) を追加する

**適切なロール**

- グローバル管理者

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

## <a name="next-steps"></a>次の手順

- [パートナー センターのコマーシャル マーケットプレースの概要](csp-commercial-marketplace-overview.md)