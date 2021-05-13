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
ms.openlocfilehash: a5e8a292ad8593dc0b94179d5f0ee418344ef9af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854691"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>アカウントのセットアップまたは MPN 更新に関する問題のトラブルシューティング

**適切なロール**: 全体管理者 |MPN パートナー管理者
 
ここでは、パートナーセンターアカウントを設定するときに発生する一般的な問題のトラブルシューティングに関するいくつかの推奨事項を示します。

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>パートナーメンバーシップセンターから移行するときに、会社情報フィールドを編集できない場合はどうなりますか

会社が既にパートナーセンター (CSP アカウントなど) に存在している場合は、読み取り専用画面が表示されます。 この画面には、パートナーセンターに存在する会社に関するすべての情報が表示されます。

この画面の詳細を変更することはできません。 これは仕様であり、エラーではありません。

[ **同意** して **続行** ] を選択して続行します。


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>IT 部門が **パートナーセンターへのサインアップ** を無効にしている場合

このメッセージは、ウイルスに感染したユーザーが無効になっているか、Azure AD テナントでウイルスによるサインアップが無効になっていることが原因で表示されます。 Azure AD アカウントの全体管理者は、次の PowerShell コマンドを実行して、必要な機能を有効にすることができます。

**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

詳細については、「 [セルフサービスサインアップ](/azure/active-directory/users-groups-roles/directory-self-service-signup)」を参照してください。

## <a name="you-forgot-your-password"></a>パスワードを忘れた場合

パスワードを忘れた場合は、サインインページの [ **アカウントにアクセスできない場合]** リンクを選択します。 このオプションを使用すると、パスワードをリセットしたり、グローバル管理者に新しい資格情報の割り当てを依頼したりすることができます。

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>[会社について教えて] 画面で、"問題が発生しました" というエラーが表示されます

このエラー メッセージは通常、会社の電話番号で特殊文字、スペース、または国番号を誤って使用した場合に表示されます。 [電話番号] フィールドに入力する値には、最大 10 文字しか含めることはできません。


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>クレジット カードの購入で、"Your order was declined. (注文が拒否されました。) というエラー メッセージが表示されます。 情報を確認してください"


常に、法人ではなく、クレジット カードに対応する住所を使用してください。 また、郵便番号が正しく、使用するアドレスに対応していることを確認します。

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>オフライン支払いからオンライン支払い方法に切り替える 

元の注文を取り消し、優先支払い方法を使用して再取得する必要があります。

注文を取り消す方法:

1. ダッシュボードの **[メンバーシップ オファー]** タブを選択します。

2. [注文の **取り消し] を選択します**

3. 確認ウィンドウが表示され、最初の注文をキャンセルするには確認する必要があります。

## <a name="next-steps"></a>次の手順

- [パートナー センター アカウントの管理](partner-center-account-setup.md)
- [請求書と調整ファイルを読み取る方法](read-your-bill.md)
