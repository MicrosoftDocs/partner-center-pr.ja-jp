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
ms.openlocfilehash: 64dbbbae0087275fa8d0c5fd4f364079623efe63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148994"
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
|  D | 15000 +   |

>[!NOTE]
>エンタープライズインセンティブレベルは、商用および公的セクタ (PS) 登録のデスクトップまたはユーザー数 (どちらか大きい方) に基づいています。 自然に関連付けられたデスクトップまたはユーザー数を含まない登録の場合、Microsoft では、付随する EA のデスクトップ数またはユーザー数に基づいてデスクトップ数を適用します。 <br><br>付随する EA がない場合、料金レベルは登録の価格レベルに基づきます。 取引の価格レベルは、 [www.explore.ms](https://www.explore.ms/)でも確認できます。 <br><br>既存の EA/EAS に複数のプールや価格レベルがある場合、Microsoft は、割り当てられた最高レベルの価格/プールレベルでインセンティブを支払います。レベル A は最下位で、レベル D は最も高くなります。

#### <a name="pool-and-pricing-levels"></a>プールと価格レベル

上記の手順に従って explore.ms で契約番号を検索した後、契約番号を選択します。 契約の詳細ページが表示され、 **契約の概要** と **オファリング** が表示されます。 オファリングセクションには、価格レベルが含まれています。

## <a name="method-2---chip"></a>方法 2-チップ

1. チップにサインインし、[LSP インセンティブ] を選択します。

2. [**パートナーの支払いの概要**] ページで、表示するレポート月を選択し、[ **Excel にエクスポート**] の下のドロップダウンリストから [**計算の詳細**] を選択します。

:::image type="content" source="images/chip/chiplocate.png" alt-text="プログラムの詳細の検索":::

3. エクスポートが開始され、ファイルを開くか、保存して保存することができます。

4. レポートが開いたら、左下にある [ **FlatFile** ] タブに移動します。

:::image type="content" source="images/chip/flatfile.png" alt-text="フラットファイルのダウンロード":::

これで、列 J で探している契約番号を検索できるようになりました。割り当てられたデスクトップ数は、[Agreement_DesktopCount] というラベルの付いた R 列にあります。 このアグリーメントの料金レベルは、[レベル] というラベルの付いた列 ' AI ' で確認することもできます。

## <a name="next-steps"></a>次のステップ

- [チップアクセスの問題のトラブルシューティング](chip-access-trouble.md)
