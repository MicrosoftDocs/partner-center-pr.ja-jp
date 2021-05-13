---
title: サインインしてサインインできないパートナー センター
ms.topic: troubleshooting
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 考えられる原因をトラブルシューティングし、パートナー センター にサインインできない場合の解決策について学習します。パスワードのリセット、ロールの確認、資格情報の確認の詳細を確認してください。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f4af8c48e2bbe65f58549b542447c80b699332be
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818798"
---
# <a name="troubleshoot-sign-in-issues-for-partner-center"></a>サインインに関する問題のトラブルシューティングを行パートナー センター

**適切なロール**: このロールに関心を持つパートナー センター

この記事には、サインインに関する一般的なサインインに関する問題の解決策パートナー センター。

## <a name="youve-forgotten-your-password-for-partner-center"></a>パスワードを忘れた場合パートナー センター

パスワードを忘れてサインインできない場合は、サポートパートナー センター問い合わせください。 適切な連絡先については、「 [ビジネス製品のサポート」を参照してください](/microsoft-365/admin/contact-support-for-business-products)。

MPN パートナーの場合は、グローバル管理者に新しいパスワードの作成を求める。 CSP 間接リセラーの場合は、間接プロバイダーに、Azure AD テナントで新しいグローバル管理者を作成するか、委任された管理者特権を使用して新しいパスワードを作成してください。

パスワードをリセットし、仕事用アカウントへのアクセスを回復する方法の詳細については、「セキュリティ情報を使用して仕事または学校のパスワードをリセット [する」を参照してください](/azure/active-directory/user-help/active-directory-passwords-update-your-own-password#how-to-change-your-password)。

## <a name="you-cant-view-or-manage-the-expected-pages-or-capabilities-in-partner-center"></a>必要なページまたは機能を表示または管理パートナー センター

ロール内のページパートナー センター、割り当てられているロールによって制御されます。 割り当てられているロールを確認するには、[設定] アイコンを選択パートナー センターアカウント設定]を選択し、[アカウント設定] で [ユーザー管理] を **選択します**。 [検索] に名前を入力し、結果を表示します。

コンピテンシー、顧客、インセンティブ、またはユーザーを表示または管理できない場合は、次のソリューションを試してください。

- MPN、CSP、紹介の機能にアクセスするには、グローバル管理者またはアカウント管理者にお問い合わせください。ロールと、ロールで有効にするタスクの詳細については、「パートナー センターにロールを割り当てる」& [を参照してください](permissions-overview.md)。
- 商用マーケットプレースと Windows & Xbox、Office ストア、Microsoft Edge、およびハードウェア開発者プログラムの機能にアクセスするには、組織内の所有者または管理者の役割の担当者にお問い合わせください。 ロールとアクセス許可の詳細については、「 [Microsoft パートナーセンターで商用 marketplace アカウントを管理する方法](/azure/marketplace/partner-center-portal/manage-account#define-user-roles-and-permissions)」を参照してください。

## <a name="you-cant-see-your-offer-or-benefits-in-partner-center"></a>パートナーセンターでプランや特典が表示されることはありません

サインインするための正しい資格情報を使用していることを確認します。 たとえば、職場と個人のアカウントは同じように見える場合がありますが (など)、作成した個人アカウントを使用することができ abc@contoso.com ます。また、ユーザーに代わってビジネスアカウントを設定することもできます。 この場合、サインインしていても、MPN、CSP、商用 Marketplace に関連する予想される機能を表示できない場合は、職場アカウントを選択してみてください。

## <a name="next-steps"></a>次の手順

- [アカウント情報を確認する](verification-responses.md)
- [パスワードのリセット](reset-my-pasword.md)
- [ユーザー パスワードのリセット](reset-a-user-password.md)