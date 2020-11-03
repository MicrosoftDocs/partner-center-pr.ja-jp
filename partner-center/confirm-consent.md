---
title: Microsoft 顧客契約へのお客様の同意を確認する
description: Microsoft 顧客契約に対する顧客の同意を確認する方法について説明します。 これは、顧客のために Microsoft の製品やサービスを注文するのに必要になる場合があります。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: aacca72e9af45b2777364734c2b07dbe8101989d
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/19/2020
ms.locfileid: "92333920"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Microsoft 顧客契約に対するお客様の同意を確認する方法 (更新版)

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

直接請求パートナーと間接プロバイダーは、パートナー センターまたはパートナー センター API 経由で取引するときに、Microsoft 顧客契約へのお客様の同意を確認する必要があります。 確認は *必須* です。

特定のお客様について確認が提供されていない場合:

- このお客様について新しい注文を作成することはできません。

- このお客様について既存のライセンス ベースのサブスクリプションのライセンス数を変更することはできません。

お客様の同意は、パートナー センターまたはパートナー センター API を使用して確認できます。 パートナー センター API でこれを行うには、以下のトピックを参照してください。

- [顧客の同意を確認する](/partner-center/develop/get-confirmation-of-customer-consent)

- [契約メタデータを取得する](/partner-center/develop/get-agreement-metadata)

- [顧客の同意を確認する](/partner-center/develop/confirm-customer-consent)

これは、運用環境とサンド ボックス環境の両方に適用されます。

## <a name="confirm-customer-acceptance-for-a-new-customer"></a>新しいお客様についてお客様の同意を確認する

パートナー センターで、新しいお客様のテナントを作成するときに、お客様の同意を確認するのには、次の手順に従います。 これを行うには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** 、 **[新しい顧客]** 、 **[アカウント情報]** の順に選択します。

2. **会社** と **主要連絡先** に関する情報を入力します。

   :::image type="content" source="images/mca/mca1.png" alt-text="会社情報":::

3. **[Microsoft 顧客契約]** で、 **[The customer has accepted the latest Microsoft customer agreement] (お客様は最新の Microsoft 顧客契約に同意しました)** を選択します。

4. **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。

5. 同意しているユーザーの詳細を入力します。

   :::image type="content" source="images/mca/MCA3.png" alt-text="会社情報":::

   既定では、第一連絡先担当者のユーザー情報が表示されます。 これが正しくない場合は、 **[更新]** を選択し、契約に同意したユーザーの **[名]** 、 **[姓]** 、 **[メール アドレス]** 、* *[電話番号]* (省略可能) を入力します。

6. **[次へ]** を選択して、お客様のテナントを作成する残りの手順を続行します。

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a>既存のお客様についてお客様の同意を確認する

これを行うには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** を選択し、表示するお客様を検索して選択します。

2. **[アカウント情報]** を選択します。

3. **[Microsoft 顧客契約]** で、 **[更新]** を選択します。

   :::image type="content" source="images/mca/mca4.png" alt-text="会社情報":::

4. 契約に同意したユーザーの **名** 、 **姓** 、 **メール アドレス** 、 **電話番号** (省略可能) を入力します。

5. **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。

6. **[Save and continue]** (保存して続行) を選択します。

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>既存のお客様について新しい注文の作成中にお客様の同意を確認する

まだ確認していない既存のお客様について新しい注文を作成しようとすると、確認を完了するよう求めるプロンプトが表示されます。 この場合、次の手順を実行します。

1. 契約に同意したユーザーの **名** 、 **姓** 、 **メール アドレス** 、 **電話番号** (省略可能) を入力します。

2. **[Agreement acceptance date]** (契約同意日) で、適切な日付を入力します。 将来の日付に設定することはできません。

3. **[Save and continue]** (保存して続行) を選択します。

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>既存のお客様についてお客様の同意の確認を取得する

以下の手順を使用して、既存のお客様について以前に提供したお客様の同意確認を取得することができます。 これを行うには、管理エージェントまたは販売エージェントである必要があります。

1. **[顧客]** を選択し、表示するお客様を検索して選択します。

2. **[アカウント情報]** を選択します。

3. **[Microsoft 顧客契約]** に、このお客様について確認が得られているかどうかが表示されます。

## <a name="next-steps"></a>次のステップ

- [CSP パートナー プログラムで Microsoft 顧客契約への顧客の同意を確認する](confirm-customer-agreement.md)

- [顧客に代わって Microsoft 顧客契約の同意を証明する](attest-acceptance-customer-agreement.md)