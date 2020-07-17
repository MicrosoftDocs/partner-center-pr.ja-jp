---
title: 暗号化マイニングアクティビティの通知
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 1つ以上の Azure サブスクリプションで潜在的な cryptocompare マイニング (または暗号化マイニング) に関する通知が表示された場合の意味について説明します。
author: aarzh-AaronZhang
ms.author: v-aarzh
robots: noindex, nofollow
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d691ef30bf01fcb25d686649291e92cfec47f100
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435201"
---
# <a name="partner-center-notification-for-cryptocurrency-mining-activity"></a>クリプトマイニング (仮想通貨の採掘) アクティビティに関するパートナー センター通知

**適用対象**

-  パートナー センター
-  CSP パートナー

パートナー センターに、クリプトマイニングに関する次のような通知が届くことがあります。

:::image type="content" source="images/crypto1.png" alt-text="パートナー センターでのセキュリティ通知の画像":::

この通知では、過去 1 週間以内に 1 つ以上の Azure サブスクリプションでクリプトマイニングが検出されたことをお知らせしています。 クリプトマイニングは必ずしも不正行為に相当するとは限りません。 ただし、Azure でのクリプトマイニング実行によるコストが金銭的な利益を上回る傾向にあるため、通常ではない行為であると言えます。

## <a name="checklist"></a>チェック リスト

皆様や皆様の顧客に影響する金融詐欺を防ぐには、次の手順をご検討ください。

1. 顧客のアカウントが良好な状態であることを確認します。 通知をクリックすると、サブスクリプションに直接アクセスできます。

2. サブスクリプションの Azure 利用パターンを確認します。 突発的な急増があれば、予想外のアクティビティを示している可能性があります。

3. 顧客にご連絡のうえ、そのアクティビティが想定内のものであるかどうかをご確認ください。

   そのアクティビティが想定内のものである場合は、顧客の Azure サブスクリプションの詳細ページに戻り、クリプトマイニングが正当であることを確認します。

   :::image type="content" source="images/crypto2.png" alt-text="顧客の Azure サブスクリプション詳細ページの画像":::

## <a name="steps-for-unexpected-activity"></a>予期しないアクティビティの手順

アクティビティが予想外のものである場合は、以下をご検討ください。

1. クリプトマイニング用の Azure リソースが不要であることを確認して削除します。これにより、Azure で料金がそれ以上発生することを回避できます。

2. そもそも、そのリソースがどのように作成されたものであるのかを把握します。 これには、Azure Resource Management ログによるリソース プロビジョニング アクティビティの確認が必要になることがあります。

3. サブスクリプションを作成したユーザーを確認する必要がある場合は、パートナー センターのアクティビティ ログを確認します。

クリプトマイニング アクティビティの検出はヒューリスティックに基づいたものであり、100% 正確ではない可能性があります。 不正行為やその他の許可されていないアクティビティに対する保護を行うには、ガバナンスと監視のシステムを備えてください。 詳しくは、「[未払い、詐欺、不正使用](https://docs.microsoft.com/partner-center/non-payment--fraud--or-misuse)」をご覧ください。

## <a name="contact-support-if-needed"></a>必要に応じてサポートにお問い合わせください

通知に関してご質問や懸念がある場合、次の手順でサポート要求を開くことができます。

1. パートナー センターで、**[サポート]** を選択し、**[Partner Center requests]\(パートナー センターの要求\)** を選択します。

2. [**新しい要求**] を選択します。 

3. **[問題の種類]** ドロップダウン メニューで、**[顧客の追加または管理]** を選択します。

4. **[影響]** ドロップダウンで、**[標準]** を選択します。

5. **[タイトル]** フィールドに、**クリプトマイニング通知**と入力します。

6. **[説明]** フィールドに、影響するサブスクリプション名と、他の質問や懸念点を入力します。

7. 連絡先情報を入力します。

8. **[Submit]\(送信\)** をクリックします。
