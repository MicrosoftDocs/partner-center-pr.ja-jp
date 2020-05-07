---
title: Microsoft 顧客契約へのお客様の同意を確認する | パートナー センター
ms.topic: article
ms.date: 02/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Microsoft 顧客契約に対する顧客の同意を確認する方法について説明します。 これは、顧客のために Microsoft の製品やサービスを注文するのに必要になる場合があります。
author: LauraBrenner
ms.author: labrenne
keywords: 顧客, お客様, 同意, MCA, Microsoft Cloud 契約, Microsoft 顧客契約, 顧客契約テンプレート
ms.localizationpriority: high
ms.openlocfilehash: a40d5fa1d737dd679699db467ce8b3b1be81f84b
ms.sourcegitcommit: 1125391fd9a1ded2a051968b3a280a10676ed8bb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/04/2020
ms.locfileid: "82741051"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Microsoft 顧客契約に対する顧客の同意を確認する

**適用対象**

- パートナー センター
- Microsoft 365 管理センター

**適切なロール**

- 管理エージェント
- 販売代理店

**適切なパートナーの種類**

- 間接リセラー、直接請求、間接プロバイダー


2019 年 10 月 1 日に、Microsoft Cloud 契約に置き換わるものとして、CPS プログラムに **Microsoft 顧客契約**が導入されました。 間接リセラー向けの追加の[ガイダンス](indirect-reseller-tasks-in-partner-center.md)をご覧ください。 新しい契約へのパートナーの移行を促進するために、2020 年 1 月 31 までは両方の契約が CSP プログラムで共存していました。 2020 年 2 月 1 日に、Microsoft Cloud 契約は Microsoft 顧客契約に置き換わりました。

顧客が Microsoft 顧客契約に同意するには、次の 2 つのオプションがあります。 

**オプション 1**:顧客の同意に対するパートナー証明 - パートナーは、パートナー センター API/SDK を使用するか、パートナー センター ダッシュボードを使用して、顧客の同意を確認できます。

**オプション 2**:顧客の直接同意 - パートナーは、URL を使用して、Microsoft 365 管理センターで契約を確認し、同意するように顧客に要請できます。

## <a name="access-microsoft-customer-agreement-template"></a>Microsoft 顧客契約テンプレートへのアクセス

