---
title: 顧客の代理で問題を報告する
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: カスタマーサービスの問題を Microsoft にエスカレートするタイミング、およびさまざまな種類の Microsoft サービスのサポートチケットをファイルにする方法について説明します。
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 12310b8c89f593122cdd9caec0aa74a712953219
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175085"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>顧客に代わってサービスの問題を報告します。その方法や方法などが含まれます。

**適用対象**

- パートナー センター
- 米国政府機関向け Microsoft Cloud のパートナー センター

**適切なロール**

- 間接プロバイダー

解決できないサービスの問題が発生していて、「 [Microsoft への問題のエスカレーション](escalate-problems-to-microsoft.md)」で説明されている条件を満たしている場合は、間接プロバイダーがサポートチケットを作成できます。 このプロセスは、請求に関する問題や紛争をエスカレートする場合や、不正行為が疑われる場合にも役に立ちます。

## <a name="submit-a-service-request-for-a-customer"></a>顧客のサービス リクエストを提出する

1. **パートナー センター** メニューの **[サービス要求]** を選択し、**[顧客の要求]** を選択します。 

2. [ユーザーの要求] ページで、対象の顧客を検索します。

3. **[新しい要求]** ドロップダウン メニューで、**[Azure]** または **[Office 365、Dynamics 365、Enterprise Mobility Suite]** を選択します。 Microsoft Azure portal または Office 365 管理センターにリダイレクトされます。

>[!NOTE]
>CSP で Dynamics 365 を操作するサポート操作パートナーは、パートナー (ASfP) プラン以降の高度なサポート契約を維持するために必要です。 このサポート契約は、CSP のお客様の代わりに Dynamics 365 インシデントを送信するために必要です。 サポート契約オプションの詳細については、[こちらを参照](https://partner.microsoft.com/support/partnersupport)してください。

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Azure で顧客のためにサービス要求を作成する必要があるときは、次のことに注意してください。
>
>- 間接リセラーとして、Azure で顧客のサービス要求を作成するには、間接プロバイダーが顧客の Azure アカウントへのアクセス権を付与する必要があります。 これは、Office 365 ユーザーに代わって管理を行うこととは異なります。
>
>- パートナー センターのヘルプデスク管理者は、Azure サービス ポータルでサービス要求を作成することはできませんが、Azure サービス ポータルでサポート グループを作成し、サポート要求をログに記録するためのアクセス許可をそのグループに与えることはできます。

1. **[新しいサポート リクエスト]** を選択します。

2. 次のようにサポート要求に適切な情報を入力し、**[作成]** を選びます。

   - サポート要求の **[基本]** セクションで、必ず **[サポート プラン]** フィールドの **[クラウド ソリューション プロバイダー]** を選びます。

   - サポート要求の **[連絡先]** 情報セクションに、顧客の情報ではなく貴社の情報を入力します。

3. 後で Microsoft Azure Portal 内で **[Manage support requests]\(サポート要求の管理\)** を選択して、顧客のサービス要求を確認します。

顧客に対する管理者のアクセス許可がない場合は、顧客に対するサポート要求を作成することが必要になる場合があります。 このようなことは、2 つのシナリオのいずれかで発生する可能性があります。

- 最初にリレーションシップを確立したときに管理者特権を要求していません。
- お客様の Azure サブスクリプションを管理するだけなので、管理者のアクセス許可がありません。
 
いずれの場合も、パートナーは次の手順でサポート要求を作成できます。 

1. パートナーセンターの [アカウント] ページから顧客のドメイン名をコピーします。

2. 移動してhttps://portal.azure.com/[customerdomainname]。 

3. サポートが必要な Azure サブスクリプションを選択します。

4. **[新しいサポート リクエスト]** を選択し、指示に従って要求を作成します。 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365、Microsoft Dynamics CRM Online、Enterprise Mobility Suite

1. [ **サービス要求の作成** ] セクションで、適切なサポートカテゴリを選択します。 その他の記事を表示するには、[ **詳細** ] を選択する必要がある場合があります。

2. サービス リクエスト フォームに記入し、**[送信]** を選びます。

   > [!TIP]
   > 顧客ではなく、必ず貴社の連絡先情報を記入してください。

3. 後で、Office 365 管理センターに移動し、[ **すべてのサポートチケットを表示**] を選択して、顧客のサービスリクエストを確認します。

### <a name="support-for-commercial-marketplace-products"></a>商用マーケットプレース製品のサポート

Microsoft では、市販の marketplace 製品に対する製品サポートは提供していません。 サポートを受けるには、製品を発行した独立系ソフトウェアベンダー (ISV) に問い合わせる必要があります。

ISV の連絡先情報を検索するには:

1.  **[Marketplace]** ページで、ヘルプが必要な製品を選択します。

2.  製品のページにサポート連絡先情報が表示されます。 次のオプションの1つまたは複数を指定できます。

    - ISV の Web サイト上のサポート エントリ ポイントへのリンク
    - サポート電子メール
    - サポート連絡先の電話番号

## <a name="faq"></a>よく寄せられる質問

顧客に代わって送信される可能性があるサービス要求に関してよく寄せられる質問については、以下を参照してください。 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>サポートの権利には何が含まれていますか?

サービスリクエストは、パートナーセンターを通じて提出する必要があります。 これらは、Azure、Microsoft Office 365、Microsoft Dynamics CRM Online、Enterprise Mobility Suite で利用できます。 クラウド ソリューション プロバイダー プログラムに参加しているパートナーの場合は、重大な問題への応答時間において優先されることが期待できます。

独自のパートナーテナントのサポートは、CSP サポート特典の一部として含まれていません。 ただし、Office 365、Microsoft Dynamics CRM Online、Enterprise Mobility Suite では、パートナーまたは顧客に対して個別のサポートサブスクリプション料金が請求されることはありません。 Azure では料金が請求されますが、署名のクラウドサポートやその他の Microsoft Partner Network (MPN) の特典を利用できる場合は、これらを使用して料金を支払うことができます。

この特典は、有料版か試用期間かにかかわらず、クラウド ソリューション プロバイダー プログラムに参加しているすべてのパートナーに適用されます。 課金とサブスクリプションの管理のサポートも、このパッケージの無料コンポーネントとして組み込まれています。

### <a name="how-quickly-will-i-get-an-initial-response"></a>どれぐらい迅速に最初の応答を受けられますか?

最初の応答時間は、提出された問題の重大度によって変わります。 問題の重大度は、サービス要求を提出するときに示されるビジネスへの影響の程度によって決められます。

**技術的な故障対策インシデント**の初回の応答時間:

- 重大な影響 (重大度 A): 2 時間 (サービスの大幅な損失または低下。 実稼働サービスの停止。)
- 中程度の影響 (重大度 B): 4 時間 (中程度の損失またはサービスの低下)。 実稼働サービスは部分的に影響を受けています。)
- 最小限の影響 (重大度 C): 8 時間 (最小限のサービスの損失または低下)。 サービスがまだ使用可能であるか、非運用サービスが影響を受けています。)

