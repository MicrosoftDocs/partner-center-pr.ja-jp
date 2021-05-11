---
title: テナント ID、ドメイン名、ユーザー オブジェクト ID を検索する
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 組織の Azure portal テナント ID、ドメイン名、または特定のユーザー オブジェクト ID Azure AD ID を検索する方法について説明します。 一部のタスクでは、この情報が必要です。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 643b1eeb96a47ee4c438f733efe3be22234d02ff
ms.sourcegitcommit: e462f562e7f26b7d6870c22638a2a841499109d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2021
ms.locfileid: "109740286"
---
# <a name="locate-important-ids-for-a-user"></a>ユーザーの重要な ID を見つける

**適切なロール**

- グローバル管理者

この記事では、ユーザーの次の [情報Azure portal](https://portal.azure.com/) を検索する方法について説明します。

- ユーザー Microsoft Azure Active DirectoryまたはAzure ADのテナント ID (テナント ID)

- テナントに関連付けられている組織または会社のプライマリ ドメインAzure AD名

- ユーザー オブジェクト ID

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>テナント ID Microsoft Azure ADドメイン名を見つける

次の手順に従って、Azure AD内のテナント ID またはプライマリ ドメイン名をAzure portal。 (プログラムでテナント ID を検索する場合は、「PowerShell または CLI を使用してテナント ID を検索する [」を参照してください](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell))。

> [!NOTE]
> テナント ID は、異なるアプリケーションまたはリソースで異なる名前と呼ばれる場合があります。 たとえば、テナント ID は、ディレクトリ ID、Azure Active Directory (Azure AD) テナント、Microsoft ID、または特定のレポート *(tenantguid*) と呼ばれる場合があります。

1. [Azure portal](https://portal.azure.com/) にサインインします。

2. メニューから **[Azure Active Directory]** を選択します。

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="メニュー Azure portalオプションを選択Azure Active Directoryオプションの一覧が表示されます。":::

3. [Azure Active Directory **の概要** ] ページが表示されます。 テナント ID またはAzure ADドメイン名を検索するには、[テナント **ID]** フィールドと [プライマリ ドメイン] **フィールドを探** します。 これらのフィールドは、[テナント情報] セクションに表示されます。

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="テナント ID とプライマリ ドメイン名の 2 つのフィールドが強調表示された [概要] ページが表示されます。":::

4. テナント ID は、他のいくつかの方法Azure portalで確認できます。 メニューから **[Azure Active Directory]** を選択します。 次に、メニューの [ **管理]** セクションを見つけて、[プロパティ] を **選択します**。

   また、[プロパティ] ページには、ユーザーに関連付けられているテナント ID も表示されます。

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="[テナント ID] フィールドが強調表示された [プロパティ] ページを表示します。":::

## <a name="find-the-user-object-id"></a>ユーザーオブジェクト ID を検索する

ドメイン名とテナント ID を検索するだけでは、必ずしも十分であるとは限りません。 また、ユーザーに割り当てられた特定のオブジェクト ID を見つける必要がある場合もあります。 Azure portal でユーザーのオブジェクト ID を検索するには、次の手順に従います。

1. [Azure portal](https://portal.azure.com/) にサインインします。

2. メニューから **[Azure Active Directory]** を選択します。

3. メニューの [ **管理** ] セクションに移動し、[ **ユーザー**] を選択します。

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="[ユーザー] オプションが強調表示されている Azure Active Directory メニューを表示します。":::

4. [ユーザー] ページで、[検索] ボックスにユーザーの名前を入力します。

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="特定のユーザーを検索するための検索ボックスが表示された [ユーザー] ページを表示します。":::

5. 一覧に表示されているユーザーの名前を選択します。  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="検索したユーザーの行を表示するユーザーページを表示します。":::

6. ユーザーのプロファイルページで、[Id] セクションを探します。 [オブジェクト ID] フィールドが、ユーザーの一意のオブジェクト ID と共に表示されます。

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Id セクションとオブジェクト ID の強調表示されたフィールドを含むユーザープロファイルページを表示します。":::

## <a name="next-steps"></a>次のステップ

- [PowerShell または CLI を使用してプログラムでテナント ID を検索する](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [ユーザープロファイルの詳細については、Azure Active Directory を参照してください。](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [パートナーセンターで顧客の詳細を表示またはエクスポートする方法について説明します](see-your-customer-list.md)

