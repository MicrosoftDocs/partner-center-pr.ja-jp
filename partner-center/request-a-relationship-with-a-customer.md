---
title: 顧客との再販業者関係の要求
ms.topic: how-to
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: マルチパートナーのマルチチャネル シナリオ、または顧客の委任された管理者特権を復元する必要がある場合は、顧客との関係を要求します。
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.openlocfilehash: f8265973157540cff698790ddb2effa912abeeb7
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856119"
---
# <a name="how-to-request-a-reseller-relationship-from-a-customer-in-partner-center"></a>パートナー センターでお客様から再販業者の関係を要請する方法

**適切なロール**: 管理エージェント |グローバル管理者

顧客の代わりに顧客のサービスまたはサブスクリプションを管理する場合、顧客は、そのサービスまたはサブスクリプションに対する管理者アクセス許可を付与し、Microsoft 顧客契約 に署名する必要があります。

顧客とのリセラー関係を確立し、プロビジョニングした Azure サブスクリプションのみを管理する場合は、管理者のアクセス許可を取得する必要があります。

>[!NOTE] 
>アクセス許可を要求しないオプションは、Microsoft Cloud for US Governmentまたは Microsoft Cloud Germany で運用されているパートナーは使用できません。 詳しくは、「[顧客がパートナーに管理特権を委任する](customers-revoke-admin-privileges.md)」をご覧ください。

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>貴社との再販業者関係を確立するために顧客を招待する

顧客とのリセラー関係は、お客様の国内または同じリージョンから要求できます。

1. **パートナー センター** メニューから **[顧客]** を選択し、 **[リセラーの関係を要求する]** を選びます。

2. この顧客に管理者のアクセス許可を要求するには、[管理者と Office **365** の委任された管理特権Azure Active Directory含める] を選択します。 管理者権限を要求せずにリレーションシップを確立するには、このオプションをオフにします。

3. 次のページで、下書きの電子メール メッセージを確認します。 既定の電子メール アプリケーションで下書きメッセージを開くことも、メッセージをクリップボードにコピーして電子メールに貼り付けることもできます。

   メールのテキストを編集することはできますが、リンクを必ず含めてください。このリンクは、顧客が貴社のアカウントに直接アクセスできるようにカスタマイズされています。 この手順を完了したら、 **[完了]** を選びます。

4. 顧客にメールを送信します。

5. 顧客が招待を受け入れた後、顧客ページに表示され、そこから顧客のサービスをプロビジョニングおよび管理できます。

   > [!NOTE]
   > 顧客が顧客の承認をまだ受けMicrosoft 顧客契約、招待を受け入れるときに、その要求を受け取るメッセージが表示されます。 招待を受け入れるには、顧客がグローバル管理者である必要があります。

6. 顧客のアカウント、サービス、ユーザー、ライセンスを管理するには、顧客の名前の下矢印を選んで、顧客のレコードを展開します。

> [!IMPORTANT]  
> 顧客は、サービスの管理者ポータルで、管理者のアクセス許可の割り当てを変更したり、削除したりすることができます。 ただし、お客様と契約を再交渉しない限り、お客様は、顧客が管理者のアクセス許可を再割り当てまたは削除した後も、引き続きカスタマー サポートを提供し、Microsoft Partner Agreement の条項に従う責任を負います。 この状況で顧客にサポートが必要となった場合、パートナーは顧客に代わって Microsoft サポートにサービス要求を求めることができます。

## <a name="changes-to-the-customer-invitation-experience"></a>顧客招待エクスペリエンスの変更

パートナーからのリセラー関係の招待を受け入クラウド ソリューション プロバイダーカスタマー エクスペリエンスは、さまざまな顧客向けポータルによってホストされます。 ポータルの場所は、顧客が Microsoft パブリック クラウドか国内クラウドかによって異なります。

|クラウドのお客様の種類  | 顧客がリセラー関係の招待を受け入れる場所 |
|---------|---------
| パブリック クラウド内の顧客 | Microsoft 365 管理センター |
| Microsoft Cloud Germany のパートナー センター内の顧客 | Microsoft Office 管理ポータル |
| Microsoft Cloud for US Government のパートナー センター内の顧客 | Microsoft Office 管理ポータル |
|

## <a name="next-steps"></a>次の手順

- [サポート連絡先の指定](assign-support-contacts.md)

- [顧客との再販業者関係の削除](remove-a-relationship.md)
