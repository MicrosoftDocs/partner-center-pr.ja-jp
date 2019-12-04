---
title: PMC からパートナー センターに移行するためのガイド | パートナー センター
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Partner Membership Center (PMC) からパートナー センターに会社を移行する方法について説明します。
author: LauraBrenner
ms.author: labrenne
keywords: PMC, 移行, パートナー センターへの移行
ms.localizationpriority: high
ms.openlocfilehash: c656981bfd5eb99e34a24f70960d4bc7da581896
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721874"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>PMC からパートナー センターに移行するためのガイド

**適切なロール**

- 全体管理者

Microsoft パートナーの Web サイト (partner.microsoft.com) は、パートナー向けの統合デジタル エクスペリエンスです。 パートナーの Web サイトで、お客様の営業案件を調査したり、ガイド付きエクスペリエンスに参加したりできます。これらのエクスペリエンスは、会社が Microsoft を使用してアプリとサービスを構築および販売するのに役立ちます。 Microsoft Partner Network のメンバーは、パートナーの Web サイト全体で利用できるダッシュボード リンクを使用して、パートナー センターにサインインできます。ここで、Microsoft との関係を管理したり、プログラムに登録したり、プランにサインアップします。 

パートナー メンバーシップ センター (PMC) は使用停止となります。 お客様の会社は、Microsoft Partner Network メンバーシップ管理からパートナー センターに移行するように招待されています。 このガイドでは、PMC からパートナー センターに移行する際に予想されることに対して準備を行います。

>[!Note]
>会社に複数のアカウントまたは場所がある場合でも、パートナー センターへの移行は、1 つの (お客様の最初の) アカウントをパートナー センターに移行することから開始されます。

## <a name="get-started"></a>はじめに

PMC で移行が開始されます。 全体管理者は、移行を開始するための招待を受け取ります。 

**PMC での準備**
- 会社の詳細を確認する 
- プライマリ プログラムの連絡先を確認する 
- 事業所を確認する
- 承認されたユーザーを更新する

**準備ができたら**

招待について **[Get started]\(開始する\)** を選択します。 パートナー センターのサインイン ページが表示されます。

![はじめに](images/migration/getstarted.jpg)

## <a name="start-with-your-work-email"></a>勤務先メールの使用を開始する

会社に勤務先メールと AAD テナントがない場合は、パートナー センターのサインイン プロセス中に設定できます。 個人用アカウントなど、勤務先メール以外のメール アカウントを使用してサインインしようとすると、AAD テナントと勤務先メールを設定できるように、会社に関する情報を提供するように指示されます。
これらの会社の詳細は、パートナー センターでアカウントを完成させるために使用されるため、正確に入力してください。

>[!Note]
>中国内のパートナーであり、Microsoft Partner Network とクラウド ソリューション プロバイダー (CSP) プログラムの両方に登録されている場合は、アカウントごとに個別のテナントが作成されます。 クラウド ソリューション プロバイダー プログラムのアカウントは国内クラウドで管理され、Microsoft Partner Network アカウントはグローバル クラウドで管理されます。 これらの 2 つのアカウントをリンクすることはできません。

![あなたの会社について教えてください](images/migration/newtellusabout.png)

情報を確認または更新したら、 **[同意して続行する]** を選択します。
このページの使用条件は、PMC で会社が既にサインインしている契約と**まったく同じ**です。  
これにより、Azure AD テナントの作成が開始され、職場アカウントを使用できるようになります。

**[同意して続行する]** を選択すると、次の処理も実行されます。

•   アカウントをそのすべての場所と共にパートナー センターに移行する

•   PMC で購入した可能性のあるコンピテンシーまたは MAP を移行する

•   PMC にあるすべての特典 (MAP、シルバー、ゴールド) を移行する

## <a name="invite-employees-to-join-you"></a>参加するように従業員を招待する

新しい Azure AD テナントが作成されたら、パートナー センターにサインインするように従業員を招待できます。

![従業員を招待する](images/migration/invite.png)


既存の AAD テナントを使用してサインインした場合は、従業員も一緒に移動されます。 この場合は、パートナー センターで何ができるかを決定するために従業員のロールを割り当てます。 注:パートナー センターのロールは、PMC のロールとは異なります。 詳細については、「[Moving from PMC to Partner Center](move-pmc-pc-map.md)」(PMC から Partner Center への移行) を参照してください。

## <a name="verify-your-domain-and-become-a-global-admin"></a>ドメインを確認し、全体管理者になる  

AAD テナントが新しい場合は、全体管理者のロールが誰にも割り当てられていません。全体管理者になるには、ドメインの所有権を確認する必要があります。 そのためには、ドメイン管理者によるサポートが必要になることがあります。 購入済みのプランを使用することはできますが、全体管理者になるための手順を完了するまで、新しいプランを購入することはできません。 

![管理する](images/migration/takecontrol.png)

[Get started]\(開始する\) を選択すると、次の画面が表示されます。

![ドメインの所有者を確認する](images/migration/verifytxt.png)

ドメイン レジストラーは既に自動入力されています。 ドメイン所有者だけが DNS ファイルを更新できます。そのため、テキスト ファイルをコピーして DNS レコードに追加することで、自分が所有者であることを確認できます。 更新が行われるまで数分かかります。 パートナー センターからサインアウトしてから、もう一度サインインする必要があります。 ロールが全体管理者に変更されています。 


## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>ダッシュボードとパートナー センターについて理解する

ダッシュボードのツアーを開始します。 ここでは、**ダッシュボード**を選択することでいつでも、メンバーシップの管理、紹介用のビジネス プロファイルの追加、クラウド ソリューション プロバイダー プログラムへの登録、ビジネスに関連する通知とプランの確認を行うことができます。 また、インセンティブの管理、マーケットプレースでの購入、市場投入サービスへのサインアップなども行うことができます。  

![ツアーを開始する](images/migration/fre.png)

## <a name="next-steps"></a>次のステップ

- [ユーザー アカウントを作成する](create-user-accounts-and-set-permissions.md)
- [ユーザー ロールとアクセス許可を割り当てる](permissions-overview.md)
- [メンバーシップ プログラムを管理する](renew-mpn-offers.md)
- [会社のビジネス プロファイルを作成する](create-a-marketing-profile.md)
- [紹介機能で顧客との関係を構築する](responding-to-referrals.md)

## <a name="see-also"></a>関連項目

- [複数の会社を PMC からパートナー センターに移行するためのガイド](move-multiple-companies.md)
