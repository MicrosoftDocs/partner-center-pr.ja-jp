---
title: パートナー アカウントで場所を管理する
ms.topic: how-to
ms.date: 01/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 新しい場所を追加する方法や、所在地 MPN ID がインセンティブ プログラム、CSP ビジネス、サブスクリプション、その他のトランザクションでどのように使用されるかについて説明します。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38ea8a451f51d80998643e2a023420ea3efaa6ba
ms.sourcegitcommit: e99882e9b6c9b1a0f7427fb133693b1d977be76b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2021
ms.locfileid: "98773428"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>MPN アカウントの所在地を管理し、新しい場所を追加する


**適切なロール**

- グローバル管理者
- アカウント管理者

所在地 MPN ID では、貴社の特定の各場所が示されます。 所在地 MPN ID を使用して、インセンティブ プログラムに登録し、クラウド ソリューション プロバイダー (CSP) ビジネスの取引を行い、他のビジネス トランザクションを行います。 グローバル MPN ID は、サポート リクエストなどの非トランザクション アクティビティに使用されます。

## <a name="the-following-is-a-typical-scenario"></a>一般的なシナリオを示します。

Contoso のパートナー グローバル アカウント (PGA) の場所はイギリスです。 これは、登録された法的な事業所であり、そのグローバル MPN ID はすべての非トランザクション ビジネスを管理するために使用されます。 Contoso には、イギリスの別の場所、フランス、米国にある子会社または部門に相当するパートナー ロケーション アカウント (PLA) もあります。 MPN アカウントの構造では、これらの PLA は一意の所在地 MPN ID として表現されます。 PLA は、CSP またはインセンティブ プログラムなどのトランザクション ビジネスに使用されます。 支払いは、特定の場所に関連付けられます。 

>[!NOTE]
>CSP テナントと MPN 所在地 ID の間には 1 対 1 の関係があります。

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 所在地の構造":::

## <a name="prerequisites-in-order-to-add-a-new-account-location-for-a-csp-business"></a>CSP ビジネスの新しいアカウントの場所を追加するための前提条件

新しい CSP 事業拠点を追加するには、いくつかの前提条件があります。

1. ビジネスを遂行する国に、所在地 MPN ID が必要です。

1. CSP にまだ登録されていない[ビジネス リージョン](regional-authorization-overview.md)には、新しい Azure AD テナントが必要です。 CSP に登録するときに、これを作成してください。
 
3. 新しい AAD テナントを使用して、リージョンの CSP プログラムに登録します。
法的企業名、住所、主要連絡先の詳細など、会社の法的な詳細情報を提供します。 このアカウントは検証されるため、必ず有効な情報を追加してください。

>[!NOTE] 
 >必ず、**新しい** Azure AD テナントの **新しい** 資格情報でサインインするようにしてください。 既存の資格情報を使用しないでください。既にアカウントを持っているものとしてパートナー センターに認識されてしまいます。

4. Microsoft Partner Agreement に同意し、アカウントをアクティブ化します。

## <a name="add-an-mpn-location"></a>MPN 所在地を追加する

1. パートナー センターで MPN アカウントを使用してサインインします。 MPN アカウントには、グローバル管理者またはアカウント管理者特権が必要です。 

1. **設定アイコン** から **[組織の設定]** を選択します。

2. **[Legal]\(法務\)** を選択し、 **[場所]** を選択します。

3. **[Add a location]\(場所の追加\)** を選択し、会社に追加する場所の住所の詳細と、その場所の主要な連絡先を挿入します。

> [!NOTE]
> パートナー センターで追加した場所は削除できません。 正しい MPN ID を使用してサインインすると、パートナー センターの左側のメニューに **MPN** が表示されます。

## <a name="change-global-partner-account-location"></a>グローバル パートナー アカウントの場所を変更する

1. **[[Business locations]\(事業所\)](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** で場所の一覧を確認して、法人にしようとしている場所が一覧表示されていることを確認します。 ない場合は、追加します。

   :::image type="content" source="images/accountsettings/location1.png" alt-text="現在のすべての場所の一覧が表示されている、パートナー センターのアカウントの場所ページのスクリーンショット。":::

2. **[Legal]\(法務\)** を選択してから、 **[Update legal business profile]\(法的ビジネス プロファイルの更新\)** を選択します。
  
3. 地域と法人を選択し、その **[送信]** を実行します。

  
## <a name="next-steps"></a>次のステップ

- [検証プロセス](verification-responses.md)に関する詳細情報。
