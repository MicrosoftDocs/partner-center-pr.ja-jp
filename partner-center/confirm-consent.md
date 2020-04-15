---
title: Microsoft 顧客契約へのお客様の同意を確認する | パートナー センター
ms.topic: article
ms.date: 04/07/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Microsoft 顧客契約に対する顧客の同意を確認する方法について説明します。 これは、顧客のために Microsoft の製品やサービスを注文するのに必要になる場合があります。
author: LauraBrenner
ms.author: labrenne
keywords: 顧客, お客様, 同意, MCA, Microsoft 顧客契約, 顧客契約テンプレート
ms.localizationpriority: high
ms.openlocfilehash: 2223a8e05a9df4c2d6ac377fc6f6b5a06944adc9
ms.sourcegitcommit: ee7f8600f566799838bda64e26c54799137f2cd5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2020
ms.locfileid: "81123324"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Microsoft 顧客契約に対する顧客の同意を確認する

**適用対象**
-  パートナー センター

**適切なロール**

- 管理エージェント
- 販売代理店

> [!NOTE]
> 契約リソースは、現在、Microsoft パブリック クラウドのパートナー センターでのみサポートされています。 以下には適用されません。
> * 21Vianet が運営するパートナー センター
> * Microsoft Cloud ドイツのパートナー センター
> * 米国政府機関向け Microsoft Cloud のパートナー センター

>[!NOTE]
>2020 年 1 月 31 日の時点で、すべてのお客様 (既存および新規) は新しい Microsoft 顧客契約に署名する必要があります。 詳細については、「[Microsoft 顧客契約に対する顧客の同意を確認する](confirm-customer-agreement.md)」を参照してください。

パートナーは、お客様のために Microsoft の製品やサービスを注文する前に、Microsoft 顧客契約へのそのお客様の同意を得る必要があります。 パートナーがコンプライアンス要件を満たすことができるように、マイクロソフトでは、パートナーに対して、契約に同意したユーザーに関する以下の詳細情報を提供することにより、同意を確認することを求めています。

- 名

- 姓

- 電子メール アドレス

- 電話番号 (オプション)

- 同意の日付

直接請求パートナーと間接プロバイダーは、パートナー センターまたはパートナー センター API 経由で取引するときに、Microsoft 顧客契約へのお客様の同意を確認する必要があります。 確認は*必須*です。

特定のお客様について確認が提供されていない場合:

-    このお客様について新しい注文を作成することはできません。

-    このお客様について既存のシート ベースのサブスクリプションのシート数を変更することはできません。

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

3. **[Microsoft 顧客契約]** で、 **[The customer has accepted the latest Microsoft customer agreement] (お客様は最新の Microsoft 顧客契約に同意しました)** を選択します。
4. **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。
5. 同意しているユーザーの詳細を入力します。

![同意の日付を追加する](images/mca/MCA3.png)

既定では、第一連絡先担当者のユーザー情報が表示されます。 これが正しくない場合は、 **[更新]** を選択し、契約に同意したユーザーの **[名]** 、 **[姓]** 、 **[メール アドレス]** 、* *[電話番号]* (省略可能) を入力します。

6. **[次へ]** を選択して、お客様のテナントを作成する残りの手順を続行します。

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>既存のお客様についてお客様の同意を確認する

これを行うには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** を選択し、表示するお客様を検索して選択します。
2. **[アカウント情報]** を選択します。
3. **[Microsoft 顧客契約]** で、 **[更新]** を選択します。

![更新プログラム、更新](images/mca/mca4.png)

4. 契約に同意したユーザーの**名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。
5. **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。
6. **[Save and continue]** (保存して続行) を選択します。

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>既存のお客様について新しい注文の作成中にお客様の同意を確認する

まだ確認していない既存のお客様について新しい注文を作成しようとすると、確認を完了するよう求めるプロンプトが表示されます。 この場合、次の手順を実行します。

1. 契約に同意したユーザーの**名**、**姓**、**メール アドレス**、**電話番号** (省略可能) を入力します。
2. **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。
3. **[Save and continue]** (保存して続行) を選択します。

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>既存のお客様についてお客様の同意の確認を取得する

以下の手順を使用して、既存のお客様について以前に提供したお客様の同意確認を取得することができます。 これを行うには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** を選択し、表示するお客様を検索して選択します。
2. **[アカウント情報]** を選択します。
3. **[Microsoft 顧客契約]** に、このお客様について確認が得られているかどうかが表示されます。
