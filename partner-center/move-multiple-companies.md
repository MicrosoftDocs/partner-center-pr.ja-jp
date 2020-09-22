---
title: PMC からパートナーセンターへの会社の移行
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーメンバーシップセンター (PMC) からパートナーセンターに複数の企業を移行し、パートナーのグローバルアカウントに統合する場合の注意事項。
author: parthpandyaMSFT
ms.author: ParthP
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 459f347d960a06f78a30a398dc51b67f2fa7d27b
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000076"
---
# <a name="moving-multiple-companies-to-partner-center-from-partner-membership-center-pmc"></a>パートナーメンバーシップセンターからの複数の企業のパートナーセンターへの移行 (PMC)

**適切なロール**

- グローバル管理者
- ユーザー管理者
- 管理エージェント
- 販売代理店

会社アカウントを PMC からパートナー センターに移動するときに、複数のアカウントを移動する場合があります。 パートナー センターでは、これらのアカウントは 1 つのグローバル アカウント (PGA) に統合されます。 移動する最初のアカウントは、パートナーのグローバルアカウントと見なされ、それ以降のすべてのアカウントは、最初のアカウントの場所として統合されます。 会社の本社の PMC アカウントを使用して移動を開始します。 詳細については、 [PMC からパートナーセンターへの移行に関するガイドを参照する](guide-to-migration.md) か、この短いビデオ [マルチロケーションアカウントを簡単](https://vimeo.com/290335248)にご覧ください。

## <a name="move-your-additional-accounts-into-partner-center"></a>追加のアカウントをパートナー センターに移動する

既にパートナーセンターに1つの会社アカウントを移動したので、サインインすると、パートナーセンターに既に存在するアカウントを知ることができます。

移行した後、間違った会社のアカウントが法務業務として指定されていることがわかった場合は、その指定を変更できます。

1. ご自身の**パートナー プロファイル**に移動します。

2. 法務業務として指定する場所が場所の一覧にあることを確認します。 ない場合は、追加します。

3. **[Update legal business profile]\(法的ビジネスプロファイルの更新\)** を選択します。

4. ビジネスと地域を選択し、保存します。

:::image type="content" source="images/migration/accountwithus.png" alt-text="既存のアカウント":::

## <a name="your-company-has-an-account-in-partner-center"></a>パートナー センターに会社のアカウントがある

既存のアカウントが表示され、会社の詳細 (現在サインインしているアカウント) が、このアカウントに統合されることが通知されます。

:::image type="content" source="images/migration/existingaccount2.png" alt-text="パートナー センターのアカウント":::

この画面には、パートナー センターで既に作成されている既存のアカウントの詳細 (名前と住所) と、主要連絡先の詳細が表示されます。

**[続行]** をクリックします。

## <a name="what-happens-during-consolidation-of-accounts"></a>アカウント統合の際の動作

- この画面では詳細を変更できません。

- PMC の (移動中の) アカウントは、この既存のアカウントに統合されます

- PMC の HQ とすべての場所が、この既存のパートナー センター アカウントに場所として移動されます

- 統合が完了すると、既存のパートナー センター アカウントにすべてのアカウントの詳細が場所として表示されます

- この統合中、すべての MPN ID が保持されます

- 既存のコンピテンシー (Gold/シルバー)、購入 (MAPS/Gold/シルバー)、および関連する特典はすべて、統合中に保持されます。

- 会社のメール ID を使用してログインしたユーザーは、必要に応じてアカウントを管理できるように、MPN 管理者およびアカウント管理者として既存のパートナー センター アカウントに自動的に追加されます

## <a name="review-your-company-information"></a>会社情報を確認する

会社に関する情報を確認し、必要に応じて編集します。  これらの詳細情報は、お客様のアカウントをパートナー センターに移行するときに使用されるため、詳細が正しいことを確認してください。

詳細は PMC の情報に基づいており、会社が正当であることを確認するために検証されます。


:::image type="content" source="images/migration/review.png" alt-text="詳細の確認":::

移動するアカウントが、既存のアカウントと同じ国または地域にある場合は、その住所を使用するか、別の住所を追加するかを決めることができます。 別の住所を使用する場合は、その住所が検証されます。 同じ住所を使用する場合は、既存の住所と主要連絡先が使用されます。

この画面の情報を確認/編集し、[送信] をクリックすると、アカウントが統合されます。

## <a name="partner-profile"></a>パートナー プロファイル

プロファイルを表示すると、法的ビジネス (PMC では本社) の情報とその他のすべての場所に関する情報が表示されます。

## <a name="next-steps"></a>次のステップ

- [PMC からパートナー センターへの移行](move-pmc-pc-map.md)
- [ユーザー アカウントの作成](create-user-accounts-and-set-permissions.md)
- [ユーザー ロールとアクセス許可を割り当てる](permissions-overview.md)
- [メンバーシップ プログラムを管理する](renew-mpn-offers.md)
- [会社のビジネス プロファイルを作成する](create-a-marketing-profile.md)
- [紹介機能で顧客との関係を構築する](manage-leads.md)
