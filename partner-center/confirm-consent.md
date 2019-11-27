---
title: Microsoft Cloud 契約に関するお客様の同意を確認する | パートナー センター
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Microsoft Cloud 契約のお客様の同意を確認する方法について説明します。 これは、お客様に Microsoft 製品とサービスを注文するために必要になる場合があります。
author: LauraBrenner
ms.author: labrenne
keywords: 顧客, 顧客たち, 同意, MCA, Microsoft Cloud 契約, 顧客契約テンプレート
ms.localizationpriority: medium
ms.openlocfilehash: d9b2df8f9cf8795eedb75bc23773942e365c83fe
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252590"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Microsoft Cloud 契約に関するお客様の同意を確認する

**適用対象**
-  パートナー センター

> [!NOTE]
> 契約リソースは、現在、Microsoft パブリック クラウドのパートナー センターでのみサポートされています。 以下には適用されません。
> * 21Vianet が運営するパートナー センター
> * Microsoft Cloud ドイツのパートナー センター
> * 米国政府機関向け Microsoft Cloud のパートナー センター

>[!NOTE]
>この契約は、2020年1月31日まで有効です。 その後、すべてのお客様 (既存および新規) は、新しい Microsoft カスタマー契約に署名する必要があります。 詳細については、「 [Microsoft カスタマーアグリーメントに対する顧客の同意を確認](confirm-customer-agreement.md)する」を参照してください。

パートナーは、その顧客に対して Microsoft 製品とサービスを注文する前に、お客様の Microsoft Cloud 契約に同意する必要があります。 パートナーがコンプライアンス要件を満たすことができるように、マイクロソフトでは、パートナーに対して、契約に同意したユーザーに関する以下の詳細情報を提供することにより、同意を確認することを求めています。 

-   名

-   姓

-   メール アドレス

-   電話番号 (オプション)

-   同意の日付

詳細については、[Microsoft Cloud 契約のお客様の同意確認に関してよく寄せられる質問](https://docs.microsoft.com/partner-center/confirm-consent-faq)を参照してください。

直接請求パートナーと間接プロバイダーは、パートナー センターまたはパートナー センター API を介して取引するときに、Microsoft Cloud 契約に関するお客様の同意を確認する必要があります。 確認は*必須*です。

特定のお客様について確認が提供されていない場合:

-   この顧客に対して新しい注文を作成することはできません。

-   この顧客の既存の接続クライアントライセンスの数を変更することはできません。

お客様の同意は、パートナー センターまたはパートナー センター API を使用して確認できます。 パートナー センター API でこれを行うには、以下のトピックを参照してください。 

-   [顧客の同意を確認する](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [契約メタデータを取得する](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [顧客の同意を確認する](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


これは、運用環境とサンド ボックス環境の両方に適用されます。

## <a name="confirming-customer-acceptance-in-partner-center"></a>パートナー センターを使用してお客様の同意を確認する

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>新しいお客様についてお客様の同意を確認する

パートナー センターで、新しいお客様のテナントを作成するときに、お客様の同意を確認するのには、次の手順に従います。 これを行うには、管理エージェントまたは販売エージェントである必要があることに注意してください。

1. **[顧客]** 、 **[新しい顧客]** 、 **[アカウント情報]** の順に選択します。
2. **会社**と**主要連絡先**に関する情報を入力します。

![会社情報](images/mca/mca1.png)

3. **[Microsoft Cloud 契約]** で **[The customer has accepted the latest Microsoft cloud agreement]** (顧客が最新の Microsoft Cloud 契約に同意済み) を選択します。
4. **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。
5. 同意しているユーザーの詳細を入力します。

![同意の日付を追加する](images/mca/MCA3.png)

既定では、第一連絡先担当者のユーザー情報が表示されます。 これが正しくない場合は、 **[更新]** を選択し、契約に同意したユーザーの**名**、**姓**、**電子メールアドレス**、**電話番号*(オプション) を入力します。

6. **[次へ]** を選択して、お客様のテナントを作成する残りの手順を続行します。

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>既存のお客様についてお客様の同意を確認する

これを行うには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** を選択し、表示するお客様を検索して選択します。
2. **[アカウント情報]** を選択します。
3. **[Microsoft Cloud 契約]** で **[更新]** を選択します。

![更新](images/mca/mca4.png)

4. 契約に同意したユーザーの**名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。
5. **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。
6. **[Save and continue]** (保存して続行) を選択します。

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>既存のお客様について新しい注文の作成中にお客様の同意を確認する

以前に確認していない既存の顧客に対して新しい注文を作成しようとすると、確認を完了するためのプロンプトが表示されます。 この場合、次の手順を実行します。

1. 契約に同意したユーザーの**名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。
2. **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。
3. **[Save and continue]** (保存して続行) を選択します。

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>既存のお客様についてお客様の同意の確認を取得する

以下の手順を使用して、既存のお客様について以前に提供したお客様の同意確認を取得することができます。 これを行うには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** を選択し、表示するお客様を検索して選択します。
2. **[アカウント情報]** を選択します。
3. **Microsoft cloud agreement**で、この顧客に対して確認が提供されているかどうかを確認します。