最新バージョンの Microsoft 顧客契約テンプレートは、[こちら](https://aka.ms/customeragreement)から手動でダウンロードできます。 Microsoft 顧客契約は国によって異なります。 Microsoft 顧客契約テンプレートを要求するときは、顧客の所在地に応じて正しい国を選択してください。 

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>オプション 1:パートナー センターを使用してお客様の同意を確認する

パートナーは、新規の顧客と既存の顧客について、パートナー センターで Microsoft 顧客契約に対する顧客の同意を確認できます。 リセラーは顧客に代わって証明を行うことができません。間接プロバイダーと協力して、証明を完了する必要があります。

### <a name="confirm-customer-acceptance-for-new-customers"></a>新しいお客様について、お客様の同意を確認する

パートナー センターで新しい顧客テナントを作成するときに、次の手順を使用して、Microsoft 顧客契約へのお客様の同意を確認します。 この手順を実行するには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** を選択し、 **[新しい顧客]** を選択します。

2. **[アカウント情報]** で、会社と主要連絡先の情報を入力します。

3. **[Microsoft agreement]\(Microsoft 契約\)** で、ボックスをオンにして、顧客が Microsoft 顧客契約に同意していることを証明します。 

4. **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。

5. 表示されたユーザーの主要連絡先情報が正しいことを確認します。 正しくない場合は、 **[更新]** を選択し、契約に同意した人の正確な情報を入力します。

6. **[次へ]** を選択して、顧客のテナントの作成を続行します。

![新しい顧客](images/mca/newcustomeragreement.jpg)  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>既存のお客様について、お客様の同意を確認する

これを行うには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** を選択します。 顧客を検索して選択します。

2. **[アカウント情報]** を選択します。

3. **[Microsoft 顧客契約]** で **[更新]** を選択します。

4. 契約に同意したユーザーの**名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。 **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。

5. **[保存]** を選択して続行します。

![既存の顧客](images/mcua2-update2.png)

### <a name="retrieve-confirmation-of-customer-acceptance"></a>お客様の同意の確認を取得する

次の手順に従って、既存のお客様が Microsoft 顧客契約に同意したことを示す確認を取得できます。 これを行うには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** を選択し、表示するお客様を検索して選択します。

2. **[アカウント情報]** を選択します。

3. **Microsoft 顧客契約** で、この顧客による確認の提供の有無を表示します。

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>パートナー センター API/SDK を使用して顧客の同意を確認する

パートナー センター API/SDK を使用して、Microsoft 顧客契約に対する顧客の同意を確認できます。 API/SDK について詳しくは、以下をご覧ください。

- [Microsoft 顧客契約の契約メタデータを取得する](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [Microsoft 顧客契約へのお客様の同意を確認する](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Microsoft 顧客契約に関するお客様の同意の確認を取得する ](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [Microsoft 顧客契約テンプレートのダウンロード リンクを取得する](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)


## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>オプション 2:Microsoft 365 管理センターでの顧客の同意

パートナーは、URL を使用して、Microsoft 365 管理センターで契約を確認し、同意するように新規および既存の顧客に要請できます。 次のいくつかのセクションでその方法を説明します。

- 新規の顧客を作成し、契約を確認して同意するよう顧客に要請します。

- リセラー関係とリセラー契約を確認して同意するよう新規の顧客に要請します。

- 契約を確認して同意するよう既存の顧客に要請します。

>[!NOTE]
> [パートナー センター API/SDK](https://docs.microsoft.com/partner-center/develop/get-direct-sign-status-of-customer-agreement) を使用して、Microsoft 顧客契約の顧客の直接同意の状況を確認できます。  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>新規の顧客を作成し、契約を確認して同意するよう顧客に要請する

パートナー センターで新規の顧客を作成し、Microsoft 365 管理センターで Microsoft 顧客契約を確認して同意するように要請するには、次の手順を使用します。

1. パートナー センターの **[顧客]** タブから、 **[顧客の追加]** を選択します。

2. **[アカウント情報]** で、顧客の会社名や主要連絡先など、すべての必須フィールドに新しい顧客に関する情報を入力します。

3. **[顧客契約]** で、最初のオプション **[Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center]\(顧客は Microsoft 365 管理センターで Microsoft 顧客契約に同意するように求められます\)** を選択します。 ページの他の必須フィールドをすべて入力します。

4. **[次へ: 確認]** を選択し、顧客のテナントを作成する手順を続行します。 (注:新規の顧客は、Microsoft 顧客契約に同意するまで新しい購入を行うことはできません。)  

![新規の顧客を作成する](images/mca/create-new-customer.jpg)

5. 新規顧客のワークフローで **[確認]** 画面が表示されたら、顧客の資格情報を保存します。 これらの資格情報は、後で顧客に提供する必要があります。

6. パートナー センターの外部で、Microsoft 365 管理センターで Microsoft 顧客契約に同意するよう顧客に要請するメールを作成して送信します。 メールには次の点を必ず含めるようにします。

   - この [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) へのリンク (サインインが必要)

   - 手順 5 で保存した顧客の資格情報

7. 顧客がパートナーから要請メールを受け取り、[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) を選択します。

8. 顧客が、パートナーから受信した顧客の資格情報を使用して Microsoft 365 管理センターにサインインします。

9. 顧客が、Microsoft 顧客契約に同意するボックスをオンにします。

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>リセラー関係と Microsoft 顧客契約を確認して同意するよう新規の顧客に要請する 

リセラー関係と Microsoft 顧客契約を確認して同意するよう新規の顧客に要請するには、次の手順を使用します。 

1. パートナー センターの **[顧客]** タブから、 **[リセラーの関係を要求する]** リンクを選択します。 

2. テキストとパラメーター化された URL を含む自動メール テンプレートが生成されます。このメールにより、顧客は Microsoft 365 管理センターに誘導されます。

3. 自動的に生成されるメール テンプレートをカスタマイズして、 **[クリップボードにコピー]** か **[電子メールで開く]** を選択することもできます。

4. このメール テンプレートを使用して、 **[reseller relationship]\(リセラー関係\)** の要求と **[Microsoft 顧客契約]** に同意するよう顧客に要請します。 (注:パートナーは、この要請メールに、自動的に作成された URL と、先ほど作成された顧客の資格情報も含めてください。)

![関係を作成する](images/mca/createrelationship.png)

5. 顧客がメールで要請を受け取り、パラメーター化された URL をクリックします。 

6. 顧客が、メールでパートナーによって提供された資格情報を使用して、Microsoft 365 管理センターにサインインします。

7. 顧客が、 **[reseller relationship]\(リセラー関係\)** と **[Microsoft 顧客契約]** に同意するボックスをオンにします。 

8. 同じ URL 内で、顧客は、協力関係にあるさまざまなパートナーの一覧を統合して表示できます。 パートナーを選択すると、詳細を表示できます。

![契約に同意する](images/mca/accept.jpg)


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>契約を確認して同意するよう既存の顧客に要請する 

Microsoft 顧客契約を確認して同意するよう既存の顧客に要請するには、次の手順を使用します。 

1. Microsoft 顧客契約に同意するよう同意するよう顧客に要請する URL が埋め込まれた顧客宛のメールを作成します。

2. 顧客がメールで招待状を受け取り、[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) をクリックします。 

3. 顧客が Microsoft 365 管理センターに資格情報を入力します。

4. 顧客が、Microsoft 顧客契約に同意するボックスをオンにします。 

5. 同じ URL 内で、顧客は、協力関係にあるさまざまなパートナーの一覧を統合して表示できます。 パートナーを選択すると、詳細を表示できます。

![顧客](images/mca/customeraccept.png)

>[!NOTE]
>特定のシナリオでは、Microsoft 顧客契約に顧客が直接同意できない場合があります。 そのようなシナリオについて詳しくは、「[顧客の代わりに証明する必要がある 2 つのシナリオ](attest-acceptance-customer-agreement.md)」をご覧ください。

### <a name="historical-timeline-details"></a>履歴タイムラインの詳細

| 日付 | マイルストーン | 詳細情報 |
|------------|------------|--------------------------------|
|2019 年 8 月 1 日|サンドボックスで UX プレビューの提供開始|パートナーは、CSP サンドボックス環境でパートナー センター ダッシュボードを使用して、Microsoft 顧客契約へのお客様の同意を確認できます。 CSP サンドボックス環境へのアクセス権を持つパートナーは、ユーザー エクスペリエンスの変更をプレビューできます。 サンドボックス環境へのアクセス権を持たないパートナーは、その変更をこのトピックで確認できます。|
|2019 年 9 月 3 日|サンドボックスで API プレビューの提供開始。|パートナーは、CSP サンドボックス環境でパートナー センター API を使用して、Microsoft 顧客契約へのお客様の同意を確認できます。 API パートナーは、この機会を利用して API の変更をプレビューし、新しい契約をサポートするために API の統合作業を開始できます。|
|2019 年 9 月 20 日|サンドボックスで .NET SDK プレビューの提供開始。|パートナーは、CSP サンドボックス環境内でパートナー センター .NET SDK を使用して、Microsoft 顧客契約へのお客様の同意を確認できます。 API パートナーは、この機会を利用して .NET SDK の変更のプレビューを表示し、新しい契約をサポートするために API の統合作業を開始できます。|
|2019 年 10 月 1 日|Microsoft 顧客契約が運用環境で使用可能|Microsoft では、Microsoft 顧客契約を CSP プログラムに導入します。これは、Microsoft Cloud 契約に置き換わるものです。 パートナーは、運用環境でパートナー センター ダッシュボードと API を使用して、Microsoft 顧客契約へのお客様の同意を確認できます。 Microsoft Cloud 契約は、CSP パートナー プログラムで引き続きサポートされます。 ただし、パートナーは、Microsoft 顧客契約への移行を開始することをお勧めします。 新しい購入および既存のサブスクリプションに対するシート数の変更では、Microsoft 顧客契約または Microsoft Cloud 契約のいずれかへのパートナーの確認が必要になります。 特定の新しいオファー (新しい Azure プランなど) では、Microsoft 顧客契約への同意の確認が求められます。|
|2020 年 1 月 31 日|Microsoft クラウド契約が運用環境から削除|Microsoft Cloud 契約は CSP パートナー プログラムでは受け入れられなくなりました。 新しい購入および既存のサブスクリプションに対するシート数の変更では、パートナーは、Microsoft 顧客契約の確認を提供する必要があります。 この要件は、以前に Microsoft Cloud 契約に同意した場合でも、新しいお客様および既存のお客様に適用されます。|
|2020 年 2 月 3 日|パートナーは、URL を使用して、認証された Microsoft 365 管理センターで契約を確認し、同意するように顧客に要請するオプションを利用できるようになりました。 | 顧客は、Microsoft 365 管理センターで Microsoft 顧客契約に同意できます。 顧客が Microsoft 365 管理センターで契約に直接同意することにより、条件を承認したことが確認されます。 
