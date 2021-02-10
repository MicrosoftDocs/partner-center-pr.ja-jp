---
title: パートナー アカウントで場所を管理する
ms.topic: how-to
ms.date: 02/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 新しい場所を追加する方法や、所在地 MPN ID がインセンティブ プログラム、CSP ビジネス、サブスクリプション、その他のトランザクションでどのように使用されるかについて説明します。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 41ffaeaf0fb46659142949872295523546bb91c1
ms.sourcegitcommit: 5768f10cd122a20fe3df3062ea34e7096d99f639
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/09/2021
ms.locfileid: "100005909"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>MPN アカウントの所在地を管理し、場所を追加 (削除) する


**適切なロール**

- グローバル管理者
- アカウント管理者

所在地 MPN ID では、貴社の特定の各場所が示されます。 所在地 MPN ID を使用して、インセンティブ プログラムに登録し、クラウド ソリューション プロバイダー (CSP) ビジネスの取引を行い、他のビジネス トランザクションを行います。 グローバル MPN ID は、サポート リクエストなどの非トランザクション アクティビティに使用されます。

## <a name="the-following-is-a-typical-scenario"></a>一般的なシナリオを示します。

Contoso のパートナー グローバル アカウント (PGA) の場所はイギリスです。 これは、登録された法的な事業所であり、そのグローバル MPN ID はすべての非トランザクション ビジネスを管理するために使用されます。 Contoso には、イギリスの別の場所、フランス、米国にある子会社または部門に相当するパートナー ロケーション アカウント (PLA) もあります。 MPN アカウントの構造では、これらの PLA は一意の所在地 MPN ID として表現されます。 PLA は、CSP またはインセンティブ プログラムなどのトランザクション ビジネスに使用されます。 支払いは、特定の場所に関連付けられます。 

>[!NOTE]
>CSP テナントと MPN 所在地 ID の間には 1 対 1 の関係があります。

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 所在地の構造":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>CSP ビジネスの新しいアカウントを追加するための前提条件

新しい CSP ビジネス アカウントを追加するには、まず前提条件を満たしていることを確認します。

1. CSP ビジネスを遂行する国に、所在地 MPN ID が必要です。 新しい MPN 所在地を作成するには、以下の「MPN 所在地を追加する」を参照してください。
  
1. 新しい CSP Indirect Reseller 登録を作成するには、[間接プロバイダーとの連携](indirect-reseller-tasks-in-partner-center.md#get-started)に関する記事を参照してください。 

>[!NOTE] 
 >必ず、**新しい** CSP アカウントの **新しい** 資格情報でサインインするようにしてください。 既存の資格情報を使用しないでください。既にアカウントを持っているものとしてパートナー センターに認識されてしまいます。

2. Microsoft Partner Agreement に同意し、アカウントをアクティブ化します。

1. 直接請求パートナーとして登録する場合は、[直接請求パートナーの要件](direct-partner-new-requirements.md)に関する記事をお読みください。

## <a name="view-your-mpn-locations"></a>MPN 所在地を表示する

1. MPN アカウントの資格情報を使用して、パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。 (MPN の資格情報は、CSP の資格情報とは異なる場合があります) 
 
1. **[設定]** アイコンで、 **[アカウント設定]** 、 **[組織プロファイル]** 、 **[Legal]\(法務\)** を選択します。 

1. **[パートナー]** タブで、PMC から移行した場所の修正を求めるバナー エラー メッセージがないことを確認します。 存在する場合は、指示に従って、それらの場所を修正します。 

3. エラー メッセージがない場合は、 **[設定]** で、 **[アカウント設定]** 、 **[組織プロファイル]** 、 **[識別子]** を選択します。

4. この CSP アカウントの国と一致する "Location" という種類の MPN ID を見つけ、それを使用して以下の検索を行い、関連付けを完了します。

5. 使用する CSP アカウントと一致する場所の MPN ID が見つからない場合は、新しい場所を追加して新しい MPN ID を作成できます。 下の「**MPN 所在地を追加する**」を参照してください。

## <a name="add-an-mpn-location"></a>MPN 所在地を追加する

1. パートナー センターで MPN アカウントを使用してサインインします (MPN の資格情報は、CSP の資格情報とは異なる場合があります)。 MPN アカウントには、グローバル管理者またはアカウント管理者特権が必要です。 

1. **設定アイコン** で、 **[Account settings]\(アカウント設定\)** を選択し、 **[組織プロファイル]** を選択します。

2. **[Legal]\(法務\)** 選択し、 **[パートナー]** タブで **[事業所]** を選択してから、 **[Add a location]\(場所の追加\)** をクリックします。

3. 会社に追加する場所の法人名、住所、連絡先など、必要な詳細情報を入力します。
 
1. **[Add location]\(場所の追加\)** をクリックします。 これにより、CSP 取引とインセンティブに使用できる新しい場所の新しい MPN ID が作成されます。

:::image type="content" source="images/legal-biz.png" alt-text="新しい法的ビジネスの追加":::

> [!NOTE]
> パートナー センターで追加された場所は、削除できません。 正しい MPN ID を使用してサインインすると、パートナー センターの左側のメニューに **MPN** が表示されます。

## <a name="delete-a-location"></a>場所を削除する

アカウントから場所を削除するには、[パートナー サポート](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)に連絡する必要があります。 このアクションによる影響を十分に理解してください。 削除された場所は取得できなくなり、その特定の MPN ID に関連付けられているものはすべて認識されなくなるか、貴社に対して有効でなくなります。

## <a name="change-country-of-partner-global-account"></a>パートナー グローバル アカウントの国を変更する 

1. パートナー センターで MPN アカウントを使用してサインインします (MPN の資格情報は、CSP の資格情報とは異なる場合があります)。 MPN アカウントには、グローバル管理者またはアカウント管理者特権が必要です。 

2. **[パートナー]** タブの **[事業所]** で場所の一覧を確認し、法人にしようとしている場所が一覧表示されていることを確認します。 
 
1. 場所を追加するには、 **[Add a location]\(場所の追加\)** をクリックし、ポップアップに、会社に追加する場所の法人名、住所、第一連絡先担当者など、必要な詳細情報を入力します。 
 
1. **[国/地域]** ドロップダウンの横にある **[Change your country]\(国の変更\)** を選択し、手順に従います。 

:::image type="content" source="images/lbp.png" alt-text="法的ビジネス プロファイル データのポップアップ":::

5. **[保存]** をクリックします。

6. MPN グローバル アカウントの国が、新しい法律上の国に変更されます。
  
## <a name="next-steps"></a>次のステップ

- [検証プロセス](verification-responses.md)に関する詳細情報。
