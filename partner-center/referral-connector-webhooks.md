---
title: Webhook を使用してリソース変更イベントを取得する
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターの Webhook Api を使用して、Dynamics 365 CRM または Salesforce CRM で参照のリソースがどのように変更されるかを学習します。
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: 紹介、webhook api、リソース変更イベント
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 89628fd6ccab6a943d8bd816afa7b5d3b0f241f7
ms.sourcegitcommit: 0154eabccdc92d1fbe73734f5514f317b9e9fee0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/12/2020
ms.locfileid: "84749172"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events-for-dynamics-365-crm-and-salesforce-crm"></a>Webhook Api を使用して Dynamics 365 CRM と Salesforce CRM のリソース変更イベントに登録する

### <a name="appropriate-roles"></a>適切なロール

- 紹介管理者
- Dynamics 365 CRM または Salesforce CRM のシステム管理者またはシステムカスタマイザー

パートナーセンターの Webhook Api を使用すると、リソース変更イベントに登録できます。 これらの変更イベントは、HTTP 投稿として url に送信されます。

>[!NOTE]
>このトピックでは、Dynamics 365 CRM と Salesforce CRM の両方の Webhook Api について説明します。

## <a name="configure-the-webhook"></a>webhook を構成する

1. Url を登録するには、**パートナーセンターの Webhook 登録 (Insider Preview)** パワー自動化フローを選択します。

2. 接続の追加 (a.)参照管理者の資格情報を持つパートナーセンターのユーザー (b)次の強調表示されているパートナーセンターのイベント

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="トリガー":::

3. これらの更新を行うと、次のように表示されます。

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. 変更内容を保存し、[**有効にする**] を選択します。

   パートナーセンターの webhook がパートナーセンターと CRM システムの IP 共同販売/独立した参照オブジェクトでイベントの変更をリッスンできるようにするには、次の手順を実行します。

5. [**パートナーセンター] を選択して Dynamics 365 (Insider preview)** または**パートナーセンターから Salesforce へ (insider preview)** を選択します。

6. [**編集**] アイコンを選択し、[ **HTTP 要求の受信時**] を選択します。

7. **コピー**アイコンを選択して、指定された HTTP POST URL をコピーします。

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="URL のコピー":::

8. 次に、"パートナーセンターの Webhook の登録 (Insider Preview)" パワー自動化フローを選択し、[**実行**] を選択します。

9. 右側のウィンドウで [実行フロー] ウィンドウが開いていることを確認し、[**続行**] をクリックします。

10. 次の詳細を入力します。

    1. **Http トリガーエンドポイント**: 前の手順からコピーされた URL

    2. **登録するイベント**: "紹介-作成" と "参照-更新"

    3. **既存のトリガーエンドポイントがある場合は上書き**します (存在する場合は既存のエンドポイントを上書きします)。

    Webhook は、変更 (イベントの作成と更新) をリッスンできるようになりました。

11. [**実行**] を選択し、[完了] を選択し**ます。**

## <a name="customize-synchronization-steps"></a>同期手順のカスタマイズ

パートナーセンターと CRM システムの間で共同販売参照が同期されると、パートナーセンター PC で同期されるフィールドがここに表示されます。

多くの場合、CRM システムは高度にカスタマイズされています。 パワー自動化フローをカスタマイズできます。 フィールドマッピングガイドに従って、必要に応じて、パワー自動化フローの手順に適切な変更を加えます。  Microsoft パートナーセンターから CRM へのマッピングが提供されますが、CRM 環境に基づいて、フィールドをさらにカスタマイズすることもできます。

各パワー自動化フローの複数の手順は、ニーズに応じてカスタマイズできます。 使用可能なカスタマイズの例を次に示します。

1. パートナーセンターで作成または更新イベントのフィールドを CRM の参照同期にカスタマイズするには、次のようにします。

   1. [パートナーセンター] を選択して Dynamics 365 (Insider Preview) またはパートナーセンターから Salesforce へ (Insider Preview) を選択します。

   2. [**編集**] を選択して、パワー自動化フローを編集またはカスタマイズします。

   3. 選択 **(スコープ) 潜在顧客または営業案件を同期**します。

2. イベントの作成用に (フィールドマッピングガイドに基づいて) CRM フィールドマッピングをカスタマイズするには、[**新しい共有の営業案件]、[] の順**に選択します。 [サブステップ**if]** を選択し、 **CRM で [新しい営業案件の作成**] を展開します。 このセクションでマッピングを編集するには、[フィールドマッピングガイド] を使用します。

   1. 更新イベントの CRM フィールドマッピングをカスタマイズする (フィールドマップガイドに基づく) 場合は、"(スコープ) 潜在顧客または営業案件の同期" ステップをクリックします。

   2. **営業案件の更新である場合は、** を選択します。 [サブステップ**if yes]** を選択し、次に**パートナーセンターと CRM の営業案件オブジェクト間の差異がある場合**は、を展開します。  

   3. **既存の営業案件を更新**する場合は、[**はい]** を選択します。

