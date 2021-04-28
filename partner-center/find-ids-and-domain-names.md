---
title: テナント ID、ドメイン名、ユーザーオブジェクト ID を検索します
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 組織の Azure AD のテナント ID、ドメイン名、または特定のユーザーオブジェクト ID を Azure portal の Id を検索する方法について説明します。 この情報が必要なタスクもあります。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 17b0100bf5e45e931a765a73fb98afddf6dba656
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172253"
---
# <a name="locate-important-ids-for-a-user"></a>ユーザーの重要な Id を検索する

**適切なロール**

- グローバル管理者

この記事では、 [Azure portal](https://portal.azure.com/) を使用して、ユーザーに関する次の情報を検索する方法について説明します。

- ユーザーの組織または会社の Microsoft Azure Active Directory (Azure AD) テナント ID

- Azure AD テナントに関連付けられている組織または会社のプライマリドメイン名

- ユーザーオブジェクト ID

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Microsoft Azure AD テナント ID とプライマリドメイン名を検索する

Azure portal 内で Azure AD テナント ID またはプライマリドメイン名を見つけるには、次の手順に従います。 (テナント ID をプログラムで検索する場合は、「 [PowerShell または CLI でテナント id を検索](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)する」を参照してください)。

> [!NOTE]
> テナント ID は、アプリケーションまたはリソースごとに異なる名前を呼び出すことができます。 たとえば、テナント ID は、ディレクトリ ID、Azure Active Directory (Azure AD) テナント、Microsoft ID、または特定のレポート ( *tenantguid* も含む) と呼ばれる場合があります。

1. [Azure portal](https://portal.azure.com/) にサインインします。

2. メニューから **[Azure Active Directory]** を選択します。

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="メニューから [Azure Active Directory] オプションを選択する Azure portal を示します。":::

3. Azure Active Directory の **概要** ] ページが表示されます。 Azure AD のテナント ID またはプライマリドメイン名を検索するには、[ **テナント id** ] フィールドと [ **プライマリドメイン** ] フィールドを探します。 これらのフィールドは、[テナント情報] セクションに表示されます。

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="2つの強調表示されたフィールド、テナント ID、プライマリドメイン名が表示された概要ページが表示されます。":::

4. テナント ID は、他のいくつかの方法で Azure portal で確認できます。 メニューから **[Azure Active Directory]** を選択します。 次に、メニューの [ **管理** ] セクションを見つけて、[ **プロパティ**] を選択します。

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

