---
title: Microsoft 顧客契約へのお客様の同意を確認する | パートナー センター
ms.topic: article
ms.date: 09/30/2019
Description: パートナーは、お客様のために Microsoft 製品とサービスを注文する前に、Microsoft 顧客契約へのお客様の同意を得る必要があります。 パートナーがコンプライアンス要件を満たすことができるように、Microsoft では、パートナーに対して、契約に同意したユーザーに関する特定の詳細情報を提供することにより、同意を確認することを求めています。
author: LauraBrenner
ms.author: labrenne
keywords: 顧客, お客様, 同意, MCA, Microsoft Cloud 契約, Microsoft 顧客契約, 顧客契約テンプレート
ms.localizationpriority: medium
ms.openlocfilehash: 5247ab8ced05edbb05d2ed690f2375541d2b43aa
ms.sourcegitcommit: 4b8cad9f24229767dd44fa9418fe57e10d74f390
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/01/2019
ms.locfileid: "71704175"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Microsoft カスタマー契約に同意するかどうかを確認する

現在、CSP パートナーがお客様の代わりに注文する前に、お客様は該当する **Microsoft Cloud 契約**に同意して署名する必要があります。 その後、パートナーは、署名者に関する情報を Microsoft に提供することで、お客様にその同意を確認する必要があります。 確認が行われていない場合:
- このお客様について新しい注文を作成することはできません。
- このお客様について既存のシート ベースのサブスクリプションのシート数を変更することはできません。

パートナー センター ダッシュボードまたは API を使用して、Microsoft Cloud 契約へのお客様の同意を確認する方法の詳細については、「[Microsoft Cloud 契約へのお客様の同意を確認する](confirm-consent.md)」を参照してください。

2019 年 10 月 1 日に、Microsoft では、CPS プログラムに **Microsoft 顧客契約**を導入する予定です。これは、Microsoft Cloud 契約に置き換わります。 新しい契約へのパートナーの移行を促進するために、現在の Microsoft Cloud 契約は、2020 年 1 月 31 まで CSP プログラムでサポートされます。 スケジュールの詳細については、次の表を参照してください。

| 日付 | マイルストーン | 詳細 |
|------------|------------|--------------------------------|
|2019 年 8 月 1 日|サンドボックスで UX プレビューの提供開始|パートナーは、CSP サンドボックス環境でパートナー センター ダッシュボードを使用して、Microsoft 顧客契約へのお客様の同意を確認できます。 CSP サンドボックス環境へのアクセス権を持つパートナーは、ユーザー エクスペリエンスの変更をプレビューできます。 サンドボックス環境へのアクセス権を持たないパートナーは、その変更をこのトピックで確認できます。|
|2019 年 9 月 3 日|サンドボックスで API プレビューの提供開始。|パートナーは、CSP サンドボックス環境でパートナー センター API を使用して、Microsoft 顧客契約へのお客様の同意を確認できます。 API パートナーは、この機会を利用して API の変更をプレビューし、新しい契約をサポートするために API の統合作業を開始できます。|
|2019年9月20日|サンドボックスで .NET SDK プレビューの提供開始。|パートナーは、CSP サンドボックス環境内でパートナー センター .NET SDK を使用して、Microsoft 顧客契約へのお客様の同意を確認できます。 API パートナーは、この機会を利用して .NET SDK の変更のプレビューを表示し、新しい契約をサポートするために API の統合作業を開始できます。|
|2019 年 10 月 1 日|Microsoft 顧客契約が運用環境で使用可能|Microsoft では、Microsoft 顧客契約を CSP プログラムに導入します。これは、Microsoft Cloud 契約に置き換わるものです。 パートナーは、運用環境でパートナー センター ダッシュボードと API を使用して、Microsoft 顧客契約へのお客様の同意を確認できます。 Microsoft Cloud 契約は、CSP パートナー プログラムで引き続きサポートされます。 ただし、パートナーは、Microsoft 顧客契約への移行を開始することをお勧めします。 新しい購入および既存のサブスクリプションに対するシート数の変更では、Microsoft 顧客契約または Microsoft Cloud 契約のいずれかへのパートナーの確認が必要になります。 特定の新しいオファー (新しい Azure プランなど) では、Microsoft 顧客契約への同意の確認が求められます。|
|2020 年 1 月 31 日|Microsoft クラウド契約が運用環境から削除|Microsoft Cloud 契約は CSP パートナー プログラムでは受け入れられなくなりました。 新しい購入および既存のサブスクリプションに対するシート数の変更では、パートナーは、Microsoft 顧客契約の確認を提供する必要があります。 この要件は、以前に Microsoft Cloud 契約に同意した場合でも、新しいお客様および既存のお客様に適用されます。|