最初の応答時間は英語によるサポートのみが対象です。 ローカル言語でのサポートは、業務時間中に提供されます。
サポート権利の境界内にあるが、障害対策インシデントとは見なされないインシデントの場合、初回の応答時間は1営業日までになることがあります。

### <a name="can-i-submit-a-service-request-by-phone"></a>電話でサービス リクエストを提出できますか?

いいえ、このプログラムには電話サポートが提供されていません。

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>Azure ポータルに直接サインインし、パートナー センターをバイパスした場合はどうなりますか?

Microsoft Azure portal に直接サインインする場合は、顧客のコンテキストではなく、独自のコンテキストでセンターを表示しています。 そのため、独自のサブスクリプションのサービス要求を作成する場合にのみ、Microsoft Azure portal に直接サインインする必要があります。

CSP プログラムのサポート資格は、パートナーのサブスクリプションでのサポートを提供していません。 このため、パートナーのサブスクリプションに関するサービス要求を作成するときに、有効なサポートプランの権利を提供する必要があります。 例としては、MPN 契約 ID、プレミア、Azure サポートプランなどがあります。 詳細については、「 [Azure サポート](https://go.microsoft.com/fwlink/?LinkId=717532)に関する FAQ」を参照してください。

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>Office 365 管理センターポータルにサインインし、パートナーセンターをバイパスするとどうなりますか。

Office 365 管理センターに直接サインインすると、顧客のコンテキストではなく、独自のコンテキストでセンターが表示されます。 そのため、自分のサブスクリプションのサービス要求を作成するときに、Office 365 管理センターに直接サインインするだけで済みます。

### <a name="how-do-i-get-additional-dynamics-365-support"></a>追加の Dynamics 365 のサポートを受けるには

Dynamics 365 Plan サブスクリプション、ライセンス、課金、財務 & 操作、Dynamics 365 製品ライセンス、またはその他のテクニカルサポートが必要な場合に関連する問題が発生しています。
 
[Dynamics サポート](/dynamics365/customer-engagement/admin/contact-technical-support)に問い合わせる

「[Microsoft Dynamics のサポート](https://support.microsoft.com/help/4052881/faq-microsoft-dynamics-365-for-unified-operations-iur)」を参照する

## <a name="next-steps"></a>次のステップ

- [顧客へのサポート提供](customer-support.md)
- [サービスの正常性の確認](check-service-health.md)