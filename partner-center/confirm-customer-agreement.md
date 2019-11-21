---
title: Microsoft 顧客契約へのお客様の同意を確認する | パートナー センター
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Learn how to confirm customer acceptance of the Microsoft Customer Agreement. This may be needed to order Microsoft products and services for customers.
author: LauraBrenner
ms.author: labrenne
keywords: 顧客, お客様, 同意, MCA, Microsoft Cloud 契約, Microsoft 顧客契約, 顧客契約テンプレート
ms.localizationpriority: medium
ms.openlocfilehash: 9d362f581d0d318b1a457ba6a75db54713fce6bb
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252233"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Confirm customer acceptance of the Microsoft Customer Agreement

Currently, before a CSP partner can place order on a customer's behalf, the customer must accept and sign the applicable **Microsoft Cloud Agreement**. その後、パートナーは、署名者に関する情報を Microsoft に提供することで、お客様にその同意を確認する必要があります。 確認が行われていない場合:
- You won't be able to create new orders for this customer.
- You won't be able to change the seat count of existing seat-based subscriptions for this customer.

パートナー センター ダッシュボードまたは API を使用して、Microsoft Cloud 契約へのお客様の同意を確認する方法の詳細については、「[Microsoft Cloud 契約へのお客様の同意を確認する](confirm-consent.md)」を参照してください。

2019 年 10 月 1 日に、Microsoft では、CPS プログラムに **Microsoft 顧客契約**を導入する予定です。これは、Microsoft Cloud 契約に置き換わります。 新しい契約へのパートナーの移行を促進するために、現在の Microsoft Cloud 契約は、2020 年 1 月 31 まで CSP プログラムでサポートされます。 スケジュールの詳細については、次の表を参照してください。

| 日付 | マイルストーン | 詳細 |
|------------|------------|--------------------------------|
|2019 年 8 月 1 日|サンドボックスで UX プレビューの提供開始|パートナーは、CSP サンドボックス環境でパートナー センター ダッシュボードを使用して、Microsoft 顧客契約へのお客様の同意を確認できます。 CSP サンドボックス環境へのアクセス権を持つパートナーは、ユーザー エクスペリエンスの変更をプレビューできます。 サンドボックス環境へのアクセス権を持たないパートナーは、その変更をこのトピックで確認できます。|
|2019 年 9 月 3 日|サンドボックスで API プレビューの提供開始。|パートナーは、CSP サンドボックス環境でパートナー センター API を使用して、Microsoft 顧客契約へのお客様の同意を確認できます。 API パートナーは、この機会を利用して API の変更をプレビューし、新しい契約をサポートするために API の統合作業を開始できます。|
|September 20, 2019|サンドボックスで .NET SDK プレビューの提供開始。|パートナーは、CSP サンドボックス環境内でパートナー センター .NET SDK を使用して、Microsoft 顧客契約へのお客様の同意を確認できます。 API パートナーは、この機会を利用して .NET SDK の変更のプレビューを表示し、新しい契約をサポートするために API の統合作業を開始できます。|
|2019 年 10 月 1 日|Microsoft 顧客契約が運用環境で使用可能|Microsoft では、Microsoft 顧客契約を CSP プログラムに導入します。これは、Microsoft Cloud 契約に置き換わるものです。 パートナーは、運用環境でパートナー センター ダッシュボードと API を使用して、Microsoft 顧客契約へのお客様の同意を確認できます。 Microsoft Cloud 契約は、CSP パートナー プログラムで引き続きサポートされます。 ただし、パートナーは、Microsoft 顧客契約への移行を開始することをお勧めします。 新しい購入および既存のサブスクリプションに対するシート数の変更では、Microsoft 顧客契約または Microsoft Cloud 契約のいずれかへのパートナーの確認が必要になります。 特定の新しいオファー (新しい Azure プランなど) では、Microsoft 顧客契約への同意の確認が求められます。|
|2020 年 1 月 31 日|Microsoft クラウド契約が運用環境から削除|Microsoft Cloud 契約は CSP パートナー プログラムでは受け入れられなくなりました。 新しい購入および既存のサブスクリプションに対するシート数の変更では、パートナーは、Microsoft 顧客契約の確認を提供する必要があります。 この要件は、以前に Microsoft Cloud 契約に同意した場合でも、新しいお客様および既存のお客様に適用されます。|

## <a name="access-microsoft-customer-agreement-template"></a>Access Microsoft Customer Agreement template
Partners can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement). Note that the Microsoft Customer Agreement is country-specific. When requesting for the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location. 

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Confirm customer acceptance using Partner Center API/SDK
Partners can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement. For details on the API/SDK, please refer to:

- [Microsoft 顧客契約の契約メタデータを取得する](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [Microsoft 顧客契約へのお客様の同意を確認する](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Microsoft 顧客契約に関するお客様の同意の確認を取得する ](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [Microsoft 顧客契約テンプレートのダウンロード リンクを取得する](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)


## <a name="confirm-customer-acceptance-in-partner-center"></a>パートナー センターを使用してお客様の同意を確認する
Partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new customers and existing customers.

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
