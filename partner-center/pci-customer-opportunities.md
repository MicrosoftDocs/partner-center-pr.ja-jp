---
title: パートナー センター Insights - CloudAscent の傾向レポート
description: CloudAscent の傾向レポートについては、パートナー センター。 Microsoft 製品を購入する顧客の傾向に関する情報が含まれます。
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 430aea81964d1b75514b6e1377bd2ba1af41b538
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110153040"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>CloudAscent の傾向レポートは、ダッシュボードからパートナー センターできます

**適切なロール**: エグゼクティブ レポート ビューアー |レポート ビューアー

[パートナー センターダッシュボードには、CloudAscent プログラムからダウンロード可能な傾向データが表示されます。 このデータは、顧客が Microsoft 製品を購入する可能性を示しています。  この記事では、このデータの内訳、スコアリングの使い方、および意味について説明します。

## <a name="summary-definitions"></a>概要の定義

- **SMC のお** 客様 – これは、傾向のダウンロードに含まれる顧客の総数です。  顧客はレコードのパートナーによって識別されます。
- **契約の期限切** れ – 現在の会計年度内に、期限切れの契約の数を提供しています。
- **Open Expiring Revenue**– オープン期限切れの契約に関連付けられている収益。

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Customers Opportunities Summary ダッシュボードのスクリーンショット。":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB のセグメント化

中小企業 (SMB) セグメントは、3 つの異なるサブセグメントに分割されます。

1. **管理されていない上位には** 、Microsoft にとって最も多くの機会を持つ最大の SMB 顧客が含まれています。 一般的なトップ アンマネージドのお客様は、マネージド アカウントと同様の特性を共有しています。従業員の数が多く、IT の予算と支出が多く、Microsoft の収益が多い可能性があります。

   Top Unmanaged は、次の 2 つの方法で定義します。

   - **上位のアンマネージド ユーザー ベース**– 300 人以上の従業員を持つアカウントが含まれます。 User-Based アカウントは、初回購入の場合は優れたターゲット、Microsoft 365、Dynamics 365、Surface などのユーザーベースのサブスクリプション製品を展開する場合に適しています。
   - 管理されていない **計算ベースの上位**– Azure が $ 10k を超える可能性のあるアカウントを含みます。 コンピューティングベースのアカウントには、既存の Azure が含まれます。 将来、Azure をまだ購入していても、Azure では $ 10k を超える可能性のある azure をまだ購入していない、未来の年の可能性があるアカウントとアカウント。

2. **中規模ビジネス** には、既存の顧客と、25 ~ 300 人の従業員を持つ見込み客アカウントが含まれます。

3. **スモールビジネス** には、10-25 人の従業員を抱える企業が含まれています。

4. **非常に小規模なビジネス** には、従業員が1-9 の企業が含まれています。

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="SMC によるお客様の種類。":::

**上位の管理対象外** および **中規模のビジネス** subsegments は、microsoft および microsoft パートナー向けの高ライフタイム値 (ltv) のお客様を表します。 このため、it 部門は、このセグメントの成長に焦点を当てています。 この2つの subsegments では、D365/Azure 基幹業務 (LOB) アプリを使用して、さらに収益化で Microsoft 365 ソケットを取得し、Microsoft 向けの高機能を実現することをお勧めします。

現在、2つの主要な領域があります。 1. お客様は成長を促進します。3. Microsoft 365 を使用してクラウドソケットを取得していますが、Dynamics 365 と Azure には大きなチャンスがあります。

次のスクリーンショットは、4つの SMB Subsegments を表しています。 CloudAscent は、すべての管理対象外および中規模のビジネスアカウントのプロファイル、スコアリング、およびモデリングに優先順位を付けます。

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="SMB subsegments のスクリーンショット。":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB では、機械学習テクノロジを使用して、上位のアンマネージおよび中規模のビジネスセグメント内の売上およびマーケティング顧客の予測を促進します。 シグナルはどのように収集され、傾向推奨事項に分類されますか。

- **データ収集**: Web クローラーは、会社のドメインに ping を実行し、ブログの投稿、ニュース リリース、ソーシャル ストリーム、技術フォーラムを監視することで、数十億の顧客シグナルをスキャンして収集します。  収集されたシグナルに加えて、企業情報は、D&B、Microsoft 内部サブスクリプション、トランザクション データなどの内部ソースと外部ソースの両方から収集されます。

- **Machine Learning:** シグナルは機械学習モデルに送り込まれており、クラウド製品とクラスターによって顧客ごとに売上とマーケティングの予測の構造化されたデータ セットが出力されます。  各顧客は、顧客の適合を決定する Microsoft の上位 SMB に似たモデルを使用してスコア付けされ、顧客のオンライン動作を統合する機械学習アルゴリズムは意図として定義されます。 スコアリングは、Microsoft Cloud Products を購入する顧客の傾向を示すクラスターにマージされます。

- **最適化**: Machine Learningトランザクション データとサブスクリプション データを四半期ごとに使用することで、モデルを最適化します。  Machine Learning は、win/loss データを使用してアルゴリズムを調整し、クラスターの推奨事項と MSX で動作する機会を比較することで、モデルが期待通り動作している検証を行います。

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="SMB 機械学習のスクリーンショット。":::

## <a name="cloudascent-propensity"></a>CloudAscent の傾向

傾向に関する推奨事項の作成方法

Web クローラーを介して収集された信号とさまざまなソースから提供されるデータを使用して、企業データと顧客のソーシャル メディアシグナルを統合します。  スコアリングでは、インテントの適合モデルとスコア付けモデルに対して、これらのシグナルとデータが比較モデルで使用されます。

1. 顧客アカウントの適合

   - 企業図を定義する内部データ ポイントと外部データ ポイント。

   - 適合スコアリングでは、Microsoft の最適な SMB に似たモデルを使用して、顧客を比較し、Microsoft Cloud Products に適合する可能性がある場合を確認します。

   - Fit スコアリングが四半期ごとに更新される

2. 顧客アカウントの意図

   - ソーシャル メディアと顧客のオンライン動作に関連するシグナルは、意図を定義します。

   - インテントのスコアリングは、クラスターを定義するために、適合の一番上に重なっています。

   - インテントスコアリングは毎月更新されます。

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB 予測モデル。":::

3. クラスタリング

   適合とインテントのための信号は、クラスタリングスコアに統合されます。 CloudAscent には、次の4つのクラスターがあります。

      - Now-販売準備ができているお客様
      - 評価-マーケティングの準備ができている顧客
      - 育成-ドライブ認識キャンペーン
      - 教育-目的を教育および監視する

   クラスターを使用すると、製品、geo、業界、および垂直などのセグメント要因に基づいて、顧客が販売およびマーケティングのイニシアチブをターゲットにすることができます。

   CloudAscent ブックの [ **傾向 model** ] タブには、傾向と推定の空白の収益が共有されています。 適合とインテントのクラスタリングを定義するには、次の手順を実行します。

      1. ML モデルを使用して、最初に100のスケールでカスタマーフィットスコアとインテントスコアを計算します。  正確なスコアは、ML モデルによって異なります。  次のスコアの例:

         |**分類**|**スコア**|
         |---------|:---------|
         |高|75 ~ 100|
         |Medium|55 ~ 74|
         |低|30 - 54|
         |非常に低い|0 - 29|

      2. 上記のルールを使用して、Customer Fit シグナルと Intent Signals の両方で、企業を High、Medium、Low、Very Low に分類します。

      3. 顧客の適合と意図のシグナルを 2D マトリックスにプロットし、各交差部分が傾向を表します。 たとえば、最も高い傾向を表す高適合 + 高意図 = A1 です。

      4. 最後に、これらのセグメントはクラスターを形成するためにグループ化されます。  たとえば、A1、A2、A3、A4 は Act Now クラスターを形成します。

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent モデル。":::

   これらのお客様には、Act Now と Evaluate customers をターゲットにすることをお勧めします。

## <a name="cloudascent-products--models"></a>CloudAscent Products & モデル

次の図は、CloudAscent 内の各傾向モデルのビューを示しています。

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent 傾向モデル。":::

空白モデルは、製品を持っなかったり、新規の見込み客である既存の Microsoft 顧客の予測で構成されています。

アップセル モデルでは、トランザクション データを使用して、Azure でのアップセルの可能性を予測し、SKU Microsoft 365します。

これらの顧客は既に Azure と Microsoft 365 の両方を持っています。アップセル モデルでは、既存の SKU の購入が多い可能性が高いという結果が示されます。

EOS は、Win 7、Office 2010、SQL Server、Windows Server のサービス終了 (EOS) のお客様を共有します。 EOS データは MS Sales からプルされ、使用可能な場合は CloudAscent 傾向モデリングでオーバーレイされます。 EOS データは Modern Work に保存され、Azure Sales が再生されます。
