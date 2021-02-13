---
title: PMC からパートナー センターに移行する
ms.topic: article
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Partner Membership Center (PMC) からパートナー センターに会社を移行する方法について、必要な手順を含めて説明します。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: dd566a6d9ef60747eb7fd515b4d63d87d991da2a
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624189"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>PMC からパートナー センターに移行するためのガイド

**適切なロール**

- グローバル管理者

Microsoft パートナーの Web サイト (partner.microsoft.com) は、パートナー向けの統合デジタル エクスペリエンスです。 パートナーの Web サイトで、お客様の営業案件を調査したり、ガイド付きエクスペリエンスに参加したりできます。これらのエクスペリエンスは、会社が Microsoft を使用してアプリとサービスを構築および販売するのに役立ちます。 Microsoft Partner Network のメンバーは、パートナーの Web サイト全体で利用できるダッシュボード リンクを使用して、パートナー センターにサインインできます。ここで、Microsoft との関係を管理したり、プログラムに登録したり、プランにサインアップします。

パートナー メンバーシップ センター (PMC) は使用停止となります。 お客様の会社は、Microsoft Partner Network メンバーシップ管理からパートナー センターに移行するように招待されています。 このガイドでは、PMC からパートナー センターに移行する際に予想されることに対して準備を行います。

>[!NOTE]
>会社に複数のアカウントまたは場所がある場合でも、パートナー センターへの移行は、1 つの (お客様の最初の) アカウントをパートナー センターに移行することから開始されます。

## <a name="get-started"></a>開始

PMC で移行が開始されます。 全体管理者は、移行を開始するための招待を受け取ります。

### <a name="prepare-in-pmc"></a>PMC での準備

- 会社の詳細を確認する
- プライマリ プログラムの連絡先を確認する
- 事業所を確認する
- 承認されたユーザーを更新する

### <a name="when-youre-ready"></a>準備ができたら

招待について **[Get started]\(開始する\)** を選択します。 パートナー センターのサインイン ページが表示されます。

:::image type="content" source="images/migration/getstarted.jpg" alt-text="作業開始":::

## <a name="start-with-your-work-email"></a>勤務先メールの使用を開始する

会社に勤務先メール アドレスと AAD テナントがない場合は、パートナー センターのサインイン プロセス中に設定できます。 個人用アカウントなど、勤務先メール アドレス以外のメール アカウントを使用してサインインしようとすると、AAD テナントと勤務先メール アドレスを設定できるように、会社に関する情報を提供するように指示されます。 これらの会社の詳細は、パートナー センターでアカウントを完成させるために使用されるため、正確に入力してください。

>[!NOTE]
>中国内のパートナーであり、Microsoft Partner Network とクラウド ソリューション プロバイダー (CSP) プログラムの両方に登録されている場合は、アカウントごとに個別のテナントが作成されます。 クラウド ソリューション プロバイダー プログラムのアカウントは国内クラウドで管理され、Microsoft Partner Network アカウントはグローバル クラウドで管理されます。 これらの 2 つのアカウントをリンクすることはできません。

:::image type="content" source="images/migration/newtellusabout.png" alt-text="あなたの会社について教えてください":::

情報を確認または更新したら、 **[同意して続行する]** を選択します。
このページの使用条件は、PMC で会社が既にサインインしている契約と **まったく同じ** です。  
この手順により、Azure AD テナントの作成が開始され、職場アカウントが提供されます。

**[同意して続行する]** を選択すると、次の処理も実行されます。

- ご利用のアカウントをそのすべての場所と共にパートナー センターに移行する

- PMC で購入した可能性のあるコンピテンシーまたは MAP を移行する

- PMC に所有していたマーケティング リソース、オファー、プログラム (MAP、Silver、Gold) を移行する

## <a name="invite-employees-to-join-you"></a>参加するように従業員を招待する

新しい Azure AD テナントが作成されたら、パートナー センターにサインインするように従業員を招待できます。

