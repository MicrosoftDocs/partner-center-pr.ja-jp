---
title: 会社のプロファイルを確認する
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 主要連絡先、住所、プログラム情報など、ご自身の会社の詳細情報を確認する方法について説明します。 また、法的住所や請求先住所を更新することもできます。
author: parthpandyaMSFT
ms.author: parthp
ms.topic: how-to
ms.date: 04/12/2021
ms.localizationpriority: medium
ms.custom: contperf-fy21q4
ms.openlocfilehash: 08e35e24dc94c81db56807b4211874996f0f487e
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315875"
---
# <a name="verify-or-update-your-company-profile-information"></a>会社のプロファイルの情報を確認または更新する 

**適切なロール**

- グローバル管理者
- MPN アカウント管理者

グローバル管理者として初めてパートナー センターにサインインするときは、ご自身の会社の詳細情報がすべて正しいことを確認する必要があります。 これには、主要連絡先、会社の正式名称と住所、プログラム情報などがあります。 会社が複数の場所に存在する場合は、場所のデータが正しいことを確認します。 全体管理者、課金管理者、または管理エージェントとして、自分の請求および税金情報を表示し、更新することもできます。

パートナー プロファイルは、法的ビジネス情報、主要連絡先担当者の名前とメール、会社が参加しているプログラム、および法的ビジネスに統合されている他の企業 (該当する場合) で構成されます。 法的ビジネス プロファイルの会社名と住所にスペルミスや省略形がなく、正式な会社のビジネス登録レコードと正確に一致していることを確認します。 個人事業として業務を行っている場合は、会社名を正式名称として使用する必要があります。


## <a name="locate-the-legal-business-profile"></a>法的ビジネス プロファイルを見つける

1. **[設定]** アイコンに移動し、 **[アカウントの設定]** を選択します。
 
1. **[組織のプロファイル]** を選択します。 

2. ご自身の **法的ビジネス プロファイル**、 **主要連絡先情報**、および **プログラム情報** を確認します。

他の企業を法人に統合している場合は、その情報を確認することもできます。 

## <a name="update-your-legal-business-profile"></a>法的ビジネス プロファイルを更新する 

パートナー センターで会社の正式名称または住所を更新します。

>[!Important]
>- MPN アカウントの場合は、グローバル管理者とアカウント管理者の両方が、会社の正式名称を更新できます。
>- CSP 間接リセラー アカウントの場合は、グローバル管理者のみが会社の正式名称を更新できます。 
>- 直接請求パートナーと間接プロバイダーは、アカウントの検証の状態が **[承認済み]** の場合、会社の正式名称を変更することはできません。 名前を変更する必要がある場合は、[サポート チケットを作成する](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=eb74583c-61b3-2124-bffc-00920e0ae772)必要があります。



1. **[設定]** 、 **[アカウント設定]** の順に移動し、 **[組織のプロファイル]** を選択します。

2. **[法的情報]** を選択してから、更新する法人プロファイル (パートナーまたはリセラー) を選択します。

1. 会社の名前または住所の横にある **[更新]** をクリックして、詳細を変更します。
 
1. **[送信]** を選択すると、法的 ID が再評価されます。 変更されたもののみが再評価されます。

1. 検証が失敗する場合は、[問題を解決する](verification-responses.md)方法を参照してください。

>[!Important]
>クラウド ソリューション プロバイダー (CSP) パートナーは、法的住所に関連付けられている国を変更できません。 法的住所の国は、お使いのテナントとサービス、およびビジネスで使用している通貨に関連付けられています。 MPN の国の更新については、[MPN の国の更新](manage-locations.md#change-country-of-partner-global-account)に関する記事を参照してください。


### <a name="who-can-update-legal-business-name-and-when"></a>企業の正式名称を更新できるユーザーとタイミング

|**Program**|**会社名を更新できるユーザー**|**更新できるタイミング (状態)**|**許可されます。**|
|---------------------|:-------------------------------|:------------|:-----------------|
MPN|グローバル管理者、アカウント管理者|承認済み、保留中、拒否済み| 許可されます。|
|CSP: 間接リセラー|グローバル管理者|承認済み、保留中、拒否済み| 許可されます。|


## <a name="update-your-mpn-global-business-account"></a>MPN グローバル ビジネス アカウントを更新する

Partner Membership Center からパートナー センターへの移行中、誤ったビジネス アカウントが法人として特定された場合は、正しい法人アカウントに変更できます。

これらの更新を行うには、グローバル管理者かアカウント管理者である必要があります。詳しくは、[MPN のグローバルな場所アカウントを管理](manage-locations.md)する方法に関する記事をご覧ください。


## <a name="update-your-mpn-id-associated-with-your-csp-account"></a>CSP アカウントに関連付けられている MPN ID を更新する

ご使用の CSP アカウントに関連付けられている MPN ID を更新するには、次のようにします。

1. CSP アカウントの資格情報を使用して、グローバル管理者としてパートナー センターの [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインし、 **[設定]** を選択します。 (MPN と CSP の資格情報は異なる場合があります。)
 
1. **[アカウント設定]** から **[識別子]** を選択します。

1. **[CSP]** セクションの **[更新]** リンクを使用して、CSP アカウントに関連付けられている MPN ID を更新します 


## <a name="update-your-csp-legal-billing-address"></a>CSP の法的請求先住所を更新する

グローバル管理者、課金管理者、または管理エージェントの場合は、請求書に表示される住所を **[Payout and tax profile]\(支払いと税金プロファイル\)** で変更できます。 ただし、請求書システムの制限により、請求書の会社名を変更することはできません。

:::image type="content" source="images/billing-profile.png" alt-text="請求情報が追加された画面のキャプチャ":::

|**フィールド**  |**説明**|  
|---------------------|:------------------|
|請求先の会社名|CSP 請求書の請求先情報に表示される会社名。  これは、パートナー センターでは編集できません。  更新するには、サポート チケットを作成してください。|
|請求先住所|CSP 請求書に表示される請求先住所。 [課金プロファイル](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial)から更新できます。|
|請求先担当者|CSP アカウントの請求先担当者の詳細 (姓、名、第一連絡先の番号)。  [課金プロファイル](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial)から更新できます。|
|発注番号|パートナーの請求書に表示される注文書番号。  [課金プロファイル](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial)から更新できます。|
|会社の税 ID|一部の国では、企業が[付加価値税 (VAT) 番号またはその国でそれに相当するもの](https://docs.microsoft.com/partner-center/organization-tax-info#submit-vat-id-number)を入力できます。 税金/VAT ID を更新するには、全体管理者、課金管理者、または管理エージェントである必要があります。|
|請求通貨|CSP アカウントの請求通貨は、CSP アカウントの法律上の国によって決まります。  これは、CSP アカウントを作成した後に変更することはできません。|


## <a name="next-steps"></a>次の手順

- [確認の状態を調べる](verification-responses.md)

- [MPN の場所を管理する](manage-locations.md)