## <a name="access-microsoft-customer-agreement-template"></a>Microsoft カスタマーアグリーメントテンプレートにアクセスする
パートナーは、Microsoft カスタマーアグリーメントテンプレートの最新バージョンを[ここ](https://aka.ms/customeragreement)から手動でダウンロードできます。 Microsoft カスタマーアグリーメントは国固有であることに注意してください。 Microsoft カスタマーアグリーメントテンプレートを要求するときは、お客様の所在地に応じて正しい国を選択してください。 

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>パートナーセンター API/SDK を使用して顧客の同意を確認する
パートナーは、パートナーセンター API/SDK を使用して、お客様が Microsoft カスタマーアグリーメントに同意したかどうかを確認できます。 API/SDK の詳細については、以下を参照してください。

- [Microsoft 顧客契約の契約メタデータを取得する](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [Microsoft 顧客契約へのお客様の同意を確認する](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Microsoft 顧客契約に関するお客様の同意の確認を取得する ](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [Microsoft 顧客契約テンプレートのダウンロード リンクを取得する](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)


## <a name="confirm-customer-acceptance-in-partner-center"></a>パートナー センターを使用してお客様の同意を確認する
パートナーは、新しい顧客と既存の顧客に対して、パートナーセンターで Microsoft カスタマー契約に同意したかどうかを確認できます。

### <a name="confirm-customer-acceptance-for-new-customers"></a>新しいお客様について、お客様の同意を確認する

パートナー センターで新しい顧客テナントを作成するときに、次の手順を使用して、Microsoft 顧客契約へのお客様の同意を確認します。 この手順を実行するには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** を選択し、 **[新しい顧客]** を選択します。

2. **[アカウント情報]** で、会社と主要連絡先の情報を入力します。

3. **[Microsoft agreement]\(Microsoft 契約\)** で、 **[Microsoft 顧客契約]** を選択します。

4. **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。

5. 表示されたユーザーの主要連絡先情報が正しいことを確認します。 正しくない場合は、 **[更新]** を選択し、契約に同意したユーザーの **名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。

6. **[次へ]** を選択して、お客様のテナントを作成する残りの手順を続行します。

![新しい顧客](images/mcua1.png)

### <a name="confirm-customer-acceptance-for-existing-customers"></a>既存のお客様について、お客様の同意を確認する

これを行うには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** を選択します。 顧客を検索して選択します。

2. **[アカウント情報]** を選択します。

3. **[Microsoft 顧客契約]** で **[更新]** を選択します。

4. 契約に同意したユーザーの**名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。 **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。

5. **[保存]** を選択して続行します。

![既存の顧客](images/mcua2.png)

### <a name="retrieve-confirmation-of-customer-acceptance"></a>お客様の同意の確認を取得する

次の手順に従って、既存のお客様が Microsoft 顧客契約に同意したことを示す確認を取得できます。 これを行うには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** を選択し、表示するお客様を検索して選択します。

2. **[アカウント情報]** を選択します。

3. **Microsoft 顧客契約** で、この顧客による確認の提供の有無を表示します。
