---
title: 多要素認証を使用してユーザーを設定する
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 従業員に MFA を設定する方法について説明します
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 355258fd20f867052fa8598e688630005262bb16
ms.sourcegitcommit: ab2ca3c5990b7f920df4ecb9c611d5b1046ec111
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/16/2020
ms.locfileid: "97578289"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>多要素認証を使用してユーザーを設定する

**適切なロール**

- グローバル管理者

プライバシーの保護とセキュリティの強化は、マイクロソフトの最優先事項の 1 つです。 最善の防御とは予防することで、私たちの強さが、最も弱いリンクと同程度でしかないことはわかっています。 そのために、エコシステムの全員が行動し、適切なセキュリティ保護を確保する必要があるのです。 すべてのパートナーが、パートナー テナント内のユーザーに対して多要素認証 (MFA) を有効にすることを強くお勧めします。 

## <a name="add-multi-factor-authentication-for-your-users"></a>ユーザーに多要素認証を追加する

このタスクを完了するには、会社のグローバル管理者である必要があります。

ユーザーを Azure AD テナントに追加する時点で MFA を有効にするのが最も簡単です。

1. [Azure portal](https://portal.azure.com) にサインインし、 **[ユーザー管理]** にアクセスします。
1. **[多要素認証]** を選択します。
1. 有効にするユーザーを選択し、 **[有効]** を選択します。

これで、このユーザーに対して MFA が有効になります。 有効にすると、そのユーザーが初めてサインインするときに MFA 検証をセットアップするように求められます。 その後のサインインでは、メールかテキスト メッセージのいずれか設定した方で届いたコードを入力するよう求められます。  

:::image type="content" source="images/MFA/securityverification.png" alt-text="検証する方法を指定する":::

>[!NOTE]
>ユーザーが MFA を使用することを **強制** するには、上記と同じ手順を使用して **[強制]** を選択します。 詳細については、「[ユーザーごとの Azure Multi-Factor Authentication を有効にしてサインイン イベントのセキュリティを確保する](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates)」をご覧ください。 

どのユーザーも最初は  **[無効]** です。 ユーザーごとに Azure Multi-Factor Authentication に登録すると、そのユーザーの状態が  **[有効]** に変わります。 有効にされたユーザーがサインインして登録プロセスを完了すると、その状態は  **[強制]** に変わります。 

## <a name="next-steps"></a>次のステップ

- [ユーザーにロールとアクセス許可を割り当てる](permissions-overview.md)

