---
title: パートナーセンターにサインインできません
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 考えられる原因のトラブルシューティングと、パートナーセンターにサインインできない場合の解決策については、パスワードのリセット、ロールの確認、および資格情報の確認に関するページを参照してください。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 17087727afcaf3dbcf47801f8668388c370758e7
ms.sourcegitcommit: 9b04509f3830462628c1bb6af2ca41ed68b52619
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/09/2021
ms.locfileid: "107266573"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>パートナーセンターのサインインに関する問題のトラブルシューティング

**適切なロール**

- パートナーセンターに関心のあるすべてのパートナー

この記事には、パートナーセンターのサインインに関する一般的な問題の解決策が記載されています。

## <a name="youve-forgotten-your-password-for-partner-center"></a>パートナーセンターのパスワードを忘れた

パスワードを忘れた場合、パートナーセンターにサインインできない場合は、サポートにお問い合わせください。 適切な連絡先については、「 [ビジネス製品のサポート](/microsoft-365/admin/contact-support-for-business-products)」を参照してください。

MPN パートナーの方は、グローバル管理者に新しいパスワードの作成を依頼してください。 CSP 間接リセラーの場合は、Azure AD テナントに新しいグローバル管理者を作成するか、代理管理者権限を使用して新しいパスワードを作成するかを、間接プロバイダーに依頼してください。

パスワードをリセットし、職場アカウントへのアクセス権を回復する方法の詳細については、「 [セキュリティ情報を使用して職場または学校のパスワードをリセット](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)する」を参照してください。

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>パートナーセンターで予想されるページまたは機能を表示または管理できない

パートナーセンターのページへのアクセスは、割り当てられているロールによって制御されます。 割り当てられているロールを確認するには、パートナーセンターで設定アイコンを選択し、[ **アカウント設定**] を選択してから、[アカウント設定] で [ **ユーザー管理**] を選択します。 [検索] に名前を入力し、結果を表示します。

期待されるコンピテンシー、顧客、インセンティブ、ユーザーを表示または管理できない場合は、次の解決策を試してください。

- MPN、CSP、および紹介の機能にアクセスするには、全体管理者またはアカウント管理者に問い合わせてください。ロールと、パートナーセンターで有効になっているタスクの詳細については、「 [ユーザーにロール & アクセス許可を割り当てる](permissions-overview.md)」を参照してください。
- 商用マーケットプレースと Windows & Xbox、Office ストア、Microsoft Edge、およびハードウェア開発者プログラムの機能にアクセスするには、組織内の所有者または管理者の役割の担当者にお問い合わせください。 ロールとアクセス許可の詳細については、「 [Microsoft パートナーセンターで商用 marketplace アカウントを管理する方法](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)」を参照してください。

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>パートナーセンターでプランや特典が表示されることはありません

サインインするための正しい資格情報を使用していることを確認します。 たとえば、職場と個人のアカウントは同じように見える場合がありますが (など)、作成した個人アカウントを使用することができ abc@contoso.com ます。また、ユーザーに代わってビジネスアカウントを設定することもできます。 この場合、サインインしていても、MPN、CSP、商用 Marketplace に関連する予想される機能を表示できない場合は、職場アカウントを選択してみてください。

## <a name="next-steps"></a>次のステップ

- [アカウント情報を確認する](verification-responses.md)
- [パスワードのリセット](reset-my-pasword.md)
- [ユーザー パスワードのリセット](reset-a-user-password.md)