3. 更新イベントの CRM から PC への参照同期のフィールドをカスタマイズするには、次のようにします。

   1. [**編集**] を選択して、パワー自動化フローを編集またはカスタマイズします。

   2. [ **(スコープ)] を選択して、営業案件を同期**します。

   3. 更新イベントの CRM フィールドマッピング (フィールドマッピングガイドに基づく) をカスタマイズする場合は、**パートナーセンターと CRM の潜在顧客オブジェクトが異なるかどうか**を選択してから、を選択します。

   4. [サブステップ**if yes]** を選択し、[**営業案件データを使用して紹介を更新する**] ステップを展開します。

   このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。

4. Create events の CRM to PC 参照同期のフィールドをカスタマイズするには

   1. [**編集**] を選択して、パワー自動化フローを編集またはカスタマイズします。

   2. **参照の同期を選択 (スコープ) します。**

   3. [イベントの作成] で (フィールドマッピングガイドに基づいて) CRM フィールドマッピングをカスタマイズする場合は、[ **Microsoft の紹介を作成する**] を選択します。

このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>エンドツーエンドの双方向の共同販売参照の同期

パワー自動化ソリューションのインストール、構成、およびカスタマイズが完了したら、Dynamics 365 または Salesforce とパートナーセンター間の共同販売参照の同期をテストできます。

### <a name="pre-requisites"></a>前提条件

パートナーセンターと Dynamics 365 CRM 間、またはパートナーセンターと Salesforce CRM 間で紹介を同期するには、Power 区別のソリューションで、Microsoft 固有の紹介フィールドを明確にする必要があります。 これにより、販売者チームは、共同販売のために Microsoft と共有する参照を決定することができます。

Dynamics 365 ソリューションの**営業案件**エンティティのパートナーセンターの紹介同期の一部として、一連のカスタムフィールドを使用できます。 CRM 管理者ユーザーは、**営業案件**のカスタムフィールドを使用して、別の crm セクションを作成する必要があります。

次のカスタムフィールドは、CRM セクションの一部にする必要があります。

- **パートナーセンターとの同期**: 営業案件を Microsoft パートナーセンターと同期するかどうか

- **参照識別子**: Microsoft パートナーセンターの紹介の読み取り専用識別子フィールド

- **紹介リンク**: Microsoft パートナーセンターでの紹介への読み取り専用リンク

- Microsoft の**ヘルプ**を参照してください。

- **製品**: この営業案件に関連付けられている製品の一覧

- **監査**: パートナーセンターの紹介と同期するための読み取り専用の監査証跡

### <a name="scenarios"></a>モデル

1. CRM で参照が作成または更新され、パートナーセンターで同期される場合の参照の同期:

   1. CRM の**営業案件**セクションで可視性を持つユーザーを使用して、DYNAMICS 365 CRM 環境にサインインします。

   2. Dynamics 365 環境で "新しい営業案件" を作成するときに、次のセクションが存在することを確認します。

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="営業案件":::

   3. この機会を Microsoft パートナーセンターと同期するには、カードビューで次のフィールドを設定していることを確認します。

      - **パートナーセンターとの同期**: はい

      - **Microsoft のヘルプを使用する方法**: 次から選択してください。

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="ヘルプの選択":::

      - **製品**: 製品のソリューション id

   4. 営業案件が Dynamics 365 で作成され、[**パートナーセンターとの同期**] オプションを **[はい]** に設定した場合は、10分間待機して、パートナーセンターアカウントにサインインします。 参照は Dynamics 365 と同期されます。

   5. そのため、[パートナーセンターとの同期] オプションを [はい] に設定した場合、Dynamics 365 CRM で営業案件を更新すると、パートナーセンターアカウントで変更が同期されます。

   6. パートナーセンターで正常に同期された営業案件は、Dynamics 365 の✔アイコンで識別されます。

2. Microsoft パートナーセンターで参照が作成または更新され、Dynamics 365 環境で同期される場合の参照同期:

   1. パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。

   2. 左側のメニューから [**紹介**] を選択します。

   3. [新しい取引] オプションをクリックして、パートナーセンターから新しい共同販売紹介を作成します。

   4. Dynamics 365 CRM 環境にサインインします。

   5. **[Open opportunity**] に移動します。 Microsoft パートナーセンターで作成された紹介が Dynamics 365 CRM で同期されるようになりました。

   6. 同期された参照を選択すると、カードビューの詳細が設定されます。

## <a name="next-steps"></a>次の手順

- [Microsoft Power の自動化プラットフォームの詳細](https://docs.microsoft.com/power-automate/)

- [パートナーセンターの webhook イベント](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [見込み客を管理する](manage-leads.md)

- [共同販売の機会を管理する](manage-co-sell-opportunities.md)
