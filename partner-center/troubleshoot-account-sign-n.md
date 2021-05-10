---
title: アカウントまたは MPN の更新パートナー センターの設定に関するトラブルシューティング
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: アプリケーションに登録しようとするときに発生する問題パートナー センター。 回答は、支払い方法やパスワードの忘れなどによる課題に対処します。
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686264"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>アカウントのセットアップまたは MPN の更新に関する問題のトラブルシューティング


**適切なロール**

- グローバル管理者
- MPN パートナー管理者
 
次に示すのは、アカウントのセットアップ時に発生する一般的な問題のトラブルシューティングパートナー センターです。

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>会社の情報フィールドを編集できないPartner Membership Centerから移行するとどうなるか

会社が既に パートナー センター に存在する場合 (CSP アカウントなど)、読み取り専用画面が表示されます。 この画面には、会社に関する情報が表示されます。この画面は、パートナー センター。

この画面で詳細を変更できない。 これは設計上の問題であり、エラーではありません。

[同意 **して続行]** **を選択して** 続行します。


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>IT 部門が [サインアップ] をオフに **したパートナー センター**

このメッセージが表示されるのは、バイラル ユーザーが無効になっているか、またはバイラル サインアップがテナントの Azure ADされます。 次の PowerShell コマンドを実行Azure ADアカウントのグローバル管理者は、必要な機能を有効にできます。

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

詳細については、「セルフサービス サインアップ [」を参照してください](/azure/active-directory/users-groups-roles/directory-self-service-signup)。

## <a name="you-forgot-your-password"></a>パスワードを忘れた

パスワードを忘れた場合は、サインイン ページの [アカウントにアクセスできませんか **?** ] リンクを選択します。 このオプションを使用すると、パスワードをリセットしたり、グローバル管理者に新しい資格情報を割り当て要求したりできます。

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>[会社について教えて] 画面で、"問題が発生しました" というエラーが表示されます

このエラーメッセージは、通常、会社の電話番号で特殊文字、スペース、または国コードを使用している場合に表示されます。 [電話番号] フィールドに入力する値には、最大で10文字まで含めることができます。


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>クレジットカードの購入で、"注文が拒否されました。 情報を確認してください "


法人ではなく、クレジットカードに対応する住所を常に使用してください。 また、郵便番号が正しいことと、使用するアドレスに対応していることを確認してください。

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>オフライン支払いからオンライン支払方法に切り替える場合 

優先支払い方法を使用して、元の注文と再購入を取り消す必要があります。

注文を取り消すには:

1. ダッシュボードの [ **メンバーシップの提供** ] タブを選択します。

2. **取り消し順序** の選択

3. 確認ウィンドウが表示され、最初の順序を取り消すために確認を行う必要があります。

## <a name="next-steps"></a>次の手順

- [パートナー センター アカウントの管理](partner-center-account-setup.md)
- [請求書と偵察を読む方法](read-your-bill.md)
