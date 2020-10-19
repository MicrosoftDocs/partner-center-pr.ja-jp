---
title: パートナーセンターのアカウントの設定または MPN の更新に関する問題のトラブルシューティング
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: パートナーセンターに登録しようとしたときに発生する問題のトラブルシューティングを行います。 回答は、支払い方法やパスワードを忘れた場合の課題に対処します。
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d990a2cb4dcb69dfc76e8a4f0d40fd4912b4f8a0
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/19/2020
ms.locfileid: "92174845"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>アカウントのセットアップまたは MPN 更新に関する問題のトラブルシューティング

**適用対象**

- パートナー センター
 
**適切なロール**

- グローバル管理者
- MPN パートナー管理者 
 
ここでは、パートナーセンターアカウントを設定するときに発生する一般的な問題のトラブルシューティングに関するいくつかの推奨事項を示します。

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>パートナーメンバーシップセンターから移行するときに、会社情報フィールドを編集できない場合はどうなりますか

会社が既にパートナーセンター (CSP アカウントなど) に存在している場合は、読み取り専用画面が表示されます。 この画面には、パートナーセンターに存在する会社に関するすべての情報が表示されます。

この画面の詳細を変更することはできません。 これは仕様であり、エラーではありません。

[ **同意** して **続行** ] を選択して続行します。


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>IT 部門が **パートナーセンターへのサインアップ**を無効にしている場合。

このメッセージは、ウイルスに感染したユーザーが無効になっているか、Azure AD テナントでウイルスによるサインアップが無効になっていることが原因で表示されます。 Azure AD アカウントの全体管理者は、次の PowerShell コマンドを実行して、必要な機能を有効にすることができます。

**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

詳細については、「[セルフサービスサインアップ](/azure/active-directory/users-groups-roles/directory-self-service-signup)」を参照してください。

## <a name="you-forgot-your-password"></a>パスワードを忘れた場合

パスワードを忘れた場合は、サインインページの [ **アカウントにアクセスできない場合]** リンクを選択します。 このオプションを使用すると、パスワードをリセットしたり、グローバル管理者に新しい資格情報の割り当てを依頼したりすることができます。

## <a name="on-the-tell-us-about-your-company-scree-you-receive-a-something-went-wrong-error"></a>「お客様の会社について教えてください」というエラーが発生すると、"問題が発生しました" というエラーが表示されます。

このエラーメッセージは、通常、会社の電話番号で特殊文字、スペース、または国コードを使用している場合に表示されます。 [電話番号] フィールドに入力する値には、最大で10文字まで含めることができます。


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>クレジットカードの購入で、"注文が拒否されました。 情報を確認してください "


法人ではなく、クレジットカードに対応する住所を常に使用してください。 また、郵便番号が正しいことと、使用するアドレスに対応していることを確認してください。

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>オフライン支払いからオンライン支払方法に切り替える場合 

優先支払い方法を使用して、元の注文と再購入を取り消す必要があります。

注文を取り消すには:

1. ダッシュボードの [ **メンバーシップの提供** ] タブを選択します。

2. **取り消し順序**の選択

3. 確認ウィンドウが表示され、最初の順序を取り消すために確認を行う必要があります。

## <a name="next-steps"></a>次の手順

- [パートナー センター アカウントの管理](partner-center-account-setup.md)
- [請求書と偵察を読む方法](read-your-bill.md)