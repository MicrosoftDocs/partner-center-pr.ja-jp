---
title: 顧客が CSP プログラムの Microsoft 顧客契約に同意していることを確認する方法
description: クラウド ソリューション プロバイダー (CSP) パートナーは、顧客に代わって Microsoft サービスを注文する前に、Microsoft 顧客契約への顧客の同意を確認する必要があります。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633780"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>顧客が CSP プログラムの Microsoft 顧客契約に同意していることを確認する方法

**適切なロール**

- 管理エージェント
- 販売代理店


顧客が Microsoft 顧客契約に同意するには、次の 2 つのオプションがあります。

**オプション 1**:顧客の同意に対するパートナー証明 - パートナーは、パートナー センター API/SDK を使用するか、パートナー センター ダッシュボードを使用して、顧客の同意を確認できます。

**オプション 2**:顧客の直接同意 - パートナーは、URL を使用して、Microsoft 365 管理センターで契約を確認し、同意するように顧客に要請できます。

## <a name="access-microsoft-customer-agreement-template"></a>Microsoft 顧客契約テンプレートへのアクセス

最新バージョンの Microsoft 顧客契約テンプレートは、[こちら](https://aka.ms/customeragreement)から手動でダウンロードできます。 Microsoft 顧客契約は国によって異なります。 Microsoft 顧客契約テンプレートを要求するときは、顧客の所在地に応じて正しい国を選択してください。

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>オプション 1:パートナー センターを使用してお客様の同意を確認する

直接請求パートナーは、新規の顧客と既存の顧客について、パートナー センターで Microsoft 顧客契約に対する顧客の同意を確認できます。 間接リセラーは顧客に代わって証明を行うことができません。間接プロバイダーと協力して、証明を完了する必要があります。

### <a name="confirm-customer-acceptance-for-new-customers"></a>新しいお客様について、お客様の同意を確認する

パートナー センターで新しい顧客テナントを作成するときに、次の手順を使用して、Microsoft 顧客契約へのお客様の同意を確認します。 この手順を実行するには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** を選択し、 **[新しい顧客]** を選択します。

2. **[アカウント情報]** で、会社と主要連絡先の情報を入力します。

3. **[Microsoft agreement]\(Microsoft 契約\)** で、ボックスをオンにして、顧客が Microsoft 顧客契約に同意していることを証明します。

4. **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。

5. 表示されたユーザーの主要連絡先情報が正しいことを確認します。 正しくない場合は、 **[更新]** を選択し、契約に同意した人の正確な情報を入力します。

6. **[次へ]** を選択して、顧客のテナントの作成を続行します。

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="新しい顧客":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>既存のお客様について、お客様の同意を確認する

これを行うには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** を選択します。 顧客を検索して選択します。

2. **[アカウント情報]** を選択します。

3. **[Microsoft 顧客契約]** で **[更新]** を選択します。

4. 契約に同意したユーザーの **名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。 **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。

5. **[保存]** を選択して続行します。

   :::image type="content" source="images/mcua2-update2.png" alt-text="既存の顧客":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>お客様の同意の確認を取得する

既存の顧客が Microsoft 顧客契約に同意したことを示す確認を取得するには、次の手順を使用します。 これを行うには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** を選択し、表示するお客様を検索して選択します。

2. **[アカウント情報]** を選択します。

3. **Microsoft 顧客契約** で、この顧客による確認の提供の有無を表示します。

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>パートナー センター API/SDK を使用して顧客の同意を確認する

パートナー センター API/SDK を使用して、Microsoft 顧客契約に対する顧客の同意を確認できます。 API/SDK について詳しくは、以下をご覧ください。

- [Microsoft 顧客契約の契約メタデータを取得する](/partner-center/develop/get-customer-agreement-metadata)

- [Microsoft 顧客契約へのお客様の同意を確認する](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Microsoft 顧客契約に関する顧客の同意の確認を取得する ](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Microsoft 顧客契約テンプレートのダウンロード リンクを取得する](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>オプション 2:Microsoft 365 管理センターでの顧客の同意

パートナーは、URL を使用して、Microsoft 365 管理センターで契約を確認し、同意するように新規および既存の顧客に要請できます。 次のいくつかのセクションでその方法を説明します。

- 新規の顧客を作成し、契約を確認して同意するよう顧客に要請します。

- リセラー関係とリセラー契約を確認して同意するよう新規の顧客に要請します。

- 契約を確認して同意するよう既存の顧客に要請します。

>[!NOTE]
> [パートナー センター API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) を使用して、Microsoft 顧客契約の顧客の直接同意の状況を確認できます。  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>新規の顧客を作成し、契約を確認して同意するよう顧客に要請する

パートナー センターで新規の顧客を作成し、Microsoft 365 管理センターで Microsoft 顧客契約を確認して同意するように要請するには、次の手順を使用します。

1. パートナー センターの **[顧客]** タブから、 **[顧客の追加]** を選択します。

2. **[アカウント情報]** で、顧客の会社名や主要連絡先など、すべての必須フィールドに新しい顧客に関する情報を入力します。

3. **[顧客契約]** で、 **[Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center]\(顧客は Microsoft 365 管理センターで Microsoft 顧客契約に同意するように求められます\)** を選択します。 ページの他の必須フィールドをすべて入力します。

4. **[次へ: 確認]** を選択し、顧客のテナントを作成する手順を続行します。 

>[!NOTE] 
>新規の顧客は、Microsoft 顧客契約に同意するまで購入を行うことはできません。  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="新規の顧客を作成する":::

5. 新規顧客のワークフローで **[確認]** 画面が表示されたら、顧客の資格情報を保存します。 これらの資格情報は、後で顧客に提供する必要があります。

6. パートナー センターの外部で、Microsoft 365 管理センターで Microsoft 顧客契約に同意するよう顧客に要請するメールを作成して送信します。 メールには次の点を必ず含めるようにします。

   - この [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) へのリンク (サインインが必要)

   - 手順 5 で保存した顧客の資格情報

7. 顧客がパートナーから要請メールを受け取り、[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) を選択します。

8. 顧客は、提供された顧客の資格情報を使用して Microsoft 365 管理センターにサインインします。

9. 顧客は、Microsoft 顧客契約に同意するためのチェック ボックスをオンにします。

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>リセラー関係と Microsoft 顧客契約を確認して同意するよう新規の顧客に要請する 

リセラー関係と Microsoft 顧客契約を確認して同意するよう新規の顧客に要請するには、次の手順を使用します。 

1. パートナー センターの **[顧客]** タブから、 **[リセラーの関係を要求する]** リンクを選択します。 

2. テキストとパラメーター化された URL を含む自動メール テンプレートが生成されます。この URL により、顧客は Microsoft 365 管理センターに誘導されます。

3. 自動的に生成されるメール テンプレートをカスタマイズして、 **[クリップボードにコピー]** か **[電子メールで開く]** を選択することもできます。

4. このメール テンプレートを使用して、 **[reseller relationship]\(リセラー関係\)** の要求と **[Microsoft 顧客契約]** に同意するよう顧客に要請します。 (注:パートナーは、この要請メールに、自動的に作成された URL と、先ほど作成された顧客の資格情報も含めてください。)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="関係を作成する":::

5. 顧客がメールで要請を受け取り、パラメーター化された URL をクリックします。 

6. 顧客は、メールで提供された資格情報を使用して、Microsoft 365 管理センターにサインインします。

7. 顧客が、 **[reseller relationship]\(リセラー関係\)** と **[Microsoft 顧客契約]** に同意するボックスをオンにします。 

8. 同じ URL 内で、顧客は、協力関係にあるさまざまなパートナーの一覧を統合して表示できます。 パートナーを選択すると、詳細を表示できます。

   :::image type="content" source="images/mca/accept.jpg" alt-text="契約に同意する":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>契約を確認して同意するよう既存の顧客に要請する

Microsoft 顧客契約を確認して同意するよう既存の顧客に要請するには、次の手順を使用します。 

1. Microsoft 顧客契約に同意するよう同意するよう顧客に要請する URL が埋め込まれた顧客宛のメールを作成します。

2. 顧客がメールで招待状を受け取り、[URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) をクリックします。 

3. 顧客が Microsoft 365 管理センターに資格情報を入力します。

4. 顧客が、Microsoft 顧客契約に同意するボックスをオンにします。 

5. 同じ URL 内で、顧客は、協力関係にあるさまざまなパートナーの一覧を統合して表示できます。 パートナーを選択すると、詳細を表示できます。

   :::image type="content" source="images/mca/customeraccept.png" alt-text="顧客":::

>[!NOTE]
>特定のシナリオでは、Microsoft 顧客契約に顧客が直接同意できない場合があります。 そのようなシナリオについて詳しくは、以下の「顧客の代わりに証明する必要がある 2 つのシナリオ」をご覧ください。

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>顧客の代わりに証明する必要がある 2 つのシナリオ

顧客が Microsoft 365 管理センター内で Microsoft 顧客契約に直接同意することができない可能性のあるシナリオが 2 つあります。

**シナリオ 1**: 既存の顧客が、既存のパートナー関係を通じて次のうちのいずれかを購入したことがある: プラン、ソフトウェアまたはソフトウェア サブスクリプション、予約インスタンス、Azure プラン。 顧客が新たな購入を行おうとしている (自動更新を除く)。 その顧客が URL をクリックすると、"Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement"(Microsoft 顧客契約に同意したことを確認するために、パートナーに連絡してください) というメッセージが表示されます。  

**解決策**:パートナーが顧客に代わって証明する必要があります。

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Microsoft 365 管理センターのページのスクリーンショット。Microsoft 顧客契約への同意を確認するためにパートナーに連絡するよう求められています。":::

**シナリオ 2**:既存の顧客が、次のうちいずれかを購入したことがある: プラン、ソフトウェアまたはソフトウェア サブスクリプション、予約インスタンス、Azure プラン。 顧客が新しいパートナーを通じて新たな購入を行おうとしている。

その顧客が Microsoft 365 管理センターへの URL をクリックして、新しいパートナー関係と契約に同意すると、"Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement"(Microsoft 顧客契約に同意したことを確認するために、パートナーに連絡してください) というメッセージが表示されます。  

**解決策**:パートナーが顧客に代わって証明する必要があります。  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>顧客が契約に同意したことを確認する

まだ確認していない既存のお客様について新しい注文を作成しようとすると、確認を完了するよう求めるプロンプトが表示されます。 この場合、次の手順を実行します。

1. 契約に同意したユーザーの **名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。

2. **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。

3. **[Save and continue]** (保存して続行) を選択します。 

## <a name="next-steps"></a>次のステップ

- [会社のプロファイルの情報を確認または更新する](update-your-partner-profile.md)
- [Microsoft 顧客契約 (地域、言語別)](Agreements.md)
