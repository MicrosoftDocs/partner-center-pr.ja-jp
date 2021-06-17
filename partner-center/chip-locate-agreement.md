---
title: デスクトップの数と料金レベルを確認する
ms.topic: how-to
ms.date: 02/18/2021
description: Channel Incentives プラットフォーム (CHIP) を使用して、契約のデスクトップ数と料金レベルの情報を見つける方法について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 288e4ebb224d3ff1b0d4050691b733e678ec29a3
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276942"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>任意の契約のデスクトップ数と料金レベルを検索する

**適切なロール**: 主要連絡先またはプログラム管理者

アカウントに [ログインして](https://www.explore.ms/) 、explore.ms 確認したり、デスクトップの数と料金レベルの契約の詳細を提供するファイルをダウンロードしたりできます。

## <a name="to-locate-the-information"></a>情報を見つけるには

### <a name="method-1--explorems"></a>方法 1 – Explore.ms

1. [[explore.ms]](https://www.explore.ms/)を開Internet Explorer。 

>[!Note]
>この関数は、Google Chrome または Microsoft Edge で実行することはできません。

2. 自分のワーク/学校アカウントまたはライブ ID でログインします。  

3. [レポート] **フィールドで** 、[契約] **を選択します**。

4. 結果のページで、[検索] フィールドに契約番号を **入力** し、[列の選択/順序] **を選択します**。

5. ポップアップ ウィンドウで、使用可能な列の一覧から **[Agreement Desktop Count]** を選択し、右矢印を選択して列を追加します。 **[OK]** を選択します。

6. [検索 **] を選択します。**

7. 結果の画面で、結果をスクロールして [Agreement Desktop Count]/(アグリーメント デスクトップ数 **)列を探** します。 

8. デスクトップ数を使用して、以下の料金表に基づいて料金レベルを決定します。  

| 料金レベル | デスクトップ数 |
| ------ | :-----------: |
|  A | 0 – 2,399    |
|  B | 2,400 – 5,999    |
|  C | 6,000 – 14,999    |
|  D | 15,000+   |

>[!NOTE]
>エンタープライズ インセンティブ レベルは、商用および公的機関 (PS) の登録におけるデスクトップまたはユーザー数 (高い方) に基づいて行います。 自然な関連付けられたデスクトップまたはユーザー数がない登録の場合、Microsoft は、付随する EA のデスクトップ数またはユーザー数に基づいてデスクトップ数を適用します。 <br><br>付随する EA がない場合、料金レベルは登録の価格レベルに基づいて行います。 取引の価格レベルは、 で表示[www.explore.ms。](https://www.explore.ms/) <br><br>既存の EA/EAS に複数のプールまたは価格レベルがある場合、Microsoft は割り当てられた最高の価格/プール レベルでインセンティブを支払います。レベル A は最も低く、レベル D は最高です。

#### <a name="pool-and-pricing-levels"></a>プールと価格レベル

上記の手順を使用して explore.ms 契約番号を検索した後、契約番号を選択します。 これにより、契約の詳細ページが表示され、[契約の概要] と [オファリング]**が****表示されます**。 [オファリング] セクションには、価格レベルが含まれている。

## <a name="method-2---chip"></a>方法 2 - CHIP

1. CHIP にサインインし、[LSP インセンティブ] を選択します。

2. [**パートナー支払いの概要**] ページで、表示するレポート月を選択し、[Excelにエクスポート] の下のドロップダウンから [計算の詳細]**を選択します**。

:::image type="content" source="images/chip/chiplocate.png" alt-text="プログラムの詳細を見つける。":::

3. エクスポートが開始され、ファイルを開く、または保存先として保存/保存することができます。

4. レポートが開いているときに、左下にある **[DetailReport-FlatFile]** タブに移動します。

:::image type="content" source="images/chip/flatfile.png" alt-text="フラット ファイルのダウンロード。":::

これで、J 列で探している契約番号を検索できます。割り当てられたデスクトップ数は、R 列に表示され、[Agreement_DesktopCount] というラベルが付Agreement_DesktopCount。 [レベル] というラベルが付いた列 'AI' で、この契約の料金レベルを確認できます。

## <a name="next-steps"></a>次のステップ

- [CHIP アクセスに関する問題のトラブルシューティング](chip-access-trouble.md)