:::image type="content" source="images/migration/invite.png" alt-text="従業員を招待する":::

既存の AAD テナントを使用してサインインした場合は、従業員も一緒に移動されます。 この場合は、パートナー センターで何ができるかを決定するために従業員のロールを割り当てます。 

>[!NOTE] 
>パートナー センターのロールは、PMC のロールとは異なります。 詳細については、「[Moving from PMC to Partner Center](move-pmc-pc-map.md)」(PMC から Partner Center への移行) を参照してください。

## <a name="verify-your-domain-and-become-a-global-admin"></a>ドメインを確認し、全体管理者になる  

AAD テナントが新しい場合は、全体管理者のロールが誰にも割り当てられていません。全体管理者になるには、ドメインの所有権を確認する必要があります。 そのためには、ドメイン管理者によるサポートが必要になることがあります。

購入済みのプランを使用することはできますが、全体管理者を割り当てるための手順を完了するまでは、新しいプランを購入することができません。

:::image type="content" source="images/migration/takecontrol.png" alt-text="管理する":::

[Get started]\(開始する\) を選択すると、次の画面が表示されます。

:::image type="content" source="images/migration/verifytxt.png" alt-text="ドメインの所有者を確認する":::

ドメイン レジストラーは既に自動入力されています。 ドメイン所有者だけが DNS ファイルを更新できます。そのため、テキスト ファイルをコピーして DNS レコードに追加することで、自分が所有者であることを確認できます。 更新が行われるまで数分かかります。 パートナー センターからサインアウトしてから、もう一度サインインする必要があります。 ロールが全体管理者に変更されています。

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>ダッシュボードとパートナー センターについて理解する

ダッシュボードのツアーを開始します。 ここでは、**ダッシュボード** を選択することでいつでも、メンバーシップの管理、紹介用のビジネス プロファイルの追加、クラウド ソリューション プロバイダー プログラムへの登録、ビジネスに関連する通知とプランの確認を行うことができます。 また、インセンティブの管理、マーケットプレースでの購入、市場投入サービスへのサインアップなども行うことができます。  

:::image type="content" source="images/migration/fre.png" alt-text="ツアーを開始する":::

## <a name="sign-the-microsoft-partner-agreement"></a>Microsoft Partner Agreement に署名する

間接リセラーの場合は、パートナー センター アカウントを設定した後、クラウド ソリューション プロバイダー プログラムに正式に登録する必要があります。 メンバーシップの状態を調べるには、[法的プロファイル](https://partner.microsoft.com/pcv/accountsettings/partnerprofile)にアクセスしてアカウントの種類を確認してください。 その後、[間接リセラー](enrolling-in-the-csp-program.md)として CSP に登録します。

 間接リセラーとして登録したら、[間接プロバイダーとの CSP 関係の要求](indirect-reseller-tasks-in-partner-center.md)に同意します。

次に、グローバル管理者の資格情報を使用して、パートナー センターの[ダッシュボード](https://partner.microsoft.com/pvc/dashboard)の概要で Microsoft Partner Agreement に同意してください。 パートナー プロファイルの [プログラム情報] セクションで、Microsoft Partner Agreement に署名したことを確認します。 また、[CSP の概要] ページに確認バナー通知が表示されます。 

## <a name="next-steps"></a>次のステップ

- [グローバル管理者を見つける](become-global-admin.md)

- [Microsoft Partner Agreement](microsoft-partner-agreement.md)

- [ユーザー アカウントの作成](create-user-accounts-and-set-permissions.md)

- [ユーザー ロールとアクセス許可を割り当てる](permissions-overview.md)

- [メンバーシップ プログラムを管理する](renew-mpn-offers.md)

- [会社のビジネス プロファイルを作成する](create-a-marketing-profile.md)

- [紹介機能で顧客との関係を構築する](manage-leads.md)

- [複数の会社を PMC からパートナー センターに移行するためのガイド](move-multiple-companies.md)
