---
title: Partner Membership Center からの移行
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Partner Membership Center からパートナー センターにビジネスを移行する前に、役立つ情報とよく寄せられる質問を確認します。
author: parthpandyamsft
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: be4250864bd07e555b0eb2079c28f3dfb4920805
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999986"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Partner Membership Center (PMC) からパートナー センターへの移行を準備する

**適切なロール**
- グローバル管理者
- ユーザー管理者
- 販売代理店
- 管理エージェント

当社では、メンバーシップの管理を Partner Membership Center (PMC) から、お客様の Microsoft との取引関係を管理するための単一の目的地であるパートナー センターに移行しています。 お客のパートナー センターへの移行をできるだけ効率的かつ簡単にしたいと考えています。 当社はパートナー センターが PMC とは異なるいくつかの領域を識別しており、お客様は移行を行う前にこれを理解し、準備する必要があります。

## <a name="account-and-identity-setup"></a>アカウントと ID のセットアップ

アカウントと ID の設定に関してよく寄せられる質問への回答については、以下を参照してください。

### <a name="what-is-an-azure-active-directory-azure-ad-work-account"></a>Azure Active Directory (Azure AD) 職場アカウントとは何ですか?

Azure 職場アカウントは、Azure パブリック クラウドにおける企業の分離された専用の仮想表現です。Azure、Microsoft Intune、Office 365などの Microsoft クラウド サービスにサブスクライブすると作成されます。

職場アカウントは、Azure AD ユーザーとそのユーザーに関する情報 (電子メール、パスワード、プロファイル データ、アクセス許可など) をホストします。 職場アカウントにはまた、グループ、アプリケーションや、会社とそのセキュリティに関連するその他の情報も含まれています。 

勤務先の電子メールは、Azure Active Directory テナントの一部です。 パートナー センターでアカウントを作成するには、AAD テナントが必要です。 Azure Active Directory の詳細については、[Azure AD でのディレクトリの作成](/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)に関するページを参照してください。

パートナー センターでは、個人の電子メールではなく、勤務先の電子メールを使用してアカウントにサインインします。

- 職場アカウント: john@contoso.com
- 個人アカウント: John@outlook.com

### <a name="what-account-should-you-sign-into-partner-center-with-if-you-have-an-aad-tenant-with-microsoft-for-office-365-for-example-and-you-also-have-a-tenant-for-your-csp-business"></a>Microsoft に AAD テナント (たとえば Office 365 用) があり、さらに CSP ビジネス用のテナントも存在する場合、どのようなアカウントを使用してパートナー センターにサインインする必要がありますか?

CSP アカウントまたは MPN の勤務先の電子メール アカウントのどちらでもパートナー センターにサインインできます。 CSP の勤務先の電子メールを使用してサインインすることを選択した場合、ダッシュボードの左側のナビゲーションには MPN と CSP の両方のプログラム情報が表示されます。 MPN Azure AD テナントの勤務先の電子メールを使用してサインインした場合は、MPN プログラム情報のみが表示されます。 

### <a name="if-you-dont-want-to-use-your-existing-office-365-azure-ad-tenant-for-partner-center-you-can-create-a-new-tenant-prior-to-migrating-from-pmc"></a>パートナー センターのために既存の Office 365 Azure AD テナントを使用したくない場合は、PMC からの移行の前に新しいテナントを作成できます。

