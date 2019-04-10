---
title: Microsoft Cloud 契約に関するお客様の同意を確認する | パートナー センター
ms.topic: article
ms.date: 04/5/2019
Description: パートナーは、お客様の Microsoft 製品とサービスを注文する前に、Microsoft Cloud 契約へのお客様の同意を得る必要があります。 より適切パートナー コンプライアンス要件、Microsoft パートナーの要求を特定の契約書に同意したユーザーについての詳細を提供することで同意を確認します。
author: LauraBrenner
ms.author: v-petand
keywords: 顧客、顧客、同意、MCA、Microsoft Cloud の契約、顧客の契約書のテンプレート
ms.localizationpriority: medium
ms.openlocfilehash: 28bc7c1dea842f9fbfc2778dfad1a8e5615a6bd7
ms.sourcegitcommit: 275d3eee5613d52f0ac7b8c78f7a7ddd74f56c9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/10/2019
ms.locfileid: "59430131"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Microsoft Cloud 契約に関するお客様の同意を確認する

**対象**
-  パートナー センター

パートナーは、お客様の Microsoft 製品とサービスを注文する前に、Microsoft Cloud 契約へのお客様の同意を得る必要があります。 パートナーがコンプライアンス要件を満たすことができるように、マイクロソフトでは、パートナーに対して、契約に同意したユーザーに関する以下の詳細情報を提供することにより、同意を確認することを求めています。 

-   名

-   姓

-   メール アドレス

-   電話番号

-   同意の日付

詳細については、Microsoft Cloud の契約のお客様承諾の確認を参照してください。[よく寄せられる質問](https://docs.microsoft.com/en-us/partner-center/confirm-consent-faq)します。

パートナーの請求書を直接と間接プロバイダーは、パートナーまたはパートナー センター API を介して処理するときに、Microsoft クラウドの契約の顧客による受け入れを確認する必要があります。 確認は*必須*です。

特定のお客様について確認が提供されていない場合:

-   このお客様について新しい注文を作成することはできません。

-   このお客様について既存のシート ベースのサブスクリプションのシート数を変更することはできません。

パートナー センターまたはパートナー センター API を使用して、顧客による受け入れの確認を実行できます。 これには、パートナー センター API を介して、以下のトピックを参照してください。 

-   [お客様の同意の確認を取得します。](https://docs.microsoft.com/en-us/partner-center/develop/get-confirmation-of-customer-consent)

-   [アグリーメントのメタデータを取得します。](https://docs.microsoft.com/en-us/partner-center/develop/get-agreement-metadata)

-   [お客様の同意を確認します。](https://docs.microsoft.com/en-us/partner-center/develop/confirm-customer-consent)


お客様の同意の確認は、Microsoft Public Cloud でのみサポートされています。

これは、運用環境とサンド ボックス環境の両方に適用されます。

## <a name="confirming-customer-acceptance-in-partner-center"></a>パートナー センターで顧客による受け入れを確認します。

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>新しいお客様についてお客様の同意を確認する

パートナー センターで、新しい顧客のテナントを作成するときに、顧客による受け入れを確認するのにには、次の手順を使用します。 これを行うには、管理エージェントまたは販売エージェントである必要があることに注意してください。
 
1.  選択**顧客**、し**新しい顧客**し、**アカウント情報**します。

2.  **会社**と**主要連絡先**に関する情報を入力します。

![会社情報](images/mca/mca1.png)

3.  **[Microsoft Cloud 契約]** で **[The customer has accepted the latest Microsoft cloud agreement]** (顧客が最新の Microsoft Cloud 契約に同意済み) を選択します。 

4.  **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。

5.  同意しているユーザーの詳細を入力します。 

![同意される日付を追加します。](images/mca/MCA3.png)

既定では、第一連絡先担当者のユーザー情報が表示されます。 これが正しくない場合は、**[更新]** を選択し、契約に同意したユーザーの **名**、**姓**、**メール アドレス**、**電話番号* (省略可能) を入力します。

6.  **[次へ]** を選択して、お客様のテナントを作成する残りの手順を続行します。

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>既存のお客様についてお客様の同意を確認する

これを行うには、管理エージェントまたは販売エージェントである必要があります。 

1.  **[顧客]** を選択し、表示するお客様を検索して選択します。 

2.  選択**アカウント情報**します。

3.  **[Microsoft Cloud 契約]** で **[更新]** を選択します。

![更新](images/mca/mca4.png)

4.  契約に同意したユーザーの**名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。

5.  **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。

6.  **[Save and continue]** (保存して続行) を選択します。

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>既存のお客様について新しい注文の作成中にお客様の同意を確認する

以前に確認していない既存のお客様について新しい注文を作成しようとすると、確認を完了するよう求めるプロンプトが表示されます。 この場合、次の手順を実行します。 

1.  契約に同意したユーザーの**名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。

2.  **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。

3.  **[Save and continue]** (保存して続行) を選択します。


### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>既存のお客様についてお客様の同意の確認を取得する

以下の手順を使用して、既存のお客様について以前に提供したお客様の同意確認を取得することができます。 これを行うには、管理エージェントまたは販売エージェントである必要があります。 

1.  **[顧客]** を選択し、表示するお客様を検索して選択します。 

2.  選択**アカウント情報**します。

3.  **[Microsoft Cloud 契約]** で、このお客様について確認が提供されているかどうかが表示されます。