パートナー センター アカウントを設定するために既存の Azure AD テナントを使用したくない理由には多くのものがあります。 パートナー センターへの移行を開始する前に、[Azure portal](https://ms.portal.azure.com/#home) に移動して新しい Azure AD テナントを作成します。 [Azure Active Directory での新しいテナントの作成](/azure/active-directory/develop/quickstart-create-new-tenant)に関するページのガイダンスに従ってください。 新しい AAD テナントを使用して、パートナー センターアカウントを設定します。 テナントを作成するには、グローバル管理者である必要があります。 

### <a name="user-roles-including-guest-user-roles-in-partner-center"></a>ロール パートナー センターのゲスト ユーザーを含むユーザー ロール

パートナー センターには、実行する必要がある作業の種類に応じて、さまざまな種類のロールが存在します。 Azure AD ロールであるグローバル管理者などのロールがあります。 一部のロールは、クラウド サービス プロバイダー プログラムまたはインセンティブなどのプログラムに固有であり、MPN に固有のロールもあります。 すべてのパートナー センター ロールの種類を見つけるには、「[ユーザー ロールとアクセス許可の割り当て](permissions-overview.md)」を参照してください。

### <a name="what-happens-to-my-users-roles-when-they-move-from-pmc-to-partner-center"></a>ユーザーが PMC からパートナー センターに移行すると、そのユーザーのロールはどうなりますか?

MPN グローバル管理者、または移行を実行するプライマリ プログラムの連絡先を除き、PMC のすべてのユーザーがその管理者ロールを失います。 移行を完了する個人は、パートナー センターでロールを割り当てる必要があります。 パートナー センターのロールは PMC のロールとは異なります。 パートナー センターのユーザー ロールの詳細については、[ユーザー ロールとアクセス許可の割り当て](permissions-overview.md) および「[PMC からパートナー センターに移動する](move-pmc-pc-map.md#user-roles)」を参照してください。

### <a name="whats-the-difference-between-my-company-profile-and-my-business-profile"></a>会社プロファイルとビジネス プロファイルの違いは何ですか?

会社プロファイルは、住所、場所、主要連絡先、銀行、税金などの詳細が含まれている、会社に関する情報です。

ビジネス プロファイルは会社を顧客に紹介する方法であり、ロゴ、ビジネスの重点に関する詳細、専門知識などを表示するマーケティング ページです。

### <a name="what-does-account-consolidation-mean-for-my-account"></a>アカウントの統合はアカウントに関してどのような意味がありますか?

同じ Azure AD テナントを使用して複数の MPN アカウントをパートナー センターに移行する場合、システムはそれを自動的に認識し、アカウントを統合するようユーザーに依頼します。 これは、同じ Azure AD テナントに複数のドメインが関連付けられている場合でも当てはまります。 

引き続き、個別の AAD テナントを使用してパートナー センターに移行するようにもできますが、それにより、コンピテンシーの評価の分離や余分な購入コストが発生することに注意してください。 アカウントの統合の詳細については、「[会社のアカウントを統合する](consolidate-accounts.md)」をお読みください。

### <a name="if-i-have-multiple-aad-tenants-and-a-single-mpn-account-is-it-possible-to-link-them-in-partner-center"></a>複数の AAD テナントと 1 つの MPN アカウントがある場合、パートナー センターでそれらをリンクできますか?

はい。パートナー センターでは、複数の Azure AD テナントを 1 つのパートナー センター アカウントにリンクできます。
アカウントの統合の詳細については、「[会社のアカウントを統合する](consolidate-accounts.md)」をお読みください。

### <a name="are-there-restrictions-to-adding-multiple-azure-ad-tenants-to-a-single-partner-center-account"></a>複数の Azure AD テナントを 1 つのパートナー センター アカウントに追加する場合の制限はありますか?

Azure AD テナントが既存のパートナー センター アカウントに既に関連付けられている場合は、マルチテナント機能を使用して、それを新しいパートナー センター アカウントに関連付けることはできません。 別の考え方をすると、Azure AD テナントは 1 つのパートナー センター アカウントにしか関連付けられませんが、パートナー センター アカウントには複数のテナントを関連付けることができます。

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Microsoft Partner Network (MPN) メンバーシップの移行 

MPN メンバーシップの移行に関してよく寄せられる質問に対する回答については、以下を参照してください。

### <a name="who-can-perform-the-move-from-pmc-to-partner-center"></a>だれが PMC からパートナー センターへの移行を実行できますか?

会社の MPN グローバル管理者またはプライマリ プログラムの連絡先 (この 2 つのロールは多くの場合、同じユーザーによって保持されます) が移行を開始および実行できます。

### <a name="will-the-person-completing-the-migration-become-the-primary-contact-on-the-company-legal-profile-in-partner-center"></a>移行を完了するユーザーは、パートナー センターでの会社の法的プロファイル上の主要連絡先になりますか?

必ずしもそうではありませんが、主要連絡先は、契約に署名する権限を持つだれかである必要があります。

### <a name="can-microsoft-migrate-my-mpn-membership-for-me"></a>Microsoft は、ユーザーの代わりに MPN メンバーシップを移行できますか?

いいえ。 Microsoft は、ユーザーのメンバーシップ アカウントのパートナー センターへの移行を支援できません。 アカウントを移行するには、職場アカウント (サインイン資格情報) で PMC にサインインして移行プロセスを開始する必要があります。 アカウントを移行する手順を完了したら、メンバーシップの管理を開始し、チームのメンバーが特典にアクセスしたり、メンバーシップを管理したりできるように、ユーザー ロールとアクセス許可をチームに割り当てることができます。 

Microsoft は、現在のコンピテンシー、特典、場所情報、インセンティブのための銀行/税金情報、Partner University へのアクセスを含む MCP の関連付けを自動的に移行します。

### <a name="how-will-the-renewal-policy-change"></a>更新ポリシーはどのように変更されますか?

パートナー センターでは、更新期間は今後 30 日間のユーザーの記念日から取得されます。

### <a name="will-our-competencies-remain-unchanged-after-we-move-to-partner-center"></a>パートナー センターに移行した後もコンピテンシーは変更されないままですか?

はい。コンピテンシーはパートナー センターへの移行の影響を受けません。 不一致に気が付いた場合は、[サポート](https://partner.microsoft.com/support)に問い合わせてください。

### <a name="will-my-benefits-including-cloud-benefits-technical-support-software-benefits-visual-studio-change-after-we-move"></a>移行した後、特典 (クラウドの特典、テクニカル サポート、ソフトウェア特典、Visual Studio を含む) は変更されますか?

対象となる特典は変更されません。 不一致に気が付いた場合は、[サポート](https://partner.microsoft.com/support)に問い合わせてください。

### <a name="will-our-microsoft-accounts-that-have-visual-studio-benefits-allocations-be-honored"></a>Visual Studio の特典が割り当てられた Microsoft アカウントは守られますか?

はい。 MSA に割り当てられた Visual Studio の特典が守られて、保持されます。 それらは、パートナー センターで更新された後も保持されます。 ただし、パートナー センターに移行された後に MSA の割り当てを削除した場合、それをパートナー センターに戻すことはできません。

パートナー センターでは、パートナーは、パートナーが Azure AD テナントの MPN 管理者である同じテナントから、MSA である職場アカウントとゲスト ユーザー アカウントを追加できます。 パートナーが複数の Azure AD テナントのグローバル管理者であり、これらすべてのテナントが同じパートナー センター アカウントに関連付けられている場合、パートナーは、これらすべてのテナントのユーザーを、Visual Studio の特典と Azure の使用量ベースの割り当てに追加することができます。

MPN 管理者または全体管理者は Visual Studio の使用量ベースのサブスクリプションにゲスト ユーザーを割り当てることができますが、ゲスト ユーザーは MSA を使用してパートナー センターにサインインすることはできません。 ただし、ゲスト ユーザーは、Azure と Visual Studio にサインインして、割り当てられた特典を検証および使用できます。

### <a name="how-should-we-manage-our-mcp-associations-and-our-partner-university-access"></a>MCP の関連付けや Partner University へのアクセスを管理するにはどうすればよいですか?

PMC から移行する MCP の関連付けに変更はありません。 ただし、パートナー センターに移行した後の新しい従業員はすべて、パートナー センターで関連付ける必要があります。 既存のユーザーの Partner University のアクセス許可はすべてそのままになりますが、新しい従業員は[トレーニング センター](https://partner.microsoft.com/training)に移動して、Partner University へのアクセスを取得する方法を確認する必要があります。

### <a name="how-do-i-view-mcp-information-once-i-move-to-partner-center"></a>パートナー センターに移行した後に MCP 情報を表示するにはどうすればよいですか?

ダッシュボードの左側のナビゲーションから **[コンピテンシー]** を選択します。 **[コンピテンシー]** ページから、スキル レポートをダウンロードできます。 スキル レポートには、パートナー センターのコンピテンシーやプログラムに関連するスキルを取得しているユーザーが一覧表示されます。 ユーザーがスキルを取得しているが、それらのスキルが対象のコンピテンシーに関連していない場合、そのユーザーはレポートに一覧表示されません。

### <a name="are-customer-references-used-in-partner-center"></a>顧客参照はパートナー センターで使用されていますか?

いいえ。パートナー センターでのコンピテンシー要件を満たすために顧客参照は必要ありません。

### <a name="will-partner-of-record-associations-move-to-partner-center"></a>レコードのパートナーの関連付けはパートナー センターに移行されますか?

はい。レコードのパートナーに変更はありません。 [顧客へのパートナー ID のリンク](/azure/billing/billing-partner-admin-link-started)の詳細を確認してください。

### <a name="is-there-an-impact-to-incentives-because-of-the-move-to-partner-center"></a>パートナー センターへの移行によりインセンティブに影響はありますか?

いいえ。場所を統合せずにアカウントを移行した場合、インセンティブに影響はありません。 PMC に複数のアカウントがあり、パートナー センターに移行するときにグローバル アカウントに統合することにした場合、インセンティブに損失は発生しませんが、インセンティブの支払いが遅延することがあります。 

インセンティブ プログラムに関連するすべての PMC アカウントを移行するわけではない場合、それらのアカウントに関連付けられているインセンティブの獲得を停止できます。

### <a name="what-are-the-incentive-roles-in-partner-center"></a>パートナー センターのインセンティブ ロールとは何ですか?

パートナー センターのインセンティブ ロールは場所に基づいており、インセンティブ管理者とインセンティブ ユーザーを含んでいます。 これらのロールが実行できる操作の詳細については「[ユーザー ロールとアクセス許可の割り当て](permissions-overview.md)」を参照してください。

### <a name="can-incentives-admins-be-assigned-at-the-global-and-location-level"></a>インセンティブ管理者をグローバル レベルと場所レベルで割り当てることはできますか?

はい。 インセンティブ管理者をすべての場所のインセンティブ管理者になるように割り当てることも、各場所に独自のインセンティブ管理者を割り当てることもできます。

### <a name="can-incentives-be-paid-at-the-global-or-location-level"></a>インセンティブをグローバル レベルまたは場所レベルで支払われるようにすることはできますか?

インセンティブは、場所レベルでのみ支払われます。

### <a name="regarding-referrals-how-many-business-profiles-can-we-create"></a>紹介に関連して、いくつのビジネス プロファイルを作成できますか?

会社は、自社の関心を十分に示すため、必要に応じてビジネス プロファイルをいくつでも作成できます。 各ビジネス プロファイルでは、最大 5 つの場所 (国ごとに 1 つの場所) を一覧表示できます。 各ビジネス プロファイルは、その各場所の紹介を受け取ることができます。

### <a name="how-will-referrals-be-assigned-what-changes-can-i-expect-for-example-if-i-have-a-global-company-in-one-market-and-locations-in-other-markets-how-will-referrals-be-assigned"></a>紹介はどのように割り当てられ、どのような変化を期待できますか? たとえば、ある市場に 1 つのグローバルな会社を持ち、その他の市場に複数の拠点がある場合、紹介はどのように割り当てられますか?

紹介は、顧客が定義する検索パラメーターに基づいて割り当てられます。 持っている場所が 1 つか複数かには関係なく、顧客が目的の場所を指定し、そこに他のパラメーターを満たすビジネスがある場合、紹介はその場所に割り当てられます。

### <a name="i-am-migrating-to-partner-center-from-within-russia-i-get-an-error-message-about-web-direct-how-do-i-continue-with-the-migration"></a>ロシア国内から、パートナー センターに移行しようとしています。 Web Direct についてのエラー メッセージが表示されるのですが、 どうすれば移行を続行できますか?

Web Direct プログラムに参加しているためにエラー メッセージが表示される場合、次を行う必要があります。

1. portal.Azure.com にサインインし、新しい Azure AD テナントを作成します。 詳細については、[新しい Azure AD テナントの作成](/azure/active-directory/fundamentals/active-directory-access-create-new-tenant)に関するページを参照してください。

2. 新しい Azure AD テナントを作成したら、それを使用して、Partner Membership Center からパートナー センターに移行するか、パートナー センターでまったく新規に登録します。